---
title: Rapport-API bijwerken
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om rapportparameters bij te werken in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376576"
---
# <a name="update-report-api"></a>Rapport-API bijwerken

Met deze API kunt u een rapportparameter wijzigen.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Beschrijving    |
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
|    ReportName     |    Ja     |    Naam die moet worden toegewezen aan het rapport     |    Tekenreeks     |
|    Beschrijving     |    Nee     |    Beschrijving van het gemaakte rapport     |    Tekenreeks     |
|    StartTime     |    Ja    |    Tijdstempel waarna het genereren van het rapport begint     |    Tekenreeks     |
|    RecurrenceInterval     |    Nee     |    Frequentie waarmee het rapport in uren moet worden gegenereerd. Minimumwaarde is 4     |    Geheel getal     |
|    RecurrenceCount     |    Nee     |    Het aantal te genereren rapport. De standaardwaarde is onbeperkt.     |    Geheel getal     |
|    Indeling     |    Nee    |    Bestandsindeling van het geëxporteerde bestand. De standaardwaarde is CSV     |    CSV/TSV     |
|    CallbackURL     |    Nee     |    HTTPS-callback-URL die moet worden aangeroepen bij het genereren van het rapport     |    Tekenreeks     |
|    CallbackMethod    |    Nee    |    Http-methode die moet worden gebruikt voor callback    |    GET/POST    |
|        |        |        |        |


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
|    ReportId     |    Universally Unique Identifier (UUID) van het rapport dat wordt bijgewerkt     |
|    ReportName     |    Naam van het rapport in de nettolading van de aanvraag     |
|    Beschrijving     |    Beschrijving van het rapport in de nettolading van de aanvraag     |
|    QueryId     |    Query-id doorgegeven op het moment dat het rapport werd gemaakt     |
|    Query’s uitvoeren     |    Querytekst die wordt uitgevoerd voor dit rapport     |
|    Gebruiker     |    Gebruikers-id die wordt gebruikt om het rapport te maken     |
|    CreatedTime     |    Tijd dat het rapport is gemaakt. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ModifiedTime     |    Het tijdstip dat het rapport voor het laatst is gewijzigd. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ExecuteNow     |    ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt    |
|    StartTime     |    Tijd dat de uitvoering van het rapport begint. De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Status van de uitvoering van het rapport. De mogelijke waarden zijn Onderbroken, Actief en Inactief.     |
|    RecurrenceInterval     |    Terugkeerpatroon dat is opgegeven in de nettolading van de aanvraag     |
|    RecurrenceCount     |    Aantal terugkeerpatroon dat is opgegeven in de nettolading van de aanvraag     |
|    CallbackUrl     |    Callback-URL die is opgegeven in de aanvraag     |
|    CallbackMethod    |    Callback-methode die is opgegeven in de aanvraag    |
|    Indeling     |    Indeling van de rapportbestanden     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |