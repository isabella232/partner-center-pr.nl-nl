---
title: Api voor rapportquery's proberen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om uw query te testen en de resultaten te valideren in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c83b56b7d52e0b9feb598597b4a8e1fdaec98a3b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845598"
---
# <a name="try-report-queries-api"></a>Api voor rapportquery's proberen

Met deze API wordt een rapportquery-instructie uitgevoerd. De API retourneert slechts 100 records die u als partner kunt gebruiken om te controleren of de gegevens zijn zoals verwacht.

> [!IMPORTANT]
> Deze API heeft een time-out voor het uitvoeren van query's van 100 seconden. Als u merkt dat de API meer dan 100 seconden duurt, is het zeer waarschijnlijk dat de query syntactisch juist is, anders zou u een andere foutcode dan 200 hebben ontvangen. De werkelijke rapportgeneratie wordt doorgegeven als de querysyntaxis juist is.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Beschrijving    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory (AAD) in de vorm`Bearer <token>`    |
|    Content-Type    |    tekenreeks    |    `Application/JSON`    |
|        |        |        |

**Padparameter**

Geen

**Queryparameter**

|    Parameternaam    |    Type    |    Vereist    |    Beschrijving    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    tekenreeks    |    No    |    Rapportqueryreeks die moet worden uitgevoerd     |
|    queryId     |    tekenreeks    |    No    |    Een geldige bestaande query-id. Sluiten elkaar wederzijds uit met een queryreeks die is opgegeven in de exportQuery-parameter    |
|    startTime     |    tekenreeks    |    No    |    Begintijd van waaruit we de gegevens willen. De periode die is opgegeven in de query wordt overschreven    |
|    endTime     |    tekenreeks    |    No    |    Eindtijd totdat we de gegevens willen. De periode die is opgegeven in de query wordt overschreven    |
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
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
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
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
