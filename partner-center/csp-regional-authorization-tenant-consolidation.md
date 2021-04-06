---
title: Tenant consolidatie CSP regionale autorisatie
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze instructies voor het consolideren van tenants voor verschillende landen/regio's. Dit omvat stappen voor het migreren van klant accounts en klant abonnementen.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502567"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="d4e40-104">Instructies voor tenantconsolidatie voor regionale autorisatie in CSP</span><span class="sxs-lookup"><span data-stu-id="d4e40-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="d4e40-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="d4e40-105">**Applies to**</span></span>

- <span data-ttu-id="d4e40-106">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="d4e40-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="d4e40-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="d4e40-107">**Appropriate roles**</span></span>

- <span data-ttu-id="d4e40-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="d4e40-108">Global admin</span></span>
- <span data-ttu-id="d4e40-109">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="d4e40-109">Admin agent</span></span>

<span data-ttu-id="d4e40-110">\[Sommige informatie is gekoppeld aan een vooraf vrijgegeven product dat ingrijpend kan worden gewijzigd voordat het commercieel wordt uitgebracht.</span><span class="sxs-lookup"><span data-stu-id="d4e40-110">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="d4e40-111">Microsoft biedt geen enkele expliciete of impliciete garanties met betrekking tot de informatie die hier wordt verstrekt.\]</span><span class="sxs-lookup"><span data-stu-id="d4e40-111">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="d4e40-112">U kunt tenants voor uw bedrijf consolideren.</span><span class="sxs-lookup"><span data-stu-id="d4e40-112">You can consolidate tenants for your business.</span></span> <span data-ttu-id="d4e40-113">Gebruik deze instructies voor het consolideren van tenants voor verschillende landen/regio's.</span><span class="sxs-lookup"><span data-stu-id="d4e40-113">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="d4e40-114">U moet rekening houden met alle ingerichte abonnementen en het aantal licenties voor elk van uw klanten in het account dat u wilt overstappen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-114">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="d4e40-115">U kunt dezelfde exacte abonnementen met dezelfde licentie aantallen onder het nieuwe centrale CSP-account opnieuw inrichten als onderdeel van het migratie proces.</span><span class="sxs-lookup"><span data-stu-id="d4e40-115">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="d4e40-116">Gebruik de functie lijst exporteren om een lijst met klanten te maken waarmee u naar de gecentraliseerde Tenant kunt gaan.</span><span class="sxs-lookup"><span data-stu-id="d4e40-116">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="d4e40-117">Zodra de consolidatie is voltooid, kunt u niet terugkeren naar de vorige Tenant status.</span><span class="sxs-lookup"><span data-stu-id="d4e40-117">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="d4e40-118">De klant actie kan ook vereist zijn.</span><span class="sxs-lookup"><span data-stu-id="d4e40-118">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="d4e40-119">Voorbereiden op migratie</span><span class="sxs-lookup"><span data-stu-id="d4e40-119">Prepare for migration</span></span>

- <span data-ttu-id="d4e40-120">Meld u aan bij het **partner centrum**  met het **overgangs** account (het abonnement dat u wilt overstappen naar het nieuwe account) en Bekijk alle klanten en alle services die voor deze klanten zijn ingericht.</span><span class="sxs-lookup"><span data-stu-id="d4e40-120">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="d4e40-121">Meld u af bij dit account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-121">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="d4e40-122">Klant accounts migreren</span><span class="sxs-lookup"><span data-stu-id="d4e40-122">Migrate customer accounts</span></span>

1. <span data-ttu-id="d4e40-123">Meld u aan bij het **partner centrum**  met het **overgangs** -(nieuwe) account (het abonnement dat u aan klanten overstapt).</span><span class="sxs-lookup"><span data-stu-id="d4e40-123">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="d4e40-124">Selecteer **Klanten**.</span><span class="sxs-lookup"><span data-stu-id="d4e40-124">Select **Customers**.</span></span>

