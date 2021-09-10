---
title: Lijst met voorbeeldquery's
description: Gebruik de voorbeeldquery's om programmatisch toegang te krijgen tot analysegegevens van partnerinzichten.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 36da8a59548142bf09daf42dbc936fba15d46d1e
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957394"
---
# <a name="sample-queries-for-partner-center-insights-report"></a>Voorbeeldquery's voor Partner Center insights-rapport

Dit artikel bevat voorbeeldquery's voor de partnerrapporten Insights rapporten. U kunt deze query's gebruiken door het eindpunt rapportquery-API maken aan te roepen. Indien nodig kan de api-aanroep [Rapportquery maken](insights-programmatic-access-paradigm.md#create-report-query-api) worden gewijzigd om meer kolommen toe te voegen, de berekeningsperiode aan te passen en filtervoorwaarden toe te voegen.

Raadpleeg gegevensdefinities voor meer informatie over de kolomnamen, kenmerken en [beschrijvingen.](insights-data-definitions.md)

## <a name="customer-details"></a>Klantgegevens

Deze voorbeeldquery's zijn van toepassing op het detailrapport van de klant:

### <a name="by-geography"></a>Op geografische locatie

Lijst met klanten van een specifieke geografie in de afgelopen maand.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Per SKU en gefactureerde omzet

Lijst met klanten die een specifieke SKU en gefactureerde omzet gebruiken, is in de afgelopen 6 maanden meer dan 20.000

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Op beschikbare seats

Top 10 klanten op basis van beschikbare seats in de afgelopen maand

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Partnerprofiel

Deze voorbeeldquery's zijn van toepassing op het partnerprofielrapport:

### <a name="by-geography"></a>Op geografische locatie

Lijst met partners uit een specifieke geografie.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Door MPN-partner

Lijst met partners onder dezelfde PGA MPN-partner

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Resellerprestaties

Deze voorbeeldquery's zijn van toepassing op het prestatierapport van de reseller:

### <a name="by-geography"></a>Op geografische locatie

Lijst met resellers van een specifieke geografie in de afgelopen maand.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Per reseller

Aantal klanten, aantal abonnementen, totale beschikbare seats, totaal aantal toegewezen seats, totale omzet voor een specifieke reseller.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>Top 10 op omzet

Top 10 resellers op basis van de totale omzet in de afgelopen maand.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Abonnementsgegevens

Deze voorbeeldquery's zijn van toepassing op het rapport met abonnementsdetails:

### <a name="by-renewal-eligibility"></a>Door geschiktheid voor verlenging

Lijst met abonnementen die niet in aanmerking komen voor automatische verlenging in de afgelopen maand.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Op abonnementsstaat

Lijst met abonnementen met de status Uitschakelen in de afgelopen maand.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Tellingen voor zes maanden

Aantal abonnementen, totaal aantal verkochte seats, klanttelling voor een specifieke partner in de afgelopen zes maanden.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Azure-gebruik

Deze voorbeeldquery's zijn van toepassing op het Azure-gebruiksrapport:

### <a name="by-meter-category"></a>Per metercategorie

Lijst met Azure-gebruiksabonnementen met gebruikseenheden en ACR voor specifieke metercategorie in de afgelopen zes maanden.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Op totaal ACR

Lijst met Azure-gebruiksabonnementen waarbij de totale ACR de afgelopen zes maanden hoger is dan 20.000

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Volgende stappen

- [API's voor toegang tot analysegegevens van partnerinzichten](insights-programmatic-analytics-available-api.md)