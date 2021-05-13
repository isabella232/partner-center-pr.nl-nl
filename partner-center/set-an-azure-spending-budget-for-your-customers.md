---
title: Een Azure-uitgavenbegroting voor uw klanten instellen
ms.topic: how-to
ms.date: 03/17/2021
description: Meer informatie over het instellen of verwijderen van maandelijkse Azure-bestedingsbudgetten voor uw klanten, en ook om Azure-bestedingsgegevens weer te geven en budgetgerelateerde meldingen in te stellen.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855349"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="ddb4b-103">Maandelijkse Azure-uitgavenbudgetten instellen, controleren of verwijderen voor klanten in Partner Center</span><span class="sxs-lookup"><span data-stu-id="ddb4b-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="ddb4b-104">**Juiste rollen:** Beheeragent</span><span class="sxs-lookup"><span data-stu-id="ddb4b-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="ddb4b-105">U kunt [een maandelijks Azure-uitgavenbudget instellen voor uw klanten](#set-azure-spending-budget) in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="ddb4b-106">Dit helpt uw klanten bij het beheren van hun Azure-uitgaven.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="ddb4b-107">Met deze optie kunt u de Azure-uitgaven van uw klanten vergelijken met het budget gedurende de maand.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="ddb4b-108">Het helpt uw klanten ook om hun Azure-uitgaven te budgeteren, zodat hun maandelijkse factuur niet hoger is dan verwacht.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="ddb4b-109">Deze functie is niet beschikbaar in sandbox- of Test in Production-accounts (TIP).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="ddb4b-110">Nadat u [een Azure-uitgavenbudget voor uw klanten](#set-azure-spending-budget)hebt ingesteld, kunt u het gebruik van klanten ook op de volgende manieren controleren.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="ddb4b-111">Deze opties kunnen u helpen bij het herkennen van onjuist geconfigureerde services of ongebruikelijke trends die fraude kunnen voorstellen.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="ddb4b-112">Vervolgens kunt u met uw klanten samenwerken om de hoofdoorzaak te achterhalen en de kosten te beheren.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="ddb4b-113">Indien nodig kunt u ook [het budget van de klant wijzigen](#set-azure-spending-budget) in een hoger bedrag.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="ddb4b-114">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="ddb4b-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="ddb4b-115">E-mailmeldingen in te stellen voor wanneer de uitgaven van een klant de budgetlimiet bijna hebben bereikt</span><span class="sxs-lookup"><span data-stu-id="ddb4b-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="ddb4b-116">Gespecificeerde kosten per service weergeven voor abonnementen op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="ddb4b-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="ddb4b-117">U kunt ook [op elk moment een Azure-uitgavenbudget](#remove-azure-spending-budget) voor klanten verwijderen.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="ddb4b-118">Azure-bestedingsgegevens</span><span class="sxs-lookup"><span data-stu-id="ddb4b-118">Azure spending data</span></span>

<span data-ttu-id="ddb4b-119">De Azure-bestedingsgegevens zijn *een schatting* en *de werkelijke factureringsbedragen kunnen variëren.*</span><span class="sxs-lookup"><span data-stu-id="ddb4b-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="ddb4b-120">De waarde van de gegevens *weerspiegelt geen belastingen,* tegoeden, aanpassingen of andere kosten die van toepassing kunnen zijn.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="ddb4b-121">De bestedingsgegevens *worden eenmaal per dag vernieuwd.*</span><span class="sxs-lookup"><span data-stu-id="ddb4b-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="ddb4b-122">Uw klanten kunnen Azure-services en -resources blijven gebruiken (en in rekening worden gebracht), tenzij u de accountinstellingen wijzigt in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="ddb4b-123">Azure-uitgavenbudget instellen</span><span class="sxs-lookup"><span data-stu-id="ddb4b-123">Set Azure spending budget</span></span>

<span data-ttu-id="ddb4b-124">U kunt *een maandelijks Azure-uitgavenbudget instellen* voor meerdere klanten in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="ddb4b-125">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ddb4b-126">Kies in het menu aan de linkerkant onder **CSP** de optie **Azure-uitgaven.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ddb4b-127">Selecteer op de azure-bestedingspagina **onder Klanten Microsoft Azure abonnementen** de klant(en) voor wie u een budget wilt instellen. </span><span class="sxs-lookup"><span data-stu-id="ddb4b-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="ddb4b-128">Voer een waarde in voor **Maandelijks budget**.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="ddb4b-129">Kies **Toepassen om** uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="ddb4b-130">U kunt ook *een budget instellen voor een afzonderlijke klant* in de abonnementsinstellingen:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="ddb4b-131">Meld u aan bij het dashboard van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="ddb4b-132">Kies in het menu aan de linkerkant onder **CSP** de optie **Klanten**.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ddb4b-133">Selecteer op **de** pagina Klanten de bedrijfsnaam van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ddb4b-134">Kies op de pagina **Abonnementen van de** klant onder Abonnement op basis van **gebruik** de optie **Budget wijzigen.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="ddb4b-135">Voer een waarde in voor het budget.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="ddb4b-136">Kies **Toepassen om** uw wijzigingen op te slaan.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="ddb4b-137">Azure-bestedingsbudget verwijderen</span><span class="sxs-lookup"><span data-stu-id="ddb4b-137">Remove Azure spending budget</span></span>

<span data-ttu-id="ddb4b-138">U kunt *een maandelijks Azure-uitgavenbudget* voor uw klanten verwijderen in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="ddb4b-139">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ddb4b-140">Kies in het menu aan de linkerkant onder **CSP** de optie **Azure-uitgaven.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ddb4b-141">Selecteer op de azure-bestedingspagina **onder Klanten Microsoft Azure abonnementen** de klant(s) waarvan u het budget wilt verwijderen. </span><span class="sxs-lookup"><span data-stu-id="ddb4b-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="ddb4b-142">Kies **Budget verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="ddb4b-143">Huidige Azure-uitgaven controleren</span><span class="sxs-lookup"><span data-stu-id="ddb4b-143">Check current Azure spending</span></span>

<span data-ttu-id="ddb4b-144">U kunt *de huidige Azure-uitgaven en maandelijkse* budgetten van uw klanten op elk moment bijhouden:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="ddb4b-145">Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ddb4b-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ddb4b-146">Kies in het menu aan de linkerkant onder **CSP** de optie **Azure-uitgaven.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="ddb4b-147">Op  de Azure-bestedingspagina, onder **Klanten met Microsoft Azure-abonnementen,** ziet u een overzicht van de maandelijkse budgetten van klanten, de huidige bestedingsschattingen en het percentage van het gebruikte budget.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="ddb4b-148">Meldingen voor budgetlimieten</span><span class="sxs-lookup"><span data-stu-id="ddb4b-148">Notifications for budget limits</span></span>

<span data-ttu-id="ddb4b-149">U kunt *e-mailmeldingen in instellen* wanneer de maandelijkse uitgaven van uw klant de budgetlimiet bijna hebben bereikt.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="ddb4b-150">Wanneer u deze optie in gebruik neemt, krijgt u een melding wanneer klanten 80% of meer van hun maandelijkse budget gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="ddb4b-151">Met deze optie kunt u uw Azure-factuur in de gaten houden.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="ddb4b-152">E-mailmeldingen configureren:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-152">To configure email notifications:</span></span>

1. <span data-ttu-id="ddb4b-153">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ddb4b-154">Ga naar **Settings**.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="ddb4b-155">Selecteer **Mijn voorkeuren.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="ddb4b-156">Configureer een voorkeurs-e-mailadres als u dat nog niet hebt.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="ddb4b-157">Configureer de voorkeurstaal voor de melding.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="ddb4b-158">Selecteer **het tabblad CSP** onder **de sectie Meldingsvoorkeuren.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="ddb4b-159">Controleer de optie E-mail **voor azure-bestedingsmeldingen** en sla **op.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="ddb4b-160">Gespecificeerde kosten per service</span><span class="sxs-lookup"><span data-stu-id="ddb4b-160">Itemized costs by service</span></span>

<span data-ttu-id="ddb4b-161">U kunt *gespecificeerde kosten (en geschat gebruik) per service weergeven voor* abonnementen op basis van gebruik:</span><span class="sxs-lookup"><span data-stu-id="ddb4b-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="ddb4b-162">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="ddb4b-163">Kies klanten in het menu aan de linkerkant **onder** **CSP**.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="ddb4b-164">Selecteer op **de** pagina Klanten de bedrijfsnaam van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="ddb4b-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="ddb4b-165">Selecteer op de pagina **Abonnementen van de** klant onder Abonnementen op basis van **gebruik** de naam van het **abonnement**.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="ddb4b-166">Op de pagina van het abonnement kunt u de gespecificeerde kosten **per** service en het **geschatte** gebruik voor de huidige maand bekijken.</span><span class="sxs-lookup"><span data-stu-id="ddb4b-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="ddb4b-167">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="ddb4b-167">Next steps</span></span>

- [<span data-ttu-id="ddb4b-168">Nieuwe Commerce-ervaring in CSP - Azure-facturering</span><span class="sxs-lookup"><span data-stu-id="ddb4b-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
