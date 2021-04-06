---
title: Locaties in uw partner account beheren
ms.topic: how-to
ms.date: 04/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-ID van de locatie wordt gebruikt in prikkel Programma's, CSP-bedrijven, abonnementen en andere trans acties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ca8c866479fbe153c1e0192edd33e8258b9d6e7
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441321"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="e0f85-103">Uw MPN-account locaties beheren en een locatie toevoegen (verwijderen)</span><span class="sxs-lookup"><span data-stu-id="e0f85-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="e0f85-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="e0f85-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e0f85-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="e0f85-105">Global admin</span></span>
- <span data-ttu-id="e0f85-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="e0f85-106">Account admin</span></span>

<span data-ttu-id="e0f85-107">De MPN-ID van de locatie identificeert elke specifieke locatie van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="e0f85-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e0f85-108">U gebruikt de MPN-ID van de locatie om in te schrijven in prikkel-Program ma's, voor het bedrijf van de Transact Cloud Solution Provider (CSP) en andere zakelijke trans acties.</span><span class="sxs-lookup"><span data-stu-id="e0f85-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e0f85-109">De ID van de globale MPN wordt gebruikt voor niet-transactionele activiteiten zoals ondersteunings aanvragen.</span><span class="sxs-lookup"><span data-stu-id="e0f85-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="e0f85-110">Het volgende scenario is gebruikelijk:</span><span class="sxs-lookup"><span data-stu-id="e0f85-110">The following scenario is typical:</span></span>

<span data-ttu-id="e0f85-111">Contoso heeft het wereld wijde account van de partner (PGA) in het Verenigd Konink rijk.</span><span class="sxs-lookup"><span data-stu-id="e0f85-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="e0f85-112">De PGA is de geregistreerde juridische onderneming en de globale MPN-ID wordt gebruikt voor het beheren van alle niet-transactionele bedrijven.</span><span class="sxs-lookup"><span data-stu-id="e0f85-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="e0f85-113">Contoso heeft ook partner locatie accounts (PLA) die gelijk zijn aan dochter ondernemingen of afdelingen op een andere locatie in UK, Frank rijk en de Verenigde Staten.</span><span class="sxs-lookup"><span data-stu-id="e0f85-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e0f85-114">In de MPN-account structuur worden deze PLAs vertegenwoordigd als unieke locatie MPN-Id's.</span><span class="sxs-lookup"><span data-stu-id="e0f85-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e0f85-115">De PLAs worden gebruikt voor transactionele activiteiten zoals CSP of prikkel Programma's.</span><span class="sxs-lookup"><span data-stu-id="e0f85-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e0f85-116">Uitbetalingen zijn gekoppeld aan specifieke locaties.</span><span class="sxs-lookup"><span data-stu-id="e0f85-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e0f85-117">Er is een 1-1-relatie tussen een CSP-Tenant en een MPN locatie-ID.</span><span class="sxs-lookup"><span data-stu-id="e0f85-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="e0f85-119">Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf</span><span class="sxs-lookup"><span data-stu-id="e0f85-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="e0f85-120">Als u een nieuw CSP-account wilt toevoegen, moet u eerst controleren of u aan de vereisten hebt voldaan.</span><span class="sxs-lookup"><span data-stu-id="e0f85-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="e0f85-121">U moet een locatie MPN-ID hebben in het land waar u de CSP-onderneming wilt maken.</span><span class="sxs-lookup"><span data-stu-id="e0f85-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="e0f85-122">Lees "een MPN-locatie toevoegen" hieronder om een nieuwe MPN-locatie te maken.</span><span class="sxs-lookup"><span data-stu-id="e0f85-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="e0f85-123">Lees voor het maken van een nieuwe CSP indirecte reseller-inschrijving [werk met indirecte providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="e0f85-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="e0f85-124">Meld u aan met de **nieuwe** referenties voor het **nieuwe** CSP-account.</span><span class="sxs-lookup"><span data-stu-id="e0f85-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="e0f85-125">Gebruik uw bestaande referenties niet als het partner centrum u heeft herkend als al een account.</span><span class="sxs-lookup"><span data-stu-id="e0f85-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="e0f85-126">Ga akkoord met de micro soft-partner overeenkomst en activeer het account.</span><span class="sxs-lookup"><span data-stu-id="e0f85-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="e0f85-127">Als u zich wilt registreren als een directe factuur partner, lees dan de [vereisten voor directe factuur partners](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="e0f85-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="e0f85-128">Uw MPN-locaties weer geven</span><span class="sxs-lookup"><span data-stu-id="e0f85-128">View your MPN locations</span></span>

