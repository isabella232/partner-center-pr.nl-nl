---
title: Api voor rapportuitvoering onderbreken - Insights analyseren
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om de uitvoering van een rapport in de Partner Center onderbreken.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 01bb70e46e5a80c039bfc90b2ac0a034aa73b1163f485af8b98676d756b73e18
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115697156"
---
# <a name="pause-report-executions-api"></a>API voor rapportuitvoeringen onderbreken

Bij de uitvoering pauzeert deze API de geplande uitvoering van rapporten.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/pause/{ReportID}`    |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory (AAD) in het formulier`Bearer <token>`    |
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

Geen

**Woordenlijst**

Geen

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
|    ReportId     |    Universally Unique Identifier (UUID) van het onderbroken rapport     |
|    ReportName     |    Naam die tijdens het maken aan het rapport is gegeven     |
|    Description     |    Beschrijving gegeven tijdens het maken van het rapport     |
|    QueryId     |    Query-id doorgegeven op het moment dat het rapport werd gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    Het tijdstip dat het rapport is gemaakt. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Het tijdstip dat het rapport voor het laatst is gewijzigd. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt     |
|    StartTime     |    Tijd dat de uitvoering van het rapport begint. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
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
