---
title: Een Azure-abonnement onder een Azure-plan overdragen aan een andere CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van Cloud Solution Provider programmapartner die is gekoppeld aan de Azure-abonnementen van een klant onder een Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 12afa751d2e7cb6b6ef0cd7308f09746a8a43b52
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284499"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="9da5e-103">De Azure-abonnementsabonnementen van een klant overdragen aan een andere partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="9da5e-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="9da5e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9da5e-105">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="9da5e-105">Account admin</span></span>
- <span data-ttu-id="9da5e-106">Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="9da5e-106">Sales agent</span></span>
- <span data-ttu-id="9da5e-107">Factureringsagent</span><span class="sxs-lookup"><span data-stu-id="9da5e-107">Billing agent</span></span>

<span data-ttu-id="9da5e-108">In dit artikel wordt beschreven hoe een klant zijn Azure-abonnementen onder een Azure-plan van de ene Cloud Solution Provider (CSP) naar een andere kan overstappen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-108">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="9da5e-109">Volg deze stappen om de Azure-abonnementen van een klant van een andere partner over te schakelen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-109">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="9da5e-110">Zowel de partner als de klant moeten de stappen voltooien.</span><span class="sxs-lookup"><span data-stu-id="9da5e-110">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="9da5e-111">Alleen partners met een directe factureringsrelatie met Microsoft hebben toegang tot de overgangshulpprogramma's.</span><span class="sxs-lookup"><span data-stu-id="9da5e-111">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="9da5e-112">Indirecte resellers moeten samenwerken met hun indirecte providers om gebruik te kunnen maken van dit overgangshulpprogramma.</span><span class="sxs-lookup"><span data-stu-id="9da5e-112">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="9da5e-113">De klant moet in gesprek zijn met beide partners (huidige en toekomstige) voordat dit hulpprogramma wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="9da5e-113">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="9da5e-114">Er moet een offline gesprek worden gehad om verwarring en verloop te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-114">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="9da5e-115">Daarnaast moeten partners en klanten deze overwegingen en vereisten begrijpen voordat ze een overgang starten:</span><span class="sxs-lookup"><span data-stu-id="9da5e-115">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="9da5e-116">**Belangrijke overwegingen:**</span><span class="sxs-lookup"><span data-stu-id="9da5e-116">**Key considerations:**</span></span>

- <span data-ttu-id="9da5e-117">Azure-reserveringen worden niet verplaatst met het abonnement naar een toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-117">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="9da5e-118">CSP-prijzen voor Azure-services onder de huidige partner zullen niet overstappen</span><span class="sxs-lookup"><span data-stu-id="9da5e-118">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="9da5e-119">Ondersteuningsverantwoordelijkheden voor klant worden verplaatst naar toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-119">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="9da5e-120">Facturering en facturering worden op het moment van overdracht verplaatst naar een toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-120">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="9da5e-121">Azure Role-Based Access Control (RBAC) wordt niet beïnvloed door de overdracht</span><span class="sxs-lookup"><span data-stu-id="9da5e-121">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="9da5e-122">Beheerder namens (AOBO) wordt niet standaard verleend aan de toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-122">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="9da5e-123">Marketplace-producten van derden worden overdragen zolang de producten voldoen aan de geschiktheidscontrole van Marketplace.</span><span class="sxs-lookup"><span data-stu-id="9da5e-123">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="9da5e-124">Er zijn geen speciale kortingen of regionale beperkingen</span><span class="sxs-lookup"><span data-stu-id="9da5e-124">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="9da5e-125">De producten zijn niet gebaseerd op een abonnement</span><span class="sxs-lookup"><span data-stu-id="9da5e-125">The products are non-subscription based</span></span>
    - <span data-ttu-id="9da5e-126">De toekomstige partner moet samenwerken met de uitgever om ervoor te zorgen dat deze op de toegestane lijst voor implementatie van het product staat</span><span class="sxs-lookup"><span data-stu-id="9da5e-126">The future partner should work with the publisher to make sure they are on the allowlist for deployment of the product</span></span>
    - <span data-ttu-id="9da5e-127">Als niet aan al deze voorwaarden wordt voldaan om de Marketplace-producten over te dragen, moeten de Azure-abonnementen worden geannuleerd en vervolgens opnieuw worden gekocht van Marketplace-producten met de nieuwe partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-127">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="9da5e-128">**Vereisten:**</span><span class="sxs-lookup"><span data-stu-id="9da5e-128">**Prerequisites:**</span></span>

