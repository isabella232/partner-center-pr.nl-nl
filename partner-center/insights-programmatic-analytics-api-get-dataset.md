---
title: Alle api voor gegevenssets op halen - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik deze API om details op te halen van alle beschikbare gegevenssets in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 8f4e69c8759c16bc38e64a361c8c077989447d3e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957415"
---
# <a name="get-all-datasets-api"></a>Alle gegevenssets-API op halen

De API Alle gegevenssets verkrijgen haalt alle beschikbare gegevenssets op. Gegevenssets maken een lijst van de tabellen, kolommen, metrische gegevens en tijdsbereiken.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

**Aanvraagheader**

|    Header    |    Type    |    Description    |
|    ----    |    ----    |    ----    |
|    Autorisatie    |    tekenreeks    |    Vereist. Het Azure Active Directory -toegang token (AAD) in het formulier`Bearer <token>`    |
|    Content-Type    |    tekenreeks    |    `Application/JSON`    |
|        |        |        |

**Padparameter**

Geen

**Queryparameter**

|    Parameternaam    |    Type    |    Vereist    |    Beschrijving    |
|    ----    |    ----    |    ----    |    ----    |
|    datasetName    |    tekenreeks    |    No    |    Filteren om details van slechts één gegevensset op te halen    |
|        |        |        |        |

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
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

**Woordenlijst**

Deze tabel definieert de belangrijkste elementen in het antwoord:

|    Parameter    |    Beschrijving    |
|    ----    |    ----    |
|    DatasetName     |    Naam van de gegevensset die door dit matrixobject wordt bepaald     |
|    SelectableColumns     |    Onbewerkte kolommen die kunnen worden opgegeven in de geselecteerde kolommen     |
|    AvailableMetrics     |    Aggregatie-/metrische kolomnamen die kunnen worden opgegeven in de geselecteerde kolommen     |
|    AvailableDateRanges     |    Datumbereik dat kan worden gebruikt in rapportquery's voor de gegevensset     |
|    minimumRecurrenceInterval     |    Minimumwaarde van terugkeerpatroon     |
|    Totaal aantal     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
