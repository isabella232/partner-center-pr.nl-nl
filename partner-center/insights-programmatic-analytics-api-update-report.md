---
title: Rapport-API bijwerken
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om rapportparameters bij te werken in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376576"
---
# <a name="update-report-api"></a><span data-ttu-id="0fb37-103">Rapport-API bijwerken</span><span class="sxs-lookup"><span data-stu-id="0fb37-103">Update report API</span></span>

<span data-ttu-id="0fb37-104">Met deze API kunt u een rapportparameter wijzigen.</span><span class="sxs-lookup"><span data-stu-id="0fb37-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="0fb37-105">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="0fb37-105">**Request syntax**</span></span>

|    <span data-ttu-id="0fb37-106">Methode</span><span class="sxs-lookup"><span data-stu-id="0fb37-106">Method</span></span>    |    <span data-ttu-id="0fb37-107">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="0fb37-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0fb37-108">PUT</span><span class="sxs-lookup"><span data-stu-id="0fb37-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="0fb37-109">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="0fb37-109">**Request header**</span></span>

|    <span data-ttu-id="0fb37-110">Header</span><span class="sxs-lookup"><span data-stu-id="0fb37-110">Header</span></span>    |    <span data-ttu-id="0fb37-111">Type</span><span class="sxs-lookup"><span data-stu-id="0fb37-111">Type</span></span>    |    <span data-ttu-id="0fb37-112">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="0fb37-113">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="0fb37-113">Authorization</span></span>    |    <span data-ttu-id="0fb37-114">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-114">string</span></span>    |    <span data-ttu-id="0fb37-115">Vereist.</span><span class="sxs-lookup"><span data-stu-id="0fb37-115">Required.</span></span> <span data-ttu-id="0fb37-116">Het Azure Active Directory (AAD) in de vorm`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="0fb37-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="0fb37-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0fb37-117">Content-Type</span></span>    |    <span data-ttu-id="0fb37-118">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="0fb37-119">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="0fb37-119">**Path parameter**</span></span>

|    <span data-ttu-id="0fb37-120">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="0fb37-120">Parameter Name</span></span>    |    <span data-ttu-id="0fb37-121">Type</span><span class="sxs-lookup"><span data-stu-id="0fb37-121">Type</span></span>    |    <span data-ttu-id="0fb37-122">Vereist</span><span class="sxs-lookup"><span data-stu-id="0fb37-122">Required</span></span>    |    <span data-ttu-id="0fb37-123">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0fb37-124">reportId</span><span class="sxs-lookup"><span data-stu-id="0fb37-124">reportId</span></span>     |    <span data-ttu-id="0fb37-125">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-125">string</span></span>    |    <span data-ttu-id="0fb37-126">No</span><span class="sxs-lookup"><span data-stu-id="0fb37-126">No</span></span>    |    <span data-ttu-id="0fb37-127">Id van het rapport dat wordt gewijzigd</span><span class="sxs-lookup"><span data-stu-id="0fb37-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="0fb37-128">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="0fb37-128">**Query parameter**</span></span>

<span data-ttu-id="0fb37-129">Geen</span><span class="sxs-lookup"><span data-stu-id="0fb37-129">None</span></span>

<span data-ttu-id="0fb37-130">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="0fb37-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="0fb37-131">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="0fb37-131">**Glossary**</span></span>

<span data-ttu-id="0fb37-132">Deze tabel bevat de belangrijkste definities van elementen in het antwoord.</span><span class="sxs-lookup"><span data-stu-id="0fb37-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="0fb37-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="0fb37-133">Parameter</span></span>    |    <span data-ttu-id="0fb37-134">Vereist</span><span class="sxs-lookup"><span data-stu-id="0fb37-134">Required</span></span>    |    <span data-ttu-id="0fb37-135">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-135">Description</span></span>    |    <span data-ttu-id="0fb37-136">Toegestane waarden</span><span class="sxs-lookup"><span data-stu-id="0fb37-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="0fb37-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="0fb37-137">ReportName</span></span>     |    <span data-ttu-id="0fb37-138">Ja</span><span class="sxs-lookup"><span data-stu-id="0fb37-138">Yes</span></span>     |    <span data-ttu-id="0fb37-139">Naam die moet worden toegewezen aan het rapport</span><span class="sxs-lookup"><span data-stu-id="0fb37-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="0fb37-140">Tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-140">String</span></span>     |
|    <span data-ttu-id="0fb37-141">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-141">Description</span></span>     |    <span data-ttu-id="0fb37-142">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-142">No</span></span>     |    <span data-ttu-id="0fb37-143">Beschrijving van het gemaakte rapport</span><span class="sxs-lookup"><span data-stu-id="0fb37-143">Description of the created report</span></span>     |    <span data-ttu-id="0fb37-144">Tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-144">String</span></span>     |
|    <span data-ttu-id="0fb37-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="0fb37-145">StartTime</span></span>     |    <span data-ttu-id="0fb37-146">Ja</span><span class="sxs-lookup"><span data-stu-id="0fb37-146">Yes</span></span>    |    <span data-ttu-id="0fb37-147">Tijdstempel waarna het genereren van het rapport begint</span><span class="sxs-lookup"><span data-stu-id="0fb37-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="0fb37-148">Tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-148">String</span></span>     |
|    <span data-ttu-id="0fb37-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0fb37-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="0fb37-150">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-150">No</span></span>     |    <span data-ttu-id="0fb37-151">Frequentie waarmee het rapport in uren moet worden gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="0fb37-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="0fb37-152">Minimumwaarde is 4</span><span class="sxs-lookup"><span data-stu-id="0fb37-152">Minimum value is 4</span></span>     |    <span data-ttu-id="0fb37-153">Geheel getal</span><span class="sxs-lookup"><span data-stu-id="0fb37-153">Integer</span></span>     |
|    <span data-ttu-id="0fb37-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0fb37-154">RecurrenceCount</span></span>     |    <span data-ttu-id="0fb37-155">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-155">No</span></span>     |    <span data-ttu-id="0fb37-156">Het aantal te genereren rapport.</span><span class="sxs-lookup"><span data-stu-id="0fb37-156">Numbers of report to be generated.</span></span> <span data-ttu-id="0fb37-157">De standaardwaarde is onbeperkt.</span><span class="sxs-lookup"><span data-stu-id="0fb37-157">Default is indefinite.</span></span>     |    <span data-ttu-id="0fb37-158">Geheel getal</span><span class="sxs-lookup"><span data-stu-id="0fb37-158">Integer</span></span>     |
|    <span data-ttu-id="0fb37-159">Indeling</span><span class="sxs-lookup"><span data-stu-id="0fb37-159">Format</span></span>     |    <span data-ttu-id="0fb37-160">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-160">No</span></span>    |    <span data-ttu-id="0fb37-161">Bestandsindeling van het geëxporteerde bestand.</span><span class="sxs-lookup"><span data-stu-id="0fb37-161">File format of the exported file.</span></span> <span data-ttu-id="0fb37-162">De standaardwaarde is CSV</span><span class="sxs-lookup"><span data-stu-id="0fb37-162">Default is CSV</span></span>     |    <span data-ttu-id="0fb37-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="0fb37-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="0fb37-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="0fb37-164">CallbackURL</span></span>     |    <span data-ttu-id="0fb37-165">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-165">No</span></span>     |    <span data-ttu-id="0fb37-166">HTTPS-callback-URL die moet worden aangeroepen bij het genereren van het rapport</span><span class="sxs-lookup"><span data-stu-id="0fb37-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="0fb37-167">Tekenreeks</span><span class="sxs-lookup"><span data-stu-id="0fb37-167">String</span></span>     |
|    <span data-ttu-id="0fb37-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0fb37-168">CallbackMethod</span></span>    |    <span data-ttu-id="0fb37-169">Nee</span><span class="sxs-lookup"><span data-stu-id="0fb37-169">No</span></span>    |    <span data-ttu-id="0fb37-170">Http-methode die moet worden gebruikt voor callback</span><span class="sxs-lookup"><span data-stu-id="0fb37-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="0fb37-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="0fb37-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="0fb37-172">**Response**</span><span class="sxs-lookup"><span data-stu-id="0fb37-172">**Response**</span></span>

<span data-ttu-id="0fb37-173">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="0fb37-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="0fb37-174">Antwoordcode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="0fb37-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="0fb37-175">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="0fb37-175">Response payload example:</span></span>

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

<span data-ttu-id="0fb37-176">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="0fb37-176">**Glossary**</span></span>

<span data-ttu-id="0fb37-177">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="0fb37-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="0fb37-178">Parameter</span><span class="sxs-lookup"><span data-stu-id="0fb37-178">Parameter</span></span>    |    <span data-ttu-id="0fb37-179">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="0fb37-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="0fb37-180">ReportId</span></span>     |    <span data-ttu-id="0fb37-181">Universally Unique Identifier (UUID) van het rapport dat wordt bijgewerkt</span><span class="sxs-lookup"><span data-stu-id="0fb37-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="0fb37-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="0fb37-182">ReportName</span></span>     |    <span data-ttu-id="0fb37-183">Naam van het rapport in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0fb37-184">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="0fb37-184">Description</span></span>     |    <span data-ttu-id="0fb37-185">Beschrijving van het rapport in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="0fb37-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="0fb37-186">QueryId</span></span>     |    <span data-ttu-id="0fb37-187">Query-id doorgegeven op het moment dat het rapport werd gemaakt</span><span class="sxs-lookup"><span data-stu-id="0fb37-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="0fb37-188">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="0fb37-188">Query</span></span>     |    <span data-ttu-id="0fb37-189">Querytekst die wordt uitgevoerd voor dit rapport</span><span class="sxs-lookup"><span data-stu-id="0fb37-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="0fb37-190">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="0fb37-190">User</span></span>     |    <span data-ttu-id="0fb37-191">Gebruikers-id die wordt gebruikt om het rapport te maken</span><span class="sxs-lookup"><span data-stu-id="0fb37-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="0fb37-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="0fb37-192">CreatedTime</span></span>     |    <span data-ttu-id="0fb37-193">Tijd dat het rapport is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="0fb37-193">Time the report was created.</span></span> <span data-ttu-id="0fb37-194">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0fb37-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0fb37-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="0fb37-195">ModifiedTime</span></span>     |    <span data-ttu-id="0fb37-196">Het tijdstip dat het rapport voor het laatst is gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="0fb37-196">Time the report was last modified.</span></span> <span data-ttu-id="0fb37-197">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0fb37-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0fb37-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="0fb37-198">ExecuteNow</span></span>     |    <span data-ttu-id="0fb37-199">ExecuteNow-vlag ingesteld op het moment dat het rapport werd gemaakt</span><span class="sxs-lookup"><span data-stu-id="0fb37-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="0fb37-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="0fb37-200">StartTime</span></span>     |    <span data-ttu-id="0fb37-201">Tijd dat de uitvoering van het rapport begint.</span><span class="sxs-lookup"><span data-stu-id="0fb37-201">Time the report execution will begin.</span></span> <span data-ttu-id="0fb37-202">De tijdnotatie is yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="0fb37-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="0fb37-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="0fb37-203">ReportStatus</span></span>     |    <span data-ttu-id="0fb37-204">Status van de uitvoering van het rapport.</span><span class="sxs-lookup"><span data-stu-id="0fb37-204">Status of the report execution.</span></span> <span data-ttu-id="0fb37-205">De mogelijke waarden zijn Onderbroken, Actief en Inactief.</span><span class="sxs-lookup"><span data-stu-id="0fb37-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="0fb37-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="0fb37-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="0fb37-207">Terugkeerpatroon dat is opgegeven in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="0fb37-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="0fb37-208">RecurrenceCount</span></span>     |    <span data-ttu-id="0fb37-209">Aantal terugkeerpatroon dat is opgegeven in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="0fb37-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="0fb37-210">CallbackUrl</span></span>     |    <span data-ttu-id="0fb37-211">Callback-URL die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="0fb37-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="0fb37-212">CallbackMethod</span></span>    |    <span data-ttu-id="0fb37-213">Callback-methode die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="0fb37-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="0fb37-214">Indeling</span><span class="sxs-lookup"><span data-stu-id="0fb37-214">Format</span></span>     |    <span data-ttu-id="0fb37-215">Indeling van de rapportbestanden</span><span class="sxs-lookup"><span data-stu-id="0fb37-215">Format of the report files</span></span>     |
|    <span data-ttu-id="0fb37-216">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="0fb37-216">TotalCount</span></span>     |    <span data-ttu-id="0fb37-217">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="0fb37-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="0fb37-218">Bericht</span><span class="sxs-lookup"><span data-stu-id="0fb37-218">Message</span></span>     |    <span data-ttu-id="0fb37-219">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="0fb37-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="0fb37-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="0fb37-220">StatusCode</span></span>     |    <span data-ttu-id="0fb37-221">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="0fb37-221">Result Code.</span></span> <span data-ttu-id="0fb37-222">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="0fb37-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |