---
title: Klantabonnementen maken in Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het verkopen van abonnementen aan uw klanten voor producten die zijn gepubliceerd door Microsoft en SaaS-producten die zijn gepubliceerd door ISV's van derden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 9052954c81ef55a2bfa06778ace651c9d0f9b26f
ms.sourcegitcommit: e0444145d7720df948b9d02ae2469206db48dba5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110201405"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="3c0eb-103">Klantabonnementen maken, onderbreken of annuleren</span><span class="sxs-lookup"><span data-stu-id="3c0eb-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="3c0eb-104">**Van toepassing op**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="3c0eb-104">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="3c0eb-105">**Juiste rollen:** beheeragent | Factureringsbeheerder | Globale beheerder | Helpdeskagent | Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="3c0eb-105">**Appropriate roles**: Admin agent | Billing admin | Global admin | Helpdesk agent | Sales agent</span></span>

<span data-ttu-id="3c0eb-106">Nadat u een record van uw klant in de Partner Center, kunt u deze abonnementen verkopen aan producten in de catalogus.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-106">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="3c0eb-107">Dit omvat producten die zijn gepubliceerd door Microsoft en SaaS-producten (Software as a Service) die door onafhankelijke onafhankelijke softwareleveranciers (ISV's) zijn gepubliceerd op [de commerciële marketplace.](https://azuremarketplace.microsoft.com/marketplace)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-107">This includes products published by Microsoft and Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="3c0eb-108">Sommige aanbiedingen zijn beperkt tot één abonnement per klant.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-108">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="3c0eb-109">Als u een lijst wilt bekijken met aanbiedingen die zijn beperkt, gaat u naar Partner Center pagina Prijzen en aanbiedingen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-109">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="3c0eb-110">Als partner in het CSP-programma kunt u  SaaS-abonnementen op basis van licenties of saaS-abonnementen met datalicenties aanschaffen bij **ISV-uitgevers** binnen Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-110">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="3c0eb-111">Dit betekent dat u elke  SaaS-aanbieding op basis van licenties of naar [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gebruik kunt aanschaffen die de **ISV-uitgever** voor u beschikbaar heeft gesteld, inclusief exclusieve aanbiedingen waarvoor u toegang hebt.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-111">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="3c0eb-112">Als u andere commerciële marketplace-aanbiedingen van ISV's wilt kopen of beheren (zoals aanbiedingen op basis van gebruik met betrekking tot Azure-toepassingen, containers of VM's), gaat u [naar de Azure Portal.](https://portal.azure.com/)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-112">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

>[!NOTE]
><span data-ttu-id="3c0eb-113">Alle datums en tijden in Partner Center worden opgegeven in de UTC-tijdstandaard (Universal Time Coordinated).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-113">All dates and times in Partner Center are given in the Universal Time Coordinated (UTC) time standard.</span></span> <span data-ttu-id="3c0eb-114">Dit kan tot 24 uur verschillen van uw lokale tijd.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-114">This can differ by up to 24 hours from your local time.</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="3c0eb-115">Een nieuw abonnement maken</span><span class="sxs-lookup"><span data-stu-id="3c0eb-115">Create a new subscription</span></span>

1. <span data-ttu-id="3c0eb-116">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3c0eb-117">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-117">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3c0eb-118">Selecteer **Abonnement toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-118">Select **Add subscription**.</span></span> <span data-ttu-id="3c0eb-119">Op **het tabblad Onlineservices** worden alle beschikbare Marketplace SaaS-aanbiedingen weergegeven.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-119">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="3c0eb-120">Als u alleen bepaalde typen abonnementen wilt zien, maakt u selecties in de beschikbare filters:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-120">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="3c0eb-121">**Uitgever:** kies **Microsoft om** alleen aanbiedingen van Microsoft of **Partner** te bekijken om commerciële marketplace-producten te zien die zijn gepubliceerd door ISV's.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-121">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="3c0eb-122">**Factureringstype:** selecteer het type abonnement dat u wilt gebruiken: **Licentie** of **Gebruik.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-122">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="3c0eb-123">Zie [Facturering op basis van licenties](license-based-billing.md) voor informatie waarmee u kunt kiezen tussen de maandelijkse en jaarlijkse factureringsfrequentie.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-123">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="3c0eb-124">**Categorie:** kies **Enterprise,** **Small Business** of **Trial.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-124">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="3c0eb-125">Zie Proefversies van Microsoft-producten aanbieden voor [meer informatie over proefabonnementen.](offer-your-customers-trials-of-microsoft-products.md)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-125">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="3c0eb-126">Selecteer de productabonnementen die u voor uw klant wilt kopen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-126">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="3c0eb-127">De producten die u ziet, zijn afhankelijk van het type klantsegment (onderwijs, overheid, enzovoort) en de filters die u hebt toegepast.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-127">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="3c0eb-128">Sommige aanbiedingen die op de Marketplace worden weergegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-128">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="3c0eb-129">Dit kan komen door:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-129">This can be because:</span></span>

   - <span data-ttu-id="3c0eb-130">De klant heeft al een abonnement op dat product en heeft er slechts één</span><span class="sxs-lookup"><span data-stu-id="3c0eb-130">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="3c0eb-131">Het abonnement van de klant is mogelijk tijdelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuw abonnement aan te schaffen.)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-131">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="3c0eb-132">Voor SAAS-aanbiedingen van ISV's zijn er mogelijk enkele redenen waarom de aanbieding niet beschikbaar is om te kopen: De ISV biedt mogelijk geen ondersteuning voor het land of de regio van de facturering van de klant; De ISV heeft er mogelijk voor gekozen om de aanbieding niet beschikbaar te maken via het CSP-programma; of de ISV heeft de aanbieding mogelijk uitsluitend [aan](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) bepaalde CSP-partners gedaan.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-132">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="3c0eb-133">De ISV-aanbieding is mogelijk ook niet transacteerbaar via de Partner Center (bijvoorbeeld containers of sommige aanbiedingen op basis van gebruik).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-133">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="3c0eb-134">Voer voor elk abonnement dat u wilt toevoegen het aantal licenties in (indien nodig) en selecteer **Toevoegen aan winkelwagen.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-134">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="3c0eb-135">Wanneer u klaar bent met het toevoegen van abonnementen, **selecteert u Uw** bestelling controleren en controleren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-135">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="3c0eb-136">Nadat u uw orders hebt gecontroleerd en klaar bent om deze abonnementen te kopen, selecteert u **Kopen.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-136">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="3c0eb-137">Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-137">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="3c0eb-138">U kunt het abonnement controleren of bewerken door de abonnementsnaam te selecteren op de pagina **Abonnementen van die** klant.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-138">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="3c0eb-139">Hier kunt u invoeglicenties selecteren als deze beschikbaar zijn, het aantal licenties wijzigen of het abonnement opschorten.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-139">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="3c0eb-140">**Voor ISV SaaS-abonnementen (op basis van licenties en naar licentie) geldt het volgende:**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-140">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="3c0eb-141">U ontvangt een koppeling naar de site van de ISV-uitgever.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-141">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="3c0eb-142">Deze koppeling helpt u bij het voltooien van de implementatie of het instellen van het account van het abonnement van de klant.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-142">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="3c0eb-143">Noch u noch uw klant ontvangt een e-mail met instructies voor het voltooien van het instellen/inrichten van het account voor dit type ISV-abonnement.)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-143">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="3c0eb-144">Als uw abonnement wordt geleverd met een gratis proefversie van 30 dagen, wordt de gratis proefperiode automatisch toegepast.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-144">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="3c0eb-145">Als partner in het CSP-programma kunt u de gratis proefperiode voor aanbiedingen die u voor klanten koopt, niet in de weg staan.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-145">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="3c0eb-146">Zodra de gratis proefperiode is afgelopen, wordt de abonnementsperiode van start en wordt het abonnement omgezet in de betaalde status.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-146">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="3c0eb-147">Het abonnement wordt vervolgens automatisch vernieuwd volgens hetzelfde schema.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-147">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="3c0eb-148">Abonnementen bijwerken met invoegtoepassingen</span><span class="sxs-lookup"><span data-stu-id="3c0eb-148">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="3c0eb-149">Als de klant een invoegabonnement wil aanschaffen, moet deze eerst een actief basisabonnement hebben.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-149">To purchase an add-on, the customer must first have an active base subscription.</span></span>  <span data-ttu-id="3c0eb-150">U kunt invoegtoepassingen niet aanschaffen via de catalogus.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-150">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="3c0eb-151">Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-151">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3c0eb-152">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-152">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3c0eb-153">Kies het abonnement dat u wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-153">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="3c0eb-154">Onder de **sectie Status** vindt u een lijst met beschikbare invoegtoepassingen voor het abonnement.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-154">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="3c0eb-155">Werk het aantal licenties voor elke vereiste invoeg-invoeging bij.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-155">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="3c0eb-156">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-156">Then **Submit** your changes.</span></span>

