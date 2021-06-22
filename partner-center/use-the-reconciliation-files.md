---
title: Uw afstemmingsbestanden gebruiken
ms.topic: article
ms.date: 03/26/2021
description: Meer informatie over afstemmingsbestanden in Partner Center en hoe u de gedetailleerde weergaven van de kosten voor een bepaalde factureringscyclus kunt interpreteren.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431559"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="4fad3-103">Informatie over het lezen van de regelitems in uw Partner Center afstemmingsbestanden</span><span class="sxs-lookup"><span data-stu-id="4fad3-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="4fad3-104">**Juiste rollen:** Factureringsbeheerders | Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="4fad3-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="4fad3-105">U kunt uw afstemmingsbestanden downloaden Partner Center voor een gedetailleerde weergave van alle kosten in een factureringscyclus.</span><span class="sxs-lookup"><span data-stu-id="4fad3-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="4fad3-106">Details van regelitem omvatten kosten voor de abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals het op de korte termijn toevoegen van licenties aan een abonnement).</span><span class="sxs-lookup"><span data-stu-id="4fad3-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="4fad3-107">Zie Uw factuur lezen voor **meer informatie** over het lezen van [uw factuur.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="4fad3-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="4fad3-108">Velden voor afstemmingsbestand begrijpen</span><span class="sxs-lookup"><span data-stu-id="4fad3-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="4fad3-109">Velden voor afstemmingsbestand op basis van licentie</span><span class="sxs-lookup"><span data-stu-id="4fad3-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="4fad3-110">Velden voor afstemmingsbestand op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="4fad3-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="4fad3-111">Velden voor afstemmingsbestand over dagelijks gebruik</span><span class="sxs-lookup"><span data-stu-id="4fad3-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="4fad3-112">Velden voor CSP-afstemmingsbestand voor een een time-aankoop</span><span class="sxs-lookup"><span data-stu-id="4fad3-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="4fad3-113">Inzicht in kostentypen in afstemmingsbestanden</span><span class="sxs-lookup"><span data-stu-id="4fad3-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="4fad3-114">Zie Kostentypen voor afstemmingsbestand voor meer [](recon-file-charge-types.md)informatie over de typen kosten in afstemmingsbestanden (de kolom **ChargeType).**</span><span class="sxs-lookup"><span data-stu-id="4fad3-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="4fad3-115">Opmaakproblemen oplossen</span><span class="sxs-lookup"><span data-stu-id="4fad3-115">Fix formatting issues</span></span>

