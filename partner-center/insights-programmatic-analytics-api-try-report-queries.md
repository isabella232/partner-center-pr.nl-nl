---
title: Rapportquery's-API uitproberen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om uw query te testen en de resultaten te valideren in Partner Center inzichten.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376736"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="3c64e-103">Rapportquery's-API uitproberen</span><span class="sxs-lookup"><span data-stu-id="3c64e-103">Try report queries API</span></span>

<span data-ttu-id="3c64e-104">Met deze API wordt een query-instructie Report uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="3c64e-104">This API executes a Report query statement.</span></span> <span data-ttu-id="3c64e-105">De API retourneert slechts 100 records die u als partner kunt gebruiken om te controleren of de gegevens zijn zoals verwacht.</span><span class="sxs-lookup"><span data-stu-id="3c64e-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3c64e-106">Deze API heeft een time-out voor het uitvoeren van query's van 100 seconden.</span><span class="sxs-lookup"><span data-stu-id="3c64e-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="3c64e-107">Als u merkt dat de API meer dan 100 seconden duurt, is het zeer waarschijnlijk dat de query syntactisch juist is, anders zou u een andere foutcode dan 200 hebben ontvangen.</span><span class="sxs-lookup"><span data-stu-id="3c64e-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="3c64e-108">De werkelijke rapportgeneratie wordt doorgegeven als de querysyntaxis juist is.</span><span class="sxs-lookup"><span data-stu-id="3c64e-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="3c64e-109">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="3c64e-109">**Request syntax**</span></span>

|    <span data-ttu-id="3c64e-110">Methode</span><span class="sxs-lookup"><span data-stu-id="3c64e-110">Method</span></span>    |    <span data-ttu-id="3c64e-111">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="3c64e-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3c64e-112">GET</span><span class="sxs-lookup"><span data-stu-id="3c64e-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="3c64e-113">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="3c64e-113">**Request header**</span></span>

|    <span data-ttu-id="3c64e-114">Header</span><span class="sxs-lookup"><span data-stu-id="3c64e-114">Header</span></span>    |    <span data-ttu-id="3c64e-115">Type</span><span class="sxs-lookup"><span data-stu-id="3c64e-115">Type</span></span>    |    <span data-ttu-id="3c64e-116">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="3c64e-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="3c64e-117">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="3c64e-117">Authorization</span></span>    |    <span data-ttu-id="3c64e-118">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-118">string</span></span>    |    <span data-ttu-id="3c64e-119">Vereist.</span><span class="sxs-lookup"><span data-stu-id="3c64e-119">Required.</span></span> <span data-ttu-id="3c64e-120">Het Azure Active Directory (AAD) in het formulier`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="3c64e-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="3c64e-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3c64e-121">Content-Type</span></span>    |    <span data-ttu-id="3c64e-122">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="3c64e-123">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="3c64e-123">**Path parameter**</span></span>

<span data-ttu-id="3c64e-124">Geen</span><span class="sxs-lookup"><span data-stu-id="3c64e-124">None</span></span>

<span data-ttu-id="3c64e-125">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="3c64e-125">**Query parameter**</span></span>

|    <span data-ttu-id="3c64e-126">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="3c64e-126">Parameter Name</span></span>    |    <span data-ttu-id="3c64e-127">Type</span><span class="sxs-lookup"><span data-stu-id="3c64e-127">Type</span></span>    |    <span data-ttu-id="3c64e-128">Vereist</span><span class="sxs-lookup"><span data-stu-id="3c64e-128">Required</span></span>    |    <span data-ttu-id="3c64e-129">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="3c64e-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="3c64e-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="3c64e-130">exportQuery</span></span>     |    <span data-ttu-id="3c64e-131">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-131">string</span></span>    |    <span data-ttu-id="3c64e-132">No</span><span class="sxs-lookup"><span data-stu-id="3c64e-132">No</span></span>    |    <span data-ttu-id="3c64e-133">Rapportqueryreeks die moet worden uitgevoerd</span><span class="sxs-lookup"><span data-stu-id="3c64e-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="3c64e-134">queryId</span><span class="sxs-lookup"><span data-stu-id="3c64e-134">queryId</span></span>     |    <span data-ttu-id="3c64e-135">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-135">string</span></span>    |    <span data-ttu-id="3c64e-136">No</span><span class="sxs-lookup"><span data-stu-id="3c64e-136">No</span></span>    |    <span data-ttu-id="3c64e-137">Een geldige bestaande query-id.</span><span class="sxs-lookup"><span data-stu-id="3c64e-137">A valid existing query ID.</span></span> <span data-ttu-id="3c64e-138">Sluiten elkaar wederzijds uit met een queryreeks die is opgegeven in de parameter exportQuery</span><span class="sxs-lookup"><span data-stu-id="3c64e-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="3c64e-139">startTime</span><span class="sxs-lookup"><span data-stu-id="3c64e-139">startTime</span></span>     |    <span data-ttu-id="3c64e-140">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-140">string</span></span>    |    <span data-ttu-id="3c64e-141">No</span><span class="sxs-lookup"><span data-stu-id="3c64e-141">No</span></span>    |    <span data-ttu-id="3c64e-142">Begintijd van waaruit we de gegevens willen.</span><span class="sxs-lookup"><span data-stu-id="3c64e-142">Start time from which we want the data.</span></span> <span data-ttu-id="3c64e-143">De periode die is opgegeven in de query wordt overschreven</span><span class="sxs-lookup"><span data-stu-id="3c64e-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="3c64e-144">endTime</span><span class="sxs-lookup"><span data-stu-id="3c64e-144">endTime</span></span>     |    <span data-ttu-id="3c64e-145">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="3c64e-145">string</span></span>    |    <span data-ttu-id="3c64e-146">No</span><span class="sxs-lookup"><span data-stu-id="3c64e-146">No</span></span>    |    <span data-ttu-id="3c64e-147">Eindtijd tot we de gegevens willen.</span><span class="sxs-lookup"><span data-stu-id="3c64e-147">End time till which we want the data.</span></span> <span data-ttu-id="3c64e-148">De periode die is opgegeven in de query wordt overschreven</span><span class="sxs-lookup"><span data-stu-id="3c64e-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="3c64e-149">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="3c64e-149">**Request payload**</span></span>

<span data-ttu-id="3c64e-150">Geen</span><span class="sxs-lookup"><span data-stu-id="3c64e-150">None</span></span>

<span data-ttu-id="3c64e-151">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="3c64e-151">**Glossary**</span></span>

<span data-ttu-id="3c64e-152">Geen</span><span class="sxs-lookup"><span data-stu-id="3c64e-152">None</span></span>

<span data-ttu-id="3c64e-153">**Response**</span><span class="sxs-lookup"><span data-stu-id="3c64e-153">**Response**</span></span>

<span data-ttu-id="3c64e-154">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="3c64e-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="3c64e-155">Responscode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="3c64e-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="3c64e-156">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="3c64e-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="3c64e-157">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="3c64e-157">**Glossary**</span></span>

<span data-ttu-id="3c64e-158">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="3c64e-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="3c64e-159">Parameter</span><span class="sxs-lookup"><span data-stu-id="3c64e-159">Parameter</span></span>    |    <span data-ttu-id="3c64e-160">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="3c64e-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="3c64e-161">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="3c64e-161">TotalCount</span></span>     |    <span data-ttu-id="3c64e-162">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="3c64e-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="3c64e-163">Bericht</span><span class="sxs-lookup"><span data-stu-id="3c64e-163">Message</span></span>     |    <span data-ttu-id="3c64e-164">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="3c64e-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="3c64e-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="3c64e-165">StatusCode</span></span>     |    <span data-ttu-id="3c64e-166">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="3c64e-166">Result Code.</span></span> <span data-ttu-id="3c64e-167">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="3c64e-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