<span data-ttu-id="3c0eb-157">De mogelijkheid om invoegtoepassingen aan te schaffen via Partner Center is alleen beschikbaar voor directe factuur- en indirecte providers.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-157">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="3c0eb-158">Alleen in aanmerking komende invoegtoepassingen worden weergegeven op basis van de basisvereisten en regionale beschikbaarheid.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-158">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="3c0eb-159">Raadpleeg de aanbiedingsmatrix voor cloud resellers voor meer informatie over prijzen en aanbiedingen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-159">For more information about pricing and offers, refer to the Cloud Reseller offer matrix.</span></span> <span data-ttu-id="3c0eb-160">Als u het basisabonnement onderbreekt, worden ook alle bijbehorende invoegtoepassingen onderbroken.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-160">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="3c0eb-161">Begindatums voor invoegtoepassingen worden afgestemd met het basisabonnement en de kosten worden berekend op basis van de begindatum van de kosten en de einddatum van de kosten met pro rata kosten op de eerste factuur.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-161">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="3c0eb-162">Zie Op licenties gebaseerde facturering [voor meer informatie.](license-based-billing.md)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-162">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="3c0eb-163">Een abonnement opschorten of annuleren</span><span class="sxs-lookup"><span data-stu-id="3c0eb-163">Suspend or cancel a subscription</span></span>

