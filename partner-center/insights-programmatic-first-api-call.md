---
title: Uw eerste API-aanroep maken om toegang te krijgen tot analysegegevens van partnerinzichten
description: Voorbeelden om te leren hoe u de API gebruikt voor toegang tot analysegegevens van partnerinzichten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 9aac83645051f3e8f32945ae908ba1fe47c08d13
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244890"
---
# <a name="make-your-first-api-call-to-access-partner-insights-analytics-data"></a>Uw eerste API-aanroep maken om toegang te krijgen tot analysegegevens van partnerinzichten

Zie API's voor toegang tot analysegegevens van partnerinzichten voor een lijst met de API's voor toegang tot [analysegegevens van partnerinzichten.](insights-programmatic-analytics-available-api.md) Voordat u uw eerste API-aanroep maakt, moet u ervoor zorgen dat u aan de vereisten voor programmatische toegang tot Partner-Insights analytics-gegevens hebt voldaan. [](insights-programmatic-prerequisites.md)

## <a name="token-generation"></a>Token genereren

Voordat u een van de methoden aanroept, moet u eerst een AAD-Azure Active Directory verkrijgen. U moet het Azure AD-toegang token doorgeven aan de autorisatie-header van elke methode in de API. Nadat u een toegangsteken hebt ontvangen, hebt u 60 minuten om het te gebruiken voordat het verloopt. Nadat het token is verlopen, kunt u het token vernieuwen en het blijven gebruiken voor verdere aanroepen naar de API.

Raadpleeg een voorbeeldaanvraag hieronder voor het genereren van een token. De drie waarden die nodig zijn om het token te `clientId` genereren, zijn `clientSecret` , en `tenantId` . De resourceparameter moet worden ingesteld op `https://api.partnercenter.microsoft.com`

#### <a name="request-example"></a>Voorbeeld van aanvraag

```console
curl --location --request POST 'https://login.microsoftonline.com/<tenantId>/oauth2/token' \
--header 'return-client-request-id: true' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Cookie: fpc=Ar2GMei7JwdKg4Y4onHrMpvxqd4FAQAAAEhU_tcOAAAA; stsservicecookie=estsfd; x-ms-gateway-slice=estsfd' \
--data-urlencode 'resource= https://api.partnercenter.microsoft.com' \
--data-urlencode 'client_id= ' \
--data-urlencode 'client_secret= ' \
--data-urlencode 'grant_type=password' \
--data-urlencode 'scope=openid' \
--data-urlencode 'username= ' \
--data-urlencode 'password= '
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
    "token_type": "Bearer",
    "expires_in": "3599",
    "ext_expires_in": "3599",
    "expires_on": "1612794445",
    "not_before": "1612790545",
    "resource": "https://api.partnercenter.microsoft.com",
    "access_token": {Token}
}
```

