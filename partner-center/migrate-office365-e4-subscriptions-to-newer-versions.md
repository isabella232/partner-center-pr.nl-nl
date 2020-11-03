---
title: Office 365 E4-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enter prise E4 Edition wordt vanaf 7 april 2017 buiten gebruik gesteld. Meer informatie over het migreren van uw klanten abonnementen naar nieuwere versies van Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/03/2020
ms.locfileid: "92527477"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="37c3e-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions (Abonnementen op Office 365 E4 naar nieuwe versies van Office 365 migreren)</span><span class="sxs-lookup"><span data-stu-id="37c3e-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="37c3e-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="37c3e-105">**Applies to**</span></span>

-  <span data-ttu-id="37c3e-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="37c3e-106">Partner Center</span></span>

<span data-ttu-id="37c3e-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="37c3e-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="37c3e-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="37c3e-108">Global admin</span></span>
-   <span data-ttu-id="37c3e-109">Gebruikersbeheerder</span><span class="sxs-lookup"><span data-stu-id="37c3e-109">User admin</span></span>
-   <span data-ttu-id="37c3e-110">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="37c3e-110">Admin agent</span></span>
-   <span data-ttu-id="37c3e-111">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="37c3e-111">Sales agent</span></span>

<span data-ttu-id="37c3e-112">Het abonnement Office 365 Enter prise E4 wordt buiten gebruik gesteld, vanaf 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="37c3e-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="37c3e-113">U kunt na deze datum geen nieuwe Office 365 E4-abonnementen meer kopen en bestaande E4-abonnementen worden niet automatisch verlengd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="37c3e-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="37c3e-114">Wanneer E4-abonnementen eindigen, worden ze geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="37c3e-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="37c3e-115">Om ervoor te zorgen dat klanten zich kunnen voordoen, moet u klanten overstappen met het verloop van E4-abonnementen naar een ondersteunde SKU-optie, hieronder weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="37c3e-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="37c3e-116">U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.</span><span class="sxs-lookup"><span data-stu-id="37c3e-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="37c3e-117">Zowel Office 365 Enter prise E4 Commercial als Government Sku's worden buiten gebruik gesteld.</span><span class="sxs-lookup"><span data-stu-id="37c3e-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="37c3e-118">Op de detail pagina van het abonnement is de status van het E4-abonnement gewijzigd in ' verloopt op [date] ' van ' automatisch relateren op [date] '.</span><span class="sxs-lookup"><span data-stu-id="37c3e-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="37c3e-119">Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen detecteren door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren.</span><span class="sxs-lookup"><span data-stu-id="37c3e-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="37c3e-120">De E4-abonnementen worden ingesteld op automatisch verlengen = False in 7 april 2017.</span><span class="sxs-lookup"><span data-stu-id="37c3e-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="37c3e-121">U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="37c3e-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="37c3e-122">Vervangings plannen voor Office 365 Enter prise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="37c3e-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="37c3e-123">U kunt ervoor kiezen om dezelfde functionaliteit te onderhouden met E4, of uw klanten profiteren van nieuwere functies en functionaliteit in Office 365 en Skype voor bedrijven online.</span><span class="sxs-lookup"><span data-stu-id="37c3e-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="37c3e-124">Prijs informatie vindt u in de matrix prijs lijst en aanbiedings lijst in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="37c3e-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="37c3e-125">Veilig product Enter prise E3 of Secure productief Enter prise E5 kan worden vervangen door respectievelijk de volgende opties voor Office 365 Enter prise E3 of Office 365 Enter prise E5.</span><span class="sxs-lookup"><span data-stu-id="37c3e-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="37c3e-126">Optie 1: Office 365 Enter prise E5</span><span class="sxs-lookup"><span data-stu-id="37c3e-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="37c3e-127">Optie 2: Office 365 Enter prise E3 + Skype voor bedrijven cloud PBX</span><span class="sxs-lookup"><span data-stu-id="37c3e-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="37c3e-128">Optie 3: Office 365 Enter prise E3 + Skype voor bedrijven plus CAL (prijs-en functionaliteits pariteit met E4)</span><span class="sxs-lookup"><span data-stu-id="37c3e-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="37c3e-129">Optie 4: Office 365 Enter prise E3</span><span class="sxs-lookup"><span data-stu-id="37c3e-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="37c3e-130">Functie</span><span class="sxs-lookup"><span data-stu-id="37c3e-130">Feature</span></span> | <span data-ttu-id="37c3e-131">Optie 1</span><span class="sxs-lookup"><span data-stu-id="37c3e-131">Option 1</span></span> | <span data-ttu-id="37c3e-132">Optie 2</span><span class="sxs-lookup"><span data-stu-id="37c3e-132">Option 2</span></span> | <span data-ttu-id="37c3e-133">Optie 3</span><span class="sxs-lookup"><span data-stu-id="37c3e-133">Option 3</span></span> | <span data-ttu-id="37c3e-134">Optie 4</span><span class="sxs-lookup"><span data-stu-id="37c3e-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="37c3e-135">Alle functies uit Office 365 Enter prise E4 ophalen?</span><span class="sxs-lookup"><span data-stu-id="37c3e-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="37c3e-136">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-136">Yes</span></span> | <span data-ttu-id="37c3e-137">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-137">Yes</span></span> | <span data-ttu-id="37c3e-138">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-138">Yes</span></span> | <span data-ttu-id="37c3e-139">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-139">No</span></span> |
| <span data-ttu-id="37c3e-140">Telefoon nummers die worden beheerd in Office 365</span><span class="sxs-lookup"><span data-stu-id="37c3e-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="37c3e-141">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-141">Yes</span></span> | <span data-ttu-id="37c3e-142">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-142">Yes</span></span> | <span data-ttu-id="37c3e-143">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-143">No</span></span> | <span data-ttu-id="37c3e-144">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-144">No</span></span> |
| <span data-ttu-id="37c3e-145">Telefoon nummers die zowel on-premises als in Office 365 (hybride implementatie) worden beheerd</span><span class="sxs-lookup"><span data-stu-id="37c3e-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="37c3e-146">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-146">Yes</span></span> | <span data-ttu-id="37c3e-147">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-147">Yes</span></span> | <span data-ttu-id="37c3e-148">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-148">No</span></span> | <span data-ttu-id="37c3e-149">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-149">No</span></span> |
| <span data-ttu-id="37c3e-150">Optie voor het toevoegen van een PSTN-telefoon gespreks plan?</span><span class="sxs-lookup"><span data-stu-id="37c3e-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="37c3e-151">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-151">Yes</span></span> | <span data-ttu-id="37c3e-152">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-152">Yes</span></span> | <span data-ttu-id="37c3e-153">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-153">No</span></span> | <span data-ttu-id="37c3e-154">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-154">No</span></span> |
| <span data-ttu-id="37c3e-155">PSTN-vergaderingen?</span><span class="sxs-lookup"><span data-stu-id="37c3e-155">PSTN Conferencing?</span></span> | <span data-ttu-id="37c3e-156">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-156">Yes</span></span> | <span data-ttu-id="37c3e-157">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-157">No</span></span> | <span data-ttu-id="37c3e-158">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-158">No</span></span> | <span data-ttu-id="37c3e-159">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-159">No</span></span> |
| <span data-ttu-id="37c3e-160">Geavanceerde hulp middelen voor samen werking, analyses en beveiliging?</span><span class="sxs-lookup"><span data-stu-id="37c3e-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="37c3e-161">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-161">Yes</span></span> | <span data-ttu-id="37c3e-162">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-162">No</span></span> | <span data-ttu-id="37c3e-163">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-163">No</span></span> | <span data-ttu-id="37c3e-164">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-164">No</span></span> |
| <span data-ttu-id="37c3e-165">Interactieve rapporten, Dash boards en gegevens visualisaties?</span><span class="sxs-lookup"><span data-stu-id="37c3e-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="37c3e-166">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-166">Yes</span></span> | <span data-ttu-id="37c3e-167">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-167">No</span></span> | <span data-ttu-id="37c3e-168">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-168">No</span></span> | <span data-ttu-id="37c3e-169">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-169">No</span></span> | 
| <span data-ttu-id="37c3e-170">Meer controle over de beveiliging van gegevens en naleving van ingebouwde privacy-, transparantie-en verfijnde gebruikers besturings elementen?</span><span class="sxs-lookup"><span data-stu-id="37c3e-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="37c3e-171">Ja</span><span class="sxs-lookup"><span data-stu-id="37c3e-171">Yes</span></span> | <span data-ttu-id="37c3e-172">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-172">No</span></span> | <span data-ttu-id="37c3e-173">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-173">No</span></span> | <span data-ttu-id="37c3e-174">Nee</span><span class="sxs-lookup"><span data-stu-id="37c3e-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="37c3e-175">Klanten overstappen naar nieuwe product abonnementen</span><span class="sxs-lookup"><span data-stu-id="37c3e-175">Transition customers to new product plans</span></span>

