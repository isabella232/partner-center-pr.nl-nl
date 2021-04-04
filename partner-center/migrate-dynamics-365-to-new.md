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
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132635"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="0f59a-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Aanbiedingen van Dynamics 365 Business Edition migreren naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="0f59a-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="0f59a-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="0f59a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0f59a-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="0f59a-105">Global admin</span></span>
- <span data-ttu-id="0f59a-106">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="0f59a-106">User management admin</span></span>
- <span data-ttu-id="0f59a-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="0f59a-107">Admin agent</span></span>
- <span data-ttu-id="0f59a-108">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="0f59a-108">Sales agent</span></span>

<span data-ttu-id="0f59a-109">Met ingang van 1 januari 2019 kunnen klanten met Dynamics 365 Business Edition-abonnementen niet langer worden verlengd naar deze verouderde aanbiedingen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="0f59a-110">Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '.</span><span class="sxs-lookup"><span data-stu-id="0f59a-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="0f59a-111">Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="0f59a-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="0f59a-112">U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="0f59a-113">Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren.</span><span class="sxs-lookup"><span data-stu-id="0f59a-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="0f59a-114">De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019.</span><span class="sxs-lookup"><span data-stu-id="0f59a-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="0f59a-115">U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="0f59a-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="0f59a-116">De Dynamics 365 Business-edities buiten gebruik gesteld</span><span class="sxs-lookup"><span data-stu-id="0f59a-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="0f59a-117">Dynamics 365 voor Financiën en operationele activiteiten, Business Edition</span><span class="sxs-lookup"><span data-stu-id="0f59a-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="0f59a-118">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="0f59a-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="0f59a-119">Dynamics business Central-de Dynamics 365 Business Edition nieuwe aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="0f59a-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="0f59a-120">Met de nieuwe aanbiedingen voor Dynamics business Central kunnen uw klanten hun financiën, verkoop, service en activiteiten verbinden om bedrijfs processen te stroom lijnen, interacties van klanten te verbeteren en betere beslissingen te nemen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="0f59a-121">Dynamics 365 Business Central is alleen beschikbaar via Cloud Solution Provider (CSP)-programma partners.</span><span class="sxs-lookup"><span data-stu-id="0f59a-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="0f59a-122">Dynamics 365 Business Edition-klanten komen in aanmerking voor korting op prijzen voor de nieuwe Business Central-aanbiedingen tot en met 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="0f59a-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="0f59a-123">Klanten overstappen naar nieuwe product abonnementen</span><span class="sxs-lookup"><span data-stu-id="0f59a-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="0f59a-124">Voor het verplaatsen van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd in deze volg orde:</span><span class="sxs-lookup"><span data-stu-id="0f59a-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="0f59a-125">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="0f59a-125">Purchase the new subscription</span></span>
- <span data-ttu-id="0f59a-126">Huidige gebruikers licenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="0f59a-126">Reassign current user licenses</span></span>
- <span data-ttu-id="0f59a-127">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="0f59a-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="0f59a-128">Koop het nieuwe abonnement voor uw klant</span><span class="sxs-lookup"><span data-stu-id="0f59a-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="0f59a-129">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u naar het nieuwe abonnement wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="0f59a-130">Selecteer **abonnement toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="0f59a-131">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="0f59a-132">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="0f59a-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="0f59a-133">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="0f59a-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="0f59a-134">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0f59a-135">Selecteer **gebruikers en licenties**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="0f59a-136">Als u een licentie wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u vervolgens **licenties beheren**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="0f59a-137">Schakel op de pagina **licenties beheren** het selectie vakje Dynamics 365 voor verkoop/klant engagement van de Basic-licentie (gekwalificeerd aanbod) uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.</span><span class="sxs-lookup"><span data-stu-id="0f59a-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="0f59a-138">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-138">Select **Submit**.</span></span> <span data-ttu-id="0f59a-139">U kunt dit doen voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="0f59a-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="0f59a-140">Zodra u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="0f59a-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="0f59a-141">Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="0f59a-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="0f59a-142">Stel op de pagina abonnements Details het oude abonnement in op **opgeschort** en selecteer **indienen**.</span><span class="sxs-lookup"><span data-stu-id="0f59a-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="0f59a-143">Het oude abonnement is nu onderbroken en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="0f59a-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="0f59a-144">Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht.</span><span class="sxs-lookup"><span data-stu-id="0f59a-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="0f59a-145">Uw klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="0f59a-145">Your customer will incur no additional costs for the old subscription.</span></span>