<span data-ttu-id="4fad3-116">Af en toe kan een afstemmingsbestand opmaakproblemen bevatten.</span><span class="sxs-lookup"><span data-stu-id="4fad3-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="4fad3-117">Dit probleem kan bijvoorbeeld optreden als de en-US-locale niet wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4fad3-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="4fad3-118">Volg deze stappen om eventuele opmaakproblemen in uw afstemmingsbestanden op te lossen:</span><span class="sxs-lookup"><span data-stu-id="4fad3-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="4fad3-119">Open het afstemmingsbestand (in .csv indeling) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4fad3-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="4fad3-120">Selecteer de eerste kolom in het bestand.</span><span class="sxs-lookup"><span data-stu-id="4fad3-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="4fad3-121">Open de **wizard Tekst converteren naar kolommen.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="4fad3-122">Selecteer op het lint **Gegevens** en selecteer vervolgens Tekst **naar kolommen.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="4fad3-123">Selecteer in de wizard **Bestandstype met scheidingstekens.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="4fad3-124">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="4fad3-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="4fad3-125">Selecteer in **het veld Scheidingstekens** de optie **Komma**.</span><span class="sxs-lookup"><span data-stu-id="4fad3-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="4fad3-126">(Als **Tab** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **Volgende.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="4fad3-127">Selecteer **datum:MDY** **in** het veld Kolomgegevensindeling.</span><span class="sxs-lookup"><span data-stu-id="4fad3-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="4fad3-128">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="4fad3-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="4fad3-129">Selecteer in **het veld Kolomgegevensindeling** de optie **Tekst** voor alle hoeveelheid kolommen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="4fad3-130">Selecteer vervolgens **Voltooien**.</span><span class="sxs-lookup"><span data-stu-id="4fad3-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="4fad3-131">Afstemmingsbestanden programmatisch downloaden</span><span class="sxs-lookup"><span data-stu-id="4fad3-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="4fad3-132">Afstemmingsbestanden kunnen erg groot zijn en zijn soms moeilijk te downloaden.</span><span class="sxs-lookup"><span data-stu-id="4fad3-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="4fad3-133">Zie Factuurregelitems downloaden om afstemmingsbestanden programmatisch [te downloaden.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="4fad3-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="4fad3-134">Als uw bestand de rijlimiet in Excel overschrijdt</span><span class="sxs-lookup"><span data-stu-id="4fad3-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="4fad3-135">Als u een afstemmingsbestand kunt downloaden maar niet kunt openen in Microsoft Excel, betekent dit waarschijnlijk dat het bestand meer rijen bevat dan Excel toestaat.</span><span class="sxs-lookup"><span data-stu-id="4fad3-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="4fad3-136">Als dit gebeurt, kunt u een van de onderstaande procedures gebruiken om het bestand te openen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="4fad3-137">Open een reconbestand in Power BI</span><span class="sxs-lookup"><span data-stu-id="4fad3-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="4fad3-138">Download het afstemmingsbestand zoals u dat normaal zou doen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4fad3-139">Download, installeer en open een exemplaar van Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="4fad3-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="4fad3-140">Selecteer op Power BI **tabblad Start** de optie **Gegevens verzamelen.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="4fad3-141">Selecteer **Tekst/CSV** **in** de lijst met algemene gegevensbronnen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="4fad3-142">Open het reconbestand wanneer u daarom wordt gevraagd.</span><span class="sxs-lookup"><span data-stu-id="4fad3-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="4fad3-143">Een reconbestand openen in een Excel-draaitabel</span><span class="sxs-lookup"><span data-stu-id="4fad3-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="4fad3-144">Download het afstemmingsbestand zoals u dat normaal zou doen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="4fad3-145">Open een nieuw bestand in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="4fad3-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="4fad3-146">Selecteer op **het** tabblad Gegevens de optie **Gegevens downloaden,** selecteer **Uit bestand** en selecteer vervolgens **Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="4fad3-147">Open het reconbestand wanneer u daarom wordt gevraagd.</span><span class="sxs-lookup"><span data-stu-id="4fad3-147">When prompted, open your recon file.</span></span> <span data-ttu-id="4fad3-148">Uw gegevens worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="4fad3-148">Your data will appear.</span></span>
5. <span data-ttu-id="4fad3-149">Selecteer in **de** vervolgkeuzelijst Laden de optie **Laden naar** en selecteer vervolgens **OK.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="4fad3-150">Selecteer in **het dialoogvenster Gegevens** importeren de optie **Draaitabelrapport om** het bestand te openen.</span><span class="sxs-lookup"><span data-stu-id="4fad3-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="4fad3-151">Negatief bedrag weergegeven</span><span class="sxs-lookup"><span data-stu-id="4fad3-151">Negative amount displayed</span></span>

<span data-ttu-id="4fad3-152">Mogelijk ziet u een negatief bedrag in uw afstemmingsbestand.</span><span class="sxs-lookup"><span data-stu-id="4fad3-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="4fad3-153">Dit wordt mogelijk veroorzaakt door een van de volgende zaken:</span><span class="sxs-lookup"><span data-stu-id="4fad3-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="4fad3-154">U hebt het aantal licenties onlangs geannuleerd of verlaagd</span><span class="sxs-lookup"><span data-stu-id="4fad3-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="4fad3-155">U hebt tegoed ontvangen voor een servicelicentieovereenkomst (SLA) of voor Azure-verbruik</span><span class="sxs-lookup"><span data-stu-id="4fad3-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="4fad3-156">Voor meer informatie over deze transactie raadpleegt u de bijbehorende kostentype-eigenschap in uw afstemmingsbestand.</span><span class="sxs-lookup"><span data-stu-id="4fad3-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="4fad3-157">Btw of btw in kaart brengen</span><span class="sxs-lookup"><span data-stu-id="4fad3-157">Map taxes or VAT</span></span>

<span data-ttu-id="4fad3-158">Belastingen of btw-waarde (BTW) aan uw factuur toe te voegen:</span><span class="sxs-lookup"><span data-stu-id="4fad3-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="4fad3-159">Som de **kolom Belasting** op uit het op licenties gebaseerde bestand.</span><span class="sxs-lookup"><span data-stu-id="4fad3-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="4fad3-160">Som de **kolom TaxAmount** op uit het bestand op basis van gebruik.</span><span class="sxs-lookup"><span data-stu-id="4fad3-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="4fad3-161">Afstemmingsbestanden itemeren per partner</span><span class="sxs-lookup"><span data-stu-id="4fad3-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="4fad3-162">Partners in het **indirecte model kunnen** deze aanvullende velden gebruiken in zowel op licenties gebaseerde als op gebruik gebaseerde afstemmingsbestanden om de bestanden per reseller te itemeren.</span><span class="sxs-lookup"><span data-stu-id="4fad3-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="4fad3-163">MPN-id</span><span class="sxs-lookup"><span data-stu-id="4fad3-163">MPN ID</span></span> | <span data-ttu-id="4fad3-164">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="4fad3-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="4fad3-165">MPN-id</span><span class="sxs-lookup"><span data-stu-id="4fad3-165">MPN ID</span></span> | <span data-ttu-id="4fad3-166">De Microsoft Partner Network (MPN)-id van de Cloud Solution Provider (CSP)-partner (direct of indirect).</span><span class="sxs-lookup"><span data-stu-id="4fad3-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="4fad3-167">MPN-id van reseller</span><span class="sxs-lookup"><span data-stu-id="4fad3-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="4fad3-168">De [MPN-id van de reseller van de record voor het abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="4fad3-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="4fad3-169">Dit veld komt overeen met de reseller-id die wordt vermeld voor het specifieke abonnement in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="4fad3-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="4fad3-170">Wordt alleen weergegeven in afstemmingsbestanden voor partners in het indirecte model.</span><span class="sxs-lookup"><span data-stu-id="4fad3-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="4fad3-171">MPN-id voor reseller</span><span class="sxs-lookup"><span data-stu-id="4fad3-171">Reseller MPN ID</span></span>

<span data-ttu-id="4fad3-172">Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt de **MPN-id** twee keer vermeld, zowel als de **MPN-id** van de reseller en de **MPN-id** van de reseller.</span><span class="sxs-lookup"><span data-stu-id="4fad3-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="4fad3-173">Als een CSP-partner een reseller zonder **MPN-id** heeft, wordt deze waarde in plaats daarvan ingesteld op de **MPN-id van de partner.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="4fad3-174">Als de CSP-partner een **MPN-id** voor resellers verwijdert, wordt deze waarde ingesteld *op -1.*</span><span class="sxs-lookup"><span data-stu-id="4fad3-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="4fad3-175">Als u de MPN-id van **de reseller wilt weergeven of bijwerken:**</span><span class="sxs-lookup"><span data-stu-id="4fad3-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="4fad3-176">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="4fad3-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="4fad3-177">Selecteer in Partner Center menu **Klanten.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="4fad3-178">Kies de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="4fad3-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="4fad3-179">Selecteer Abonnementen in het menu **van de klant.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="4fad3-180">Kies het abonnement in de lijst.</span><span class="sxs-lookup"><span data-stu-id="4fad3-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="4fad3-181">Selecteer **Update om** de Reseller **(MPN-id) te wijzigen.**</span><span class="sxs-lookup"><span data-stu-id="4fad3-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4fad3-182">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="4fad3-182">Next steps</span></span>

- [<span data-ttu-id="4fad3-183">Uw factuur lezen & recon-bestand</span><span class="sxs-lookup"><span data-stu-id="4fad3-183">How to read your bill & recon file</span></span>](read-your-bill.md) 