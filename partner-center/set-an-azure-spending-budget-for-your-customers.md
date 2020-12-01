---
title: Een Azure-uitgaven budget instellen voor klanten
ms.topic: how-to
ms.date: 06/03/2020
description: Meer informatie over het instellen of verwijderen van maandelijkse Azure-uitgaven budgetten voor uw klanten, en voor het weer geven van Azure-uitgaven gegevens en het instellen van meldingen met betrekking tot budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438978"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="524e1-103">Maandelijkse Azure-uitgaven budgetten instellen, controleren of verwijderen voor klanten in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="524e1-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="524e1-104">Van toepassing op:</span><span class="sxs-lookup"><span data-stu-id="524e1-104">Applies to:</span></span>

- <span data-ttu-id="524e1-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="524e1-105">Partner Center</span></span>
- <span data-ttu-id="524e1-106">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="524e1-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="524e1-107">U kunt [een maandelijks Azure-uitgaven budget instellen voor uw klanten](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="524e1-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="524e1-108">Dit helpt uw klanten hun Azure-uitgaven te beheren.</span><span class="sxs-lookup"><span data-stu-id="524e1-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="524e1-109">Met deze optie kunt u de Azure-uitgaven van uw klanten vergelijken met het budget tijdens de maand.</span><span class="sxs-lookup"><span data-stu-id="524e1-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="524e1-110">Het helpt uw klanten ook hun Azure-uitgaven te budget teren, zodat de maandelijkse factuur niet hoger is dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="524e1-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="524e1-111">Deze functie is niet beschikbaar in sandbox-of test accounts voor productie (TIP).</span><span class="sxs-lookup"><span data-stu-id="524e1-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="524e1-112">Nadat u [een Azure-uitgaven budget hebt ingesteld voor uw klant (s)](#set-azure-spending-budget), kunt u het klant gebruik ook op de volgende manieren bekijken.</span><span class="sxs-lookup"><span data-stu-id="524e1-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="524e1-113">Deze opties helpen u bij het herkennen van onjuist geconfigureerde services of ongebruikelijke trends die fraude kunnen Voorst Ellen.</span><span class="sxs-lookup"><span data-stu-id="524e1-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="524e1-114">U kunt vervolgens samen werken met uw klant (s) om de hoofd oorzaak te bepalen en de kosten te beheren.</span><span class="sxs-lookup"><span data-stu-id="524e1-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="524e1-115">Als dat nodig is, kunt u [het budget van de klant ook wijzigen](#set-azure-spending-budget) in een hoger bedrag.</span><span class="sxs-lookup"><span data-stu-id="524e1-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="524e1-116">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="524e1-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="524e1-117">E-mail meldingen inschakelen voor wanneer de uitgaven van een klant in de buurt zijn van de budget limiet</span><span class="sxs-lookup"><span data-stu-id="524e1-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="524e1-118">Gespecificeerde kosten per service weer geven voor op gebruik gebaseerde abonnementen</span><span class="sxs-lookup"><span data-stu-id="524e1-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="524e1-119">U kunt ook [een Azure-uitgaven budget](#remove-azure-spending-budget) voor klant (en) op elk gewenst moment verwijderen.</span><span class="sxs-lookup"><span data-stu-id="524e1-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="524e1-120">Azure-uitgaven gegevens</span><span class="sxs-lookup"><span data-stu-id="524e1-120">Azure spending data</span></span>

<span data-ttu-id="524e1-121">De kosten voor Azure-uitgaven zijn een *schatting* en de *werkelijke facturerings bedragen kunnen variëren*.</span><span class="sxs-lookup"><span data-stu-id="524e1-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="524e1-122">De waarde van de gegevens *weerspiegelt niet* de belastingen, tegoeden, aanpassingen of andere kosten die van toepassing kunnen zijn.</span><span class="sxs-lookup"><span data-stu-id="524e1-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="524e1-123">De uitgaven gegevens worden *eenmaal per dag vernieuwd*.</span><span class="sxs-lookup"><span data-stu-id="524e1-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="524e1-124">Uw klanten kunnen Azure-Services en-resources blijven gebruiken (en worden gefactureerd), tenzij u de account instellingen in de Azure Portal wijzigt.</span><span class="sxs-lookup"><span data-stu-id="524e1-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="524e1-125">Azure-uitgaven budget instellen</span><span class="sxs-lookup"><span data-stu-id="524e1-125">Set Azure spending budget</span></span>

<span data-ttu-id="524e1-126">U kunt *een maandelijks Azure-uitgaven budget instellen* voor meerdere klanten in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="524e1-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="524e1-127">Meld u aan bij het [dash board van de partner centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="524e1-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="524e1-128">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="524e1-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="524e1-129">Selecteer op de pagina **Azure-uitgaven** onder **klanten met Microsoft Azure abonnementen** de klant (en) waarvoor u een budget wilt instellen.</span><span class="sxs-lookup"><span data-stu-id="524e1-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="524e1-130">Voer een waarde in voor het **maandelijkse budget**.</span><span class="sxs-lookup"><span data-stu-id="524e1-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="524e1-131">Kies **Toep assen** om uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="524e1-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="524e1-132">U kunt ook *een budget voor een individuele klant instellen* in de abonnements instellingen:</span><span class="sxs-lookup"><span data-stu-id="524e1-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="524e1-133">Meld u aan bij het dash board van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="524e1-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="524e1-134">Kies in het menu aan de rechter kant onder **CSP** de optie **klanten**.</span><span class="sxs-lookup"><span data-stu-id="524e1-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="524e1-135">Selecteer op de pagina **klanten** de **Bedrijfs naam** van de klant.</span><span class="sxs-lookup"><span data-stu-id="524e1-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="524e1-136">Op de pagina **abonnementen** van de klant, onder op **gebruik gebaseerd abonnement**, kiest u **budget wijzigen**.</span><span class="sxs-lookup"><span data-stu-id="524e1-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="524e1-137">Voer een waarde in voor het budget.</span><span class="sxs-lookup"><span data-stu-id="524e1-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="524e1-138">Kies **Toep assen** om uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="524e1-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="524e1-139">Azure-uitgaven budget verwijderen</span><span class="sxs-lookup"><span data-stu-id="524e1-139">Remove Azure spending budget</span></span>

<span data-ttu-id="524e1-140">U kunt *een maandelijks Azure-uitgaven budget* voor uw klanten (s) verwijderen in het partner centrum:</span><span class="sxs-lookup"><span data-stu-id="524e1-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="524e1-141">Meld u aan bij het [dash board van de partner centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="524e1-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="524e1-142">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="524e1-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="524e1-143">Selecteer op de pagina **Azure-uitgaven** onder **klanten met Microsoft Azure abonnementen** de klant (s) waarvan u het budget wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="524e1-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="524e1-144">Kies **budget verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="524e1-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="524e1-145">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="524e1-145">Check current Azure spending</span></span>

<span data-ttu-id="524e1-146">U kunt op elk gewenst moment *de huidige Azure-uitgaven en maandelijkse budgetten van uw klanten volgen* :</span><span class="sxs-lookup"><span data-stu-id="524e1-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="524e1-147">Meld u aan bij het [dash board van de partner centrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="524e1-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="524e1-148">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="524e1-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="524e1-149">Op de pagina **Azure-uitgaven** , onder **klanten met Microsoft Azure abonnementen**, ziet u een overzicht van de maandelijkse budgetten van klanten, de huidige uitgaven ramingen en het percentage van het gebruikte budget.</span><span class="sxs-lookup"><span data-stu-id="524e1-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="524e1-150">Meldingen voor budget limieten</span><span class="sxs-lookup"><span data-stu-id="524e1-150">Notifications for budget limits</span></span>

<span data-ttu-id="524e1-151">U kunt *e-mail meldingen inschakelen* voor wanneer de maandelijkse uitgaven van uw klant bijna de budget limiet overschrijden.</span><span class="sxs-lookup"><span data-stu-id="524e1-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="524e1-152">Wanneer u deze optie inschakelt, ontvangt u een melding wanneer klanten 80% of meer van het maandelijkse budget gebruiken.</span><span class="sxs-lookup"><span data-stu-id="524e1-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="524e1-153">Met deze optie kunt u uw Azure-factuur blijven gebruiken.</span><span class="sxs-lookup"><span data-stu-id="524e1-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="524e1-154">E-mail meldingen configureren:</span><span class="sxs-lookup"><span data-stu-id="524e1-154">To configure email notifications:</span></span>

1. <span data-ttu-id="524e1-155">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="524e1-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="524e1-156">Ga naar **Settings**.</span><span class="sxs-lookup"><span data-stu-id="524e1-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="524e1-157">Selecteer **mijn voor keuren**.</span><span class="sxs-lookup"><span data-stu-id="524e1-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="524e1-158">Configureer een voor keur e-mail adres als u dat nog niet hebt gedaan.</span><span class="sxs-lookup"><span data-stu-id="524e1-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="524e1-159">Configureer de voorkeurs taal voor de melding.</span><span class="sxs-lookup"><span data-stu-id="524e1-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="524e1-160">Selecteer het tabblad **CSP** onder **meldings voorkeuren** .</span><span class="sxs-lookup"><span data-stu-id="524e1-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="524e1-161">Controleer de e-mail optie voor **Azure-uitgaven** meldingen en **Sla** deze op.</span><span class="sxs-lookup"><span data-stu-id="524e1-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="524e1-162">Gespecificeerde kosten per service</span><span class="sxs-lookup"><span data-stu-id="524e1-162">Itemized costs by service</span></span>

<span data-ttu-id="524e1-163">U kunt de *gespecificeerde kosten (en het geschatte gebruik) per service weer geven voor op gebruik gebaseerde abonnementen*:</span><span class="sxs-lookup"><span data-stu-id="524e1-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="524e1-164">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="524e1-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="524e1-165">Kies in het menu aan de rechter kant onder **CSP** de optie **klanten**.</span><span class="sxs-lookup"><span data-stu-id="524e1-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="524e1-166">Selecteer op de pagina **klanten** de **Bedrijfs naam** van de klant.</span><span class="sxs-lookup"><span data-stu-id="524e1-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="524e1-167">Selecteer op de pagina **abonnementen** van de klant onder **op gebruik gebaseerde abonnementen** de naam van het **abonnement**.</span><span class="sxs-lookup"><span data-stu-id="524e1-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="524e1-168">Op de pagina van het abonnement kunt u de **gespecificeerde kosten** per service controleren en het **geschatte gebruik** voor de huidige maand.</span><span class="sxs-lookup"><span data-stu-id="524e1-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
