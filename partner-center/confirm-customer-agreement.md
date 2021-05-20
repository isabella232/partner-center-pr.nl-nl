---
title: Controleren of uw klant de Microsoft-klantovereenkomst heeft geaccepteerd voor het CSP-programma
description: Cloud Solution Provider (CSP)-partners moeten de klantacceptatie van de Microsoft-klantovereenkomst bevestigen voordat ze Microsoft-services klanten bestellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: c75f129ae5a0755833462138f60901cc7ff36732
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148513"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="ed904-103">Controleren of uw klant de Microsoft-klantovereenkomst heeft geaccepteerd voor het CSP-programma</span><span class="sxs-lookup"><span data-stu-id="ed904-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="ed904-104">**Juiste rollen:** beheeragent | Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="ed904-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="ed904-105">Klanten hebben twee opties voor de manier waarop ze de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="ed904-106">**Optie 1:** Partnerverklaring van klantacceptatie: de partner kan de acceptatie van de klant bevestigen met behulp van Partner Center API/SDK of via het Partner Center dashboard.</span><span class="sxs-lookup"><span data-stu-id="ed904-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="ed904-107">**Optie 2:** directe acceptatie door de klant: de partner kan de klant via een URL uitnodigen om de overeenkomst te controleren en te accepteren in het Microsoft 365-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="ed904-108">Toegang Microsoft-klantovereenkomst sjabloon</span><span class="sxs-lookup"><span data-stu-id="ed904-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="ed904-109">U kunt hier handmatig de nieuwste versie van de Microsoft-klantovereenkomst [downloaden.](https://aka.ms/customeragreement)</span><span class="sxs-lookup"><span data-stu-id="ed904-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="ed904-110">De Microsoft-klantovereenkomst is specifiek voor het land.</span><span class="sxs-lookup"><span data-stu-id="ed904-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="ed904-111">Wanneer u de sjabloon Microsoft-klantovereenkomst, moet u het juiste land selecteren op basis van de locatie van de klant.</span><span class="sxs-lookup"><span data-stu-id="ed904-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="ed904-112">Optie 1: Bevestig de acceptatie van de klant in Partner Center</span><span class="sxs-lookup"><span data-stu-id="ed904-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="ed904-113">Partners met directe factuur kunnen bevestigen dat de klant de Microsoft-klantovereenkomst in Partner Center nieuwe en bestaande klanten.</span><span class="sxs-lookup"><span data-stu-id="ed904-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="ed904-114">Indirecte resellers kunnen niet namens hun klanten bevestigen en moeten samenwerken met hun indirecte provider om de attestation te laten uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="ed904-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="ed904-115">Acceptatie van de klant bevestigen voor nieuwe klanten</span><span class="sxs-lookup"><span data-stu-id="ed904-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="ed904-116">Wanneer u een nieuwe klant-tenant maakt in Partner Center, gebruikt u de volgende stappen om te bevestigen dat de klant de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="ed904-117">U moet een beheerderagent of verkoopagent zijn om deze stappen uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="ed904-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="ed904-118">Selecteer **Klanten** en vervolgens **Nieuwe klant.**</span><span class="sxs-lookup"><span data-stu-id="ed904-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="ed904-119">Voer **onder Accountgegevens** de gegevens voor het bedrijf en de primaire contactpersoon in.</span><span class="sxs-lookup"><span data-stu-id="ed904-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="ed904-120">Schakel **onder Microsoft-overeenkomst** het selectievakje in om te bevestigen dat de klant de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="ed904-121">Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="ed904-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="ed904-122">U kunt dit niet instellen op een toekomstige datum.</span><span class="sxs-lookup"><span data-stu-id="ed904-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="ed904-123">Zorg ervoor dat de weergegeven contactgegevens van de primaire gebruiker juist zijn.</span><span class="sxs-lookup"><span data-stu-id="ed904-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="ed904-124">Als dit onjuist is, selecteert u **Bijwerken** en voert u de juiste informatie in voor de persoon die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="ed904-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="ed904-125">Selecteer **Volgende om** door te gaan met het maken van de tenant van de klant.</span><span class="sxs-lookup"><span data-stu-id="ed904-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nieuwe klant":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="ed904-127">Klantacceptatie voor bestaande klanten bevestigen</span><span class="sxs-lookup"><span data-stu-id="ed904-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="ed904-128">U moet een beheerderagent of verkoopagent zijn om dit te doen:</span><span class="sxs-lookup"><span data-stu-id="ed904-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="ed904-129">Selecteer **Klanten**.</span><span class="sxs-lookup"><span data-stu-id="ed904-129">Select **Customers**.</span></span> <span data-ttu-id="ed904-130">Zoek en selecteer de klant.</span><span class="sxs-lookup"><span data-stu-id="ed904-130">Find and select the customer.</span></span>

