---
title: Gekwalificeerde Dynamics 365-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u migreert van gekwalificeerd, Basic Dynamics 365-abonnementen naar een nieuw abonnement voordat bestaande abonnementen verlopen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527518"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="2c508-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Abonnement van Dynamics 365 en Customer Engagement (gekwalificeerde aanbiedingen) migreren van Basic naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="2c508-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="2c508-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="2c508-104">**Applies to**</span></span>

-  <span data-ttu-id="2c508-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="2c508-105">Partner Center</span></span>

<span data-ttu-id="2c508-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="2c508-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="2c508-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="2c508-107">Global admin</span></span>
-   <span data-ttu-id="2c508-108">Gebruikersbeheerder</span><span class="sxs-lookup"><span data-stu-id="2c508-108">User admin</span></span>
-   <span data-ttu-id="2c508-109">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="2c508-109">Admin agent</span></span>
-   <span data-ttu-id="2c508-110">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="2c508-110">Sales agent</span></span>

<span data-ttu-id="2c508-111">Met ingang van 1 januari 2019 kunnen deze verouderde aanbiedingen niet langer worden vernieuwd door klanten met Dynamics 365 voor verkoop-en klant betrokkenheid van basis abonnementen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="2c508-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="2c508-112">Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '.</span><span class="sxs-lookup"><span data-stu-id="2c508-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2c508-113">Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="2c508-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="2c508-114">U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.</span><span class="sxs-lookup"><span data-stu-id="2c508-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="2c508-115">Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren.</span><span class="sxs-lookup"><span data-stu-id="2c508-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="2c508-116">De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="2c508-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="2c508-117">U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c508-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="2c508-118">De Dynamics 365-aanbiedingen die buiten gebruik worden gesteld</span><span class="sxs-lookup"><span data-stu-id="2c508-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="2c508-119">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-120">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2c508-121">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-122">Dynamics 365 voor Sales Enter prise Edition (prijzen voor de overheid) CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-123">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-124">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2c508-125">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-126">Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-127">Dynamics 365 for Sales Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-128">Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2c508-129">Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-130">Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-131">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-132">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) CRMOL Basic (aanbieding in aanmerking komend)</span><span class="sxs-lookup"><span data-stu-id="2c508-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-133">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-134">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2c508-135">Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-136">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-137">Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-138">Dynamics 365 Customer engagement plan Enter prise Edition van SA for CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="2c508-139">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-140">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-141">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="2c508-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="2c508-142">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="2c508-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="2c508-143">Dynamics 365 voor verkoop/klant engagement plan van basis (aanbiedingen)</span><span class="sxs-lookup"><span data-stu-id="2c508-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="2c508-144">**Aanbiedingen buiten gebruik gesteld**</span><span class="sxs-lookup"><span data-stu-id="2c508-144">**Retired offers**</span></span>   

- <span data-ttu-id="2c508-145">Dynamics 365 voor verkoop van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="2c508-146">Dynamics 365 Customer engagement plan van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="2c508-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="2c508-147">**Vervangende opties**</span><span class="sxs-lookup"><span data-stu-id="2c508-147">**Replacement options**</span></span>
- <span data-ttu-id="2c508-148">Dynamics 365 voor Sales Professional (nieuw)</span><span class="sxs-lookup"><span data-stu-id="2c508-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="2c508-149">Dynamics 365 voor Sales Professional (nieuw)</span><span class="sxs-lookup"><span data-stu-id="2c508-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="2c508-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="2c508-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="2c508-151">Dynamics 365 Customer engagement-abonnement of</span><span class="sxs-lookup"><span data-stu-id="2c508-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="2c508-152">Dynamics 365-team leden</span><span class="sxs-lookup"><span data-stu-id="2c508-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2c508-153">Klanten overstappen naar nieuwe product abonnementen</span><span class="sxs-lookup"><span data-stu-id="2c508-153">Transition customers to new product plans</span></span>

<span data-ttu-id="2c508-154">Voor het verplaatsen van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd in deze volg orde:</span><span class="sxs-lookup"><span data-stu-id="2c508-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="2c508-155">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="2c508-155">Purchase the new subscription</span></span>
- <span data-ttu-id="2c508-156">Huidige gebruikers licenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="2c508-156">Reassign current user licenses</span></span>
- <span data-ttu-id="2c508-157">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="2c508-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="2c508-158">Koop het nieuwe abonnement voor uw klant</span><span class="sxs-lookup"><span data-stu-id="2c508-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="2c508-159">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u naar het nieuwe abonnement wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="2c508-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="2c508-160">Selecteer **abonnement toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="2c508-160">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="2c508-161">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden** .</span><span class="sxs-lookup"><span data-stu-id="2c508-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="2c508-162">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c508-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="2c508-163">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="2c508-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="2c508-164">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="2c508-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="2c508-165">Selecteer **gebruikers en licenties** .</span><span class="sxs-lookup"><span data-stu-id="2c508-165">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="2c508-166">Als u een licentie wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u vervolgens **licenties beheren** .</span><span class="sxs-lookup"><span data-stu-id="2c508-166">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="2c508-167">Schakel op de pagina **licenties beheren** het selectie vakje Dynamics 365 voor verkoop/klant engagement van de Basic-licentie (gekwalificeerd aanbod) uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.</span><span class="sxs-lookup"><span data-stu-id="2c508-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="2c508-168">Selecteer **Indienen** .</span><span class="sxs-lookup"><span data-stu-id="2c508-168">Select **Submit** .</span></span> <span data-ttu-id="2c508-169">U kunt dit doen voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="2c508-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="2c508-170">Zodra u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="2c508-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="2c508-171">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="2c508-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="2c508-172">Stel op de pagina abonnements Details het oude abonnement in op **opgeschort** en selecteer **indienen** .</span><span class="sxs-lookup"><span data-stu-id="2c508-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="2c508-173">Het oude abonnement is nu onderbroken en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="2c508-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="2c508-174">Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht.</span><span class="sxs-lookup"><span data-stu-id="2c508-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2c508-175">Uw klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="2c508-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



