---
title: Alle gegevenssets-API-gegevenssets Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om details op te halen van alle beschikbare gegevenssets in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376513"
---
# <a name="get-all-datasets-api"></a>Api voor alle gegevenssets krijgen

De API Alle gegevenssets verkrijgen haalt alle beschikbare gegevenssets op. Gegevenssets maken een lijst van de tabellen, kolommen, metrische gegevens en tijdsbereiken.

**Aanvraagsyntaxis**

|    Methode    |    Aanvraag-URI    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
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
|    datasetName    |    tekenreeks    |    No    |    Filteren om details van slechts één gegevensset op te halen    |
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
|    DatasetName     |    Naam van de gegevensset die dit matrixobject definieert     |
|    SelectableColumns     |    Onbewerkte kolommen die kunnen worden opgegeven in de geselecteerde kolommen     |
|    AvailableMetrics     |    Aggregatie-/metrische kolomnamen die kunnen worden opgegeven in de geselecteerde kolommen     |
|    AvailableDateRanges     |    Datumbereik dat kan worden gebruikt in rapportquery's voor de gegevensset     |
|    minimumRecurrenceInterval     |    Minimale waarde van terugkeerinterval     |
|    TotalCount     |    Aantal gegevenssets in de matrix Waarde     |
|    Bericht     |    Statusbericht van de uitvoering van de API     |
|    StatusCode     |    Resultaatcode. De mogelijke waarden zijn 200, 400, 401, 403, 500     |
|        |        |
