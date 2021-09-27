---
title: Aangepaste queryspecificatie
description: Meer informatie over het maken van aangepaste query's voor het extraheren van gegevens uit analysetabellen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 2bf688e5068c1a88d0c5d1b6e7da7c94f8a4e7e8
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129073411"
---
# <a name="custom-query-specification"></a>Aangepaste queryspecificatie

Partners kunnen deze queryspecificatie gebruiken om eenvoudig aangepaste query's te formuleren voor het extraheren van gegevens uit analysetabellen. De query's kunnen worden gebruikt om alleen de gewenste kolommen en metrische gegevens te selecteren die aan een bepaald criterium voldoen. De kern van de taalspecificatie is de gegevenssetdefinitie waarop een aangepaste query kan worden geschreven.

## <a name="datasets"></a>Gegevenssets

Op dezelfde manier als sommige query's worden uitgevoerd op een database met tabellen en kolommen, werkt een aangepaste query op gegevenssets met kolommen en metrische gegevens. De volledige lijst met beschikbare gegevenssets voor het formuleren van een query kan worden verkregen met behulp van de API voor gegevenssets.

Dit is een voorbeeld van een gegevensset die wordt weergegeven als een JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Onderdelen van een gegevensset

- De naam van een gegevensset is net als de naam van een databasetabel. Bijvoorbeeld OfficeUsage. Een gegevensset bevat een lijst met kolommen die kunnen worden geselecteerd, zoals CustomerTenantId.
- Een gegevensset bevat ook metrische gegevens, zoals aggregatiefuncties in een database. Bijvoorbeeld TotalMonthlyActiveUsers.
- Er zijn vaste tijdsspannen waarin gegevens kunnen worden geëxporteerd.

## <a name="formulating-a-query-on-a-dataset"></a>Een query op een gegevensset formuleren

Dit zijn enkele voorbeeldquery's die laten zien hoe u verschillende typen gegevens kunt extraheren.

|Query’s uitvoeren|    Beschrijving    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Met deze query worden elke CusotmerTenantID en de bijbehorende PaidAvailableUnits in de afgelopen maand opgevraagd.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Met deze query worden de top 10 van de tenants van klanten in aflopende volgorde van het aantal betaalde beschikbare eenheden opgevraagd.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Deze query krijgt de PaidAvailableUnits en MonthlyActiveUsers van alle klanten met MonthlyActiveUsers die groter zijn dan 100.000.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Met deze query worden de CustomerTenantId en de maandelijks actieve gebruikers voor elke maand opgevraagd met de twee waarden voor CustomerTpId: '2a31c234-1f4e-4c60-909e-976d234f93161' en '80780748-3f9a-11eb-b378-0242ac130002'.     |
|        |        |

## <a name="query-specification"></a>Queryspecificatie

In deze sectie worden de querydefinitie en -structuur beschreven.

## <a name="grammar-reference"></a>Grammaticaverwijzing

In deze tabel worden de symbolen beschreven die worden gebruikt in query's.

|    Query’s uitvoeren    |    Beschrijving    |
|    ----    |    ----    |
|    `?`    |    Optioneel    |
|    `*`    |    Nul of meer    |
|    `+`    |    Een of meer    |
|    `\|`    |    Of / Een van de lijsten    |
|        |        |

## <a name="query-definition"></a>Querydefinitie

De query-instructie bevat de volgende componenten: SelectClause, FromClause, WhereClause, OrderClause, LimitClause en TimeSpan.

- **SelectClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName:** kolommen en metrische gegevens die zijn gedefinieerd in de gegevensset
- **FromClause:**`FROM DatasetName`
    - **DatasetName:** de naam van de gegevensset die is gedefinieerd in de gegevensset
