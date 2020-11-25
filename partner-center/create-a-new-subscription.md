---
title: Klant abonnementen maken in het partner centrum
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het verkopen van uw klanten abonnementen voor producten die door micro soft zijn gepubliceerd, evenals SaaS-producten die zijn gepubliceerd door onafhankelijke software fabrikanten.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038877"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="d3882-103">Klantabonnementen maken, onderbreken of annuleren</span><span class="sxs-lookup"><span data-stu-id="d3882-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="d3882-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="d3882-104">**Applies to**</span></span>

- <span data-ttu-id="d3882-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="d3882-105">Partner Center</span></span>
- <span data-ttu-id="d3882-106">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d3882-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="d3882-107">CSP-partners</span><span class="sxs-lookup"><span data-stu-id="d3882-107">CSP partners</span></span>

<span data-ttu-id="d3882-108">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="d3882-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d3882-109">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="d3882-109">Admin agent</span></span>
- <span data-ttu-id="d3882-110">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="d3882-110">Billing admin</span></span>
- <span data-ttu-id="d3882-111">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="d3882-111">Global admin</span></span>
- <span data-ttu-id="d3882-112">Helpdesk medewerker</span><span class="sxs-lookup"><span data-stu-id="d3882-112">Helpdesk agent</span></span>
- <span data-ttu-id="d3882-113">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="d3882-113">Sales agent</span></span>

<span data-ttu-id="d3882-114">Nadat u een record van uw klant in het partner centrum hebt gemaakt, kunt u deze abonnementen verkopen aan producten in de catalogus.</span><span class="sxs-lookup"><span data-stu-id="d3882-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="d3882-115">Dit geldt ook voor producten die door micro soft worden gepubliceerd, evenals SaaS-producten (Software as a Service) die door onafhankelijke software leveranciers (Isv's) van derden naar de [commerciële Marketplace](https://azuremarketplace.microsoft.com/marketplace)worden gepubliceerd.</span><span class="sxs-lookup"><span data-stu-id="d3882-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="d3882-116">Sommige aanbiedingen zijn beperkt tot één abonnement per klant.</span><span class="sxs-lookup"><span data-stu-id="d3882-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="d3882-117">Ga naar de pagina prijzen en aanbiedingen van het partner centrum om een lijst weer te geven van welke aanbiedingen zijn beperkt.</span><span class="sxs-lookup"><span data-stu-id="d3882-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="d3882-118">Als partner in het CSP-programma kunt u SaaS **-abonnementen op basis van licenties** of **Data limieten** aanschaffen bij ISV-uitgevers in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="d3882-118">As a partner in the CSP program, you can purchase **license-based** or **metered** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="d3882-119">Dit betekent dat u een **op licenties gebaseerde** SaaS- **metered** aanbieding kunt aanschaffen die de ISV-Uitgever voor u beschikbaar heeft gesteld, met inbegrip van [exclusieve aanbiedingen](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) waartoe u toegang hebt.</span><span class="sxs-lookup"><span data-stu-id="d3882-119">This means you can purchase any **license-based** or **metered** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="d3882-120">Als u andere commerciële Marketplace-aanbiedingen van onafhankelijke software leveranciers wilt kopen of beheren (zoals aanbiedingen op basis van het gebruik van Azure-toepassingen, containers of Vm's), gaat u naar de [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="d3882-120">To purchase or manage other, commercial marketplace offers from ISVs (such as usage-based offers involving Azure applications, Containers or VMs), you must go to the [Azure portal](https://portal.azure.com/).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="d3882-121">Een nieuw abonnement maken</span><span class="sxs-lookup"><span data-stu-id="d3882-121">Create a new subscription</span></span>

1. <span data-ttu-id="d3882-122">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="d3882-122">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3882-123">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="d3882-123">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3882-124">Selecteer **abonnement toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="d3882-124">Select **Add subscription**.</span></span> <span data-ttu-id="d3882-125">Op het tabblad **Online Services** worden alle beschik bare SaaS-aanbiedingen voor Marketplace weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="d3882-125">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="d3882-126">Als u alleen bepaalde typen abonnementen wilt zien, selecteert u de gewenste opties in de beschik bare filters:</span><span class="sxs-lookup"><span data-stu-id="d3882-126">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="d3882-127">**Uitgever**: Kies **micro soft** om alleen aanbiedingen van micro soft of **partner** te bekijken voor commerciële Marketplace-producten die door isv's worden gepubliceerd.</span><span class="sxs-lookup"><span data-stu-id="d3882-127">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="d3882-128">**Facturerings type**: Selecteer het type abonnement facturering dat u wilt gebruiken: **licentie** of **gebruik**.</span><span class="sxs-lookup"><span data-stu-id="d3882-128">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="d3882-129">Zie [factuur op basis van licenties](license-based-billing.md) voor informatie die u kan helpen bij het bepalen van de maandelijkse en jaarlijkse facturerings frequentie.</span><span class="sxs-lookup"><span data-stu-id="d3882-129">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="d3882-130">**Categorie**: Kies **Enter prise**, **Small Business** of **proef versie**.</span><span class="sxs-lookup"><span data-stu-id="d3882-130">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="d3882-131">Zie voor meer informatie over proef abonnementen [uw klanten een proef versie van micro soft-producten aanbieden](offer-your-customers-trials-of-microsoft-products.md).</span><span class="sxs-lookup"><span data-stu-id="d3882-131">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="d3882-132">Selecteer de product abonnementen die u wilt kopen voor uw klant.</span><span class="sxs-lookup"><span data-stu-id="d3882-132">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="d3882-133">De producten die u ziet, zijn afhankelijk van het type klant segment (onderwijs, overheid enz.) en de filters die u hebt toegepast.</span><span class="sxs-lookup"><span data-stu-id="d3882-133">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="d3882-134">Sommige aanbiedingen die op Marketplace worden weer gegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner.</span><span class="sxs-lookup"><span data-stu-id="d3882-134">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="d3882-135">Dit kan een van de volgende zijn:</span><span class="sxs-lookup"><span data-stu-id="d3882-135">This can be because:</span></span>

   - <span data-ttu-id="d3882-136">De klant heeft al een abonnement op dat product en is slechts toegestaan</span><span class="sxs-lookup"><span data-stu-id="d3882-136">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="d3882-137">Het abonnement van de klant is mogelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuwe te kopen.)</span><span class="sxs-lookup"><span data-stu-id="d3882-137">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="d3882-138">Voor ISV SaaS-aanbiedingen kunnen er een paar redenen zijn waarom de aanbieding niet beschikbaar is voor aankoop: de ISV biedt mogelijk geen ondersteuning voor het factuur land of de regio van de klant. de ISV heeft mogelijk ervoor gekozen om de aanbieding niet beschikbaar te stellen via het CSP-programma; het is ook mogelijk dat de ISV de aanbieding [exclusief](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) heeft gemaakt voor bepaalde CSP-partners.</span><span class="sxs-lookup"><span data-stu-id="d3882-138">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="d3882-139">De ISV-aanbieding kan ook niet worden verwerkt via het partner centrum (bijvoorbeeld containers of bepaalde op gebruik gebaseerde aanbiedingen).</span><span class="sxs-lookup"><span data-stu-id="d3882-139">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="d3882-140">Voer het aantal licenties (indien nodig) in voor elk abonnement dat u wilt toevoegen en selecteer **toevoegen aan winkel wagen**.</span><span class="sxs-lookup"><span data-stu-id="d3882-140">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="d3882-141">Wanneer u klaar bent met het toevoegen van abonnementen, selecteert u uw bestelling **controleren** en controleren.</span><span class="sxs-lookup"><span data-stu-id="d3882-141">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="d3882-142">Wanneer u uw orders hebt gecontroleerd en u klaar bent om deze abonnementen te kopen, selecteert u **kopen**.</span><span class="sxs-lookup"><span data-stu-id="d3882-142">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="d3882-143">Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:</span><span class="sxs-lookup"><span data-stu-id="d3882-143">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="d3882-144">U kunt het abonnement bekijken of bewerken door de naam van het abonnement te selecteren op de pagina **abonnementen** van die klant.</span><span class="sxs-lookup"><span data-stu-id="d3882-144">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="d3882-145">Hier kunt u licenties voor invoeg toepassingen selecteren als er een beschikbaar is, het aantal licenties wijzigen of het abonnement opschorten.</span><span class="sxs-lookup"><span data-stu-id="d3882-145">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="d3882-146">**Voor ISV SaaS-abonnementen (op basis van licenties en data limieten):**</span><span class="sxs-lookup"><span data-stu-id="d3882-146">**For ISV SaaS (license-based and metered) subscriptions:**</span></span>
    - <span data-ttu-id="d3882-147">U ontvangt een koppeling naar de site van de ISV-Uitgever.</span><span class="sxs-lookup"><span data-stu-id="d3882-147">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="d3882-148">Deze koppeling helpt u bij het volt ooien van de implementatie of het instellen van het account voor het abonnement van de klant.</span><span class="sxs-lookup"><span data-stu-id="d3882-148">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="d3882-149">U en uw klant ontvangen geen e-mail bericht met instructies voor het volt ooien van het account dat is ingesteld/inrichten voor dit type ISV-abonnement.)</span><span class="sxs-lookup"><span data-stu-id="d3882-149">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="d3882-150">Als uw abonnement wordt geleverd met een gratis proef versie van 30 dagen, wordt de gratis proef periode automatisch toegepast.</span><span class="sxs-lookup"><span data-stu-id="d3882-150">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="d3882-151">Als partner in het CSP-programma kunt u de gratis proef periode van aanbiedingen die u aanschaft voor klanten niet kwijt schelden.</span><span class="sxs-lookup"><span data-stu-id="d3882-151">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="d3882-152">Zodra de gratis proef periode is afgelopen, wordt de abonnements termijn gestart en wordt het abonnement omgezet in de betaalde status.</span><span class="sxs-lookup"><span data-stu-id="d3882-152">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="d3882-153">Het abonnement wordt vervolgens automatisch verlengd volgens hetzelfde schema.</span><span class="sxs-lookup"><span data-stu-id="d3882-153">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="d3882-154">Abonnementen bijwerken met invoegtoepassingen</span><span class="sxs-lookup"><span data-stu-id="d3882-154">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="d3882-155">Als u een invoegtoepassing wilt kopen, moet de klant eerst een actief basisabonnement hebben.</span><span class="sxs-lookup"><span data-stu-id="d3882-155">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="d3882-156">U kunt invoegtoepassingen niet aanschaffen via de catalogus.</span><span class="sxs-lookup"><span data-stu-id="d3882-156">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="d3882-157">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="d3882-157">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3882-158">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="d3882-158">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3882-159">Kies het abonnement dat u wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="d3882-159">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d3882-160">Onder de sectie **status** ziet u een lijst met beschik bare invoeg toepassingen voor het abonnement.</span><span class="sxs-lookup"><span data-stu-id="d3882-160">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="d3882-161">Werk het aantal licenties voor elke vereiste invoeg toepassing bij.</span><span class="sxs-lookup"><span data-stu-id="d3882-161">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="d3882-162">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="d3882-162">Then **Submit** your changes.</span></span>

<span data-ttu-id="d3882-163">De mogelijkheid om invoeg toepassingen te kopen via partner centrum is alleen beschikbaar voor directe factuur-en indirecte providers.</span><span class="sxs-lookup"><span data-stu-id="d3882-163">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="d3882-164">Alleen in aanmerking komende invoeg toepassingen worden weer gegeven op basis van de basis vereisten en regionale Beschik baarheid.</span><span class="sxs-lookup"><span data-stu-id="d3882-164">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="d3882-165">Raadpleeg de aanbiedingsmatrix voor cloudresellers voor meer informatie over prijzen en aanbiedingen.</span><span class="sxs-lookup"><span data-stu-id="d3882-165">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="d3882-166">Als u het basisabonnement onderbreekt, worden ook alle bijbehorende invoegtoepassingen onderbroken.</span><span class="sxs-lookup"><span data-stu-id="d3882-166">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="d3882-167">Begindatums voor invoegtoepassingen worden afgestemd met het basisabonnement en de kosten worden berekend op basis van de begindatum van de kosten en de einddatum van de kosten met pro rata kosten op de eerste factuur.</span><span class="sxs-lookup"><span data-stu-id="d3882-167">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="d3882-168">Zie voor meer informatie [facturering op basis van licenties](license-based-billing.md).</span><span class="sxs-lookup"><span data-stu-id="d3882-168">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="d3882-169">Een abonnement opschorten of annuleren</span><span class="sxs-lookup"><span data-stu-id="d3882-169">Suspend or cancel a subscription</span></span>

<span data-ttu-id="d3882-170">Partners kunnen een abonnement opschorten of annuleren indien dit wordt aangevraagd door de klant of in gevallen van niet-betaling of fraude.</span><span class="sxs-lookup"><span data-stu-id="d3882-170">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="d3882-171">Een abonnement opschorten</span><span class="sxs-lookup"><span data-stu-id="d3882-171">Suspend a subscription</span></span>

<span data-ttu-id="d3882-172">Wanneer u de status van een abonnement wijzigt in **opgeschort**, kunnen gebruikers zich niet aanmelden of hebben geen toegang tot services.</span><span class="sxs-lookup"><span data-stu-id="d3882-172">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="d3882-173">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="d3882-173">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3882-174">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="d3882-174">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3882-175">Kies het abonnement dat u wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="d3882-175">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="d3882-176">Kies **Onderbroken** bij **Status**.</span><span class="sxs-lookup"><span data-stu-id="d3882-176">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="d3882-177">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="d3882-177">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d3882-178">Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd 90, plus het aantal dagen tussen het tijdstip waarop het account is geopend en de eerste facturerings periode (Maxi maal 120 dagen).</span><span class="sxs-lookup"><span data-stu-id="d3882-178">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="d3882-179">Wanneer u een abonnement uitbreekt, wordt de datum weer gegeven die u onder de **onderbroken** knop ziet wanneer het abonnement automatisch verloopt als u het niet opnieuw activeert.</span><span class="sxs-lookup"><span data-stu-id="d3882-179">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="d3882-180">Een abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="d3882-180">Cancel a subscription</span></span>

<span data-ttu-id="d3882-181">U hebt de mogelijkheid om op licenties gebaseerde SaaS-abonnementen te annuleren vanuit ISV-uitgevers van derden binnen de [commerciële Marketplace](csp-commercial-marketplace-overview.md)van partner Center.</span><span class="sxs-lookup"><span data-stu-id="d3882-181">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="d3882-182">Zolang u de annulerings periode hebt geannuleerd, ontvangt u een volledige terugbetaling.</span><span class="sxs-lookup"><span data-stu-id="d3882-182">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="d3882-183">Voor ISV-aanbiedingen worden maandelijks gefactureerd:</span><span class="sxs-lookup"><span data-stu-id="d3882-183">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="d3882-184">Als u minder dan 24 uur annuleert nadat u de order hebt geplaatst, ontvangt u een volledig tegoed op de volgende factuur.</span><span class="sxs-lookup"><span data-stu-id="d3882-184">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d3882-185">Als u later dan 24 uur annuleert nadat u de order hebt geplaatst, wordt de annulering gepland om te worden uitgevoerd bij het vernieuwen.</span><span class="sxs-lookup"><span data-stu-id="d3882-185">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d3882-186">Voor aanbiedingen die jaarlijks worden gefactureerd:</span><span class="sxs-lookup"><span data-stu-id="d3882-186">For offers billed annually:</span></span>

