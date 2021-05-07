---
title: Locaties in uw partneraccount beheren
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-id van de locatie wordt gebruikt in incentive-programma's, CSP-bedrijven, abonnementen en andere transacties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702889"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="66315-103">Uw MPN-accountlocaties beheren en een locatie toevoegen (verwijderen)</span><span class="sxs-lookup"><span data-stu-id="66315-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="66315-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="66315-104">**Appropriate roles**</span></span>

- <span data-ttu-id="66315-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="66315-105">Global admin</span></span>
- <span data-ttu-id="66315-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="66315-106">Account admin</span></span>

<span data-ttu-id="66315-107">De MPN-id van de locatie identificeert elke specifieke locatie van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="66315-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="66315-108">U gebruikt de MPN-locatie-id om u in te schrijven voor incentive-programma's, om Cloud Solution Provider (CSP)-transacties en andere zakelijke transacties uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="66315-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="66315-109">De algemene MPN-id wordt gebruikt voor niet-transactionele activiteiten, zoals ondersteuningsaanvragen.</span><span class="sxs-lookup"><span data-stu-id="66315-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="66315-110">Het volgende scenario is gebruikelijk:</span><span class="sxs-lookup"><span data-stu-id="66315-110">The following scenario is typical:</span></span>

<span data-ttu-id="66315-111">Contoso heeft een Partner Global Account (PGA) in het Vk.</span><span class="sxs-lookup"><span data-stu-id="66315-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="66315-112">De PGA is hun geregistreerde juridische bedrijf en de globale MPN-id wordt gebruikt voor het beheren van alle niet-transactionele bedrijf.</span><span class="sxs-lookup"><span data-stu-id="66315-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="66315-113">Contoso heeft ook partnerlocatieaccounts (PLA) die gelijk zijn aan dochterondernemingen of divisies op een andere locatie in het Vk, Frankrijk en de Verenigde Staten.</span><span class="sxs-lookup"><span data-stu-id="66315-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="66315-114">In de structuur van het MPN-account worden deze PLA's weergegeven als unieke LOCATIE-MPN-ID's.</span><span class="sxs-lookup"><span data-stu-id="66315-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="66315-115">De PLA's worden gebruikt voor transactionele activiteiten zoals CSP of incentives-programma's.</span><span class="sxs-lookup"><span data-stu-id="66315-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="66315-116">Uitbetalingen zijn gekoppeld aan specifieke locaties.</span><span class="sxs-lookup"><span data-stu-id="66315-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="66315-117">Er is een 1-1-relatie tussen een CSP-tenant en een MPN-locatie-id.</span><span class="sxs-lookup"><span data-stu-id="66315-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="66315-119">Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf</span><span class="sxs-lookup"><span data-stu-id="66315-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="66315-120">Als u een nieuw CSP-bedrijfsaccount wilt toevoegen, moet u er eerst voor zorgen dat u aan de vereisten hebt voldaan.</span><span class="sxs-lookup"><span data-stu-id="66315-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="66315-121">U moet een MPN-locatie-id hebben in het land waar u CSP-zaken wilt doen.</span><span class="sxs-lookup"><span data-stu-id="66315-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="66315-122">Lees 'Een MPN-locatie toevoegen' hieronder om een nieuwe MPN-locatie te maken.</span><span class="sxs-lookup"><span data-stu-id="66315-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="66315-123">Als u een nieuwe CSP Indirect Reseller wilt maken, leest [u Werken met indirecte providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="66315-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="66315-124">Vergeet niet om u aan te melden met **de nieuwe** referenties voor het **nieuwe** CSP-account.</span><span class="sxs-lookup"><span data-stu-id="66315-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="66315-125">Gebruik uw bestaande referenties niet, omdat Partner Center herkent dat u al een account hebt.</span><span class="sxs-lookup"><span data-stu-id="66315-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="66315-126">Accepteer de Microsoft Partner-overeenkomst en activeer het account.</span><span class="sxs-lookup"><span data-stu-id="66315-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="66315-127">Als u zich wilt inschrijven als partner voor directe factuur, leest u [Vereisten voor directe factuurpartners](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="66315-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="66315-128">Uw MPN-locaties weergeven en bijwerken</span><span class="sxs-lookup"><span data-stu-id="66315-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="66315-129">Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) met de referenties van uw MPN-account.</span><span class="sxs-lookup"><span data-stu-id="66315-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="66315-130">(Uw MPN-referenties kunnen verschillen van uw CSP-referenties)</span><span class="sxs-lookup"><span data-stu-id="66315-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="66315-131">Selecteer in **het** pictogram Instellingen de optie **Accountinstellingen,** **Organisatieprofiel,** **Juridisch.**</span><span class="sxs-lookup"><span data-stu-id="66315-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="66315-132">Controleer op **het tabblad Partner** of er geen bannerfoutbericht wordt weergegeven waarin u wordt gevraagd om gemigreerde locaties van PMC op te lossen.</span><span class="sxs-lookup"><span data-stu-id="66315-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="66315-133">Als uw locaties niet correct zijn ingesteld in PMC en nog niet zijn overgestappen naar pc, moet u deze locaties bijwerken.</span><span class="sxs-lookup"><span data-stu-id="66315-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Schermkapje laat zien hoe u de locatie bij kunt werken.":::
 