2. <span data-ttu-id="ed904-131">Selecteer **Accountgegevens.**</span><span class="sxs-lookup"><span data-stu-id="ed904-131">Select **Account info**.</span></span>

3. <span data-ttu-id="ed904-132">Selecteer **onder Microsoft-klantovereenkomst** de optie **Bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="ed904-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="ed904-133">Voer de **voornaam,** **achternaam,** het **e-mailadres** en **het** telefoonnummer (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="ed904-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="ed904-134">Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="ed904-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="ed904-135">U kunt dit niet instellen op een toekomstige datum.</span><span class="sxs-lookup"><span data-stu-id="ed904-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="ed904-136">Selecteer **Opslaan** en doorgaan.</span><span class="sxs-lookup"><span data-stu-id="ed904-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestaande klant":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="ed904-138">Bevestiging van klantacceptatie ophalen</span><span class="sxs-lookup"><span data-stu-id="ed904-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="ed904-139">Als u bevestiging wilt ophalen dat een bestaande klant de Microsoft-klantovereenkomst heeft geaccepteerd, gebruikt u de volgende stappen.</span><span class="sxs-lookup"><span data-stu-id="ed904-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="ed904-140">U moet een beheerderagent of verkoopagent zijn om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="ed904-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="ed904-141">Selecteer **Klanten** en zoek en selecteer vervolgens de klant die u wilt zien.</span><span class="sxs-lookup"><span data-stu-id="ed904-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="ed904-142">Selecteer **Accountgegevens.**</span><span class="sxs-lookup"><span data-stu-id="ed904-142">Select **Account info**.</span></span>

3. <span data-ttu-id="ed904-143">Bekijk **onder Microsoft-klantovereenkomst** of er al dan niet bevestiging is gegeven door deze klant.</span><span class="sxs-lookup"><span data-stu-id="ed904-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="ed904-144">Klantacceptatie bevestigen met behulp Partner Center API/SDK</span><span class="sxs-lookup"><span data-stu-id="ed904-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="ed904-145">U kunt Partner Center API/SDK gebruiken om te bevestigen dat de klant de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="ed904-146">Voor meer informatie over de API/SDK raadpleegt u:</span><span class="sxs-lookup"><span data-stu-id="ed904-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="ed904-147">Metagegevens van de overeenkomst voor de Microsoft-klantovereenkomst ophalen</span><span class="sxs-lookup"><span data-stu-id="ed904-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="ed904-148">Acceptatie door de klant van Microsoft-klantovereenkomst bevestigen</span><span class="sxs-lookup"><span data-stu-id="ed904-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="ed904-149">Bevestiging van acceptatie door de klant van Microsoft-klantovereenkomst ophalen</span><span class="sxs-lookup"><span data-stu-id="ed904-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="ed904-150">Een downloadkoppeling voor de sjabloon Microsoft-klantovereenkomst downloaden</span><span class="sxs-lookup"><span data-stu-id="ed904-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="ed904-151">Optie 2: Klantacceptatie in Microsoft 365-beheercentrum</span><span class="sxs-lookup"><span data-stu-id="ed904-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="ed904-152">Partners kunnen nieuwe en bestaande klanten via een URL uitnodigen om de overeenkomst te controleren en te accepteren in Microsoft 365 Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="ed904-153">In de volgende secties ziet u hoe u het volgende kunt doen:</span><span class="sxs-lookup"><span data-stu-id="ed904-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="ed904-154">Maak een nieuwe klant en nodig de klant uit om de overeenkomst te beoordelen en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="ed904-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="ed904-155">Nodig een nieuwe klant uit om de resellerrelatie en overeenkomst te controleren en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="ed904-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="ed904-156">Nodig een bestaande klant uit om de overeenkomst te beoordelen en te accepteren.</span><span class="sxs-lookup"><span data-stu-id="ed904-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="ed904-157">U kunt Partner Center [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) gebruiken om de status op te halen van de directe acceptatie van de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="ed904-158">Maak een nieuwe klant en nodig de klant uit om de overeenkomst te beoordelen en te accepteren</span><span class="sxs-lookup"><span data-stu-id="ed904-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="ed904-159">Gebruik de volgende stappen om een nieuwe klant te maken in Partner Center nodig deze vervolgens uit om de Microsoft-klantovereenkomst te controleren en te accepteren in Microsoft 365 Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="ed904-160">Selecteer op **het** tabblad Klanten in Partner Center de optie **Klant toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="ed904-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="ed904-161">Voer **onder Accountgegevens** in alle vereiste velden informatie over de nieuwe klant in, met inbegrip van de bedrijfsnaam van de klant en de primaire contactpersoon.</span><span class="sxs-lookup"><span data-stu-id="ed904-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="ed904-162">Selecteer **onder Klantovereenkomst** de **optie Klant wordt gevraagd om de Microsoft-klantovereenkomst te Microsoft 365 in het beheercentrum.**</span><span class="sxs-lookup"><span data-stu-id="ed904-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="ed904-163">Vul alle andere vereiste velden op de pagina in.</span><span class="sxs-lookup"><span data-stu-id="ed904-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="ed904-164">Selecteer **Volgende: Controleren en** ga vervolgens verder met de stappen voor het maken van de tenant van de klant.</span><span class="sxs-lookup"><span data-stu-id="ed904-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="ed904-165">Nieuwe klanten kunnen pas een aankoop doen als ze de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Nieuwe klant maken":::

5. <span data-ttu-id="ed904-167">Wanneer u het **bevestigingsscherm** in de nieuwe klantwerkstroom bereikt, moet u de klantreferenties opslaan.</span><span class="sxs-lookup"><span data-stu-id="ed904-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="ed904-168">U moet deze referenties later aan uw klant geven.</span><span class="sxs-lookup"><span data-stu-id="ed904-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="ed904-169">Maak buiten Partner Center een e-mailbericht waarin de klant wordt uitgenodigd om de Microsoft-klantovereenkomst te Microsoft 365 het beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="ed904-170">Zorg ervoor dat u deze items in het e-mailbericht op neem:</span><span class="sxs-lookup"><span data-stu-id="ed904-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="ed904-171">Een koppeling naar deze [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (aanmelden vereist)</span><span class="sxs-lookup"><span data-stu-id="ed904-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="ed904-172">De referenties van de klant die u in stap 5 hebt opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="ed904-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="ed904-173">De klant ontvangt vervolgens de e-mail-uitnodiging van de partner en selecteert de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="ed904-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="ed904-174">De klant meldt zich aan bij Microsoft 365-beheercentrum met behulp van de klantreferenties die u hebt opgegeven.</span><span class="sxs-lookup"><span data-stu-id="ed904-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="ed904-175">De klant controleert het selectievakje om de Microsoft-klantovereenkomst te accepteren.</span><span class="sxs-lookup"><span data-stu-id="ed904-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="ed904-176">Een nieuwe klant uitnodigen om de resellerrelatie en -Microsoft-klantovereenkomst</span><span class="sxs-lookup"><span data-stu-id="ed904-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="ed904-177">Gebruik de volgende stappen om een nieuwe klant uit te nodigen om de resellerrelatie en de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="ed904-178">Selecteer op **het** tabblad Klanten Partner Center koppeling **Een resellerrelatie aanvragen.**</span><span class="sxs-lookup"><span data-stu-id="ed904-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="ed904-179">Er wordt een automatische e-mailsjabloon gegenereerd, inclusief tekst en een geparameteriseerde URL die de klant naar het Microsoft 365 leidt.</span><span class="sxs-lookup"><span data-stu-id="ed904-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="ed904-180">U kunt de automatisch gegenereerde e-mailsjabloon aanpassen en vervolgens **Kopiëren naar klembord of** Openen in **e-mail selecteren.**</span><span class="sxs-lookup"><span data-stu-id="ed904-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="ed904-181">Gebruik deze e-mailsjabloon om de klant uit te nodigen om de **aanvraag voor een resellerrelatie** en **de** Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="ed904-182">(Opmerking: Zorg ervoor dat de partner in de e-mailnodiging ook de URL bevat die automatisch is opgegeven, evenals de klantreferenties die onlangs zijn gemaakt.)</span><span class="sxs-lookup"><span data-stu-id="ed904-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="een relatie maken":::

5. <span data-ttu-id="ed904-184">De klant ontvangt een uitnodiging via e-mail en klikt op de geparameteriseerde URL.</span><span class="sxs-lookup"><span data-stu-id="ed904-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="ed904-185">De klant gebruikt de referenties die u in het e-mailbericht hebt verstrekt om zich aan te melden bij Microsoft 365-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="ed904-186">De klant controleert het selectievakje om de **resellerrelatie te** accepteren en **Microsoft-klantovereenkomst**.</span><span class="sxs-lookup"><span data-stu-id="ed904-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="ed904-187">Binnen dezelfde URL kan de klant een geconsolideerde lijst zien van de verschillende partners met wie ze werken.</span><span class="sxs-lookup"><span data-stu-id="ed904-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="ed904-188">Ze kunnen een partner selecteren om details te bekijken.</span><span class="sxs-lookup"><span data-stu-id="ed904-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Overeenkomst accepteren":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="ed904-190">Een bestaande klant uitnodigen om de overeenkomst te beoordelen en te accepteren</span><span class="sxs-lookup"><span data-stu-id="ed904-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="ed904-191">Gebruik de volgende stappen om een bestaande klant uit te nodigen om de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="ed904-192">Maak het e-mailadres van de klant met de ingesloten URL waarin u uw klant uitnodigt om de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="ed904-193">Uw klant ontvangt de uitnodiging via e-mail en klikt op de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="ed904-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="ed904-194">De klant voert zijn of haar referenties in Microsoft 365-beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="ed904-195">Uw klant controleert het selectievakje om de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="ed904-196">Binnen dezelfde URL kan de klant de geconsolideerde lijst zien van de verschillende partners met wie ze werken.</span><span class="sxs-lookup"><span data-stu-id="ed904-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="ed904-197">Ze kunnen een partner selecteren om details te bekijken.</span><span class="sxs-lookup"><span data-stu-id="ed904-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Klant":::

