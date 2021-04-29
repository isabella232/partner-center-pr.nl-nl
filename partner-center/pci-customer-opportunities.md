---
title: Partner Center Insights - CloudAscent Propensity-rapporten
description: Meer informatie over de CloudAscent Propensity-rapporten in Partner Center. Bevat informatie over de reensiteit van een klant om Microsoft-producten te kopen.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213437"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="d3106-104">CloudAscent Propensity-rapporten die beschikbaar zijn via Partner Center dashboard</span><span class="sxs-lookup"><span data-stu-id="d3106-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="d3106-105">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="d3106-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d3106-106">Rapportviewer voor leidinggevenden</span><span class="sxs-lookup"><span data-stu-id="d3106-106">Executive report viewer</span></span>
- <span data-ttu-id="d3106-107">Rapportviewer</span><span class="sxs-lookup"><span data-stu-id="d3106-107">Report viewer</span></span>

<span data-ttu-id="d3106-108">Het Partner Center dashboard bevat downloadbare propensiteitsgegevens uit het CloudAscent-programma.</span><span class="sxs-lookup"><span data-stu-id="d3106-108">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="d3106-109">De gegevens tonen de kans van klanten om Microsoft-producten te kopen.</span><span class="sxs-lookup"><span data-stu-id="d3106-109">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="d3106-110">In dit artikel wordt de uitsplitsing van deze gegevens beschreven, hoe u de score gebruikt en wat het betekent.</span><span class="sxs-lookup"><span data-stu-id="d3106-110">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="d3106-111">Samenvattingsdefinities</span><span class="sxs-lookup"><span data-stu-id="d3106-111">Summary definitions</span></span>

- <span data-ttu-id="d3106-112">**SMC-klanten:** dit is het totale aantal klanten in de smc-downloads.</span><span class="sxs-lookup"><span data-stu-id="d3106-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="d3106-113">Klanten worden geïdentificeerd door de recordpartner.</span><span class="sxs-lookup"><span data-stu-id="d3106-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="d3106-114">**Verlopen-overeenkomsten:** binnen het huidige fiscale jaar geven we het aantal verlopende overeenkomsten op.</span><span class="sxs-lookup"><span data-stu-id="d3106-114">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="d3106-115">**Open Expiring Revenue:** de omzet die is gekoppeld aan de openstaande verlopende overeenkomsten.</span><span class="sxs-lookup"><span data-stu-id="d3106-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Schermopname van het dashboard Verkoopkansen van klanten.":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="d3106-117">CloudAscent SMB-segmentatie</span><span class="sxs-lookup"><span data-stu-id="d3106-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="d3106-118">Het segment voor kleine tot middelgrote bedrijven (SMB) is onderverdeeld in drie afzonderlijke subsegmenten.</span><span class="sxs-lookup"><span data-stu-id="d3106-118">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="d3106-119">**Top Unmanaged** omvat de grootste SMB-klanten met de meeste mogelijkheden voor Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3106-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="d3106-120">Veel klanten die het meest worden beheerd, hebben vergelijkbare kenmerken als beheerde accounts, met een groot aantal werknemers, grote IT-budgetten en uitgaven en grote hoeveelheden potentiële omzet voor Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d3106-120">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="d3106-121">We definiëren Top Unmanaged op twee manieren:</span><span class="sxs-lookup"><span data-stu-id="d3106-121">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="d3106-122">**Belangrijkste niet-managed op basis van gebruikers:** bevat accounts met 300 of meer werknemers.</span><span class="sxs-lookup"><span data-stu-id="d3106-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="d3106-123">User-Based-accounts zijn geweldige doelen voor de eerste aankoop of uitbreiding van abonnementsproducten op basis van gebruikers, zoals Microsoft 365, Dynamics 365 of Surface.</span><span class="sxs-lookup"><span data-stu-id="d3106-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="d3106-124">**Belangrijkste onmanaged rekenkracht:** bevat accounts met een Azure-potentieel hoger dan $ 10.000.</span><span class="sxs-lookup"><span data-stu-id="d3106-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="d3106-125">Rekenaccounts omvatten bestaande Azure.</span><span class="sxs-lookup"><span data-stu-id="d3106-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="d3106-126">accounts met een aanzienlijk potentieel voor het komende jaar en accounts die Azure nog niet hebben aangeschaft, maar potentieel voor Azure groter zijn dan $ 10.000.</span><span class="sxs-lookup"><span data-stu-id="d3106-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="d3106-127">**Middelgrote bedrijven** omvatten bestaande klanten en prospectaccounts met 25 tot 300 werknemers.</span><span class="sxs-lookup"><span data-stu-id="d3106-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="d3106-128">**Kleine bedrijven** omvatten bedrijven met 10-25 werknemers.</span><span class="sxs-lookup"><span data-stu-id="d3106-128">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="d3106-129">**Zeer kleine bedrijven** zijn bedrijven met 1-9 werknemers.</span><span class="sxs-lookup"><span data-stu-id="d3106-129">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Klant op SMC-type.":::

