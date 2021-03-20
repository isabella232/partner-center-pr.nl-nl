---
title: Een Azure-uitgavenbegroting voor uw klanten instellen
ms.topic: how-to
ms.date: 03/17/2021
description: Meer informatie over het instellen of verwijderen van maandelijkse Azure-uitgaven budgetten voor uw klanten, en voor het weer geven van Azure-uitgaven gegevens en het instellen van meldingen met betrekking tot budget.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712746"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="d59c7-103">Maandelijkse Azure-uitgaven budgetten instellen, controleren of verwijderen voor klanten in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="d59c7-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="d59c7-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="d59c7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d59c7-105">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="d59c7-105">Admin agent</span></span>

<span data-ttu-id="d59c7-106">U kunt [een maandelijks Azure-uitgaven budget instellen voor uw klanten](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="d59c7-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="d59c7-107">Dit helpt uw klanten hun Azure-uitgaven te beheren.</span><span class="sxs-lookup"><span data-stu-id="d59c7-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="d59c7-108">Met deze optie kunt u de Azure-uitgaven van uw klanten vergelijken met het budget tijdens de maand.</span><span class="sxs-lookup"><span data-stu-id="d59c7-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="d59c7-109">Het helpt uw klanten ook hun Azure-uitgaven te budget teren, zodat de maandelijkse factuur niet hoger is dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="d59c7-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="d59c7-110">Deze functie is niet beschikbaar in sandbox-of test accounts voor productie (TIP).</span><span class="sxs-lookup"><span data-stu-id="d59c7-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="d59c7-111">Nadat u [een Azure-uitgaven budget hebt ingesteld voor uw klant (s)](#set-azure-spending-budget), kunt u het klant gebruik ook op de volgende manieren bekijken.</span><span class="sxs-lookup"><span data-stu-id="d59c7-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="d59c7-112">Deze opties helpen u bij het herkennen van onjuist geconfigureerde services of ongebruikelijke trends die fraude kunnen Voorst Ellen.</span><span class="sxs-lookup"><span data-stu-id="d59c7-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="d59c7-113">U kunt vervolgens samen werken met uw klant (s) om de hoofd oorzaak te bepalen en de kosten te beheren.</span><span class="sxs-lookup"><span data-stu-id="d59c7-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="d59c7-114">Als dat nodig is, kunt u [het budget van de klant ook wijzigen](#set-azure-spending-budget) in een hoger bedrag.</span><span class="sxs-lookup"><span data-stu-id="d59c7-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="d59c7-115">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="d59c7-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="d59c7-116">E-mail meldingen inschakelen voor wanneer de uitgaven van een klant in de buurt zijn van de budget limiet</span><span class="sxs-lookup"><span data-stu-id="d59c7-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="d59c7-117">Gespecificeerde kosten per service weer geven voor op gebruik gebaseerde abonnementen</span><span class="sxs-lookup"><span data-stu-id="d59c7-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="d59c7-118">U kunt ook [een Azure-uitgaven budget](#remove-azure-spending-budget) voor klant (en) op elk gewenst moment verwijderen.</span><span class="sxs-lookup"><span data-stu-id="d59c7-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="d59c7-119">Azure-uitgaven gegevens</span><span class="sxs-lookup"><span data-stu-id="d59c7-119">Azure spending data</span></span>

<span data-ttu-id="d59c7-120">De kosten voor Azure-uitgaven zijn een *schatting* en de *werkelijke facturerings bedragen kunnen variëren*.</span><span class="sxs-lookup"><span data-stu-id="d59c7-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="d59c7-121">De waarde van de gegevens *weerspiegelt niet* de belastingen, tegoeden, aanpassingen of andere kosten die van toepassing kunnen zijn.</span><span class="sxs-lookup"><span data-stu-id="d59c7-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="d59c7-122">De uitgaven gegevens worden *eenmaal per dag vernieuwd*.</span><span class="sxs-lookup"><span data-stu-id="d59c7-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="d59c7-123">Uw klanten kunnen Azure-Services en-resources blijven gebruiken (en worden gefactureerd), tenzij u de account instellingen in de Azure Portal wijzigt.</span><span class="sxs-lookup"><span data-stu-id="d59c7-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="d59c7-124">Azure-uitgaven budget instellen</span><span class="sxs-lookup"><span data-stu-id="d59c7-124">Set Azure spending budget</span></span>

<span data-ttu-id="d59c7-125">U kunt *een maandelijks Azure-uitgaven budget instellen* voor meerdere klanten in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="d59c7-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="d59c7-126">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d59c7-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d59c7-127">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d59c7-128">Selecteer op de pagina **Azure-uitgaven** onder **klanten met Microsoft Azure abonnementen** de klant (en) waarvoor u een budget wilt instellen.</span><span class="sxs-lookup"><span data-stu-id="d59c7-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="d59c7-129">Voer een waarde in voor het **maandelijkse budget**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="d59c7-130">Kies **Toep assen** om uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="d59c7-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="d59c7-131">U kunt ook *een budget voor een individuele klant instellen* in de abonnements instellingen:</span><span class="sxs-lookup"><span data-stu-id="d59c7-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="d59c7-132">Meld u aan bij het dashboard van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="d59c7-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="d59c7-133">Kies in het menu aan de rechter kant onder **CSP** de optie **klanten**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="d59c7-134">Selecteer op de pagina **klanten** de **Bedrijfs naam** van de klant.</span><span class="sxs-lookup"><span data-stu-id="d59c7-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="d59c7-135">Op de pagina **abonnementen** van de klant, onder op **gebruik gebaseerd abonnement**, kiest u **budget wijzigen**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="d59c7-136">Voer een waarde in voor het budget.</span><span class="sxs-lookup"><span data-stu-id="d59c7-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="d59c7-137">Kies **Toep assen** om uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="d59c7-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="d59c7-138">Azure-uitgaven budget verwijderen</span><span class="sxs-lookup"><span data-stu-id="d59c7-138">Remove Azure spending budget</span></span>

<span data-ttu-id="d59c7-139">U kunt *een maandelijks Azure-uitgaven budget* voor uw klanten (s) verwijderen in het partner centrum:</span><span class="sxs-lookup"><span data-stu-id="d59c7-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="d59c7-140">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d59c7-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d59c7-141">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d59c7-142">Selecteer op de pagina **Azure-uitgaven** onder **klanten met Microsoft Azure abonnementen** de klant (s) waarvan u het budget wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="d59c7-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="d59c7-143">Kies **budget verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="d59c7-144">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="d59c7-144">Check current Azure spending</span></span>

<span data-ttu-id="d59c7-145">U kunt op elk gewenst moment *de huidige Azure-uitgaven en maandelijkse budgetten van uw klanten volgen* :</span><span class="sxs-lookup"><span data-stu-id="d59c7-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="d59c7-146">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="d59c7-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="d59c7-147">Kies in het menu aan de rechter kant onder **CSP** de optie **Azure-uitgaven**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="d59c7-148">Op de pagina **Azure-uitgaven** , onder **klanten met Microsoft Azure abonnementen**, ziet u een overzicht van de maandelijkse budgetten van klanten, de huidige uitgaven ramingen en het percentage van het gebruikte budget.</span><span class="sxs-lookup"><span data-stu-id="d59c7-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="d59c7-149">Meldingen voor budget limieten</span><span class="sxs-lookup"><span data-stu-id="d59c7-149">Notifications for budget limits</span></span>

<span data-ttu-id="d59c7-150">U kunt *e-mail meldingen inschakelen* voor wanneer de maandelijkse uitgaven van uw klant bijna de budget limiet overschrijden.</span><span class="sxs-lookup"><span data-stu-id="d59c7-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="d59c7-151">Wanneer u deze optie inschakelt, ontvangt u een melding wanneer klanten 80% of meer van het maandelijkse budget gebruiken.</span><span class="sxs-lookup"><span data-stu-id="d59c7-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="d59c7-152">Met deze optie kunt u uw Azure-factuur blijven gebruiken.</span><span class="sxs-lookup"><span data-stu-id="d59c7-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="d59c7-153">E-mail meldingen configureren:</span><span class="sxs-lookup"><span data-stu-id="d59c7-153">To configure email notifications:</span></span>

1. <span data-ttu-id="d59c7-154">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="d59c7-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="d59c7-155">Ga naar **Settings**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="d59c7-156">Selecteer **mijn voor keuren**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="d59c7-157">Configureer een voor keur e-mail adres als u dat nog niet hebt gedaan.</span><span class="sxs-lookup"><span data-stu-id="d59c7-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="d59c7-158">Configureer de voorkeurs taal voor de melding.</span><span class="sxs-lookup"><span data-stu-id="d59c7-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="d59c7-159">Selecteer het tabblad **CSP** onder **meldings voorkeuren** .</span><span class="sxs-lookup"><span data-stu-id="d59c7-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="d59c7-160">Controleer de e-mail optie voor **Azure-uitgaven** meldingen en **Sla** deze op.</span><span class="sxs-lookup"><span data-stu-id="d59c7-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="d59c7-161">Gespecificeerde kosten per service</span><span class="sxs-lookup"><span data-stu-id="d59c7-161">Itemized costs by service</span></span>

<span data-ttu-id="d59c7-162">U kunt de *gespecificeerde kosten (en het geschatte gebruik) per service weer geven voor op gebruik gebaseerde abonnementen*:</span><span class="sxs-lookup"><span data-stu-id="d59c7-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="d59c7-163">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="d59c7-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="d59c7-164">Kies in het menu aan de rechter kant onder **CSP** de optie **klanten**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="d59c7-165">Selecteer op de pagina **klanten** de **Bedrijfs naam** van de klant.</span><span class="sxs-lookup"><span data-stu-id="d59c7-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="d59c7-166">Selecteer op de pagina **abonnementen** van de klant onder **op gebruik gebaseerde abonnementen** de naam van het **abonnement**.</span><span class="sxs-lookup"><span data-stu-id="d59c7-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="d59c7-167">Op de pagina van het abonnement kunt u de **gespecificeerde kosten** per service controleren en het **geschatte gebruik** voor de huidige maand.</span><span class="sxs-lookup"><span data-stu-id="d59c7-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="d59c7-168">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="d59c7-168">Next steps</span></span>

- [<span data-ttu-id="d59c7-169">Nieuwe Commerce-ervaring in CSP - Azure-facturering</span><span class="sxs-lookup"><span data-stu-id="d59c7-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
