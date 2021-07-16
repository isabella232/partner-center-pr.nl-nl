---
title: Alle gegevenssets-API-gegevenssets Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om details op te halen van alle beschikbare gegevenssets in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376513"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="b31b9-103">Api voor alle gegevenssets krijgen</span><span class="sxs-lookup"><span data-stu-id="b31b9-103">Get all datasets API</span></span>

<span data-ttu-id="b31b9-104">De API Alle gegevenssets verkrijgen haalt alle beschikbare gegevenssets op.</span><span class="sxs-lookup"><span data-stu-id="b31b9-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="b31b9-105">Gegevenssets maken een lijst van de tabellen, kolommen, metrische gegevens en tijdsbereiken.</span><span class="sxs-lookup"><span data-stu-id="b31b9-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="b31b9-106">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="b31b9-106">**Request syntax**</span></span>

|    <span data-ttu-id="b31b9-107">Methode</span><span class="sxs-lookup"><span data-stu-id="b31b9-107">Method</span></span>    |    <span data-ttu-id="b31b9-108">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="b31b9-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b31b9-109">GET</span><span class="sxs-lookup"><span data-stu-id="b31b9-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="b31b9-110">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="b31b9-110">**Request header**</span></span>

|    <span data-ttu-id="b31b9-111">Header</span><span class="sxs-lookup"><span data-stu-id="b31b9-111">Header</span></span>    |    <span data-ttu-id="b31b9-112">Type</span><span class="sxs-lookup"><span data-stu-id="b31b9-112">Type</span></span>    |    <span data-ttu-id="b31b9-113">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="b31b9-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="b31b9-114">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="b31b9-114">Authorization</span></span>    |    <span data-ttu-id="b31b9-115">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="b31b9-115">string</span></span>    |    <span data-ttu-id="b31b9-116">Vereist.</span><span class="sxs-lookup"><span data-stu-id="b31b9-116">Required.</span></span> <span data-ttu-id="b31b9-117">Het Azure Active Directory (AAD) in de vorm`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="b31b9-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="b31b9-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b31b9-118">Content-Type</span></span>    |    <span data-ttu-id="b31b9-119">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="b31b9-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="b31b9-120">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="b31b9-120">**Path parameter**</span></span>

<span data-ttu-id="b31b9-121">Geen</span><span class="sxs-lookup"><span data-stu-id="b31b9-121">None</span></span>

<span data-ttu-id="b31b9-122">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="b31b9-122">**Query parameter**</span></span>

|    <span data-ttu-id="b31b9-123">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="b31b9-123">Parameter Name</span></span>    |    <span data-ttu-id="b31b9-124">Type</span><span class="sxs-lookup"><span data-stu-id="b31b9-124">Type</span></span>    |    <span data-ttu-id="b31b9-125">Vereist</span><span class="sxs-lookup"><span data-stu-id="b31b9-125">Required</span></span>    |    <span data-ttu-id="b31b9-126">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="b31b9-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="b31b9-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="b31b9-127">datasetName</span></span>    |    <span data-ttu-id="b31b9-128">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="b31b9-128">string</span></span>    |    <span data-ttu-id="b31b9-129">No</span><span class="sxs-lookup"><span data-stu-id="b31b9-129">No</span></span>    |    <span data-ttu-id="b31b9-130">Filteren om details van slechts één gegevensset op te halen</span><span class="sxs-lookup"><span data-stu-id="b31b9-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="b31b9-131">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="b31b9-131">**Request payload**</span></span>

<span data-ttu-id="b31b9-132">Geen</span><span class="sxs-lookup"><span data-stu-id="b31b9-132">None</span></span>

<span data-ttu-id="b31b9-133">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="b31b9-133">**Glossary**</span></span>

<span data-ttu-id="b31b9-134">Geen</span><span class="sxs-lookup"><span data-stu-id="b31b9-134">None</span></span>

<span data-ttu-id="b31b9-135">**Response**</span><span class="sxs-lookup"><span data-stu-id="b31b9-135">**Response**</span></span>

<span data-ttu-id="b31b9-136">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="b31b9-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="b31b9-137">Antwoordcode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="b31b9-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="b31b9-138">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="b31b9-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="b31b9-139">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="b31b9-139">**Glossary**</span></span>

<span data-ttu-id="b31b9-140">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="b31b9-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="b31b9-141">Parameter</span><span class="sxs-lookup"><span data-stu-id="b31b9-141">Parameter</span></span>    |    <span data-ttu-id="b31b9-142">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="b31b9-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="b31b9-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="b31b9-143">DatasetName</span></span>     |    <span data-ttu-id="b31b9-144">Naam van de gegevensset die dit matrixobject definieert</span><span class="sxs-lookup"><span data-stu-id="b31b9-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="b31b9-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="b31b9-145">SelectableColumns</span></span>     |    <span data-ttu-id="b31b9-146">Onbewerkte kolommen die kunnen worden opgegeven in de geselecteerde kolommen</span><span class="sxs-lookup"><span data-stu-id="b31b9-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="b31b9-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="b31b9-147">AvailableMetrics</span></span>     |    <span data-ttu-id="b31b9-148">Aggregatie-/metrische kolomnamen die kunnen worden opgegeven in de geselecteerde kolommen</span><span class="sxs-lookup"><span data-stu-id="b31b9-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="b31b9-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="b31b9-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="b31b9-150">Datumbereik dat kan worden gebruikt in rapportquery's voor de gegevensset</span><span class="sxs-lookup"><span data-stu-id="b31b9-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="b31b9-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="b31b9-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="b31b9-152">Minimale waarde van terugkeerinterval</span><span class="sxs-lookup"><span data-stu-id="b31b9-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="b31b9-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="b31b9-153">TotalCount</span></span>     |    <span data-ttu-id="b31b9-154">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="b31b9-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="b31b9-155">Bericht</span><span class="sxs-lookup"><span data-stu-id="b31b9-155">Message</span></span>     |    <span data-ttu-id="b31b9-156">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="b31b9-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="b31b9-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="b31b9-157">StatusCode</span></span>     |    <span data-ttu-id="b31b9-158">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="b31b9-158">Result Code.</span></span> <span data-ttu-id="b31b9-159">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="b31b9-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
