---
title: Kosten typen van het afstemmings bestand
ms.topic: article
ms.date: 06/05/2020
description: Ontdek de typen kosten (zoals, op gebruik gebaseerde en eenmalige), tegoeden en kortingen in Partner Center-afstemmings bestanden.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/31/2020
ms.locfileid: "92527572"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="a154b-103">Meer informatie over de verschillende kosten typen in Partner Center reconciliatie bestanden</span><span class="sxs-lookup"><span data-stu-id="a154b-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="a154b-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="a154b-104">**Applies to**</span></span>

- <span data-ttu-id="a154b-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="a154b-105">Partner Center</span></span>
- <span data-ttu-id="a154b-106">Partner centrum voor Microsoft Cloud voor de Amerikaanse overheid</span><span class="sxs-lookup"><span data-stu-id="a154b-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a154b-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="a154b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="a154b-108">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="a154b-108">Admin agent</span></span>
- <span data-ttu-id="a154b-109">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="a154b-109">Billing admin</span></span>
- <span data-ttu-id="a154b-110">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="a154b-110">Global admin</span></span>

<span data-ttu-id="a154b-111">In dit onderwerp vindt u een beschrijving van de toewijzingen tussen een factuur gedeelte en gekoppelde kosten typen die mogelijk in uw afstemmings bestand staan.</span><span class="sxs-lookup"><span data-stu-id="a154b-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="a154b-112">Uw factuur bevat een samen vatting van de kosten.</span><span class="sxs-lookup"><span data-stu-id="a154b-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="a154b-113">Uw afstemmings bestand bevat een gedetailleerde verdeling van trans acties met regel items, inclusief kosten typen.</span><span class="sxs-lookup"><span data-stu-id="a154b-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="a154b-114">Zie [reconciliatie bestanden gebruiken](use-the-reconciliation-files.md)voor meer informatie over het afstemmen van bestanden.</span><span class="sxs-lookup"><span data-stu-id="a154b-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="a154b-115">Zowel [afstemmings bestanden op basis van gebruik](usage-based-recon-files.md) en [afstemmings bestanden op basis van een licentie](license-based-recon-files.md) geven alleen gebruiks gerelateerde trans acties en kosten (verbruikte eenheden en gerelateerde kosten) weer.</span><span class="sxs-lookup"><span data-stu-id="a154b-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="a154b-116">Eenmalige kredieten, kortingen of terugstortingen die worden weer gegeven op de factuur als **aanpassingen** , worden niet weer gegeven in het afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="a154b-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="a154b-117">Kosten typen toewijzen aan facturerings kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="a154b-118">Gebruik de filter opties in micro soft Excel om de bedragen te verdelen tussen uw factuur-en afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="a154b-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="a154b-119">Filter op kosten typen in het afstemmings bestand om de kosten van de factuur toe te wijzen aan een set toeslag uitsplitsingen in het afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="a154b-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="a154b-120">Kosten op basis van licenties</span><span class="sxs-lookup"><span data-stu-id="a154b-120">License-based charges</span></span>

