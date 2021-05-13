---
title: Een Azure-abonnement onder een Azure-plan overdragen naar een andere CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van de Cloud Solution Provider programmapartner die is gekoppeld aan de Azure-abonnementen van een klant onder een Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856046"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="172d9-103">De Azure-abonnementsabonnementen van een klant overdragen aan een andere partner</span><span class="sxs-lookup"><span data-stu-id="172d9-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="172d9-104">**Juiste rollen:** Accountbeheerder | Verkoopagent | Factureringsagent</span><span class="sxs-lookup"><span data-stu-id="172d9-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="172d9-105">In dit artikel wordt beschreven hoe een klant zijn Azure-abonnementen onder een Azure-plan van de ene Cloud Solution Provider (CSP) naar een andere kan overstappen.</span><span class="sxs-lookup"><span data-stu-id="172d9-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="172d9-106">Volg deze stappen om de Azure-abonnementen van een klant over te schakelen van een andere partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="172d9-107">Zowel de partner als de klant moeten de stappen voltooien.</span><span class="sxs-lookup"><span data-stu-id="172d9-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="172d9-108">Alleen partners met een directe factureringsrelatie met Microsoft hebben toegang tot de overgangshulpprogramma's.</span><span class="sxs-lookup"><span data-stu-id="172d9-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="172d9-109">Indirecte resellers moeten samenwerken met hun indirecte providers om gebruik te kunnen maken van dit overgangshulpprogramma.</span><span class="sxs-lookup"><span data-stu-id="172d9-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="172d9-110">De klant moet in gesprek zijn met beide partners (huidige en toekomstige) voordat dit hulpprogramma wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="172d9-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="172d9-111">Er moet een offline gesprek worden gehad om verwarring en verloop te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="172d9-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="172d9-112">Daarnaast moeten partners en klanten deze overwegingen en vereisten begrijpen voordat ze een overgang starten:</span><span class="sxs-lookup"><span data-stu-id="172d9-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="172d9-113">**Belangrijke overwegingen:**</span><span class="sxs-lookup"><span data-stu-id="172d9-113">**Key considerations:**</span></span>

- <span data-ttu-id="172d9-114">Azure-reserveringen worden niet verplaatst met het abonnement naar een toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="172d9-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="172d9-115">CSP-prijzen voor Azure-services onder de huidige partner gaan niet over</span><span class="sxs-lookup"><span data-stu-id="172d9-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="172d9-116">Ondersteuningsverantwoordelijkheden voor klant worden verplaatst naar toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="172d9-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="172d9-117">Facturering en facturering worden verplaatst naar een toekomstige partner op het moment van overdracht</span><span class="sxs-lookup"><span data-stu-id="172d9-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="172d9-118">Azure Role-Based Access Control (RBAC) wordt niet beïnvloed door de overdracht</span><span class="sxs-lookup"><span data-stu-id="172d9-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="172d9-119">Beheerder namens (AOBO) wordt niet standaard verleend aan de toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="172d9-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="172d9-120">Marketplace-producten van derden worden overdragen zolang de producten voldoen aan de geschiktheidscontrole van Marketplace.</span><span class="sxs-lookup"><span data-stu-id="172d9-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="172d9-121">Er zijn geen speciale kortingen of regionale beperkingen</span><span class="sxs-lookup"><span data-stu-id="172d9-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="172d9-122">De producten zijn niet gebaseerd op een abonnement</span><span class="sxs-lookup"><span data-stu-id="172d9-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="172d9-123">De toekomstige partner moet samenwerken met de uitgever om ervoor te zorgen dat deze op de lijst met toegestane producten staat voor de implementatie van het product</span><span class="sxs-lookup"><span data-stu-id="172d9-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="172d9-124">Als niet aan al deze voorwaarden wordt voldaan om de Marketplace-producten over te dragen, moeten ze worden geannuleerd, de Azure-abonnementen worden overgedragen en vervolgens opnieuw worden gekocht van Marketplace-producten met de nieuwe partner</span><span class="sxs-lookup"><span data-stu-id="172d9-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="172d9-125">**Vereisten:**</span><span class="sxs-lookup"><span data-stu-id="172d9-125">**Prerequisites:**</span></span>

