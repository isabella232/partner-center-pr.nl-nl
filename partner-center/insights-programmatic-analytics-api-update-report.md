---
title: Rapport-API bijwerken
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om rapportparameters bij te werken in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 64ef897dc3c883e4adfda4285183e441f27f3c7f
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957436"
---
# <a name="update-report-api"></a>Rapport-API bijwerken

Met deze API kunt u een rapportparameter wijzigen.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory -toegang token (AAD) in het formulier`Bearer <token>`    |
|    Content-Type    |    tekenreeks    |    `Application/JSON`    |
|        |        |        |

**Padparameter**

|    Parameternaam    |    Type    |    Vereist    |    Beschrijving    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    tekenreeks    |    No    |    Id van het rapport dat wordt gewijzigd     |
|        |        |        |        |

**Queryparameter**

Geen

**Nettolading aanvragen**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Woordenlijst**

Deze tabel bevat de belangrijkste definities van elementen in het antwoord.

|    Parameter    |    Vereist    |    Beschrijving    |    Toegestane waarden    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Yes     |    Naam die moet worden toegewezen aan het rapport     |    Tekenreeks     |
|    Beschrijving     |    Nee     |    Beschrijving van het gemaakte rapport     |    Tekenreeks     |
|    StartTime     |    Yes    |    Tijdstempel waarna het genereren van het rapport begint     |    Tekenreeks     |
|    RecurrenceInterval     |    No     |    Frequentie waarmee het rapport in uren moet worden gegenereerd. Minimumwaarde is 4     |    Geheel getal     |
|    RecurrenceCount     |    No     |    Het aantal te genereren rapport. De standaardwaarde is onbeperkt.     |    Geheel getal     |
|    Indeling     |    No    |    Bestandsindeling van het geëxporteerde bestand. De standaardwaarde is CSV     |    CSV/TSV     |
|    CallbackURL     |    No     |    HTTPS-callback-URL die moet worden aangeroepen bij het genereren van een rapport     |    Tekenreeks     |
|    CallbackMethod    |    No    |    Http-methode die moet worden gebruikt voor callback    |    GET/POST    |
|        |        |        |        |


**Response**

De nettolading van het antwoord is als volgt gestructureerd:

Responscode: 200, 400, 401, 403, 404, 500

Voorbeeld van nettolading van antwoord:

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

**Woordenlijst**

Deze tabel definieert de belangrijkste elementen in het antwoord:

|    Parameter    |    Beschrijving    |
|    ----    |    ----    |
|    ReportId     |    Universally Unique Identifier (UUID) van het rapport dat wordt bijgewerkt     |
|    ReportName     |    Naam van het rapport in de nettolading van de aanvraag     |
|    Description     |    Beschrijving van het rapport in de nettolading van de aanvraag     |
|    QueryId     |    Query-id doorgegeven op het moment dat het rapport werd gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    Het tijdstip dat het rapport is gemaakt. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Het tijdstip dat het rapport voor het laatst is gewijzigd. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt    |
|    StartTime     |    Tijd dat de uitvoering van het rapport begint. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status van de uitvoering van het rapport. De mogelijke waarden zijn Onderbroken, Actief en Inactief.     |
|    RecurrenceInterval     |    Terugkeerpatroon opgegeven in de nettolading van de aanvraag     |
|    RecurrenceCount     |    Aantal terugkeerpatroon dat is opgegeven in de nettolading van de aanvraag     |
|    CallbackUrl     |    Callback-URL die is opgegeven in de aanvraag     |
|    CallbackMethod    |    Callback-methode die is opgegeven in de aanvraag    |
|    Indeling     |    Indeling van de rapportbestanden     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |