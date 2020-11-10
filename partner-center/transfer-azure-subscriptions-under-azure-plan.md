---
title: Azure-abonnement overdragen onder een Azure-plan naar een andere CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van de partner van het Cloud Solution Provider-programma dat is gekoppeld aan de Azure-abonnementen van een klant onder een Azure-abonnement.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 81f64e117f9e0a4abc817746d11dc9acae887577
ms.sourcegitcommit: 146964ce0cc72bd821692f73f9c0b55e6fefb0fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/10/2020
ms.locfileid: "94433343"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="6741c-103">De Azure-plan abonnementen van een klant overdragen naar een andere partner</span><span class="sxs-lookup"><span data-stu-id="6741c-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="6741c-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="6741c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="6741c-105">Partners in het Cloud Solution Provider-programma (CSP)</span><span class="sxs-lookup"><span data-stu-id="6741c-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="6741c-106">In dit artikel wordt beschreven hoe een klant hun Azure-abonnementen kan veranderen onder een Azure-abonnement van één Cloud Solution Provider (CSP) naar een andere.</span><span class="sxs-lookup"><span data-stu-id="6741c-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="6741c-107">Voer de volgende stappen uit om de Azure-abonnementen van een klant te wisselen van een andere partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="6741c-108">Zowel de partner als de klant heeft stappen om te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="6741c-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="6741c-109">Alleen partners met een directe facturerings relatie met micro soft hebben toegang tot het hulp programma overgang.</span><span class="sxs-lookup"><span data-stu-id="6741c-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="6741c-110">Indirecte wederverkopers moeten samen werken met hun indirecte providers om gebruik te maken van dit overgangs programma.</span><span class="sxs-lookup"><span data-stu-id="6741c-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="6741c-111">De klant moet in gesprek zijn met beide partners (huidige en toekomstige) voordat dit hulp programma wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="6741c-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="6741c-112">Er moet een offline conversatie zijn om Verwar ring en verloop te voor komen.</span><span class="sxs-lookup"><span data-stu-id="6741c-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="6741c-113">Daarnaast moeten partners en klanten op de hoogte zijn van deze overwegingen en vereisten voordat ze een overgang initiëren:</span><span class="sxs-lookup"><span data-stu-id="6741c-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="6741c-114">**Belangrijkste overwegingen:**</span><span class="sxs-lookup"><span data-stu-id="6741c-114">**Key considerations:**</span></span>

- <span data-ttu-id="6741c-115">Azure Reservations wordt niet met het abonnement verplaatst naar een toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="6741c-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="6741c-116">CSP-prijzen voor Azure-Services onder huidige partner worden niet overgezet</span><span class="sxs-lookup"><span data-stu-id="6741c-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="6741c-117">De ondersteunings verantwoordelijkheden voor de klant worden verplaatst naar de volgende partner</span><span class="sxs-lookup"><span data-stu-id="6741c-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="6741c-118">Facturering en facturering worden verplaatst naar de volgende partner op het moment van de overdracht</span><span class="sxs-lookup"><span data-stu-id="6741c-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="6741c-119">Azure Role-Based Access Control (RBAC) is niet van invloed op de overdracht</span><span class="sxs-lookup"><span data-stu-id="6741c-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="6741c-120">Beheerder namens (ADMINISTRATE) wordt niet standaard verleend aan de toekomstige partner</span><span class="sxs-lookup"><span data-stu-id="6741c-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="6741c-121">Marketplace-Producten van derden worden overgezet zolang de producten de controle op Marketplace door voeren.</span><span class="sxs-lookup"><span data-stu-id="6741c-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="6741c-122">Er zijn geen speciale kortingen of regionale beperkingen</span><span class="sxs-lookup"><span data-stu-id="6741c-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="6741c-123">De producten zijn niet gebaseerd op een abonnement</span><span class="sxs-lookup"><span data-stu-id="6741c-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="6741c-124">De volgende partner moet samen werken met de uitgever om er zeker van te zijn dat ze zich op de acceptatie lijst bevinden voor de implementatie van het product</span><span class="sxs-lookup"><span data-stu-id="6741c-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="6741c-125">Als niet aan al deze voor waarden wordt voldaan om de Marketplace-producten te kunnen overdragen, moeten de Azure-abonnementen worden overgezet en vervolgens opnieuw worden gekocht van Marketplace-Producten met de nieuwe partner</span><span class="sxs-lookup"><span data-stu-id="6741c-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="6741c-126">**Vereisten:**</span><span class="sxs-lookup"><span data-stu-id="6741c-126">**Prerequisites:**</span></span>

