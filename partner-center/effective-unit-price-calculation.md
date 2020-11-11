---
title: Prijs berekening effectief eenheid
ms.topic: how-to
ms.date: 11/10/2020
description: Meer informatie over de werkelijke prijs eenheid en hoe deze worden berekend. Bevat een voor beeld van een berekening.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94499138"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="0d679-104">Efficiënte eenheid prijs berekening voor het verbruik van het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="0d679-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="0d679-105">De werkelijke eenheids prijs</span><span class="sxs-lookup"><span data-stu-id="0d679-105">The effective unit price</span></span>

<span data-ttu-id="0d679-106">De werkelijke eenheids prijs wordt berekend op het niveau van de meter (in plaats van het resource niveau) en wordt dagelijks aangepast op basis van het gebruik van metingen.</span><span class="sxs-lookup"><span data-stu-id="0d679-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="0d679-107">De werkelijke eenheids prijs wordt berekend aan de hand van de volgende drie factoren:</span><span class="sxs-lookup"><span data-stu-id="0d679-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="0d679-108">Verbruik, dat dagelijks wordt bewaakt tijdens de facturerings cyclus</span><span class="sxs-lookup"><span data-stu-id="0d679-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="0d679-109">Factureer bare kosten voor de meter</span><span class="sxs-lookup"><span data-stu-id="0d679-109">Billable cost for the meter</span></span>
- <span data-ttu-id="0d679-110">Trapsgewijs scha kelen (indien van toepassing)</span><span class="sxs-lookup"><span data-stu-id="0d679-110">Tiering (if applicable)</span></span>

<span data-ttu-id="0d679-111">Omdat we dagelijks het verbruik in de facturerings cyclus controleren, schommelt de werkelijke eenheids prijs.</span><span class="sxs-lookup"><span data-stu-id="0d679-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="0d679-112">De uiteindelijke prijs voor een bepaalde facturerings cyclus is beschikbaar nadat de verbruiks berekening is gestopt en de facturerings periode is gesloten.</span><span class="sxs-lookup"><span data-stu-id="0d679-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="0d679-113">U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimaal positie.</span><span class="sxs-lookup"><span data-stu-id="0d679-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="0d679-114">Nagaan of uw meter gelaagde prijzen gebruikt</span><span class="sxs-lookup"><span data-stu-id="0d679-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="0d679-115">Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen.</span><span class="sxs-lookup"><span data-stu-id="0d679-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="0d679-116">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0d679-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="0d679-117">Selecteer **verkopen** , selecteer **prijzen en aanbiedingen** en selecteer vervolgens de **prijs** van het Azure-abonnement.</span><span class="sxs-lookup"><span data-stu-id="0d679-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="0d679-118">Zoek uw meter op ID en down load de prijs gegevens.</span><span class="sxs-lookup"><span data-stu-id="0d679-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="0d679-119">Voorbeeld berekening</span><span class="sxs-lookup"><span data-stu-id="0d679-119">Sample calculation</span></span>

<span data-ttu-id="0d679-120">De onderstaande tabel geeft een voor beeld van hoe we de werkelijke eenheids prijs berekenen tijdens de open periode.</span><span class="sxs-lookup"><span data-stu-id="0d679-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="0d679-121">De volgende waarden zijn van toepassing in de tabel:</span><span class="sxs-lookup"><span data-stu-id="0d679-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="0d679-122">**Up** = eenheids prijs van resource/uur = 0,868</span><span class="sxs-lookup"><span data-stu-id="0d679-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="0d679-123">**BCU** = factureer bare verbruiks eenheid voor de meter</span><span class="sxs-lookup"><span data-stu-id="0d679-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="0d679-124">**BC** = factureer bare kosten voor de meter = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="0d679-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="0d679-125">Dit weerspiegelt een aanpassing voor de PEC-korting van 15%.</span><span class="sxs-lookup"><span data-stu-id="0d679-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="0d679-126">Vervolgens gebruiken we de ondergrens van de functie om de waarde te beperken tot twee cijfers na het decimaal teken, zodat de minimum hoeveelheid kan worden gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="0d679-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="0d679-127">**Werkelijke eenheids prijs** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="0d679-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="0d679-128">Opmerking: de meter in dit voor beeld heeft geen lagen voor de prijzen.</span><span class="sxs-lookup"><span data-stu-id="0d679-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="0d679-129">Datum</span><span class="sxs-lookup"><span data-stu-id="0d679-129">Date</span></span> | <span data-ttu-id="0d679-130">BCU (factureer bare verbruiks eenheid)</span><span class="sxs-lookup"><span data-stu-id="0d679-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="0d679-131">BC (factureer bare kosten)</span><span class="sxs-lookup"><span data-stu-id="0d679-131">BC (Billable cost)</span></span> | <span data-ttu-id="0d679-132">Werkelijke eenheids prijs</span><span class="sxs-lookup"><span data-stu-id="0d679-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="0d679-133">3-aug</span><span class="sxs-lookup"><span data-stu-id="0d679-133">3-Aug</span></span> | <span data-ttu-id="0d679-134">29</span><span class="sxs-lookup"><span data-stu-id="0d679-134">29</span></span> | <span data-ttu-id="0d679-135">21,39</span><span class="sxs-lookup"><span data-stu-id="0d679-135">21.39</span></span> | <span data-ttu-id="0d679-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="0d679-136">0.737586206896552</span></span> |
| <span data-ttu-id="0d679-137">10-aug</span><span class="sxs-lookup"><span data-stu-id="0d679-137">10-Aug</span></span> | <span data-ttu-id="0d679-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="0d679-138">210.950039</span></span> | <span data-ttu-id="0d679-139">155,63</span><span class="sxs-lookup"><span data-stu-id="0d679-139">155.63</span></span> | <span data-ttu-id="0d679-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="0d679-140">0.737757626107858</span></span> |
| <span data-ttu-id="0d679-141">25-aug</span><span class="sxs-lookup"><span data-stu-id="0d679-141">25-Aug</span></span> | <span data-ttu-id="0d679-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="0d679-142">555.950039</span></span> | <span data-ttu-id="0d679-143">410,17</span><span class="sxs-lookup"><span data-stu-id="0d679-143">410.17</span></span> | <span data-ttu-id="0d679-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="0d679-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="0d679-145">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="0d679-145">Next steps</span></span>

- [<span data-ttu-id="0d679-146">Facturering en belastingen</span><span class="sxs-lookup"><span data-stu-id="0d679-146">Billing and taxes</span></span>](billing.md)
