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
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431754"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="ddbef-104">Problemen met accountinstallatie of MPN-verlenging oplossen</span><span class="sxs-lookup"><span data-stu-id="ddbef-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="ddbef-105">**Juiste rollen:** Globale | MPN-partnerbeheerder</span><span class="sxs-lookup"><span data-stu-id="ddbef-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="ddbef-106">Hier zijn enkele suggesties voor het oplossen van veelvoorkomende problemen die zich voordoen bij het instellen van Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="ddbef-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="ddbef-107">Wat gebeurt er als u migreert van Partner Membership Center en u geen velden met bedrijfsgegevens kunt bewerken</span><span class="sxs-lookup"><span data-stu-id="ddbef-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="ddbef-108">In gevallen waarin uw bedrijf al aanwezig is in Partner Center (bijvoorbeeld een Cloud Solution Provider(CSP)-account), wordt er een alleen-lezen scherm weergegeven.</span><span class="sxs-lookup"><span data-stu-id="ddbef-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="ddbef-109">In dit scherm wordt alle informatie over uw bedrijf weergegeven zoals deze bestaat in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddbef-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="ddbef-110">U kunt de details op dit scherm niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="ddbef-110">You can't change the details on this screen.</span></span> <span data-ttu-id="ddbef-111">Dit is een ontwerp en geen fout.</span><span class="sxs-lookup"><span data-stu-id="ddbef-111">This is by design and not an error.</span></span>

<span data-ttu-id="ddbef-112">Als u wilt doorgaan, **selecteert u** Accepteren en selecteert u **vervolgens Doorgaan.**</span><span class="sxs-lookup"><span data-stu-id="ddbef-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="ddbef-113">Als de IT-afdeling Aanmelden voor eenmalige **aanmelding heeft Partner Center**</span><span class="sxs-lookup"><span data-stu-id="ddbef-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="ddbef-114">U ziet dit bericht omdat virale gebruikers zijn uitgeschakeld of omdat virale aanmelding is uitgeschakeld op de Azure Active Directory (AD)-tenant.</span><span class="sxs-lookup"><span data-stu-id="ddbef-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="ddbef-115">De globale beheerder voor uw Azure AD-account kan vereiste functies inschakelen door de volgende PowerShell-opdracht uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="ddbef-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="ddbef-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="ddbef-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="ddbef-117">Lees Selfservice registreren [voor meer informatie.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="ddbef-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="ddbef-118">U bent uw wachtwoord vergeten</span><span class="sxs-lookup"><span data-stu-id="ddbef-118">You forgot your password</span></span>

<span data-ttu-id="ddbef-119">Als u uw wachtwoord bent vergeten, selecteert u Op de aanmeldingspagina de optie **Hebt u geen toegang tot uw account?**.</span><span class="sxs-lookup"><span data-stu-id="ddbef-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="ddbef-120">Met deze optie kunt u uw wachtwoord opnieuw instellen of uw globale beheerder vragen om u nieuwe referenties toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="ddbef-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="ddbef-121">Op het scherm Vertel ons over uw bedrijf ziet u de fout 'Er is iets misgegaan'</span><span class="sxs-lookup"><span data-stu-id="ddbef-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="ddbef-122">Dit foutbericht wordt meestal weergegeven als u per ongeluk speciale tekens, spaties of landcode in uw bedrijfstelefoonnummer gebruikt.</span><span class="sxs-lookup"><span data-stu-id="ddbef-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="ddbef-123">De waarde die is ingevoerd in het veld Telefoonnummer mag maximaal 10 tekens bevatten.</span><span class="sxs-lookup"><span data-stu-id="ddbef-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="ddbef-124">Uw creditcardaankoop ontvangt een foutbericht met de mededeling dat uw bestelling is afgewezen.</span><span class="sxs-lookup"><span data-stu-id="ddbef-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="ddbef-125">Controleer uw gegevens'</span><span class="sxs-lookup"><span data-stu-id="ddbef-125">Please verify your information”</span></span>


<span data-ttu-id="ddbef-126">Gebruik altijd het adres dat overeenkomt met uw creditcard in plaats van uw juridische entiteit.</span><span class="sxs-lookup"><span data-stu-id="ddbef-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="ddbef-127">Zorg er ook voor dat de postcode juist is en overeenkomt met het adres dat u gebruikt.</span><span class="sxs-lookup"><span data-stu-id="ddbef-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="ddbef-128">U wilt overschakelen van offline betaling naar online betalingswijze</span><span class="sxs-lookup"><span data-stu-id="ddbef-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="ddbef-129">U moet de oorspronkelijke order annuleren en de oorspronkelijke bestelling opnieuw inkopen met behulp van de gewenste betalingswijze.</span><span class="sxs-lookup"><span data-stu-id="ddbef-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="ddbef-130">Een order annuleren:</span><span class="sxs-lookup"><span data-stu-id="ddbef-130">To cancel an order:</span></span>

1. <span data-ttu-id="ddbef-131">Selecteer in Partner Center dashboard het tabblad **Lidmaatschapsaanbiedingen.**</span><span class="sxs-lookup"><span data-stu-id="ddbef-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="ddbef-132">Selecteer **Order annuleren**</span><span class="sxs-lookup"><span data-stu-id="ddbef-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="ddbef-133">Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.</span><span class="sxs-lookup"><span data-stu-id="ddbef-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ddbef-134">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="ddbef-134">Next steps</span></span>

- [<span data-ttu-id="ddbef-135">Uw Partner Center-account beheren</span><span class="sxs-lookup"><span data-stu-id="ddbef-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="ddbef-136">Uw factuur- en reconbestand lezen</span><span class="sxs-lookup"><span data-stu-id="ddbef-136">How to read your bill and recon file</span></span>](read-your-bill.md)
