---
title: Uw afstemmings bestanden gebruiken
ms.topic: article
ms.date: 06/08/2020
description: Meer informatie over reconciliatie bestanden in het partner centrum en het interpreteren van gedetailleerde weer gaven van het regel item van kosten voor een bepaalde facturerings cyclus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488076"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="c7b08-103">Meer informatie over het lezen van regel items in uw partner centrum-afstemmings bestanden</span><span class="sxs-lookup"><span data-stu-id="c7b08-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="c7b08-104">Van toepassing op:</span><span class="sxs-lookup"><span data-stu-id="c7b08-104">Applies to:</span></span>

- <span data-ttu-id="c7b08-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="c7b08-105">Partner Center</span></span>
- <span data-ttu-id="c7b08-106">Partnercentrum voor Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c7b08-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c7b08-107">U kunt uw afstemmings bestanden downloaden van het partner centrum voor een gedetailleerde weer gave van regel items van elke kosten in een facturerings cyclus.</span><span class="sxs-lookup"><span data-stu-id="c7b08-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="c7b08-108">Details van regel items zijn kosten voor abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals een middel grote aanvulling van licenties voor een abonnement).</span><span class="sxs-lookup"><span data-stu-id="c7b08-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="c7b08-109">Juiste rollen:</span><span class="sxs-lookup"><span data-stu-id="c7b08-109">Appropriate roles:</span></span>

- <span data-ttu-id="c7b08-110">Factureringsbeheerder</span><span class="sxs-lookup"><span data-stu-id="c7b08-110">Billing admin</span></span>
- <span data-ttu-id="c7b08-111">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="c7b08-111">Global admin</span></span>

<span data-ttu-id="c7b08-112">Zie [uw factuur lezen](read-your-bill.md)voor meer informatie over het lezen van uw **facturen**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-112">For information on how to read your **invoice** , see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="c7b08-113">Informatie over afstemmings bestand velden</span><span class="sxs-lookup"><span data-stu-id="c7b08-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="c7b08-114">Velden voor afstemmings bestanden op basis van licentie</span><span class="sxs-lookup"><span data-stu-id="c7b08-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="c7b08-115">Velden voor afstemmings bestand op basis van gebruik</span><span class="sxs-lookup"><span data-stu-id="c7b08-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="c7b08-116">Velden voor het afstemmen van dagelijks geclassificeerd gebruik</span><span class="sxs-lookup"><span data-stu-id="c7b08-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="c7b08-117">Eenmalige inkopen CSP-afstemmings bestand velden</span><span class="sxs-lookup"><span data-stu-id="c7b08-117">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="c7b08-118">Meer informatie over kosten typen in afstemmings bestanden</span><span class="sxs-lookup"><span data-stu-id="c7b08-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="c7b08-119">Zie [reconciliatie bestands toeslag typen](recon-file-charge-types.md)voor meer informatie over de typen kosten in reconciliatie bestanden (de kolom **ChargeType** ).</span><span class="sxs-lookup"><span data-stu-id="c7b08-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="c7b08-120">Opmaak problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="c7b08-120">Fix formatting issues</span></span>

<span data-ttu-id="c7b08-121">Af en toe kan een afstemmings bestand opmaak problemen bevatten.</span><span class="sxs-lookup"><span data-stu-id="c7b08-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="c7b08-122">Dit probleem kan bijvoorbeeld optreden als de land instelling en niet wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="c7b08-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="c7b08-123">Volg deze stappen voor het oplossen van problemen met de opmaak in uw afstemmings bestanden:</span><span class="sxs-lookup"><span data-stu-id="c7b08-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="c7b08-124">Open het afstemmings bestand (in CSV-indeling) in micro soft Excel.</span><span class="sxs-lookup"><span data-stu-id="c7b08-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="c7b08-125">Selecteer de eerste kolom in het bestand.</span><span class="sxs-lookup"><span data-stu-id="c7b08-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="c7b08-126">Open de **wizard tekst naar kolommen converteren**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="c7b08-127">Selecteer op het lint de optie **gegevens** en selecteer vervolgens **tekst naar kolommen**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-127">On the ribbon, select **Data** , then select **Text to Columns**.</span></span>
4. <span data-ttu-id="c7b08-128">Selecteer in de wizard **gescheiden bestands type**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="c7b08-129">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="c7b08-130">Selecteer **komma** in het veld scheidings **tekens** .</span><span class="sxs-lookup"><span data-stu-id="c7b08-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="c7b08-131">(Als **tabblad** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **volgende**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="c7b08-132">Selecteer in het veld **kolom gegevens indeling** de optie **datum: MDJ**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="c7b08-133">Selecteer vervolgens **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="c7b08-134">Selecteer in het veld **kolom gegevens indeling** de **tekst** voor alle bedragkolommen.</span><span class="sxs-lookup"><span data-stu-id="c7b08-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="c7b08-135">Selecteer vervolgens **Voltooien**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="c7b08-136">Afstemmings bestanden programmatisch downloaden</span><span class="sxs-lookup"><span data-stu-id="c7b08-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="c7b08-137">Afstemmings bestanden kunnen erg groot zijn en soms moeilijk te downloaden.</span><span class="sxs-lookup"><span data-stu-id="c7b08-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="c7b08-138">Zie [factuur regel items ophalen](/partner-center/develop/get-invoiceline-items)om de afstemmings bestanden via een programma te downloaden.</span><span class="sxs-lookup"><span data-stu-id="c7b08-138">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="c7b08-139">Belastingen of BTW toewijzen</span><span class="sxs-lookup"><span data-stu-id="c7b08-139">Map taxes or VAT</span></span>

<span data-ttu-id="c7b08-140">BTW of belasting toegevoegde waarde (BTW) toewijzen aan uw factuur:</span><span class="sxs-lookup"><span data-stu-id="c7b08-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="c7b08-141">Som van de **belasting** kolom van het bestand op basis van licentie.</span><span class="sxs-lookup"><span data-stu-id="c7b08-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="c7b08-142">Som van de kolom **TaxAmount** van het bestand op basis van gebruik.</span><span class="sxs-lookup"><span data-stu-id="c7b08-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="c7b08-143">Afstemmings bestanden specificeren op partner</span><span class="sxs-lookup"><span data-stu-id="c7b08-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="c7b08-144">Partners in het **indirecte model** kunnen deze extra velden gebruiken in zowel op licenties gebaseerde afstemmings bestanden als voor het specificeren van de bestanden op reseller.</span><span class="sxs-lookup"><span data-stu-id="c7b08-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="c7b08-145">MPN-id</span><span class="sxs-lookup"><span data-stu-id="c7b08-145">MPN ID</span></span> | <span data-ttu-id="c7b08-146">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="c7b08-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="c7b08-147">MPN-id</span><span class="sxs-lookup"><span data-stu-id="c7b08-147">MPN ID</span></span> | <span data-ttu-id="c7b08-148">De Microsoft Partner Network-ID (MPN) van de Cloud Solution Provider (CSP)-partner (direct of indirect).</span><span class="sxs-lookup"><span data-stu-id="c7b08-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="c7b08-149">Reseller MPN-ID</span><span class="sxs-lookup"><span data-stu-id="c7b08-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="c7b08-150">De [MPN-id van de dealer van de record voor het abonnement](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="c7b08-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="c7b08-151">Dit veld komt overeen met de wederverkoper-ID die wordt vermeld voor het specifieke abonnement in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="c7b08-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="c7b08-152">Wordt alleen weer gegeven voor reconciliatie bestanden voor partners in het indirecte model.</span><span class="sxs-lookup"><span data-stu-id="c7b08-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="c7b08-153">Reseller MPN-ID</span><span class="sxs-lookup"><span data-stu-id="c7b08-153">Reseller MPN ID</span></span>

<span data-ttu-id="c7b08-154">Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt hun **MPN-id** twee keer vermeld, zowel de **MPN-id** als de **wederverkoper MPN-id**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="c7b08-155">Als een CSP-partner een wederverkoper heeft zonder **MPN-id** , wordt deze waarde in plaats daarvan ingesteld op de **MPN-id** van de partner.</span><span class="sxs-lookup"><span data-stu-id="c7b08-155">If a CSP partner has a reseller with no **MPN ID** , this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="c7b08-156">Als de CSP-partner een **wederverkoper MPN-id** verwijdert, wordt deze waarde ingesteld op *-1*.</span><span class="sxs-lookup"><span data-stu-id="c7b08-156">If the CSP partner removes a **Reseller MPN ID** , this value will be set to *-1*.</span></span>

<span data-ttu-id="c7b08-157">De **wederverkoper MPN-id** weer geven of bijwerken:</span><span class="sxs-lookup"><span data-stu-id="c7b08-157">To view or update the **Reseller MPN ID** :</span></span>

1. <span data-ttu-id="c7b08-158">Meld u aan bij Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="c7b08-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="c7b08-159">Selecteer **klanten** in het menu van het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="c7b08-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="c7b08-160">Kies de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="c7b08-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="c7b08-161">Selecteer in het menu klant de optie **abonnementen**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="c7b08-162">Kies het abonnement in de lijst.</span><span class="sxs-lookup"><span data-stu-id="c7b08-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="c7b08-163">Selecteer **bijwerken** om de wederverkoper te wijzigen **(MPN-id)**.</span><span class="sxs-lookup"><span data-stu-id="c7b08-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>