<span data-ttu-id="a154b-121">Als u deze kosten op basis van licenties aan uw factuur wilt toewijzen, moet u de kolom **bedrag** in het bestand op basis van licentie optellen.</span><span class="sxs-lookup"><span data-stu-id="a154b-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="a154b-122">Beschrijving van kosten (kolom ChargeType in afstemmings bestand)</span><span class="sxs-lookup"><span data-stu-id="a154b-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="a154b-123">Uitleg bij kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="a154b-124">Activerings kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-124">Activation fee</span></span> | <span data-ttu-id="a154b-125">De hoeveelheid die bij de klant in rekening wordt gebracht wanneer deze na de aankoop gebruikmaakt van het abonnement.</span><span class="sxs-lookup"><span data-stu-id="a154b-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="a154b-126">Annulerings kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-126">Cancel fee</span></span> | <span data-ttu-id="a154b-127">Gefactureerde kosten worden aan de klant gerestitueerd wanneer de gekoppelde licenties worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a154b-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="a154b-128">Exemplaar van prorente annuleren</span><span class="sxs-lookup"><span data-stu-id="a154b-128">Cancel instance prorate</span></span> | <span data-ttu-id="a154b-129">Gefactureerde kosten worden geannuleerd wanneer de klant met een maandelijks abonnement abonnementen heeft opgeschort en de bijbehorende licenties zijn gewijzigd binnen dezelfde maand.</span><span class="sxs-lookup"><span data-stu-id="a154b-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="a154b-130">Cyclus kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-130">Cycle fee</span></span> | <span data-ttu-id="a154b-131">Periodieke kosten voor een abonnement.</span><span class="sxs-lookup"><span data-stu-id="a154b-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="a154b-132">Cyclus exemplaar prorente</span><span class="sxs-lookup"><span data-stu-id="a154b-132">Cycle instance prorate</span></span> | <span data-ttu-id="a154b-133">De geraamde kosten die van de klant worden berekend wanneer de gekoppelde licenties worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a154b-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="a154b-134">Tarief vergoedingen wanneer annuleren</span><span class="sxs-lookup"><span data-stu-id="a154b-134">Prorate fees when cancel</span></span> | <span data-ttu-id="a154b-135">Gefactureerde restitutie voor ongebruikt servicef onderdeel na annulering.</span><span class="sxs-lookup"><span data-stu-id="a154b-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="a154b-136">Kosten evenredigheid bij het converteren van de huidige aanbieding</span><span class="sxs-lookup"><span data-stu-id="a154b-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="a154b-137">Gefactureerde kosten na de conversie van het huidige maandelijkse abonnement op een jaar abonnement.</span><span class="sxs-lookup"><span data-stu-id="a154b-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="a154b-138">Kosten per tarief bij conversie naar een nieuwe aanbieding</span><span class="sxs-lookup"><span data-stu-id="a154b-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="a154b-139">Gefactureerde kosten nadat een maandelijks abonnement is geconverteerd naar een nieuw jaarlijks abonnement.</span><span class="sxs-lookup"><span data-stu-id="a154b-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="a154b-140">Tarief vergoedingen bij aankoop</span><span class="sxs-lookup"><span data-stu-id="a154b-140">Prorate fees when purchase</span></span> | <span data-ttu-id="a154b-141">Het type kosten voor een abonnement bij het gebruik van zowel maandelijkse als jaarlijkse facturering.</span><span class="sxs-lookup"><span data-stu-id="a154b-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="a154b-142">Tarief vergoeding bij verlenging</span><span class="sxs-lookup"><span data-stu-id="a154b-142">Prorate fee when renew</span></span> | <span data-ttu-id="a154b-143">Gefactureerde kosten bij het verlengen van het abonnement.</span><span class="sxs-lookup"><span data-stu-id="a154b-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="a154b-144">Kosten verlengen</span><span class="sxs-lookup"><span data-stu-id="a154b-144">Renew fee</span></span> | <span data-ttu-id="a154b-145">Kosten voor het vernieuwen van een abonnement</span><span class="sxs-lookup"><span data-stu-id="a154b-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="a154b-146">Tarief vergoedingen bij activeren</span><span class="sxs-lookup"><span data-stu-id="a154b-146">Prorate fees when activate</span></span> | <span data-ttu-id="a154b-147">Gefactureerde kosten van de Activering tot het einde van de facturerings periode.</span><span class="sxs-lookup"><span data-stu-id="a154b-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="a154b-148">Eenmalige kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-148">One-time charges</span></span>

<span data-ttu-id="a154b-149">Als u deze eenmalige kosten aan uw factuur wilt toewijzen, moet u de kolom **bedrag** in het bestand op basis van licentie optellen.</span><span class="sxs-lookup"><span data-stu-id="a154b-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="a154b-150">Beschrijving van kosten (kolom ChargeType in afstemmings bestand)</span><span class="sxs-lookup"><span data-stu-id="a154b-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="a154b-151">Uitleg bij kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="a154b-152">Nieuw</span><span class="sxs-lookup"><span data-stu-id="a154b-152">New</span></span> | <span data-ttu-id="a154b-153">Wordt gebruikt wanneer een nieuwe aankoop wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="a154b-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="a154b-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="a154b-154">addQuantity</span></span> | <span data-ttu-id="a154b-155">Wordt gebruikt in de restitutie van de oorspronkelijke aankoop en de nieuwe hoeveelheid na een verhoging.</span><span class="sxs-lookup"><span data-stu-id="a154b-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="a154b-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="a154b-156">removeQuantity</span></span> | <span data-ttu-id="a154b-157">Wordt gebruikt in de restitutie van de oorspronkelijke aankoop en de nieuwe hoeveelheid na een afname.</span><span class="sxs-lookup"><span data-stu-id="a154b-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="a154b-158">Annuleren</span><span class="sxs-lookup"><span data-stu-id="a154b-158">Cancel</span></span> | <span data-ttu-id="a154b-159">Wordt gebruikt wanneer een abonnement wordt geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="a154b-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="a154b-160">Converteren</span><span class="sxs-lookup"><span data-stu-id="a154b-160">Convert</span></span> | <span data-ttu-id="a154b-161">Wordt gebruikt wanneer een licentie wordt bijgewerkt, maar het aantal licenties blijft ongewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a154b-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="a154b-162">Gebruikskosten</span><span class="sxs-lookup"><span data-stu-id="a154b-162">Usage charges</span></span>

<span data-ttu-id="a154b-163">Als u deze gebruiks kosten aan uw factuur wilt toewijzen, moet u de kolom **PretaxCharges** in het op gebruik gebaseerde bestand opsommen.</span><span class="sxs-lookup"><span data-stu-id="a154b-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="a154b-164">Beschrijving van kosten (kolom ChargeType in afstemmings bestand)</span><span class="sxs-lookup"><span data-stu-id="a154b-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="a154b-165">Uitleg bij kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="a154b-166">Gebruiks kosten evalueren bij annuleren</span><span class="sxs-lookup"><span data-stu-id="a154b-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="a154b-167">Toegang tot gebruiks kosten na annulering voor onbetaald gebruik tijdens de huidige facturerings periode.</span><span class="sxs-lookup"><span data-stu-id="a154b-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="a154b-168">Gebruiks kosten evalueren voor de huidige cyclus</span><span class="sxs-lookup"><span data-stu-id="a154b-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="a154b-169">Gebruiks kosten voor de huidige facturerings periode.</span><span class="sxs-lookup"><span data-stu-id="a154b-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="a154b-170">Tegoeden</span><span class="sxs-lookup"><span data-stu-id="a154b-170">Credits</span></span>

<span data-ttu-id="a154b-171">Deze tegoeden toewijzen aan uw factuur:</span><span class="sxs-lookup"><span data-stu-id="a154b-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="a154b-172">Som van de **TotalForCustomer** van het bestand op basis van licentie.</span><span class="sxs-lookup"><span data-stu-id="a154b-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="a154b-173">Som van de kolom **PostTaxTotal** van het bestand op basis van gebruik.</span><span class="sxs-lookup"><span data-stu-id="a154b-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="a154b-174">Beschrijving van kosten (kolom ChargeType in afstemmings bestand)</span><span class="sxs-lookup"><span data-stu-id="a154b-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="a154b-175">Uitleg bij kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="a154b-176">Verschuiving van een regel item</span><span class="sxs-lookup"><span data-stu-id="a154b-176">Offset a line item</span></span> | <span data-ttu-id="a154b-177">Gedeeltelijke of volledige restitutie voor een regel item, inclusief BTW.</span><span class="sxs-lookup"><span data-stu-id="a154b-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="a154b-178">Kortingen op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="a154b-178">Usage-based discounts</span></span>

<span data-ttu-id="a154b-179">Als u deze op gebruik gebaseerde kortingen wilt toewijzen aan uw factuur, kunt u de kolom **PretaxCharges** van het bestand op basis van gebruik opsommen.</span><span class="sxs-lookup"><span data-stu-id="a154b-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="a154b-180">Beschrijving van kosten (kolom ChargeType in afstemmings bestand)</span><span class="sxs-lookup"><span data-stu-id="a154b-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="a154b-181">Uitleg bij kosten</span><span class="sxs-lookup"><span data-stu-id="a154b-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="a154b-182">Activerings korting</span><span class="sxs-lookup"><span data-stu-id="a154b-182">Activation discount</span></span> | <span data-ttu-id="a154b-183">Korting toegepast wanneer het abonnement wordt geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="a154b-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="a154b-184">Cyclus korting</span><span class="sxs-lookup"><span data-stu-id="a154b-184">Cycle discount</span></span> | <span data-ttu-id="a154b-185">Korting toegepast op periodieke kosten.</span><span class="sxs-lookup"><span data-stu-id="a154b-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="a154b-186">Korting vernieuwen</span><span class="sxs-lookup"><span data-stu-id="a154b-186">Renew discount</span></span> | <span data-ttu-id="a154b-187">Korting toegepast wanneer het abonnement wordt verlengd.</span><span class="sxs-lookup"><span data-stu-id="a154b-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="a154b-188">Korting annuleren</span><span class="sxs-lookup"><span data-stu-id="a154b-188">Cancel discount</span></span> | <span data-ttu-id="a154b-189">Kosten worden toegepast wanneer kortingen worden geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="a154b-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="a154b-190">Kortingen op basis van licenties</span><span class="sxs-lookup"><span data-stu-id="a154b-190">License-based discounts</span></span>

<span data-ttu-id="a154b-191">Als u kortingen op basis van licenties aan uw factuur wilt toewijzen, moet u de kolom **TotalOtherDiscount** in het bestand op basis van licentie opsommen.</span><span class="sxs-lookup"><span data-stu-id="a154b-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="a154b-192">*Kortingen op basis van licenties kunnen worden toegepast op meerdere kosten typen.*</span><span class="sxs-lookup"><span data-stu-id="a154b-192">*License-based discounts may be applied to multiple charge types.*</span></span>