<span data-ttu-id="3c0eb-164">Partners kunnen een abonnement opzeggen of annuleren als dit wordt aangevraagd door de klant, of in het geval van niet-vooruitbetaling of fraude.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-164">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="3c0eb-165">Een abonnement opschorten</span><span class="sxs-lookup"><span data-stu-id="3c0eb-165">Suspend a subscription</span></span>

<span data-ttu-id="3c0eb-166">Wanneer u de status van een abonnement wijzigt in **Tijdelijk,** kunnen gebruikers zich niet aanmelden of toegang krijgen tot services.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-166">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="3c0eb-167">Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-167">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3c0eb-168">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-168">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3c0eb-169">Kies het abonnement dat u wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-169">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="3c0eb-170">Kies **Onderbroken** bij **Status**.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-170">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="3c0eb-171">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-171">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="3c0eb-172">Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd, of 90 dagen plus het aantal dagen tussen het moment dat het account is geopend en de eerste factureringsperiode (maximaal 120 dagen).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-172">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="3c0eb-173">Wanneer u een abonnement onder de  knop Tijdelijk opschorten ziet, wordt aangegeven wanneer het abonnement automatisch verloopt als u het abonnement niet opnieuw activeren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-173">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

>[!NOTE]
><span data-ttu-id="3c0eb-174">CSP-abonnementen hebben geen verlopen periode (zoals web-directe abonnementen) waarin de services nog steeds werken, maar het abonnement geen factureringskosten genereert.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-174">CSP subscriptions don't have an expired period (the way web-direct subscriptions do) during which the services are still working but the subscription doesn't generate any billing charges.</span></span> <span data-ttu-id="3c0eb-175">CSP-abonnementen zijn actief of tijdelijk (of volledig verwijderd).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-175">CSP subscriptions are either active or suspended (or fully deleted).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="3c0eb-176">Een abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="3c0eb-176">Cancel a subscription</span></span>

<span data-ttu-id="3c0eb-177">U kunt SaaS-abonnementen op basis van licenties van ISV-uitgevers van derden annuleren binnen de Partner Center [commerciële marketplace.](csp-commercial-marketplace-overview.md)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-177">You can cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="3c0eb-178">Zolang u binnen de annuleringsperiode annuleert, ontvangt u een volledige restitutie.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-178">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="3c0eb-179">Voor ISV-aanbiedingen die maandelijks worden gefactureerd:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-179">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="3c0eb-180">Als u minder dan 24 uur na het plaatsen van de order annuleert, ontvangt u een volledig tegoed op de volgende factuur.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-180">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="3c0eb-181">Als u later dan 24 uur na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-181">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="3c0eb-182">Voor aanbiedingen die jaarlijks worden gefactureerd:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-182">For offers billed annually:</span></span>

