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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172214"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="044f1-104">Berekening van de effectieve eenheidsprijs voor azure-planverbruik</span><span class="sxs-lookup"><span data-stu-id="044f1-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="044f1-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="044f1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="044f1-106">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="044f1-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="044f1-107">De effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="044f1-107">The effective unit price</span></span>

<span data-ttu-id="044f1-108">De effectieve eenheidsprijs wordt berekend op meterniveau (in tegenstelling tot het resourceniveau) en wordt dagelijks aangepast op basis van het metergebruik.</span><span class="sxs-lookup"><span data-stu-id="044f1-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="044f1-109">We berekenen de effectieve eenheidsprijs aan de hand van de volgende drie factoren:</span><span class="sxs-lookup"><span data-stu-id="044f1-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="044f1-110">Verbruik, dat dagelijks wordt bewaakt gedurende de factureringscyclus</span><span class="sxs-lookup"><span data-stu-id="044f1-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="044f1-111">Factureerbare kosten voor de meter</span><span class="sxs-lookup"><span data-stu-id="044f1-111">Billable cost for the meter</span></span>
- <span data-ttu-id="044f1-112">Lagen (indien van toepassing)</span><span class="sxs-lookup"><span data-stu-id="044f1-112">Tiering (if applicable)</span></span>

<span data-ttu-id="044f1-113">Omdat we het verbruik dagelijks bewaken gedurende de factureringscyclus, zal de effectieve eenheidsprijs fluctueren.</span><span class="sxs-lookup"><span data-stu-id="044f1-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="044f1-114">De uiteindelijke prijs voor een bepaalde factureringscyclus is beschikbaar nadat we de verbruiksberekening hebben gestopt en de factureringsperiode hebben gesloten.</span><span class="sxs-lookup"><span data-stu-id="044f1-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="044f1-115">U ziet de meeste wijzigingen in het verbruik na de vierde of vijfde decimale plaats.</span><span class="sxs-lookup"><span data-stu-id="044f1-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="044f1-116">Uitzoeken of voor uw meter gelaagde prijzen worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="044f1-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="044f1-117">Als u niet weet of uw meter gelaagde prijzen gebruikt, gebruikt u de onderstaande procedure om erachter te komen.</span><span class="sxs-lookup"><span data-stu-id="044f1-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="044f1-118">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="044f1-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="044f1-119">Selecteer **Verkopen,** selecteer **Prijzen en aanbiedingen** en selecteer vervolgens Prijzen voor **Azure-abonnement.**</span><span class="sxs-lookup"><span data-stu-id="044f1-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="044f1-120">Zoek uw meter op id en download vervolgens uw prijsgegevens.</span><span class="sxs-lookup"><span data-stu-id="044f1-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="044f1-121">Voorbeeldberekening</span><span class="sxs-lookup"><span data-stu-id="044f1-121">Sample calculation</span></span>

<span data-ttu-id="044f1-122">De onderstaande tabel geeft een voorbeeld van hoe we de effectieve eenheidsprijs berekenen tijdens de open periode.</span><span class="sxs-lookup"><span data-stu-id="044f1-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="044f1-123">In de tabel zijn de volgende waarden van toepassing:</span><span class="sxs-lookup"><span data-stu-id="044f1-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="044f1-124">**UP** = Eenheidsprijs van de resource/uur = 0,868</span><span class="sxs-lookup"><span data-stu-id="044f1-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="044f1-125">**BCU** = Factureerbare verbruikseenheid voor de meter</span><span class="sxs-lookup"><span data-stu-id="044f1-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="044f1-126">**BC** = Factureerbare kosten voor de meter = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="044f1-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="044f1-127">Dit weerspiegelt een aanpassing voor de PEC-korting van 15%.</span><span class="sxs-lookup"><span data-stu-id="044f1-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="044f1-128">Vervolgens gebruiken we de onderste limiet van de functie om de waarde te beperken tot twee cijfers achter het decimaalteken om het minimumbedrag in rekening te brengen.</span><span class="sxs-lookup"><span data-stu-id="044f1-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="044f1-129">**Effectieve eenheidsprijs** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="044f1-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="044f1-130">Opmerking: De meter in dit voorbeeld heeft geen prijscategorie of andere kortingen: de effectieve eenheidsprijs houdt rekening met kortingspercentages en andere aanpassingen.</span><span class="sxs-lookup"><span data-stu-id="044f1-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="044f1-131">Datum</span><span class="sxs-lookup"><span data-stu-id="044f1-131">Date</span></span> | <span data-ttu-id="044f1-132">BCU (factureerbare verbruikseenheid)</span><span class="sxs-lookup"><span data-stu-id="044f1-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="044f1-133">BC (factureerbare kosten)</span><span class="sxs-lookup"><span data-stu-id="044f1-133">BC (Billable cost)</span></span> | <span data-ttu-id="044f1-134">Effectieve eenheidsprijs</span><span class="sxs-lookup"><span data-stu-id="044f1-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="044f1-135">3 aug</span><span class="sxs-lookup"><span data-stu-id="044f1-135">3-Aug</span></span> | <span data-ttu-id="044f1-136">29</span><span class="sxs-lookup"><span data-stu-id="044f1-136">29</span></span> | <span data-ttu-id="044f1-137">21.39</span><span class="sxs-lookup"><span data-stu-id="044f1-137">21.39</span></span> | <span data-ttu-id="044f1-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="044f1-138">0.737586206896552</span></span> |
| <span data-ttu-id="044f1-139">10 aug</span><span class="sxs-lookup"><span data-stu-id="044f1-139">10-Aug</span></span> | <span data-ttu-id="044f1-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="044f1-140">210.950039</span></span> | <span data-ttu-id="044f1-141">155.63</span><span class="sxs-lookup"><span data-stu-id="044f1-141">155.63</span></span> | <span data-ttu-id="044f1-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="044f1-142">0.737757626107858</span></span> |
| <span data-ttu-id="044f1-143">25 aug</span><span class="sxs-lookup"><span data-stu-id="044f1-143">25-Aug</span></span> | <span data-ttu-id="044f1-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="044f1-144">555.950039</span></span> | <span data-ttu-id="044f1-145">410.17</span><span class="sxs-lookup"><span data-stu-id="044f1-145">410.17</span></span> | <span data-ttu-id="044f1-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="044f1-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="044f1-147">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="044f1-147">Next steps</span></span>

- [<span data-ttu-id="044f1-148">Facturering en belastingen</span><span class="sxs-lookup"><span data-stu-id="044f1-148">Billing and taxes</span></span>](billing.md)