1. <span data-ttu-id="e0f85-129">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/home) van de partner centrum met de referenties van uw MPN-account.</span><span class="sxs-lookup"><span data-stu-id="e0f85-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="e0f85-130">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties)</span><span class="sxs-lookup"><span data-stu-id="e0f85-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="e0f85-131">Selecteer op het pictogram **instellingen** **account instellingen**, **organisatie profiel**, **juridisch**.</span><span class="sxs-lookup"><span data-stu-id="e0f85-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="e0f85-132">Controleer op het tabblad **partner** of er geen banner fout bericht wordt weer gegeven waarin u wordt gevraagd om gemigreerde locaties te herstellen vanuit PMC.</span><span class="sxs-lookup"><span data-stu-id="e0f85-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="e0f85-133">Als uw locaties niet correct zijn ingesteld in PMC en nog niet zijn overgezet naar de PC, moet u die locaties bijwerken.</span><span class="sxs-lookup"><span data-stu-id="e0f85-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Scherm afbeelding laat zien hoe u de locatie kunt bijwerken.":::
 
4.  <span data-ttu-id="e0f85-135">Selecteer **bijwerken** op het scherm **PMC locaties controleren** .</span><span class="sxs-lookup"><span data-stu-id="e0f85-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="e0f85-136">Werk de volgende velden bij:</span><span class="sxs-lookup"><span data-stu-id="e0f85-136">Update the following fields:</span></span>

- <span data-ttu-id="e0f85-137">**Naam veld**: Controleer of de naam van de bedrijfs locatie juist is.</span><span class="sxs-lookup"><span data-stu-id="e0f85-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="e0f85-138">Als er een dubbele fout wordt weer gegeven, kunt u het wijzigen van, bijvoorbeeld contoso naar contoso, Inc.</span><span class="sxs-lookup"><span data-stu-id="e0f85-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="e0f85-139">**Juridisch entiteits veld**: Zorg ervoor dat u de rechts persoon hebt gekozen waaraan de locatie is gekoppeld</span><span class="sxs-lookup"><span data-stu-id="e0f85-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="e0f85-140">**Adres regel 1 & 2 velden**: Controleer of het adres juist is</span><span class="sxs-lookup"><span data-stu-id="e0f85-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="e0f85-141">**Plaats & velden voor provincie**: Zorg ervoor dat de combi natie tussen de plaats en de staat/provincie juist is.</span><span class="sxs-lookup"><span data-stu-id="e0f85-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="e0f85-142">Er zijn landen waar het vervolg keuzemenu voor het kiezen van de staat/provincie van toepassing is, en in andere landen dat veld hand matig moet worden ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="e0f85-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="e0f85-143">Post **code**: Controleer of het veld post code overeenkomt met het land of de regio, de plaats of het adres van de aangegeven categorie.</span><span class="sxs-lookup"><span data-stu-id="e0f85-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="e0f85-144">**Velden met primaire contact gegevens**: Controleer of de velden voor de voor-en achternaam zijn gevuld en of het opgegeven e-mail adres een werk-e-mail adres is, en niet een persoonlijk account (bijvoorbeeld, @outlook.com @live.com enzovoort)</span><span class="sxs-lookup"><span data-stu-id="e0f85-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="e0f85-145">**Telefoonnummer veld**: Zorg ervoor dat het telefoon nummer geen speciale tekens, spaties of land code bevat.</span><span class="sxs-lookup"><span data-stu-id="e0f85-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="e0f85-146">De waarde die u in het veld telefoon nummer hebt opgegeven, bevat altijd Maxi maal 10 tekens.</span><span class="sxs-lookup"><span data-stu-id="e0f85-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="e0f85-147">Als er geen fout bericht wordt weer gegeven, selecteert u in  **instellingen**  **account instellingen**, **organisatie profiel**, **id's**.</span><span class="sxs-lookup"><span data-stu-id="e0f85-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="e0f85-148">Zoek de MPN-ID van het type "locatie" die overeenkomt met het land van dit CSP-account en gebruik deze om de koppeling te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="e0f85-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="e0f85-149">Als u de locatie MPN-ID die overeenkomt met de CSP-account die u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen, waarmee een nieuwe MPN-ID wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="e0f85-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="e0f85-150">Zie hieronder **een MPN-locatie toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="e0f85-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="e0f85-151">Een MPN-locatie toevoegen</span><span class="sxs-lookup"><span data-stu-id="e0f85-151">Add an MPN location</span></span>

