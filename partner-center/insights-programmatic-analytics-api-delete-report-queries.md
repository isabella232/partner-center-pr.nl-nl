---
title: API voor rapportquery's verwijderen - Insights verwijderen
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze API om door de gebruiker gedefinieerde query's in Partner Center verwijderen.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376518"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="25926-103">API voor rapportquery's verwijderen</span><span class="sxs-lookup"><span data-stu-id="25926-103">Delete report queries API</span></span>

<span data-ttu-id="25926-104">Met deze API worden door de gebruiker gedefinieerde query's verwijderd.</span><span class="sxs-lookup"><span data-stu-id="25926-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="25926-105">**Aanvraagsyntaxis**</span><span class="sxs-lookup"><span data-stu-id="25926-105">**Request syntax**</span></span>

|    <span data-ttu-id="25926-106">Methode</span><span class="sxs-lookup"><span data-stu-id="25926-106">Method</span></span>    |    <span data-ttu-id="25926-107">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="25926-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="25926-108">DELETE</span><span class="sxs-lookup"><span data-stu-id="25926-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="25926-109">**Aanvraagheader**</span><span class="sxs-lookup"><span data-stu-id="25926-109">**Request header**</span></span>

|    <span data-ttu-id="25926-110">Header</span><span class="sxs-lookup"><span data-stu-id="25926-110">Header</span></span>    |    <span data-ttu-id="25926-111">Type</span><span class="sxs-lookup"><span data-stu-id="25926-111">Type</span></span>    |    <span data-ttu-id="25926-112">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="25926-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="25926-113">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="25926-113">Authorization</span></span>    |    <span data-ttu-id="25926-114">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="25926-114">string</span></span>    |    <span data-ttu-id="25926-115">Vereist.</span><span class="sxs-lookup"><span data-stu-id="25926-115">Required.</span></span> <span data-ttu-id="25926-116">Het Azure Active Directory (AAD) in het formulier`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="25926-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="25926-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="25926-117">Content-Type</span></span>    |    <span data-ttu-id="25926-118">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="25926-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="25926-119">**Padparameter**</span><span class="sxs-lookup"><span data-stu-id="25926-119">**Path parameter**</span></span>

|    <span data-ttu-id="25926-120">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="25926-120">Parameter Name</span></span>    |    <span data-ttu-id="25926-121">Type</span><span class="sxs-lookup"><span data-stu-id="25926-121">Type</span></span>    |    <span data-ttu-id="25926-122">Vereist</span><span class="sxs-lookup"><span data-stu-id="25926-122">Required</span></span>    |    <span data-ttu-id="25926-123">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="25926-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="25926-124">queryId</span><span class="sxs-lookup"><span data-stu-id="25926-124">queryId</span></span>     |    <span data-ttu-id="25926-125">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="25926-125">string</span></span>     |    <span data-ttu-id="25926-126">No</span><span class="sxs-lookup"><span data-stu-id="25926-126">No</span></span>    |    <span data-ttu-id="25926-127">Filter om details op te halen van alleen query's met de id die is opgegeven in het argument</span><span class="sxs-lookup"><span data-stu-id="25926-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="25926-128">**Queryparameter**</span><span class="sxs-lookup"><span data-stu-id="25926-128">**Query parameter**</span></span>

<span data-ttu-id="25926-129">Geen</span><span class="sxs-lookup"><span data-stu-id="25926-129">None</span></span>

<span data-ttu-id="25926-130">**Nettolading aanvragen**</span><span class="sxs-lookup"><span data-stu-id="25926-130">**Request payload**</span></span>

<span data-ttu-id="25926-131">Geen</span><span class="sxs-lookup"><span data-stu-id="25926-131">None</span></span>

<span data-ttu-id="25926-132">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="25926-132">**Glossary**</span></span>

<span data-ttu-id="25926-133">Geen</span><span class="sxs-lookup"><span data-stu-id="25926-133">None</span></span>

<span data-ttu-id="25926-134">**Response**</span><span class="sxs-lookup"><span data-stu-id="25926-134">**Response**</span></span>

<span data-ttu-id="25926-135">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="25926-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="25926-136">Responscode: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="25926-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="25926-137">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="25926-137">Response payload example:</span></span>

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

<span data-ttu-id="25926-138">**Woordenlijst**</span><span class="sxs-lookup"><span data-stu-id="25926-138">**Glossary**</span></span>

<span data-ttu-id="25926-139">Deze tabel definieert de belangrijkste elementen in het antwoord:</span><span class="sxs-lookup"><span data-stu-id="25926-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="25926-140">Parameter</span><span class="sxs-lookup"><span data-stu-id="25926-140">Parameter</span></span>    |    <span data-ttu-id="25926-141">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="25926-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="25926-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="25926-142">QueryId</span></span>     |    <span data-ttu-id="25926-143">Unieke UUID van de query die is verwijderd</span><span class="sxs-lookup"><span data-stu-id="25926-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="25926-144">Name</span><span class="sxs-lookup"><span data-stu-id="25926-144">Name</span></span>     |    <span data-ttu-id="25926-145">Naam van de query die is verwijderd</span><span class="sxs-lookup"><span data-stu-id="25926-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="25926-146">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="25926-146">Description</span></span>     |    <span data-ttu-id="25926-147">Beschrijving van de verwijderde query</span><span class="sxs-lookup"><span data-stu-id="25926-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="25926-148">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="25926-148">Query</span></span>     |    <span data-ttu-id="25926-149">Rapportqueryreeks van de verwijderde query</span><span class="sxs-lookup"><span data-stu-id="25926-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="25926-150">Type</span><span class="sxs-lookup"><span data-stu-id="25926-150">Type</span></span>     |    <span data-ttu-id="25926-151">Ingesteld op userDefined voor door de gebruiker gemaakte query's</span><span class="sxs-lookup"><span data-stu-id="25926-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="25926-152">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="25926-152">User</span></span>     |    <span data-ttu-id="25926-153">Gebruikers-id die de query heeft gemaakt</span><span class="sxs-lookup"><span data-stu-id="25926-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="25926-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="25926-154">CreatedTime</span></span>     |    <span data-ttu-id="25926-155">Tijdstip van het maken van de query</span><span class="sxs-lookup"><span data-stu-id="25926-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="25926-156">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="25926-156">TotalCount</span></span>     |    <span data-ttu-id="25926-157">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="25926-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="25926-158">Bericht</span><span class="sxs-lookup"><span data-stu-id="25926-158">Message</span></span>     |    <span data-ttu-id="25926-159">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="25926-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="25926-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="25926-160">StatusCode</span></span>     |    <span data-ttu-id="25926-161">Resultaatcode.</span><span class="sxs-lookup"><span data-stu-id="25926-161">Result Code.</span></span> <span data-ttu-id="25926-162">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="25926-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