3. <span data-ttu-id="d4e40-125">Selecteer **een reseller-relatie aanvragen**.</span><span class="sxs-lookup"><span data-stu-id="d4e40-125">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="d4e40-126">Er wordt een standaard e-mail bericht weer gegeven dat u naar uw klanten kunt verzenden.</span><span class="sxs-lookup"><span data-stu-id="d4e40-126">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="d4e40-127">Dit bericht bevat een URL met de organisatie-ID die uniek is voor uw nieuwe partner Center-account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-127">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="d4e40-128">**Actie van klant:** Zorg ervoor dat alle actieve klanten die u wilt migreren, deze URL bezoeken.</span><span class="sxs-lookup"><span data-stu-id="d4e40-128">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="d4e40-129">Bij het openen van de URL wordt de klant gevraagd zich aan te melden bij de Office 365-Portal.</span><span class="sxs-lookup"><span data-stu-id="d4e40-129">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="d4e40-130">De klant meldt zich aan met dezelfde organisatie-ID die ze gebruiken voor toegang tot de beheer portals van Azure en Office 365.</span><span class="sxs-lookup"><span data-stu-id="d4e40-130">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="d4e40-131">Nadat u zich hebt aangemeld, wordt de globale beheerder voor het **klant account** gevraagd om een overeenkomst in te dienen die gedelegeerde beheerders bevoegdheden aan het nieuwe CSP-account verleent.</span><span class="sxs-lookup"><span data-stu-id="d4e40-131">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="d4e40-132">Als ze akkoord gaan, selecteert de klant het selectie vakje en gaat ermee akkoord de relatie te autoriseren.</span><span class="sxs-lookup"><span data-stu-id="d4e40-132">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="d4e40-133">De klanten worden weer gegeven in de klanten lijst van de partner nadat ze de overeenkomst één voor één hebben ingediend.</span><span class="sxs-lookup"><span data-stu-id="d4e40-133">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="d4e40-134">Office 365 en niet-Azure-op gebruik gebaseerde abonnementen migreren</span><span class="sxs-lookup"><span data-stu-id="d4e40-134">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="d4e40-135">Zodra uw klant de overeenkomst heeft ondertekend, kunt u hun abonnementen opnieuw maken onder uw gecentraliseerde partner-Tenant.</span><span class="sxs-lookup"><span data-stu-id="d4e40-135">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="d4e40-136">Selecteer **klanten** in het **partner centrum**.</span><span class="sxs-lookup"><span data-stu-id="d4e40-136">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="d4e40-137">Open de bedrijfs naam voor de klant die u wilt migreren.</span><span class="sxs-lookup"><span data-stu-id="d4e40-137">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="d4e40-138">Selecteer **abonnement toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="d4e40-138">Select **Add subscription**.</span></span>

5. <span data-ttu-id="d4e40-139">Voeg de juiste abonnementen en licentie aantallen toe vanuit de catalogus.</span><span class="sxs-lookup"><span data-stu-id="d4e40-139">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="d4e40-140">Controleer met de informatie in de **overgang van** partner accounts.</span><span class="sxs-lookup"><span data-stu-id="d4e40-140">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="klanten lijst":::

6. <span data-ttu-id="d4e40-142">Selecteer **verzenden.**</span><span class="sxs-lookup"><span data-stu-id="d4e40-142">Select **Submit.**</span></span>

   <span data-ttu-id="d4e40-143">De services worden nu aan de klant door gegeven van de **overgang naar** het partner account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-143">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="d4e40-144">Herhaal deze stappen om abonnementen voor alle extra klanten te migreren.</span><span class="sxs-lookup"><span data-stu-id="d4e40-144">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="d4e40-145">Voordat u doorgaat naar de volgende sectie, moet u ervoor zorgen dat alle abonnementen van klanten die zijn gemaakt onder de **overgang van** partner accounts, opnieuw worden ingericht onder de **overgang naar** het partner account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-145">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="d4e40-146">Partners moeten abonnementen opschorten voor de **overgang van** het partner Tenant account in het partner centrum op dezelfde dag dat deze abonnementen worden overgezet en ingesteld onder de **overgang naar** het Tenant account van de partner in het partner centrum om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="d4e40-146">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="d4e40-147">Ondersteunings aanvragen worden afgewezen als gevolg van een overlap ping in de facturering, waardoor de **overgang** van abonnementen niet correct wordt uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d4e40-147">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="d4e40-148">De Office 365-abonnementen uitschakelen onder de overgang van partner-account</span><span class="sxs-lookup"><span data-stu-id="d4e40-148">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="d4e40-149">Als u het CSP-abonnement uitschakelt onder de **overgang van** partner accounts, wordt een toekomstige facturering stopgezet.</span><span class="sxs-lookup"><span data-stu-id="d4e40-149">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="d4e40-150">U hoeft Azure-abonnementen niet hand matig uit te scha kelen, omdat Azure-abonnementen tijdens het migratie proces automatisch worden uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d4e40-150">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="d4e40-151">Meld u aan bij het **partner centrum** met de **overgang van** het CSP-account en navigeer naar de klanten lijst.</span><span class="sxs-lookup"><span data-stu-id="d4e40-151">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="d4e40-152">Open de klant met abonnementen om uit te scha kelen en selecteer vervolgens de eerste aanbieding die u wilt uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-152">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="d4e40-153">Stel het abonnement in op **opgeschort** en selecteer vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="d4e40-153">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="d4e40-154">Het onderbreken van het abonnement zorgt ervoor dat er geen dubbele facturering plaatsvindt.</span><span class="sxs-lookup"><span data-stu-id="d4e40-154">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="d4e40-155">Het abonnement wordt **uitgesteld** weer gegeven in de lijst abonnementen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-155">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="d4e40-156">Herhaal deze stappen voor alle abonnementen onder de klant.</span><span class="sxs-lookup"><span data-stu-id="d4e40-156">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="d4e40-157">Zorg ervoor dat alle weer geven zijn **onderbroken.**</span><span class="sxs-lookup"><span data-stu-id="d4e40-157">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="d4e40-158">Selecteer de volgende klant in de lijst en herhaal het proces voor het uitschakelen van alle abonnementen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-158">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="d4e40-159">Op Azure-gebruik gebaseerde abonnementen migreren</span><span class="sxs-lookup"><span data-stu-id="d4e40-159">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="d4e40-160">In tegens telling tot de Office 365 CSP-abonnementen, hoeven Azure CSP-abonnementen op basis van gebruik niet hand matig te worden gemigreerd.</span><span class="sxs-lookup"><span data-stu-id="d4e40-160">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="d4e40-161">Met de ondersteuning van Microsoft Azure worden de Azure-abonnementen en alle geïmplementeerde Services of resources gemigreerd van de overschakeling **van** de CSP-reseller-accounts **naar de CSP** -reseller-account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-161">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="d4e40-162">Er is geen onderbreking van de service voor de klant tijdens deze overgang.</span><span class="sxs-lookup"><span data-stu-id="d4e40-162">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="d4e40-163">Zorg ervoor dat de klant accounts die Azure-abonnementen hebben gemigreerd, de overeenkomst hebben geaccepteerd om te koppelen aan de nieuwe **overgang naar** het CSP-account.</span><span class="sxs-lookup"><span data-stu-id="d4e40-163">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="d4e40-164">U ontvangt een melding van micro soft van welke klant accounts klaar zijn om te migreren, en bieden de bedrijfs namen van die klant.</span><span class="sxs-lookup"><span data-stu-id="d4e40-164">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="d4e40-165">Micro soft migreert de op Azure-gebruik gebaseerde abonnementen en brengt u op de hoogte wanneer de migratie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="d4e40-165">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="d4e40-166">U moet bevestigen dat het Azure-abonnement onder de **overstap van** het CSP-reseller-account nu is gemarkeerd als **opgeschort** in het partner centrum in het gedeelte klant abonnementen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-166">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="d4e40-167">Controleer of het Azure-abonnement onder de **overgang naar** het CSP-reseller-account nu de status **actief** in Partner Center weergeeft in het gedeelte klant abonnementen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-167">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="d4e40-168">Het uitschakelen van de abonnementen onder de klant heeft geen invloed op de weer gave van de klant in de lijst klanten.</span><span class="sxs-lookup"><span data-stu-id="d4e40-168">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="d4e40-169">Er is momenteel geen optie om klanten te verwijderen uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="d4e40-169">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="d4e40-170">Partners moeten voor komen dat abonnementen worden toegevoegd aan deze klanten via hun **overgang van** account in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="d4e40-170">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="d4e40-171">Herhaal deze stappen voor alle abonnementen onder al uw klanten om toekomstige kosten te stoppen voor de **overgang van** een of meer accounts.</span><span class="sxs-lookup"><span data-stu-id="d4e40-171">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="d4e40-172">De partner ontvangt één definitieve factuur met een tegoed voor het aantal ongebruikte dagen tussen de dag van de annulering en de laatste dag van de facturerings periode.</span><span class="sxs-lookup"><span data-stu-id="d4e40-172">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="d4e40-173">Er worden geen toekomstige facturen gegenereerd na de laatste facturerings periode.</span><span class="sxs-lookup"><span data-stu-id="d4e40-173">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="d4e40-174">Aanvullende informatie</span><span class="sxs-lookup"><span data-stu-id="d4e40-174">Additional information</span></span>

