---
title: Facturering van Azure-abonnement-factuur & afstemmings bestanden
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de bestands structuur van de factuur en reconciliatie die betrekking heeft op facturering voor het Azure-abonnement.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658430"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="f116f-103">Nieuwe Commerce-ervaring in CSP - Azure-facturering</span><span class="sxs-lookup"><span data-stu-id="f116f-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="f116f-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="f116f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="f116f-105">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="f116f-105">Admin agent</span></span>
- <span data-ttu-id="f116f-106">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="f116f-106">Billing admin</span></span>
- <span data-ttu-id="f116f-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f116f-107">Global admin</span></span>

<span data-ttu-id="f116f-108">In dit artikel wordt uitgelegd hoe u de bestands structuur van de factuur en de reconciliatie voor het Azure-abonnement kunt openen en begrijpen.</span><span class="sxs-lookup"><span data-stu-id="f116f-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="f116f-109">Facturering onder het Azure-abonnement is een vereenvoudigde facturerings ervaring met behulp van een uitgelijnde enkele facturerings datum en facturerings periode op basis van een kalender maand.</span><span class="sxs-lookup"><span data-stu-id="f116f-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="f116f-110">Samen vatting van de basis beginselen van facturering</span><span class="sxs-lookup"><span data-stu-id="f116f-110">Summary of billing essentials</span></span>

- <span data-ttu-id="f116f-111">**Factuur datum**: factuur-en afstemmings bestand is beschikbaar in het dash board van de partner centrum/API door de achtste (middernacht UTC).</span><span class="sxs-lookup"><span data-stu-id="f116f-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="f116f-112">**Facturerings periode factuur**: de facturerings periode van de factuur is uitgelijnd op de kalender maand, bijvoorbeeld 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="f116f-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="f116f-113">**Kosten voor service perioden**: kosten worden uitgelijnd op de kalender maand.</span><span class="sxs-lookup"><span data-stu-id="f116f-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="f116f-114">Als er bijvoorbeeld een gefactureerde partner Azure-Services toevoegt via een Azure-abonnement op 10/15 en de klant begint met het verbruik van Azure-Services op 10/15, ontvangt de factuur dan op basis van het gebruik van facturen/afstemming op 11/8 voor klant verbruik voor de service periode 10/15-10/31.</span><span class="sxs-lookup"><span data-stu-id="f116f-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="f116f-115">De factuur van de volgende maand die wordt gegenereerd op 12/8 bevat alle kosten voor de service periode 11/1-11/31.</span><span class="sxs-lookup"><span data-stu-id="f116f-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="f116f-116">**Factuur betalings termijn**: netto 60 dagen.</span><span class="sxs-lookup"><span data-stu-id="f116f-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="f116f-117">**Factuur valuta**: partners worden nog steeds gefactureerd in de country's toegewezen valuta van de klant.</span><span class="sxs-lookup"><span data-stu-id="f116f-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="f116f-118">Als de gefactureerde partner zich bijvoorbeeld in Ierland bevindt met klanten in het Verenigd Konink rijk, Noor wegen en Duitsland, ontvangt de gefactureerde partner een factuur/afstemming van GBP, NOK en EUR.</span><span class="sxs-lookup"><span data-stu-id="f116f-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="f116f-119">**Partner prikkels**: betaalde 45 dagen aan het einde van de factuur maand.</span><span class="sxs-lookup"><span data-stu-id="f116f-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="f116f-120">Toegang tot uw facturen en reconciliatie bestanden</span><span class="sxs-lookup"><span data-stu-id="f116f-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="f116f-121">De globale beheerder of facturerings beheerder van uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="f116f-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="f116f-122">Om toegang te krijgen tot de factuur en het afstemmings bestand:</span><span class="sxs-lookup"><span data-stu-id="f116f-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="f116f-123">Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard/) van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="f116f-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f116f-124">Selecteer **facturering** in het menu van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="f116f-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="f116f-125">Selecteer het tabblad voor de **terugkerende** en **eenmalige** en de valuta waarin u bent geïnteresseerd.</span><span class="sxs-lookup"><span data-stu-id="f116f-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="verrekeningscode":::

