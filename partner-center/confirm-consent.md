---
title: Acceptatie van klant bevestigen voor micro soft-klant overeenkomst
description: Meer informatie over het bevestigen van de acceptatie van de klant door de klant overeenkomst van micro soft. Dit kan nodig zijn om micro soft-producten en-services voor klanten te best Ellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354607"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="001f5-104">Bijgewerkte methode om acceptatie van klant te bevestigen van de micro soft-klant overeenkomst</span><span class="sxs-lookup"><span data-stu-id="001f5-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>


<span data-ttu-id="001f5-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="001f5-105">**Appropriate roles**</span></span>

- <span data-ttu-id="001f5-106">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="001f5-106">Admin agent</span></span>
- <span data-ttu-id="001f5-107">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="001f5-107">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="001f5-108">De bron van de overeenkomst wordt momenteel alleen ondersteund door het partner centrum in de open bare cloud van micro soft.</span><span class="sxs-lookup"><span data-stu-id="001f5-108">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="001f5-109">Het is niet van toepassing op:</span><span class="sxs-lookup"><span data-stu-id="001f5-109">It is not applicable to:</span></span>
> * <span data-ttu-id="001f5-110">Partner centrum beheerd door 21Vianet</span><span class="sxs-lookup"><span data-stu-id="001f5-110">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="001f5-111">Partnercentrum voor Microsoft Cloud Duitsland</span><span class="sxs-lookup"><span data-stu-id="001f5-111">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="001f5-112">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="001f5-112">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="001f5-113">Vanaf 31 januari 2020 moeten alle klanten, bestaande en nieuwe, de nieuwe micro soft-klant overeenkomst ondertekenen.</span><span class="sxs-lookup"><span data-stu-id="001f5-113">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="001f5-114">Lees voor meer informatie [klant acceptatie bevestigen van de micro soft-klant overeenkomst](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="001f5-114">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="001f5-115">Als partner moet u de acceptatie van de klant van micro soft verkrijgen voordat u micro soft-producten en-services voor die klant kunt best Ellen.</span><span class="sxs-lookup"><span data-stu-id="001f5-115">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="001f5-116">Om ervoor te zorgen dat partners voldoen aan nalevings vereisten, vraagt micro soft partners om acceptatie te bevestigen door de volgende gegevens te verstrekken over degene die de overeenkomst heeft geaccepteerd:</span><span class="sxs-lookup"><span data-stu-id="001f5-116">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="001f5-117">Voornaam</span><span class="sxs-lookup"><span data-stu-id="001f5-117">First name</span></span>

- <span data-ttu-id="001f5-118">Achternaam</span><span class="sxs-lookup"><span data-stu-id="001f5-118">Last name</span></span>

- <span data-ttu-id="001f5-119">E-mailadres</span><span class="sxs-lookup"><span data-stu-id="001f5-119">Email address</span></span>

- <span data-ttu-id="001f5-120">Telefoon nummer (optioneel)</span><span class="sxs-lookup"><span data-stu-id="001f5-120">Phone number (optional)</span></span>

- <span data-ttu-id="001f5-121">Datum van acceptatie</span><span class="sxs-lookup"><span data-stu-id="001f5-121">Date of acceptance</span></span>

<span data-ttu-id="001f5-122">Directe factuur partners en indirecte providers moeten acceptatie van klant bevestigen van de klant overeenkomst van micro soft bij het handelen via partner Center of partner Center-API.</span><span class="sxs-lookup"><span data-stu-id="001f5-122">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="001f5-123">Bevestiging is *verplicht*.</span><span class="sxs-lookup"><span data-stu-id="001f5-123">Confirmation is *mandatory*.</span></span>

<span data-ttu-id="001f5-124">Als er geen bevestiging is opgegeven voor een bepaalde klant:</span><span class="sxs-lookup"><span data-stu-id="001f5-124">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="001f5-125">U kunt geen nieuwe orders maken voor deze klant.</span><span class="sxs-lookup"><span data-stu-id="001f5-125">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="001f5-126">U kunt het aantal licenties van bestaande abonnementen op licenties voor deze klant niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="001f5-126">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="001f5-127">Bevestiging van acceptatie van klanten kan worden gedaan via partner centrum of de Partner Center-API.</span><span class="sxs-lookup"><span data-stu-id="001f5-127">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="001f5-128">Zie de volgende onderwerpen voor meer informatie over de Partner Center-API:</span><span class="sxs-lookup"><span data-stu-id="001f5-128">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="001f5-129">Bevestiging van toestemming van de klant verkrijgen</span><span class="sxs-lookup"><span data-stu-id="001f5-129">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="001f5-130">Meta gegevens van de overeenkomst ophalen</span><span class="sxs-lookup"><span data-stu-id="001f5-130">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="001f5-131">Toestemming van de klant bevestigen</span><span class="sxs-lookup"><span data-stu-id="001f5-131">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="001f5-132">Dit geldt voor productie-en sandbox-omgevingen.</span><span class="sxs-lookup"><span data-stu-id="001f5-132">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="001f5-133">Acceptatie van klant bevestigen voor een nieuwe klant</span><span class="sxs-lookup"><span data-stu-id="001f5-133">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="001f5-134">Gebruik de volgende procedure om de acceptatie van klanten te bevestigen terwijl u een nieuwe klant Tenant maakt in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="001f5-134">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="001f5-135">U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="001f5-135">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="001f5-136">Selecteer **klanten** en vervolgens **nieuwe klant** en selecteer vervolgens **account gegevens**.</span><span class="sxs-lookup"><span data-stu-id="001f5-136">Select **Customers**, and then **New customer** and then select **Account info**.</span></span>

2. <span data-ttu-id="001f5-137">Voer de gegevens in van het **bedrijf** en de **primaire contact persoon**.</span><span class="sxs-lookup"><span data-stu-id="001f5-137">Enter the information about the **Company** and **Primary contact**.</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Bedrijfs gegevens":::

3. <span data-ttu-id="001f5-139">Onder **micro soft-klant overeenkomst** selecteert u dat de **klant de nieuwste micro soft-klant overeenkomst heeft geaccepteerd**.</span><span class="sxs-lookup"><span data-stu-id="001f5-139">Under **Microsoft customer agreement**, select **The customer has accepted the latest Microsoft customer agreement**.</span></span>

4. <span data-ttu-id="001f5-140">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="001f5-140">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="001f5-141">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="001f5-141">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="001f5-142">Voer de details in van de gebruiker die de acceptatie heeft opgegeven.</span><span class="sxs-lookup"><span data-stu-id="001f5-142">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Acceptatie datum toevoegen":::

   <span data-ttu-id="001f5-144">Standaard worden de gegevens van de primaire contact persoon weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="001f5-144">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="001f5-145">Als dat niet het geval is, selecteert u **bijwerken** en voert u vervolgens de **voor naam**, **Achternaam**, **e-mail adres** en het \**telefoon nummer* (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="001f5-145">If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and \**Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="001f5-146">Selecteer **volgende** om door te gaan met de resterende stappen voor het maken van de Tenant van de klant.</span><span class="sxs-lookup"><span data-stu-id="001f5-146">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="001f5-147">Acceptatie van klant bevestigen voor een bestaande klant</span><span class="sxs-lookup"><span data-stu-id="001f5-147">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="001f5-148">U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="001f5-148">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="001f5-149">Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.</span><span class="sxs-lookup"><span data-stu-id="001f5-149">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="001f5-150">Selecteer **account gegevens**.</span><span class="sxs-lookup"><span data-stu-id="001f5-150">Select **Account info**.</span></span>

3. <span data-ttu-id="001f5-151">Selecteer in de **micro soft-klant overeenkomst** **Update**.</span><span class="sxs-lookup"><span data-stu-id="001f5-151">Under **Microsoft customer agreement**, select **Update**.</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Bijwerken":::

4. <span data-ttu-id="001f5-153">Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="001f5-153">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="001f5-154">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="001f5-154">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="001f5-155">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="001f5-155">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="001f5-156">Selecteer **Opslaan en doorgaan**.</span><span class="sxs-lookup"><span data-stu-id="001f5-156">Select **Save and continue**.</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="001f5-157">Acceptatie van klant bevestigen bij het maken van een nieuwe order voor een bestaande klant</span><span class="sxs-lookup"><span data-stu-id="001f5-157">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="001f5-158">Als u probeert een nieuwe bestelling te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te volt ooien.</span><span class="sxs-lookup"><span data-stu-id="001f5-158">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="001f5-159">Gebruik de volgende procedure om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="001f5-159">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="001f5-160">Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="001f5-160">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="001f5-161">Voer bij **acceptatie datum** van de overeenkomst de juiste datum in.</span><span class="sxs-lookup"><span data-stu-id="001f5-161">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="001f5-162">U kunt dit niet instellen op een datum in de toekomst.</span><span class="sxs-lookup"><span data-stu-id="001f5-162">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="001f5-163">Selecteer **Opslaan en doorgaan**.</span><span class="sxs-lookup"><span data-stu-id="001f5-163">Select **Save and continue**.</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="001f5-164">Bevestiging van acceptatie van klant voor een bestaande klant ophalen</span><span class="sxs-lookup"><span data-stu-id="001f5-164">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="001f5-165">U kunt de bevestiging van acceptatie van klanten ophalen voor een bestaande klant die u eerder hebt gegeven met behulp van de onderstaande procedure.</span><span class="sxs-lookup"><span data-stu-id="001f5-165">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="001f5-166">U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.</span><span class="sxs-lookup"><span data-stu-id="001f5-166">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="001f5-167">Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.</span><span class="sxs-lookup"><span data-stu-id="001f5-167">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="001f5-168">Selecteer **account gegevens**.</span><span class="sxs-lookup"><span data-stu-id="001f5-168">Select **Account info**.</span></span>

3. <span data-ttu-id="001f5-169">Onder **micro soft-klant overeenkomst** ziet u of er al dan niet een bevestiging voor deze klant is ontvangen.</span><span class="sxs-lookup"><span data-stu-id="001f5-169">Under **Microsoft customer agreement**, you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="001f5-170">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="001f5-170">Next steps</span></span>

- [<span data-ttu-id="001f5-171">Acceptatie van klant bevestigen van de micro soft-klant overeenkomst in het CSP-partner programma</span><span class="sxs-lookup"><span data-stu-id="001f5-171">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="001f5-172">Verklaring van de micro soft-klant overeenkomst namens uw klant aanvaar ding</span><span class="sxs-lookup"><span data-stu-id="001f5-172">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)