Zie Toegang tot analysegegevens met Store-services voor meer informatie over het verkrijgen van een Azure AD-token voor [uw toepassing.](/windows/uwp/monetize/access-analytics-data-using-windows-store-services#step-2-obtain-an-azure-ad-access-token)

## <a name="programmatic-api-call"></a>Programmatische API-aanroep

Nadat u het AAD-token hebt ontvangen zoals beschreven in de vorige sectie, volgt u deze stappen om uw eerste programmatisch toegangsrapport te maken.

Gegevens kunnen worden gedownload uit de volgende gegevenssets (datasetName):

- CustomersAndTenants
- SeatsSubscriptionsAndRevenue
- AzureUsage
- MSLearn
- OfficeUsage
- Profiel
- TrainingCompletions
- DynamicsUsage
- CompetencySummaryHistory
- PowerBIUsage
- EMSUsage
- CompetencyPeformanceRequirement
- ResellerPerformance
- CLASAgreementRenewalsPropensity
- CLASAzurePropensity
- CLASD365Propensity
- CLASM365Propensity
- TeamsUsage3PApps
- TeamsUsageWorkload
- TeamsUsageMeetingsAndCalls

In de volgende sectie ziet u voorbeelden van hoe u programmatisch toegang kunt krijgen `SubscriptionId` vanuit de DynamicsUsage-gegevensset.

### <a name="step-1-make-a-rest-call-using-the-get-datasets-api"></a>Stap 1: maak een REST-aanroep met behulp van de API gegevenssets op halen

Het API-antwoord geeft de naam van de gegevensset op van waar u het rapport kunt downloaden. Voor de specifieke gegevensset bevat het API-antwoord ook de lijst met selecteerbare kolommen die kunnen worden gebruikt voor uw aangepaste rapportsjabloon. U kunt ook verwijzen naar de [gegevensdefinities](insights-data-definitions.md) om de namen van de kolommen op te halen.

#### <a name="request-example"></a>Voorbeeld van aanvraag

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset'\
--header 'Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
  "value": [
    {
      "datasetName": "DynamicsUsage",
      "selectableColumns": [
        "PGAMpnId",
        "SubscriptionId",
        "SubscriptionStartDate",
        "SubscriptionEndDate",
        "SubscriptionStatus",
        "Month",
        "RevSumDivisionName",
        "RevSumCategoryName",
        "SKU",
        "SKUId",
        "FreeVsPaidSKU",
        "SalesModel",
        "DetailedSalesModel",
        "CustomerName",
        "CustomerTenantId",
        "CustomerTpid",
        "CustomerSegment",
        "CustomerMarket",
        "MPNId",
        "PartnerName",
        "PartnerLocation",
        "PartnerAttachType",
        "AvailableSeats",
        "AssignedSeats",
        "ActiveSeats",
        "DeploymentOpportunity",
        "ActiveUsagePercent"
      ],
      "availableMetrics": [
        "SubscriptionCount",
        "TotalAssignedSeats",
        "TotalSoldSeats",
        "TotalActiveSeats",
        "TotalRevenueAndACR",
        "CustomerCount",
        "CustomerTenantCount"
      ],
      "availableDateRanges": [
        "LAST_MONTH",
        "LAST_3_MONTHS",
        "LAST_6_MONTHS",
        "LAST_1_YEAR",
        "LIFETIME"
      ],
      "minimumRecurrenceInterval": 24
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Dataset fetched successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-2-create-the-custom-query"></a>Stap 2: de aangepaste query maken

In deze stap gebruiken we SubscriptionId uit de DynamicsUsage-gegevensset om een aangepaste query te maken voor het gepersonaliseerde rapport. De standaardtijdsduur als deze niet is opgegeven in de query is 6 maanden.

#### <a name="request-example"></a>Voorbeeld van aanvraag

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries' \ 
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
{
  "Name": "SubscriptionId Dynamics ",
  "Description": "List of Subscription Id from DynamicsUsage",
  "Query": "SELECT SubscriptionId from DynamicsUsage "
            }"
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
  "value": [
    {
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "name": "SubscriptionId Dynamics",
      "description": "List of Subscription Id from DynamicsUsage",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T07:28:37Z"
    }
 ],
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
}
```

Als de query is uitgevoerd, wordt er `queryId` een gegenereerd die moet worden gebruikt om het rapport te genereren.

### <a name="step-3-execute-test-query-api"></a>Stap 3: testquery-API uitvoeren

In deze stap gebruiken we de testquery-API om de bovenste 100 rijen op te halen voor de query die is gemaakt.

#### <a name="request-example"></a>Voorbeeld van aanvraag

```cli
curl 
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?queryId=7d19305c-56db-4edc-b776-428340e3a9c8' \
--header ' Authorization: Bearer <AADToken>'
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
  "value": [
    {
      "SubscriptionId": "251DE3D4-8868-4032-B518-F142DA50522F"
    },
    {
      "SubscriptionId": "758A0647-790C-435B-BEAA-652DF47E327C"
    },
    {
      "SubscriptionId": "ACE5A84B-9794-4480-82C5-AF9462DE2589"
    },
    {
      "SubscriptionId": "C75163EE-A0CA-4822-8275-E29E2490FF1C"
    },
    {
      "SubscriptionId": "082A8A18-0834-4376-A9A4-3AA4ECD02826"
    },
    .
    .
    .
    {
      "SubscriptionId": "5E10B817-7FCB-43CE-9F32-9CB60CF14658"
    },
    {
      "SubscriptionId": "7578872A-18C1-4E6B-8F51-469555337389"
    },
    {
      "SubscriptionId": "00601E10-4C05-4BA2-B977-6578F5C81D69"
    },
    {
      "SubscriptionId": "7EBFC3A9-D502-4EA2-87E7-C42971639E8C"
    },
    {
      "SubscriptionId": "2AC30AE1-5934-48FB-A0E5-EF6985761138"
    }
  ],
  "nextLink": null,
  "totalCount": 100,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

### <a name="step-4-create-the-report"></a>Stap 4: Het rapport maken

In deze stap gebruiken we de eerder gegenereerde QueryId om het rapport te maken.

#### <a name="request-example"></a>Voorbeeld van aanvraag

```cli
curl 
--location 
--request POST 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport'\
--header ' Authorization: Bearer <AADToken>' \ 
--header 'Content-Type: application/json' \ 
--data-raw 
'{
  "ReportName": "DynamicsUsage Subscription ID Report",
  "Description": "Report for getting list of Subscription Id for Dynamics Usage",
  "QueryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
  "StartTime": "2021-04-01T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": "2021-03-31T18:41:00Z",
  "QueryEndTime": "2021-06-30T18:41:00Z",
  "RecurrenceInterval": 48,
  "RecurrenceCount": 20,
  "Format": "csv",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}'
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
  "value": [
    {
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "reportName": "DynamicsUsage Subscription ID Report",
      "description": "Report for getting list of Subscription Id for Dynamics Usage",
      "queryId": "7d19305c-56db-4edc-b776-428340e3a9c8",
      "query": "SELECT SubscriptionId from DynamicsUsage",
      "user": "GAUser@PITEST2.ccsctp.net",
      "createdTime": "2021-03-31T08:15:15Z",
      "modifiedTime": null,
      "executeNow": false,
      "startTime": "2021-04-01T18:41:00Z",
      "reportStatus": "Active",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": "https://<SampleCallbackUrl>",
      "CallbackMethod": "GET",
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

Bij een geslaagde uitvoering wordt `reportId` een gegenereerd die moet worden gebruikt om een download van het rapport te plannen.

### <a name="step-5-execute-report-executions-api"></a>Stap 5: API voor het uitvoeren van rapportuitvoeringen

In deze stap gebruiken we de API voor rapportuitvoeringen om de beveiligde locatie (URL) van het rapport op te halen.

#### <a name="request-example"></a>Voorbeeld van aanvraag

```cli
Curl
--location 
--request GET 'https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/ cdc61cfe-d028-4333-a215-a1df51ccbfd4?getLatestExecution=true'\
--header ' Authorization: Bearer <AADToken>' \
```

#### <a name="response-example"></a>Voorbeeld van antwoord

```json
{
  "value": [
    {
      "executionId": "315eb63e-e2b2-41a2-ad8e-790b040fdce3",
      "reportId": "cdc61cfe-d028-4333-a215-a1df51ccbfd4",
      "recurrenceInterval": 48,
      "recurrenceCount": 20,
      "callbackUrl": null,
      "CallbackMethod": null,
      "format": "csv",
      "executionStatus": "Pending",
      "reportLocation": null,
      "reportAccessSecureLink": null,
      "reportExpiryTime": null,
      "reportGeneratedTime": null
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

## <a name="next-steps"></a>Volgende stappen

- Probeer de API's uit via de [Swagger API-URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)