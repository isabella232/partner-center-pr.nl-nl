---
title: Gekwalificeerde Dynamics 365-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Leer hoe u migreert van gekwalificeerde, eenvoudige Dynamics 365-abonnementen naar een nieuw abonnement voordat bestaande abonnementen verlopen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151641"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="25c3f-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Abonnement van Dynamics 365 en Customer Engagement (gekwalificeerde aanbiedingen) migreren van Basic naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="25c3f-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="25c3f-104">**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="25c3f-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="25c3f-105">Vanaf 1 januari 2019 kunnen klanten met een Dynamics 365 for Sales-/Customer Engagement-abonnement van Basic-abonnementen (gekwalificeerde aanbiedingen) deze verouderde aanbiedingen niet meer vernieuwen; bestaande abonnementen worden niet automatisch verlengd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="25c3f-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="25c3f-106">Op de detailpagina van het abonnement wordt de status van het abonnement gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'.</span><span class="sxs-lookup"><span data-stu-id="25c3f-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="25c3f-107">Om de continuïteit voor klanten te waarborgen, moet u de klanten met verlopen abonnementen overstappen naar een ondersteunde optie, die hieronder wordt vermeld.</span><span class="sxs-lookup"><span data-stu-id="25c3f-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="25c3f-108">Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="25c3f-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="25c3f-109">Als u de API (ZOWEL VOOR als Partner Center) gebruikt, kunt u verlopende abonnementen vinden door de einddatum van het abonnement te evalueren, samen met de eigenschap auto renew = False.</span><span class="sxs-lookup"><span data-stu-id="25c3f-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="25c3f-110">De abonnementen in kwestie worden op 1 januari 2019 ingesteld op automatisch verlengen=Onwaar.</span><span class="sxs-lookup"><span data-stu-id="25c3f-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="25c3f-111">U kunt klanten op elk moment naar een nieuw plan verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="25c3f-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="25c3f-112">De Dynamics 365-aanbiedingen worden niet meer gebruikt</span><span class="sxs-lookup"><span data-stu-id="25c3f-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="25c3f-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="25c3f-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers</span><span class="sxs-lookup"><span data-stu-id="25c3f-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="25c3f-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="25c3f-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="25c3f-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="25c3f-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="25c3f-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="25c3f-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers</span><span class="sxs-lookup"><span data-stu-id="25c3f-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="25c3f-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="25c3f-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="25c3f-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="25c3f-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers</span><span class="sxs-lookup"><span data-stu-id="25c3f-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="25c3f-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="25c3f-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="25c3f-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="25c3f-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span><span class="sxs-lookup"><span data-stu-id="25c3f-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span><span class="sxs-lookup"><span data-stu-id="25c3f-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="25c3f-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span><span class="sxs-lookup"><span data-stu-id="25c3f-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="25c3f-137">Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span><span class="sxs-lookup"><span data-stu-id="25c3f-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="25c3f-138">**Gestopte aanbiedingen**</span><span class="sxs-lookup"><span data-stu-id="25c3f-138">**Retired offers**</span></span>   

- <span data-ttu-id="25c3f-139">Dynamics 365 for Sales van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="25c3f-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="25c3f-140">Dynamics 365 Customer Engagement Plan van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="25c3f-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="25c3f-141">**Vervangingsopties**</span><span class="sxs-lookup"><span data-stu-id="25c3f-141">**Replacement options**</span></span>
- <span data-ttu-id="25c3f-142">Dynamics 365 for Sales Professional (NIEUW)</span><span class="sxs-lookup"><span data-stu-id="25c3f-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="25c3f-143">Dynamics 365 for Sales Professional (NIEUW)</span><span class="sxs-lookup"><span data-stu-id="25c3f-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="25c3f-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="25c3f-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="25c3f-145">Dynamics 365 Customer Engagement Plan of</span><span class="sxs-lookup"><span data-stu-id="25c3f-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="25c3f-146">Dynamics 365-teamleden</span><span class="sxs-lookup"><span data-stu-id="25c3f-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="25c3f-147">Klanten overstappen op nieuwe productplannen</span><span class="sxs-lookup"><span data-stu-id="25c3f-147">Transition customers to new product plans</span></span>

<span data-ttu-id="25c3f-148">Voor het verplaatsen van klanten van niet-bestaande SKU's naar nieuwere SKU's zijn de volgende stappen in deze volgorde vereist:</span><span class="sxs-lookup"><span data-stu-id="25c3f-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="25c3f-149">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="25c3f-149">Purchase the new subscription</span></span>
- <span data-ttu-id="25c3f-150">Huidige gebruikerslicenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="25c3f-150">Reassign current user licenses</span></span>
- <span data-ttu-id="25c3f-151">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="25c3f-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="25c3f-152">Het nieuwe abonnement voor uw klant kopen</span><span class="sxs-lookup"><span data-stu-id="25c3f-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="25c3f-153">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u wilt verplaatsen naar het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="25c3f-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="25c3f-154">Selecteer **Abonnement toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="25c3f-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="25c3f-155">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **verzenden.**</span><span class="sxs-lookup"><span data-stu-id="25c3f-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="25c3f-156">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="25c3f-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="25c3f-157">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="25c3f-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="25c3f-158">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.</span><span class="sxs-lookup"><span data-stu-id="25c3f-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="25c3f-159">Selecteer **Gebruikers en licenties.**</span><span class="sxs-lookup"><span data-stu-id="25c3f-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="25c3f-160">Als u een licentie opnieuw wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u **vervolgens Licenties beheren.**</span><span class="sxs-lookup"><span data-stu-id="25c3f-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="25c3f-161">Schakel **op** de pagina Licenties beheren het selectievakje Licentie voor Dynamics 365 for Sales/Customer Engagement Plan van Basic (gekwalificeerde aanbieding) uit en selecteer een nieuw serviceplan voor het abonnement waar de klant naar overstapt.</span><span class="sxs-lookup"><span data-stu-id="25c3f-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="25c3f-162">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="25c3f-162">Select **Submit**.</span></span> <span data-ttu-id="25c3f-163">U doet dit voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="25c3f-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="25c3f-164">Nadat u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="25c3f-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="25c3f-165">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.</span><span class="sxs-lookup"><span data-stu-id="25c3f-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="25c3f-166">Stel op de detailpagina van het abonnement het oude abonnement in op **Tijdelijk en** selecteer **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="25c3f-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="25c3f-167">Het oude abonnement is nu opgeschort en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="25c3f-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="25c3f-168">De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd.</span><span class="sxs-lookup"><span data-stu-id="25c3f-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="25c3f-169">Uw klant maakt geen extra kosten voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="25c3f-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



