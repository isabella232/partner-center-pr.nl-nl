---
title: Lijst met voorbeeldquery's
description: Gebruik de voorbeeldquery's om programmatisch toegang te krijgen tot analysegegevens van partnerinzichten.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376507"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="c89a9-103">Voorbeeldquery's voor Partner Center insights-rapport</span><span class="sxs-lookup"><span data-stu-id="c89a9-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="c89a9-104">Dit artikel bevat voorbeeldquery's voor de partnerrapporten Insights rapporten.</span><span class="sxs-lookup"><span data-stu-id="c89a9-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="c89a9-105">U kunt deze query's gebruiken door het eindpunt van de API rapportquery maken aan te roepen.</span><span class="sxs-lookup"><span data-stu-id="c89a9-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="c89a9-106">Indien nodig kan de api-aanroep [Rapportquery maken](insights-programmatic-access-paradigm.md#create-report-query-api) worden gewijzigd om meer kolommen toe te voegen, de berekeningsperiode aan te passen en filtervoorwaarden toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="c89a9-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="c89a9-107">Raadpleeg gegevensdefinities voor meer informatie over de kolomnamen, kenmerken en [beschrijvingen.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="c89a9-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="c89a9-108">Klantgegevens</span><span class="sxs-lookup"><span data-stu-id="c89a9-108">Customer details</span></span>

<span data-ttu-id="c89a9-109">Deze voorbeeldquery's zijn van toepassing op het detailrapport van de klant:</span><span class="sxs-lookup"><span data-stu-id="c89a9-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="c89a9-110">Op geografische locatie</span><span class="sxs-lookup"><span data-stu-id="c89a9-110">By geography</span></span>

<span data-ttu-id="c89a9-111">Lijst met klanten van een specifieke geografie in de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="c89a9-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="c89a9-112">Per SKU en gefactureerde omzet</span><span class="sxs-lookup"><span data-stu-id="c89a9-112">By SKU and billed revenue</span></span>

<span data-ttu-id="c89a9-113">Lijst met klanten die een specifieke SKU en gefactureerde omzet gebruiken, is in de afgelopen 6 maanden meer dan 20.000</span><span class="sxs-lookup"><span data-stu-id="c89a9-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="c89a9-114">Op beschikbare seats</span><span class="sxs-lookup"><span data-stu-id="c89a9-114">By available seats</span></span>

<span data-ttu-id="c89a9-115">Top 10 klanten op basis van beschikbare seats in de afgelopen maand</span><span class="sxs-lookup"><span data-stu-id="c89a9-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="c89a9-116">Partnerprofiel</span><span class="sxs-lookup"><span data-stu-id="c89a9-116">Partner Profile</span></span>

<span data-ttu-id="c89a9-117">Deze voorbeeldquery's zijn van toepassing op het partnerprofielrapport:</span><span class="sxs-lookup"><span data-stu-id="c89a9-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="c89a9-118">Op geografische locatie</span><span class="sxs-lookup"><span data-stu-id="c89a9-118">By geography</span></span>

<span data-ttu-id="c89a9-119">Lijst met partners uit een specifieke geografie.</span><span class="sxs-lookup"><span data-stu-id="c89a9-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="c89a9-120">Door MPN-partner</span><span class="sxs-lookup"><span data-stu-id="c89a9-120">By MPN partner</span></span>

<span data-ttu-id="c89a9-121">Lijst met partners onder dezelfde PGA MPN-partner</span><span class="sxs-lookup"><span data-stu-id="c89a9-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="c89a9-122">Resellerprestaties</span><span class="sxs-lookup"><span data-stu-id="c89a9-122">Reseller Performance</span></span>

<span data-ttu-id="c89a9-123">Deze voorbeeldquery's zijn van toepassing op het prestatierapport van de reseller:</span><span class="sxs-lookup"><span data-stu-id="c89a9-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="c89a9-124">Op geografische locatie</span><span class="sxs-lookup"><span data-stu-id="c89a9-124">By geography</span></span>

<span data-ttu-id="c89a9-125">Lijst met resellers van een specifieke geografie in de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="c89a9-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="c89a9-126">Per reseller</span><span class="sxs-lookup"><span data-stu-id="c89a9-126">By reseller</span></span>

<span data-ttu-id="c89a9-127">Aantal klanten, aantal abonnementen, totale beschikbare seats, totaal aantal toegewezen seats, totale omzet voor een specifieke reseller.</span><span class="sxs-lookup"><span data-stu-id="c89a9-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="c89a9-128">Top 10 op omzet</span><span class="sxs-lookup"><span data-stu-id="c89a9-128">Top 10 by revenue</span></span>

<span data-ttu-id="c89a9-129">Top 10 resellers op basis van de totale omzet in de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="c89a9-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="c89a9-130">Abonnementsgegevens</span><span class="sxs-lookup"><span data-stu-id="c89a9-130">Subscription Details</span></span>

<span data-ttu-id="c89a9-131">Deze voorbeeldquery's zijn van toepassing op het rapport met abonnementsgegevens:</span><span class="sxs-lookup"><span data-stu-id="c89a9-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="c89a9-132">Door geschiktheid voor verlenging</span><span class="sxs-lookup"><span data-stu-id="c89a9-132">By renewal eligibility</span></span>

<span data-ttu-id="c89a9-133">Lijst met abonnementen die niet in aanmerking komen voor automatische verlenging in de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="c89a9-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="c89a9-134">Op abonnementsstaat</span><span class="sxs-lookup"><span data-stu-id="c89a9-134">By subscription state</span></span>

<span data-ttu-id="c89a9-135">Lijst met abonnementen met de status Uitschakelen in de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="c89a9-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="c89a9-136">Tellingen voor zes maanden</span><span class="sxs-lookup"><span data-stu-id="c89a9-136">Counts for six months</span></span>

<span data-ttu-id="c89a9-137">Aantal abonnementen, totaal aantal verkochte seats, klanttelling voor een specifieke partner in de afgelopen zes maanden.</span><span class="sxs-lookup"><span data-stu-id="c89a9-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="c89a9-138">Azure-gebruik</span><span class="sxs-lookup"><span data-stu-id="c89a9-138">Azure Usage</span></span>

<span data-ttu-id="c89a9-139">Deze voorbeeldquery's zijn van toepassing op het Azure-gebruiksrapport:</span><span class="sxs-lookup"><span data-stu-id="c89a9-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="c89a9-140">Per metercategorie</span><span class="sxs-lookup"><span data-stu-id="c89a9-140">By meter category</span></span>

<span data-ttu-id="c89a9-141">Lijst met Azure-gebruiksabonnementen met gebruikseenheden en ACR voor specifieke metercategorie in de afgelopen zes maanden.</span><span class="sxs-lookup"><span data-stu-id="c89a9-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="c89a9-142">Op totaal ACR</span><span class="sxs-lookup"><span data-stu-id="c89a9-142">By total ACR</span></span>

<span data-ttu-id="c89a9-143">Lijst met Azure-gebruiksabonnementen waarbij de totale ACR de afgelopen zes maanden hoger is dan 20.000</span><span class="sxs-lookup"><span data-stu-id="c89a9-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="c89a9-144">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="c89a9-144">Next steps</span></span>

- [<span data-ttu-id="c89a9-145">API's voor toegang tot analysegegevens van partnerinzichten</span><span class="sxs-lookup"><span data-stu-id="c89a9-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)