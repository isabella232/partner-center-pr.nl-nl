---
title: Api voor rapportuitvoering onderbreken - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om de uitvoering van een rapport in uw Partner Center onderbreken.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 798c5e87a3935923bd91d8e74716999fb8be4f54
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957427"
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
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory (AAD) in de vorm`Bearer <token>`    |
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
|    ReportName     |    Naam die aan het rapport is gegeven tijdens het maken     |
|    Description     |    Beschrijving gegeven tijdens het maken van het rapport     |
|    QueryId     |    Query-id doorgegeven op het moment dat het rapport werd gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    Tijd dat het rapport is gemaakt. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Het tijdstip dat het rapport voor het laatst is gewijzigd. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt     |
|    StartTime     |    Tijd dat de uitvoering van het rapport begint. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status van de uitvoering van het rapport. De mogelijke waarden zijn Onderbroken, Actief en Inactief.     |
|    RecurrenceInterval     |    Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport     |
|    RecurrenceCount     |    Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport     |
|    CallbackUrl     |    Callback-URL die is opgegeven in de aanvraag     |
|    CallbackMethod    |    Callback-methode die is opgegeven in de aanvraag    |
|    Indeling     |    Indeling van de rapportbestanden     |
|    TotalCount     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
