---
title: API voor rapportquery's opvragen - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om alle beschikbare query's op te halen voor gebruik in de rapport-API.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 5f65784ce93350c92e0ffe38849ce505f045e0b0
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244896"
---
# <a name="get-report-queries-api"></a>API voor rapportquery's opvragen

De API Rapportquery's verkrijgen haalt alle query's op die beschikbaar zijn voor gebruik in rapporten. Alle systeem- en door de gebruiker gedefinieerde query's worden standaard opgevraagd.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    queryId     |    tekenreeks     |    No    |    Filter om alleen details van query's op te halen met de id die is opgegeven in het argument     |
|    queryName     |    tekenreeks     |    No    |    Filter om alleen details van query's op te halen met de naam die is opgegeven in het argument     |
|    IncludeSystemQueries     |    booleaans     |    No    |    Vooraf gedefinieerde systeemquery's opnemen in het antwoord     |
|    IncludeOnlySystemQueries     |    booleaans     |    No    |    Alleen systeemquery's opnemen in het antwoord     |
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
|    Description     |    Beschrijving opgegeven tijdens het maken van de query     |
|    Query’s uitvoeren     |    Rapportqueryreeks     |
|    Type     |    Ingesteld op userDefined voor door de gebruiker gemaakte query's en systeem voor vooraf gedefinieerde systeemquery's     |
|    Gebruiker     |    Gebruikers-id die de query heeft gemaakt     |
|    CreatedTime     |    Tijdstip van het maken van de query     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
