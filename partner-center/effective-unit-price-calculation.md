---
title: Effectieve berekening van eenheidsprijs
ms.topic: how-to
ms.date: 11/10/2020
description: Meer informatie over de werkelijke eenheids prijs en hoe deze worden berekend. Dit artikel bevat ook een voor beeld van een berekening.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556324"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="2f8fd-104">Efficiënte eenheid prijs berekening voor het verbruik van het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="2f8fd-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="2f8fd-105">De werkelijke eenheids prijs</span><span class="sxs-lookup"><span data-stu-id="2f8fd-105">The effective unit price</span></span>

<span data-ttu-id="2f8fd-106">De werkelijke eenheids prijs wordt berekend op het niveau van de meter (in plaats van het resource niveau) en wordt dagelijks aangepast op basis van het gebruik van metingen.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="2f8fd-107">De werkelijke eenheids prijs wordt berekend aan de hand van de volgende drie factoren:</span><span class="sxs-lookup"><span data-stu-id="2f8fd-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="2f8fd-108">Verbruik, dat dagelijks wordt bewaakt tijdens de facturerings cyclus</span><span class="sxs-lookup"><span data-stu-id="2f8fd-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="2f8fd-109">Factureer bare kosten voor de meter</span><span class="sxs-lookup"><span data-stu-id="2f8fd-109">Billable cost for the meter</span></span>
- <span data-ttu-id="2f8fd-110">Trapsgewijs scha kelen (indien van toepassing)</span><span class="sxs-lookup"><span data-stu-id="2f8fd-110">Tiering (if applicable)</span></span>

<span data-ttu-id="2f8fd-111">Omdat we dagelijks het verbruik in de facturerings cyclus controleren, schommelt de werkelijke eenheids prijs.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="2f8fd-112">De uiteindelijke prijs voor een bepaalde facturerings cyclus is beschikbaar nadat de verbruiks berekening is gestopt en de facturerings periode is gesloten.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="2f8fd-113">U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimaal positie.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="2f8fd-114">Nagaan of uw meter gelaagde prijzen gebruikt</span><span class="sxs-lookup"><span data-stu-id="2f8fd-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="2f8fd-115">Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="2f8fd-116">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="2f8fd-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="2f8fd-117">Selecteer **verkopen**, selecteer **prijzen en aanbiedingen** en selecteer vervolgens de **prijs** van het Azure-abonnement.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="2f8fd-118">Zoek uw meter op ID en down load de prijs gegevens.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="2f8fd-119">Voorbeeld berekening</span><span class="sxs-lookup"><span data-stu-id="2f8fd-119">Sample calculation</span></span>

<span data-ttu-id="2f8fd-120">De onderstaande tabel geeft een voor beeld van hoe we de werkelijke eenheids prijs berekenen tijdens de open periode.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="2f8fd-121">De volgende waarden zijn van toepassing in de tabel:</span><span class="sxs-lookup"><span data-stu-id="2f8fd-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="2f8fd-122">**Up** = eenheids prijs van resource/uur = 0,868</span><span class="sxs-lookup"><span data-stu-id="2f8fd-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="2f8fd-123">**BCU** = factureer bare verbruiks eenheid voor de meter</span><span class="sxs-lookup"><span data-stu-id="2f8fd-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="2f8fd-124">**BC** = factureer bare kosten voor de meter = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="2f8fd-125">Dit weerspiegelt een aanpassing voor de PEC-korting van 15%.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="2f8fd-126">Vervolgens gebruiken we de ondergrens van de functie om de waarde te beperken tot twee cijfers na het decimaal teken, zodat de minimum hoeveelheid kan worden gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="2f8fd-127">**Werkelijke eenheids prijs** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="2f8fd-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="2f8fd-128">Opmerking: de meter in dit voor beeld heeft geen lagen voor de prijzen.</span><span class="sxs-lookup"><span data-stu-id="2f8fd-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="2f8fd-129">Date</span><span class="sxs-lookup"><span data-stu-id="2f8fd-129">Date</span></span> | <span data-ttu-id="2f8fd-130">BCU (factureer bare verbruiks eenheid)</span><span class="sxs-lookup"><span data-stu-id="2f8fd-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="2f8fd-131">BC (factureer bare kosten)</span><span class="sxs-lookup"><span data-stu-id="2f8fd-131">BC (Billable cost)</span></span> | <span data-ttu-id="2f8fd-132">Werkelijke eenheids prijs</span><span class="sxs-lookup"><span data-stu-id="2f8fd-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="2f8fd-133">3-aug</span><span class="sxs-lookup"><span data-stu-id="2f8fd-133">3-Aug</span></span> | <span data-ttu-id="2f8fd-134">29</span><span class="sxs-lookup"><span data-stu-id="2f8fd-134">29</span></span> | <span data-ttu-id="2f8fd-135">21,39</span><span class="sxs-lookup"><span data-stu-id="2f8fd-135">21.39</span></span> | <span data-ttu-id="2f8fd-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="2f8fd-136">0.737586206896552</span></span> |
| <span data-ttu-id="2f8fd-137">10-aug</span><span class="sxs-lookup"><span data-stu-id="2f8fd-137">10-Aug</span></span> | <span data-ttu-id="2f8fd-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="2f8fd-138">210.950039</span></span> | <span data-ttu-id="2f8fd-139">155,63</span><span class="sxs-lookup"><span data-stu-id="2f8fd-139">155.63</span></span> | <span data-ttu-id="2f8fd-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="2f8fd-140">0.737757626107858</span></span> |
| <span data-ttu-id="2f8fd-141">25-aug</span><span class="sxs-lookup"><span data-stu-id="2f8fd-141">25-Aug</span></span> | <span data-ttu-id="2f8fd-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="2f8fd-142">555.950039</span></span> | <span data-ttu-id="2f8fd-143">410,17</span><span class="sxs-lookup"><span data-stu-id="2f8fd-143">410.17</span></span> | <span data-ttu-id="2f8fd-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="2f8fd-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="2f8fd-145">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="2f8fd-145">Next steps</span></span>

- [<span data-ttu-id="2f8fd-146">Facturering en belastingen</span><span class="sxs-lookup"><span data-stu-id="2f8fd-146">Billing and taxes</span></span>](billing.md)