4.  <span data-ttu-id="66315-135">Selecteer in **het scherm PMC-locaties** controleren de optie **Bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="66315-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="66315-136">Werk de volgende velden bij:</span><span class="sxs-lookup"><span data-stu-id="66315-136">Update the following fields:</span></span>

- <span data-ttu-id="66315-137">**Veld Naam:** zorg ervoor dat de naam van de bedrijfslocatie juist is.</span><span class="sxs-lookup"><span data-stu-id="66315-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="66315-138">Als er een dubbele fout wordt weergegeven, probeert u te wijzigen van bijvoorbeeld Contoso in Contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="66315-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="66315-139">**Veld Juridische entiteit:** Zorg ervoor dat u de juridische entiteit hebt gekozen waar de locatie aan is gekoppeld</span><span class="sxs-lookup"><span data-stu-id="66315-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="66315-140">**Adresregel 1 & 2 velden:** zorg ervoor dat het adres juist is</span><span class="sxs-lookup"><span data-stu-id="66315-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="66315-141">**Velden & plaats/provincie:** zorg ervoor dat de combinatie tussen de plaats en de staat/provincie juist is.</span><span class="sxs-lookup"><span data-stu-id="66315-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="66315-142">Er zijn landen waar de vervolgkeuzelijst voor het kiezen van staat/provincie van toepassing is en in andere landen moet dat veld handmatig worden ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="66315-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="66315-143">**Postcodeveld: zorg** ervoor dat het postcodeveld overeenkomt met uw aangegeven land, regio, plaats of adres.</span><span class="sxs-lookup"><span data-stu-id="66315-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="66315-144">**Velden** met primaire contactgegevens: zorg ervoor dat de velden voor- en achternaam zijn ingevuld en dat het aangegeven e-mailadres een werk-e-mailadres is en geen persoonlijk e-mailadres (bijvoorbeeld @outlook.com , , @live.com enzovoort)</span><span class="sxs-lookup"><span data-stu-id="66315-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="66315-145">**Veld Telefoonnummer:** zorg ervoor dat het telefoonnummer GEEN speciale tekens, spaties of landcode bevat.</span><span class="sxs-lookup"><span data-stu-id="66315-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="66315-146">De waarde die in het veld Telefoonnummer wordt ingevoerd, bevat altijd maximaal 10 tekens.</span><span class="sxs-lookup"><span data-stu-id="66315-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="66315-147">Als er geen foutbericht is, selecteert u in Instellingen de optie **Accountinstellingen,** **Organisatieprofiel,** **Id's.**</span><span class="sxs-lookup"><span data-stu-id="66315-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="66315-148">Zoek de MPN-id met het type 'Locatie' die overeenkomt met het land van dit CSP-account en gebruik deze om de associatie te voltooien.</span><span class="sxs-lookup"><span data-stu-id="66315-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="66315-149">Als u de MPN-locatie-id die overeenkomt met het CSP-account dat u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen, waarmee een nieuwe MPN-id wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="66315-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="66315-150">Zie **Een MPN-locatie toevoegen** hieronder.</span><span class="sxs-lookup"><span data-stu-id="66315-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="66315-151">Een MPN-locatie toevoegen</span><span class="sxs-lookup"><span data-stu-id="66315-151">Add an MPN location</span></span>