1. <span data-ttu-id="e0f85-152">Meld u aan met het MPN-account in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e0f85-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e0f85-153">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="e0f85-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e0f85-154">Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="e0f85-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="e0f85-155">Selecteer op het **pictogram instellingen** de **account instellingen** en selecteer vervolgens **organisatie profiel**.</span><span class="sxs-lookup"><span data-stu-id="e0f85-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="e0f85-156">Selecteer **juridisch** en selecteer vervolgens op het tabblad **partner** de optie **bedrijfs locaties** en klik op **een locatie toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="e0f85-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="e0f85-157">Geef de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="e0f85-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="e0f85-158">Klik op **locatie toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="e0f85-158">Click **Add location**.</span></span> <span data-ttu-id="e0f85-159">Hiermee wordt een nieuwe MPN-ID gemaakt voor de nieuwe locatie die u kunt gebruiken voor CSP-trans acties en-prikkels.</span><span class="sxs-lookup"><span data-stu-id="e0f85-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Een nieuw juridisch bedrijf toevoegen":::

> [!NOTE]
> <span data-ttu-id="e0f85-161">Zodra een locatie is toegevoegd in het partner centrum, kunt u deze niet meer verwijderen.</span><span class="sxs-lookup"><span data-stu-id="e0f85-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="e0f85-162">U ziet **MPN** in het menu links van partner centrum als u de juiste MPN-id hebt gebruikt om u aan te melden.</span><span class="sxs-lookup"><span data-stu-id="e0f85-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>


## <a name="delete-a-location"></a><span data-ttu-id="e0f85-163">Een locatie verwijderen</span><span class="sxs-lookup"><span data-stu-id="e0f85-163">Delete a location</span></span>

<span data-ttu-id="e0f85-164">Als u een locatie uit uw account wilt verwijderen, moet u contact opnemen met de [partner ondersteuning](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="e0f85-164">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="e0f85-165">Zorg ervoor dat u begrijpt wat het effect is van deze actie.</span><span class="sxs-lookup"><span data-stu-id="e0f85-165">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="e0f85-166">Verwijderde locaties kunnen niet worden opgehaald en items die zijn gekoppeld aan de specifieke MPN-id, worden niet meer herkend of zijn actief voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="e0f85-166">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="e0f85-167">Het wereld wijde account land van de partner wijzigen</span><span class="sxs-lookup"><span data-stu-id="e0f85-167">Change country of Partner global account</span></span> 

1. <span data-ttu-id="e0f85-168">Meld u aan met het MPN-account in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e0f85-168">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="e0f85-169">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="e0f85-169">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="e0f85-170">Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="e0f85-170">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="e0f85-171">Ga op het tabblad **partner** naar **bedrijfs locaties** en controleer de lijst met locaties om te controleren of de gewenste locatie als uw juridische entiteit wordt vermeld.</span><span class="sxs-lookup"><span data-stu-id="e0f85-171">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="e0f85-172">Als u een locatie wilt toevoegen, klikt u op **een locatie toevoegen** en geeft u in de vlucht uit de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de primaire contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="e0f85-172">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="e0f85-173">Selecteer **uw land wijzigen** naast de vervolg keuzelijst **land/regio** en volg de stappen.</span><span class="sxs-lookup"><span data-stu-id="e0f85-173">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Gegevens van juridisch zakelijk profiel worden in vlucht gegeven":::

5. <span data-ttu-id="e0f85-175">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="e0f85-175">Click **Save**.</span></span>

6. <span data-ttu-id="e0f85-176">De land instelling van het MPN Global-account wordt gewijzigd in het nieuwe juridische land.</span><span class="sxs-lookup"><span data-stu-id="e0f85-176">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e0f85-177">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="e0f85-177">Next steps</span></span>

- <span data-ttu-id="e0f85-178">Meer informatie over het [verificatie proces](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="e0f85-178">Learn about the [verification process](verification-responses.md).</span></span>
