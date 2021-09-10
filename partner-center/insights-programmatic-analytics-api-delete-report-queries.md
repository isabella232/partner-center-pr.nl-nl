---
title: API voor rapportquery's verwijderen - Insights verwijderen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om door de gebruiker gedefinieerde query's in Partner Center verwijderen.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: f755bc13ff4e0c4bc3a2c6ceda123c6a2bc47dc5
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957409"
---
# <a name="delete-report-queries-api"></a>API voor rapportquery's verwijderen

Met deze API worden door de gebruiker gedefinieerde query's verwijderd.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    DELETE    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
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
|    queryId     |    tekenreeks     |    No    |    Filter om alleen details van query's op te halen met de id die is opgegeven in het argument     |
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
|    QueryId     |    Unieke UUID van de verwijderde query    |
|    Name     |    Naam van de verwijderde query    |
|    Description     |    Beschrijving van de verwijderde query     |
|    Query’s uitvoeren     |    Rapportqueryreeks van de verwijderde query    |
|    Type     |    Ingesteld op userDefined voor door de gebruiker gemaakte query's     |
|    Gebruiker     |    Gebruikers-id die de query heeft gemaakt     |
|    CreatedTime     |    Tijdstip van het maken van de query     |
|    TotalCount     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