- <span data-ttu-id="172d9-126">Klant gaat in contact met huidige CSP-partner over hun intentie tot overgang</span><span class="sxs-lookup"><span data-stu-id="172d9-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="172d9-127">Toekomstige CSP-partner werkt samen met de klant om ervoor te zorgen dat aan de behoeften van de klant kan worden voldaan</span><span class="sxs-lookup"><span data-stu-id="172d9-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="172d9-128">Toekomstige CSP-partner brengt een relatie tot leven met de klant en koopt een Azure-plan voordat de overgang begint</span><span class="sxs-lookup"><span data-stu-id="172d9-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="172d9-129">De klant moet zich Microsoft-klantovereenkomst toekomstige CSP-partner aanmelden</span><span class="sxs-lookup"><span data-stu-id="172d9-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="172d9-130">Toekomstige CSP-partner moet de Microsoft Partner-overeenkomst hebben ondertekend om dit hulpprogramma te kunnen gebruiken</span><span class="sxs-lookup"><span data-stu-id="172d9-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="172d9-131">Te voltooien klanttaken</span><span class="sxs-lookup"><span data-stu-id="172d9-131">Customer tasks to be completed</span></span>

<span data-ttu-id="172d9-132">Als u een Azure-abonnement wilt overdragen onder een Azure-plan, moet de klant het proces starten door contact op te nemen met zijn huidige partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="172d9-133">Ze moeten de bedrijfsnaam en het domein van hun huidige partner verzamelen, zodat hun toekomstige partner het formulier voor overdracht namens hen kan invullen.</span><span class="sxs-lookup"><span data-stu-id="172d9-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="172d9-134">De klant moet ook de abonnementen identificeren die hij wil overdragen van zijn huidige partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="172d9-135">U kunt geen partners wijzigen voor abonnementen op Office 365, Enterprise Mobility Suite of Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="172d9-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="172d9-136">Het is de verantwoordelijkheid van de toekomstige partner om het overdrachtsaanvraagformulier in te vullen dat het overdrachtsproces initieert.</span><span class="sxs-lookup"><span data-stu-id="172d9-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="172d9-137">Microsoft kan niet ingrijpen namens de klant of de huidige partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="172d9-138">De klant moet nauw samenwerken met zijn toekomstige en huidige partner om de overgang soepel te laten verlopen.</span><span class="sxs-lookup"><span data-stu-id="172d9-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="172d9-139">Toekomstige partnertaken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="172d9-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="172d9-140">De toekomstige partner van het abonnement moet een overdrachtsaanvraagformulier invullen van Partner Center om een abonnementsoverdracht aan te vragen:</span><span class="sxs-lookup"><span data-stu-id="172d9-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="172d9-141">Selecteer in Partner Center menu Klanten **en** selecteer vervolgens de klant die u namens een overdrachtsaanvraagformulier wilt invullen.</span><span class="sxs-lookup"><span data-stu-id="172d9-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="172d9-142">Selecteer abonnementen in het menu **Klant.**</span><span class="sxs-lookup"><span data-stu-id="172d9-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="172d9-143">Selecteer de **sectie Overdrachtsaanvraag.**</span><span class="sxs-lookup"><span data-stu-id="172d9-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="172d9-144">Selecteer in **de sectie Overdrachtsaanvraag** **de optie Nieuwe aanvraag toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="172d9-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sectie Overdrachten":::

5.  <span data-ttu-id="172d9-146">Vul het **formulier Nieuwe overdrachtsaanvraag** in.</span><span class="sxs-lookup"><span data-stu-id="172d9-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="172d9-147">Selecteer **Overdrachtsaanvraag verzenden**  >  **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="172d9-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulier voor overdrachtsaanvraag voltooien":::