- <span data-ttu-id="d4e40-175">Het uitschakelen **van het abonnement van de CSP-** account heeft geen invloed op de service van de eind klant zolang de service is ingericht van de **overgang naar** het CSP-account voordat het abonnement is uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="d4e40-175">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="d4e40-176">Abonnementen kunnen niet worden gebruikt door de klant en er worden geen kosten in rekening gebracht wanneer deze zijn onderbroken of geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="d4e40-176">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="d4e40-177">Er is momenteel geen manier om een klant volledig uit de lijst met **klanten** te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="d4e40-177">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="d4e40-178">Partners moeten abonnementen opschorten voor de **overgang van** het partner Tenant account in het partner centrum op dezelfde dag dat deze abonnementen worden overgezet en ingesteld op basis van de **overgang naar** het account om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="d4e40-178">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="d4e40-179">Micro soft biedt geen ondersteuning voor tegoed aanvragen als gevolg van een overlap ping in de facturering, waardoor de **overgang** van abonnementen naar opgeschort niet goed kan worden ingesteld.</span><span class="sxs-lookup"><span data-stu-id="d4e40-179">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="d4e40-180">Migratie vereenvoudigen met exporteren</span><span class="sxs-lookup"><span data-stu-id="d4e40-180">Simplify migration using Export</span></span>

<span data-ttu-id="d4e40-181">Met de **functie exporteren** kunt u de abonnementen vastleggen die u moet gebruiken in de nieuwe geconsolideerde structuur:</span><span class="sxs-lookup"><span data-stu-id="d4e40-181">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="d4e40-182">Selecteer **klanten** in het partner centrum om de lijst met klanten te bekijken.</span><span class="sxs-lookup"><span data-stu-id="d4e40-182">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="d4e40-183">Open de naam van de gewenste klant.</span><span class="sxs-lookup"><span data-stu-id="d4e40-183">Open the desired customer name.</span></span>

3. <span data-ttu-id="d4e40-184">Selecteer op de pagina **abonnementen** de optie **abonnementen exporteren** om de details van abonnementen te exporteren naar een Excel-bestand.</span><span class="sxs-lookup"><span data-stu-id="d4e40-184">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="d4e40-185">Gebruik deze lijst om de abonnementen in uw nieuwe geconsolideerde Tenant opnieuw te maken.</span><span class="sxs-lookup"><span data-stu-id="d4e40-185">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="d4e40-186">API-registratie</span><span class="sxs-lookup"><span data-stu-id="d4e40-186">API registration</span></span>

<span data-ttu-id="d4e40-187">Zie [API-toegang instellen in partner centrum](/partner-center/develop/set-up-api-access-in-partner-center)voor meer informatie over API-registratie.</span><span class="sxs-lookup"><span data-stu-id="d4e40-187">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d4e40-188">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="d4e40-188">Next steps</span></span>

- [<span data-ttu-id="d4e40-189">Cloud Solution Provider-programma regionale markten en valuta's waar u CSP-aanbiedingen kunt verkopen</span><span class="sxs-lookup"><span data-stu-id="d4e40-189">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
