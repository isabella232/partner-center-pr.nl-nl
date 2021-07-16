---
title: Rapport-API op Insights halen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om alle beschikbare rapport-id's in Partner Center verkrijgen.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376749"
---
# <a name="get-report-api"></a><span data-ttu-id="1daae-103">Rapport-API op halen</span><span class="sxs-lookup"><span data-stu-id="1daae-103">Get report API</span></span>

<span data-ttu-id="1daae-104">Met deze API worden alle geplande rapporten opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="1daae-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="1daae-105">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="1daae-105">**Request syntax**</span></span>

|    <span data-ttu-id="1daae-106">Methode</span><span class="sxs-lookup"><span data-stu-id="1daae-106">Method</span></span>    |    <span data-ttu-id="1daae-107">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="1daae-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1daae-108">GET</span><span class="sxs-lookup"><span data-stu-id="1daae-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="1daae-109">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="1daae-109">**Request header**</span></span>

|    <span data-ttu-id="1daae-110">Header</span><span class="sxs-lookup"><span data-stu-id="1daae-110">Header</span></span>    |    <span data-ttu-id="1daae-111">Type</span><span class="sxs-lookup"><span data-stu-id="1daae-111">Type</span></span>    |    <span data-ttu-id="1daae-112">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="1daae-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="1daae-113">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="1daae-113">Authorization</span></span>    |    <span data-ttu-id="1daae-114">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="1daae-114">string</span></span>    |    <span data-ttu-id="1daae-115">Vereist.</span><span class="sxs-lookup"><span data-stu-id="1daae-115">Required.</span></span> <span data-ttu-id="1daae-116">Het Azure Active Directory (AAD) in het formulier`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="1daae-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="1daae-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1daae-117">Content-Type</span></span>    |    <span data-ttu-id="1daae-118">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="1daae-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="1daae-119">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="1daae-119">**Path parameter**</span></span>

<span data-ttu-id="1daae-120">Geen</span><span class="sxs-lookup"><span data-stu-id="1daae-120">None</span></span>

<span data-ttu-id="1daae-121">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="1daae-121">**Query parameter**</span></span>

|    <span data-ttu-id="1daae-122">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="1daae-122">Parameter Name</span></span>    |    <span data-ttu-id="1daae-123">Type</span><span class="sxs-lookup"><span data-stu-id="1daae-123">Type</span></span>    |    <span data-ttu-id="1daae-124">Vereist</span><span class="sxs-lookup"><span data-stu-id="1daae-124">Required</span></span>    |    <span data-ttu-id="1daae-125">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="1daae-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="1daae-126">reportId</span><span class="sxs-lookup"><span data-stu-id="1daae-126">reportId</span></span>     |    <span data-ttu-id="1daae-127">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="1daae-127">string</span></span>    |    <span data-ttu-id="1daae-128">No</span><span class="sxs-lookup"><span data-stu-id="1daae-128">No</span></span>    |    <span data-ttu-id="1daae-129">Filter om alleen details op te halen van rapporten met de reportId die in dit argument is opgegeven</span><span class="sxs-lookup"><span data-stu-id="1daae-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="1daae-130">reportName</span><span class="sxs-lookup"><span data-stu-id="1daae-130">reportName</span></span>     |    <span data-ttu-id="1daae-131">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="1daae-131">string</span></span>    |    <span data-ttu-id="1daae-132">No</span><span class="sxs-lookup"><span data-stu-id="1daae-132">No</span></span>    |    <span data-ttu-id="1daae-133">Filter om alleen details van rapporten op te halen met de reportName in dit argument</span><span class="sxs-lookup"><span data-stu-id="1daae-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="1daae-134">queryId</span><span class="sxs-lookup"><span data-stu-id="1daae-134">queryId</span></span>     |    <span data-ttu-id="1daae-135">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="1daae-135">string</span></span>    |    <span data-ttu-id="1daae-136">No</span><span class="sxs-lookup"><span data-stu-id="1daae-136">No</span></span>    |    <span data-ttu-id="1daae-137">Filter om alleen details van rapporten op te halen met de queryId die in dit argument is opgegeven</span><span class="sxs-lookup"><span data-stu-id="1daae-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="1daae-138">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="1daae-138">**Request payload**</span></span>

<span data-ttu-id="1daae-139">Geen</span><span class="sxs-lookup"><span data-stu-id="1daae-139">None</span></span>

<span data-ttu-id="1daae-140">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="1daae-140">**Glossary**</span></span>

<span data-ttu-id="1daae-141">Geen</span><span class="sxs-lookup"><span data-stu-id="1daae-141">None</span></span>