1. <span data-ttu-id="66315-152">Meld u aan met het MPN-account in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="66315-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="66315-153">(Uw MPN-referenties kunnen verschillen van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="66315-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="66315-154">Het MPN-account moet globale beheerders- of accountbeheerdersbevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="66315-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="66315-155">Selecteer in **het pictogram Instellingen** de **accountinstellingen en** selecteer vervolgens **Organisatieprofiel.**</span><span class="sxs-lookup"><span data-stu-id="66315-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="66315-156">Selecteer **Juridisch** en selecteer vervolgens op het **tabblad Partner** de optie **Bedrijfslocaties en** klik op Een locatie **toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="66315-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="66315-157">Geef de vereiste gegevens op, zoals de bedrijfsnaam, het adres en de contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="66315-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="66315-158">Klik **op Locatie toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="66315-158">Click **Add location**.</span></span> <span data-ttu-id="66315-159">Hiermee maakt u een nieuwe MPN-id voor de nieuwe locatie die u kunt gebruiken voor CSP-transacties en incentives.</span><span class="sxs-lookup"><span data-stu-id="66315-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Een nieuw juridisch bedrijf toevoegen":::

> [!NOTE]
> <span data-ttu-id="66315-161">Zodra een locatie is toegevoegd aan Partner Center, kunt u deze niet verwijderen.</span><span class="sxs-lookup"><span data-stu-id="66315-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="66315-162">U ziet **MPN** in het linkermenu van Partner Center als u de juiste MPN-id hebt gebruikt om u aan te melden.</span><span class="sxs-lookup"><span data-stu-id="66315-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="66315-163">De id van het registratienummer toevoegen</span><span class="sxs-lookup"><span data-stu-id="66315-163">Add the registration number ID</span></span>

<span data-ttu-id="66315-164">Als u een indirecte provider, directe factuurpartner of indirecte reseller bent en u zaken doet met nieuwe of bestaande klanten in de volgende landen, moet u registratie-id-nummers voor uw bedrijf verstrekken.</span><span class="sxs-lookup"><span data-stu-id="66315-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="66315-165">Als het land waarin u zaken doet niet hieronder wordt vermeld, is de registratie-id optioneel.</span><span class="sxs-lookup"><span data-stu-id="66315-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="66315-166">Armenië</span><span class="sxs-lookup"><span data-stu-id="66315-166">Armenia</span></span> 
- <span data-ttu-id="66315-167">Azerbeidzjan</span><span class="sxs-lookup"><span data-stu-id="66315-167">Azerbaijan</span></span> 
- <span data-ttu-id="66315-168">Belarus</span><span class="sxs-lookup"><span data-stu-id="66315-168">Belarus</span></span> 
- <span data-ttu-id="66315-169">Brazilië</span><span class="sxs-lookup"><span data-stu-id="66315-169">Brazil</span></span> 
- <span data-ttu-id="66315-170">Hongarije</span><span class="sxs-lookup"><span data-stu-id="66315-170">Hungary</span></span> 
- <span data-ttu-id="66315-171">India</span><span class="sxs-lookup"><span data-stu-id="66315-171">India</span></span> 
- <span data-ttu-id="66315-172">Irak</span><span class="sxs-lookup"><span data-stu-id="66315-172">Iraq</span></span> 
- <span data-ttu-id="66315-173">Kazachstan</span><span class="sxs-lookup"><span data-stu-id="66315-173">Kazakhstan</span></span> 
- <span data-ttu-id="66315-174">Kirgistan</span><span class="sxs-lookup"><span data-stu-id="66315-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="66315-175">Moldavië</span><span class="sxs-lookup"><span data-stu-id="66315-175">Moldova</span></span> 
- <span data-ttu-id="66315-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="66315-176">Myanmar</span></span> 
- <span data-ttu-id="66315-177">Polen</span><span class="sxs-lookup"><span data-stu-id="66315-177">Poland</span></span> 
- <span data-ttu-id="66315-178">Rusland</span><span class="sxs-lookup"><span data-stu-id="66315-178">Russia</span></span> 
- <span data-ttu-id="66315-179">Saoedi-Arabië</span><span class="sxs-lookup"><span data-stu-id="66315-179">Saudi Arabia</span></span> 
- <span data-ttu-id="66315-180">Zuid-Afrika</span><span class="sxs-lookup"><span data-stu-id="66315-180">South Africa</span></span> 
- <span data-ttu-id="66315-181">Zuid-Soedan</span><span class="sxs-lookup"><span data-stu-id="66315-181">South Sudan</span></span>  
- <span data-ttu-id="66315-182">Tadzjikistan</span><span class="sxs-lookup"><span data-stu-id="66315-182">Tajikistan</span></span> 
- <span data-ttu-id="66315-183">Thailand</span><span class="sxs-lookup"><span data-stu-id="66315-183">Thailand</span></span>
- <span data-ttu-id="66315-184">Turkije</span><span class="sxs-lookup"><span data-stu-id="66315-184">Turkey</span></span> 
- <span data-ttu-id="66315-185">Oekraïne</span><span class="sxs-lookup"><span data-stu-id="66315-185">Ukraine</span></span> 
- <span data-ttu-id="66315-186">Verenigde Arabische Emiraten</span><span class="sxs-lookup"><span data-stu-id="66315-186">United Arab Emirates</span></span> 
- <span data-ttu-id="66315-187">Oezbekistan</span><span class="sxs-lookup"><span data-stu-id="66315-187">Uzbekistan</span></span> 
- <span data-ttu-id="66315-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="66315-188">Venezuela</span></span>
- <span data-ttu-id="66315-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="66315-189">Vietnam</span></span> 


