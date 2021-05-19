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
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147119"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="0dabd-104">Berekening van de effectieve eenheidsprijs voor azure-planverbruik</span><span class="sxs-lookup"><span data-stu-id="0dabd-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="0dabd-105">**Juiste rollen:** Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="0dabd-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="0dabd-106">De effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="0dabd-106">The effective unit price</span></span>

<span data-ttu-id="0dabd-107">De effectieve eenheidsprijs wordt berekend op meterniveau (in tegenstelling tot het resourceniveau) en wordt dagelijks aangepast op basis van het metergebruik.</span><span class="sxs-lookup"><span data-stu-id="0dabd-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="0dabd-108">We berekenen de effectieve eenheidsprijs aan de hand van de volgende drie factoren:</span><span class="sxs-lookup"><span data-stu-id="0dabd-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="0dabd-109">Verbruik, dat dagelijks wordt bewaakt gedurende de factureringscyclus</span><span class="sxs-lookup"><span data-stu-id="0dabd-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="0dabd-110">Factureerbare kosten voor de meter</span><span class="sxs-lookup"><span data-stu-id="0dabd-110">Billable cost for the meter</span></span>
- <span data-ttu-id="0dabd-111">Lagen (indien van toepassing)</span><span class="sxs-lookup"><span data-stu-id="0dabd-111">Tiering (if applicable)</span></span>

<span data-ttu-id="0dabd-112">Omdat we het verbruik dagelijks bewaken gedurende de factureringscyclus, zal de effectieve eenheidsprijs fluctueren.</span><span class="sxs-lookup"><span data-stu-id="0dabd-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="0dabd-113">De uiteindelijke prijs voor een bepaalde factureringscyclus is beschikbaar nadat we de verbruiksberekening hebben gestopt en de factureringsperiode hebben gesloten.</span><span class="sxs-lookup"><span data-stu-id="0dabd-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="0dabd-114">U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimale plaats.</span><span class="sxs-lookup"><span data-stu-id="0dabd-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="0dabd-115">Uitzoeken of voor uw meter gelaagde prijzen worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="0dabd-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="0dabd-116">Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen.</span><span class="sxs-lookup"><span data-stu-id="0dabd-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="0dabd-117">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="0dabd-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="0dabd-118">Selecteer **Verkopen,** selecteer **Prijzen en aanbiedingen** en selecteer vervolgens Prijzen voor **Azure-abonnement.**</span><span class="sxs-lookup"><span data-stu-id="0dabd-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="0dabd-119">Zoek uw meter op id en download vervolgens uw prijsgegevens.</span><span class="sxs-lookup"><span data-stu-id="0dabd-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="0dabd-120">Voorbeeldberekening</span><span class="sxs-lookup"><span data-stu-id="0dabd-120">Sample calculation</span></span>

<span data-ttu-id="0dabd-121">De onderstaande tabel geeft een voorbeeld van hoe we de effectieve eenheidsprijs berekenen tijdens de open periode.</span><span class="sxs-lookup"><span data-stu-id="0dabd-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="0dabd-122">In de tabel zijn de volgende waarden van toepassing:</span><span class="sxs-lookup"><span data-stu-id="0dabd-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="0dabd-123">**UP** = Eenheidsprijs van de resource/uur = 0,868</span><span class="sxs-lookup"><span data-stu-id="0dabd-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="0dabd-124">**BCU** = Factureerbare verbruikseenheid voor de meter</span><span class="sxs-lookup"><span data-stu-id="0dabd-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="0dabd-125">**BC** = Factureerbare kosten voor de meter = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="0dabd-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="0dabd-126">Dit weerspiegelt een aanpassing voor de PEC-korting van 15%.</span><span class="sxs-lookup"><span data-stu-id="0dabd-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="0dabd-127">Vervolgens gebruiken we de onderste limiet van de functie om de waarde te beperken tot twee cijfers achter het decimaalteken om het minimumbedrag in rekening te brengen.</span><span class="sxs-lookup"><span data-stu-id="0dabd-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="0dabd-128">**Effectieve eenheidsprijs** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="0dabd-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="0dabd-129">Opmerking: De meter in dit voorbeeld heeft geen prijscategorie of andere kortingen: de effectieve eenheidsprijs houdt rekening met kortingspercentages en andere aanpassingen.</span><span class="sxs-lookup"><span data-stu-id="0dabd-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="0dabd-130">Datum</span><span class="sxs-lookup"><span data-stu-id="0dabd-130">Date</span></span> | <span data-ttu-id="0dabd-131">BCU (factureerbare verbruikseenheid)</span><span class="sxs-lookup"><span data-stu-id="0dabd-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="0dabd-132">BC (factureerbare kosten)</span><span class="sxs-lookup"><span data-stu-id="0dabd-132">BC (Billable cost)</span></span> | <span data-ttu-id="0dabd-133">Effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="0dabd-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="0dabd-134">3 aug</span><span class="sxs-lookup"><span data-stu-id="0dabd-134">3-Aug</span></span> | <span data-ttu-id="0dabd-135">29</span><span class="sxs-lookup"><span data-stu-id="0dabd-135">29</span></span> | <span data-ttu-id="0dabd-136">21.39</span><span class="sxs-lookup"><span data-stu-id="0dabd-136">21.39</span></span> | <span data-ttu-id="0dabd-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="0dabd-137">0.737586206896552</span></span> |
| <span data-ttu-id="0dabd-138">10 aug</span><span class="sxs-lookup"><span data-stu-id="0dabd-138">10-Aug</span></span> | <span data-ttu-id="0dabd-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="0dabd-139">210.950039</span></span> | <span data-ttu-id="0dabd-140">155.63</span><span class="sxs-lookup"><span data-stu-id="0dabd-140">155.63</span></span> | <span data-ttu-id="0dabd-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="0dabd-141">0.737757626107858</span></span> |
| <span data-ttu-id="0dabd-142">25 aug</span><span class="sxs-lookup"><span data-stu-id="0dabd-142">25-Aug</span></span> | <span data-ttu-id="0dabd-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="0dabd-143">555.950039</span></span> | <span data-ttu-id="0dabd-144">410.17</span><span class="sxs-lookup"><span data-stu-id="0dabd-144">410.17</span></span> | <span data-ttu-id="0dabd-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="0dabd-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="0dabd-146">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="0dabd-146">Next steps</span></span>

- [<span data-ttu-id="0dabd-147">Facturering en belastingen</span><span class="sxs-lookup"><span data-stu-id="0dabd-147">Billing and taxes</span></span>](billing.md)