- **WhereClause:**`WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition:** ColumOrMetricName Operator Value
        - **Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Waarde:**| StringLiteral | MultiNumberList-| MultiStringList
            - **Getal**: `-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral:**`' [a-zA-Z0-9_]*'`
            - **MultiNumberList:**`(Number (,Number)*)`
            - **MultiStringList:**`(StringLiteral (,StringLiteral)*)`
- **OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition:**`ColumOrMetricName (ASC | DESC)*`
- **LimitClause:**`LIMIT [0-9]+`
- **TimeSpan:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Querystructuur

Een rapportquery bestaat uit meerdere onderdelen:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

Elk onderdeel wordt hieronder beschreven.

### `SELECT`

In dit deel van de query worden de kolommen opgegeven die worden geëxporteerd. De kolommen die kunnen worden geselecteerd, zijn de velden die worden vermeld in de secties *selectableColumns* en *availableMetrics* van een gegevensset.

Optioneel kan `DISTINCT` het trefwoord worden opgegeven na `SELECT` . Als `DISTINCT` is opgegeven, bevatten de uiteindelijke geëxporteerde rijen altijd afzonderlijke waarden van de geselecteerde kolommen. Metrische gegevens worden berekend voor elke afzonderlijke combinatie van de geselecteerde kolommen. Het trefwoord is daarom niet vereist wanneer een kolom met metrische gegevens wordt opgenomen `DISTINCT` in de lijst met geselecteerde kolommen.

**Voorbeeld:**

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Dit deel van de query geeft de gegevensset aan van waaruit gegevens moeten worden geëxporteerd. De hier opgegeven naam van de gegevensset moet een geldige gegevenssetnaam zijn die wordt geretourneerd door de API voor gegevenssets.

**Voorbeeld:**

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Dit deel van de query wordt gebruikt om filtervoorwaarden op te geven voor de gegevensset. Alleen rijen die overeenkomen met alle voorwaarden die in deze component worden vermeld, zijn aanwezig in het uiteindelijke geëxporteerde bestand. De filtervoorwaarde kan worden gebruikt voor alle kolommen die worden vermeld in *selectableColumns* en *availableMetrics.* De waarden die zijn opgegeven in de filtervoorwaarde kunnen alleen een lijst met getallen of een lijst met tekenreeksen zijn als de operator `IN` of `NOT IN` is. De waarden kunnen altijd worden opgegeven als een letterlijke tekenreeks en worden geconverteerd naar de native typen kolommen. Meerdere filtervoorwaarden moeten worden gescheiden door een AND-bewerking.

**Voorbeeld:**

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

In dit deel van de query worden de bestelcriteria voor de geëxporteerde rijen opgegeven. De kolommen waarop de volgorde kan worden gedefinieerd, moeten afkomstig zijn uit *de selectableColumns* en *availableMetrics* van de gegevensset. Als er geen volgorde is opgegeven, wordt deze standaard ingesteld op DESC in de kolom. Volgorde kan worden gedefinieerd voor meerdere kolommen door de criteria te scheiden met een komma.

**Voorbeeld:**

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

In dit deel van de query wordt het aantal rijen opgegeven dat wordt geëxporteerd. Het getal dat u opgeeft, moet een positief geheel getal zonderzero zijn.

### `TIMESPAN`

Dit deel van de query geeft de tijdsduur aan waarvoor de gegevens moeten worden geëxporteerd. De mogelijke waarden moeten afkomstig zijn uit het *veld availableDateRanges* in de definitie van de gegevensset.

### <a name="case-sensitivity-in-query-specification"></a>Gevoeligheid van case in queryspecificatie

De specificatie is volledig niet-casegevoelig. Vooraf gedefinieerde trefwoorden, kolomnamen en waarden kunnen worden opgegeven met behulp van hoofdletters of kleine waarden.

## <a name="next-steps"></a>Volgende stappen

- [Lijst met systeemquery's](insights-programmatic-system-queries.md)
- [Lijst met voorbeeldquery's](insights-programmatic-sample-queries.md)