7.  <span data-ttu-id="172d9-149">Bevestiging van overdrachtsaanvraag controleren</span><span class="sxs-lookup"><span data-stu-id="172d9-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Overdracht in behandeling controleren":::

    >[!Note]
    ><span data-ttu-id="172d9-151">De toekomstige partner kan de overdrachtsaanvraag annuleren door **aanvraag** annuleren alleen in de rechterbovenhoek te selecteren wanneer de status van de overdrachtsaanvraag 'in behandeling' is.</span><span class="sxs-lookup"><span data-stu-id="172d9-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="172d9-152">Zodra de status van de overdrachtsaanvraag 'wordt uitgevoerd' of 'voltooid' is, zijn annuleringen niet meer mogelijk.</span><span class="sxs-lookup"><span data-stu-id="172d9-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="172d9-153">Huidige partnertaken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="172d9-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="172d9-154">De beheerderagent van de huidige partner van de klant ontvangt een e-mailbericht dat de klant een overdracht van zijn of haar abonnementen aanvraagt:</span><span class="sxs-lookup"><span data-stu-id="172d9-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Beoordelen":::

<span data-ttu-id="172d9-156">Controleer en accepteer het overdrachtsaanvraagformulier van Partner Center om de abonnementsoverdracht te voltooien.</span><span class="sxs-lookup"><span data-stu-id="172d9-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="172d9-157">Als de huidige partner binnen 30 dagen geen actie onderneemt, verloopt de aanvraag en heeft de toekomstige partner een om een nieuwe overdrachtsaanvraag te maken.</span><span class="sxs-lookup"><span data-stu-id="172d9-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="172d9-158">Selecteer **Overdrachtsaanvraag controleren in** de e-mail OF</span><span class="sxs-lookup"><span data-stu-id="172d9-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="172d9-159">Selecteer in Partner Center menu Klanten **en** selecteer vervolgens de klant namens welke een overdrachtsaanvraag is ingediend.</span><span class="sxs-lookup"><span data-stu-id="172d9-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="172d9-160">Selecteer abonnementen in het menu **Klant.**</span><span class="sxs-lookup"><span data-stu-id="172d9-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="172d9-161">Selecteer de **sectie Overdrachtsaanvraag.**</span><span class="sxs-lookup"><span data-stu-id="172d9-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="172d9-162">Vouw overdrachtsgegevens uit door de gekozen id voor de **overdrachtsaanvraag te selecteren** **onder Ontvangen aanvragen**</span><span class="sxs-lookup"><span data-stu-id="172d9-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Overdrachtsaanvraag voor bronbeoordelingen":::

5.  <span data-ttu-id="172d9-164">Controleer de overdrachtsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="172d9-164">Review transfer request.</span></span> <span data-ttu-id="172d9-165">Selecteer de aangevraagde Azure-abonnementen die u wilt overdragen.</span><span class="sxs-lookup"><span data-stu-id="172d9-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="172d9-166">Voordat u doorgaat, hebt u geen toegang meer tot de geselecteerde abonnementen.</span><span class="sxs-lookup"><span data-stu-id="172d9-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="172d9-167">U wordt niet gefactureerd voor verder gebruik.</span><span class="sxs-lookup"><span data-stu-id="172d9-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="172d9-168">Azure-reserveringen worden niet overdraagt met de abonnementen.</span><span class="sxs-lookup"><span data-stu-id="172d9-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="172d9-169">Selecteer vervolgens **Accepteren en overdragen om** het overdrachtsproces te voltooien.</span><span class="sxs-lookup"><span data-stu-id="172d9-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Abonnementen selecteren die moeten worden overgedragen onder uw Azure-abonnementen":::

