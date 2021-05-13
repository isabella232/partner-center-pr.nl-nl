---
title: Gebruik Partner Center Analytics voor Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het weergeven van uw zakelijke gegevens met behulp van Analyse-app van het Partnercentrum voor Power BI (voor directe partners in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855026"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="c74c9-103">Uw zakelijke gegevens weergeven met de Partner Center Analytics-app voor Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="c74c9-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="c74c9-104">**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Verkoopagent | Beheeragent</span><span class="sxs-lookup"><span data-stu-id="c74c9-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="c74c9-105">Uw bedrijfsgegevens weergeven</span><span class="sxs-lookup"><span data-stu-id="c74c9-105">View your business data</span></span>

<span data-ttu-id="c74c9-106">Krijg een visuele weergave van uw zakelijke gegevens met de Analyse-app van het Partnercentrum voor Power BI, waaronder:</span><span class="sxs-lookup"><span data-stu-id="c74c9-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="c74c9-107">Groei van uw klantenbestand, abonnementen en licenties</span><span class="sxs-lookup"><span data-stu-id="c74c9-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="c74c9-108">Gebruik van Office 365-, Microsoft Dynamics- en Microsoft Azure producten</span><span class="sxs-lookup"><span data-stu-id="c74c9-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="c74c9-109">Dagelijkse verbruikseenheden voor elke resource naar gebruik in elk Azure-abonnement voor de afgelopen 60 dagen</span><span class="sxs-lookup"><span data-stu-id="c74c9-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="c74c9-110">Geschatte kosten (op basis van de meest recente tariefkaart)</span><span class="sxs-lookup"><span data-stu-id="c74c9-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="c74c9-111">Mogelijkheid om gegevenssets te exporteren en aangepaste rapporten te maken, inclusief per klant.</span><span class="sxs-lookup"><span data-stu-id="c74c9-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="c74c9-112">Over de preview Partner Center versie van de app Partner Center Analytics</span><span class="sxs-lookup"><span data-stu-id="c74c9-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="c74c9-113">Deze app is alleen voor directe partners in Cloud Solution Provider programma.</span><span class="sxs-lookup"><span data-stu-id="c74c9-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="c74c9-114">Andere partners in CSP (indirecte resellers, bijvoorbeeld) kunnen zich niet aanmelden.</span><span class="sxs-lookup"><span data-stu-id="c74c9-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="c74c9-115">Geschatte kosten zijn facturerings-/factuurgegevens vóór belasting en zijn niet juridisch binding.</span><span class="sxs-lookup"><span data-stu-id="c74c9-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="c74c9-116">Geschatte kosten zijn alleen bedoeld om te worden gebruikt voor gegevensinzichten.</span><span class="sxs-lookup"><span data-stu-id="c74c9-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="c74c9-117">Klantgegevens zijn gebaseerd op abonnementen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="c74c9-118">Klanten voor wie u onlangs accounts hebt gemaakt, maar die nog geen abonnementen hebben, worden niet opgenomen in tellingen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="c74c9-119">De geschatte kosten zijn gebaseerd op de meest recente tariefkaart, die is gebaseerd op CSP-prijzen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="c74c9-120">Dagen zijn kalenderdagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="c74c9-121">Business Insights-rapport</span><span class="sxs-lookup"><span data-stu-id="c74c9-121">Business Insights report</span></span>

- <span data-ttu-id="c74c9-122">**Tenants van klanten:** aantal afzonderlijke Azure AD-tenants van klanten die abonnementen hebben aangeschaft</span><span class="sxs-lookup"><span data-stu-id="c74c9-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="c74c9-123">**Nieuw (afgelopen 30 dagen)**: Nieuwe klanten hebben in de afgelopen 30 dagen ten minste één abonnement aanschaffen</span><span class="sxs-lookup"><span data-stu-id="c74c9-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="c74c9-124">**Verloop (afgelopen 30 dagen)**: Klanten zonder abonnementen 'actief', 'in respijt' of 'uitgeschakeld'.</span><span class="sxs-lookup"><span data-stu-id="c74c9-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="c74c9-125">**Nieuw (afgelopen 24 uur)**: Nieuwe klanten hebben in de afgelopen 24 uur ten minste één abonnement aanschaffen</span><span class="sxs-lookup"><span data-stu-id="c74c9-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="c74c9-126">**Geschatte maandelijkse kosten in** de afgelopen 12 maanden: Trend in maand van geschatte factuurbedrag vóór belasting, samengevoegd maandelijks in de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="c74c9-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c74c9-127">**Geschatte kosten per product in** de afgelopen 12 maanden: verkochte producten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 12 maanden.</span><span class="sxs-lookup"><span data-stu-id="c74c9-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="c74c9-128">Deze status geeft aan dat de belangrijkste producten de meeste omzet opleveren.</span><span class="sxs-lookup"><span data-stu-id="c74c9-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="c74c9-129">**Klanten in de afgelopen 12** maanden: Trend van nieuwe klanten en verloopklanten per maand gedurende de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="c74c9-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c74c9-130">**Geschatte kosten per klant in** de afgelopen 12 maanden: Klanten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 12 maanden.</span><span class="sxs-lookup"><span data-stu-id="c74c9-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="c74c9-131">Deze status geeft aan dat de belangrijkste klanten de meeste omzet genereren.</span><span class="sxs-lookup"><span data-stu-id="c74c9-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="c74c9-132">**Aantal klanten per product:** verkochte producten gesorteerd op gekoppelde klanten.</span><span class="sxs-lookup"><span data-stu-id="c74c9-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="c74c9-133">Deze status geeft de belangrijkste producten aan die aan de meeste klanten zijn verkocht.</span><span class="sxs-lookup"><span data-stu-id="c74c9-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="c74c9-134">Abonnementsinzichten-rapport</span><span class="sxs-lookup"><span data-stu-id="c74c9-134">Subscription Insights report</span></span>

- <span data-ttu-id="c74c9-135">**Abonnementsstatus:**</span><span class="sxs-lookup"><span data-stu-id="c74c9-135">**Subscription status**:</span></span>

- <span data-ttu-id="c74c9-136">Actief: Abonnementen die behoren tot de status Actief of In respijtperiode</span><span class="sxs-lookup"><span data-stu-id="c74c9-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="c74c9-137">Tijdelijk: Abonnementen die behoren tot de status Uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="c74c9-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="c74c9-138">De-provisioned: Abonnementen die behoren tot de status 'de-provisioned' of 'expired'</span><span class="sxs-lookup"><span data-stu-id="c74c9-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="c74c9-139">**Verloopstatus:**</span><span class="sxs-lookup"><span data-stu-id="c74c9-139">**Expiry status**:</span></span>

  - <span data-ttu-id="c74c9-140">Verlopen: Abonnementen die al zijn verlopen (waarbij de einddatum van het abonnement in het verleden ligt)</span><span class="sxs-lookup"><span data-stu-id="c74c9-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="c74c9-141">Verloopt na 30 dagen: Abonnementen die na 30 dagen verlopen (waarbij de einddatum van het abonnement na de volgende 30 dagen valt)</span><span class="sxs-lookup"><span data-stu-id="c74c9-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="c74c9-142">Verloopt binnen 30 dagen: Abonnementen die binnen de volgende 30 dagen verlopen (waarbij de einddatum van het abonnement tussen vandaag en de volgende 30 dagen ligt)</span><span class="sxs-lookup"><span data-stu-id="c74c9-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="c74c9-143">**Totaal aantal abonnementen:** Abonnementen met de status Actief, In respijtperiode of Uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="c74c9-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="c74c9-144">**Nieuw (afgelopen 30 dagen)**: Nieuwe abonnementen die zijn gekocht door klanten in de afgelopen 30 dagen</span><span class="sxs-lookup"><span data-stu-id="c74c9-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="c74c9-145">**Nieuw (afgelopen 24 uur)**: Nieuwe abonnementen die zijn gekocht door klanten in de afgelopen 24 uur</span><span class="sxs-lookup"><span data-stu-id="c74c9-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="c74c9-146">**Verloopt over 30 dagen:** abonnementen die binnen de komende 30 dagen verlopen</span><span class="sxs-lookup"><span data-stu-id="c74c9-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="c74c9-147">**Verloop (afgelopen 30 dagen)**: Abonnementen die de inrichting in de afgelopen 30 dagen zijn beëindigd of tijdelijk zijn beëindigd (uitgeschakeld)</span><span class="sxs-lookup"><span data-stu-id="c74c9-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="c74c9-148">**Distributie op abonnementstypen:**% distributie van het totale aantal abonnementen op basis van licenties en abonnementstypen op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="c74c9-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="c74c9-149">**Aantal actieve abonnementen per product:** verkochte producten gesorteerd op aantal actieve abonnementen</span><span class="sxs-lookup"><span data-stu-id="c74c9-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="c74c9-150">**Abonnementen in de afgelopen 12** maanden: trend van maand tot maand voor nieuwe abonnementen en verloopabonnementen die maandelijks zijn samengevoegd in de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="c74c9-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c74c9-151">**Details van klantabonnement:** gedetailleerde weergave van de klanten, abonnementen en aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="c74c9-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="c74c9-152">License Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="c74c9-152">License Insights report:</span></span>

- <span data-ttu-id="c74c9-153">**Totaal aantal licenties:** totaal aantal licenties dat is geaggregeerd voor alle op licenties gebaseerde abonnementen</span><span class="sxs-lookup"><span data-stu-id="c74c9-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="c74c9-154">**Nieuw (afgelopen 30 dagen)**: Optelling van licentie in de afgelopen 30 dagen</span><span class="sxs-lookup"><span data-stu-id="c74c9-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="c74c9-155">**Verloop (afgelopen 30 dagen)**: Licentievermindering binnen de afgelopen 30 dagen</span><span class="sxs-lookup"><span data-stu-id="c74c9-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="c74c9-156">**Nieuw (afgelopen 24 uur)**: Optelling van licenties in de afgelopen 24 uur</span><span class="sxs-lookup"><span data-stu-id="c74c9-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="c74c9-157">**Licenties in de afgelopen 90** dagen: de trend van maandelijkse toevoegingen en verlagingen van licenties die maandelijks zijn geaggregeerd in de afgelopen 90 dagen</span><span class="sxs-lookup"><span data-stu-id="c74c9-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="c74c9-158">**Aantal actieve licenties per product:** verkochte producten gesorteerd op aantal actieve licenties</span><span class="sxs-lookup"><span data-stu-id="c74c9-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="c74c9-159">**Aantal actieve licenties per klant:** klanten gesorteerd op aantal actieve licenties</span><span class="sxs-lookup"><span data-stu-id="c74c9-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="c74c9-160">**Gebeurtenisdetails** van klantlicenties in de afgelopen 90 dagen: gedetailleerde weergave van de klanten, abonnementen en abonnementsgebeurtenissen, waaronder gebeurtenisdatum, gebeurtenisnaam, hoeveelheid en wijziging in hoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="c74c9-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="c74c9-161">Gebruiksrapport licenties:</span><span class="sxs-lookup"><span data-stu-id="c74c9-161">Licenses Usage report:</span></span>

- <span data-ttu-id="c74c9-162">**Licenties die zijn toegewezen per product:** verkochte producten gesorteerd op aantal licentietoewijzingen</span><span class="sxs-lookup"><span data-stu-id="c74c9-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="c74c9-163">**Licenties die worden gebruikt door product:** Verkochte producten gesorteerd op aantal licenties</span><span class="sxs-lookup"><span data-stu-id="c74c9-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="c74c9-164">**Klantdistributie van toegewezen** licenties: % distributie van het totale aantal klanten, opgesplitst in buckets van 20% bereik op licentietoewijzing %</span><span class="sxs-lookup"><span data-stu-id="c74c9-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="c74c9-165">**Klantdistributie van licenties in gebruik:**% distributie van het totale aantal klanten, opgesplitst in buckets van 20% bereik op licentiegebruik %</span><span class="sxs-lookup"><span data-stu-id="c74c9-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="c74c9-166">**Licenties die zijn toegewezen door de klant:** gedetailleerde weergave van verkochte licenties en licenties die zijn toegewezen door klanten en producten</span><span class="sxs-lookup"><span data-stu-id="c74c9-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="c74c9-167">**Licenties die door de klant worden gebruikt:** gedetailleerde weergave van verkochte licenties en licenties die worden gebruikt door klanten en producten</span><span class="sxs-lookup"><span data-stu-id="c74c9-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="c74c9-168">Azure Insights-rapport:</span><span class="sxs-lookup"><span data-stu-id="c74c9-168">Azure Insights report:</span></span>

- <span data-ttu-id="c74c9-169">Op gebruik gebaseerde klanten in de afgelopen **12** maanden: Trend van maandelijks nieuwe op gebruik gebaseerde klanten en op basis van verloop van gebruik gebaseerde klanten die maandelijks zijn geaggregeerd in de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="c74c9-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c74c9-170">Abonnementen op basis van gebruik in de afgelopen **12** maanden: trend van maand tot maand voor nieuwe op gebruik gebaseerde abonnementen en abonnementen op basis van verloop, maandelijks samengevoegd in de periode van de afgelopen 12 maanden</span><span class="sxs-lookup"><span data-stu-id="c74c9-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="c74c9-171">**Geschatte gebruikskosten** per klant in de afgelopen 60 dagen: op gebruik gebaseerde klanten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="c74c9-172">Deze status geeft aan dat de belangrijkste klanten op basis van gebruik de meeste omzet genereren</span><span class="sxs-lookup"><span data-stu-id="c74c9-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="c74c9-173">**Geschatte gebruikskosten per** categorie gedurende de afgelopen 60 dagen: Metercategorieën van op gebruik gebaseerde abonnementen gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="c74c9-174">**Geschatte gebruikskosten per** abonnement gedurende de afgelopen 60 dagen: Abonnementen op basis van gebruik op basis van geschatte factuurbedragen vóór belasting, geaggregeerd in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="c74c9-175">**Geschatte gebruikskosten van de klant op uitgavenbudget:** Klanten gesorteerd op percentage van hun huidige gebruiksbestedingsbudget dat de drempelwaarde overschrijdt (100%).</span><span class="sxs-lookup"><span data-stu-id="c74c9-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="c74c9-176">Rapport azure-resourcegebruik:</span><span class="sxs-lookup"><span data-stu-id="c74c9-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="c74c9-177">**Gebruik van Azure-resources per dag** voor de geselecteerde periode: dagelijkse verbruikseenheden voor elke resource naar gebruik in elk abonnement op basis van gebruik voor de geselecteerde periode in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="c74c9-178">**Geschatte gebruikskosten van Azure-resources** voor de geselecteerde periode: Geschatte kosten op basis van de kaart met het meest recente tarief voor elke resource naar gebruik in elk abonnement op basis van gebruik voor de geselecteerde periode in de afgelopen 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="c74c9-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c74c9-179">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="c74c9-179">Next steps</span></span>

- [<span data-ttu-id="c74c9-180">Partner Center Analytics voor Power BI-app</span><span class="sxs-lookup"><span data-stu-id="c74c9-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- <span data-ttu-id="c74c9-181">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Partner Center Analytics-app voor Microsoft Power BI installeren en preview bekijken)</span><span class="sxs-lookup"><span data-stu-id="c74c9-181">[Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md)</span></span>
