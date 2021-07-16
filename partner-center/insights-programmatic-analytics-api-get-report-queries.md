---
title: API voor rapportquery's opvragen - Insights gegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om alle beschikbare query's op te halen voor gebruik in de rapport-API.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376752"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="ce73a-103">API voor rapportquery's opvragen</span><span class="sxs-lookup"><span data-stu-id="ce73a-103">Get report queries API</span></span>

<span data-ttu-id="ce73a-104">De API Rapportquery's krijgen haalt alle query's op die beschikbaar zijn voor gebruik in rapporten.</span><span class="sxs-lookup"><span data-stu-id="ce73a-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="ce73a-105">Alle systeem- en door de gebruiker gedefinieerde query's worden standaard opgevraagd.</span><span class="sxs-lookup"><span data-stu-id="ce73a-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="ce73a-106">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="ce73a-106">**Request syntax**</span></span>

|    <span data-ttu-id="ce73a-107">Methode</span><span class="sxs-lookup"><span data-stu-id="ce73a-107">Method</span></span>    |    <span data-ttu-id="ce73a-108">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="ce73a-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ce73a-109">GET</span><span class="sxs-lookup"><span data-stu-id="ce73a-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="ce73a-110">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="ce73a-110">**Request header**</span></span>

|    <span data-ttu-id="ce73a-111">Header</span><span class="sxs-lookup"><span data-stu-id="ce73a-111">Header</span></span>    |    <span data-ttu-id="ce73a-112">Type</span><span class="sxs-lookup"><span data-stu-id="ce73a-112">Type</span></span>    |    <span data-ttu-id="ce73a-113">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ce73a-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="ce73a-114">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="ce73a-114">Authorization</span></span>    |    <span data-ttu-id="ce73a-115">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="ce73a-115">string</span></span>    |    <span data-ttu-id="ce73a-116">Vereist.</span><span class="sxs-lookup"><span data-stu-id="ce73a-116">Required.</span></span> <span data-ttu-id="ce73a-117">Het Azure Active Directory (AAD) in het formulier`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="ce73a-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="ce73a-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce73a-118">Content-Type</span></span>    |    <span data-ttu-id="ce73a-119">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="ce73a-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="ce73a-120">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="ce73a-120">**Path parameter**</span></span>

<span data-ttu-id="ce73a-121">Geen</span><span class="sxs-lookup"><span data-stu-id="ce73a-121">None</span></span>

<span data-ttu-id="ce73a-122">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="ce73a-122">**Query parameter**</span></span>

|    <span data-ttu-id="ce73a-123">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="ce73a-123">Parameter Name</span></span>    |    <span data-ttu-id="ce73a-124">Type</span><span class="sxs-lookup"><span data-stu-id="ce73a-124">Type</span></span>    |    <span data-ttu-id="ce73a-125">Vereist</span><span class="sxs-lookup"><span data-stu-id="ce73a-125">Required</span></span>    |    <span data-ttu-id="ce73a-126">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ce73a-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="ce73a-127">queryId</span><span class="sxs-lookup"><span data-stu-id="ce73a-127">queryId</span></span>     |    <span data-ttu-id="ce73a-128">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="ce73a-128">string</span></span>     |    <span data-ttu-id="ce73a-129">No</span><span class="sxs-lookup"><span data-stu-id="ce73a-129">No</span></span>    |    <span data-ttu-id="ce73a-130">Filter om alleen details van query's op te halen met de id die is opgegeven in het argument</span><span class="sxs-lookup"><span data-stu-id="ce73a-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="ce73a-131">queryName</span><span class="sxs-lookup"><span data-stu-id="ce73a-131">queryName</span></span>     |    <span data-ttu-id="ce73a-132">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="ce73a-132">string</span></span>     |    <span data-ttu-id="ce73a-133">No</span><span class="sxs-lookup"><span data-stu-id="ce73a-133">No</span></span>    |    <span data-ttu-id="ce73a-134">Filter om alleen details van query's op te halen met de naam die is opgegeven in het argument</span><span class="sxs-lookup"><span data-stu-id="ce73a-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="ce73a-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="ce73a-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="ce73a-136">booleaans</span><span class="sxs-lookup"><span data-stu-id="ce73a-136">boolean</span></span>     |    <span data-ttu-id="ce73a-137">Nee</span><span class="sxs-lookup"><span data-stu-id="ce73a-137">No</span></span>    |    <span data-ttu-id="ce73a-138">Vooraf gedefinieerde systeemquery's opnemen in het antwoord</span><span class="sxs-lookup"><span data-stu-id="ce73a-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="ce73a-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="ce73a-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="ce73a-140">booleaans</span><span class="sxs-lookup"><span data-stu-id="ce73a-140">boolean</span></span>     |    <span data-ttu-id="ce73a-141">Nee</span><span class="sxs-lookup"><span data-stu-id="ce73a-141">No</span></span>    |    <span data-ttu-id="ce73a-142">Alleen systeemquery's opnemen in het antwoord</span><span class="sxs-lookup"><span data-stu-id="ce73a-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="ce73a-143">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="ce73a-143">**Request payload**</span></span>

<span data-ttu-id="ce73a-144">Geen</span><span class="sxs-lookup"><span data-stu-id="ce73a-144">None</span></span>

<span data-ttu-id="ce73a-145">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="ce73a-145">**Glossary**</span></span>

<span data-ttu-id="ce73a-146">Geen</span><span class="sxs-lookup"><span data-stu-id="ce73a-146">None</span></span>

<span data-ttu-id="ce73a-147">**Response**</span><span class="sxs-lookup"><span data-stu-id="ce73a-147">**Response**</span></span>

<span data-ttu-id="ce73a-148">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="ce73a-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="ce73a-149">Antwoordcode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="ce73a-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="ce73a-150">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="ce73a-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="ce73a-151">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="ce73a-151">**Glossary**</span></span>

<span data-ttu-id="ce73a-152">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="ce73a-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="ce73a-153">Parameter</span><span class="sxs-lookup"><span data-stu-id="ce73a-153">Parameter</span></span>    |    <span data-ttu-id="ce73a-154">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ce73a-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="ce73a-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="ce73a-155">QueryId</span></span>     |    <span data-ttu-id="ce73a-156">Unieke UUID van de query</span><span class="sxs-lookup"><span data-stu-id="ce73a-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="ce73a-157">Name</span><span class="sxs-lookup"><span data-stu-id="ce73a-157">Name</span></span>     |    <span data-ttu-id="ce73a-158">Naam die aan de query is gegeven op het moment dat de query wordt gemaakt</span><span class="sxs-lookup"><span data-stu-id="ce73a-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="ce73a-159">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="ce73a-159">Description</span></span>     |    <span data-ttu-id="ce73a-160">Beschrijving gegeven tijdens het maken van de query</span><span class="sxs-lookup"><span data-stu-id="ce73a-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="ce73a-161">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="ce73a-161">Query</span></span>     |    <span data-ttu-id="ce73a-162">Rapportqueryreeks</span><span class="sxs-lookup"><span data-stu-id="ce73a-162">Report query string</span></span>     |
|    <span data-ttu-id="ce73a-163">Type</span><span class="sxs-lookup"><span data-stu-id="ce73a-163">Type</span></span>     |    <span data-ttu-id="ce73a-164">Ingesteld op userDefined voor door de gebruiker gemaakte query's en systeem voor vooraf gedefinieerde systeemquery's</span><span class="sxs-lookup"><span data-stu-id="ce73a-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="ce73a-165">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="ce73a-165">User</span></span>     |    <span data-ttu-id="ce73a-166">Gebruikers-id die de query heeft gemaakt</span><span class="sxs-lookup"><span data-stu-id="ce73a-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="ce73a-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="ce73a-167">CreatedTime</span></span>     |    <span data-ttu-id="ce73a-168">Tijdstip van het maken van de query</span><span class="sxs-lookup"><span data-stu-id="ce73a-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="ce73a-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ce73a-169">TotalCount</span></span>     |    <span data-ttu-id="ce73a-170">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="ce73a-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="ce73a-171">Bericht</span><span class="sxs-lookup"><span data-stu-id="ce73a-171">Message</span></span>     |    <span data-ttu-id="ce73a-172">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="ce73a-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="ce73a-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="ce73a-173">StatusCode</span></span>     |    <span data-ttu-id="ce73a-174">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="ce73a-174">Result Code.</span></span> <span data-ttu-id="ce73a-175">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="ce73a-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
