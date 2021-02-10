---
title: Locaties in uw partner account beheren
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-ID van de locatie wordt gebruikt in prikkel Programma's, CSP-bedrijven, abonnementen en andere trans acties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005913"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="0b4b6-103">Uw MPN-account locaties beheren en een locatie toevoegen (verwijderen)</span><span class="sxs-lookup"><span data-stu-id="0b4b6-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="0b4b6-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="0b4b6-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0b4b6-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="0b4b6-105">Global admin</span></span>
- <span data-ttu-id="0b4b6-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="0b4b6-106">Account admin</span></span>

<span data-ttu-id="0b4b6-107">De MPN-ID van de locatie identificeert elke specifieke locatie van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="0b4b6-108">U gebruikt de MPN-ID van de locatie om in te schrijven in prikkel-Program ma's, voor het bedrijf van de Transact Cloud Solution Provider (CSP) en andere zakelijke trans acties.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="0b4b6-109">De ID van de globale MPN wordt gebruikt voor niet-transactionele activiteiten zoals ondersteunings aanvragen.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="0b4b6-110">Hier volgt een typisch scenario:</span><span class="sxs-lookup"><span data-stu-id="0b4b6-110">The following is a typical scenario:</span></span>

<span data-ttu-id="0b4b6-111">Contoso heeft het wereld wijde account van de partner (PGA) in het Verenigd Konink rijk.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="0b4b6-112">Dit is hun rechts bedrijf en de algemene MPN-ID wordt gebruikt voor het beheren van alle niet-transactionele zakelijke activiteiten.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="0b4b6-113">Contoso heeft ook partner locatie accounts (PLA) die gelijk zijn aan dochter ondernemingen of afdelingen op een andere locatie in UK, Frank rijk en de Verenigde Staten.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="0b4b6-114">In de MPN-account structuur worden deze PLAs vertegenwoordigd als unieke locatie MPN-Id's.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="0b4b6-115">De PLAs worden gebruikt voor transactionele activiteiten zoals CSP of prikkel Programma's.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="0b4b6-116">Uitbetalingen zijn gekoppeld aan specifieke locaties.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="0b4b6-117">Er is een 1-1-relatie tussen een CSP-Tenant en een MPN locatie-ID.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="0b4b6-119">Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf</span><span class="sxs-lookup"><span data-stu-id="0b4b6-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="0b4b6-120">Als u een nieuw CSP-account wilt toevoegen, moet u eerst controleren of u aan de vereisten hebt voldaan.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="0b4b6-121">U moet een locatie MPN-ID hebben in het land waar u de CSP-onderneming wilt maken.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="0b4b6-122">Lees "een MPN-locatie toevoegen" hieronder om een nieuwe MPN-locatie te maken.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="0b4b6-123">Lees voor het maken van een nieuwe CSP indirecte reseller-inschrijving [werk met indirecte providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="0b4b6-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="0b4b6-124">Meld u aan met de **nieuwe** referenties voor het **nieuwe** CSP-account.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="0b4b6-125">Gebruik uw bestaande referenties niet als het partner centrum u heeft herkend als al een account.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="0b4b6-126">Ga akkoord met de micro soft-partner overeenkomst en activeer het account.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="0b4b6-127">Als u zich wilt registreren als een directe factuur partner, lees dan de [vereisten voor directe factuur partners](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="0b4b6-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="0b4b6-128">Uw MPN-locaties weer geven</span><span class="sxs-lookup"><span data-stu-id="0b4b6-128">View your MPN locations</span></span>

1. <span data-ttu-id="0b4b6-129">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/home) van de partner centrum met de referenties van uw MPN-account.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="0b4b6-130">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties)</span><span class="sxs-lookup"><span data-stu-id="0b4b6-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="0b4b6-131">Selecteer op het pictogram **instellingen** **account instellingen**, **organisatie profiel**, **juridisch**.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="0b4b6-132">Controleer op het tabblad **partner** of er geen banner fout bericht wordt weer gegeven waarin u wordt gevraagd om gemigreerde locaties te herstellen vanuit PMC.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="0b4b6-133">Als dat het geval is, volgt u de instructies en verhelpt u deze locaties.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="0b4b6-134">Als er geen fout bericht wordt weer gegeven, selecteert u in  **instellingen**  **account instellingen**, **organisatie profiel**, **id's**.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="0b4b6-135">Zoek naar de MPN-ID van het type "locatie" die overeenkomt met het land van dit CSP-account en gebruik het om de koppeling te doorzoeken en te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="0b4b6-136">Als u de locatie MPN-ID die overeenkomt met de CSP-account die u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen waarmee een nieuwe MPN-ID wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="0b4b6-137">Zie hieronder **een MPN-locatie toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="0b4b6-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="0b4b6-138">Een MPN-locatie toevoegen</span><span class="sxs-lookup"><span data-stu-id="0b4b6-138">Add an MPN location</span></span>

