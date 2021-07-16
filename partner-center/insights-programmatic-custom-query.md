---
title: Aangepaste queryspecificatie
description: Meer informatie over het maken van aangepaste query's voor het extraheren van gegevens uit analysetabellen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376571"
---
# <a name="custom-query-specification"></a><span data-ttu-id="ade13-103">Aangepaste queryspecificatie</span><span class="sxs-lookup"><span data-stu-id="ade13-103">Custom query specification</span></span>

<span data-ttu-id="ade13-104">Partners kunnen deze queryspecificatie gebruiken om eenvoudig aangepaste query's te formuleren voor het extraheren van gegevens uit analysetabellen.</span><span class="sxs-lookup"><span data-stu-id="ade13-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="ade13-105">De query's kunnen worden gebruikt om alleen de gewenste kolommen en metrische gegevens te selecteren die aan een bepaald criterium voldoen.</span><span class="sxs-lookup"><span data-stu-id="ade13-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="ade13-106">De kern van de taalspecificatie is de gegevenssetdefinitie waarop een aangepaste query kan worden geschreven.</span><span class="sxs-lookup"><span data-stu-id="ade13-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="ade13-107">Gegevenssets</span><span class="sxs-lookup"><span data-stu-id="ade13-107">Datasets</span></span>

<span data-ttu-id="ade13-108">Op dezelfde manier als sommige query's worden uitgevoerd op een database met tabellen en kolommen, werkt een aangepaste query voor gegevenssets met kolommen en metrische gegevens.</span><span class="sxs-lookup"><span data-stu-id="ade13-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="ade13-109">De volledige lijst met beschikbare gegevenssets voor het formuleren van een query kan worden verkregen met behulp van de API voor gegevenssets.</span><span class="sxs-lookup"><span data-stu-id="ade13-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="ade13-110">Dit is een voorbeeld van een gegevensset die wordt weergegeven als een JSON:</span><span class="sxs-lookup"><span data-stu-id="ade13-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="ade13-111">Onderdelen van een gegevensset</span><span class="sxs-lookup"><span data-stu-id="ade13-111">Parts of a dataset</span></span>

- <span data-ttu-id="ade13-112">De naam van een gegevensset is net als de naam van een databasetabel.</span><span class="sxs-lookup"><span data-stu-id="ade13-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="ade13-113">Bijvoorbeeld OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="ade13-113">For example, OfficeUsage.</span></span> <span data-ttu-id="ade13-114">Een gegevensset bevat een lijst met kolommen die kunnen worden geselecteerd, zoals CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="ade13-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="ade13-115">Een gegevensset bevat ook metrische gegevens, zoals aggregatiefuncties in een database.</span><span class="sxs-lookup"><span data-stu-id="ade13-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="ade13-116">Bijvoorbeeld TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="ade13-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="ade13-117">Er zijn vaste tijdsspannen waarin gegevens kunnen worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="ade13-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="ade13-118">Een query op een gegevensset formuleren</span><span class="sxs-lookup"><span data-stu-id="ade13-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="ade13-119">Dit zijn enkele voorbeeldquery's die laten zien hoe u verschillende typen gegevens kunt extraheren.</span><span class="sxs-lookup"><span data-stu-id="ade13-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="ade13-120">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="ade13-120">Query</span></span>|    <span data-ttu-id="ade13-121">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ade13-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="ade13-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="ade13-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="ade13-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="ade13-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="ade13-124">Met deze query worden elke CusotmerTenantID en de bijbehorende PaidAvailableUnits in de afgelopen maand opgevraagd.</span><span class="sxs-lookup"><span data-stu-id="ade13-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="ade13-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="ade13-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="ade13-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="ade13-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="ade13-127">Met deze query worden de top 10 van tenants van klanten in aflopende volgorde van het aantal betaalde beschikbare eenheden opgevraagd.</span><span class="sxs-lookup"><span data-stu-id="ade13-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="ade13-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="ade13-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="ade13-129">Deze query krijgt de PaidAvailableUnits en MonthlyActiveUsers van alle klanten met MonthlyActiveUsers die groter zijn dan 100.000.</span><span class="sxs-lookup"><span data-stu-id="ade13-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="ade13-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="ade13-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="ade13-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="ade13-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="ade13-132">Met deze query worden de CustomerTenantId en de maandelijks actieve gebruikers voor elke maand opgevraagd met de twee waarden voor CustomerTpId: '2a31c234-1f4e-4c60-909e-909e76d234f93161' en '80780748-3f9a-11eb-b378-0242ac130002'.</span><span class="sxs-lookup"><span data-stu-id="ade13-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="ade13-133">Queryspecificatie</span><span class="sxs-lookup"><span data-stu-id="ade13-133">Query specification</span></span>

