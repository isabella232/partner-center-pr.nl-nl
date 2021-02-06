---
title: Uitbetaling en belastingprofielen in het Partnercentrum
ms.topic: how-to
ms.date: 11/12/2020
description: Maak en beheer uw uitbetalings-en BTW-profiel zodat u kunt betalen voor uw prikkel werkzaamheden. Omvat het maken, beheren en gebruiken van verschillende profielen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624235"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8232b-104">Toekennings-en belasting profielen voor stimuli maken en beheren in partner centrum</span><span class="sxs-lookup"><span data-stu-id="8232b-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="8232b-105">**Juiste rollen:**</span><span class="sxs-lookup"><span data-stu-id="8232b-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="8232b-106">Prikkel beheerder</span><span class="sxs-lookup"><span data-stu-id="8232b-106">Incentives admin</span></span>
- <span data-ttu-id="8232b-107">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="8232b-107">Account admin</span></span>
- <span data-ttu-id="8232b-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="8232b-108">Global admin</span></span>

<span data-ttu-id="8232b-109">Voordat u een betaling kunt ontvangen voor uw incentive-programma's voor een bepaalde MPN-locatie, moet u uw inschrijving voltooien door een geldig betalings- en belastingprofiel te koppelen aan het programma en de MPN-locatie.</span><span class="sxs-lookup"><span data-stu-id="8232b-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="8232b-110">Microsoft gebruikt dit profiel om betalingen te doen.</span><span class="sxs-lookup"><span data-stu-id="8232b-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="8232b-111">U kunt mogelijk een bankoverboeking of een creditnota gebruiken voor betaling, afhankelijk van de regels van het incentive-programma.</span><span class="sxs-lookup"><span data-stu-id="8232b-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="8232b-112">Rollen, valuta's en andere micro soft-Program ma's</span><span class="sxs-lookup"><span data-stu-id="8232b-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="8232b-113">Het is belang rijk dat u de onderstaande informatie begrijpt voordat u aan de slag gaat met uw uitbetalings-en BTW-profiel.</span><span class="sxs-lookup"><span data-stu-id="8232b-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="8232b-114">Rollen en machtigingen</span><span class="sxs-lookup"><span data-stu-id="8232b-114">Roles and permissions</span></span>

