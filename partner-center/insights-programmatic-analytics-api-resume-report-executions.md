---
title: Api voor rapportuitvoering hervatten - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om de uitvoering van onderbroken rapport in Partner Center hervatten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376744"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="6f596-103">API voor rapportuitvoeringen hervatten</span><span class="sxs-lookup"><span data-stu-id="6f596-103">Resume report executions API</span></span>

<span data-ttu-id="6f596-104">Bij de uitvoering hervat deze API de geplande uitvoering van een onderbroken rapport.</span><span class="sxs-lookup"><span data-stu-id="6f596-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="6f596-105">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="6f596-105">**Request syntax**</span></span>

|    <span data-ttu-id="6f596-106">Methode</span><span class="sxs-lookup"><span data-stu-id="6f596-106">Method</span></span>    |    <span data-ttu-id="6f596-107">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="6f596-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6f596-108">PUT</span><span class="sxs-lookup"><span data-stu-id="6f596-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="6f596-109">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="6f596-109">**Request header**</span></span>

|    <span data-ttu-id="6f596-110">Header</span><span class="sxs-lookup"><span data-stu-id="6f596-110">Header</span></span>    |    <span data-ttu-id="6f596-111">Type</span><span class="sxs-lookup"><span data-stu-id="6f596-111">Type</span></span>    |    <span data-ttu-id="6f596-112">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="6f596-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="6f596-113">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="6f596-113">Authorization</span></span>    |    <span data-ttu-id="6f596-114">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="6f596-114">string</span></span>    |    <span data-ttu-id="6f596-115">Vereist.</span><span class="sxs-lookup"><span data-stu-id="6f596-115">Required.</span></span> <span data-ttu-id="6f596-116">Het Azure Active Directory (AAD) in de vorm`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="6f596-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="6f596-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6f596-117">Content-Type</span></span>    |    <span data-ttu-id="6f596-118">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="6f596-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="6f596-119">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="6f596-119">**Path parameter**</span></span>

|    <span data-ttu-id="6f596-120">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="6f596-120">Parameter Name</span></span>    |    <span data-ttu-id="6f596-121">Type</span><span class="sxs-lookup"><span data-stu-id="6f596-121">Type</span></span>    |    <span data-ttu-id="6f596-122">Vereist</span><span class="sxs-lookup"><span data-stu-id="6f596-122">Required</span></span>    |    <span data-ttu-id="6f596-123">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="6f596-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="6f596-124">reportId</span><span class="sxs-lookup"><span data-stu-id="6f596-124">reportId</span></span>     |    <span data-ttu-id="6f596-125">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="6f596-125">string</span></span>    |    <span data-ttu-id="6f596-126">No</span><span class="sxs-lookup"><span data-stu-id="6f596-126">No</span></span>    |    <span data-ttu-id="6f596-127">Id van het rapport dat wordt gewijzigd</span><span class="sxs-lookup"><span data-stu-id="6f596-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="6f596-128">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="6f596-128">**Query parameter**</span></span>

<span data-ttu-id="6f596-129">Geen</span><span class="sxs-lookup"><span data-stu-id="6f596-129">None</span></span>

<span data-ttu-id="6f596-130">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="6f596-130">**Request payload**</span></span>

<span data-ttu-id="6f596-131">Geen</span><span class="sxs-lookup"><span data-stu-id="6f596-131">None</span></span>

<span data-ttu-id="6f596-132">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="6f596-132">**Glossary**</span></span>

<span data-ttu-id="6f596-133">Geen</span><span class="sxs-lookup"><span data-stu-id="6f596-133">None</span></span>

<span data-ttu-id="6f596-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="6f596-134">**Response**</span></span>

<span data-ttu-id="6f596-135">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="6f596-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="6f596-136">Antwoordcode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="6f596-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="6f596-137">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="6f596-137">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="6f596-138">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="6f596-138">**Glossary**</span></span>