- <span data-ttu-id="6741c-127">De klant houdt de huidige CSP-partner op hun intentie om over te gaan naar overgang</span><span class="sxs-lookup"><span data-stu-id="6741c-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="6741c-128">Toekomstige CSP-partner werkt samen met de klant om ervoor te zorgen dat aan de behoeften van de klant kan worden voldaan</span><span class="sxs-lookup"><span data-stu-id="6741c-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="6741c-129">Toekomstige CSP-partner brengt een relatie met de klant tot stand voordat de overgang begint</span><span class="sxs-lookup"><span data-stu-id="6741c-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="6741c-130">De klant moet de klant overeenkomst van micro soft ondertekenen met een toekomstige CSP-partner</span><span class="sxs-lookup"><span data-stu-id="6741c-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="6741c-131">Toekomstige CSP-partner moet de micro soft-partner overeenkomst hebben ondertekend om dit hulp programma te gebruiken</span><span class="sxs-lookup"><span data-stu-id="6741c-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="6741c-132">Klant taken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="6741c-132">Customer tasks to be completed</span></span>

<span data-ttu-id="6741c-133">Als u een Azure-abonnement wilt overdragen onder een Azure-plan, moet de klant het proces starten door contact op te nemen met de huidige partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="6741c-134">Ze moeten hun bedrijfs naam en domein van hun huidige partner verzamelen, zodat hun toekomstige partner het aanvraag formulier voor de overdracht kan volt ooien.</span><span class="sxs-lookup"><span data-stu-id="6741c-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="6741c-135">De klant moet ook de abonnementen identificeren die ze willen overdragen vanaf hun huidige partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="6741c-136">U kunt de partners voor Office 365, Enter prise Mobility Suite of micro soft Dynamics CRM-abonnementen niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="6741c-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="6741c-137">Het is de verantwoordelijkheid van de toekomstige partner om het aanvraag formulier voor de overdracht te volt ooien waarmee het overdrachts proces wordt gestart.</span><span class="sxs-lookup"><span data-stu-id="6741c-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="6741c-138">Micro soft kan niet namens de klant of de huidige partner worden gehandeld.</span><span class="sxs-lookup"><span data-stu-id="6741c-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="6741c-139">De klant moet plannen om nauw keurig aan de slag te gaan met hun toekomstige en huidige partner om de overgang soepel te laten verlopen.</span><span class="sxs-lookup"><span data-stu-id="6741c-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="6741c-140">Toekomstige partner taken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="6741c-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="6741c-141">De volgende partner van het abonnement moet een aanvraag formulier voor de overdracht van het partner centrum volt ooien om een abonnements overdracht aan te vragen:</span><span class="sxs-lookup"><span data-stu-id="6741c-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="6741c-142">Selecteer **klanten** in het menu van het partner centrum en selecteer de klant waarvoor u een aanvraag formulier voor de overdracht wilt uitvoeren namens.</span><span class="sxs-lookup"><span data-stu-id="6741c-142">From the Partner Center menu, select **Customers** , then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="6741c-143">Selecteer in het menu klant **abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="6741c-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6741c-144">Selecteer de sectie **overdrachts aanvraag** .</span><span class="sxs-lookup"><span data-stu-id="6741c-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6741c-145">Selecteer in de **sectie overdrachts aanvraag** de optie **nieuwe aanvraag toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="6741c-145">From the **Transfer request section** , select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sectie overdrachten":::

