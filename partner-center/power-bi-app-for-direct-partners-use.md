---
title: Partner Center Analytics voor Power BI gebruiken
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het weer geven van uw zakelijke gegevens met behulp van de Partner Center Analytics-App voor Power BI (voor rechtstreekse partners in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633859"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="bfe7d-103">Uw bedrijfs gegevens weer geven met de Partner Center Analytics-App voor micro soft Power BI</span><span class="sxs-lookup"><span data-stu-id="bfe7d-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="bfe7d-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="bfe7d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bfe7d-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="bfe7d-105">Global admin</span></span>
- <span data-ttu-id="bfe7d-106">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="bfe7d-106">User management admin</span></span>
- <span data-ttu-id="bfe7d-107">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="bfe7d-107">Sales agent</span></span>
- <span data-ttu-id="bfe7d-108">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="bfe7d-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="bfe7d-109">Uw zakelijke gegevens weer geven</span><span class="sxs-lookup"><span data-stu-id="bfe7d-109">View your business data</span></span>

<span data-ttu-id="bfe7d-110">Maak een visuele representatie van uw bedrijfs gegevens met de Partner Center Analytics-App voor Power BI, met inbegrip van:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="bfe7d-111">De groei van uw klanten basis, abonnementen en licenties</span><span class="sxs-lookup"><span data-stu-id="bfe7d-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="bfe7d-112">Gebruik van Office 365-, micro soft Dynamics-en Microsoft Azure-producten</span><span class="sxs-lookup"><span data-stu-id="bfe7d-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="bfe7d-113">Dagelijkse verbruiks eenheden voor elke resource met data limiet in elk Azure-abonnement gedurende de afgelopen 60 dagen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="bfe7d-114">Geschatte kosten (op basis van de meest recente tarieven kaart)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="bfe7d-115">De mogelijkheid om gegevens sets te exporteren en aangepaste rapporten te maken, inclusief per klant.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="bfe7d-116">De preview-versie van app Center Analytics-apps</span><span class="sxs-lookup"><span data-stu-id="bfe7d-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="bfe7d-117">Deze app is alleen voor directe partners in het Cloud Solution Provider-programma.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="bfe7d-118">Andere partners in CSP (bijvoorbeeld indirecte wederverkopers) kunnen zich niet aanmelden.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="bfe7d-119">Alle geschatte kosten zijn facturen voor facturering/factuur vooraf en zijn niet juridisch bindend.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="bfe7d-120">Geschatte kosten zijn alleen bedoeld voor gebruik voor data Insights.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="bfe7d-121">Klant gegevens zijn gebaseerd op abonnementen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="bfe7d-122">Klanten waarvoor u onlangs accounts hebt gemaakt, maar die nog geen abonnementen hebben, worden niet opgenomen in aantallen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="bfe7d-123">De geschatte kosten zijn gebaseerd op de meest recente tarief kaart, die is gebaseerd op CSP-prijzen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="bfe7d-124">Dagen zijn kalender dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="bfe7d-125">Rapport van Business Insights</span><span class="sxs-lookup"><span data-stu-id="bfe7d-125">Business Insights report</span></span>

- <span data-ttu-id="bfe7d-126">**Tenants van klanten**: aantal afzonderlijke Azure AD-tenants van klanten die hebben gekochte abonnementen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="bfe7d-127">**Nieuw (afgelopen 30 dagen)**: nieuwe klanten die in de afgelopen 30 dagen ten minste één abonnement kopen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="bfe7d-128">**Verloop (afgelopen 30 dagen)**: klanten zonder ' Active ', ' in respijt ' of ' uitgeschakelde ' abonnementen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="bfe7d-129">**Nieuw (afgelopen 24 uur)**: nieuwe klanten hebben ten minste één abonnement in de afgelopen 24 uur kopen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="bfe7d-130">**Geschatte maandelijkse kosten gedurende de afgelopen 12 maanden**: maand over maand trend van het geschatte vooraf-BTW-factuur bedrag, geaggregeerd maandelijks voor de periode van afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="bfe7d-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bfe7d-131">**Geschatte kosten per product gedurende een periode van 12 maanden**: verkochte producten, gesorteerd op basis van het geschatte bedrag vóór de BTW-factuur, geaggregeerd over de periode van de afgelopen 12 maanden.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="bfe7d-132">Deze status geeft aan dat de belangrijkste producten de meeste omzet.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="bfe7d-133">**Klanten in de afgelopen 12 maanden**: maand over maand trend van nieuwe klanten en verloop klanten die maandelijks zijn geaggregeerd over de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="bfe7d-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bfe7d-134">**Geschatte kosten per klant gedurende de afgelopen 12 maanden**: klanten gesorteerd op geschat bedrag factuur vooraf BTW, geaggregeerd over de periode van afgelopen 12 maanden.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="bfe7d-135">Deze status geeft aan dat de belangrijkste klanten de meeste omzet.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="bfe7d-136">**Aantal klanten per product**: verkochte producten gesorteerd op gekoppelde klanten.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="bfe7d-137">Deze status duidt op de belangrijkste producten die aan de meeste klanten worden verkocht.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="bfe7d-138">Rapport met abonnement Insights</span><span class="sxs-lookup"><span data-stu-id="bfe7d-138">Subscription Insights report</span></span>

- <span data-ttu-id="bfe7d-139">**Abonnements status**:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-139">**Subscription status**:</span></span>

- <span data-ttu-id="bfe7d-140">Actief: abonnementen die horen bij de status ' actief ' of ' in de respijt periode '</span><span class="sxs-lookup"><span data-stu-id="bfe7d-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="bfe7d-141">Onderbroken: abonnementen die horen bij de status ' uitgeschakeld '</span><span class="sxs-lookup"><span data-stu-id="bfe7d-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="bfe7d-142">Niet-ingericht: abonnementen die horen bij de status ' niet-ingericht ' of ' verlopen '</span><span class="sxs-lookup"><span data-stu-id="bfe7d-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="bfe7d-143">**Verloop status**:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-143">**Expiry status**:</span></span>

  - <span data-ttu-id="bfe7d-144">Verlopen: abonnementen die al zijn verlopen (waarbij de eind datum van het abonnement in het verleden ligt)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="bfe7d-145">Verlopen na 30 dagen: abonnementen die na 30 dagen verlopen (waarbij de eind datum van het abonnement na de volgende 30 dagen valt)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="bfe7d-146">Verloopt over 30 dagen: abonnementen die binnen de komende 30 dagen verlopen (waarbij de eind datum van het abonnement tussen vandaag en de volgende 30 dagen ligt)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="bfe7d-147">**Totaal aantal abonnementen**: abonnementen in actief, in de respijt periode of de status uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="bfe7d-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="bfe7d-148">**Nieuw (afgelopen 30 dagen)**: nieuwe abonnementen die klanten in de afgelopen 30 dagen zijn aangeschaft</span><span class="sxs-lookup"><span data-stu-id="bfe7d-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="bfe7d-149">**Nieuw (afgelopen 24 uur)**: nieuwe abonnementen die klanten in de afgelopen 24 uur zijn aangeschaft</span><span class="sxs-lookup"><span data-stu-id="bfe7d-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="bfe7d-150">**Verloopt over 30 dagen**: abonnementen die binnen de komende 30 dagen verlopen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="bfe7d-151">**Verloop (afgelopen 30 dagen)**: abonnementen die in de afgelopen 30 dagen zijn uitgezet of geblokkeerd (uitgeschakeld)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="bfe7d-152">**Distributie per abonnements** type:% distributie van het totale aantal abonnementen per licentie op basis van en op gebruik gebaseerd abonnement</span><span class="sxs-lookup"><span data-stu-id="bfe7d-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="bfe7d-153">**Aantal actieve abonnementen per product**: verkochte producten gesorteerd op actief aantal abonnementen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="bfe7d-154">**Abonnementen over de afgelopen 12 maanden**: maand over maand trend van nieuwe abonnementen en verloop abonnementen die maandelijks worden geaggregeerd over de periode van afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="bfe7d-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bfe7d-155">**Details van klant abonnement**: gedetailleerd overzicht van de klanten, abonnementen en aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="bfe7d-156">Licentie Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-156">License Insights report:</span></span>

- <span data-ttu-id="bfe7d-157">**Totale licenties**: totaal aantal licenties dat is geaggregeerd op alle abonnementen op basis van licenties</span><span class="sxs-lookup"><span data-stu-id="bfe7d-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="bfe7d-158">**Nieuw (afgelopen 30 dagen)**: licentie toevoeging binnen de afgelopen 30 dagen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="bfe7d-159">**Verloop (laatste 30 dagen)**: licentie reductie binnen de afgelopen 30 dagen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="bfe7d-160">**Nieuw (afgelopen 24 uur)**: licentie toevoeging in de afgelopen 24 uur</span><span class="sxs-lookup"><span data-stu-id="bfe7d-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="bfe7d-161">**Licenties gedurende de afgelopen 90 dagen**: maand over maand trend van licentie toevoegingen en kortingen die maandelijks worden geaggregeerd over de periode van afgelopen 90 dagen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="bfe7d-162">**Aantal actieve licenties per product**: verkochte producten gesorteerd op aantal actieve licenties</span><span class="sxs-lookup"><span data-stu-id="bfe7d-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="bfe7d-163">**Aantal actieve licenties per klant**: klanten gesorteerd op aantal actieve licenties</span><span class="sxs-lookup"><span data-stu-id="bfe7d-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="bfe7d-164">**Details van de klant licentie gebeurtenis gedurende de afgelopen 90 dagen**: gedetailleerde weer gave van de evenementen klanten, abonnementen en abonnementen, waaronder gebeurtenis datum, gebeurtenis naam, hoeveelheid en wijziging in hoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="bfe7d-165">Gebruiks rapport licenties:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-165">Licenses Usage report:</span></span>

- <span data-ttu-id="bfe7d-166">**Licenties die zijn toegewezen door product**: verkochte producten gesorteerd op aantal licenties toewijzingen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="bfe7d-167">**Licenties die worden gebruikt door product**: verkochte producten gesorteerd op aantal licenties gebruik</span><span class="sxs-lookup"><span data-stu-id="bfe7d-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="bfe7d-168">**Klant distributie van verleende licenties**:% distributie van totaal aantal klanten verbroken in buckets van 20% bereik per licentie toewijzing%</span><span class="sxs-lookup"><span data-stu-id="bfe7d-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="bfe7d-169">**Klant distributie van in gebruik** zijnde licenties:% distributie van totaal aantal klanten die zijn gebroken in buckets met een licentie gebruik%</span><span class="sxs-lookup"><span data-stu-id="bfe7d-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="bfe7d-170">**Licenties die zijn toegewezen door de klant**: gedetailleerde weer gave van licenties die worden verkocht en licenties die zijn toegewezen door klanten en producten</span><span class="sxs-lookup"><span data-stu-id="bfe7d-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="bfe7d-171">**Licenties die worden gebruikt door de klant**: gedetailleerde weer gave van licenties die worden verkocht en licenties die worden gebruikt door klanten en producten</span><span class="sxs-lookup"><span data-stu-id="bfe7d-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="bfe7d-172">Azure Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-172">Azure Insights report:</span></span>

- <span data-ttu-id="bfe7d-173">**Klanten op basis van gebruik gedurende de afgelopen 12 maanden**: maand over maand trend van nieuwe op gebruik gebaseerde klanten en klanten die zijn gebaseerd op het gebruik van getijden op basis van verbruik, zijn maandelijks geaggregeerd over de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="bfe7d-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bfe7d-174">**Op gebruik gebaseerde abonnementen gedurende de afgelopen 12 maanden**: maand over maand trend van nieuwe op gebruik gebaseerde abonnementen en gespreide, op basis van gebruik geplaatste abonnementen maandelijks voor de periode van afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="bfe7d-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="bfe7d-175">**Geschatte kosten voor gebruik door de klant gedurende de afgelopen 60 dagen**: op gebruik gebaseerde klanten, gesorteerd op geschat bedrag factuur vooraf BTW, geaggregeerd over de periode van afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="bfe7d-176">Deze status geeft aan dat klanten op het hoogste gebruik de meeste omzet</span><span class="sxs-lookup"><span data-stu-id="bfe7d-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="bfe7d-177">**Geschatte kosten van gebruik per categorie gedurende de afgelopen 60 dagen**: meter categorieën van op gebruik gebaseerde abonnementen, gesorteerd op het geschatte bedrag vóór de BTW-factuur, geaggregeerd over de periode van de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="bfe7d-178">**Geschatte kosten voor gebruik per abonnement gedurende de afgelopen 60 dagen**: op gebruik gebaseerde abonnementen op geraamde pre-BTW factuur bedrag, geaggregeerd over de periode van de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="bfe7d-179">**Geschatte gebruiks kosten van klanten per uitgaven budget**: klanten die zijn gesorteerd op percentage van hun huidige bestedings budget overschrijden de drempel waarde (100%).</span><span class="sxs-lookup"><span data-stu-id="bfe7d-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="bfe7d-180">Azure resource gebruik-rapport:</span><span class="sxs-lookup"><span data-stu-id="bfe7d-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="bfe7d-181">**Gebruik van Azure-resources per dag voor de geselecteerde periode**: dagelijks verbruiks eenheden voor elke resource met data limiet in elk op gebruik gebaseerd abonnement voor geselecteerde periode in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="bfe7d-182">**Geschatte gebruiks kosten van Azure-resources voor de geselecteerde periode**: geschatte kosten op basis van de meest recente tarieven kaart voor elke resource met een licentie in elk op gebruik gebaseerd abonnement voor geselecteerde periode in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="bfe7d-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bfe7d-183">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="bfe7d-183">Next steps</span></span>

- [<span data-ttu-id="bfe7d-184">Overzicht van partner Center Analytics for Power BI-app</span><span class="sxs-lookup"><span data-stu-id="bfe7d-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- <span data-ttu-id="bfe7d-185">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Partner Center Analytics-app voor Microsoft Power BI installeren en preview bekijken)</span><span class="sxs-lookup"><span data-stu-id="bfe7d-185">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md)</span></span>
