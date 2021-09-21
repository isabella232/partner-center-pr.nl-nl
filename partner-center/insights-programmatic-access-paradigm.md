---
title: Programmatisch toegangsparadigma voor inzichtgegevens
description: Informatie over de stroom op hoog niveau van het API-aanroeppatroon voor programmatische analyses. De API's voor toegang tot analyserapporten van partnerinzichten worden ook behandeld.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 304607b5d79b0ad8a07c3efe690ccb7feef83331
ms.sourcegitcommit: ab5eda007f87f22fa3375b8e05adfccd6ebc285e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/21/2021
ms.locfileid: "128058940"
---
# <a name="programmatic-access-paradigm"></a>Programmatisch toegangsparadigma

In dit diagram ziet u het API-aanroeppatroon dat wordt gebruikt om een nieuwe rapportsjabloon te maken, het aangepaste rapport te plannen en foutgegevens op te halen.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Stroom op hoog niveau":::
***Afbeelding 1: Stroom op hoog niveau van het API-aanroeppatroon***

Deze lijst bevat meer informatie over afbeelding 1.

1. De clienttoepassing kan het aangepaste rapportschema/de aangepaste sjabloon definiëren door de [API rapportquery maken aan te roepen.](#create-report-query-api) U kunt ook een rapportsjabloon (QueryId) kiezen uit de voorbeelden van de rapportsjabloonbibliotheek in Lijst met systeemquery's voor programmatische toegang tot [partnerinzichten.](insights-programmatic-system-queries.md)
2. Als dit is gelukt, retourneert de API Rapportquery maken de QueryId.
3. De clienttoepassing moet vervolgens [](#create-report-api) de API Rapport maken aanroepen met behulp van de QueryId, samen met de begindatum van het rapport, het herhalingsinterval, het terugkeerpatroon en een optionele callback-URI.
4. Bij geslaagd retourneert [de API Rapport maken](#create-report-api) de ReportId.
5. De clienttoepassing krijgt een melding via de callback-URL zodra de rapportgegevens gereed zijn om te worden gedownload.
6. De clienttoepassing gebruikt vervolgens de GET [Report Executions-API om](#get-report-execution-api) de status van het rapport op te vragen met de rapport-id en het datumbereik.
7. Als het downloaden van het rapport is geslaagd, wordt de koppeling geretourneerd en kan de toepassing het downloaden van de gegevens starten.

## <a name="report-query-language-specification"></a>Specificatie van rapportquerytaal

Hoewel we [systeemquery's bieden die](insights-programmatic-system-queries.md) u kunt gebruiken om rapporten te maken, kunt u ook uw eigen query's maken op basis van uw bedrijfsbehoeften. Zie Aangepaste queryspecificatie voor meer informatie [over aangepaste query's.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>Rapportquery-API maken

De API helpt bij het maken van aangepaste query's die de gegevensset definiëren van waaruit kolommen en metrische gegevens moeten worden geëxporteerd. De API biedt de flexibiliteit om een nieuwe rapportagesjabloon te maken op basis van de behoeften van uw bedrijf.  

U kunt ook de [systeemquery's gebruiken die](insights-programmatic-system-queries.md) we bieden. Wanneer aangepaste rapportsjablonen niet nodig zijn, kunt u [Rapport-API](#create-report-api) maken rechtstreeks aanroepen met behulp van de QueryId's van de systeemquery's die worden geleverd.  

In het volgende voorbeeld ziet u hoe u een aangepaste query maakt om de top 10 klanten op te halen op omzet voor de afgelopen maand.

### <a name="request-syntax"></a>Aanvraagsyntaxis

|    Methode     |    Aanvraag-URI     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Aanvraagheader

|    Header     |    Type     |    Description     |
|-------|-----|------|
|    Autorisatie     |    tekenreeks |Vereist. Het Azure Active Directory -toegang token (Azure AD). De indeling is  `Bearer <token>` .|
|    Content-Type     |tekenreeks |`Application/JSON` |
||||

### <a name="path-parameter"></a>Padparameter

Geen

### <a name="query-parameter"></a>Queryparameter

Geen

### <a name="sample-request-payload"></a>Voorbeeld van nettolading van aanvraag

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Woordenlijst

Deze tabel bevat de belangrijkste definities van elementen in de nettolading van de aanvraag.

|Parameter|    Vereist     |    Beschrijving     |    Toegestane waarden     |
|-----|    -----    |    -----    |    -----    |
|Naam |    Yes     |    Gebruiksvriendelijke naam van de query     |    tekenreeks     |
|    Beschrijving     |    Nee     |    Beschrijving van wat de query retourneert     |    tekenreeks     |
|    Query’s uitvoeren     |    Yes     |    Rapportqueryreeks     |    Gegevenstype: tekenreeks <br> [Aangepaste query op](insights-programmatic-custom-query.md) basis van bedrijfsvraag |
|        |        |        |        |

> [!Note]
> Zie Voorbeelden van voorbeeldquery's [voor voorbeelden van aangepaste query's.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Voorbeeldantwoord

De nettolading van het antwoord is als volgt gestructureerd:

Responscodes: 200, 400, 401, 403, 500

Voorbeeld van nettolading van antwoord:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Woordenlijst

Deze tabel bevat de belangrijkste definities van elementen in de nettolading van de aanvraag.

|    Parameter     |    Beschrijving     |
|    ----    |    ----    |
|    QueryId     |    Universally Unique Identifier (UUID) van de query die u hebt gemaakt     |
|    Naam     |    Gebruiksvriendelijke naam voor de query in de nettolading van de aanvraag     |
|    Description     |    Beschrijving gegeven tijdens het maken van de query     |
|    Query’s uitvoeren     |    Rapportquery doorgegeven als invoer tijdens het maken van de query     |
|    Type     |    Ingesteld op `userDefined`     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om de query te maken     |
|    CreatedTime     |    UTC-tijd dat de query is gemaakt in deze indeling: yyyy-MM-ddTHH:mm:ssZ     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    StatusCode     |    Resultaatcode <br> De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|    message     |    Statusbericht van de uitvoering van de API     |
|        |        |

## <a name="create-report-api"></a>Rapport-API maken

Wanneer u een aangepaste rapportsjabloon maakt [](#create-report-query-api) en de QueryID ontvangt als onderdeel van het antwoord Rapportquery maken, kan deze API worden aangeroepen om een query te plannen die regelmatig moet worden uitgevoerd. U kunt een frequentie en planning instellen om het rapport te leveren.
Voor systeemquery's die we bieden, kan de API rapport maken ook worden aangeroepen met [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>URL voor aanroep

De API voor het maken van een rapport accepteert een callback-URL. Deze URL wordt aangeroepen zodra het genereren van het rapport is geslaagd. De callback-URL moet openbaar bereikbaar zijn. Naast de URL kan ook een callback-methode worden gegeven. De callback-methode kan alleen GET of POST zijn. De standaardmethode als er geen waarde wordt doorgegeven, is POST. De reportId die het genereren heeft voltooid, wordt altijd terugverdiend tijdens de callback.

POST-callback: Als de doorgegeven URL `https://www.contosso.com/callback` is, wordt de teruggeroepen URL `https://www.contosso.com/callback/<reportID>` 

GET-callback: als de doorgegeven URL is, wordt de teruggeroepen `https://www.contosso.com/callback` URL `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>ExecuteNow-rapporten

Er is een inrichting voor het genereren van een rapport zonder planning. In het rapport API-nettolading maken kan een parameter worden geaccepteerd, waarmee het rapport in dequerie wordt opgemaakt zodra `ExecuteNow` de API wordt aangeroepen. Wanneer `ExecuteNow` is ingesteld op true, worden de velden, , genegeerd omdat deze rapporten niet zijn `StartTime` `RecurrenceCount` `RecurrenceInterval` gepland.

Er kunnen twee extra velden worden doorgegeven wanneer `ExecuteNow` waar is, `QueryStartTime` en `QueryEndTime` . Deze twee velden overschrijven het `TIMESPAN` veld in de query. Deze velden zijn niet van toepassing op geplande rapporten, omdat gegevens continu worden gegenereerd gedurende een vaste periode die niet verandert.

### <a name="request-syntax"></a>Aanvraagsyntaxis

|    Methode     |    Aanvraag-URI     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Aanvraagheader

|    Header     |    Type     |    Description     |
|-------|-----|------|
|    Autorisatie     |    tekenreeks |Vereist. Het Azure Active Directory -toegang token (Azure AD). De indeling is  `Bearer <token>` .|
|    Content-Type     |tekenreeks |`Application/JSON` |

### <a name="path-parameter"></a>Padparameter

Geen

### <a name="query-parameter"></a>Queryparameter

Geen

### <a name="sample-request-payload"></a>Voorbeeld van nettolading van aanvraag

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Woordenlijst

De belangrijkste definities van elementen in de nettolading van de aanvraag worden hieronder verwoord:

|    Parameter     |    Vereist     |    Beschrijving     |    Toegestane waarden     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Naam die moet worden toegewezen aan het rapport     |    tekenreeks     |
|    Beschrijving     |    Nee     |    Beschrijving van het gemaakte rapport     |    tekenreeks     |
|    QueryId     |    Yes     |    Rapportquery-id     |    tekenreeks     |
|    StartTime     |    Yes     |    UTC-tijdstempel waarop het genereren van het rapport begint. <br> De indeling moet zijn: yyyy-MM-ddTHH:mm:ssZ       |    tekenreeks     |
|    ExecuteNow     |    No     |    Deze parameter moet worden gebruikt om een rapport te maken dat slechts één keer wordt uitgevoerd. `StartTime`, `RecurrenceInterval` en worden genegeerd als deze is ingesteld op `RecurrenceCount` true. Het rapport wordt onmiddellijk op een asynchrone manier uitgevoerd     |    waar/onwaar     |
|    QueryStartTime     |    No     |    Hiermee geeft u eventueel de begintijd op voor de query die de gegevens extraheert. Deze parameter is alleen van toepassing voor een een time-execution reports die `ExecuteNow` zijn ingesteld op true. Als u deze parameter instelt, `TIMESPAN` worden de opgegeven in de query overschrijven. De indeling moet yyyy-MM-ddTHH:mm:ssZ zijn     |    Tijdstempel als tekenreeks     |
|    QueryEndTime     |    No     |    Hiermee geeft u eventueel de eindtijd op voor de query die de gegevens extraheert. Deze parameter is alleen van toepassing voor één keer uitvoeringsrapport dat `ExecuteNow` is ingesteld op true. Als u deze parameter instelt, `TIMESPAN` worden de opgegeven in de query overschrijven. De indeling moet yyyy-MM-ddTHH:mm:ssZ zijn     |    Tijdstempel als tekenreeks     |
|    RecurrenceInterval     |    Yes     |    Frequentie in uren waarop het rapport moet worden gegenereerd. <br> Minimumwaarde is 4 en Maximumwaarde is 2160.      |    geheel getal     |
|    RecurrenceCount     |    No     |    Het aantal rapporten dat moet worden gegenereerd.     |    geheel getal     |
|    Indeling     |    No     |    Bestandsindeling van het geëxporteerde bestand. <br> De standaardwaarde is CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    Openbaar bereikbare URL die optioneel kan worden geconfigureerd als callback-bestemming     |    Tekenreeks (HTTP-URL)     |
|    CallbackMethod     |    No     |    De methode die moet worden gebruikt voor callback     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Voorbeeldantwoord

De nettolading van het antwoord is als volgt gestructureerd:

Antwoordcodes: 200, 400, 401, 403, 404, 500

Voorbeeld van nettolading van antwoord:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Woordenlijst

De belangrijkste definities van elementen in het antwoord worden hieronder verwoord:

|    Parameter     |    Beschrijving     |
|    ----    |    ----    |
|    ReportId     |    Universally Unique Identifier (UUID) van het rapport dat u hebt gemaakt     |
|    ReportName     |    Naam van het rapport in de nettolading van de aanvraag     |
|    Description     |    Beschrijving gegeven tijdens het maken van het rapport     |
|    QueryId     |    Query-id doorgegeven op het moment dat u het rapport hebt gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    UTC-tijd dat het rapport is gemaakt in deze indeling: yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    UTC Tijd dat het rapport voor het laatst is gewijzigd in deze indeling: yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    `ExecuteNow` de vlag die is ingesteld op het moment dat het rapport is gemaakt     |
|    StartTime     |    UTC-tijd dat de uitvoering van het rapport in deze indeling begint: yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status van de uitvoering van het rapport. De mogelijke waarden zijn `Paused` , `Active` en `Inactive`     |
|    RecurrenceInterval     |    Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport     |
|    RecurrenceCount     |    Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport.      |
|    CallbackUrl     |    Callback-URL die is opgegeven in de aanvraag     |
|    CallbackMethod     |    Callback-methode die is opgegeven in de aanvraag     |
|    Indeling     |    Indeling van de rapportbestanden. De mogelijke waarden zijn `CSV` of `TSV` .     |
|    Totaal aantal     |    Aantal records in de matrix Waarde     |
|    StatusCode     |    Resultaatcode     |
|    message     |    De mogelijke waarden zijn 200, 400, 401, 403, 500. Statusbericht van de uitvoering van de API     |
|        |        |

## <a name="get-report-execution-api"></a>API voor rapportuitvoeringen krijgen

U kunt deze methode gebruiken om een query uit te voeren op de status van een rapportuitvoering met behulp van de ReportId die u hebt ontvangen [van De rapport-API maken.](#create-report-api) De methode retourneert de downloadkoppeling voor het rapport als het rapport gereed is om te worden gedownload. Anders retourneert de methode de status. U kunt deze API ook gebruiken om alle uitvoeringen op te halen die voor een bepaald rapport zijn uitgevoerd.  

>[!IMPORTANT]
>Voor deze API zijn standaardqueryparameters ingesteld `executionStatus=Completed` voor en `getLatestExecution=true` . Als u de API aanroept voordat het rapport voor de eerste keer wordt uitgevoerd, wordt er dus 404 als 404-code gebruikt. Uitvoeringen in behandeling kunnen worden verkregen door in te `executionStatus=Pending` stellen.

### <a name="request-syntax"></a>Aanvraagsyntaxis

|    Methode     |    Aanvraag-URI     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Aanvraagheader

|    Header     |    Type     |    Description     |
|-------|-----|------|
|    Autorisatie     |    tekenreeks |Vereist. Het Azure Active Directory -toegang token (Azure AD). De indeling is  `Bearer <token>` .|
|    Content-Type     |tekenreeks |`Application/JSON` |

### <a name="path-parameter"></a>Padparameter

|    Parameternaam    |    Vereist    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Yes    |    tekenreeks    |    Filter om alleen uitvoeringsdetails van rapporten op te halen met de reportId die in dit argument is opgegeven. Meerdere reportIds kunnen worden opgegeven door ze te scheiden met een puntkomma ;".    |
|        |        |        |        |

### <a name="query-parameter"></a>Queryparameter

|    Parameternaam    |    Vereist    |    Type    |    Description    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    No    |    tekenreeks    |    Filter om alleen details van rapporten op te halen met de executionId die in dit argument is opgegeven. Meerdere executionIds kunnen worden opgegeven door ze te scheiden met een puntkomma ;".    |
|    executionStatus    |    No    |    Tekenreeks/enum    |    Filter om alleen details op te halen van rapporten met de executionStatus in dit argument. <br> Geldige waarden zijn: `Pending` , `Running` , en `Paused` `Completed` . <br> De standaardwaarde is `Completed`. <br> Meerdere statussen kunnen worden opgegeven door ze te scheiden met een puntkomma ;".    |
|    getLatestExecution    |    No    |    booleaans    |    De API retournt gegevens over de meest recente uitvoering. Deze parameter is standaard ingesteld op true.<br> Als u ervoor kiest om de waarde van deze parameter als onwaar door te geven, retourneert de API de uitvoerings-exemplaren van de afgelopen 90 dagen.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Voorbeeld van nettolading van aanvraag

Geen

### <a name="sample-response"></a>Voorbeeldreactie

De nettolading van het antwoord is als volgt gestructureerd:

Responscodes: 200, 400, 401, 403, 404, 500

Voorbeeld van nettolading van antwoord:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Zodra de uitvoering van het rapport is voltooid, wordt de `Completed` uitvoeringsstatus weergegeven. U kunt het rapport downloaden door de URL in de te `reportAccessSecureLink` selecteren.

### <a name="glossary"></a>Woordenlijst

Sleuteldefinities van elementen in het antwoord.

|    Parameter    |    Beschrijving    |
|    ----    |    ----    |
|    ExecutionId    |    Universally Unique Identifier (UUID) van het uitvoerings exemplaar    |
|    ReportId    |    Rapport-id die is gekoppeld aan het uitvoerings exemplaar    |
|    RecurrenceInterval    |    Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport    |
|    RecurrenceCount    |    Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport    |
|    CallbackUrl    |    Callback-URL die is gekoppeld aan het uitvoeringsin exemplaar    |
|    CallbackMethod    |    Callback-methode die is gekoppeld aan het uitvoeringsin exemplaar    |
|    Indeling    |    Indeling van het gegenereerde bestand aan het einde van de uitvoering    |
|    ExecutionStatus    |    Status van het exemplaar van de uitvoering van het rapport. <br> Geldige waarden zijn: `Pending` , `Running` , `Paused` en `Completed`    |
|    ReportAccessSecureLink    |Koppeling waarmee het rapport veilig kan worden gebruikt        |
|    ReportExpiryTime    |    UTC-tijd waarna de rapportkoppeling verloopt in deze indeling: yyyy-MM-ddTHH:mm:ssZ    |
|    ReportGeneratedTime    |    UTC-tijd waarop het rapport is gegenereerd in deze indeling: yyyy-MM-ddTHH:mm:ssZ    |
|    Totaal aantal    |    Aantal gegevenssets in de matrix Waarde    |
|    StatusCode    |    Resultaatcode <br> De mogelijke waarden zijn 200, 400, 401, 403, 404 en 500    |
|    message    |    Statusbericht van de uitvoering van de API    |
|        |        |

## <a name="next-steps"></a>Volgende stappen

- Probeer de API's uit via de [Swagger API-URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Uw eerste API-aanroep maken] (insights-programmatic-first-api-call.md