<span data-ttu-id="1daae-142">**Response**</span><span class="sxs-lookup"><span data-stu-id="1daae-142">**Response**</span></span>

<span data-ttu-id="1daae-143">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="1daae-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="1daae-144">Responscode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="1daae-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="1daae-145">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="1daae-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="1daae-146">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="1daae-146">**Glossary**</span></span>

<span data-ttu-id="1daae-147">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="1daae-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="1daae-148">Parameter</span><span class="sxs-lookup"><span data-stu-id="1daae-148">Parameter</span></span>    |    <span data-ttu-id="1daae-149">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="1daae-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="1daae-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="1daae-150">ReportId</span></span>     |    <span data-ttu-id="1daae-151">Unieke UUID van het rapport dat is gemaakt</span><span class="sxs-lookup"><span data-stu-id="1daae-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="1daae-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="1daae-152">ReportName</span></span>     |    <span data-ttu-id="1daae-153">Naam van het rapport in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="1daae-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="1daae-154">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="1daae-154">Description</span></span>     |    <span data-ttu-id="1daae-155">Beschrijving gegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="1daae-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="1daae-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="1daae-156">QueryId</span></span>     |    <span data-ttu-id="1daae-157">Query-id doorgegeven op het moment dat het rapport werd gemaakt</span><span class="sxs-lookup"><span data-stu-id="1daae-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="1daae-158">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="1daae-158">Query</span></span>     |    <span data-ttu-id="1daae-159">Querytekst die wordt uitgevoerd voor dit rapport</span><span class="sxs-lookup"><span data-stu-id="1daae-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="1daae-160">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="1daae-160">User</span></span>     |    <span data-ttu-id="1daae-161">Gebruikers-id die wordt gebruikt om het rapport te maken</span><span class="sxs-lookup"><span data-stu-id="1daae-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="1daae-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="1daae-162">CreatedTime</span></span>     |    <span data-ttu-id="1daae-163">Het tijdstip dat het rapport is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="1daae-163">Time the report was created.</span></span> <span data-ttu-id="1daae-164">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1daae-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1daae-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="1daae-165">ModifiedTime</span></span>     |    <span data-ttu-id="1daae-166">Het tijdstip dat het rapport voor het laatst is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="1daae-166">Time the report was last modified.</span></span> <span data-ttu-id="1daae-167">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1daae-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1daae-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="1daae-168">executeNow</span></span>     |    <span data-ttu-id="1daae-169">ExecuteNow-vlag ingesteld op het moment dat het rapport is gemaakt</span><span class="sxs-lookup"><span data-stu-id="1daae-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="1daae-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="1daae-170">StartTime</span></span>     |    <span data-ttu-id="1daae-171">De uitvoering van de tijd begint.</span><span class="sxs-lookup"><span data-stu-id="1daae-171">Time execution will begin.</span></span> <span data-ttu-id="1daae-172">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="1daae-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="1daae-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="1daae-173">ReportStatus</span></span>     |    <span data-ttu-id="1daae-174">Status van de uitvoering van het rapport.</span><span class="sxs-lookup"><span data-stu-id="1daae-174">Status of the report execution.</span></span> <span data-ttu-id="1daae-175">De mogelijke waarden zijn Onderbroken, Actief en Inactief.</span><span class="sxs-lookup"><span data-stu-id="1daae-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="1daae-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="1daae-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="1daae-177">Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="1daae-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="1daae-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="1daae-178">RecurrenceCount</span></span>     |    <span data-ttu-id="1daae-179">Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="1daae-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="1daae-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="1daae-180">CallbackUrl</span></span>     |    <span data-ttu-id="1daae-181">Callback-URL die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="1daae-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="1daae-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="1daae-182">CallbackMethod</span></span>    |    <span data-ttu-id="1daae-183">Callback-methode die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="1daae-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="1daae-184">Indeling</span><span class="sxs-lookup"><span data-stu-id="1daae-184">Format</span></span>     |    <span data-ttu-id="1daae-185">Indeling van de rapportbestanden</span><span class="sxs-lookup"><span data-stu-id="1daae-185">Format of the report files</span></span>     |
|    <span data-ttu-id="1daae-186">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="1daae-186">TotalCount</span></span>     |    <span data-ttu-id="1daae-187">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="1daae-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="1daae-188">Bericht</span><span class="sxs-lookup"><span data-stu-id="1daae-188">Message</span></span>     |    <span data-ttu-id="1daae-189">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="1daae-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="1daae-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="1daae-190">StatusCode</span></span>     |    <span data-ttu-id="1daae-191">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="1daae-191">Result Code.</span></span> <span data-ttu-id="1daae-192">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="1daae-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |