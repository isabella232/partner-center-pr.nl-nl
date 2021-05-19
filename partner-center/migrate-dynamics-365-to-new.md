---
title: Dynamics 365 Business Edition migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het migreren van gekwalificeerde Aanbiedingen van Dynamics 365 Business Edition naar nieuwere versies voordat ze verlopen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151522"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="afca0-103">Migrate Dynamics 365 Business Edition Offers to newer versions (Aanbiedingen van Dynamics 365 Business Edition migreren naar nieuwere versies)</span><span class="sxs-lookup"><span data-stu-id="afca0-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="afca0-104">**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Verkoopagent</span><span class="sxs-lookup"><span data-stu-id="afca0-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="afca0-105">Vanaf 1 januari 2019 kunnen klanten met Dynamics 365 Business Edition-abonnementen niet meer worden verlengd voor deze verouderde aanbiedingen; bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen.</span><span class="sxs-lookup"><span data-stu-id="afca0-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="afca0-106">Op de detailpagina van het abonnement wordt de status van het abonnement gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'.</span><span class="sxs-lookup"><span data-stu-id="afca0-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="afca0-107">Om de continuïteit voor klanten te waarborgen, moet u de klanten met verlopen abonnementen overstappen naar een ondersteunde optie, die hieronder wordt vermeld.</span><span class="sxs-lookup"><span data-stu-id="afca0-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="afca0-108">Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="afca0-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="afca0-109">Als u de API (ZOWEL DEP als Partner Center) gebruikt, kunt u verlopende abonnementen vinden door de einddatum van het abonnement samen met de eigenschap auto renew = False te evalueren.</span><span class="sxs-lookup"><span data-stu-id="afca0-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="afca0-110">De abonnementen in kwestie worden op 1 januari 2019 ingesteld op automatisch verlengen=Onwaar.</span><span class="sxs-lookup"><span data-stu-id="afca0-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="afca0-111">U kunt klanten op elk moment verplaatsen naar een nieuw abonnement.</span><span class="sxs-lookup"><span data-stu-id="afca0-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="afca0-112">De Dynamics 365 Business Editions die niet meer worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="afca0-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="afca0-113">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="afca0-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="afca0-114">Dynamics 365 for Team Members, Business edition</span><span class="sxs-lookup"><span data-stu-id="afca0-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="afca0-115">Dynamics Business Central: de nieuwe aanbiedingen voor Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="afca0-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="afca0-116">Met de nieuwe Dynamics Business Central-aanbiedingen kunnen uw klanten hun financiën, verkoop, service en activiteiten verbinden om bedrijfsprocessen te stroomlijnen, interacties van klanten te verbeteren en betere beslissingen te nemen.</span><span class="sxs-lookup"><span data-stu-id="afca0-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="afca0-117">Dynamics 365 Business Central is gebaseerd op de cloud en is alleen beschikbaar via Cloud Solution Provider (CSP)-programmapartners.</span><span class="sxs-lookup"><span data-stu-id="afca0-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="afca0-118">Klanten van Dynamics 365 Business Edition komen in aanmerking voor korting op overgangsprijzen voor de nieuwe Business Central-aanbiedingen tot en met 30 juni 2020.</span><span class="sxs-lookup"><span data-stu-id="afca0-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="afca0-119">Klanten overstappen op nieuwe productplannen</span><span class="sxs-lookup"><span data-stu-id="afca0-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="afca0-120">Voor het verplaatsen van klanten van niet-bestaande SKU's naar nieuwere SKU's zijn de volgende stappen in deze volgorde vereist:</span><span class="sxs-lookup"><span data-stu-id="afca0-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="afca0-121">Het nieuwe abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="afca0-121">Purchase the new subscription</span></span>
- <span data-ttu-id="afca0-122">Huidige gebruikerslicenties opnieuw toewijzen</span><span class="sxs-lookup"><span data-stu-id="afca0-122">Reassign current user licenses</span></span>
- <span data-ttu-id="afca0-123">Oud abonnement annuleren</span><span class="sxs-lookup"><span data-stu-id="afca0-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="afca0-124">Het nieuwe abonnement voor uw klant kopen</span><span class="sxs-lookup"><span data-stu-id="afca0-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="afca0-125">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u wilt verplaatsen naar het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="afca0-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="afca0-126">Selecteer **Abonnement toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="afca0-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="afca0-127">Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **verzenden.**</span><span class="sxs-lookup"><span data-stu-id="afca0-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="afca0-128">Uw klant heeft nu zowel het oude als het nieuwe abonnement.</span><span class="sxs-lookup"><span data-stu-id="afca0-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="afca0-129">De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="afca0-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="afca0-130">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.</span><span class="sxs-lookup"><span data-stu-id="afca0-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="afca0-131">Selecteer **Gebruikers en licenties.**</span><span class="sxs-lookup"><span data-stu-id="afca0-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="afca0-132">Als u een licentie opnieuw wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u **vervolgens Licenties beheren.**</span><span class="sxs-lookup"><span data-stu-id="afca0-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="afca0-133">Schakel **op** de pagina Licenties beheren het selectievakje Licentie voor Dynamics 365 for Sales/Customer Engagement Plan van Basic (gekwalificeerde aanbieding) uit en selecteer een nieuw serviceplan voor het abonnement waar de klant naar overstapt.</span><span class="sxs-lookup"><span data-stu-id="afca0-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="afca0-134">Selecteer **Indienen**.</span><span class="sxs-lookup"><span data-stu-id="afca0-134">Select **Submit**.</span></span> <span data-ttu-id="afca0-135">U doet dit voor elke gebruiker die de nieuwe licentie nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="afca0-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="afca0-136">Nadat u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren.</span><span class="sxs-lookup"><span data-stu-id="afca0-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="afca0-137">Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.</span><span class="sxs-lookup"><span data-stu-id="afca0-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="afca0-138">Stel op de detailpagina van het abonnement het oude abonnement in op **Tijdelijk en** selecteer **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="afca0-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="afca0-139">Het oude abonnement is nu opgeschort en het nieuwe abonnement is actief.</span><span class="sxs-lookup"><span data-stu-id="afca0-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="afca0-140">De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd.</span><span class="sxs-lookup"><span data-stu-id="afca0-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="afca0-141">Uw klant maakt geen extra kosten voor het oude abonnement.</span><span class="sxs-lookup"><span data-stu-id="afca0-141">Your customer will incur no additional costs for the old subscription.</span></span>