- <span data-ttu-id="3c0eb-183">Als u minder dan 14 dagen na het plaatsen van de bestelling annuleert, ontvangt u een volledig tegoed op de volgende factuur.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-183">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="3c0eb-184">Als u later dan 14 dagen na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-184">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="3c0eb-185">Nadat deze perioden zijn afgelopen, ziet u niet langer de optie om het abonnement te annuleren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-185">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="3c0eb-186">ISV-services van derden (die bijvoorbeeld virtuele machines of containers gebruiken) op basis van gebruik en naar gebruik komen niet in aanmerking voor retournering.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-186">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="3c0eb-187">Op gebruik gebaseerde services kunnen worden verwijderd als annuleringsmethode.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-187">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="3c0eb-188">Omdat de kosten na gebruik worden gefactureerd, komen deze services niet in aanmerking voor restitutie.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-188">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="3c0eb-189">Ga als volgt te werk om een SaaS-abonnement op basis van een licentie van een ISV-uitgever te annuleren:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-189">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="3c0eb-190">Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-190">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3c0eb-191">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-191">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3c0eb-192">Zoek het abonnement dat u wilt annuleren.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-192">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="3c0eb-193">Selecteer annuleren **in de** kolom **Status.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-193">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="3c0eb-194">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-194">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="3c0eb-195">Als er een dialoogvenster wordt weergegeven, vult u relevante gegevens in en selecteert u **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-195">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="3c0eb-196">Selecteer Ja, annuleren om de annulering te **bevestigen.**</span><span class="sxs-lookup"><span data-stu-id="3c0eb-196">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="3c0eb-197">U kunt er ook voor kiezen om een abonnement Azure Marketplace annuleren met behulp van API's.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-197">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="3c0eb-198">Zie Een abonnement op Azure Marketplace [annuleren om dit te doen.](/partner-center/develop/cancel-an-azure-marketplace-subscription)</span><span class="sxs-lookup"><span data-stu-id="3c0eb-198">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="3c0eb-199">Kiezen of u een abonnement op de commerciële marketplace automatisch wilt verlengen</span><span class="sxs-lookup"><span data-stu-id="3c0eb-199">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="3c0eb-200">Actieve abonnementen zijn standaard ingesteld om automatisch te worden verlengd wanneer de abonnementsperiode verloopt.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-200">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="3c0eb-201">Voor [abonnementen op commerciële marketplace-producten](csp-commercial-marketplace-overview.md)kunt u ervoor kiezen om het abonnement niet automatisch te verlengen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-201">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="3c0eb-202">Als u wilt voorkomen dat een actief abonnement op de commerciële marketplace automatisch wordt verlengd:</span><span class="sxs-lookup"><span data-stu-id="3c0eb-202">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="3c0eb-203">Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="3c0eb-203">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="3c0eb-204">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-204">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="3c0eb-205">Selecteer **Abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-205">Select **Subscriptions**.</span></span> <span data-ttu-id="3c0eb-206">Hier worden alle op licenties gebaseerde abonnementen vermeld die u voor de klant hebt aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-206">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="3c0eb-207">Selecteer in **de** kolom Abonnement het abonnement dat u wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-207">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="3c0eb-208">Zoek op de pagina met abonnementsdetails **de sectie Status** en vink het selectievakje Automatisch **verlengen** uit.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-208">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="3c0eb-209">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="3c0eb-209">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3c0eb-210">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="3c0eb-210">Next steps</span></span>

- [<span data-ttu-id="3c0eb-211">Commerciële marketplace-producten kopen voor uw klanten</span><span class="sxs-lookup"><span data-stu-id="3c0eb-211">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="3c0eb-212">Commerciële marketplace-producten voor uw klanten beheren</span><span class="sxs-lookup"><span data-stu-id="3c0eb-212">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="3c0eb-213">Overzicht van commerciële marketplace</span><span class="sxs-lookup"><span data-stu-id="3c0eb-213">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)