<span data-ttu-id="8232b-115">U moet een stimulans beheerder zijn voor het invoeren van Bank-en belasting gegevens voor het stimuleren van betalingen.</span><span class="sxs-lookup"><span data-stu-id="8232b-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="8232b-116">Als u een MPN/account beheerder bent, kunt u zichzelf en/of een collega toewijzen als stimulans beheerder.</span><span class="sxs-lookup"><span data-stu-id="8232b-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="8232b-117">Neem contact op met uw MPN-beheerder of globale beheerder als u beheerders machtigingen voor prikkels wilt aanvragen. U kunt nagaan wie in uw bedrijf deze rollen heeft door zich aan te melden bij het [dash board van de partner centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="8232b-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="8232b-118">Klik op het pictogram **instellingen** rechtsboven op **gebruikers beheer** en vervolgens op globale beheerder filteren.</span><span class="sxs-lookup"><span data-stu-id="8232b-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="8232b-119">Gebruikers met prikkels kunnen prikkel winst en betalings gegevens en-rapporten weer geven, maar kunnen geen bank-en belasting gegevens bewerken.</span><span class="sxs-lookup"><span data-stu-id="8232b-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="8232b-120">Kies uw valuta voor schot</span><span class="sxs-lookup"><span data-stu-id="8232b-120">Choose your disbursement currency</span></span>

<span data-ttu-id="8232b-121">Belonings betalingen worden uitgevoerd in de valuta die u hebt geselecteerd bij het instellen van uw betalings profiel.</span><span class="sxs-lookup"><span data-stu-id="8232b-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="8232b-122">Betalingen worden berekend met behulp van een wissel koers die maandelijks door micro soft is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="8232b-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="8232b-123">Als gevolg van de geselecteerde valuta bent u verantwoordelijk voor eventuele wijzigingen in de waarde.</span><span class="sxs-lookup"><span data-stu-id="8232b-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="8232b-124">Verschillende profielen gebruiken voor verschillende micro soft-Program ma's</span><span class="sxs-lookup"><span data-stu-id="8232b-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="8232b-125">Als uw bedrijf is inge schreven in meerdere stimulerings Programma's, kunt u hetzelfde betalings account voor al deze Program ma's gebruiken of kiezen voor het gebruik van verschillende betalings accounts voor verschillende Program ma's.</span><span class="sxs-lookup"><span data-stu-id="8232b-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="8232b-126">Uitbetalings-en BTW-profielen maken en beheren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="8232b-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="8232b-127">In de volgende secties vindt u een overzicht van het proces voor het maken en beheren van betalings-en belasting profielen in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="8232b-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="8232b-128">U moet een stimulans beheerder zijn om betalings profielen te maken of te beheren in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="8232b-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="8232b-129">Prikkel rollen moeten worden toegewezen aan elke MPN-locatie onder elk stimulanss programma.</span><span class="sxs-lookup"><span data-stu-id="8232b-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="8232b-130">Zie voor meer informatie over het toevoegen van prikkel beheerders in Partner Center [gebruikers accounts maken](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="8232b-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="8232b-131">Toegang tot de sectie uitbetaling en belasting in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="8232b-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="8232b-132">Meld u aan bij het [Partner Center-dash board](https://partner.microsoft.com/dashboard/) met uw Azure Active Directory (Azure AD)-account (bedrijfs account) of het juiste e-mail adres als er een is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="8232b-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="8232b-133">Meerdere domeinen kunnen worden geregistreerd binnen één Azure AD-account.</span><span class="sxs-lookup"><span data-stu-id="8232b-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="8232b-134">Neem contact op met uw globale beheerder om te bepalen welke domeinen zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="8232b-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="8232b-135">Als u zich alleen kunt aanmelden met het @onmicrosoft.com domein, neemt u contact op met uw account beheerder om extra domeinen toe te voegen aan het Azure ad-account.</span><span class="sxs-lookup"><span data-stu-id="8232b-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="8232b-136">Als u wordt gevraagd om een **werk-of school account** of een **persoonlijk account** te selecteren, selecteert u **werk-of school account**.</span><span class="sxs-lookup"><span data-stu-id="8232b-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="8232b-137">Selecteer het tandwiel pictogram om het menu **instellingen** te openen en selecteer vervolgens **account instellingen**.</span><span class="sxs-lookup"><span data-stu-id="8232b-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="8232b-138">Selecteer in het menu **account instellingen** de optie **uitbetaling en belasting**.</span><span class="sxs-lookup"><span data-stu-id="8232b-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="8232b-139">Uitbetalings-en BTW-profielen toewijzen aan afzonderlijke Program ma's</span><span class="sxs-lookup"><span data-stu-id="8232b-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="8232b-140">Meld u aan bij het [dash board van het partner centrum](https://partner.microsoft.com/dashboard/)en selecteer vervolgens het tandwiel pictogram om het menu **instellingen** te openen.</span><span class="sxs-lookup"><span data-stu-id="8232b-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="8232b-141">Selecteer **account instellingen**, vouw de **sectie uitbetaling en belasting** uit en selecteer vervolgens **toekennings-en BTW-profiel toewijzing**.</span><span class="sxs-lookup"><span data-stu-id="8232b-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="8232b-142">Er wordt een lijst met uw Program ma's weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="8232b-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="8232b-143">Selecteer de pijl naast een programma om de profiel gegevens weer te geven.</span><span class="sxs-lookup"><span data-stu-id="8232b-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="8232b-144">Selecteer in het vervolg keuzemenu **BTW-profiel** het gewenste BTW-profiel of selecteer de optie om een nieuw profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="8232b-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8232b-145">Wanneer u de optie voor het maken van een nieuw profiel selecteert, wordt u naar behoren omgeleid.</span><span class="sxs-lookup"><span data-stu-id="8232b-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="8232b-146">Selecteer door gaan in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="8232b-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8232b-147">Het proces voor het maken van een nieuw BTW-profiel is hieronder beschreven.</span><span class="sxs-lookup"><span data-stu-id="8232b-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="8232b-148">Selecteer de **Betalings wijze**.</span><span class="sxs-lookup"><span data-stu-id="8232b-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="8232b-149">Als u **elektronische Bank overboeking** hebt geselecteerd als uw betalings wijze, selecteert u het gewenste betalings profiel of selecteert u de optie om een nieuw profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="8232b-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="8232b-150">Wanneer u de optie voor het maken van een nieuw profiel selecteert, wordt u naar behoren omgeleid.</span><span class="sxs-lookup"><span data-stu-id="8232b-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="8232b-151">Selecteer door gaan in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="8232b-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="8232b-152">Het proces voor het maken van een nieuw betalings profiel is hieronder opgenomen.</span><span class="sxs-lookup"><span data-stu-id="8232b-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="8232b-153">Als u **credit nota** hebt geselecteerd als Betalings wijze, voert u de verificatie uit.</span><span class="sxs-lookup"><span data-stu-id="8232b-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="8232b-154">Hiermee wordt bevestigd dat het SAP-nummer waarnaar wordt verwezen, deel uitmaakt van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="8232b-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8232b-155">Als er meerdere micro soft-bedrijfs entiteiten worden weer gegeven, moet u een betalings profiel voor elke entiteit selecteren.</span><span class="sxs-lookup"><span data-stu-id="8232b-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8232b-156">De beschik baarheid van de betalings wijze is afhankelijk van de regels van het prestatie programma.</span><span class="sxs-lookup"><span data-stu-id="8232b-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="8232b-157">Selecteer de **valuta**.</span><span class="sxs-lookup"><span data-stu-id="8232b-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="8232b-158">Wanneer u alle velden van betaling hebt ingevuld, selecteert u **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="8232b-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="8232b-159">Uw bank profiel maken</span><span class="sxs-lookup"><span data-stu-id="8232b-159">Create your bank profile</span></span>

<span data-ttu-id="8232b-160">Bank profielen worden op organisatie niveau gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8232b-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="8232b-161">Hierdoor kan één bank profiel worden toegewezen aan meerdere MPN-id's en stimulerings Programma's binnen een organisatie.</span><span class="sxs-lookup"><span data-stu-id="8232b-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="8232b-162">Er kunnen uitzonde ringen zijn bij het Toep assen van het Bank profiel in verschillende landen, omdat er mogelijk verschillende bank-en belasting regels van toepassing zijn.</span><span class="sxs-lookup"><span data-stu-id="8232b-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="8232b-163">Op de volgende pagina's zijn velden met een sterretje vereist.</span><span class="sxs-lookup"><span data-stu-id="8232b-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="8232b-164">Als u niet weet wat een veld is, selecteert u het informatie pictogram.</span><span class="sxs-lookup"><span data-stu-id="8232b-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="8232b-165">Vul op de pagina **Details** de volgende velden in: **profiel naam:** Voer een unieke naam in om dit betalings profiel aan te duiden.</span><span class="sxs-lookup"><span data-stu-id="8232b-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="8232b-166">**Locatie van bank account:** Het land waar de Bank van uw bedrijf zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="8232b-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="8232b-167">**Betalings wijze:** De betalings wijze die de voor keur heeft voor partner centrum is een elektronische bank overdracht.</span><span class="sxs-lookup"><span data-stu-id="8232b-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="8232b-168">Selecteer **Next**.</span><span class="sxs-lookup"><span data-stu-id="8232b-168">Select **Next**.</span></span>

3. <span data-ttu-id="8232b-169">Geef uw gegevens op de pagina **Bank account** op.</span><span class="sxs-lookup"><span data-stu-id="8232b-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="8232b-170">De velden die op deze pagina worden weer gegeven, variëren per land.</span><span class="sxs-lookup"><span data-stu-id="8232b-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="8232b-171">Selecteer **Next**.</span><span class="sxs-lookup"><span data-stu-id="8232b-171">Select **Next**.</span></span>

5. <span data-ttu-id="8232b-172">Voer op de pagina **begunstigde** de juiste informatie in.</span><span class="sxs-lookup"><span data-stu-id="8232b-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="8232b-173">De begunstigde is degene die de Bank zou contacteren als ze uw account moeten bespreken.</span><span class="sxs-lookup"><span data-stu-id="8232b-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="8232b-174">Wanneer de velden zijn voltooid, selecteert u **volt ooien** en selecteert u vervolgens **bevestigen** om uw bank profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="8232b-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="8232b-175">U wordt omgeleid naar de pagina **uitbetalings-en BTW-profielen** .</span><span class="sxs-lookup"><span data-stu-id="8232b-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="8232b-176">De status van uw nieuwe profiel wordt **in afwachting van micro soft-validatie** weer gegeven totdat de validatie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="8232b-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="8232b-177">Dit proces kan Maxi maal 48 uur duren.</span><span class="sxs-lookup"><span data-stu-id="8232b-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="8232b-178">Zodra de validatie is voltooid, wordt de profiel status weer gegeven als **goedgekeurd** of **actie vereist**.</span><span class="sxs-lookup"><span data-stu-id="8232b-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="8232b-179">Als **actie vereist** is, herhaalt u de bovenstaande stappen om de benodigde gegevens op te geven.</span><span class="sxs-lookup"><span data-stu-id="8232b-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="8232b-180">Uw BTW-profiel maken</span><span class="sxs-lookup"><span data-stu-id="8232b-180">Create your tax profile</span></span>

<span data-ttu-id="8232b-181">Gebruik de volgende procedure om micro soft te voorzien van de belasting gegevens die voor uw organisatie zijn vereist.</span><span class="sxs-lookup"><span data-stu-id="8232b-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="8232b-182">De pagina's in deze sectie zijn dynamisch en variëren op basis van uw land of regio.</span><span class="sxs-lookup"><span data-stu-id="8232b-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="8232b-183">Als u hulp nodig hebt bij het identificeren van de juiste belasting gegevens, neemt u contact op met de juiste overheids bronnen in uw land.</span><span class="sxs-lookup"><span data-stu-id="8232b-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="8232b-184">Als u informatie nodig hebt over het volt ooien van de W8-of W9-formulieren, kunt u voor partner bedrijven in het Amerikaans continent de volgende adressen gebruiken om naar de IRS-site te gaan:</span><span class="sxs-lookup"><span data-stu-id="8232b-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="8232b-185">Voer alleen details in voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8232b-185">Enter only details for your company.</span></span> <span data-ttu-id="8232b-186">Geef nooit persoonlijke gegevens op.</span><span class="sxs-lookup"><span data-stu-id="8232b-186">Never enter personal details.</span></span>

1. <span data-ttu-id="8232b-187">Vul op de pagina **zakelijk profiel** de vereiste velden in en selecteer **volgende**.</span><span class="sxs-lookup"><span data-stu-id="8232b-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="8232b-188">Selecteer op de pagina **instellen** de optie die van toepassing is op uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8232b-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="8232b-189">Selecteer de optie aan de linkerkant als uw bedrijf is opgenomen in de Verenigde Staten alleen, of als dit profiel voor een persoon is.</span><span class="sxs-lookup"><span data-stu-id="8232b-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="8232b-190">Selecteer de optie aan de rechter kant als uw bedrijf is opgenomen buiten het Verenigde Staten en selecteer uw land/regio in de lijst.</span><span class="sxs-lookup"><span data-stu-id="8232b-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="8232b-191">Selecteer **Next**.</span><span class="sxs-lookup"><span data-stu-id="8232b-191">Select **Next**.</span></span> 

4. <span data-ttu-id="8232b-192">Geef op de pagina **belasting status** de vereiste gegevens op en selecteer **volgende**.</span><span class="sxs-lookup"><span data-stu-id="8232b-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="8232b-193">De velden op deze pagina kunnen per land verschillen.</span><span class="sxs-lookup"><span data-stu-id="8232b-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="8232b-194">uw gegevens.</span><span class="sxs-lookup"><span data-stu-id="8232b-194">your details.</span></span> 

5. <span data-ttu-id="8232b-195">Op de pagina **extra documentatie** , de vereiste velden en selecteer **volgende**.</span><span class="sxs-lookup"><span data-stu-id="8232b-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="8232b-196">Selecteer **Bladeren** om documenten te uploaden die vereist zijn voor uw land of regio.</span><span class="sxs-lookup"><span data-stu-id="8232b-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="8232b-197">Wanneer de document naam wordt weer gegeven, selecteert u **uploaden**.</span><span class="sxs-lookup"><span data-stu-id="8232b-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="8232b-198">Selecteer **verwijderen** als u het document wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8232b-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="8232b-199">Selecteer **volt ooien** om op te slaan en door te gaan.</span><span class="sxs-lookup"><span data-stu-id="8232b-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="8232b-200">Selecteer **bevestigen** in het pop-upbericht.</span><span class="sxs-lookup"><span data-stu-id="8232b-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="8232b-201">U wordt teruggeleid naar de pagina voor het instellen van de **betaling en de BTW** .</span><span class="sxs-lookup"><span data-stu-id="8232b-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8232b-202">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="8232b-202">Next steps</span></span>

- [<span data-ttu-id="8232b-203">Veelgestelde vragen over uitbetalingen en belastingen</span><span class="sxs-lookup"><span data-stu-id="8232b-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