7.  <span data-ttu-id="172d9-171">Bevestiging van acceptatie van overdracht weergeven.</span><span class="sxs-lookup"><span data-stu-id="172d9-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="172d9-172">Op dit moment worden de toekomstige partner, de klant en de huidige partner via e-mail op de hoogte gesteld van de geaccepteerde overdrachtsaanvraag.</span><span class="sxs-lookup"><span data-stu-id="172d9-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="172d9-173">Nadat de overgang is geaccepteerd, kan de overdrachtsstatus maximaal 15 minuten in behandeling blijven terwijl het systeem wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="172d9-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="172d9-174">Als het langer duurt, blijft het systeem het drie dagen proberen.</span><span class="sxs-lookup"><span data-stu-id="172d9-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="172d9-175">Als de overdrachtsstatus nog steeds In behandeling is, moet de partner een serviceaanvraag indienen.</span><span class="sxs-lookup"><span data-stu-id="172d9-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="172d9-176">Zodra de overdracht is voltooid, worden de abonnementen die in de aanvraag zijn opgenomen, weergegeven in het Azure-plan van de toekomstige partner en worden ze niet meer bij u vermeld.</span><span class="sxs-lookup"><span data-stu-id="172d9-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="172d9-177">Voor indirecte providers: informeer uw indirecte reseller dat de overdrachtsaanvraag is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="172d9-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="172d9-178">Uw overgedragen klantabonnementen beheren</span><span class="sxs-lookup"><span data-stu-id="172d9-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="172d9-179">Toegang voor bestaande gebruikers, groepen of service-principals die is toegewezen met behulp van Azure RBAC (op rollen gebaseerd toegangsbeheer) wordt niet beïnvloed tijdens de overgang.</span><span class="sxs-lookup"><span data-stu-id="172d9-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="172d9-180">Op rollen gebaseerd toegangsbeheer [van Azure (Azure RBAC)](/azure/role-based-access-control/overview) helpt uw klant bij het beheren van wie toegang heeft tot Azure-resources, wat ze kunnen doen met deze resources en tot welke gebieden ze toegang hebben.</span><span class="sxs-lookup"><span data-stu-id="172d9-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="172d9-181">Als nieuwe partner krijgt u na de abonnementsoverdracht geen RBAC-toegang tot de resources van uw klant.</span><span class="sxs-lookup"><span data-stu-id="172d9-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="172d9-182">De vorige partner van uw klant behoudt zijn RBAC-toegang.</span><span class="sxs-lookup"><span data-stu-id="172d9-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="172d9-183">Werk samen met uw klant om te begrijpen wie inzicht heeft in hun abonnementen en hoe u gezochte wijzigingen kunt aanbrengen.</span><span class="sxs-lookup"><span data-stu-id="172d9-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="172d9-184">Daarom is het belangrijk dat uw klant Azure RBAC-toegang voor de vorige partner verwijdert en toegang toevoegt voor de nieuwe partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="172d9-185">Zie Wat is op rollen gebaseerd toegangsbeheer van [Azure (Azure RBAC)?](/azure/role-based-access-control/overview) voor meer informatie over het verlenen van nieuwe toegang door uw klant.</span><span class="sxs-lookup"><span data-stu-id="172d9-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="172d9-186">Zie Een roltoewijzing [verwijderen](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)voor meer informatie over het verwijderen van de RBAC-toegang van uw vorige partner.</span><span class="sxs-lookup"><span data-stu-id="172d9-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="172d9-187">Bovendien krijgt u niet automatisch beheerderstoegang [namens (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) tot uw abonnementen.</span><span class="sxs-lookup"><span data-stu-id="172d9-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="172d9-188">AOBO is nodig voor partners om de Azure-abonnementen van hun klant namens hen te beheren.</span><span class="sxs-lookup"><span data-stu-id="172d9-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="172d9-189">Zie Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant voor meer informatie over [Azure-bevoegdheden.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="172d9-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="172d9-190">Volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="172d9-190">Next steps:</span></span>

- [<span data-ttu-id="172d9-191">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="172d9-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="172d9-192">Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant.</span><span class="sxs-lookup"><span data-stu-id="172d9-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