- <span data-ttu-id="9da5e-129">Klant betrek huidige CSP-partner bij de intentie om over te zetten</span><span class="sxs-lookup"><span data-stu-id="9da5e-129">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="9da5e-130">Toekomstige CSP-partner werkt samen met de klant om ervoor te zorgen dat aan de behoeften van de klant kan worden voldaan</span><span class="sxs-lookup"><span data-stu-id="9da5e-130">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="9da5e-131">Toekomstige CSP-partner brengt een relatie tot leven met de klant en koopt een Azure-plan voordat de overgang begint</span><span class="sxs-lookup"><span data-stu-id="9da5e-131">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="9da5e-132">De klant moet een Microsoft-klantovereenkomst met een toekomstige CSP-partner</span><span class="sxs-lookup"><span data-stu-id="9da5e-132">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="9da5e-133">Toekomstige CSP-partner moet de Microsoft Partner-overeenkomst hebben ondertekend om dit hulpprogramma te kunnen gebruiken</span><span class="sxs-lookup"><span data-stu-id="9da5e-133">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="9da5e-134">Te voltooien klanttaken</span><span class="sxs-lookup"><span data-stu-id="9da5e-134">Customer tasks to be completed</span></span>

<span data-ttu-id="9da5e-135">Als u een Azure-abonnement wilt overdragen onder een Azure-plan, moet de klant het proces starten door contact op te nemen met de huidige partner.</span><span class="sxs-lookup"><span data-stu-id="9da5e-135">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="9da5e-136">Ze moeten de bedrijfsnaam en het domein van hun huidige partner verzamelen, zodat hun toekomstige partner het formulier voor overdrachtsaanvraag namens hen kan invullen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-136">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="9da5e-137">De klant moet ook de abonnementen identificeren die hij wil overdragen van zijn huidige partner.</span><span class="sxs-lookup"><span data-stu-id="9da5e-137">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="9da5e-138">U kunt geen partners wijzigen voor abonnementen op Office 365, Enterprise Mobility Suite of Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="9da5e-138">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="9da5e-139">Het is de verantwoordelijkheid van de toekomstige partner om het overdrachtsaanvraagformulier in te vullen dat het overdrachtsproces initieert.</span><span class="sxs-lookup"><span data-stu-id="9da5e-139">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="9da5e-140">Microsoft kan niet ingrijpen namens de klant of de huidige partner.</span><span class="sxs-lookup"><span data-stu-id="9da5e-140">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="9da5e-141">De klant moet van plan zijn nauw samen te werken met zijn toekomstige en huidige partner om de overgang soepel te laten verlopen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-141">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="9da5e-142">Toekomstige partnertaken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="9da5e-142">Future partner tasks to be completed</span></span>

<span data-ttu-id="9da5e-143">De toekomstige partner van het abonnement moet een overdrachtsaanvraagformulier invullen van Partner Center om een abonnementsoverdracht aan te vragen:</span><span class="sxs-lookup"><span data-stu-id="9da5e-143">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="9da5e-144">Selecteer in Partner Center menu Klanten **en** selecteer vervolgens de klant die u namens een overdrachtsaanvraagformulier wilt invullen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-144">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="9da5e-145">Selecteer abonnementen in het menu **Klant.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-145">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="9da5e-146">Selecteer de **sectie Overdrachtsaanvraag.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-146">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="9da5e-147">Selecteer in **de sectie Overdrachtsaanvraag** **de optie Nieuwe aanvraag toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-147">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sectie Overdrachten":::