<span data-ttu-id="37c3e-176">Micro soft biedt voortdurend nieuwe producten en services aan onze partners.</span><span class="sxs-lookup"><span data-stu-id="37c3e-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="37c3e-177">In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren vanuit Sku's die uiteindelijk worden afgesloten.</span><span class="sxs-lookup"><span data-stu-id="37c3e-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="37c3e-178">Voor het migreren van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="37c3e-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="37c3e-179">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="37c3e-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="37c3e-180">Huidige gebruikers licenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="37c3e-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="37c3e-181">Het oude abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="37c3e-181">Cancel the old subscription</span></span>

<span data-ttu-id="37c3e-182">Voer de volgende stappen uit om het Office 365 Enter prise E4-abonnement van de klant te migreren naar een van de opties in de bovenstaande tabel.</span><span class="sxs-lookup"><span data-stu-id="37c3e-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="37c3e-183">Stap 1: het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="37c3e-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="37c3e-184">Selecteer in het menu **Partner Center** **klanten** , selecteer de klant die u wilt verplaatsen en selecteer vervolgens **abonnementen toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-184">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Add subscriptions** .</span></span>

2. <span data-ttu-id="37c3e-185">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span>

   <span data-ttu-id="37c3e-186">Uw klant moet nu over zowel oude als nieuwe abonnementen beschikken, het oude Office 365 Enter prise E4-abonnement en het nieuwe ' target '-abonnement, bijvoorbeeld optie 1-Office 365 Enter prise E5.</span><span class="sxs-lookup"><span data-stu-id="37c3e-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="37c3e-187">Stap 2: de gebruikers licenties van de klant opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="37c3e-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="37c3e-188">Selecteer in het menu **Partner Center** **klanten** , selecteer de klant die u wilt verplaatsen en selecteer vervolgens **gebruikers en licenties** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-188">From the **Partner Center** menu, select **Customers** , select the customer you wish to move, and then select **Users and licenses** .</span></span> <span data-ttu-id="37c3e-189">De pagina gebruikers en licenties van de klant wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="37c3e-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="37c3e-190">Als u gebruikers licenties opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u vervolgens **licenties beheren** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses** .</span></span>