<span data-ttu-id="ade13-134">In deze sectie worden de querydefinitie en -structuur beschreven.</span><span class="sxs-lookup"><span data-stu-id="ade13-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="ade13-135">Grammaticaverwijzing</span><span class="sxs-lookup"><span data-stu-id="ade13-135">Grammar reference</span></span>

<span data-ttu-id="ade13-136">In deze tabel worden de symbolen beschreven die worden gebruikt in query's.</span><span class="sxs-lookup"><span data-stu-id="ade13-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="ade13-137">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="ade13-137">Query</span></span>    |    <span data-ttu-id="ade13-138">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ade13-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="ade13-139">Optioneel</span><span class="sxs-lookup"><span data-stu-id="ade13-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="ade13-140">Nul of meer</span><span class="sxs-lookup"><span data-stu-id="ade13-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="ade13-141">Een of meer</span><span class="sxs-lookup"><span data-stu-id="ade13-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="ade13-142">Of / Een van de lijsten</span><span class="sxs-lookup"><span data-stu-id="ade13-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="ade13-143">Querydefinitie</span><span class="sxs-lookup"><span data-stu-id="ade13-143">Query definition</span></span>

<span data-ttu-id="ade13-144">De query-instructie bevat de volgende componenten: SelectClause, FromClause, WhereClause, OrderClause, LimitClause en TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="ade13-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="ade13-145">**SelectClause:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="ade13-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="ade13-146">**ColumOrMetricName:** kolommen en metrische gegevens die zijn gedefinieerd in de gegevensset</span><span class="sxs-lookup"><span data-stu-id="ade13-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="ade13-147">**FromClause:**`FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="ade13-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="ade13-148">**DatasetName:** de naam van de gegevensset die is gedefinieerd in de gegevensset</span><span class="sxs-lookup"><span data-stu-id="ade13-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="ade13-149">**WhereClause:**`WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="ade13-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="ade13-150">**FilterCondition:** ColumOrMetricName Operator Value</span><span class="sxs-lookup"><span data-stu-id="ade13-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="ade13-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="ade13-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="ade13-152">**Waarde:**| StringLiteral | MultiNumberList-| MultiStringList</span><span class="sxs-lookup"><span data-stu-id="ade13-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="ade13-153">**Getal**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="ade13-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="ade13-154">**StringLiteral:**`' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="ade13-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="ade13-155">**MultiNumberList:**`(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="ade13-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="ade13-156">**MultiStringList:**`(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="ade13-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="ade13-157">**OrderClause:**`ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="ade13-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="ade13-158">**OrderCondition:**`ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="ade13-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="ade13-159">**LimitClause:**`LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="ade13-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="ade13-160">**TimeSpan:**`TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="ade13-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="ade13-161">Querystructuur</span><span class="sxs-lookup"><span data-stu-id="ade13-161">Query Structure</span></span>

<span data-ttu-id="ade13-162">Een rapportquery bestaat uit meerdere onderdelen:</span><span class="sxs-lookup"><span data-stu-id="ade13-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="ade13-163">Elk onderdeel wordt hieronder beschreven.</span><span class="sxs-lookup"><span data-stu-id="ade13-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="ade13-164">In dit deel van de query worden de kolommen opgegeven die worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="ade13-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="ade13-165">De kolommen die kunnen worden geselecteerd, zijn de velden die worden vermeld in de secties *selectableColumns* en *availableMetrics* van een gegevensset.</span><span class="sxs-lookup"><span data-stu-id="ade13-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="ade13-166">Optioneel kan `DISTINCT` het trefwoord worden opgegeven na `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="ade13-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="ade13-167">Als `DISTINCT` is opgegeven, bevatten de uiteindelijke geëxporteerde rijen altijd afzonderlijke waarden van de geselecteerde kolommen.</span><span class="sxs-lookup"><span data-stu-id="ade13-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="ade13-168">Metrische gegevens worden berekend voor elke afzonderlijke combinatie van de geselecteerde kolommen. Het trefwoord is daarom niet vereist wanneer een metrische kolom wordt opgenomen `DISTINCT` in de lijst met geselecteerde kolommen.</span><span class="sxs-lookup"><span data-stu-id="ade13-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="ade13-169">**Voorbeeld:**</span><span class="sxs-lookup"><span data-stu-id="ade13-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="ade13-170">Dit deel van de query geeft de gegevensset aan van waaruit gegevens moeten worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="ade13-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="ade13-171">De hier opgegeven naam van de gegevensset moet een geldige gegevenssetnaam zijn die wordt geretourneerd door de API voor gegevenssets.</span><span class="sxs-lookup"><span data-stu-id="ade13-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="ade13-172">**Voorbeeld:**</span><span class="sxs-lookup"><span data-stu-id="ade13-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="ade13-173">Dit deel van de query wordt gebruikt om filtervoorwaarden op te geven voor de gegevensset.</span><span class="sxs-lookup"><span data-stu-id="ade13-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="ade13-174">Alleen rijen die overeenkomen met alle voorwaarden die in deze component worden vermeld, zijn aanwezig in het uiteindelijke geëxporteerde bestand.</span><span class="sxs-lookup"><span data-stu-id="ade13-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="ade13-175">De filtervoorwaarde kan worden gebruikt voor alle kolommen die worden vermeld in *selectableColumns* en *availableMetrics.*</span><span class="sxs-lookup"><span data-stu-id="ade13-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="ade13-176">De waarden die zijn opgegeven in de filtervoorwaarde kunnen alleen een lijst met getallen of een lijst met tekenreeksen zijn als de operator `IN` of `NOT IN` is.</span><span class="sxs-lookup"><span data-stu-id="ade13-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="ade13-177">De waarden kunnen altijd worden opgegeven als een letterlijke tekenreeks en worden geconverteerd naar de native typen kolommen.</span><span class="sxs-lookup"><span data-stu-id="ade13-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="ade13-178">Meerdere filtervoorwaarden moeten worden gescheiden door een AND-bewerking.</span><span class="sxs-lookup"><span data-stu-id="ade13-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="ade13-179">**Voorbeeld:**</span><span class="sxs-lookup"><span data-stu-id="ade13-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="ade13-180">In dit deel van de query worden de bestelcriteria voor de geëxporteerde rijen opgegeven.</span><span class="sxs-lookup"><span data-stu-id="ade13-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="ade13-181">De kolommen waarop de volgorde kan worden gedefinieerd, moeten afkomstig zijn uit *de selectableColumns* en *availableMetrics* van de gegevensset.</span><span class="sxs-lookup"><span data-stu-id="ade13-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="ade13-182">Als er geen volgorde is opgegeven, wordt deze standaard ingesteld op DESC in de kolom.</span><span class="sxs-lookup"><span data-stu-id="ade13-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="ade13-183">Volgorde kan worden gedefinieerd voor meerdere kolommen door de criteria te scheiden met een komma.</span><span class="sxs-lookup"><span data-stu-id="ade13-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="ade13-184">**Voorbeeld:**</span><span class="sxs-lookup"><span data-stu-id="ade13-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="ade13-185">In dit deel van de query wordt het aantal rijen opgegeven dat wordt geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="ade13-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="ade13-186">Het getal dat u opgeeft, moet een positief geheel getal zonderzero zijn.</span><span class="sxs-lookup"><span data-stu-id="ade13-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="ade13-187">Dit deel van de query geeft de tijdsduur aan waarvoor de gegevens moeten worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="ade13-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="ade13-188">De mogelijke waarden moeten afkomstig zijn uit het *veld availableDateRanges* in de definitie van de gegevensset.</span><span class="sxs-lookup"><span data-stu-id="ade13-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="ade13-189">Gevoeligheid van case in queryspecificatie</span><span class="sxs-lookup"><span data-stu-id="ade13-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="ade13-190">De specificatie is volledig niet-casegevoelig.</span><span class="sxs-lookup"><span data-stu-id="ade13-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="ade13-191">Vooraf gedefinieerde trefwoorden, kolomnamen en waarden kunnen worden opgegeven met behulp van hoofdletters of kleine hoofdletters.</span><span class="sxs-lookup"><span data-stu-id="ade13-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ade13-192">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="ade13-192">Next steps</span></span>

- [<span data-ttu-id="ade13-193">Lijst met systeemquery's</span><span class="sxs-lookup"><span data-stu-id="ade13-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="ade13-194">Lijst met voorbeeldquery's</span><span class="sxs-lookup"><span data-stu-id="ade13-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)