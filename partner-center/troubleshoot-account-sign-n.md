---
title: Problemen oplossen met het instellen van uw partner Center-account of problemen met MPN-vernieuwing
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Problemen oplossen bij het registreren in het partner centrum. Beantwoordt antwoorden op uitdagingen met betalings wijzen, wacht woorden verg eten en nog veel meer.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381406"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="dc7fd-104">Problemen met de account installatie of MPN oplossen</span><span class="sxs-lookup"><span data-stu-id="dc7fd-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="dc7fd-105">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="dc7fd-105">**Applies to**</span></span>

- <span data-ttu-id="dc7fd-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="dc7fd-106">Partner Center</span></span>
 
<span data-ttu-id="dc7fd-107">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="dc7fd-107">**Appropriate roles**</span></span>

- <span data-ttu-id="dc7fd-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="dc7fd-108">Global admin</span></span>
- <span data-ttu-id="dc7fd-109">MPN-partner beheerder</span><span class="sxs-lookup"><span data-stu-id="dc7fd-109">MPN partner admin</span></span> 
 
<span data-ttu-id="dc7fd-110">Hier volgen enkele suggesties voor het oplossen van veelvoorkomende problemen die zich voordoen bij het instellen van uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="dc7fd-111">Wat gebeurt er als u migreert van het lidmaatschaps centrum van de partner en u geen bedrijfs gegevens velden kunt bewerken</span><span class="sxs-lookup"><span data-stu-id="dc7fd-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="dc7fd-112">In gevallen waarin uw bedrijf al een aanwezigheid heeft in het partner centrum (bijvoorbeeld CSP-account), wordt er een alleen-lezen scherm weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="dc7fd-113">In dit scherm worden alle gegevens van uw bedrijf weer gegeven, zoals deze in het partner centrum aanwezig zijn.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="dc7fd-114">U kunt de details op dit scherm niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-114">You can't change the details on this screen.</span></span> <span data-ttu-id="dc7fd-115">Dit is een ontwerp en geen fout.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-115">This is by design and not an error.</span></span>

<span data-ttu-id="dc7fd-116">Selecteer **accepteren** en **door gaan** om door te gaan.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="dc7fd-117">Als de IT-afdeling zich heeft **aangemeld voor partner centrum**.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="dc7fd-118">Dit bericht wordt weer gegeven omdat er virus gebruikers zijn uitgeschakeld of omdat een virus registratie is uitgeschakeld op de Azure AD-Tenant.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="dc7fd-119">De globale beheerder voor uw Azure AD-account kan de vereiste functies inschakelen door de volgende Power shell-opdracht uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="dc7fd-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="dc7fd-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="dc7fd-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="dc7fd-121">Lees voor meer informatie [self-service registreren](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="dc7fd-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="dc7fd-122">U hebt uw wacht woord verg eten</span><span class="sxs-lookup"><span data-stu-id="dc7fd-122">You forgot your password</span></span>

<span data-ttu-id="dc7fd-123">Als u uw wacht woord bent verg eten, selecteert u de koppeling **geen toegang tot uw account?** op de aanmeldings pagina.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="dc7fd-124">Met deze optie kunt u uw wacht woord opnieuw instellen of uw globale beheerder vragen om u nieuwe referenties toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="dc7fd-125">In het scherm ' vertel ons over uw bedrijf ' verschijnt de fout melding ' er is iets fout gegaan '</span><span class="sxs-lookup"><span data-stu-id="dc7fd-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="dc7fd-126">Dit fout bericht wordt meestal weer gegeven als u per ongeluk speciale tekens, spaties of land code gebruikt in het telefoon nummer van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="dc7fd-127">De waarde die is opgegeven in het veld telefoon nummer mag Maxi maal 10 tekens bevatten.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="dc7fd-128">Er wordt een fout bericht weer gegeven met de melding dat uw bestelling is afgewezen.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="dc7fd-129">Controleer uw gegevens</span><span class="sxs-lookup"><span data-stu-id="dc7fd-129">Please verify your information”</span></span>


<span data-ttu-id="dc7fd-130">Gebruik altijd het adres dat overeenkomt met uw credit card in plaats van uw juridische entiteit.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="dc7fd-131">Zorg er ook voor dat de post code juist is en overeenkomt met het adres dat u gebruikt.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="dc7fd-132">U wilt overschakelen van de offline betaling naar de online betalings methode</span><span class="sxs-lookup"><span data-stu-id="dc7fd-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="dc7fd-133">U moet de oorspronkelijke volg orde annuleren en kopen met de gewenste Betalings wijze.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="dc7fd-134">Een order annuleren:</span><span class="sxs-lookup"><span data-stu-id="dc7fd-134">To cancel an order:</span></span>

1. <span data-ttu-id="dc7fd-135">Selecteer het tabblad met **lidmaatschaps aanbiedingen** in het dash board.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="dc7fd-136">**Order annuleren** selecteren</span><span class="sxs-lookup"><span data-stu-id="dc7fd-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="dc7fd-137">Er wordt een bevestigings venster weer gegeven en u moet bevestigen om de oorspronkelijke volg orde te annuleren.</span><span class="sxs-lookup"><span data-stu-id="dc7fd-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="dc7fd-138">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="dc7fd-138">Next steps</span></span>

- [<span data-ttu-id="dc7fd-139">Uw Partner Center-account beheren</span><span class="sxs-lookup"><span data-stu-id="dc7fd-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="dc7fd-140">Uw factuur-en afstemmings bestand lezen</span><span class="sxs-lookup"><span data-stu-id="dc7fd-140">How to read your bill and recon file</span></span>](read-your-bill.md)