5.  <span data-ttu-id="9da5e-149">Vul het **formulier Nieuwe overdrachtsaanvraag** in.</span><span class="sxs-lookup"><span data-stu-id="9da5e-149">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="9da5e-150">Selecteer **Overdrachtsaanvraag verzenden**  >  **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-150">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulier voor overdrachtsaanvraag voltooien":::

7.  <span data-ttu-id="9da5e-152">Bevestiging van overdrachtsaanvraag controleren</span><span class="sxs-lookup"><span data-stu-id="9da5e-152">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Overdracht in behandeling controleren":::

    >[!Note]
    ><span data-ttu-id="9da5e-154">De toekomstige partner kan de overdrachtsaanvraag annuleren door **aanvraag** annuleren alleen in de rechterbovenhoek te selecteren wanneer de status van de overdrachtsaanvraag 'in behandeling' is.</span><span class="sxs-lookup"><span data-stu-id="9da5e-154">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="9da5e-155">Zodra de status van de overdrachtsaanvraag 'wordt uitgevoerd' of 'voltooid' is, zijn annuleringen niet meer mogelijk.</span><span class="sxs-lookup"><span data-stu-id="9da5e-155">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="9da5e-156">Huidige partnertaken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="9da5e-156">Current partner tasks to be completed</span></span>

<span data-ttu-id="9da5e-157">De beheerderagent van de huidige partner van de klant ontvangt een e-mailbericht dat de klant een overdracht van zijn of haar abonnementen aanvraagt:</span><span class="sxs-lookup"><span data-stu-id="9da5e-157">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Beoordelen":::

<span data-ttu-id="9da5e-159">Controleer en accepteer het overdrachtsaanvraagformulier van Partner Center om de abonnementsoverdracht te voltooien.</span><span class="sxs-lookup"><span data-stu-id="9da5e-159">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="9da5e-160">Als de huidige partner binnen 30 dagen geen actie onderneemt, verloopt de aanvraag en heeft de toekomstige partner een om een nieuwe overdrachtsaanvraag te maken.</span><span class="sxs-lookup"><span data-stu-id="9da5e-160">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="9da5e-161">Selecteer **Overdrachtsaanvraag controleren in** de e-mail OF</span><span class="sxs-lookup"><span data-stu-id="9da5e-161">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="9da5e-162">Selecteer in Partner Center menu Klanten **en** selecteer vervolgens de klant namens welke een overdrachtsaanvraag is ingediend.</span><span class="sxs-lookup"><span data-stu-id="9da5e-162">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="9da5e-163">Selecteer abonnementen in het menu **Klant.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-163">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="9da5e-164">Selecteer de **sectie Overdrachtsaanvraag.**</span><span class="sxs-lookup"><span data-stu-id="9da5e-164">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="9da5e-165">Vouw overdrachtsgegevens uit door de gekozen **aanvraag-id voor overdracht te selecteren** onder Ontvangen **aanvragen**</span><span class="sxs-lookup"><span data-stu-id="9da5e-165">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Overdrachtsaanvraag voor bronbeoordelingen":::

5.  <span data-ttu-id="9da5e-167">Controleer de overdrachtsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="9da5e-167">Review transfer request.</span></span> <span data-ttu-id="9da5e-168">Selecteer de aangevraagde Azure-abonnementen die u wilt overdragen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-168">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="9da5e-169">Voordat u doorgaat, hebt u geen toegang meer tot de geselecteerde abonnementen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-169">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="9da5e-170">U wordt niet gefactureerd voor verder gebruik.</span><span class="sxs-lookup"><span data-stu-id="9da5e-170">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="9da5e-171">Azure-reserveringen worden niet overdraagt met de abonnementen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-171">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="9da5e-172">Selecteer vervolgens **Accepteren en overdragen om** het overdrachtsproces te voltooien.</span><span class="sxs-lookup"><span data-stu-id="9da5e-172">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Abonnementen selecteren die moeten worden overgedragen onder uw Azure-abonnementen":::

