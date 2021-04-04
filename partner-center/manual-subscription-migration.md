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
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132737"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="b8a2a-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Abonnement van Dynamics 365 en Customer Engagement (gekwalificeerde aanbiedingen) migreren van Basic naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="b8a2a-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="b8a2a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b8a2a-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="b8a2a-105">Global admin</span></span>
- <span data-ttu-id="b8a2a-106">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="b8a2a-106">User management admin</span></span>
- <span data-ttu-id="b8a2a-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="b8a2a-107">Admin agent</span></span>
- <span data-ttu-id="b8a2a-108">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="b8a2a-108">Sales agent</span></span>

<span data-ttu-id="b8a2a-109">Met ingang van 1 januari 2019 kunnen deze verouderde aanbiedingen niet langer worden vernieuwd door klanten met Dynamics 365 voor verkoop-en klant betrokkenheid van basis abonnementen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="b8a2a-110">Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="b8a2a-111">Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="b8a2a-112">U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="b8a2a-113">Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="b8a2a-114">De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="b8a2a-115">U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="b8a2a-116">De Dynamics 365-aanbiedingen die buiten gebruik worden gesteld</span><span class="sxs-lookup"><span data-stu-id="b8a2a-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="b8a2a-117">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-118">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8a2a-119">Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-120">Dynamics 365 voor Sales Enter prise Edition (prijzen voor de overheid) CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-121">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-122">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8a2a-123">Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-124">Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-125">Dynamics 365 for Sales Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-126">Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8a2a-127">Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-128">Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-129">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-130">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) CRMOL Basic (aanbieding in aanmerking komend)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-131">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-132">Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8a2a-133">Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-134">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-135">Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-136">Dynamics 365 Customer engagement plan Enter prise Edition van SA for CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="b8a2a-137">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-138">Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-139">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="b8a2a-140">Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten</span><span class="sxs-lookup"><span data-stu-id="b8a2a-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="b8a2a-141">Dynamics 365 voor verkoop/klant engagement plan van basis (aanbiedingen)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="b8a2a-142">**Aanbiedingen buiten gebruik gesteld**</span><span class="sxs-lookup"><span data-stu-id="b8a2a-142">**Retired offers**</span></span>   

- <span data-ttu-id="b8a2a-143">Dynamics 365 voor verkoop van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="b8a2a-144">Dynamics 365 Customer engagement plan van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="b8a2a-145">**Vervangende opties**</span><span class="sxs-lookup"><span data-stu-id="b8a2a-145">**Replacement options**</span></span>
- <span data-ttu-id="b8a2a-146">Dynamics 365 voor Sales Professional (nieuw)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b8a2a-147">Dynamics 365 voor Sales Professional (nieuw)</span><span class="sxs-lookup"><span data-stu-id="b8a2a-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="b8a2a-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="b8a2a-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="b8a2a-149">Dynamics 365 Customer engagement-abonnement of</span><span class="sxs-lookup"><span data-stu-id="b8a2a-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="b8a2a-150">Dynamics 365-team leden</span><span class="sxs-lookup"><span data-stu-id="b8a2a-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b8a2a-151">Klanten overstappen naar nieuwe product abonnementen</span><span class="sxs-lookup"><span data-stu-id="b8a2a-151">Transition customers to new product plans</span></span>

<span data-ttu-id="b8a2a-152">Voor het verplaatsen van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd in deze volg orde:</span><span class="sxs-lookup"><span data-stu-id="b8a2a-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="b8a2a-153">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="b8a2a-153">Purchase the new subscription</span></span>
- <span data-ttu-id="b8a2a-154">Huidige gebruikers licenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="b8a2a-154">Reassign current user licenses</span></span>
- <span data-ttu-id="b8a2a-155">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="b8a2a-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="b8a2a-156">Koop het nieuwe abonnement voor uw klant</span><span class="sxs-lookup"><span data-stu-id="b8a2a-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="b8a2a-157">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u naar het nieuwe abonnement wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="b8a2a-158">Selecteer **abonnement toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="b8a2a-159">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="b8a2a-160">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="b8a2a-161">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="b8a2a-162">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b8a2a-163">Selecteer **gebruikers en licenties**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="b8a2a-164">Als u een licentie wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u vervolgens **licenties beheren**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="b8a2a-165">Schakel op de pagina **licenties beheren** het selectie vakje Dynamics 365 voor verkoop/klant engagement van de Basic-licentie (gekwalificeerd aanbod) uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="b8a2a-166">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-166">Select **Submit**.</span></span> <span data-ttu-id="b8a2a-167">U kunt dit doen voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="b8a2a-168">Zodra u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="b8a2a-169">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="b8a2a-170">Stel op de pagina abonnements Details het oude abonnement in op **opgeschort** en selecteer **indienen**.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="b8a2a-171">Het oude abonnement is nu onderbroken en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="b8a2a-172">Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b8a2a-173">Uw klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="b8a2a-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