5.  <span data-ttu-id="6741c-147">Vul het formulier voor de **nieuwe overdrachts aanvraag** in.</span><span class="sxs-lookup"><span data-stu-id="6741c-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="6741c-148">Selecteer verzenden **overdracht aanvraag**  >  **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="6741c-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulier voor aanvraag voor overdracht volt ooien":::

7.  <span data-ttu-id="6741c-150">Bevestiging van overdrachts aanvraag controleren</span><span class="sxs-lookup"><span data-stu-id="6741c-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="In behandeling zijnde overdracht bekijken":::

    >[!Note]
    ><span data-ttu-id="6741c-152">De volgende partner kan de overdrachts aanvraag annuleren door **Aanvraag annuleren** te selecteren in de rechter bovenhoek alleen wanneer de status van de overdrachts aanvraag ' in behandeling ' is.</span><span class="sxs-lookup"><span data-stu-id="6741c-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="6741c-153">Wanneer de status van de overdrachts aanvraag ' wordt uitgevoerd ' of ' voltooid ' is, kunnen annuleringen niet worden geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="6741c-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="6741c-154">Huidige partner taken die moeten worden voltooid</span><span class="sxs-lookup"><span data-stu-id="6741c-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="6741c-155">De beheerder agent van de huidige partner van de klant ontvangt een e-mail dat de klant een overdracht van hun abonnementen heeft aangevraagd:</span><span class="sxs-lookup"><span data-stu-id="6741c-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Beoordelen":::

<span data-ttu-id="6741c-157">Bekijk en accepteer het aanvraag formulier voor de overdracht van het partner centrum om de overdracht van het abonnement te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="6741c-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="6741c-158">Als er binnen 30 dagen geen actie wordt ondernomen door de huidige partner, verloopt de aanvraag en zal de volgende partner een nieuwe overdrachts aanvraag maken.</span><span class="sxs-lookup"><span data-stu-id="6741c-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="6741c-159">Selecteer **aanvraag voor overdracht controleren** van de e-mail of</span><span class="sxs-lookup"><span data-stu-id="6741c-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="6741c-160">Selecteer **klanten** in het menu van het partner centrum en selecteer de klant voor wie een aanvraag voor de overdracht is ingediend namens.</span><span class="sxs-lookup"><span data-stu-id="6741c-160">From the Partner Center menu, select **Customers** , then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="6741c-161">Selecteer in het menu klant **abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="6741c-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="6741c-162">Selecteer de sectie **overdrachts aanvraag** .</span><span class="sxs-lookup"><span data-stu-id="6741c-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="6741c-163">Uitbrei ding van overdrachts gegevens door de gekozen **aanvraag-id** voor de overdracht te selecteren onder **ontvangen aanvragen**</span><span class="sxs-lookup"><span data-stu-id="6741c-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Overdrachts aanvraag bron controles":::

5.  <span data-ttu-id="6741c-165">Overdrachts aanvraag controleren.</span><span class="sxs-lookup"><span data-stu-id="6741c-165">Review transfer request.</span></span> <span data-ttu-id="6741c-166">Selecteer de aangevraagde Azure-abonnementen om over te dragen.</span><span class="sxs-lookup"><span data-stu-id="6741c-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="6741c-167">Opmerking: u hebt geen toegang meer tot de geselecteerde abonnementen voordat u doorgaat.</span><span class="sxs-lookup"><span data-stu-id="6741c-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="6741c-168">U wordt niet gefactureerd voor verder gebruik.</span><span class="sxs-lookup"><span data-stu-id="6741c-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="6741c-169">Azure-reserve ringen worden niet overgedragen met de abonnementen.</span><span class="sxs-lookup"><span data-stu-id="6741c-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="6741c-170">Selecteer vervolgens **accepteren en overdragen** om het overdrachts proces te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="6741c-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Abonnementen selecteren die moeten worden overgedragen onder uw Azure-abonnementen":::