1. <span data-ttu-id="0b4b6-139">Meld u aan met het MPN-account in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0b4b6-140">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="0b4b6-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0b4b6-141">Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="0b4b6-142">Selecteer op het **pictogram instellingen** de **account instellingen** en selecteer vervolgens **organisatie profiel**.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="0b4b6-143">Selecteer **juridisch** en selecteer vervolgens op het tabblad **partner** de optie **bedrijfs locaties** en klik op **een locatie toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="0b4b6-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="0b4b6-144">Geef de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="0b4b6-145">Klik op **locatie toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-145">Click **Add location**.</span></span> <span data-ttu-id="0b4b6-146">Hiermee wordt een nieuwe MPN-ID gemaakt voor de nieuwe locatie die u kunt gebruiken voor CSP-trans acties en-prikkels.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Een nieuw juridisch bedrijf toevoegen":::

> [!NOTE]
> <span data-ttu-id="0b4b6-148">Zodra een locatie is toegevoegd in het partner centrum, kunt u deze niet meer verwijderen.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="0b4b6-149">U ziet **MPN** in het menu links van partner centrum als u de juiste MPN-id hebt gebruikt om u aan te melden.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="0b4b6-150">Een locatie verwijderen</span><span class="sxs-lookup"><span data-stu-id="0b4b6-150">Delete a location</span></span>

<span data-ttu-id="0b4b6-151">Als u een locatie uit uw account wilt verwijderen, moet u contact opnemen met de [partner ondersteuning](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="0b4b6-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="0b4b6-152">Zorg ervoor dat u begrijpt wat het effect is van deze actie.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="0b4b6-153">Verwijderde locaties kunnen niet worden opgehaald en items die zijn gekoppeld aan de specifieke MPN-id, worden niet meer herkend of zijn actief voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="0b4b6-154">Het wereld wijde account land van de partner wijzigen</span><span class="sxs-lookup"><span data-stu-id="0b4b6-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="0b4b6-155">Meld u aan met het MPN-account in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="0b4b6-156">(Uw MPN-referenties kunnen afwijken van uw CSP-referenties).</span><span class="sxs-lookup"><span data-stu-id="0b4b6-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="0b4b6-157">Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="0b4b6-158">Ga op het tabblad **partner** naar **bedrijfs locaties** en controleer de lijst met locaties om te controleren of de gewenste locatie als uw juridische entiteit wordt vermeld.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="0b4b6-159">Als u een locatie wilt toevoegen, klikt u op **een locatie toevoegen** en geeft u in de vlucht uit de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de primaire contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="0b4b6-160">Selecteer **uw land wijzigen** naast de vervolg keuzelijst **land/regio** en volg de stappen.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Gegevens van juridisch zakelijk profiel worden in vlucht gegeven":::

5. <span data-ttu-id="0b4b6-162">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-162">Click **Save**.</span></span>

6. <span data-ttu-id="0b4b6-163">De land instelling van het MPN Global-account wordt gewijzigd in het nieuwe juridische land.</span><span class="sxs-lookup"><span data-stu-id="0b4b6-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="0b4b6-164">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="0b4b6-164">Next steps</span></span>

- <span data-ttu-id="0b4b6-165">Meer informatie over het [verificatie proces](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="0b4b6-165">Learn about the [verification process](verification-responses.md).</span></span>
