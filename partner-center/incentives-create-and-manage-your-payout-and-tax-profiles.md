---
title: Uitbetaling en belastingprofielen in het Partnercentrum
ms.topic: how-to
ms.date: 09/11/2020
description: Maak en beheer uw uitbetalings-en BTW-profiel zodat u kunt betalen voor uw prikkel werkzaamheden. Omvat het maken, beheren en gebruiken van verschillende profielen.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528782"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="f295e-104">Toekennings-en belasting profielen voor stimuli maken en beheren in partner centrum</span><span class="sxs-lookup"><span data-stu-id="f295e-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="f295e-105">**Van toepassing op:**</span><span class="sxs-lookup"><span data-stu-id="f295e-105">**Applies to:**</span></span>

- <span data-ttu-id="f295e-106">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="f295e-106">Partner Center</span></span>

<span data-ttu-id="f295e-107">**Juiste rollen:**</span><span class="sxs-lookup"><span data-stu-id="f295e-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="f295e-108">Prikkel beheerder</span><span class="sxs-lookup"><span data-stu-id="f295e-108">Incentives admin</span></span>
- <span data-ttu-id="f295e-109">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="f295e-109">Billing admin</span></span>
- <span data-ttu-id="f295e-110">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f295e-110">Global admin</span></span>

<span data-ttu-id="f295e-111">Voordat u een betaling kunt ontvangen voor uw incentive-programma's voor een bepaalde MPN-locatie, moet u uw inschrijving voltooien door een geldig betalings- en belastingprofiel te koppelen aan het programma en de MPN-locatie.</span><span class="sxs-lookup"><span data-stu-id="f295e-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="f295e-112">Microsoft gebruikt dit profiel om betalingen te doen.</span><span class="sxs-lookup"><span data-stu-id="f295e-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="f295e-113">U kunt mogelijk een bankoverboeking of een creditnota gebruiken voor betaling, afhankelijk van de regels van het incentive-programma.</span><span class="sxs-lookup"><span data-stu-id="f295e-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="f295e-114">Rollen, valuta's en andere micro soft-Program ma's</span><span class="sxs-lookup"><span data-stu-id="f295e-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="f295e-115">Het is belang rijk dat u de onderstaande informatie begrijpt voordat u aan de slag gaat met uw uitbetalings-en BTW-profiel.</span><span class="sxs-lookup"><span data-stu-id="f295e-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="f295e-116">Rollen en machtigingen</span><span class="sxs-lookup"><span data-stu-id="f295e-116">Roles and permissions</span></span>

