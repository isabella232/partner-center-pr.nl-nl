---
title: Locaties in uw partner account beheren
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-ID van de locatie wordt gebruikt in prikkel Programma's, CSP-bedrijven, abonnementen en andere trans acties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773433"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="5363e-103">Uw MPN-account locaties beheren en een nieuwe locatie toevoegen</span><span class="sxs-lookup"><span data-stu-id="5363e-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="5363e-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="5363e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5363e-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="5363e-105">Global admin</span></span>
- <span data-ttu-id="5363e-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="5363e-106">Account admin</span></span>

<span data-ttu-id="5363e-107">De MPN-ID van de locatie identificeert elke specifieke locatie van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="5363e-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="5363e-108">U gebruikt de MPN-ID van de locatie om in te schrijven in prikkel-Program ma's, voor het bedrijf van de Transact Cloud Solution Provider (CSP) en andere zakelijke trans acties.</span><span class="sxs-lookup"><span data-stu-id="5363e-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="5363e-109">De ID van de globale MPN wordt gebruikt voor niet-transactionele activiteiten zoals ondersteunings aanvragen.</span><span class="sxs-lookup"><span data-stu-id="5363e-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="5363e-110">Hier volgt een typisch scenario:</span><span class="sxs-lookup"><span data-stu-id="5363e-110">The following is a typical scenario:</span></span>

<span data-ttu-id="5363e-111">Contoso heeft het wereld wijde account van de partner (PGA) in het Verenigd Konink rijk.</span><span class="sxs-lookup"><span data-stu-id="5363e-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="5363e-112">Dit is hun rechts bedrijf en de algemene MPN-ID wordt gebruikt voor het beheren van alle niet-transactionele zakelijke activiteiten.</span><span class="sxs-lookup"><span data-stu-id="5363e-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="5363e-113">Contoso heeft ook partner locatie accounts (PLA) die gelijk zijn aan dochter ondernemingen of afdelingen op een andere locatie in UK, Frank rijk en de Verenigde Staten.</span><span class="sxs-lookup"><span data-stu-id="5363e-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="5363e-114">In de MPN-account structuur worden deze PLAs vertegenwoordigd als unieke locatie MPN-Id's.</span><span class="sxs-lookup"><span data-stu-id="5363e-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="5363e-115">De PLAs worden gebruikt voor transactionele activiteiten zoals CSP of prikkel Programma's.</span><span class="sxs-lookup"><span data-stu-id="5363e-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="5363e-116">Uitbetalingen zijn gekoppeld aan specifieke locaties.</span><span class="sxs-lookup"><span data-stu-id="5363e-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="5363e-117">Er is een 1-1-relatie tussen een CSP-Tenant en een MPN locatie-ID.</span><span class="sxs-lookup"><span data-stu-id="5363e-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="5363e-119">Vereisten voor het toevoegen van een nieuwe account locatie voor een CSP-bedrijf</span><span class="sxs-lookup"><span data-stu-id="5363e-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="5363e-120">Er zijn verschillende vereisten om een nieuwe CSP-bedrijfs locatie toe te voegen:</span><span class="sxs-lookup"><span data-stu-id="5363e-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="5363e-121">U moet een locatie MPN-ID hebben in het land waar u zaken wilt doen.</span><span class="sxs-lookup"><span data-stu-id="5363e-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="5363e-122">U hebt een nieuwe Azure AD-Tenant nodig in de [bedrijfs regio](regional-authorization-overview.md) die nog niet is inge SCHREVEN bij CSP.</span><span class="sxs-lookup"><span data-stu-id="5363e-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="5363e-123">Dit maken wanneer u zich registreert bij CSP.</span><span class="sxs-lookup"><span data-stu-id="5363e-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="5363e-124">Gebruik de nieuwe AAD-Tenant om u aan te melden bij het CSP-programma in de regio.</span><span class="sxs-lookup"><span data-stu-id="5363e-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="5363e-125">Juridische Bedrijfs gegevens opgeven, inclusief de naam van het bedrijf, het adres, de primaire contact gegevens.</span><span class="sxs-lookup"><span data-stu-id="5363e-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="5363e-126">Dit account wordt gecontroleerd. Zorg er dus voor dat u geldige gegevens toevoegt.</span><span class="sxs-lookup"><span data-stu-id="5363e-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="5363e-127">Meld u aan met de **nieuwe** referenties voor de **nieuwe** Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="5363e-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="5363e-128">Gebruik uw bestaande referenties niet als het partner centrum u heeft herkend als al een account.</span><span class="sxs-lookup"><span data-stu-id="5363e-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="5363e-129">Ga akkoord met de micro soft-partner overeenkomst en activeer het account.</span><span class="sxs-lookup"><span data-stu-id="5363e-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="5363e-130">Een MPN-locatie toevoegen</span><span class="sxs-lookup"><span data-stu-id="5363e-130">Add an MPN location</span></span>

1. <span data-ttu-id="5363e-131">Meld u aan met het MPN-account in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="5363e-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="5363e-132">Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben.</span><span class="sxs-lookup"><span data-stu-id="5363e-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="5363e-133">Selecteer de **organisatie-instellingen** op het **pictogram instelling**.</span><span class="sxs-lookup"><span data-stu-id="5363e-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="5363e-134">Selecteer **juridisch** en selecteer vervolgens **locaties.**</span><span class="sxs-lookup"><span data-stu-id="5363e-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="5363e-135">Selecteer **een locatie toevoegen** en voeg de adres gegevens in van de locatie die u wilt toevoegen aan uw bedrijf, evenals een primaire contact persoon voor de locatie.</span><span class="sxs-lookup"><span data-stu-id="5363e-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="5363e-136">Zodra een locatie is toegevoegd in het partner centrum, kan deze niet meer worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="5363e-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="5363e-137">U ziet **MPN** in het menu links van partner centrum als u de juiste MPN-id hebt gebruikt om u aan te melden.</span><span class="sxs-lookup"><span data-stu-id="5363e-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="5363e-138">Locatie van globale partner account wijzigen</span><span class="sxs-lookup"><span data-stu-id="5363e-138">Change Global partner account location</span></span>

1. <span data-ttu-id="5363e-139">Controleer op **[bedrijfs locaties](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** de lijst met locaties om ervoor te zorgen dat de gewenste locatie als uw rechts persoon wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="5363e-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="5363e-140">Als dat niet het geval is, voegt u deze toe.</span><span class="sxs-lookup"><span data-stu-id="5363e-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Scherm afbeelding van de pagina account locaties van partner centrum met een lijst met alle huidige locaties.":::

2. <span data-ttu-id="5363e-142">Selecteer **juridisch** en selecteer **juridisch zakelijk profiel bijwerken**</span><span class="sxs-lookup"><span data-stu-id="5363e-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="5363e-143">Selecteer de regio en rechts persoon en **Verzend** deze.</span><span class="sxs-lookup"><span data-stu-id="5363e-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="5363e-144">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="5363e-144">Next steps</span></span>

- <span data-ttu-id="5363e-145">Meer informatie over het [verificatie proces](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="5363e-145">Learn about the [verification process](verification-responses.md).</span></span>