7.  <span data-ttu-id="6741c-172">Bevestiging van acceptatie van overdracht weer geven.</span><span class="sxs-lookup"><span data-stu-id="6741c-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="6741c-173">Op dit moment wordt de volgende partner, de klant en de huidige partner op de hoogte gesteld van de geaccepteerde overdrachts aanvraag via e-mail.</span><span class="sxs-lookup"><span data-stu-id="6741c-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="6741c-174">Nadat de overgang is geaccepteerd, kan de overdrachts status Maxi maal 15 minuten in behandeling blijven terwijl het systeem wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="6741c-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="6741c-175">Als het langer duurt, blijft het systeem drie dagen proberen.</span><span class="sxs-lookup"><span data-stu-id="6741c-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="6741c-176">Als de overdrachts status nog steeds in behandeling blijft, moet de partner een service aanvraag indienen.</span><span class="sxs-lookup"><span data-stu-id="6741c-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="6741c-177">Zodra de overdracht is voltooid, worden de abonnementen die zijn opgenomen in de aanvraag, weer gegeven in het Azure-abonnement van de toekomstige partner en worden ze niet meer met u vermeld.</span><span class="sxs-lookup"><span data-stu-id="6741c-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="6741c-178">Voor indirecte providers: Informeer uw indirecte wederverkoper dat de overdrachts aanvraag is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="6741c-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="6741c-179">Uw overgedragen klant abonnementen beheren</span><span class="sxs-lookup"><span data-stu-id="6741c-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="6741c-180">Toegang voor bestaande gebruikers, groepen of service-principals die is toegewezen met behulp van Azure RBAC (op rollen gebaseerd toegangsbeheer) wordt niet beïnvloed tijdens de overgang.</span><span class="sxs-lookup"><span data-stu-id="6741c-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="6741c-181">Met Azure [RBAC (](/azure/role-based-access-control/overview) op rollen gebaseerd toegangs beheer) kan uw klant beheren wie toegang heeft tot Azure-resources, wat ze kunnen doen met deze resources en op welke gebieden ze toegang hebben.</span><span class="sxs-lookup"><span data-stu-id="6741c-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="6741c-182">Als de nieuwe partner hebt u geen RBAC-toegang tot de resources van uw klant na de overdracht van het abonnement.</span><span class="sxs-lookup"><span data-stu-id="6741c-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="6741c-183">De vorige partner van uw klant behoudt de RBAC-toegang.</span><span class="sxs-lookup"><span data-stu-id="6741c-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="6741c-184">Werk samen met uw klant om te begrijpen wie inzicht heeft in hun abonnementen en hoe u de gewenste wijzigingen kunt aanbrengen.</span><span class="sxs-lookup"><span data-stu-id="6741c-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="6741c-185">Het is dus belang rijk dat uw klant de Azure RBAC-toegang voor hun vorige partner verwijdert en dat er toegang wordt toegevoegd voor de nieuwe partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="6741c-186">Zie [Wat is Azure Role-based Access Control (Azure RBAC)?](/azure/role-based-access-control/overview) voor meer informatie over de klant die nieuwe toegang geeft.</span><span class="sxs-lookup"><span data-stu-id="6741c-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="6741c-187">Zie [een roltoewijzing verwijderen](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)voor meer informatie over uw klant bij het verwijderen van de RBAC-toegang van uw vorige partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="6741c-188">Daarnaast krijgt u niet automatisch een [beheerder namens (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) toegang tot uw abonnementen.</span><span class="sxs-lookup"><span data-stu-id="6741c-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="6741c-189">ADMINISTRATE is nodig voor het beheren van de Azure-abonnementen van hun klanten namens de partner.</span><span class="sxs-lookup"><span data-stu-id="6741c-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="6741c-190">Zie [machtigingen voor het beheren van de service of het abonnement van een klant verkrijgen](./customers-revoke-admin-privileges.md) voor meer informatie over de bevoegdheden van Azure.</span><span class="sxs-lookup"><span data-stu-id="6741c-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="6741c-191">Volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="6741c-191">Next steps:</span></span>

- [<span data-ttu-id="6741c-192">(Azure RBAC)</span><span class="sxs-lookup"><span data-stu-id="6741c-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="6741c-193">Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant.</span><span class="sxs-lookup"><span data-stu-id="6741c-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