4. <span data-ttu-id="f116f-127">Selecteer **factuur** of **afstemmings bestand**.</span><span class="sxs-lookup"><span data-stu-id="f116f-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="f116f-128">Als u historische facturen en afstemmings bestanden wilt weer geven, vouwt u de rij facturerings geschiedenis hieronder uit.</span><span class="sxs-lookup"><span data-stu-id="f116f-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="f116f-129">Informatie over gebruiks gegevens</span><span class="sxs-lookup"><span data-stu-id="f116f-129">Understanding usage data</span></span> 

1. <span data-ttu-id="f116f-130">Azure-plan is de hoofd container of het hoogste niveau voor gebruik.</span><span class="sxs-lookup"><span data-stu-id="f116f-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="f116f-131">Al het gebruik is gekoppeld aan één Azure-abonnement.</span><span class="sxs-lookup"><span data-stu-id="f116f-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="f116f-132">Binnen een plan worden er een of meer Azure-abonnementen.</span><span class="sxs-lookup"><span data-stu-id="f116f-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="f116f-133">Dit zijn containers die worden gebruikt voor het beheren en implementeren van resources.</span><span class="sxs-lookup"><span data-stu-id="f116f-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="f116f-134">Binnen een abonnement voegen resource groepen toe aan groeps resources.</span><span class="sxs-lookup"><span data-stu-id="f116f-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="f116f-135">Elke resource wordt geïmplementeerd in één resource groep.</span><span class="sxs-lookup"><span data-stu-id="f116f-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="f116f-136">Voor beelden van resources zijn virtuele machines en opslag accounts.</span><span class="sxs-lookup"><span data-stu-id="f116f-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="f116f-137">Resource-verzend meters: meters zijn metingen van het verbruik van een resource en een resource kan gebruik voor meerdere meters verzenden.</span><span class="sxs-lookup"><span data-stu-id="f116f-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="f116f-138">Meters worden aangeduid met een ProductId, SKUId en AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="f116f-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="f116f-139">Hiërarchie van abonnements resource groepen en-meting</span><span class="sxs-lookup"><span data-stu-id="f116f-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="f116f-140">**Azure-account (Tenant)**</span><span class="sxs-lookup"><span data-stu-id="f116f-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="f116f-141">Abonnement A</span><span class="sxs-lookup"><span data-stu-id="f116f-141">Subscription A</span></span>
    - <span data-ttu-id="f116f-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="f116f-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="f116f-143">Virtuele machine (resource)</span><span class="sxs-lookup"><span data-stu-id="f116f-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f116f-144">Reken meter</span><span class="sxs-lookup"><span data-stu-id="f116f-144">Compute meter</span></span>
        - <span data-ttu-id="f116f-145">Virtueel netwerk (resource)</span><span class="sxs-lookup"><span data-stu-id="f116f-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="f116f-146">Geen facturerings meter</span><span class="sxs-lookup"><span data-stu-id="f116f-146">No billing meter</span></span>

    - <span data-ttu-id="f116f-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="f116f-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="f116f-148">Virtuele machine (resource)</span><span class="sxs-lookup"><span data-stu-id="f116f-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="f116f-149">Computer meter</span><span class="sxs-lookup"><span data-stu-id="f116f-149">Computer meter</span></span>
        - <span data-ttu-id="f116f-150">Premium-SSD-beheerde schijf (resource)</span><span class="sxs-lookup"><span data-stu-id="f116f-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="f116f-151">Opslag capaciteits meter</span><span class="sxs-lookup"><span data-stu-id="f116f-151">Storage capacity meter</span></span>
            - <span data-ttu-id="f116f-152">Meter voor opslag bewerkingen</span><span class="sxs-lookup"><span data-stu-id="f116f-152">Storage operations meter</span></span>

- <span data-ttu-id="f116f-153">Abonnement B-ResourceGroup 1-Azure SQL (resource)-DTU-meter-VPN Gateway (resource)-VPN-gateway meter</span><span class="sxs-lookup"><span data-stu-id="f116f-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="f116f-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="f116f-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="f116f-155">Virtual Network-Interface (resource)</span><span class="sxs-lookup"><span data-stu-id="f116f-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="f116f-156">Geen facturerings meter</span><span class="sxs-lookup"><span data-stu-id="f116f-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="f116f-157">De factuur lezen</span><span class="sxs-lookup"><span data-stu-id="f116f-157">Read the invoice</span></span>

1. <span data-ttu-id="f116f-158">Factuur is niet later beschikbaar dan de achtste van elke maand.</span><span class="sxs-lookup"><span data-stu-id="f116f-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="f116f-159">Partners hebben 60 dagen de betaling te betalen.</span><span class="sxs-lookup"><span data-stu-id="f116f-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="f116f-160">De facturerings periode geldt voor een bepaalde kalender maand, bijvoorbeeld 10/1-10/31.</span><span class="sxs-lookup"><span data-stu-id="f116f-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="f116f-161">Kosten zijn netto-aanpassingen (de hoeveelheid is net of het tegoed van de partner voor beheerde services).</span><span class="sxs-lookup"><span data-stu-id="f116f-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="f116f-162">Bekijk het factuur afstemmings bestand en het dagelijks geclassificeerde gebruiks bestand voor aanvullende facturerings gegevens.</span><span class="sxs-lookup"><span data-stu-id="f116f-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="betalen":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="f116f-164">Het afstemmings bestand van de factuur lezen</span><span class="sxs-lookup"><span data-stu-id="f116f-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="f116f-165">Elk Azure-abonnement en elke combi natie van meters kunnen Maxi maal twee facturerings regels bevatten voor het afstemmings bestand.</span><span class="sxs-lookup"><span data-stu-id="f116f-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="f116f-166">Als de meter die wordt gebruikt voor elk type korting of tegoed (zoals gelaagde kortingen of de partner die is gefactureerd voor services die worden beheerd) in de hele kalender maand voor komt, bevat het afstemmings bestand slechts één facturerings regel.</span><span class="sxs-lookup"><span data-stu-id="f116f-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="f116f-167">In de kolom **PriceAdjusmentDescription** wordt verwezen naar de korting of het tegoed.</span><span class="sxs-lookup"><span data-stu-id="f116f-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="f116f-168">Als er geen resources zijn voor een bepaalde meter die is gekwalificeerd voor de korting of het tegoed van een partner, dan bevat het afstemmings bestand slechts één facturerings regel en de werkelijke eenheids prijs is de prijs van de goed keuring (de prijs per eenheid).</span><span class="sxs-lookup"><span data-stu-id="f116f-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="f116f-169">Als de meter of resources die deze meter uitbrengen, gekwalificeerd zijn voor een partner die wordt **beheerd** voor een deel van de maand, bevat het afstemmings bestand twee facturerings regels.</span><span class="sxs-lookup"><span data-stu-id="f116f-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="f116f-170">Eén regel staat voor de dagen waarin de meting is gekwalificeerd en de tweede regel geeft de dagen aan die de meter niet in aanmerking komt.</span><span class="sxs-lookup"><span data-stu-id="f116f-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="f116f-171">Het dagelijks gebruiks bestand lezen</span><span class="sxs-lookup"><span data-stu-id="f116f-171">Read the daily usage file</span></span>

