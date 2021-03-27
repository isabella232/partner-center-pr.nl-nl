---
title: Controleren of uw klant de micro soft-klant overeenkomst heeft geaccepteerd voor het CSP-programma
description: Cloud Solution Provider (CSP)-partners moeten acceptatie van de klant bevestigen van de klant overeenkomst van micro soft voordat ze micro soft-Services voor klanten best Ellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633775"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="e91fc-103">Controleren of uw klant de micro soft-klant overeenkomst heeft geaccepteerd voor het CSP-programma</span><span class="sxs-lookup"><span data-stu-id="e91fc-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="e91fc-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="e91fc-104">**Appropriate roles**</span></span>

- <span data-ttu-id="e91fc-105">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="e91fc-105">Admin agent</span></span>
- <span data-ttu-id="e91fc-106">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="e91fc-106">Sales agent</span></span>


<span data-ttu-id="e91fc-107">Klanten hebben twee opties voor het accepteren van de klant overeenkomst van micro soft.</span><span class="sxs-lookup"><span data-stu-id="e91fc-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="e91fc-108">**Optie 1**: partner attest van klant acceptatie: de partner kan acceptatie van de klant bevestigen met de Partner Center API/SDK of via het dash board van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="e91fc-109">**Optie 2**: klant direct accepteren-partner kan de klant via een URL uitnodigen om de overeenkomst in het Microsoft 365-beheer centrum te bekijken en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="e91fc-110">Toegang tot micro soft-sjabloon voor klant overeenkomst</span><span class="sxs-lookup"><span data-stu-id="e91fc-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="e91fc-111">U kunt de nieuwste [versie van de](https://aka.ms/customeragreement)micro soft-sjabloon voor klant overeenkomsten hand matig downloaden.</span><span class="sxs-lookup"><span data-stu-id="e91fc-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="e91fc-112">De klant overeenkomst van micro soft is specifiek voor het land.</span><span class="sxs-lookup"><span data-stu-id="e91fc-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="e91fc-113">Zorg ervoor dat u het juiste land selecteert op basis van de locatie van de klant wanneer u de micro soft-sjabloon voor klant overeenkomsten aanvraagt.</span><span class="sxs-lookup"><span data-stu-id="e91fc-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="e91fc-114">Optie 1: acceptatie van klant bevestigen in partner centrum</span><span class="sxs-lookup"><span data-stu-id="e91fc-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="e91fc-115">Directe factuur partners kunnen acceptatie van klant bevestigen van de klant overeenkomst van micro soft in het partner centrum voor nieuwe en bestaande klanten.</span><span class="sxs-lookup"><span data-stu-id="e91fc-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="e91fc-116">Indirecte wederverkopers kunnen geen attesten namens hun klanten afgeven en moeten samen werken met hun indirecte provider om de Attestation te kunnen volt ooien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="e91fc-117">Acceptatie van klant bevestigen voor nieuwe klanten</span><span class="sxs-lookup"><span data-stu-id="e91fc-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="e91fc-118">Wanneer u een nieuwe eigenaar van de klant in het partner centrum maakt, moet u de volgende stappen gebruiken om de acceptatie van de klant overeenkomst van micro soft te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e91fc-119">U moet een beheer agent of een verkoop agent zijn om deze stappen uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="e91fc-120">Selecteer **klanten** en vervolgens **nieuwe klant**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="e91fc-121">Voer onder **account info** informatie in voor het bedrijf en de primaire contact persoon.</span><span class="sxs-lookup"><span data-stu-id="e91fc-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="e91fc-122">Schakel onder **micro soft Agreement** het selectie vakje in om te bevestigen dat de klant de micro soft-klant overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="e91fc-123">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="e91fc-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e91fc-124">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="e91fc-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="e91fc-125">Zorg ervoor dat de contact gegevens van de primaire gebruiker correct worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="e91fc-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="e91fc-126">Als het niet juist is, selecteert u **bijwerken** en voert u de juiste informatie in voor de persoon die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="e91fc-127">Selecteer **volgende** om door te gaan met het maken van de Tenant van de klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nieuwe klant":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="e91fc-129">Acceptatie van klant bevestigen voor bestaande klanten</span><span class="sxs-lookup"><span data-stu-id="e91fc-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="e91fc-130">U moet een beheer agent of verkoop agent zijn om dit te kunnen doen:</span><span class="sxs-lookup"><span data-stu-id="e91fc-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="e91fc-131">Selecteer **Klanten**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-131">Select **Customers**.</span></span> <span data-ttu-id="e91fc-132">Zoek en selecteer de klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-132">Find and select the customer.</span></span>

2. <span data-ttu-id="e91fc-133">Selecteer **account gegevens**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-133">Select **Account info**.</span></span>

3. <span data-ttu-id="e91fc-134">Selecteer in de **micro soft-klant overeenkomst** **Update**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="e91fc-135">Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="e91fc-136">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="e91fc-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e91fc-137">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="e91fc-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="e91fc-138">Selecteer **Opslaan** en door gaan.</span><span class="sxs-lookup"><span data-stu-id="e91fc-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestaande klant":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="e91fc-140">Bevestiging van acceptatie van klant ophalen</span><span class="sxs-lookup"><span data-stu-id="e91fc-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="e91fc-141">Gebruik de volgende stappen om de bevestiging te verkrijgen dat een bestaande klant de micro soft-klant overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="e91fc-142">U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="e91fc-143">Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="e91fc-144">Selecteer **account gegevens**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-144">Select **Account info**.</span></span>

3. <span data-ttu-id="e91fc-145">Onder de **klant overeenkomst van micro soft** wordt weer gegeven of er een bevestiging is ontvangen door deze klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="e91fc-146">Acceptatie van klant bevestigen met partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="e91fc-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="e91fc-147">U kunt de API/SDK van partner Center gebruiken om de acceptatie van de klant van micro soft te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e91fc-148">Raadpleeg voor meer informatie over de API/SDK:</span><span class="sxs-lookup"><span data-stu-id="e91fc-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="e91fc-149">Metagegevens van de overeenkomst voor de Microsoft-klantovereenkomst ophalen</span><span class="sxs-lookup"><span data-stu-id="e91fc-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="e91fc-150">Acceptatie door de klant van Microsoft-klantovereenkomst bevestigen</span><span class="sxs-lookup"><span data-stu-id="e91fc-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="e91fc-151">Bevestiging van acceptatie door de klant van Microsoft-klantovereenkomst ophalen</span><span class="sxs-lookup"><span data-stu-id="e91fc-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="e91fc-152">Een download koppeling voor de micro soft-sjabloon voor klant overeenkomsten ophalen</span><span class="sxs-lookup"><span data-stu-id="e91fc-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="e91fc-153">Optie 2: acceptatie van klant in Microsoft 365-beheer centrum</span><span class="sxs-lookup"><span data-stu-id="e91fc-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="e91fc-154">Partners kunnen nieuwe en bestaande klanten uitnodigen via een URL om de overeenkomst te bekijken en te accepteren binnen het Microsoft 365-beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="e91fc-155">In de volgende secties ziet u hoe u het volgende kunt doen:</span><span class="sxs-lookup"><span data-stu-id="e91fc-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="e91fc-156">Maak een nieuwe klant en vraag de klant om de overeenkomst te bekijken en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="e91fc-157">Een nieuwe klant uitnodigen om de wederverkoper-relatie en-overeenkomst te bekijken en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="e91fc-158">Een bestaande klant uitnodigen om de overeenkomst te bekijken en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="e91fc-159">U kunt de [API/SDK van partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) gebruiken om de status van de directe acceptatie van de klant van micro soft te verkrijgen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="e91fc-160">Een nieuwe klant maken en de klant uitnodigen om de overeenkomst te bekijken en te accepteren</span><span class="sxs-lookup"><span data-stu-id="e91fc-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="e91fc-161">Voer de volgende stappen uit om een nieuwe klant te maken in het partner centrum en vraag ze om de klant overeenkomst van micro soft te bekijken en te accepteren binnen Microsoft 365 beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="e91fc-162">Selecteer **klant toevoegen** op het tabblad **klanten** binnen partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="e91fc-163">Voer onder **account gegevens** informatie over de nieuwe klant in alle vereiste velden in, waaronder de bedrijfs naam en de primaire contact persoon van de klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="e91fc-164">Onder **klant overeenkomst** selecteert **u de optie klant wordt gevraagd om de micro soft-klant overeenkomst in Microsoft 365 beheer centrum te accepteren**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="e91fc-165">Alle andere verplichte velden op de pagina volt ooien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="e91fc-166">Selecteer **volgende: controleren** en ga door met de stappen voor het maken van de Tenant van de klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="e91fc-167">Nieuwe klanten kunnen pas een aankoop doen als ze de micro soft-klant overeenkomst accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Nieuwe klant maken":::

5. <span data-ttu-id="e91fc-169">Wanneer u het **bevestigings** scherm in de nieuwe klant werk stroom bereikt, slaat u de referenties van de klant op.</span><span class="sxs-lookup"><span data-stu-id="e91fc-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="e91fc-170">U moet deze referenties later aan uw klant verlenen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="e91fc-171">Maak en verzend buiten het partner centrum een e-mail die de klant nodig heeft om de micro soft-klant overeenkomst te accepteren in Microsoft 365 beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="e91fc-172">Zorg ervoor dat u deze items opneemt in het e-mail bericht:</span><span class="sxs-lookup"><span data-stu-id="e91fc-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="e91fc-173">Een koppeling naar deze [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (aanmelden vereist)</span><span class="sxs-lookup"><span data-stu-id="e91fc-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="e91fc-174">De referenties van de klant die u hebt opgeslagen in stap 5.</span><span class="sxs-lookup"><span data-stu-id="e91fc-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="e91fc-175">De klant ontvangt vervolgens de uitnodiging voor e-mail van de partner en selecteert de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="e91fc-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="e91fc-176">De klant meldt zich aan Microsoft 365 beheer centrum met de referenties van de klant die u hebt ingevoerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="e91fc-177">De klant controleert het vakje om de klant overeenkomst van micro soft te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="e91fc-178">Een nieuwe klant uitnodigen om de reseller relationship-en micro soft-klant overeenkomst te bekijken en te accepteren</span><span class="sxs-lookup"><span data-stu-id="e91fc-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="e91fc-179">Gebruik de volgende stappen om een nieuwe klant uit te nodigen om de reseller-relatie en de micro soft-klant overeenkomst te bekijken en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="e91fc-180">Selecteer **een reseller-relatie koppeling aanvragen** op het tabblad **klanten** binnen partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="e91fc-181">Er wordt een automatische e-mail sjabloon gegenereerd, inclusief tekst en een geparametriseerde URL die de klant doorstuurt naar het Microsoft 365-beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="e91fc-182">U kunt de automatisch gegenereerde e-mail sjabloon aanpassen en vervolgens **kopiëren naar klem bord** selecteren of **in e-mail bericht openen**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="e91fc-183">Gebruik deze e-mail sjabloon om de klant uit te nodigen om een **wederverkoper-relatie** aanvraag en de **micro soft-klant overeenkomst** te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="e91fc-184">(Opmerking: in de uitnodiging voor het e-mail bericht moet u ervoor zorgen dat de partner ook de URL bevat die automatisch is geleverd, evenals de referenties van de klant die onlangs zijn gemaakt.)</span><span class="sxs-lookup"><span data-stu-id="e91fc-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="een relatie maken":::

5. <span data-ttu-id="e91fc-186">Klant ontvangt uitnodiging via e-mail en klikt op de para meter-URL.</span><span class="sxs-lookup"><span data-stu-id="e91fc-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="e91fc-187">De klant gebruikt de referenties die u binnen e-mail verstrekt om zich aan te melden bij Microsoft 365-beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="e91fc-188">Klant controleert het vakje om de **reseller Relationship** en de **klant overeenkomst van micro soft** te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="e91fc-189">Binnen dezelfde URL is de klant in staat een geconsolideerde lijst te zien met verschillende partners waarmee ze werken.</span><span class="sxs-lookup"><span data-stu-id="e91fc-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="e91fc-190">Ze kunnen een partner selecteren om de details te zien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Overeenkomst accepteren":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="e91fc-192">Een bestaande klant uitnodigen om de overeenkomst te bekijken en te accepteren</span><span class="sxs-lookup"><span data-stu-id="e91fc-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="e91fc-193">Gebruik de volgende stappen om een bestaande klant uit te nodigen om de micro soft-klant overeenkomst te controleren en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="e91fc-194">Maak de e-mail van de klant met de Inge sloten URL die uw klant uitnodigt om de micro soft-klant overeenkomst te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="e91fc-195">Uw klant ontvangt de uitnodiging via e-mail en klikt op de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="e91fc-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="e91fc-196">De klant voert hun referenties in Microsoft 365-beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="e91fc-197">Uw klant controleert het vakje om de klant overeenkomst van micro soft te accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="e91fc-198">Binnen dezelfde URL kan de klant de geconsolideerde lijst zien van verschillende partners waarmee ze werken.</span><span class="sxs-lookup"><span data-stu-id="e91fc-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="e91fc-199">Ze kunnen een partner selecteren om de details te zien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="gebruikers":::

>[!NOTE]
><span data-ttu-id="e91fc-201">In bepaalde scenario's kunnen klanten de micro soft-klant overeenkomst mogelijk niet rechtstreeks accepteren.</span><span class="sxs-lookup"><span data-stu-id="e91fc-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="e91fc-202">Lees voor meer informatie over deze situaties twee scenario's waarbij u de volgende stappen moet afhandelen namens uw klant.</span><span class="sxs-lookup"><span data-stu-id="e91fc-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="e91fc-203">Twee scenario's waarin u namens uw klant moet worden verklaard</span><span class="sxs-lookup"><span data-stu-id="e91fc-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="e91fc-204">Er zijn twee scenario's waarbij klanten de micro soft-klant overeenkomst mogelijk niet direct kunnen accepteren binnen het Microsoft 365-beheer centrum.</span><span class="sxs-lookup"><span data-stu-id="e91fc-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="e91fc-205">**Scenario 1**: een bestaande klant heeft een van de volgende gekocht via een bestaande partner relationship: aanbiedingen, software-of software-abonnementen, gereserveerde instanties of Azure-abonnement.</span><span class="sxs-lookup"><span data-stu-id="e91fc-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="e91fc-206">De klant probeert nu een nieuwe aankoop te maken (met uitzonde ring van automatische verlenging).</span><span class="sxs-lookup"><span data-stu-id="e91fc-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="e91fc-207">Wanneer die klant op de URL klikt, ontvangt het bericht ' Neem contact op met uw partner om te bevestigen dat u de micro soft-klant overeenkomst accepteert. '</span><span class="sxs-lookup"><span data-stu-id="e91fc-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="e91fc-208">**Om dit op te lossen**, moet u namens de klant een verklaring doen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Scherm opname van Microsoft 365 beheer centrum pagina waarin u wordt gevraagd om uw partner te bereiken om acceptatie van de micro soft-klant overeenkomst te bevestigen.":::

<span data-ttu-id="e91fc-210">**Scenario 2**: een bestaande klant heeft een van de volgende aanbiedingen gekocht, software-en software-abonnementen, gereserveerde instanties en Azure-abonnement.</span><span class="sxs-lookup"><span data-stu-id="e91fc-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="e91fc-211">De klant probeert nu een nieuwe aankoop te doen met een nieuwe partner.</span><span class="sxs-lookup"><span data-stu-id="e91fc-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="e91fc-212">Wanneer de klant op de URL klikt om het beheer centrum te Microsoft 365 om de nieuwe partner relatie en de overeenkomst te accepteren, ontvangen ze het bericht ' Neem contact op met uw partner om te bevestigen dat de micro soft-klant overeenkomst wordt geaccepteerd. '</span><span class="sxs-lookup"><span data-stu-id="e91fc-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="e91fc-213">**Om dit op te lossen**, moet u namens de klant een verklaring doen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="e91fc-214">Bevestigen dat een klant de overeenkomst heeft geaccepteerd</span><span class="sxs-lookup"><span data-stu-id="e91fc-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="e91fc-215">Als u probeert een nieuwe bestelling te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="e91fc-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="e91fc-216">Gebruik de volgende procedure om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="e91fc-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="e91fc-217">Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="e91fc-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="e91fc-218">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="e91fc-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="e91fc-219">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="e91fc-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="e91fc-220">Selecteer **Opslaan en doorgaan**.</span><span class="sxs-lookup"><span data-stu-id="e91fc-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="e91fc-221">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="e91fc-221">Next steps</span></span>

- [<span data-ttu-id="e91fc-222">De gegevens van uw bedrijfs profiel controleren of bijwerken</span><span class="sxs-lookup"><span data-stu-id="e91fc-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="e91fc-223">Microsoft-klantovereenkomsten (op regio, taal)</span><span class="sxs-lookup"><span data-stu-id="e91fc-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