<span data-ttu-id="66315-190">Lees Registratie-id-nummergegevens [voor meer informatie](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="66315-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="66315-191">Een locatie verwijderen</span><span class="sxs-lookup"><span data-stu-id="66315-191">Delete a location</span></span>

<span data-ttu-id="66315-192">Als u een locatie uit uw account wilt verwijderen, moet u contact opnemen met [partnerondersteuning.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)</span><span class="sxs-lookup"><span data-stu-id="66315-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="66315-193">Zorg ervoor dat u begrijpt wat de impact van deze actie is.</span><span class="sxs-lookup"><span data-stu-id="66315-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="66315-194">Verwijderde locaties kunnen niet worden opgehaald en alles wat is gekoppeld aan die specifieke MPN-id, wordt niet meer herkend of is actief voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="66315-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="66315-195">Land van algemeen partneraccount wijzigen</span><span class="sxs-lookup"><span data-stu-id="66315-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="66315-196">Meld u aan met het MPN-account in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="66315-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="66315-197">(Uw MPN-referenties kunnen verschillen van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="66315-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="66315-198">Het MPN-account moet de bevoegdheden Globale beheerder of Accountbeheerder hebben.</span><span class="sxs-lookup"><span data-stu-id="66315-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="66315-199">Ga op **het tabblad Partner** naar Bedrijfslocaties en controleer de lijst met locaties om ervoor te zorgen dat de locatie die u wilt gebruiken als uw juridische entiteit wordt vermeld. </span><span class="sxs-lookup"><span data-stu-id="66315-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="66315-200">Als u een locatie wilt toevoegen, klikt u op Een locatie toevoegen en geeft u in het fly-outvenster de vereiste gegevens op, waaronder de bedrijfsnaam, het adres en de primaire contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="66315-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="66315-201">Selecteer **Uw land wijzigen** naast de **vervolgkeuzekeuze** selecteren en volg de stappen.</span><span class="sxs-lookup"><span data-stu-id="66315-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Juridische bedrijfsprofielgegevens zijn beschikbaar":::

5. <span data-ttu-id="66315-203">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="66315-203">Click **Save**.</span></span>

6. <span data-ttu-id="66315-204">Het land van het globale MPN-account wordt gewijzigd in het nieuwe juridische land.</span><span class="sxs-lookup"><span data-stu-id="66315-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="66315-205">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="66315-205">Next steps</span></span>

- <span data-ttu-id="66315-206">Meer informatie over het [verificatieproces](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="66315-206">Learn about the [verification process](verification-responses.md).</span></span>