3. <span data-ttu-id="37c3e-191">Schakel op de pagina **licenties beheren** het selectie vakje **Office 365 Enter prise E4** -licentie uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.</span><span class="sxs-lookup"><span data-stu-id="37c3e-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="37c3e-192">Selecteer **Indienen** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-192">Select **Submit** .</span></span> <span data-ttu-id="37c3e-193">Een bevestigings pagina bevat een lijst met de nieuwe licentie toewijzingen.</span><span class="sxs-lookup"><span data-stu-id="37c3e-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="37c3e-194">Herhaal dezelfde stappen met andere gebruikers van klanten die de licentie opnieuw moeten toewijzen.</span><span class="sxs-lookup"><span data-stu-id="37c3e-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="37c3e-195">Nadat u de gebruikers licenties naar de nieuwe service hebt verplaatst, kunt u het buiten gebruik gestelde abonnement op het hoogste klant niveau gewoon annuleren.</span><span class="sxs-lookup"><span data-stu-id="37c3e-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="37c3e-196">Stap 3: het oude abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="37c3e-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="37c3e-197">Selecteer in het menu **Partner Center** **klanten** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-197">From the **Partner Center** menu, select **Customers** .</span></span> <span data-ttu-id="37c3e-198">Selecteer de klant die u wilt verplaatsen en selecteer het abonnement dat u wilt annuleren.</span><span class="sxs-lookup"><span data-stu-id="37c3e-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="37c3e-199">Stel op de pagina abonnements Details de status van het abonnement in op **opgeschort** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-199">In the subscription details page, set the subscription status to **Suspended** .</span></span>

3. <span data-ttu-id="37c3e-200">Selecteer **Indienen** .</span><span class="sxs-lookup"><span data-stu-id="37c3e-200">Select **Submit** .</span></span>

<span data-ttu-id="37c3e-201">Het oude abonnement is onderbroken en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="37c3e-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="37c3e-202">Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht.</span><span class="sxs-lookup"><span data-stu-id="37c3e-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="37c3e-203">De klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="37c3e-203">The customer incurs no additional costs for the old subscription.</span></span>



 



