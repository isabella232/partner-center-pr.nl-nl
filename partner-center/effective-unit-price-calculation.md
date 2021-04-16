---
title: Effectieve berekening van eenheidsprijs
ms.topic: how-to
ms.date: 04/02/2021
description: Meer informatie over de effectieve eenheidsprijs en hoe deze wordt berekend. Dit artikel bevat ook een voorbeeldberekening.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c3c3a672de015c9f38fa0e34232da8d9913177c
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528563"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="51e20-104">Berekening van de effectieve eenheidsprijs voor azure-planverbruik</span><span class="sxs-lookup"><span data-stu-id="51e20-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="51e20-105">De effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="51e20-105">The effective unit price</span></span>

<span data-ttu-id="51e20-106">De effectieve eenheidsprijs wordt berekend op meterniveau (in tegenstelling tot het resourceniveau) en wordt dagelijks aangepast op basis van metergebruik.</span><span class="sxs-lookup"><span data-stu-id="51e20-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="51e20-107">We berekenen de effectieve eenheidsprijs aan de hand van de volgende drie factoren:</span><span class="sxs-lookup"><span data-stu-id="51e20-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="51e20-108">Verbruik, dat dagelijks wordt bewaakt gedurende de factureringscyclus</span><span class="sxs-lookup"><span data-stu-id="51e20-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="51e20-109">Factureerbare kosten voor de meter</span><span class="sxs-lookup"><span data-stu-id="51e20-109">Billable cost for the meter</span></span>
- <span data-ttu-id="51e20-110">Lagen (indien van toepassing)</span><span class="sxs-lookup"><span data-stu-id="51e20-110">Tiering (if applicable)</span></span>

<span data-ttu-id="51e20-111">Omdat we het verbruik dagelijks bewaken gedurende de factureringscyclus, zal de effectieve eenheidsprijs fluctueren.</span><span class="sxs-lookup"><span data-stu-id="51e20-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="51e20-112">De uiteindelijke prijs voor een bepaalde factureringscyclus is beschikbaar nadat we de verbruiksberekening hebben gestopt en de factureringsperiode hebben gesloten.</span><span class="sxs-lookup"><span data-stu-id="51e20-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="51e20-113">U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimale plaats.</span><span class="sxs-lookup"><span data-stu-id="51e20-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="51e20-114">Uitzoeken of voor uw meter gelaagde prijzen worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="51e20-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="51e20-115">Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen.</span><span class="sxs-lookup"><span data-stu-id="51e20-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="51e20-116">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="51e20-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="51e20-117">Selecteer **Verkopen,** selecteer **Prijzen en aanbiedingen** en selecteer vervolgens Prijzen voor **Azure-abonnement.**</span><span class="sxs-lookup"><span data-stu-id="51e20-117">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="51e20-118">Zoek uw meter op id en download vervolgens uw prijsgegevens.</span><span class="sxs-lookup"><span data-stu-id="51e20-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="51e20-119">Voorbeeldberekening</span><span class="sxs-lookup"><span data-stu-id="51e20-119">Sample calculation</span></span>

<span data-ttu-id="51e20-120">De onderstaande tabel geeft een voorbeeld van hoe we de effectieve eenheidsprijs berekenen tijdens de open periode.</span><span class="sxs-lookup"><span data-stu-id="51e20-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="51e20-121">In de tabel zijn de volgende waarden van toepassing:</span><span class="sxs-lookup"><span data-stu-id="51e20-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="51e20-122">**UP** = Eenheidsprijs van de resource/uur = 0,868</span><span class="sxs-lookup"><span data-stu-id="51e20-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="51e20-123">**BCU** = Factureerbare verbruikseenheid voor de meter</span><span class="sxs-lookup"><span data-stu-id="51e20-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="51e20-124">**BC** = Factureerbare kosten voor de meter = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="51e20-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="51e20-125">Dit weerspiegelt een aanpassing voor de PEC-korting van 15%.</span><span class="sxs-lookup"><span data-stu-id="51e20-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="51e20-126">Vervolgens gebruiken we de onderste limiet van de functie om de waarde te beperken tot twee cijfers achter het decimaalteken om het minimumbedrag in rekening te brengen.</span><span class="sxs-lookup"><span data-stu-id="51e20-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="51e20-127">**Effectieve eenheidsprijs** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="51e20-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="51e20-128">Opmerking: De meter in dit voorbeeld heeft geen prijscategorie of andere kortingen: de effectieve eenheidsprijs houdt rekening met kortingspercentages en andere aanpassingen.</span><span class="sxs-lookup"><span data-stu-id="51e20-128">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="51e20-129">Datum</span><span class="sxs-lookup"><span data-stu-id="51e20-129">Date</span></span> | <span data-ttu-id="51e20-130">BCU (factureerbare verbruikseenheid)</span><span class="sxs-lookup"><span data-stu-id="51e20-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="51e20-131">BC (factureerbare kosten)</span><span class="sxs-lookup"><span data-stu-id="51e20-131">BC (Billable cost)</span></span> | <span data-ttu-id="51e20-132">Effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="51e20-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="51e20-133">3 aug</span><span class="sxs-lookup"><span data-stu-id="51e20-133">3-Aug</span></span> | <span data-ttu-id="51e20-134">29</span><span class="sxs-lookup"><span data-stu-id="51e20-134">29</span></span> | <span data-ttu-id="51e20-135">21.39</span><span class="sxs-lookup"><span data-stu-id="51e20-135">21.39</span></span> | <span data-ttu-id="51e20-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="51e20-136">0.737586206896552</span></span> |
| <span data-ttu-id="51e20-137">10 aug</span><span class="sxs-lookup"><span data-stu-id="51e20-137">10-Aug</span></span> | <span data-ttu-id="51e20-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="51e20-138">210.950039</span></span> | <span data-ttu-id="51e20-139">155.63</span><span class="sxs-lookup"><span data-stu-id="51e20-139">155.63</span></span> | <span data-ttu-id="51e20-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="51e20-140">0.737757626107858</span></span> |
| <span data-ttu-id="51e20-141">25 aug</span><span class="sxs-lookup"><span data-stu-id="51e20-141">25-Aug</span></span> | <span data-ttu-id="51e20-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="51e20-142">555.950039</span></span> | <span data-ttu-id="51e20-143">410.17</span><span class="sxs-lookup"><span data-stu-id="51e20-143">410.17</span></span> | <span data-ttu-id="51e20-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="51e20-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="51e20-145">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="51e20-145">Next steps</span></span>

- [<span data-ttu-id="51e20-146">Facturering en belastingen</span><span class="sxs-lookup"><span data-stu-id="51e20-146">Billing and taxes</span></span>](billing.md)
