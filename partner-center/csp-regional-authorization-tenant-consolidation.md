---
title: Regionale CSP-autorisatie tenantconsolidatie
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze instructies om tenants te consolideren voor verschillende landen/regio's. Dit omvat stappen voor het migreren van klantaccounts en klantabonnementen.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147578"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="afe94-104">Instructies voor tenantconsolidatie voor regionale autorisatie in CSP</span><span class="sxs-lookup"><span data-stu-id="afe94-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="afe94-105">**Van toepassing op**: Partner Center | Partner Center for Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="afe94-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="afe94-106">**Juiste rollen:** Globale | Beheeragent</span><span class="sxs-lookup"><span data-stu-id="afe94-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="afe94-107">\[Sommige informatie heeft betrekking op vooraf uitgebracht product dat aanzienlijk kan worden gewijzigd voordat het commercieel wordt uitgebracht.</span><span class="sxs-lookup"><span data-stu-id="afe94-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="afe94-108">Microsoft biedt geen enkele expliciete of impliciete garanties met betrekking tot de informatie die hier wordt verstrekt.\]</span><span class="sxs-lookup"><span data-stu-id="afe94-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="afe94-109">U kunt tenants consolideren voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="afe94-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="afe94-110">Gebruik deze instructies om tenants te consolideren voor verschillende landen/regio's.</span><span class="sxs-lookup"><span data-stu-id="afe94-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="afe94-111">U moet rekening houden met alle inrichtende abonnementen en het aantal licenties voor elk van uw klanten in het account van waar u over overstapt.</span><span class="sxs-lookup"><span data-stu-id="afe94-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="afe94-112">U gaat dezelfde exacte abonnementen met dezelfde licentietellingen opnieuw inrichten onder het nieuwe centrale CSP-account als onderdeel van het migratieproces.</span><span class="sxs-lookup"><span data-stu-id="afe94-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="afe94-113">Gebruik de exportlijstfunctie om een lijst met klanten te maken om over te gaan naar de gecentraliseerde tenant.</span><span class="sxs-lookup"><span data-stu-id="afe94-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="afe94-114">Zodra de consolidatie is voltooid, kunt u niet terugkeren naar de vorige tenanttoestand.</span><span class="sxs-lookup"><span data-stu-id="afe94-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="afe94-115">De actie van de klant is mogelijk ook vereist.</span><span class="sxs-lookup"><span data-stu-id="afe94-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="afe94-116">Voorbereiden op migratie</span><span class="sxs-lookup"><span data-stu-id="afe94-116">Prepare for migration</span></span>

- <span data-ttu-id="afe94-117">Meld u **aan bij Partner Center** het overgangsaccount (het account dat u wilt overstappen naar het nieuwe account) en controleer alle klanten en alle services die voor deze klanten zijn ingericht. </span><span class="sxs-lookup"><span data-stu-id="afe94-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="afe94-118">Meld u af bij dit account.</span><span class="sxs-lookup"><span data-stu-id="afe94-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="afe94-119">Klantaccounts migreren</span><span class="sxs-lookup"><span data-stu-id="afe94-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="afe94-120">Meld u aan **Partner Center**  met het **(nieuwe)** overgangsaccount (het account waarin u klanten over wilt zetten).</span><span class="sxs-lookup"><span data-stu-id="afe94-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="afe94-121">Selecteer **Klanten**.</span><span class="sxs-lookup"><span data-stu-id="afe94-121">Select **Customers**.</span></span>

3. <span data-ttu-id="afe94-122">Selecteer **Een resellerrelatie aanvragen.**</span><span class="sxs-lookup"><span data-stu-id="afe94-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="afe94-123">U krijgt een standaard-e-mailbericht te zien dat u naar uw klanten kunt verzenden.</span><span class="sxs-lookup"><span data-stu-id="afe94-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="afe94-124">Dit bericht bevat een URL met de organisatie-id die uniek is voor uw nieuwe Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="afe94-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="afe94-125">**Actie van de klant:** Zorg ervoor dat elk van de actieve klanten die u wilt migreren deze URL bezoekt.</span><span class="sxs-lookup"><span data-stu-id="afe94-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="afe94-126">Bij het openen van de URL wordt de klant gevraagd zich aan te melden bij de Office 365-portal.</span><span class="sxs-lookup"><span data-stu-id="afe94-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="afe94-127">De klant meldt zich aan met dezelfde organisatie-id die hij gebruikt voor toegang tot de Azure- en Office 365-beheerportals.</span><span class="sxs-lookup"><span data-stu-id="afe94-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="afe94-128">Na het aanmelden wordt de globale beheerder voor het **klantaccount** gevraagd een overeenkomst in te dienen die gedelegeerde beheerdersbevoegdheden voor het nieuwe CSP-account biedt.</span><span class="sxs-lookup"><span data-stu-id="afe94-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="afe94-129">Als de klant akkoord gaat, wordt het selectievakje in het selectievakje geselecteerd en wordt de relatie geautoriseerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="afe94-130">De klanten worden één voor één weergegeven in de klantenlijst van de partner nadat ze de overeenkomst hebben ingediend.</span><span class="sxs-lookup"><span data-stu-id="afe94-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="afe94-131">Office 365- en niet-Azure-abonnementen op basis van gebruik migreren</span><span class="sxs-lookup"><span data-stu-id="afe94-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="afe94-132">Zodra uw klant de overeenkomst heeft ondertekend, kunt u de abonnementen opnieuw maken onder uw gecentraliseerde partnerten tenant.</span><span class="sxs-lookup"><span data-stu-id="afe94-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="afe94-133">Selecteer **Partner Center** in **het bestand .**</span><span class="sxs-lookup"><span data-stu-id="afe94-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="afe94-134">Open de bedrijfsnaam voor de klant die u wilt migreren.</span><span class="sxs-lookup"><span data-stu-id="afe94-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="afe94-135">Selecteer **Abonnement toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="afe94-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="afe94-136">Voeg de juiste abonnementen en het aantal licenties uit de catalogus toe.</span><span class="sxs-lookup"><span data-stu-id="afe94-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="afe94-137">Controleer met de informatie in de **overgang van** partneraccounts.</span><span class="sxs-lookup"><span data-stu-id="afe94-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="klantenlijst":::

6. <span data-ttu-id="afe94-139">Selecteer **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="afe94-139">Select **Submit.**</span></span>

   <span data-ttu-id="afe94-140">De services worden nu aan de klant geleverd vanuit het **overgangsaccount naar** het partneraccount.</span><span class="sxs-lookup"><span data-stu-id="afe94-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="afe94-141">Herhaal deze stappen om abonnementen voor alle extra klanten te migreren.</span><span class="sxs-lookup"><span data-stu-id="afe94-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="afe94-142">Voordat u doorgaat met de volgende sectie,  moet u ervoor zorgen dat alle bestaande klantabonnementen onder de overgang van partneraccounts opnieuw worden ingericht onder het overgangsaccount **naar** partneraccount.</span><span class="sxs-lookup"><span data-stu-id="afe94-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="afe94-143">Partners moeten abonnementen op het account **Transitioning From** Partner Tenant in Partner Center op dezelfde dag dat deze abonnementen worden overge zetten en ingesteld onder het **transitioning to** Partner Tenant-account in de Partner Center om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="afe94-144">Ondersteuningsaanvragen worden geweigerd voor tegoeden vanwege overlappingen in facturering die zich voordoen door het niet juist uitschakelen van de overgang van **abonnementen.**</span><span class="sxs-lookup"><span data-stu-id="afe94-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="afe94-145">De Office 365-abonnementen uitschakelen onder Het partneraccount overstappen</span><span class="sxs-lookup"><span data-stu-id="afe94-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="afe94-146">Het uitschakelen van het CSP-abonnement onder de **overgang van** partneraccounts stopt toekomstige facturering.</span><span class="sxs-lookup"><span data-stu-id="afe94-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="afe94-147">U hoeft Azure-abonnementen niet handmatig uit te schakelen, omdat Azure-abonnementen automatisch worden uitgeschakeld tijdens het migratieproces.</span><span class="sxs-lookup"><span data-stu-id="afe94-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="afe94-148">Meld u aan bij **Partner Center** **CSP-account** en navigeer naar de lijst met klanten.</span><span class="sxs-lookup"><span data-stu-id="afe94-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="afe94-149">Open de klant met abonnementen die u wilt uitschakelen en selecteer vervolgens de eerste aanbieding die u wilt uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="afe94-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="afe94-150">Stel het abonnement in op **Tijdelijk en** selecteer **verzenden.**</span><span class="sxs-lookup"><span data-stu-id="afe94-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="afe94-151">Door het abonnement op te schorten, wordt er geen dubbele facturering uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="afe94-152">Het abonnement wordt **tijdelijk in de** lijst met abonnementen weergegeven.</span><span class="sxs-lookup"><span data-stu-id="afe94-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="afe94-153">Herhaal deze stappen voor alle abonnementen onder de klant.</span><span class="sxs-lookup"><span data-stu-id="afe94-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="afe94-154">Controleer of alles is **opgeschort.**</span><span class="sxs-lookup"><span data-stu-id="afe94-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="afe94-155">Selecteer de volgende klant in de lijst en herhaal het proces van het uitschakelen van alle abonnementen.</span><span class="sxs-lookup"><span data-stu-id="afe94-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="afe94-156">Azure-abonnementen op basis van gebruik migreren</span><span class="sxs-lookup"><span data-stu-id="afe94-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="afe94-157">In tegenstelling tot de Office 365 CSP-abonnementen hoeven Op gebruik gebaseerde CSP-abonnementen niet handmatig te worden gemigreerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="afe94-158">Microsoft Azure-ondersteuning worden de Azure-abonnementen en alle geïmplementeerde services  of resources gemigreerd van de overgang van CSP-reselleraccounts naar het overstappen naar het CSP-reselleraccount. </span><span class="sxs-lookup"><span data-stu-id="afe94-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="afe94-159">Er is geen onderbreking van de service voor de klant tijdens deze overgang.</span><span class="sxs-lookup"><span data-stu-id="afe94-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="afe94-160">Zorg ervoor dat de klantaccounts met gemigreerde Azure-abonnementen de overeenkomst hebben geaccepteerd om te worden gekoppeld aan het nieuwe **Overgang** naar CSP-account.</span><span class="sxs-lookup"><span data-stu-id="afe94-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="afe94-161">U informeert Microsoft over welke klantaccounts gereed zijn om te worden gemigreerd en geeft de bedrijfsnamen van die klanten op.</span><span class="sxs-lookup"><span data-stu-id="afe94-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="afe94-162">Microsoft migreert de azure-abonnementen op basis van gebruik en waarschuwt u wanneer de migratie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="afe94-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="afe94-163">U moet controleren of het Azure-abonnement onder het reselleraccount Overstappen van **CSP** nu is gemarkeerd **als** tijdelijk Partner Center onder de sectie Klantabonnementen.</span><span class="sxs-lookup"><span data-stu-id="afe94-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="afe94-164">Controleer of in het Azure-abonnement onder het overstappen naar **het** CSP-reselleraccount nu de status actief **wordt** Partner Center onder de sectie Klantabonnementen.</span><span class="sxs-lookup"><span data-stu-id="afe94-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="afe94-165">Het uitschakelen van de abonnementen onder de klant verandert niet het uiterlijk van de klant in de lijst Klanten.</span><span class="sxs-lookup"><span data-stu-id="afe94-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="afe94-166">Er is momenteel geen optie om klanten uit de lijst te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="afe94-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="afe94-167">Partners moeten voorkomen dat ze in de toekomst abonnementen aan deze klanten toevoegen vanuit hun **Overgang van-account.**</span><span class="sxs-lookup"><span data-stu-id="afe94-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="afe94-168">Herhaal deze stappen voor alle abonnementen onder al uw  klanten om toekomstige kosten voor de overgang van account(en) te stoppen.</span><span class="sxs-lookup"><span data-stu-id="afe94-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="afe94-169">De partner ontvangt één definitieve factuur met een tegoed voor het aantal ongebruikte dagen tussen de dag van annulering en de laatste dag van de factureringsperiode.</span><span class="sxs-lookup"><span data-stu-id="afe94-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="afe94-170">Er worden geen toekomstige facturen gegenereerd na die laatste factureringsperiode.</span><span class="sxs-lookup"><span data-stu-id="afe94-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="afe94-171">Aanvullende informatie</span><span class="sxs-lookup"><span data-stu-id="afe94-171">Additional information</span></span>

