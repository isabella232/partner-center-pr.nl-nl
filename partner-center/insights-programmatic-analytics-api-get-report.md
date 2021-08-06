---
title: Rapport-API op Insights halen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om alle beschikbare rapport-id's op te halen in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 9c6930d8be430f6a9219e7b3d11b2e64ed2af5253b81581581ad6254a2a1d8d3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697139"
---
# <a name="get-report-api"></a>Rapport-API op halen

Deze API haalt alle rapporten op die zijn gepland.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory (AAD) in de vorm`Bearer <token>`    |
|    Content-Type    |    tekenreeks    |    `Application/JSON`    |
|        |        |        |

**Padparameter**

Geen

**Queryparameter**

|    Parameternaam    |    Type    |    Vereist    |    Beschrijving    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    tekenreeks    |    No    |    Filter om alleen details van rapporten op te halen met de reportId die in dit argument is opgegeven     |
|    reportName     |    tekenreeks    |    No    |    Filter om alleen details van rapporten op te halen met de reportName in dit argument     |
|    queryId     |    tekenreeks    |    No    |    Filter om alleen details van rapporten op te halen met de queryId die in dit argument is opgegeven     |
|        |        |        |        |


**Nettolading aanvragen**

Geen

**Woordenlijst**

Geen

**Response**

De nettolading van het antwoord is als volgt gestructureerd:

Antwoordcode: 200, 400, 401, 403, 404, 500

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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Woordenlijst**

Deze tabel definieert de belangrijkste elementen in het antwoord:

|    Parameter    |    Beschrijving    |
|    ----    |    ----    |
|    ReportId     |    Unieke UUID van het rapport dat is gemaakt     |
|    ReportName     |    Naam van het rapport in de nettolading van de aanvraag     |
|    Description     |    Beschrijving die is opgegeven bij het maken van het rapport     |
|    QueryId     |    Query-id doorgegeven op het moment dat het rapport werd gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    Tijd dat het rapport is gemaakt. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Het tijdstip dat het rapport voor het laatst is gewijzigd. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    executeNow     |    ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt    |
|    StartTime     |    De uitvoering van de tijd begint. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status van de uitvoering van het rapport. De mogelijke waarden zijn Onderbroken, Actief en Inactief.     |
|    RecurrenceInterval     |    Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport     |
|    RecurrenceCount     |    Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport     |
|    CallbackUrl     |    Callback-URL die is opgegeven in de aanvraag     |
|    CallbackMethod    |    Callback-methode die is opgegeven in de aanvraag    |
|    Indeling     |    Indeling van de rapportbestanden     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |