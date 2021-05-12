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
ms.openlocfilehash: 755881d0bd96b9d601346ebb6271bd524c31d0a3
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/12/2021
ms.locfileid: "109794952"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="f51a1-103">Informatie over het lezen van de regelitems in uw Partner Center afstemmingsbestanden</span><span class="sxs-lookup"><span data-stu-id="f51a1-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="f51a1-104">**Juiste rollen:** Factureringsbeheerders | Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="f51a1-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="f51a1-105">U kunt uw afstemmingsbestanden downloaden Partner Center voor een gedetailleerde weergave van alle kosten in een factureringscyclus.</span><span class="sxs-lookup"><span data-stu-id="f51a1-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="f51a1-106">Details van regelitem omvatten kosten voor de abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals het op de korte termijn toevoegen van licenties aan een abonnement).</span><span class="sxs-lookup"><span data-stu-id="f51a1-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="f51a1-107">Zie Uw factuur lezen voor **meer informatie** over het lezen van [uw factuur.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="f51a1-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="f51a1-108">Velden voor afstemmingsbestand begrijpen</span><span class="sxs-lookup"><span data-stu-id="f51a1-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="f51a1-109">Velden voor afstemmingsbestand op basis van licentie</span><span class="sxs-lookup"><span data-stu-id="f51a1-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="f51a1-110">Velden voor afstemmingsbestand op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="f51a1-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="f51a1-111">Velden voor afstemmingsbestand over dagelijks gebruik</span><span class="sxs-lookup"><span data-stu-id="f51a1-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="f51a1-112">Velden voor CSP-afstemmingsbestand voor een een time-aankoop</span><span class="sxs-lookup"><span data-stu-id="f51a1-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="f51a1-113">Inzicht in kostentypen in afstemmingsbestanden</span><span class="sxs-lookup"><span data-stu-id="f51a1-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="f51a1-114">Zie Kostentypen voor afstemmingsbestand voor meer [](recon-file-charge-types.md)informatie over de typen kosten in afstemmingsbestanden (de kolom **ChargeType).**</span><span class="sxs-lookup"><span data-stu-id="f51a1-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="f51a1-115">Opmaakproblemen oplossen</span><span class="sxs-lookup"><span data-stu-id="f51a1-115">Fix formatting issues</span></span>

<span data-ttu-id="f51a1-116">Af en toe kan een afstemmingsbestand opmaakproblemen bevatten.</span><span class="sxs-lookup"><span data-stu-id="f51a1-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="f51a1-117">Dit probleem kan bijvoorbeeld optreden als de en-US-locale niet wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="f51a1-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="f51a1-118">Volg deze stappen om eventuele opmaakproblemen in uw afstemmingsbestanden op te lossen:</span><span class="sxs-lookup"><span data-stu-id="f51a1-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="f51a1-119">Open het afstemmingsbestand (in CSV-indeling) in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f51a1-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="f51a1-120">Selecteer de eerste kolom in het bestand.</span><span class="sxs-lookup"><span data-stu-id="f51a1-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="f51a1-121">Open de **wizard Tekst converteren naar kolommen.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="f51a1-122">Selecteer op het lint **Gegevens** en selecteer vervolgens Tekst **naar kolommen.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="f51a1-123">Selecteer in de wizard **Bestandstype met scheidingstekens.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="f51a1-124">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="f51a1-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="f51a1-125">Selecteer in **het veld Scheidingstekens** de optie **Komma**.</span><span class="sxs-lookup"><span data-stu-id="f51a1-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="f51a1-126">(Als **Tab** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **Volgende.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="f51a1-127">Selecteer  **datum:MDY** in het veld Kolomgegevensindeling.</span><span class="sxs-lookup"><span data-stu-id="f51a1-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="f51a1-128">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="f51a1-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="f51a1-129">Selecteer in **het veld Kolomgegevensindeling** de optie **Tekst** voor alle hoeveelheid kolommen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="f51a1-130">Selecteer vervolgens **Voltooien**.</span><span class="sxs-lookup"><span data-stu-id="f51a1-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="f51a1-131">Afstemmingsbestanden programmatisch downloaden</span><span class="sxs-lookup"><span data-stu-id="f51a1-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="f51a1-132">Afstemmingsbestanden kunnen erg groot zijn en zijn soms moeilijk te downloaden.</span><span class="sxs-lookup"><span data-stu-id="f51a1-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="f51a1-133">Zie Factuurregelitems downloaden om afstemmingsbestanden programmatisch [te downloaden.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="f51a1-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="f51a1-134">Als uw bestand de rijlimiet in Excel overschrijdt</span><span class="sxs-lookup"><span data-stu-id="f51a1-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="f51a1-135">Als u een afstemmingsbestand kunt downloaden maar niet kunt openen in Microsoft Excel, betekent dit waarschijnlijk dat het bestand meer rijen bevat dan Excel toestaat.</span><span class="sxs-lookup"><span data-stu-id="f51a1-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="f51a1-136">Als dit gebeurt, kunt u een van de onderstaande procedures gebruiken om het bestand te openen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="f51a1-137">Open een reconbestand in Power BI</span><span class="sxs-lookup"><span data-stu-id="f51a1-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="f51a1-138">Download het afstemmingsbestand zoals u dat normaal zou doen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="f51a1-139">Download, installeer en open een exemplaar van Power BI.</span><span class="sxs-lookup"><span data-stu-id="f51a1-139">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="f51a1-140">Selecteer op Power BI **tabblad Start** de optie **Gegevens op halen.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="f51a1-141">Selecteer **Tekst/CSV** **in** de lijst met algemene gegevensbronnen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="f51a1-142">Open het reconbestand wanneer u daarom wordt gevraagd.</span><span class="sxs-lookup"><span data-stu-id="f51a1-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="f51a1-143">Een reconbestand openen in een Excel-draaitabel</span><span class="sxs-lookup"><span data-stu-id="f51a1-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="f51a1-144">Download het afstemmingsbestand zoals u dat normaal zou doen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="f51a1-145">Open een nieuw bestand in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="f51a1-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="f51a1-146">Selecteer op **het** tabblad Gegevens de optie **Gegevens downloaden,** selecteer **Uit bestand** en selecteer vervolgens **Tekst/CSV.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="f51a1-147">Wanneer u hier om wordt gevraagd, opent u het recon-bestand.</span><span class="sxs-lookup"><span data-stu-id="f51a1-147">When prompted, open your recon file.</span></span> <span data-ttu-id="f51a1-148">Uw gegevens worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="f51a1-148">Your data will appear.</span></span>
5. <span data-ttu-id="f51a1-149">Selecteer in **de** vervolgkeuzelijst Laden de optie **Laden naar** en vervolgens **OK.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-149">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="f51a1-150">Selecteer in **het dialoogvenster Gegevens** importeren de optie **Draaitabelrapport om** het bestand te openen.</span><span class="sxs-lookup"><span data-stu-id="f51a1-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="f51a1-151">Negatief bedrag weergegeven</span><span class="sxs-lookup"><span data-stu-id="f51a1-151">Negative amount displayed</span></span>

<span data-ttu-id="f51a1-152">Mogelijk ziet u een negatief bedrag in uw afstemmingsbestand.</span><span class="sxs-lookup"><span data-stu-id="f51a1-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="f51a1-153">Dit wordt mogelijk veroorzaakt door een van de volgende zaken:</span><span class="sxs-lookup"><span data-stu-id="f51a1-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="f51a1-154">U hebt het aantal licenties onlangs geannuleerd of verlaagd</span><span class="sxs-lookup"><span data-stu-id="f51a1-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="f51a1-155">U hebt tegoed ontvangen voor een servicelicentieovereenkomst (SLA) of voor Azure-verbruik</span><span class="sxs-lookup"><span data-stu-id="f51a1-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="f51a1-156">Voor meer informatie over deze transactie raadpleegt u de bijbehorende kostentype-eigenschap in uw afstemmingsbestand.</span><span class="sxs-lookup"><span data-stu-id="f51a1-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="f51a1-157">Btw of btw in kaart brengen</span><span class="sxs-lookup"><span data-stu-id="f51a1-157">Map taxes or VAT</span></span>

<span data-ttu-id="f51a1-158">Belastingen of btw-waarde (BTW) aan uw factuur toe te voegen:</span><span class="sxs-lookup"><span data-stu-id="f51a1-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="f51a1-159">Som de **kolom Belasting** op uit het op licenties gebaseerde bestand.</span><span class="sxs-lookup"><span data-stu-id="f51a1-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="f51a1-160">Som de **kolom TaxAmount** op uit het bestand op basis van gebruik.</span><span class="sxs-lookup"><span data-stu-id="f51a1-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="f51a1-161">Afstemmingsbestanden itemeren per partner</span><span class="sxs-lookup"><span data-stu-id="f51a1-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="f51a1-162">Partners in het **indirecte model kunnen** deze aanvullende velden gebruiken in zowel op licenties gebaseerde als op gebruik gebaseerde afstemmingsbestanden om de bestanden per reseller te itemeren.</span><span class="sxs-lookup"><span data-stu-id="f51a1-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="f51a1-163">MPN-id</span><span class="sxs-lookup"><span data-stu-id="f51a1-163">MPN ID</span></span> | <span data-ttu-id="f51a1-164">Description</span><span class="sxs-lookup"><span data-stu-id="f51a1-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="f51a1-165">MPN-id</span><span class="sxs-lookup"><span data-stu-id="f51a1-165">MPN ID</span></span> | <span data-ttu-id="f51a1-166">De Microsoft Partner Network (MPN)-id van de Cloud Solution Provider (CSP)-partner (direct of indirect).</span><span class="sxs-lookup"><span data-stu-id="f51a1-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="f51a1-167">MPN-id van reseller</span><span class="sxs-lookup"><span data-stu-id="f51a1-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="f51a1-168">De [MPN-id van de reseller van de record voor het abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="f51a1-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="f51a1-169">Dit veld komt overeen met de reseller-id die wordt vermeld voor het specifieke abonnement in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f51a1-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="f51a1-170">Wordt alleen weergegeven in afstemmingsbestanden voor partners in het indirecte model.</span><span class="sxs-lookup"><span data-stu-id="f51a1-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="f51a1-171">MPN-id van reseller</span><span class="sxs-lookup"><span data-stu-id="f51a1-171">Reseller MPN ID</span></span>

<span data-ttu-id="f51a1-172">Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt de **MPN-id** twee keer weergegeven, zowel als de **MPN-id** en de **MPN-id** van de reseller.</span><span class="sxs-lookup"><span data-stu-id="f51a1-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="f51a1-173">Als een CSP-partner een reseller zonder **MPN-id** heeft, wordt deze waarde in plaats daarvan ingesteld op de **MPN-id van de partner.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="f51a1-174">Als de CSP-partner een **MPN-id voor** resellers verwijdert, wordt deze waarde ingesteld *op -1.*</span><span class="sxs-lookup"><span data-stu-id="f51a1-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="f51a1-175">Als u de MPN-id van **de reseller wilt weergeven of bijwerken:**</span><span class="sxs-lookup"><span data-stu-id="f51a1-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="f51a1-176">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="f51a1-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="f51a1-177">Selecteer in Partner Center menu **Klanten.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="f51a1-178">Kies de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="f51a1-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="f51a1-179">Selecteer Abonnementen in het menu **van de klant.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="f51a1-180">Kies het abonnement in de lijst.</span><span class="sxs-lookup"><span data-stu-id="f51a1-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="f51a1-181">Selecteer **Update om** de Reseller **(MPN-id) te wijzigen.**</span><span class="sxs-lookup"><span data-stu-id="f51a1-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f51a1-182">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f51a1-182">Next steps</span></span>

- [<span data-ttu-id="f51a1-183">Uw factuur lezen & recon-bestand</span><span class="sxs-lookup"><span data-stu-id="f51a1-183">How to read your bill & recon file</span></span>](read-your-bill.md) 