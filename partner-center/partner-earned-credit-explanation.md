---
title: Het tegoed van de partner voor beheerde services
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe micro soft partner (PEC) voor beheerde services wordt berekend en betaald, en hoe u ervoor kunt zorgen dat u in aanmerking komt.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 010f74164b0428a5cd6ffcde5000b52ac6a6993f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99623997"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="b9b8c-103">Hoe het verdiende tegoed van de partner wordt berekend en betaald</span><span class="sxs-lookup"><span data-stu-id="b9b8c-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="b9b8c-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="b9b8c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b9b8c-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="b9b8c-105">Global admin</span></span>
- <span data-ttu-id="b9b8c-106">Gebruikersbeheerder</span><span class="sxs-lookup"><span data-stu-id="b9b8c-106">User admin</span></span>
- <span data-ttu-id="b9b8c-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="b9b8c-107">Admin agent</span></span>
- <span data-ttu-id="b9b8c-108">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="b9b8c-108">Billing admin</span></span>
- <span data-ttu-id="b9b8c-109">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="b9b8c-109">Sales agent</span></span>

<span data-ttu-id="b9b8c-110">De partner die het tegoed voor beheerde services (PEC) heeft behaald, erkent en beloont partners die eigenaar zijn van het operationele beheer en het beheer van onderdelen van, of de volledige Azure-omgeving van hun klanten.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="b9b8c-111">In CSP krijgen partners standaard de benodigde toegangs rechten voor het abonnement van de klant, zodat ze 24 X 7 operationeel beheer en beheer van de resources in het abonnement kunnen uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="b9b8c-112">In de volgende sectie worden extra manieren beschreven waarop de klant toegang kan inrichten voor het handelen van partners.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="b9b8c-113">Het maandelijkse factuurbedrag is het nettobedrag van het tegoed van de partner.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="b9b8c-114">Partners kunnen de PEC-gegevens zien op hun maandelijkse afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="b9b8c-115">Lees [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)voor meer informatie over de manier waarop een klant toegang kan inrichten voor de handelende partner.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="b9b8c-116">Lees ook de [beheerders bevoegdheden voor Azure CSP-abonnementen opnieuw invoeren](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="b9b8c-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="b9b8c-117">Geschiktheid</span><span class="sxs-lookup"><span data-stu-id="b9b8c-117">Eligibility</span></span>

<span data-ttu-id="b9b8c-118">De volgende vereisten zijn van toepassing op het ontvangen van de partner (PEC):</span><span class="sxs-lookup"><span data-stu-id="b9b8c-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="b9b8c-119">U moet over een actieve MPN-overeenkomst en een geldige RBAC-rol (Role-based Access Control) beschikken om het ontvangen van tegoed voor de door u beheerde Azure-assets te krijgen.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="b9b8c-120">U moet over een 24x7 operationeel beheer en beheer van de Azure-resources van de klant in CSP beschikken.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="b9b8c-121">Dit betekent dat u beheerders bevoegdheden nodig hebt voor het Azure-abonnement van de klant, Azure-resource groep, Azure-resource.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="b9b8c-122">In het geval van indirecte providers en hun indirecte wederverkopers komt de indirecte provider in aanmerking voor PEC als hetzij de indirecte provider ofwel de indirecte reseller ofwel beide over dit operationele beheer beschikken.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="b9b8c-123">Zie [beheerders bevoegdheden voor Azure CSP-abonnementen herstellen voor](./revoke-reinstate-csp.md)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](./revoke-reinstate-csp.md).</span></span>

- <span data-ttu-id="b9b8c-124">Naast de bovenstaande vereisten is PEC alleen van toepassing op Services die worden vermeld in de prijzen van het Azure-abonnement. deze kunt u exporteren via de prijs pagina voor [Azure-abonnementen](https://partner.microsoft.com/commerce/sales) .</span><span class="sxs-lookup"><span data-stu-id="b9b8c-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="b9b8c-125">PEC is **niet** van toepassing op de volgende services:</span><span class="sxs-lookup"><span data-stu-id="b9b8c-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="b9b8c-126">Azure plan-reserve ringen</span><span class="sxs-lookup"><span data-stu-id="b9b8c-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="b9b8c-127">Producten van derden geïdentificeerd als derde partij in de kolom Tags van de verbruiks prijs van het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="b9b8c-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="b9b8c-128">Producten in de prijs lijst voor Marketplace</span><span class="sxs-lookup"><span data-stu-id="b9b8c-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="b9b8c-129">Azure Spot Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="b9b8c-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="b9b8c-130">PEC wordt naar het Azure-resource niveau geverdiend.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="b9b8c-131">Als u geldige toegang hebt op het niveau van het abonnement of de resource groep, verdient elke resource die tot de hogere entiteit rolt, een PEC.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="b9b8c-132">Meer informatie over PEC is ook beschikbaar op de pagina [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) .</span><span class="sxs-lookup"><span data-stu-id="b9b8c-132">Details on PEC are also available on the [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="b9b8c-133">Berekening</span><span class="sxs-lookup"><span data-stu-id="b9b8c-133">Calculation</span></span>

<span data-ttu-id="b9b8c-134">PEC wordt dagelijks berekend en kan worden weer gegeven in het dagelijks gebruiks bestand en het maandelijkse factuur afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="b9b8c-135">Een partner (een indirecte provider of een indirecte wederverkoper) moet toegang hebben tot de hele dag (24x7) om ervoor te zorgen dat ze PEC verdienen.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="b9b8c-136">PEC wordt dagelijks berekend op basis van de beheerde Azure-assets.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="b9b8c-137">Partners die permanente privileged Access via de maand (toegangs duur) bewaren en voor alle in aanmerking komende resources (bereik van toegang), verdienen volledige PEC.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-137">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC.</span></span> <span data-ttu-id="b9b8c-138">De beperking van het bereik en de periode resulteert in een lager PEC-tempo voor de maand.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-138">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="b9b8c-139">Dagelijks geclassificeerd gebruiks bestand wordt dagelijks op een Azure-Asset weer gegeven, of PEC wordt toegepast.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-139">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="b9b8c-140">Partners kunnen ook worden inge schreven in waarschuwingen om wijzigingen in permanente toegang te controleren.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-140">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="b9b8c-141">Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="b9b8c-141">Azure Cost Management</span></span>

<span data-ttu-id="b9b8c-142">Azure Cost Management (ACM) met behulp van kosten analyse kunt u als partner de kosten bekijken die het voor deel van PEC hebben ontvangen.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-142">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="b9b8c-143">Meld u aan bij de partner-Tenant in het [Azure Portal](https://portal.azure.com)en selecteer **Cost Management + facturering**.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-143">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="b9b8c-144">**Kosten beheer** selecteren</span><span class="sxs-lookup"><span data-stu-id="b9b8c-144">Select **Cost management**</span></span>

3. <span data-ttu-id="b9b8c-145">**Kosten analyse** selecteren</span><span class="sxs-lookup"><span data-stu-id="b9b8c-145">Select **Cost Analysis**</span></span>

   <span data-ttu-id="b9b8c-146">In de weer gave kosten analyse worden de kosten voor uw facturerings account weer gegeven, voor alle services die zijn gekocht en verbruikt tegen de prijzen die u micro soft betaalt.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-146">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="b9b8c-147">Selecteer **PartnerEarnedCreditApplied** in de vervolg keuzelijst van een draai grafiek om de kosten weer te geven waarop een PEC is toegepast.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-147">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="b9b8c-148">Wanneer de eigenschap **PartnerEarnedCreditApplied** is ingesteld op True, hebben de bijbehorende kosten het voor deel van het tegoed van de partner.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-148">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="b9b8c-149">Wanneer de eigenschap PartnerEarnedCreditApplied is ingesteld op False, voldoen de bijbehorende kosten niet aan het vereiste recht voor het tegoed of is de aangeschafte service niet in aanmerking komen voor een partner die het tegoed ontvangt.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-149">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="b9b8c-150">Normaal gesp roken duurt het gebruik voor Services 8-24 uur in **Cost Management** en de PEC-tegoeden worden binnen 48 uur na de toegangs tijd weer gegeven in azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-150">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="b9b8c-151">U kunt ook groeperen op, en filteren op, de eigenschap **PartnerEarnedCreditApplied** met behulp **van de Group by en** filter functies toevoegen om te zoomen op de kosten met PEC en de kosten waarop geen PEC is toegepast.</span><span class="sxs-lookup"><span data-stu-id="b9b8c-151">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9b8c-152">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="b9b8c-152">Next steps</span></span>

- [<span data-ttu-id="b9b8c-153">Creditering van de partner-overzicht</span><span class="sxs-lookup"><span data-stu-id="b9b8c-153">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="b9b8c-154">Gedetailleerde voor beelden van de credit berekeningen van de partner bevinden zich in de prijs lijst die u kunt bereiken via het dash board van de partner centrum (aanmelden is vereist).</span><span class="sxs-lookup"><span data-stu-id="b9b8c-154">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="b9b8c-155">Naar Azure-plan gaan-aan de slag</span><span class="sxs-lookup"><span data-stu-id="b9b8c-155">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="b9b8c-156">Abonnementen en resources beheren onder het Azure-abonnement</span><span class="sxs-lookup"><span data-stu-id="b9b8c-156">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="b9b8c-157">Beheerders bevoegdheden voor Azure CSP-abonnementen intrekken of opnieuw instatussen</span><span class="sxs-lookup"><span data-stu-id="b9b8c-157">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