<span data-ttu-id="f295e-117">U moet een stimulans beheerder zijn voor het invoeren van Bank-en belasting gegevens voor het stimuleren van betalingen.</span><span class="sxs-lookup"><span data-stu-id="f295e-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="f295e-118">Als u een MPN/account beheerder bent, kunt u zichzelf en/of een collega toewijzen als stimulans beheerder.</span><span class="sxs-lookup"><span data-stu-id="f295e-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="f295e-119">Neem contact op met uw MPN-beheerder of globale beheerder als u beheerders machtigingen voor prikkels wilt aanvragen. U kunt nagaan wie in uw bedrijf deze rollen heeft door zich aan te melden bij het [dash board van de partner centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f295e-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="f295e-120">Klik op het pictogram **instellingen** rechtsboven op **gebruikers beheer** en vervolgens op globale beheerder filteren.</span><span class="sxs-lookup"><span data-stu-id="f295e-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="f295e-121">Gebruikers met prikkels kunnen prikkel winst en betalings gegevens en-rapporten weer geven, maar kunnen geen bank-en belasting gegevens bewerken.</span><span class="sxs-lookup"><span data-stu-id="f295e-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="f295e-122">Kies uw valuta voor schot</span><span class="sxs-lookup"><span data-stu-id="f295e-122">Choose your disbursement currency</span></span>

<span data-ttu-id="f295e-123">In de lokale valuta van elke respectieve entiteit worden standaard kosten voor het stimuleren van een stimulans gemaakt.</span><span class="sxs-lookup"><span data-stu-id="f295e-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="f295e-124">U kunt tijdens het instellen van het profiel een andere valuta opgeven.</span><span class="sxs-lookup"><span data-stu-id="f295e-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="f295e-125">Betalingen worden berekend met behulp van een wissel koers die maandelijks door micro soft is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="f295e-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="f295e-126">Als gevolg van de geselecteerde valuta bent u verantwoordelijk voor eventuele wijzigingen in de waarde.</span><span class="sxs-lookup"><span data-stu-id="f295e-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="f295e-127">Bank-en belasting gegevens en andere Program ma's</span><span class="sxs-lookup"><span data-stu-id="f295e-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="f295e-128">Geef de gegevens op die hieronder worden beschreven, zelfs als micro soft uw bank gegevens al gebruikt voor betalingen.</span><span class="sxs-lookup"><span data-stu-id="f295e-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="f295e-129">Dit zorgt voor de privacy en beveiliging van de gegevens van uw bedrijf, omdat het kopiëren van uw profiel naar het nieuwe hulp programma gevoelige informatie kan openbaren.</span><span class="sxs-lookup"><span data-stu-id="f295e-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="f295e-130">Door loop dit proces is ook een goede kans om ervoor te zorgen dat de gegevens volledig en nauw keurig zijn.</span><span class="sxs-lookup"><span data-stu-id="f295e-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="f295e-131">Verschillende profielen gebruiken voor verschillende micro soft-Program ma's</span><span class="sxs-lookup"><span data-stu-id="f295e-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="f295e-132">Binnen de detail handel kunnen betalingen voor elk van de vijf Retail prikkel-Program ma's naar dezelfde bank rekening gaan.</span><span class="sxs-lookup"><span data-stu-id="f295e-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="f295e-133">U kunt er ook voor kiezen om Retail Xbox-betalingen te laten gaan naar één bank rekening terwijl Retail Office wordt betaald aan een ander bank account.</span><span class="sxs-lookup"><span data-stu-id="f295e-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="f295e-134">Uitbetalings-en BTW-profielen maken en beheren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="f295e-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="f295e-135">In de volgende secties vindt u een overzicht van het proces voor het maken en beheren van betalings-en belasting profielen in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="f295e-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="f295e-136">U moet een stimulans beheerder zijn om betalings profielen te maken of te beheren in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="f295e-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="f295e-137">Prikkel rollen moeten worden toegewezen aan elke MPN-locatie onder elk stimulanss programma.</span><span class="sxs-lookup"><span data-stu-id="f295e-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="f295e-138">Zie voor meer informatie over het toevoegen van prikkel beheerders in Partner Center [gebruikers accounts maken](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="f295e-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="f295e-139">Toegang tot de sectie uitbetaling en belasting in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="f295e-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="f295e-140">Meld u aan bij het [Partner Center-dash board](https://partner.microsoft.com/dashboard/) met uw Azure Active Directory (Azure AD)-account (bedrijfs account) of het juiste e-mail adres als er een is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="f295e-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="f295e-141">Meerdere domeinen kunnen worden geregistreerd binnen één Azure AD-account.</span><span class="sxs-lookup"><span data-stu-id="f295e-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="f295e-142">Neem contact op met uw globale beheerder om te bepalen welke domeinen zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="f295e-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="f295e-143">Als u zich alleen kunt aanmelden met het @onmicrosoft.com domein, neemt u contact op met uw account beheerder om extra domeinen toe te voegen aan het Azure ad-account.</span><span class="sxs-lookup"><span data-stu-id="f295e-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="f295e-144">Als u wordt gevraagd om een **werk-of school account** of een **persoonlijk account** te selecteren, selecteert u **werk-of school account** .</span><span class="sxs-lookup"><span data-stu-id="f295e-144">If you're prompted to select **Work or school account** or **Personal Account** , select **Work or school account** .</span></span>

2. <span data-ttu-id="f295e-145">Selecteer het tandwiel pictogram om het menu **instellingen** te openen en selecteer vervolgens **partner instellingen** .</span><span class="sxs-lookup"><span data-stu-id="f295e-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings** .</span></span>

3. <span data-ttu-id="f295e-146">Selecteer in het menu **account instellingen** de optie **uitbetaling en belasting** .</span><span class="sxs-lookup"><span data-stu-id="f295e-146">In the **Account settings** menu, select **Payout and tax** .</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="f295e-147">Uitbetalings-en BTW-profielen toewijzen aan afzonderlijke Program ma's</span><span class="sxs-lookup"><span data-stu-id="f295e-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="f295e-148">Meld u aan bij het [dash board van het partner centrum](https://partner.microsoft.com/dashboard/)en selecteer vervolgens het tandwiel pictogram om het menu **instellingen** te openen.</span><span class="sxs-lookup"><span data-stu-id="f295e-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="f295e-149">Selecteer **partner instellingen** , vouw de **sectie uitbetaling en belasting** uit en selecteer vervolgens **toekennings-en BTW-profiel toewijzing** .</span><span class="sxs-lookup"><span data-stu-id="f295e-149">Select **Partner settings** , expand the **Payout and tax section** , and then select **Payout and tax profile assignment** .</span></span> 
   
   <span data-ttu-id="f295e-150">Er wordt een lijst met uw Program ma's weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="f295e-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="f295e-151">Selecteer de pijl naast een programma om de profiel gegevens weer te geven.</span><span class="sxs-lookup"><span data-stu-id="f295e-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="f295e-152">Selecteer in het vervolg keuzemenu **BTW-profiel** het gewenste BTW-profiel of selecteer de optie om een nieuw profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="f295e-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="f295e-153">Wanneer u de optie voor het maken van een nieuw profiel selecteert, wordt u naar behoren omgeleid.</span><span class="sxs-lookup"><span data-stu-id="f295e-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="f295e-154">Selecteer door gaan in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="f295e-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="f295e-155">Het proces voor het maken van een nieuw BTW-profiel is hieronder beschreven.</span><span class="sxs-lookup"><span data-stu-id="f295e-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="f295e-156">Selecteer de **Betalings wijze** .</span><span class="sxs-lookup"><span data-stu-id="f295e-156">Select **Payment method** .</span></span>

   - <span data-ttu-id="f295e-157">Als u **elektronische Bank overboeking** hebt geselecteerd als uw betalings wijze, selecteert u het gewenste betalings profiel of selecteert u de optie om een nieuw profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="f295e-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="f295e-158">Wanneer u de optie voor het maken van een nieuw profiel selecteert, wordt u naar behoren omgeleid.</span><span class="sxs-lookup"><span data-stu-id="f295e-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="f295e-159">Selecteer door gaan in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="f295e-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="f295e-160">Het proces voor het maken van een nieuw betalings profiel is hieronder opgenomen.</span><span class="sxs-lookup"><span data-stu-id="f295e-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="f295e-161">Als u **credit nota** hebt geselecteerd als Betalings wijze, voert u de verificatie uit.</span><span class="sxs-lookup"><span data-stu-id="f295e-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="f295e-162">Hiermee wordt bevestigd dat het SAP-nummer waarnaar wordt verwezen, deel uitmaakt van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="f295e-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="f295e-163">Als er meerdere micro soft-bedrijfs entiteiten worden weer gegeven, moet u een betalings profiel voor elke entiteit selecteren.</span><span class="sxs-lookup"><span data-stu-id="f295e-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="f295e-164">De beschik baarheid van de betalings wijze is afhankelijk van de regels van het prestatie programma.</span><span class="sxs-lookup"><span data-stu-id="f295e-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="f295e-165">Selecteer de **valuta** .</span><span class="sxs-lookup"><span data-stu-id="f295e-165">Select the **Currency** .</span></span>

6. <span data-ttu-id="f295e-166">Wanneer u alle velden van betaling hebt ingevuld, selecteert u **verzenden** .</span><span class="sxs-lookup"><span data-stu-id="f295e-166">When you’ve completed all of the payment fields, select **Submit** .</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="f295e-167">Uw bank profiel maken</span><span class="sxs-lookup"><span data-stu-id="f295e-167">Create your bank profile</span></span>

<span data-ttu-id="f295e-168">Bank profielen worden op organisatie niveau gemaakt.</span><span class="sxs-lookup"><span data-stu-id="f295e-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="f295e-169">Hierdoor kan één bank profiel worden toegewezen aan meerdere MPN-id's en stimulerings Programma's binnen een organisatie.</span><span class="sxs-lookup"><span data-stu-id="f295e-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="f295e-170">Er kunnen uitzonde ringen zijn bij het Toep assen van het Bank profiel in verschillende landen, omdat er mogelijk verschillende bank-en belasting regels van toepassing zijn.</span><span class="sxs-lookup"><span data-stu-id="f295e-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="f295e-171">Op de volgende pagina's zijn velden met een sterretje vereist.</span><span class="sxs-lookup"><span data-stu-id="f295e-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="f295e-172">Als u niet weet wat een veld is, selecteert u het informatie pictogram.</span><span class="sxs-lookup"><span data-stu-id="f295e-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="f295e-173">Vul op de pagina **Details** de volgende velden in: **profiel naam:** Voer een unieke naam in om dit betalings profiel aan te duiden.</span><span class="sxs-lookup"><span data-stu-id="f295e-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="f295e-174">**Locatie van bank account:** Het land waar de Bank van uw bedrijf zich bevindt.</span><span class="sxs-lookup"><span data-stu-id="f295e-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="f295e-175">**Betalings wijze:** De betalings wijze die de voor keur heeft voor partner centrum is een elektronische bank overdracht.</span><span class="sxs-lookup"><span data-stu-id="f295e-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="f295e-176">Selecteer **Next** .</span><span class="sxs-lookup"><span data-stu-id="f295e-176">Select **Next** .</span></span>

3. <span data-ttu-id="f295e-177">Geef uw gegevens op de pagina **Bank account** op.</span><span class="sxs-lookup"><span data-stu-id="f295e-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="f295e-178">De velden die op deze pagina worden weer gegeven, variëren per land.</span><span class="sxs-lookup"><span data-stu-id="f295e-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="f295e-179">Selecteer **Next** .</span><span class="sxs-lookup"><span data-stu-id="f295e-179">Select **Next** .</span></span>

5. <span data-ttu-id="f295e-180">Voer op de pagina **begunstigde** de juiste informatie in.</span><span class="sxs-lookup"><span data-stu-id="f295e-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="f295e-181">De begunstigde is degene die de Bank zou contacteren als ze uw account moeten bespreken.</span><span class="sxs-lookup"><span data-stu-id="f295e-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="f295e-182">Wanneer de velden zijn voltooid, selecteert u **volt ooien** en selecteert u vervolgens **bevestigen** om uw bank profiel te maken.</span><span class="sxs-lookup"><span data-stu-id="f295e-182">When the fields are completed, select **Finish** , and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="f295e-183">U wordt omgeleid naar de pagina **uitbetalings-en BTW-profielen** .</span><span class="sxs-lookup"><span data-stu-id="f295e-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="f295e-184">De status van uw nieuwe profiel wordt **in afwachting van micro soft-validatie** weer gegeven totdat de validatie is voltooid.</span><span class="sxs-lookup"><span data-stu-id="f295e-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="f295e-185">Dit proces kan Maxi maal 48 uur duren.</span><span class="sxs-lookup"><span data-stu-id="f295e-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="f295e-186">Zodra de validatie is voltooid, wordt de profiel status weer gegeven als **goedgekeurd** of **actie vereist** .</span><span class="sxs-lookup"><span data-stu-id="f295e-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required** .</span></span> <span data-ttu-id="f295e-187">Als **actie vereist** is, herhaalt u de bovenstaande stappen om de benodigde gegevens op te geven.</span><span class="sxs-lookup"><span data-stu-id="f295e-187">If **Action Required** , repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="f295e-188">Uw BTW-profiel maken</span><span class="sxs-lookup"><span data-stu-id="f295e-188">Create your tax profile</span></span>

<span data-ttu-id="f295e-189">Gebruik de volgende procedure om micro soft te voorzien van de belasting gegevens die voor uw organisatie zijn vereist.</span><span class="sxs-lookup"><span data-stu-id="f295e-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="f295e-190">De pagina's in deze sectie zijn dynamisch en variëren op basis van uw land of regio.</span><span class="sxs-lookup"><span data-stu-id="f295e-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="f295e-191">Als u hulp nodig hebt bij het identificeren van de juiste belasting gegevens, neemt u contact op met de juiste overheids bronnen in uw land.</span><span class="sxs-lookup"><span data-stu-id="f295e-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="f295e-192">Als u informatie nodig hebt over het volt ooien van de W8-of W9-formulieren, kunt u voor partner bedrijven in het Amerikaans continent de volgende adressen gebruiken om naar de IRS-site te gaan:</span><span class="sxs-lookup"><span data-stu-id="f295e-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="f295e-193">Voer alleen details in voor uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="f295e-193">Enter only details for your company.</span></span> <span data-ttu-id="f295e-194">Geef nooit persoonlijke gegevens op.</span><span class="sxs-lookup"><span data-stu-id="f295e-194">Never enter personal details.</span></span>

1. <span data-ttu-id="f295e-195">Vul op de pagina **zakelijk profiel** de vereiste velden in en selecteer **volgende** .</span><span class="sxs-lookup"><span data-stu-id="f295e-195">On the **Business Profile** page, complete the required fields and then select **Next** .</span></span> 

2. <span data-ttu-id="f295e-196">Selecteer op de pagina **instellen** de optie die van toepassing is op uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="f295e-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="f295e-197">Selecteer de optie aan de linkerkant als uw bedrijf is opgenomen in de Verenigde Staten alleen, of als dit profiel voor een persoon is.</span><span class="sxs-lookup"><span data-stu-id="f295e-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="f295e-198">Selecteer de optie aan de rechter kant als uw bedrijf is opgenomen buiten het Verenigde Staten en selecteer uw land/regio in de lijst.</span><span class="sxs-lookup"><span data-stu-id="f295e-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="f295e-199">Selecteer **Next** .</span><span class="sxs-lookup"><span data-stu-id="f295e-199">Select **Next** .</span></span> 

4. <span data-ttu-id="f295e-200">Geef op de pagina **belasting status** de vereiste gegevens op en selecteer **volgende** .</span><span class="sxs-lookup"><span data-stu-id="f295e-200">On the **Tax status** page, enter the required information, and then select **Next** .</span></span> <span data-ttu-id="f295e-201">De velden op deze pagina kunnen per land verschillen.</span><span class="sxs-lookup"><span data-stu-id="f295e-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="f295e-202">uw gegevens.</span><span class="sxs-lookup"><span data-stu-id="f295e-202">your details.</span></span> 

5. <span data-ttu-id="f295e-203">Op de pagina **extra documentatie** , de vereiste velden en selecteer **volgende** .</span><span class="sxs-lookup"><span data-stu-id="f295e-203">On the **Additional documentation** page, the required fields and select **Next** .</span></span> 

6. <span data-ttu-id="f295e-204">Selecteer **Bladeren** om documenten te uploaden die vereist zijn voor uw land of regio.</span><span class="sxs-lookup"><span data-stu-id="f295e-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="f295e-205">Wanneer de document naam wordt weer gegeven, selecteert u **uploaden** .</span><span class="sxs-lookup"><span data-stu-id="f295e-205">When the document name is shown, select **Upload** .</span></span> 

7. <span data-ttu-id="f295e-206">Selecteer **verwijderen** als u het document wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="f295e-206">If you need to remove the document, select **Remove** .</span></span>

8. <span data-ttu-id="f295e-207">Selecteer **volt ooien** om op te slaan en door te gaan.</span><span class="sxs-lookup"><span data-stu-id="f295e-207">To save and continue, select **Finish** .</span></span>

9. <span data-ttu-id="f295e-208">Selecteer **bevestigen** in het pop-upbericht.</span><span class="sxs-lookup"><span data-stu-id="f295e-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="f295e-209">U wordt teruggeleid naar de pagina voor het instellen van de **betaling en de BTW** .</span><span class="sxs-lookup"><span data-stu-id="f295e-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f295e-210">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f295e-210">Next steps</span></span>

- [<span data-ttu-id="f295e-211">Veelgestelde vragen over prikkels en BTW-profielen</span><span class="sxs-lookup"><span data-stu-id="f295e-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