7.  <span data-ttu-id="9da5e-174">Bevestiging van acceptatie van overdracht weergeven.</span><span class="sxs-lookup"><span data-stu-id="9da5e-174">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="9da5e-175">Op dit moment worden de toekomstige partner, de klant en de huidige partner via e-mail op de hoogte gesteld van de geaccepteerde overdrachtsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="9da5e-175">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="9da5e-176">Nadat de overgang is geaccepteerd, kan de overdrachtsstatus maximaal 15 minuten in behandeling blijven terwijl het systeem wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="9da5e-176">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="9da5e-177">Als het langer duurt, blijft het systeem het drie dagen proberen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-177">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="9da5e-178">Als de overdrachtsstatus nog steeds In behandeling is, moet de partner een serviceaanvraag indienen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-178">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="9da5e-179">Zodra de overdracht is voltooid, worden de abonnementen die in de aanvraag zijn opgenomen, weergegeven in het Azure-plan van de toekomstige partner en worden ze niet meer bij u vermeld.</span><span class="sxs-lookup"><span data-stu-id="9da5e-179">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="9da5e-180">Voor indirecte providers: informeer uw indirecte reseller dat de overdrachtsaanvraag is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="9da5e-180">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="9da5e-181">Uw overgedragen klantabonnementen beheren</span><span class="sxs-lookup"><span data-stu-id="9da5e-181">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="9da5e-182">Toegang voor bestaande gebruikers, groepen of service-principals die is toegewezen met behulp van Azure RBAC (op rollen gebaseerd toegangsbeheer) wordt niet beïnvloed tijdens de overgang.</span><span class="sxs-lookup"><span data-stu-id="9da5e-182">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="9da5e-183">Op rollen gebaseerd toegangsbeheer [van Azure (Azure RBAC)](/azure/role-based-access-control/overview) helpt uw klant bij het beheren van wie toegang heeft tot Azure-resources, wat ze kunnen doen met deze resources en tot welke gebieden ze toegang hebben.</span><span class="sxs-lookup"><span data-stu-id="9da5e-183">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="9da5e-184">Als nieuwe partner krijgt u na de abonnementsoverdracht geen RBAC-toegang tot de resources van uw klant.</span><span class="sxs-lookup"><span data-stu-id="9da5e-184">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="9da5e-185">De vorige partner van uw klant behoudt zijn RBAC-toegang.</span><span class="sxs-lookup"><span data-stu-id="9da5e-185">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="9da5e-186">Werk samen met uw klant om te begrijpen wie inzicht heeft in hun abonnementen en hoe u gezochte wijzigingen kunt aanbrengen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-186">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="9da5e-187">Daarom is het belangrijk dat uw klant Azure RBAC-toegang voor de vorige partner verwijdert en toegang toevoegt voor de nieuwe partner.</span><span class="sxs-lookup"><span data-stu-id="9da5e-187">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="9da5e-188">Zie Wat is op rollen gebaseerd toegangsbeheer van [Azure (Azure RBAC)?](/azure/role-based-access-control/overview) voor meer informatie over het verlenen van nieuwe toegang door uw klant.</span><span class="sxs-lookup"><span data-stu-id="9da5e-188">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="9da5e-189">Zie Een roltoewijzing [verwijderen](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)voor meer informatie over het verwijderen van de RBAC-toegang van uw vorige partner.</span><span class="sxs-lookup"><span data-stu-id="9da5e-189">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="9da5e-190">Bovendien krijgt u niet automatisch beheerderstoegang [namens (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) tot uw abonnementen.</span><span class="sxs-lookup"><span data-stu-id="9da5e-190">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="9da5e-191">AOBO is nodig voor partners om de Azure-abonnementen van hun klant namens hen te beheren.</span><span class="sxs-lookup"><span data-stu-id="9da5e-191">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="9da5e-192">Zie Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant voor meer informatie over [Azure-bevoegdheden.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="9da5e-192">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="9da5e-193">Volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="9da5e-193">Next steps:</span></span>

- [<span data-ttu-id="9da5e-194">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="9da5e-194">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="9da5e-195">Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant.</span><span class="sxs-lookup"><span data-stu-id="9da5e-195">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