<span data-ttu-id="d3106-131">**De belangrijkste subsegmenten Unmanaged** en **Medium Business** vertegenwoordigen klanten met een hoge levensduur (LTV) voor Microsoft en Microsoft-partners.</span><span class="sxs-lookup"><span data-stu-id="d3106-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="d3106-132">Daarom zijn ze de hoofdgebieden van de focus om de groei in dit segment te stimuleren.</span><span class="sxs-lookup"><span data-stu-id="d3106-132">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="d3106-133">In deze twee subsegmenten zijn we beter in staat om de socket te verkrijgen met Microsoft 365, verder geld te verdienen met D365-/Azure LOB-apps (Line-Of-Business) en een hoge LTV voor Microsoft te realiseren.</span><span class="sxs-lookup"><span data-stu-id="d3106-133">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="d3106-134">Op dit moment hebben we twee belangrijke gebieden van kansen: 1.</span><span class="sxs-lookup"><span data-stu-id="d3106-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="d3106-135">onze klant voegt groei toe; 2.</span><span class="sxs-lookup"><span data-stu-id="d3106-135">our customer adds growth; 2.</span></span> <span data-ttu-id="d3106-136">hoewel we goed in staat zijn om cloudsockers te verkrijgen die Microsoft 365, hebben we een grote kans in Dynamics 365 en Azure.</span><span class="sxs-lookup"><span data-stu-id="d3106-136">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="d3106-137">De volgende schermopname vertegenwoordigt de vier SMB-subsegmenten.</span><span class="sxs-lookup"><span data-stu-id="d3106-137">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="d3106-138">CloudAscent prioriteert de profilering, score en modellering van alle niet-beherende en middelgrote zakelijke accounts.</span><span class="sxs-lookup"><span data-stu-id="d3106-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Schermopname van SMB-subsegmenten.":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="d3106-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="d3106-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="d3106-141">SMB maakt gebruik machine learning om voorspellingen van verkoop- en marketingklant binnen de segmenten Top Unmanaged en Medium Business te stimuleren.</span><span class="sxs-lookup"><span data-stu-id="d3106-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="d3106-142">Hoe worden signalen verzameld en omgezet in aanbevelingen voor goedheid?</span><span class="sxs-lookup"><span data-stu-id="d3106-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="d3106-143">**Gegevensverzameling:** web-crawlers scannen en verzamelen miljarden klantsignalen door de bedrijfsdomeinen te pingen en blogposts, releases, sociale streams en technische forums te bewaken.</span><span class="sxs-lookup"><span data-stu-id="d3106-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="d3106-144">Naast de verzamelde signalen worden er firmographics-gegevens verzameld uit zowel interne als externe bronnen, zoals D&B, een intern Microsoft-abonnement en transactionele gegevens.</span><span class="sxs-lookup"><span data-stu-id="d3106-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="d3106-145">**Machine Learning:** De signalen worden ingevoerd in het machine learning-model dat een gestructureerde gegevensset met verkoop- en marketingvoorspellingen voor elke klant op basis van een cloudproduct en cluster als uitvoer geeft.</span><span class="sxs-lookup"><span data-stu-id="d3106-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="d3106-146">Elke klant wordt op basis van een look-gelijk model scoren op de belangrijkste SMB van Microsoft die de Fit-algoritmen van de klant bepaalt, en machine learning-algoritmen die het onlinegedrag van de klant integreren, definiëren als Intentie.</span><span class="sxs-lookup"><span data-stu-id="d3106-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="d3106-147">De score wordt samengevoegd in clusters die laten zien dat een klant microsoft-cloudproducten wil kopen.</span><span class="sxs-lookup"><span data-stu-id="d3106-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="d3106-148">**Optimalisatie:** het Machine Learning optimaliseert de modellen door de transactiegegevens maandelijks en per kwartaal te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="d3106-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="d3106-149">Met behulp van de winst-/verliesgegevens past de Machine Learning de algoritmen aan en controleert deze of de modellen werken zoals verwacht door clusteraanbevelingen te vergelijken met verkoopkansen die in MSX zijn gebruikt.</span><span class="sxs-lookup"><span data-stu-id="d3106-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Schermopname van SMB machine learning.":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="d3106-151">CloudAscent Propensity</span><span class="sxs-lookup"><span data-stu-id="d3106-151">CloudAscent Propensity</span></span>

<span data-ttu-id="d3106-152">Hoe worden aanbevelingen voor aan-eigenheid gemaakt?</span><span class="sxs-lookup"><span data-stu-id="d3106-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="d3106-153">Met behulp van signalen die worden verzameld via web-crawlers en gegevens die afkomstig zijn uit verschillende bronnen, consolideren we de firmographics-gegevens en de signalen voor sociale media van de klant.</span><span class="sxs-lookup"><span data-stu-id="d3106-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="d3106-154">De score maakt gebruik van deze signalen en gegevens in vergelijkingsmodellen voor fit- en scoremodellen voor Intent.</span><span class="sxs-lookup"><span data-stu-id="d3106-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="d3106-155">Klantaccount aanpassen</span><span class="sxs-lookup"><span data-stu-id="d3106-155">Customer Account Fit</span></span>

   - <span data-ttu-id="d3106-156">Interne en externe gegevenspunten die firmographics definiëren.</span><span class="sxs-lookup"><span data-stu-id="d3106-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="d3106-157">Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft Cloud Products.</span><span class="sxs-lookup"><span data-stu-id="d3106-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="d3106-158">Passend scoren wordt elk kwartaal bijgewerkt</span><span class="sxs-lookup"><span data-stu-id="d3106-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="d3106-159">Intentie van klantaccount</span><span class="sxs-lookup"><span data-stu-id="d3106-159">Customer Account Intent</span></span>

   - <span data-ttu-id="d3106-160">Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie.</span><span class="sxs-lookup"><span data-stu-id="d3106-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="d3106-161">Het scoren van intenties wordt boven op fit om de clusters te definiëren.</span><span class="sxs-lookup"><span data-stu-id="d3106-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="d3106-162">Het scoren van intenties wordt maandelijks bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="d3106-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB-voorspellende modellen.":::

