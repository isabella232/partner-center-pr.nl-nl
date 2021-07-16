---
title: API voor rapportquery's opvragen - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om alle beschikbare query's op te halen voor gebruik in de rapport-API.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376752"
---
# <a name="get-report-queries-api"></a>API voor rapportquery's opvragen

De API Rapportquery's krijgen haalt alle query's op die beschikbaar zijn voor gebruik in rapporten. Alle systeem- en door de gebruiker gedefinieerde query's worden standaard opgevraagd.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Beschrijving    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory (AAD) in het formulier`Bearer <token>`    |
|    Content-Type    |    tekenreeks    |    `Application/JSON`    |
|        |        |        |

**Padparameter**

Geen

**Queryparameter**

|    Parameternaam    |    Type    |    Vereist    |    Beschrijving    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    tekenreeks     |    No    |    Filter om alleen details van query's op te halen met de id die is opgegeven in het argument     |
|    queryName     |    tekenreeks     |    No    |    Filter om alleen details van query's op te halen met de naam die is opgegeven in het argument     |
|    IncludeSystemQueries     |    booleaans     |    Nee    |    Vooraf gedefinieerde systeemquery's opnemen in het antwoord     |
|    IncludeOnlySystemQueries     |    booleaans     |    Nee    |    Alleen systeemquery's opnemen in het antwoord     |
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
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
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
|    QueryId     |    Unieke UUID van de query     |
|    Name     |    Naam die aan de query is gegeven op het moment dat de query wordt gemaakt     |
|    Beschrijving     |    Beschrijving gegeven tijdens het maken van de query     |
|    Query’s uitvoeren     |    Rapportqueryreeks     |
|    Type     |    Ingesteld op userDefined voor door de gebruiker gemaakte query's en systeem voor vooraf gedefinieerde systeemquery's     |
|    Gebruiker     |    Gebruikers-id die de query heeft gemaakt     |
|    CreatedTime     |    Tijdstip van het maken van de query     |
|    TotalCount     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
