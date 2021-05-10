---
title: Problemen met het instellen van Partner Center-account of MPN-verlenging oplossen
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Problemen oplossen bij het registreren bij Partner Center. Antwoorden op problemen met betalingswijzen, het vergeten van wachtwoorden en meer.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686259"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="af8d6-104">Problemen met accountinstallatie of MPN-verlenging oplossen</span><span class="sxs-lookup"><span data-stu-id="af8d6-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="af8d6-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="af8d6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="af8d6-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="af8d6-106">Global admin</span></span>
- <span data-ttu-id="af8d6-107">MPN-partnerbeheerder</span><span class="sxs-lookup"><span data-stu-id="af8d6-107">MPN partner admin</span></span>
 
<span data-ttu-id="af8d6-108">Hier zijn enkele suggesties voor het oplossen van veelvoorkomende problemen die zich voordoen bij het instellen van uw Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="af8d6-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="af8d6-109">Wat gebeurt er als u migreert van Partner Membership Center en u geen velden met bedrijfsgegevens kunt bewerken</span><span class="sxs-lookup"><span data-stu-id="af8d6-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="af8d6-110">In gevallen waarin uw bedrijf al aanwezig is in Partner Center (bijvoorbeeld een CSP-account), wordt een alleen-lezen scherm weergegeven.</span><span class="sxs-lookup"><span data-stu-id="af8d6-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="af8d6-111">In dit scherm wordt alle informatie over uw bedrijf weergegeven zoals deze bestaat in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="af8d6-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="af8d6-112">U kunt de details op dit scherm niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="af8d6-112">You can't change the details on this screen.</span></span> <span data-ttu-id="af8d6-113">Dit is een ontwerp en geen fout.</span><span class="sxs-lookup"><span data-stu-id="af8d6-113">This is by design and not an error.</span></span>

<span data-ttu-id="af8d6-114">Selecteer **Accepteren** en **Doorgaan om door** te gaan.</span><span class="sxs-lookup"><span data-stu-id="af8d6-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="af8d6-115">Als de IT-afdeling Aanmelden voor eenmalige **aanmelding heeft Partner Center**</span><span class="sxs-lookup"><span data-stu-id="af8d6-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="af8d6-116">U ziet dit bericht omdat virale gebruikers zijn uitgeschakeld of omdat virale aanmelding is uitgeschakeld in de Azure AD-tenant.</span><span class="sxs-lookup"><span data-stu-id="af8d6-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="af8d6-117">De globale beheerder voor uw Azure AD-account kan vereiste functies inschakelen door de volgende PowerShell-opdracht uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="af8d6-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="af8d6-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="af8d6-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="af8d6-119">Lees Selfservice registreren [voor meer informatie.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="af8d6-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="af8d6-120">U bent uw wachtwoord vergeten</span><span class="sxs-lookup"><span data-stu-id="af8d6-120">You forgot your password</span></span>

<span data-ttu-id="af8d6-121">Als u uw wachtwoord bent vergeten, selecteert u de koppeling Hebt u geen toegang tot uw **account?** op de aanmeldingspagina.</span><span class="sxs-lookup"><span data-stu-id="af8d6-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="af8d6-122">Met deze optie kunt u uw wachtwoord opnieuw instellen of uw globale beheerder vragen om u nieuwe referenties toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="af8d6-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="af8d6-123">Op het scherm Vertel ons over uw bedrijf ziet u de fout 'Er is iets misgegaan'</span><span class="sxs-lookup"><span data-stu-id="af8d6-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="af8d6-124">Dit foutbericht wordt meestal weergegeven als u per ongeluk speciale tekens, spaties of landcode in uw bedrijfstelefoonnummer gebruikt.</span><span class="sxs-lookup"><span data-stu-id="af8d6-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="af8d6-125">De waarde die is ingevoerd in het veld Telefoonnummer mag maximaal 10 tekens bevatten.</span><span class="sxs-lookup"><span data-stu-id="af8d6-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="af8d6-126">Uw creditcardaankoop ontvangt een foutbericht met de mededeling dat uw bestelling is afgewezen.</span><span class="sxs-lookup"><span data-stu-id="af8d6-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="af8d6-127">Controleer uw gegevens"</span><span class="sxs-lookup"><span data-stu-id="af8d6-127">Please verify your information”</span></span>


<span data-ttu-id="af8d6-128">Gebruik altijd het adres dat overeenkomt met uw creditcard in plaats van uw juridische entiteit.</span><span class="sxs-lookup"><span data-stu-id="af8d6-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="af8d6-129">Zorg er ook voor dat de postcode juist is en overeenkomt met het adres dat u gebruikt.</span><span class="sxs-lookup"><span data-stu-id="af8d6-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="af8d6-130">U wilt overschakelen van offline betaling naar online betalingswijze</span><span class="sxs-lookup"><span data-stu-id="af8d6-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="af8d6-131">U moet de oorspronkelijke order annuleren en de oorspronkelijke bestelling opnieuw inkopen met behulp van de gewenste betalingswijze.</span><span class="sxs-lookup"><span data-stu-id="af8d6-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="af8d6-132">Een order annuleren:</span><span class="sxs-lookup"><span data-stu-id="af8d6-132">To cancel an order:</span></span>

1. <span data-ttu-id="af8d6-133">Selecteer **het tabblad Lidmaatschapsaanbiedingen** in het dashboard.</span><span class="sxs-lookup"><span data-stu-id="af8d6-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="af8d6-134">Selecteer **Order annuleren**</span><span class="sxs-lookup"><span data-stu-id="af8d6-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="af8d6-135">Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.</span><span class="sxs-lookup"><span data-stu-id="af8d6-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="af8d6-136">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="af8d6-136">Next steps</span></span>

- [<span data-ttu-id="af8d6-137">Uw Partner Center-account beheren</span><span class="sxs-lookup"><span data-stu-id="af8d6-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="af8d6-138">Uw factuur- en reconbestand lezen</span><span class="sxs-lookup"><span data-stu-id="af8d6-138">How to read your bill and recon file</span></span>](read-your-bill.md)