- <span data-ttu-id="afe94-172">Het uitschakelen van het  abonnement van het CSP-account voor overstappen heeft geen invloed op de service van de eindklant zolang de service is ingericht vanuit het overgangsaccount naar **het** CSP-account voordat het abonnement werd uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="afe94-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="afe94-173">Abonnementen kunnen niet worden gebruikt door de klant en genereren geen kosten wanneer ze worden opgeschort of geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="afe94-174">Er is momenteel geen manier om een klant volledig te verwijderen uit de **lijst Klanten.**</span><span class="sxs-lookup"><span data-stu-id="afe94-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="afe94-175">Partners moeten abonnementen op het tenantaccount van de **partner** overstappen in Partner Center op dezelfde dag dat deze abonnementen worden overgemaakt naar en ingesteld onder het overgangsaccount naar **account** om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="afe94-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="afe94-176">Microsoft biedt geen ondersteuning voor aanvragen voor tegoeden als gevolg  van overlappingen in de facturering die optreden door het niet juist instellen van de overgang van abonnementen naar opgeschort.</span><span class="sxs-lookup"><span data-stu-id="afe94-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="afe94-177">Migratie vereenvoudigen met behulp van Exporteren</span><span class="sxs-lookup"><span data-stu-id="afe94-177">Simplify migration using Export</span></span>

<span data-ttu-id="afe94-178">Met de **functie Exporteren** kunt u de abonnementen vastleggen die u moet gebruiken in uw nieuwe geconsolideerde structuur:</span><span class="sxs-lookup"><span data-stu-id="afe94-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="afe94-179">Selecteer **Klanten** op Partner Center om de lijst met klanten weer te geven.</span><span class="sxs-lookup"><span data-stu-id="afe94-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="afe94-180">Open de gewenste klantnaam.</span><span class="sxs-lookup"><span data-stu-id="afe94-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="afe94-181">Selecteer op **de pagina Abonnementen** de optie Abonnementen exporteren **om** details van abonnementen naar een Excel-bestand te exporteren.</span><span class="sxs-lookup"><span data-stu-id="afe94-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="afe94-182">Gebruik deze lijst om de abonnementen in uw nieuwe geconsolideerde tenant opnieuw te maken.</span><span class="sxs-lookup"><span data-stu-id="afe94-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="afe94-183">API-registratie</span><span class="sxs-lookup"><span data-stu-id="afe94-183">API registration</span></span>

<span data-ttu-id="afe94-184">Zie API-toegang instellen in Partner Center voor meer informatie [over API-registratie.](/partner-center/develop/set-up-api-access-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="afe94-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="afe94-185">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="afe94-185">Next steps</span></span>

- [<span data-ttu-id="afe94-186">Cloud Solution Provider programma regionale markten en valuta's waar u CSP-aanbiedingen kunt verkopen</span><span class="sxs-lookup"><span data-stu-id="afe94-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