3. <span data-ttu-id="d3106-164">Clustering</span><span class="sxs-lookup"><span data-stu-id="d3106-164">Clustering</span></span>

   <span data-ttu-id="d3106-165">De signalen voor passend en intentie worden samengevoegd in een clusteringscore.</span><span class="sxs-lookup"><span data-stu-id="d3106-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="d3106-166">CloudAscent heeft vier clusters:</span><span class="sxs-lookup"><span data-stu-id="d3106-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="d3106-167">Nu actie ondernemen - klanten die klaar zijn voor verkoop</span><span class="sxs-lookup"><span data-stu-id="d3106-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="d3106-168">Evalueren - klanten die klaar zijn voor marketing</span><span class="sxs-lookup"><span data-stu-id="d3106-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="d3106-169">Ouverture - bewustzijnscampagnes aandurveren</span><span class="sxs-lookup"><span data-stu-id="d3106-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="d3106-170">Opleiden : intenties opleiden en controleren</span><span class="sxs-lookup"><span data-stu-id="d3106-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="d3106-171">Met de clustering kunnen gebruikers zich richten op specifieke klanten voor verkoop- en marketinginitiatieven op basis van segmentfactoren, bijvoorbeeld: product, geo, branche en verticaal.</span><span class="sxs-lookup"><span data-stu-id="d3106-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="d3106-172">Het **tabblad Propensity-model** in de CloudAscent Workbooks deelt de reactiviteit en de geschatte witruimte-omzet.</span><span class="sxs-lookup"><span data-stu-id="d3106-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="d3106-173">Voor het definiëren van de clustering van Fit and Intent doorlopen we de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="d3106-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="d3106-174">Met behulp van ML-modellen berekenen we eerst de score en intentiescore van Customer Fit op een schaal van 100.</span><span class="sxs-lookup"><span data-stu-id="d3106-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="d3106-175">Exacte scores variëren op basis van ML-modellen.</span><span class="sxs-lookup"><span data-stu-id="d3106-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="d3106-176">Voorbeeldscores hieronder:</span><span class="sxs-lookup"><span data-stu-id="d3106-176">Example Scores Below:</span></span>

         |<span data-ttu-id="d3106-177">**Classificatie**</span><span class="sxs-lookup"><span data-stu-id="d3106-177">**Classification**</span></span>|<span data-ttu-id="d3106-178">**Score**</span><span class="sxs-lookup"><span data-stu-id="d3106-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="d3106-179">Hoog</span><span class="sxs-lookup"><span data-stu-id="d3106-179">High</span></span>|<span data-ttu-id="d3106-180">75 - 100</span><span class="sxs-lookup"><span data-stu-id="d3106-180">75 - 100</span></span>|
         |<span data-ttu-id="d3106-181">Normaal</span><span class="sxs-lookup"><span data-stu-id="d3106-181">Medium</span></span>|<span data-ttu-id="d3106-182">55 - 74</span><span class="sxs-lookup"><span data-stu-id="d3106-182">55 - 74</span></span>|
         |<span data-ttu-id="d3106-183">Beperkt</span><span class="sxs-lookup"><span data-stu-id="d3106-183">Low</span></span>|<span data-ttu-id="d3106-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="d3106-184">30 - 54</span></span>|
         |<span data-ttu-id="d3106-185">Zeer laag</span><span class="sxs-lookup"><span data-stu-id="d3106-185">Very Low</span></span>|<span data-ttu-id="d3106-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="d3106-186">0 - 29</span></span>|

      2. <span data-ttu-id="d3106-187">Met behulp van de bovenstaande regel classificeren we bedrijven als Hoog, Gemiddeld, Laag en Zeer laag voor zowel Klantfitte als Intentiesignalen.</span><span class="sxs-lookup"><span data-stu-id="d3106-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="d3106-188">We plotten signalen over de passen van klanten en intenties op een 2D-matrix met elk snijpunt dat de achterheid vertegenwoordigt.</span><span class="sxs-lookup"><span data-stu-id="d3106-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="d3106-189">Bijvoorbeeld High Fit + High Intent = A1, die de hoogste reensiteit vertegenwoordigt.</span><span class="sxs-lookup"><span data-stu-id="d3106-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="d3106-190">Ten slotte worden deze segmenten gegroepeerd om clusters te vormen.</span><span class="sxs-lookup"><span data-stu-id="d3106-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="d3106-191">Zo vormen A1, A2, A3 en A4 het cluster Nu reageren.</span><span class="sxs-lookup"><span data-stu-id="d3106-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent-modellen.":::

   <span data-ttu-id="d3106-193">Voor deze klanten wordt u aangeraden zich te richten op Nu handelen en Klanten evalueren.</span><span class="sxs-lookup"><span data-stu-id="d3106-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="d3106-194">CloudAscent Products & modellen</span><span class="sxs-lookup"><span data-stu-id="d3106-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="d3106-195">De volgende afbeelding geeft een weergave van elk ondersteuningsmodel in CloudAscent:</span><span class="sxs-lookup"><span data-stu-id="d3106-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent propensity-model.":::

<span data-ttu-id="d3106-197">Witruimtemodellen bestaan uit voorspellingen voor bestaande Microsoft-klanten waar ze geen product hebben en/of net nieuwe prospectklanten zijn.</span><span class="sxs-lookup"><span data-stu-id="d3106-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="d3106-198">Bij upsell-modellen worden transactiegegevens gebruikt om de kans op upsell in Azure te voorspellen en Microsoft 365 SKU's.</span><span class="sxs-lookup"><span data-stu-id="d3106-198">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="d3106-199">Deze klanten hebben al zowel Azure als Microsoft 365 en het upsell-model laat zien dat ze waarschijnlijk meer van hun bestaande SKU zullen aanschaffen.</span><span class="sxs-lookup"><span data-stu-id="d3106-199">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="d3106-200">EOS deelt de EOS-klanten (end-of-service) voor Win 7, Office 2010, SQL Server en Windows Server.</span><span class="sxs-lookup"><span data-stu-id="d3106-200">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="d3106-201">De EOS-gegevens worden uit MS Sales gehaald en waar beschikbaar over de CloudAscent-propensiteitsmodelleren heen getrokken.</span><span class="sxs-lookup"><span data-stu-id="d3106-201">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="d3106-202">EOS-gegevens zijn te zien in Modern Work en Azure Sales.</span><span class="sxs-lookup"><span data-stu-id="d3106-202">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