- <span data-ttu-id="f116f-172">Abonnements meters onder een Azure-abonnement worden beoordeeld en worden op dagelijkse basis gecumuleerd.</span><span class="sxs-lookup"><span data-stu-id="f116f-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="f116f-173">Het **tegoed van de partner voor beheerde services** wordt dagelijks bepaald en toegepast.</span><span class="sxs-lookup"><span data-stu-id="f116f-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="f116f-174">Elke abonnements meter heeft een rij voor elke dag van de maand waarin het verbruik is.</span><span class="sxs-lookup"><span data-stu-id="f116f-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="f116f-175">In het voorbeeld hieronder:</span><span class="sxs-lookup"><span data-stu-id="f116f-175">In the example below:</span></span>

  - <span data-ttu-id="f116f-176">De ingangs prijs voor de partner die wordt **beheerd** via 7/1-7/3 (Houd rekening met de prijzen van de werkelijke eenheid is de prijs van de verkoop op het tegoed van de partner.</span><span class="sxs-lookup"><span data-stu-id="f116f-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="f116f-177">De meter is niet gekwalificeerd voor het tegoed van de **partner voor services** die worden beheerd via 7/4-7/7 (de werkelijke eenheids prijs is de verkoop prijs).</span><span class="sxs-lookup"><span data-stu-id="f116f-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="f116f-178">Meting die geschikt is voor de partner die wordt beheerd via 7/8-7/31 (de werkelijke prijs van een eenheid is de prijs van de **onderneming** , het tegoed van de partner.</span><span class="sxs-lookup"><span data-stu-id="f116f-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="f116f-180">Factuur in klant valuta</span><span class="sxs-lookup"><span data-stu-id="f116f-180">Invoice in customer currency</span></span>

<span data-ttu-id="f116f-181">Voor Azure-Services via een Azure-abonnement geldt een prijs in USD en gefactureerd in de toegewezen valuta van het klant land.</span><span class="sxs-lookup"><span data-stu-id="f116f-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="f116f-182">Als de facturerings valuta niet-USD is, wordt de gebruikte FX-tarief op de laatste pagina van de factuur weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="f116f-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="f116f-183">De FX-tarieven worden maandelijks bepaald en toegepast op de volgende factuur.</span><span class="sxs-lookup"><span data-stu-id="f116f-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="f116f-184">Bekijk de [nieuwe Commerce-Beschik baarheid voor landen en de matrix voor klant](https://go.microsoft.com/fwlink/?linkid=2112354)valuta's voor een volledige lijst met landen valuta's.</span><span class="sxs-lookup"><span data-stu-id="f116f-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="f116f-185">Micro soft volgt de Londen aandelen beurs voor conversie.</span><span class="sxs-lookup"><span data-stu-id="f116f-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="f116f-186">We gebruiken de wissel koers, die gelijk is aan de wissel koers die is vastgelegd op de laatste seconde van de laatste werkdag van de maand op de beurs in Londen.</span><span class="sxs-lookup"><span data-stu-id="f116f-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="f116f-187">De FX-tarieven worden vernieuwd en beschikbaar op de dag vóór de eerste van de maand waarop ze van toepassing zijn.</span><span class="sxs-lookup"><span data-stu-id="f116f-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="f116f-188">Azure-reserveringen</span><span class="sxs-lookup"><span data-stu-id="f116f-188">Azure reservations</span></span>


<span data-ttu-id="f116f-189">Als u [Azure-reserve ringen](azure-reservations.md) aanschaft via een Azure-abonnement, kunt u kiezen voor eenmalige of maandelijkse facturering.</span><span class="sxs-lookup"><span data-stu-id="f116f-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="f116f-190">Uitgaven voor Azure</span><span class="sxs-lookup"><span data-stu-id="f116f-190">Azure spending</span></span>

<span data-ttu-id="f116f-191">De bestaande Azure-bestedings ervaring is bijgewerkt ter ondersteuning van de nieuwe Azure plan-facturering in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f116f-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="f116f-192">Hierdoor kunnen partners:</span><span class="sxs-lookup"><span data-stu-id="f116f-192">This enables partners to:</span></span>

- <span data-ttu-id="f116f-193">Waarschuwingen voor budget sets op klant niveau weer geven, beheren en ontvangen</span><span class="sxs-lookup"><span data-stu-id="f116f-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="f116f-194">Totale geschatte uitgaven voor een Azure-abonnement weer geven (gesplitst op resource-en meter niveau)</span><span class="sxs-lookup"><span data-stu-id="f116f-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="f116f-195">Omdat het facturerings model voor Azure-Services via een Azure-abonnement post-pay-verbruik is, om een grotere factuur te voor komen dan verwacht, kunnen partners een maandelijks budget Toep assen en het percentage van het gebruik bijhouden.</span><span class="sxs-lookup"><span data-stu-id="f116f-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="f116f-196">Een budget kan worden toegepast op één klant of meerdere klanten tegelijk.</span><span class="sxs-lookup"><span data-stu-id="f116f-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Uitgaven voor Azure":::

## <a name="next-steps"></a><span data-ttu-id="f116f-198">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f116f-198">Next steps</span></span>

- <span data-ttu-id="f116f-199">Bekijk hoe het tegoed van de partner (PEC) wordt berekend.</span><span class="sxs-lookup"><span data-stu-id="f116f-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="f116f-200">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/) van het partner centrum en zoek de prijs lijst die beschikbaar is.</span><span class="sxs-lookup"><span data-stu-id="f116f-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="f116f-201">Meer informatie over [het aanschaffen van het Azure-abonnement](purchase-azure-plan.md)</span><span class="sxs-lookup"><span data-stu-id="f116f-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="f116f-202">Zie de [prijs lijst voor de nieuwe Commerce-ervaring in CSP](azure-plan-price-list.md)</span><span class="sxs-lookup"><span data-stu-id="f116f-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