- <span data-ttu-id="d3882-187">Als u minder dan 14 dagen na het plaatsen van de bestelling annuleert, ontvangt u een volledig tegoed op de volgende factuur.</span><span class="sxs-lookup"><span data-stu-id="d3882-187">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="d3882-188">Als u later dan 14 dagen na het plaatsen van de order annuleert, wordt de annulering gepland om te worden uitgevoerd bij het vernieuwen.</span><span class="sxs-lookup"><span data-stu-id="d3882-188">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="d3882-189">Nadat deze peri Oden zijn afgelopen, ziet u niet langer de optie om het abonnement te annuleren.</span><span class="sxs-lookup"><span data-stu-id="d3882-189">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="d3882-190">Op basis van gebruik en meting van de ISV-services van derden (die bijvoorbeeld virtuele machines of containers gebruiken) komen niet in aanmerking voor retour.</span><span class="sxs-lookup"><span data-stu-id="d3882-190">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="d3882-191">Op gebruik gebaseerde services kunnen niet worden ingericht als een annulerings methode.</span><span class="sxs-lookup"><span data-stu-id="d3882-191">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="d3882-192">Omdat kosten worden gefactureerd na gebruik, komen deze services niet in aanmerking voor een restitutie.</span><span class="sxs-lookup"><span data-stu-id="d3882-192">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="d3882-193">Ga als volgt te werk om een SaaS-abonnement op basis van een licentie van een ISV-uitgever te annuleren:</span><span class="sxs-lookup"><span data-stu-id="d3882-193">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="d3882-194">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="d3882-194">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3882-195">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="d3882-195">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3882-196">Zoek het abonnement dat u wilt annuleren.</span><span class="sxs-lookup"><span data-stu-id="d3882-196">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="d3882-197">Selecteer **Annuleren** in de kolom **status** .</span><span class="sxs-lookup"><span data-stu-id="d3882-197">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="d3882-198">Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="d3882-198">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="d3882-199">Als er een dialoog venster wordt weer gegeven, vult u de relevante gegevens in en selecteert u vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="d3882-199">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="d3882-200">Selecteer **Ja, annuleren** om de annulering te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="d3882-200">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="d3882-201">U kunt er ook voor kiezen om een Azure Marketplace-abonnement te annuleren met behulp van Api's.</span><span class="sxs-lookup"><span data-stu-id="d3882-201">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="d3882-202">Zie [een abonnement op Azure Marketplace annuleren](/partner-center/develop/cancel-an-azure-marketplace-subscription)als u dit wilt doen.</span><span class="sxs-lookup"><span data-stu-id="d3882-202">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="d3882-203">Kies of u automatisch een abonnement op commerciële Marketplace wilt vernieuwen</span><span class="sxs-lookup"><span data-stu-id="d3882-203">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="d3882-204">Actieve abonnementen zijn standaard ingesteld om automatisch te worden verlengd wanneer de abonnementsperiode verloopt.</span><span class="sxs-lookup"><span data-stu-id="d3882-204">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="d3882-205">Voor [abonnementen op commerciële Marketplace-Producten](csp-commercial-marketplace-overview.md)kunt u ervoor kiezen om het abonnement optioneel niet automatisch te vernieuwen.</span><span class="sxs-lookup"><span data-stu-id="d3882-205">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="d3882-206">Als u wilt voor komen dat een actief abonnement op commerciële Marketplace automatisch wordt vernieuwd:</span><span class="sxs-lookup"><span data-stu-id="d3882-206">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="d3882-207">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="d3882-207">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d3882-208">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="d3882-208">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d3882-209">Selecteer **Abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="d3882-209">Select **Subscriptions**.</span></span> <span data-ttu-id="d3882-210">Hier vindt u een overzicht van de op licenties gebaseerde abonnementen die u hebt aangeschaft voor de klant.</span><span class="sxs-lookup"><span data-stu-id="d3882-210">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="d3882-211">Selecteer in de kolom **abonnement** het abonnement dat u wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="d3882-211">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="d3882-212">Zoek op de pagina abonnements Details het gedeelte **status** en schakel het selectie vakje **automatisch verlengen** uit.</span><span class="sxs-lookup"><span data-stu-id="d3882-212">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="d3882-213">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="d3882-213">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d3882-214">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="d3882-214">Next steps</span></span>

- [<span data-ttu-id="d3882-215">Commerciële Marketplace-producten kopen voor uw klanten</span><span class="sxs-lookup"><span data-stu-id="d3882-215">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="d3882-216">Commerciële Marketplace-Producten voor uw klanten beheren</span><span class="sxs-lookup"><span data-stu-id="d3882-216">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="d3882-217">Overzicht van commerciële marketplace</span><span class="sxs-lookup"><span data-stu-id="d3882-217">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)