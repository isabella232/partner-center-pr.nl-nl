---
title: Dynamics 365 Business Edition migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het migreren van gekwalificeerde Dynamics 365 Business Edition-aanbiedingen naar nieuwere versies voordat ze verlopen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/17/2020
ms.locfileid: "92527517"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="913c7-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Aanbiedingen van Dynamics 365 Business Edition migreren naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="913c7-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="913c7-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="913c7-104">**Applies to**</span></span>

- <span data-ttu-id="913c7-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="913c7-105">Partner Center</span></span>

<span data-ttu-id="913c7-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="913c7-106">**Appropriate roles**</span></span>
- <span data-ttu-id="913c7-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="913c7-107">Global admin</span></span>
- <span data-ttu-id="913c7-108">Gebruikersbeheerder</span><span class="sxs-lookup"><span data-stu-id="913c7-108">User admin</span></span>
- <span data-ttu-id="913c7-109">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="913c7-109">Admin agent</span></span>
- <span data-ttu-id="913c7-110">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="913c7-110">Sales agent</span></span>

<span data-ttu-id="913c7-111">Met ingang van 1 januari 2019 kunnen klanten met Dynamics 365 Business Edition-abonnementen niet langer worden verlengd naar deze verouderde aanbiedingen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="913c7-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="913c7-112">Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '.</span><span class="sxs-lookup"><span data-stu-id="913c7-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="913c7-113">Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="913c7-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="913c7-114">U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.</span><span class="sxs-lookup"><span data-stu-id="913c7-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="913c7-115">Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren.</span><span class="sxs-lookup"><span data-stu-id="913c7-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="913c7-116">De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="913c7-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="913c7-117">U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="913c7-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="913c7-118">De Dynamics 365 Business-edities buiten gebruik gesteld</span><span class="sxs-lookup"><span data-stu-id="913c7-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="913c7-119">Dynamics 365 voor Financiën en operationele activiteiten, Business Edition</span><span class="sxs-lookup"><span data-stu-id="913c7-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="913c7-120">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="913c7-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="913c7-121">Dynamics business Central-de Dynamics 365 Business Edition nieuwe aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="913c7-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="913c7-122">Met de nieuwe aanbiedingen voor Dynamics business Central kunnen uw klanten hun financiën, verkoop, service en activiteiten verbinden om bedrijfs processen te stroom lijnen, interacties van klanten te verbeteren en betere beslissingen te nemen.</span><span class="sxs-lookup"><span data-stu-id="913c7-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="913c7-123">Dynamics 365 Business Central is alleen beschikbaar via Cloud Solution Provider (CSP)-programma partners.</span><span class="sxs-lookup"><span data-stu-id="913c7-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="913c7-124">Dynamics 365 Business Edition-klanten komen in aanmerking voor korting op prijzen voor de nieuwe Business Central-aanbiedingen tot en met 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="913c7-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="913c7-125">Klanten overstappen naar nieuwe product abonnementen</span><span class="sxs-lookup"><span data-stu-id="913c7-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="913c7-126">Voor het verplaatsen van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd in deze volg orde:</span><span class="sxs-lookup"><span data-stu-id="913c7-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="913c7-127">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="913c7-127">Purchase the new subscription</span></span>
- <span data-ttu-id="913c7-128">Huidige gebruikers licenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="913c7-128">Reassign current user licenses</span></span>
- <span data-ttu-id="913c7-129">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="913c7-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="913c7-130">Koop het nieuwe abonnement voor uw klant</span><span class="sxs-lookup"><span data-stu-id="913c7-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="913c7-131">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u naar het nieuwe abonnement wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="913c7-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="913c7-132">Selecteer **abonnement toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="913c7-132">Select **Add Subscription** .</span></span>
3. <span data-ttu-id="913c7-133">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden** .</span><span class="sxs-lookup"><span data-stu-id="913c7-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit** .</span></span> 

<span data-ttu-id="913c7-134">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="913c7-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="913c7-135">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="913c7-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="913c7-136">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="913c7-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="913c7-137">Selecteer **gebruikers en licenties** .</span><span class="sxs-lookup"><span data-stu-id="913c7-137">Select **Users and licenses** .</span></span>
3. <span data-ttu-id="913c7-138">Als u een licentie wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u vervolgens **licenties beheren** .</span><span class="sxs-lookup"><span data-stu-id="913c7-138">To reassign a license to a user, select the user and then select **Manage licenses** .</span></span> 
4. <span data-ttu-id="913c7-139">Schakel op de pagina **licenties beheren** het selectie vakje Dynamics 365 voor verkoop/klant engagement van de Basic-licentie (gekwalificeerd aanbod) uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.</span><span class="sxs-lookup"><span data-stu-id="913c7-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="913c7-140">Selecteer **Indienen** .</span><span class="sxs-lookup"><span data-stu-id="913c7-140">Select **Submit** .</span></span> <span data-ttu-id="913c7-141">U kunt dit doen voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="913c7-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="913c7-142">Zodra u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="913c7-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="913c7-143">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="913c7-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="913c7-144">Stel op de pagina abonnements Details het oude abonnement in op **opgeschort** en selecteer **indienen** .</span><span class="sxs-lookup"><span data-stu-id="913c7-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit** .</span></span>

<span data-ttu-id="913c7-145">Het oude abonnement is nu onderbroken en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="913c7-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="913c7-146">Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht.</span><span class="sxs-lookup"><span data-stu-id="913c7-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="913c7-147">Uw klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="913c7-147">Your customer will incur no additional costs for the old subscription.</span></span>
