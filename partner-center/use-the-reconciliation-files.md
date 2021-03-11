---
title: Uw afstemmings bestanden gebruiken
ms.topic: article
ms.date: 03/10/2021
description: Meer informatie over reconciliatie bestanden in het partner centrum en het interpreteren van gedetailleerde weer gaven van het regel item van kosten voor een bepaalde facturerings cyclus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022771"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="2b54e-103">Meer informatie over het lezen van regel items in uw partner centrum-afstemmings bestanden</span><span class="sxs-lookup"><span data-stu-id="2b54e-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="2b54e-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="2b54e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2b54e-105">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="2b54e-105">Billing admin</span></span>
- <span data-ttu-id="2b54e-106">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="2b54e-106">Global admin</span></span>

<span data-ttu-id="2b54e-107">U kunt uw afstemmings bestanden downloaden van het partner centrum voor een gedetailleerde weer gave van regel items van elke kosten in een facturerings cyclus.</span><span class="sxs-lookup"><span data-stu-id="2b54e-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="2b54e-108">Details van regel items zijn kosten voor abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals een middel grote aanvulling van licenties voor een abonnement).</span><span class="sxs-lookup"><span data-stu-id="2b54e-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="2b54e-109">Zie [uw factuur lezen](read-your-bill.md)voor meer informatie over het lezen van uw **facturen**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="2b54e-110">Informatie over afstemmings bestand velden</span><span class="sxs-lookup"><span data-stu-id="2b54e-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="2b54e-111">Velden voor afstemmingsbestand op basis van licentie</span><span class="sxs-lookup"><span data-stu-id="2b54e-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="2b54e-112">Velden voor afstemmingsbestand op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="2b54e-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="2b54e-113">Velden voor afstemmingsbestand over dagelijks gebruik</span><span class="sxs-lookup"><span data-stu-id="2b54e-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="2b54e-114">Eenmalige inkopen CSP-afstemmings bestand velden</span><span class="sxs-lookup"><span data-stu-id="2b54e-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="2b54e-115">Meer informatie over kosten typen in afstemmings bestanden</span><span class="sxs-lookup"><span data-stu-id="2b54e-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="2b54e-116">Zie [reconciliatie bestands toeslag typen](recon-file-charge-types.md)voor meer informatie over de typen kosten in reconciliatie bestanden (de kolom **ChargeType** ).</span><span class="sxs-lookup"><span data-stu-id="2b54e-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="2b54e-117">Opmaak problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="2b54e-117">Fix formatting issues</span></span>

<span data-ttu-id="2b54e-118">Af en toe kan een afstemmings bestand opmaak problemen bevatten.</span><span class="sxs-lookup"><span data-stu-id="2b54e-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="2b54e-119">Dit probleem kan bijvoorbeeld optreden als de land instelling en niet wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="2b54e-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="2b54e-120">Volg deze stappen voor het oplossen van problemen met de opmaak in uw afstemmings bestanden:</span><span class="sxs-lookup"><span data-stu-id="2b54e-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="2b54e-121">Open het afstemmings bestand (in CSV-indeling) in micro soft Excel.</span><span class="sxs-lookup"><span data-stu-id="2b54e-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="2b54e-122">Selecteer de eerste kolom in het bestand.</span><span class="sxs-lookup"><span data-stu-id="2b54e-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="2b54e-123">Open de **wizard tekst naar kolommen converteren**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="2b54e-124">Selecteer op het lint de optie **gegevens** en selecteer vervolgens **tekst naar kolommen**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="2b54e-125">Selecteer in de wizard **gescheiden bestands type**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="2b54e-126">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="2b54e-127">Selecteer **komma** in het veld scheidings **tekens** .</span><span class="sxs-lookup"><span data-stu-id="2b54e-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="2b54e-128">(Als **tabblad** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **volgende**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="2b54e-129">Selecteer in het veld **kolom gegevens indeling** de optie **datum: MDJ**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="2b54e-130">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="2b54e-131">Selecteer in het veld **kolom gegevens indeling** de **tekst** voor alle bedragkolommen.</span><span class="sxs-lookup"><span data-stu-id="2b54e-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="2b54e-132">Selecteer vervolgens **Voltooien**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="2b54e-133">Afstemmings bestanden programmatisch downloaden</span><span class="sxs-lookup"><span data-stu-id="2b54e-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="2b54e-134">Afstemmings bestanden kunnen erg groot zijn en soms moeilijk te downloaden.</span><span class="sxs-lookup"><span data-stu-id="2b54e-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="2b54e-135">Zie [factuur regel items ophalen](/partner-center/develop/get-invoiceline-items)om de afstemmings bestanden via een programma te downloaden.</span><span class="sxs-lookup"><span data-stu-id="2b54e-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="2b54e-136">Belastingen of BTW toewijzen</span><span class="sxs-lookup"><span data-stu-id="2b54e-136">Map taxes or VAT</span></span>

<span data-ttu-id="2b54e-137">BTW of belasting toegevoegde waarde (BTW) toewijzen aan uw factuur:</span><span class="sxs-lookup"><span data-stu-id="2b54e-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="2b54e-138">Som van de **belasting** kolom van het bestand op basis van licentie.</span><span class="sxs-lookup"><span data-stu-id="2b54e-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="2b54e-139">Som van de kolom **TaxAmount** van het bestand op basis van gebruik.</span><span class="sxs-lookup"><span data-stu-id="2b54e-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="2b54e-140">Afstemmings bestanden specificeren op partner</span><span class="sxs-lookup"><span data-stu-id="2b54e-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="2b54e-141">Partners in het **indirecte model** kunnen deze extra velden gebruiken in zowel op licenties gebaseerde afstemmings bestanden als voor het specificeren van de bestanden op reseller.</span><span class="sxs-lookup"><span data-stu-id="2b54e-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="2b54e-142">MPN-id</span><span class="sxs-lookup"><span data-stu-id="2b54e-142">MPN ID</span></span> | <span data-ttu-id="2b54e-143">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="2b54e-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="2b54e-144">MPN-id</span><span class="sxs-lookup"><span data-stu-id="2b54e-144">MPN ID</span></span> | <span data-ttu-id="2b54e-145">De Microsoft Partner Network-ID (MPN) van de Cloud Solution Provider (CSP)-partner (direct of indirect).</span><span class="sxs-lookup"><span data-stu-id="2b54e-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="2b54e-146">Reseller MPN-ID</span><span class="sxs-lookup"><span data-stu-id="2b54e-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="2b54e-147">De [MPN-id van de dealer van de record voor het abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="2b54e-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="2b54e-148">Dit veld komt overeen met de wederverkoper-ID die wordt vermeld voor het specifieke abonnement in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="2b54e-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="2b54e-149">Wordt alleen weer gegeven voor reconciliatie bestanden voor partners in het indirecte model.</span><span class="sxs-lookup"><span data-stu-id="2b54e-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="2b54e-150">Reseller MPN-ID</span><span class="sxs-lookup"><span data-stu-id="2b54e-150">Reseller MPN ID</span></span>

<span data-ttu-id="2b54e-151">Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt hun **MPN-id** twee keer vermeld, zowel de **MPN-id** als de **wederverkoper MPN-id**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="2b54e-152">Als een CSP-partner een wederverkoper heeft zonder **MPN-id**, wordt deze waarde in plaats daarvan ingesteld op de **MPN-id** van de partner.</span><span class="sxs-lookup"><span data-stu-id="2b54e-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="2b54e-153">Als de CSP-partner een **wederverkoper MPN-id** verwijdert, wordt deze waarde ingesteld op *-1*.</span><span class="sxs-lookup"><span data-stu-id="2b54e-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="2b54e-154">De **wederverkoper MPN-id** weer geven of bijwerken:</span><span class="sxs-lookup"><span data-stu-id="2b54e-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="2b54e-155">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="2b54e-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="2b54e-156">Selecteer **klanten** in het menu van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="2b54e-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="2b54e-157">Kies de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="2b54e-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="2b54e-158">Selecteer in het menu klant de optie **abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="2b54e-159">Kies het abonnement in de lijst.</span><span class="sxs-lookup"><span data-stu-id="2b54e-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="2b54e-160">Selecteer **bijwerken** om de wederverkoper te wijzigen **(MPN-id)**.</span><span class="sxs-lookup"><span data-stu-id="2b54e-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2b54e-161">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="2b54e-161">Next steps</span></span>

- [<span data-ttu-id="2b54e-162">Uw factuur & afstemmings bestand lezen</span><span class="sxs-lookup"><span data-stu-id="2b54e-162">How to read your bill & recon file</span></span>](read-your-bill.md) 