>[!NOTE]
><span data-ttu-id="ed904-199">In bepaalde scenario's kunnen klanten de Microsoft-klantovereenkomst.</span><span class="sxs-lookup"><span data-stu-id="ed904-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="ed904-200">Lees hieronder Twee scenario's waarin u namens uw klant moet bevestigen voor meer informatie over deze situaties.</span><span class="sxs-lookup"><span data-stu-id="ed904-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="ed904-201">Twee scenario's waarbij u namens uw klant moet bevestigen</span><span class="sxs-lookup"><span data-stu-id="ed904-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="ed904-202">Er zijn twee scenario's waarin klanten de Microsoft-klantovereenkomst mogelijk niet rechtstreeks kunnen Microsoft 365 het beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ed904-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="ed904-203">**Scenario 1:** Een bestaande klant heeft een van de volgende aankopen gedaan via een bestaande partnerrelatie: aanbiedingen, software- of softwareabonnementen, gereserveerde instanties of Azure-plan.</span><span class="sxs-lookup"><span data-stu-id="ed904-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="ed904-204">De klant probeert nu een nieuwe aankoop te doen (met uitzondering van automatische verlenging).</span><span class="sxs-lookup"><span data-stu-id="ed904-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="ed904-205">Wanneer die klant op de URL klikt, ontvangt deze het bericht 'Neem contact op met uw partner om te bevestigen dat u de Microsoft-klantovereenkomst.'</span><span class="sxs-lookup"><span data-stu-id="ed904-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="ed904-206">**Oplossen:** u moet namens de klant bevestigen.</span><span class="sxs-lookup"><span data-stu-id="ed904-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Schermopname van Microsoft 365 de pagina Beheercentrum waarin u wordt gevraagd contact op te nemen met uw partner om de acceptatie van de Microsoft-klantovereenkomst.":::

<span data-ttu-id="ed904-208">**Scenario 2:** Een bestaande klant heeft een van de volgende aanbiedingen, software- en softwareabonnementen, gereserveerde instanties en Azure Plan aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="ed904-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="ed904-209">De klant probeert nu een nieuwe aankoop te doen met een nieuwe partner.</span><span class="sxs-lookup"><span data-stu-id="ed904-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="ed904-210">Wanneer de klant op de URL naar het Microsoft 365-beheercentrum klikt om de nieuwe partnerrelatie en de overeenkomst te accepteren, ontvangt deze het bericht 'Neem contact op met uw partner om te bevestigen dat u de Microsoft-klantovereenkomst.'</span><span class="sxs-lookup"><span data-stu-id="ed904-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="ed904-211">**Oplossen:** u moet namens de klant bevestigen.</span><span class="sxs-lookup"><span data-stu-id="ed904-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="ed904-212">Bevestigen dat een klant de overeenkomst heeft geaccepteerd</span><span class="sxs-lookup"><span data-stu-id="ed904-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="ed904-213">Als u probeert een nieuwe order te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te voltooien.</span><span class="sxs-lookup"><span data-stu-id="ed904-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="ed904-214">Gebruik de volgende procedure om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="ed904-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="ed904-215">Voer de **voornaam**, **achternaam, het** **e-mailadres** en **het** telefoonnummer (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="ed904-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="ed904-216">Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="ed904-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="ed904-217">U kunt dit niet instellen op een toekomstige datum.</span><span class="sxs-lookup"><span data-stu-id="ed904-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="ed904-218">Selecteer **Opslaan en doorgaan**.</span><span class="sxs-lookup"><span data-stu-id="ed904-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="ed904-219">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="ed904-219">Next steps</span></span>

- [<span data-ttu-id="ed904-220">Uw bedrijfsprofielgegevens controleren of bijwerken</span><span class="sxs-lookup"><span data-stu-id="ed904-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="ed904-221">Microsoft-klantovereenkomsten (op regio, taal)</span><span class="sxs-lookup"><span data-stu-id="ed904-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