<span data-ttu-id="6f596-139">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="6f596-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="6f596-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="6f596-140">Parameter</span></span>    |    <span data-ttu-id="6f596-141">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="6f596-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="6f596-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="6f596-142">ReportId</span></span>     |    <span data-ttu-id="6f596-143">Universally Unique Identifier (UUID) van het hervatte rapport</span><span class="sxs-lookup"><span data-stu-id="6f596-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="6f596-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="6f596-144">ReportName</span></span>     |    <span data-ttu-id="6f596-145">Naam die aan het rapport is gegeven tijdens het maken</span><span class="sxs-lookup"><span data-stu-id="6f596-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="6f596-146">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="6f596-146">Description</span></span>     |    <span data-ttu-id="6f596-147">Beschrijving opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="6f596-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="6f596-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="6f596-148">QueryId</span></span>     |    <span data-ttu-id="6f596-149">Query-id doorgegeven op het moment dat het rapport werd gemaakt</span><span class="sxs-lookup"><span data-stu-id="6f596-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="6f596-150">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="6f596-150">Query</span></span>     |    <span data-ttu-id="6f596-151">Querytekst die wordt uitgevoerd voor dit rapport</span><span class="sxs-lookup"><span data-stu-id="6f596-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="6f596-152">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="6f596-152">User</span></span>     |    <span data-ttu-id="6f596-153">Gebruikers-id die wordt gebruikt om het rapport te maken</span><span class="sxs-lookup"><span data-stu-id="6f596-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="6f596-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="6f596-154">CreatedTime</span></span>     |    <span data-ttu-id="6f596-155">Tijd dat het rapport is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="6f596-155">Time the report was created.</span></span> <span data-ttu-id="6f596-156">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="6f596-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="6f596-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="6f596-157">ModifiedTime</span></span>     |    <span data-ttu-id="6f596-158">Het tijdstip dat het rapport voor het laatst is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="6f596-158">Time the report was last modified.</span></span> <span data-ttu-id="6f596-159">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="6f596-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="6f596-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="6f596-160">ExecuteNow</span></span>     |    <span data-ttu-id="6f596-161">ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt</span><span class="sxs-lookup"><span data-stu-id="6f596-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="6f596-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="6f596-162">StartTime</span></span>     |    <span data-ttu-id="6f596-163">Tijd dat de uitvoering van het rapport begint.</span><span class="sxs-lookup"><span data-stu-id="6f596-163">Time the report execution will begin.</span></span> <span data-ttu-id="6f596-164">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="6f596-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="6f596-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="6f596-165">ReportStatus</span></span>     |    <span data-ttu-id="6f596-166">Status van de uitvoering van het rapport.</span><span class="sxs-lookup"><span data-stu-id="6f596-166">Status of the report execution.</span></span> <span data-ttu-id="6f596-167">De mogelijke waarden zijn Onderbroken, Actief en Inactief.</span><span class="sxs-lookup"><span data-stu-id="6f596-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="6f596-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="6f596-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="6f596-169">Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="6f596-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="6f596-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="6f596-170">RecurrenceCount</span></span>     |    <span data-ttu-id="6f596-171">Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="6f596-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="6f596-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="6f596-172">CallbackUrl</span></span>     |    <span data-ttu-id="6f596-173">Callback-URL die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="6f596-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="6f596-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="6f596-174">CallbackMethod</span></span>    |    <span data-ttu-id="6f596-175">Callback-methode die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="6f596-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="6f596-176">Indeling</span><span class="sxs-lookup"><span data-stu-id="6f596-176">Format</span></span>     |    <span data-ttu-id="6f596-177">Indeling van de rapportbestanden</span><span class="sxs-lookup"><span data-stu-id="6f596-177">Format of the report files</span></span>     |
|    <span data-ttu-id="6f596-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="6f596-178">TotalCount</span></span>     |    <span data-ttu-id="6f596-179">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="6f596-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="6f596-180">Bericht</span><span class="sxs-lookup"><span data-stu-id="6f596-180">Message</span></span>     |    <span data-ttu-id="6f596-181">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="6f596-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="6f596-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="6f596-182">StatusCode</span></span>     |    <span data-ttu-id="6f596-183">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="6f596-183">Result Code.</span></span> <span data-ttu-id="6f596-184">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="6f596-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
