---
title: Programmatisch toegangsparadigma voor Insights gegevens
description: Informatie over de stroom op hoog niveau van het API-aanroeppatroon voor programmatische analyses. De API's voor toegang tot analyserapporten van partnerinzichten worden ook behandeld.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376519"
---
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="a8fc3-104">Programmatisch toegangsparadigma</span><span class="sxs-lookup"><span data-stu-id="a8fc3-104">Programmatic access paradigm</span></span>

<span data-ttu-id="a8fc3-105">In dit diagram ziet u het API-aanroeppatroon dat wordt gebruikt om een nieuwe rapportsjabloon te maken, het aangepaste rapport te plannen en foutgegevens op te halen.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Stroom op hoog niveau":::
<span data-ttu-id="a8fc3-107">***Afbeelding 1: Stroom op hoog niveau van het API-aanroeppatroon***</span><span class="sxs-lookup"><span data-stu-id="a8fc3-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="a8fc3-108">Deze lijst bevat meer informatie over afbeelding 1.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="a8fc3-109">De clienttoepassing kan het aangepaste rapportschema/de aangepaste sjabloon definiëren door de [API rapportquery maken aan te roepen.](#create-report-query-api)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="a8fc3-110">U kunt ook een rapportsjabloon (QueryId) kiezen uit de voorbeelden van de rapportsjabloonbibliotheek die hier worden [vermeld.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="a8fc3-111">Als dit is gelukt, retourneert de API Rapportquery maken de QueryId.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="a8fc3-112">De clienttoepassing moet vervolgens [](#create-report-api) de API Rapport maken aanroepen met behulp van de QueryId, samen met de begindatum van het rapport, het herhalingsinterval, het terugkeerpatroon en een optionele callback-URI.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="a8fc3-113">Bij geslaagd retourneert [de API Rapport maken](#create-report-api) de ReportId.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="a8fc3-114">De clienttoepassing krijgt een melding via de callback-URL zodra de rapportgegevens gereed zijn om te worden gedownload.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="a8fc3-115">De clienttoepassing gebruikt vervolgens de [GET Report Executions-API om](#get-report-execution-api) de status van het rapport op te vragen met de rapport-id en het datumbereik.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="a8fc3-116">Als het downloaden van het rapport is geslaagd, wordt de koppeling geretourneerd en kan de toepassing het downloaden van de gegevens starten.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="a8fc3-117">Specificatie van rapportquerytaal</span><span class="sxs-lookup"><span data-stu-id="a8fc3-117">Report query language specification</span></span>

<span data-ttu-id="a8fc3-118">Hoewel we [systeemquery's bieden die](insights-programmatic-system-queries.md) u kunt gebruiken om rapporten te maken, kunt u ook uw eigen query's maken op basis van uw bedrijfsbehoeften.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="a8fc3-119">Zie Aangepaste queryspecificatie voor meer informatie [over aangepaste query's.](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="a8fc3-120">Rapportquery-API maken</span><span class="sxs-lookup"><span data-stu-id="a8fc3-120">Create report query API</span></span>

<span data-ttu-id="a8fc3-121">De API helpt bij het maken van aangepaste query's die de gegevensset definiëren van waaruit kolommen en metrische gegevens moeten worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="a8fc3-122">De API biedt de flexibiliteit om een nieuwe rapportagesjabloon te maken op basis van de behoeften van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="a8fc3-123">U kunt ook de [systeemquery's gebruiken die](insights-programmatic-system-queries.md) we bieden.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="a8fc3-124">Wanneer u geen aangepaste rapportsjablonen nodig hebt, kunt u [Rapport-API](#create-report-api) maken rechtstreeks aanroepen met behulp van de QueryIds van de systeemquery's die worden geleverd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="a8fc3-125">In het volgende voorbeeld ziet u hoe u een aangepaste query maakt om de top 10 klanten op te halen op omzet voor de afgelopen maand.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a8fc3-126">Aanvraagsyntaxis</span><span class="sxs-lookup"><span data-stu-id="a8fc3-126">Request syntax</span></span>

|    <span data-ttu-id="a8fc3-127">Methode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-127">Method</span></span>     |    <span data-ttu-id="a8fc3-128">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="a8fc3-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a8fc3-129">POST</span><span class="sxs-lookup"><span data-stu-id="a8fc3-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="a8fc3-130">Aanvraagheader</span><span class="sxs-lookup"><span data-stu-id="a8fc3-130">Request header</span></span>

|    <span data-ttu-id="a8fc3-131">Header</span><span class="sxs-lookup"><span data-stu-id="a8fc3-131">Header</span></span>     |    <span data-ttu-id="a8fc3-132">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-132">Type</span></span>     |    <span data-ttu-id="a8fc3-133">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a8fc3-134">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="a8fc3-134">Authorization</span></span>     |    <span data-ttu-id="a8fc3-135">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-135">string</span></span> |<span data-ttu-id="a8fc3-136">Vereist.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-136">Required.</span></span> <span data-ttu-id="a8fc3-137">Het Azure Active Directory -toegang token (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a8fc3-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a8fc3-138">De indeling is  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a8fc3-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-139">Content-Type</span></span>     |<span data-ttu-id="a8fc3-140">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="a8fc3-141">Padparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-141">Path parameter</span></span>

<span data-ttu-id="a8fc3-142">Geen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="a8fc3-143">Queryparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-143">Query parameter</span></span>

<span data-ttu-id="a8fc3-144">Geen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="a8fc3-145">Voorbeeld van nettolading van aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="a8fc3-146">Woordenlijst</span><span class="sxs-lookup"><span data-stu-id="a8fc3-146">Glossary</span></span>

<span data-ttu-id="a8fc3-147">Deze tabel bevat de belangrijkste definities van elementen in de nettolading van de aanvraag.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="a8fc3-148">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-148">Parameter</span></span>|    <span data-ttu-id="a8fc3-149">Vereist</span><span class="sxs-lookup"><span data-stu-id="a8fc3-149">Required</span></span>     |    <span data-ttu-id="a8fc3-150">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-150">Description</span></span>     |    <span data-ttu-id="a8fc3-151">Toegestane waarden</span><span class="sxs-lookup"><span data-stu-id="a8fc3-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="a8fc3-152">Name</span><span class="sxs-lookup"><span data-stu-id="a8fc3-152">Name</span></span> |    <span data-ttu-id="a8fc3-153">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-153">Yes</span></span>     |    <span data-ttu-id="a8fc3-154">Gebruiksvriendelijke naam van de query</span><span class="sxs-lookup"><span data-stu-id="a8fc3-154">Friendly name of the query</span></span>     |    <span data-ttu-id="a8fc3-155">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-155">string</span></span>     |
|    <span data-ttu-id="a8fc3-156">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-156">Description</span></span>     |    <span data-ttu-id="a8fc3-157">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-157">No</span></span>     |    <span data-ttu-id="a8fc3-158">Beschrijving van wat de query retourneert</span><span class="sxs-lookup"><span data-stu-id="a8fc3-158">Description of what the query returns</span></span>     |    <span data-ttu-id="a8fc3-159">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-159">string</span></span>     |
|    <span data-ttu-id="a8fc3-160">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="a8fc3-160">Query</span></span>     |    <span data-ttu-id="a8fc3-161">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-161">Yes</span></span>     |    <span data-ttu-id="a8fc3-162">Rapportqueryreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-162">Report query string</span></span>     |    <span data-ttu-id="a8fc3-163">Gegevenstype: tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-163">Data type: string</span></span> <br> <span data-ttu-id="a8fc3-164">[Aangepaste query op](insights-programmatic-custom-query.md) basis van bedrijfsvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="a8fc3-165">Zie Voorbeelden van voorbeeldquery's [voor voorbeelden van aangepaste query's.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="a8fc3-166">Voorbeeldantwoord</span><span class="sxs-lookup"><span data-stu-id="a8fc3-166">Sample response</span></span>

<span data-ttu-id="a8fc3-167">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="a8fc3-168">Responscodes: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="a8fc3-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="a8fc3-169">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-169">Response payload example:</span></span>

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a><span data-ttu-id="a8fc3-170">Woordenlijst</span><span class="sxs-lookup"><span data-stu-id="a8fc3-170">Glossary</span></span>

<span data-ttu-id="a8fc3-171">Deze tabel bevat de belangrijkste definities van elementen in de nettolading van de aanvraag.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="a8fc3-172">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-172">Parameter</span></span>     |    <span data-ttu-id="a8fc3-173">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="a8fc3-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-174">QueryId</span></span>     |    <span data-ttu-id="a8fc3-175">Universally Unique Identifier (UUID) van de query die u hebt gemaakt</span><span class="sxs-lookup"><span data-stu-id="a8fc3-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="a8fc3-176">Name</span><span class="sxs-lookup"><span data-stu-id="a8fc3-176">Name</span></span>     |    <span data-ttu-id="a8fc3-177">Gebruiksvriendelijke naam voor de query in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="a8fc3-178">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-178">Description</span></span>     |    <span data-ttu-id="a8fc3-179">Beschrijving gegeven tijdens het maken van de query</span><span class="sxs-lookup"><span data-stu-id="a8fc3-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="a8fc3-180">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="a8fc3-180">Query</span></span>     |    <span data-ttu-id="a8fc3-181">Rapportquery doorgegeven als invoer tijdens het maken van de query</span><span class="sxs-lookup"><span data-stu-id="a8fc3-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="a8fc3-182">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-182">Type</span></span>     |    <span data-ttu-id="a8fc3-183">Ingesteld op `userDefined`</span><span class="sxs-lookup"><span data-stu-id="a8fc3-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="a8fc3-184">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="a8fc3-184">User</span></span>     |    <span data-ttu-id="a8fc3-185">Gebruikers-id die wordt gebruikt om de query te maken</span><span class="sxs-lookup"><span data-stu-id="a8fc3-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="a8fc3-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-186">CreatedTime</span></span>     |    <span data-ttu-id="a8fc3-187">UTC-tijd dat de query is gemaakt in deze indeling: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8fc3-188">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="a8fc3-188">TotalCount</span></span>     |    <span data-ttu-id="a8fc3-189">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="a8fc3-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="a8fc3-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-190">StatusCode</span></span>     |    <span data-ttu-id="a8fc3-191">Resultaatcode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-191">Result Code</span></span> <br> <span data-ttu-id="a8fc3-192">De mogelijke waarden zijn 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="a8fc3-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="a8fc3-193">message</span><span class="sxs-lookup"><span data-stu-id="a8fc3-193">message</span></span>     |    <span data-ttu-id="a8fc3-194">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="a8fc3-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="a8fc3-195">Rapport-API maken</span><span class="sxs-lookup"><span data-stu-id="a8fc3-195">Create report API</span></span>

<span data-ttu-id="a8fc3-196">Wanneer u een aangepaste rapportsjabloon maakt [](#create-report-query-api) en de QueryID ontvangt als onderdeel van het antwoord Rapportquery maken, kan deze API worden aangeroepen om een query te plannen die regelmatig moet worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="a8fc3-197">U kunt een frequentie en planning instellen om het rapport te leveren.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="a8fc3-198">Voor systeemquery's die we bieden, kan de API rapport maken ook worden aangeroepen met [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="a8fc3-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="a8fc3-199">URL voor aanroep</span><span class="sxs-lookup"><span data-stu-id="a8fc3-199">Callback URL</span></span>

<span data-ttu-id="a8fc3-200">De API voor het maken van een rapport accepteert een callback-URL.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="a8fc3-201">Deze URL wordt aangeroepen zodra het genereren van het rapport is geslaagd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="a8fc3-202">De callback-URL moet openbaar bereikbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="a8fc3-203">Naast de URL kan ook een callback-methode worden gegeven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="a8fc3-204">De callback-methode kan alleen GET of POST zijn.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="a8fc3-205">De standaardmethode als er geen waarde wordt doorgegeven, is POST.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="a8fc3-206">De reportId die het genereren heeft voltooid, wordt altijd tijdens de callback terugverdiend.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="a8fc3-207">POST-callback: Als de doorgegeven URL is, wordt de teruggeroepen `https://www.contosso.com/callback` URL `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="a8fc3-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="a8fc3-208">GET-callback: als de doorgegeven URL is, wordt de teruggeroepen `https://www.contosso.com/callback` URL `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="a8fc3-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="a8fc3-209">ExecuteNow-rapporten</span><span class="sxs-lookup"><span data-stu-id="a8fc3-209">ExecuteNow reports</span></span>

<span data-ttu-id="a8fc3-210">Er is een inrichting voor het genereren van een rapport zonder planning.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="a8fc3-211">Het rapport API-nettolading maken kan een parameter accepteren, waardoor het rapport in dequeque wordt opgemaakt zodra de `ExecuteNow` API wordt aangeroepen.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="a8fc3-212">Wanneer `ExecuteNow` is ingesteld op true, worden de velden: , , genegeerd omdat deze rapporten niet zijn `StartTime` `RecurrenceCount` `RecurrenceInterval` gepland.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="a8fc3-213">Er kunnen twee extra velden worden doorgegeven wanneer `ExecuteNow` waar is, `QueryStartTime` en `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="a8fc3-214">Deze twee velden overschrijven het `TIMESPAN` veld in de query.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="a8fc3-215">Deze velden zijn niet van toepassing op geplande rapporten, omdat gegevens continu worden gegenereerd gedurende een vaste periode die niet verandert.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a8fc3-216">Aanvraagsyntaxis</span><span class="sxs-lookup"><span data-stu-id="a8fc3-216">Request syntax</span></span>

|    <span data-ttu-id="a8fc3-217">Methode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-217">Method</span></span>     |    <span data-ttu-id="a8fc3-218">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="a8fc3-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a8fc3-219">POST</span><span class="sxs-lookup"><span data-stu-id="a8fc3-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="a8fc3-220">Aanvraagheader</span><span class="sxs-lookup"><span data-stu-id="a8fc3-220">Request header</span></span>

|    <span data-ttu-id="a8fc3-221">Header</span><span class="sxs-lookup"><span data-stu-id="a8fc3-221">Header</span></span>     |    <span data-ttu-id="a8fc3-222">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-222">Type</span></span>     |    <span data-ttu-id="a8fc3-223">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a8fc3-224">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="a8fc3-224">Authorization</span></span>     |    <span data-ttu-id="a8fc3-225">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-225">string</span></span> |<span data-ttu-id="a8fc3-226">Vereist.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-226">Required.</span></span> <span data-ttu-id="a8fc3-227">Het Azure Active Directory -toegang token (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a8fc3-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a8fc3-228">De indeling is  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a8fc3-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-229">Content-Type</span></span>     |<span data-ttu-id="a8fc3-230">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="a8fc3-231">Padparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-231">Path Parameter</span></span>

<span data-ttu-id="a8fc3-232">Geen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="a8fc3-233">Queryparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-233">Query Parameter</span></span>

<span data-ttu-id="a8fc3-234">Geen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="a8fc3-235">Nettolading van voorbeeldaanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-235">Sample request payload</span></span>

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a><span data-ttu-id="a8fc3-236">Woordenlijst</span><span class="sxs-lookup"><span data-stu-id="a8fc3-236">Glossary</span></span>

<span data-ttu-id="a8fc3-237">De belangrijkste definities van elementen in de nettolading van de aanvraag worden hieronder verwoord:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="a8fc3-238">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-238">Parameter</span></span>     |    <span data-ttu-id="a8fc3-239">Vereist</span><span class="sxs-lookup"><span data-stu-id="a8fc3-239">Required</span></span>     |    <span data-ttu-id="a8fc3-240">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-240">Description</span></span>     |    <span data-ttu-id="a8fc3-241">Toegestane waarden</span><span class="sxs-lookup"><span data-stu-id="a8fc3-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a8fc3-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="a8fc3-242">ReportName</span></span>     |    <span data-ttu-id="a8fc3-243">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-243">Yes</span></span>     |    <span data-ttu-id="a8fc3-244">Naam die moet worden toegewezen aan het rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="a8fc3-245">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-245">string</span></span>     |
|    <span data-ttu-id="a8fc3-246">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-246">Description</span></span>     |    <span data-ttu-id="a8fc3-247">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-247">No</span></span>     |    <span data-ttu-id="a8fc3-248">Beschrijving van het gemaakte rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-248">Description of the created report</span></span>     |    <span data-ttu-id="a8fc3-249">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-249">string</span></span>     |
|    <span data-ttu-id="a8fc3-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-250">QueryId</span></span>     |    <span data-ttu-id="a8fc3-251">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-251">Yes</span></span>     |    <span data-ttu-id="a8fc3-252">Rapportquery-id</span><span class="sxs-lookup"><span data-stu-id="a8fc3-252">Report query ID</span></span>     |    <span data-ttu-id="a8fc3-253">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-253">string</span></span>     |
|    <span data-ttu-id="a8fc3-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-254">StartTime</span></span>     |    <span data-ttu-id="a8fc3-255">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-255">Yes</span></span>     |    <span data-ttu-id="a8fc3-256">UTC-tijdstempel waarop het genereren van het rapport begint.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="a8fc3-257">De indeling moet zijn: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="a8fc3-258">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-258">string</span></span>     |
|    <span data-ttu-id="a8fc3-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a8fc3-259">ExecuteNow</span></span>     |    <span data-ttu-id="a8fc3-260">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-260">No</span></span>     |    <span data-ttu-id="a8fc3-261">Deze parameter moet worden gebruikt om een rapport te maken dat slechts één keer wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="a8fc3-262">`StartTime`en `RecurrenceInterval` `RecurrenceCount` worden genegeerd als deze is ingesteld op true.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="a8fc3-263">Het rapport wordt onmiddellijk asynchroon uitgevoerd</span><span class="sxs-lookup"><span data-stu-id="a8fc3-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="a8fc3-264">waar/onwaar</span><span class="sxs-lookup"><span data-stu-id="a8fc3-264">true/false</span></span>     |
|    <span data-ttu-id="a8fc3-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-265">QueryStartTime</span></span>     |    <span data-ttu-id="a8fc3-266">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-266">No</span></span>     |    <span data-ttu-id="a8fc3-267">Hiermee geeft u optioneel de begintijd op voor de query die de gegevens extraheert.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="a8fc3-268">Deze parameter is alleen van toepassing voor een keer uitvoeringsrapport dat `ExecuteNow` is ingesteld op true.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="a8fc3-269">Als u deze parameter instelt, `TIMESPAN` worden de opgegeven in de query overschrijven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="a8fc3-270">De indeling moet yyyy-MM-ddTHH:mm:ssZ zijn</span><span class="sxs-lookup"><span data-stu-id="a8fc3-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="a8fc3-271">Tijdstempel als tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="a8fc3-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-272">QueryEndTime</span></span>     |    <span data-ttu-id="a8fc3-273">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-273">No</span></span>     |    <span data-ttu-id="a8fc3-274">Hiermee geeft u desgewenst de eindtijd op voor het extraheren van de gegevens door de query.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="a8fc3-275">Deze parameter is alleen van toepassing voor een keer uitvoeringsrapport dat `ExecuteNow` is ingesteld op true.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="a8fc3-276">Als u deze parameter instelt, `TIMESPAN` worden de opgegeven in de query overschrijven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="a8fc3-277">De indeling moet yyyy-MM-ddTHH:mm:ssZ zijn</span><span class="sxs-lookup"><span data-stu-id="a8fc3-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="a8fc3-278">Tijdstempel als tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="a8fc3-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="a8fc3-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="a8fc3-280">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-280">Yes</span></span>     |    <span data-ttu-id="a8fc3-281">Frequentie in uren waarop het rapport moet worden gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="a8fc3-282">Minimumwaarde is 4 en Maximumwaarde is 2160.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="a8fc3-283">geheel getal</span><span class="sxs-lookup"><span data-stu-id="a8fc3-283">integer</span></span>     |
|    <span data-ttu-id="a8fc3-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="a8fc3-284">RecurrenceCount</span></span>     |    <span data-ttu-id="a8fc3-285">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-285">No</span></span>     |    <span data-ttu-id="a8fc3-286">Het aantal rapporten dat moet worden gegenereerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="a8fc3-287">geheel getal</span><span class="sxs-lookup"><span data-stu-id="a8fc3-287">integer</span></span>     |
|    <span data-ttu-id="a8fc3-288">Indeling</span><span class="sxs-lookup"><span data-stu-id="a8fc3-288">Format</span></span>     |    <span data-ttu-id="a8fc3-289">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-289">No</span></span>     |    <span data-ttu-id="a8fc3-290">Bestandsindeling van het geëxporteerde bestand.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-290">File format of the exported file.</span></span> <br> <span data-ttu-id="a8fc3-291">De standaardwaarde is CSV.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-291">Default is CSV.</span></span>    |    <span data-ttu-id="a8fc3-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="a8fc3-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="a8fc3-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a8fc3-293">CallbackUrl</span></span>     |    <span data-ttu-id="a8fc3-294">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-294">No</span></span>     |    <span data-ttu-id="a8fc3-295">Openbaar bereikbare URL die optioneel kan worden geconfigureerd als callback-bestemming</span><span class="sxs-lookup"><span data-stu-id="a8fc3-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="a8fc3-296">Tekenreeks (HTTP-URL)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-296">String (http URL)</span></span>     |
|    <span data-ttu-id="a8fc3-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a8fc3-297">CallbackMethod</span></span>     |    <span data-ttu-id="a8fc3-298">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-298">No</span></span>     |    <span data-ttu-id="a8fc3-299">De methode die moet worden gebruikt voor callback</span><span class="sxs-lookup"><span data-stu-id="a8fc3-299">The method to be used for callback</span></span>     |    <span data-ttu-id="a8fc3-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="a8fc3-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="a8fc3-301">Voorbeeldantwoord</span><span class="sxs-lookup"><span data-stu-id="a8fc3-301">Sample response</span></span>

<span data-ttu-id="a8fc3-302">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="a8fc3-303">Antwoordcodes: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a8fc3-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a8fc3-304">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-304">Response payload example:</span></span>

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a><span data-ttu-id="a8fc3-305">Woordenlijst</span><span class="sxs-lookup"><span data-stu-id="a8fc3-305">Glossary</span></span>

<span data-ttu-id="a8fc3-306">De belangrijkste definities van elementen in het antwoord worden hieronder verwoord:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="a8fc3-307">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-307">Parameter</span></span>     |    <span data-ttu-id="a8fc3-308">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="a8fc3-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-309">ReportId</span></span>     |    <span data-ttu-id="a8fc3-310">Universally Unique Identifier (UUID) van het rapport dat u hebt gemaakt</span><span class="sxs-lookup"><span data-stu-id="a8fc3-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="a8fc3-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="a8fc3-311">ReportName</span></span>     |    <span data-ttu-id="a8fc3-312">Naam van het rapport in de nettolading van de aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="a8fc3-313">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-313">Description</span></span>     |    <span data-ttu-id="a8fc3-314">Beschrijving gegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="a8fc3-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-315">QueryId</span></span>     |    <span data-ttu-id="a8fc3-316">Query-id doorgegeven op het moment dat u het rapport hebt gemaakt</span><span class="sxs-lookup"><span data-stu-id="a8fc3-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="a8fc3-317">Query’s uitvoeren</span><span class="sxs-lookup"><span data-stu-id="a8fc3-317">Query</span></span>     |    <span data-ttu-id="a8fc3-318">Querytekst die wordt uitgevoerd voor dit rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="a8fc3-319">Gebruiker</span><span class="sxs-lookup"><span data-stu-id="a8fc3-319">User</span></span>     |    <span data-ttu-id="a8fc3-320">Gebruikers-id die wordt gebruikt om het rapport te maken</span><span class="sxs-lookup"><span data-stu-id="a8fc3-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="a8fc3-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-321">CreatedTime</span></span>     |    <span data-ttu-id="a8fc3-322">UTC-tijd dat het rapport is gemaakt in deze indeling: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8fc3-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-323">ModifiedTime</span></span>     |    <span data-ttu-id="a8fc3-324">UTC Tijd dat het rapport voor het laatst is gewijzigd in deze indeling: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8fc3-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a8fc3-325">ExecuteNow</span></span>     |    <span data-ttu-id="a8fc3-326">`ExecuteNow` de vlag die is ingesteld op het moment dat het rapport is gemaakt</span><span class="sxs-lookup"><span data-stu-id="a8fc3-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="a8fc3-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-327">StartTime</span></span>     |    <span data-ttu-id="a8fc3-328">UTC Tijd dat de uitvoering van het rapport in deze indeling begint: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a8fc3-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="a8fc3-329">ReportStatus</span></span>     |    <span data-ttu-id="a8fc3-330">Status van de uitvoering van het rapport.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-330">Status of the report execution.</span></span> <span data-ttu-id="a8fc3-331">De mogelijke waarden zijn `Paused` , `Active` en `Inactive`</span><span class="sxs-lookup"><span data-stu-id="a8fc3-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="a8fc3-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="a8fc3-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="a8fc3-333">Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="a8fc3-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="a8fc3-334">RecurrenceCount</span></span>     |    <span data-ttu-id="a8fc3-335">Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="a8fc3-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a8fc3-336">CallbackUrl</span></span>     |    <span data-ttu-id="a8fc3-337">Callback-URL die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="a8fc3-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a8fc3-338">CallbackMethod</span></span>     |    <span data-ttu-id="a8fc3-339">Callback-methode die is opgegeven in de aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="a8fc3-340">Indeling</span><span class="sxs-lookup"><span data-stu-id="a8fc3-340">Format</span></span>     |    <span data-ttu-id="a8fc3-341">Indeling van de rapportbestanden.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-341">Format of the report files.</span></span> <span data-ttu-id="a8fc3-342">De mogelijke waarden zijn `CSV` of `TSV` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="a8fc3-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a8fc3-343">TotalCount</span></span>     |    <span data-ttu-id="a8fc3-344">Aantal records in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="a8fc3-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="a8fc3-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-345">StatusCode</span></span>     |    <span data-ttu-id="a8fc3-346">Resultaatcode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-346">Result Code</span></span>     |
|    <span data-ttu-id="a8fc3-347">message</span><span class="sxs-lookup"><span data-stu-id="a8fc3-347">message</span></span>     |    <span data-ttu-id="a8fc3-348">De mogelijke waarden zijn 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="a8fc3-349">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="a8fc3-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="a8fc3-350">API voor rapportuitvoeringen krijgen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-350">Get report execution API</span></span>

<span data-ttu-id="a8fc3-351">U kunt deze methode gebruiken om de status van een rapportuitvoering op te vragen met behulp van de ReportId die u hebt ontvangen [van De rapport-API maken.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="a8fc3-352">De methode retourneert de downloadkoppeling voor het rapport als het rapport gereed is om te worden gedownload.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="a8fc3-353">Anders retourneert de methode de status.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="a8fc3-354">U kunt deze API ook gebruiken om alle uitvoeringen op te halen die voor een bepaald rapport zijn uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="a8fc3-355">Voor deze API zijn standaardqueryparameters ingesteld `executionStatus=Completed` voor en `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="a8fc3-356">Als u de API aanroept voordat het rapport voor de eerste keer wordt uitgevoerd, wordt er dus 404 als uitvoerder gebruikt.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="a8fc3-357">Uitvoeringen in behandeling kunnen worden verkregen door in te `executionStatus=Pending` stellen.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="a8fc3-358">Aanvraagsyntaxis</span><span class="sxs-lookup"><span data-stu-id="a8fc3-358">Request syntax</span></span>

|    <span data-ttu-id="a8fc3-359">Methode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-359">Method</span></span>     |    <span data-ttu-id="a8fc3-360">Aanvraag-URI</span><span class="sxs-lookup"><span data-stu-id="a8fc3-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="a8fc3-361">GET</span><span class="sxs-lookup"><span data-stu-id="a8fc3-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="a8fc3-362">Aanvraagheader</span><span class="sxs-lookup"><span data-stu-id="a8fc3-362">Request header</span></span>

|    <span data-ttu-id="a8fc3-363">Header</span><span class="sxs-lookup"><span data-stu-id="a8fc3-363">Header</span></span>     |    <span data-ttu-id="a8fc3-364">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-364">Type</span></span>     |    <span data-ttu-id="a8fc3-365">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="a8fc3-366">Autorisatie</span><span class="sxs-lookup"><span data-stu-id="a8fc3-366">Authorization</span></span>     |    <span data-ttu-id="a8fc3-367">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-367">string</span></span> |<span data-ttu-id="a8fc3-368">Vereist.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-368">Required.</span></span> <span data-ttu-id="a8fc3-369">Het Azure Active Directory -toegang token (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a8fc3-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="a8fc3-370">De indeling is  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="a8fc3-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-371">Content-Type</span></span>     |<span data-ttu-id="a8fc3-372">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="a8fc3-373">Padparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-373">Path parameter</span></span>

|    <span data-ttu-id="a8fc3-374">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="a8fc3-374">Parameter Name</span></span>    |    <span data-ttu-id="a8fc3-375">Vereist</span><span class="sxs-lookup"><span data-stu-id="a8fc3-375">Required</span></span>    |    <span data-ttu-id="a8fc3-376">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-376">Type</span></span>    |    <span data-ttu-id="a8fc3-377">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a8fc3-378">reportId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-378">reportId</span></span>    |    <span data-ttu-id="a8fc3-379">Ja</span><span class="sxs-lookup"><span data-stu-id="a8fc3-379">Yes</span></span>    |    <span data-ttu-id="a8fc3-380">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-380">string</span></span>    |    <span data-ttu-id="a8fc3-381">Filter om alleen uitvoeringsdetails van rapporten op te halen met de reportId die in dit argument is opgegeven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="a8fc3-382">Meerdere reportIds kunnen worden opgegeven door ze te scheiden met een puntkomma ;".</span><span class="sxs-lookup"><span data-stu-id="a8fc3-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="a8fc3-383">Queryparameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-383">Query parameter</span></span>

|    <span data-ttu-id="a8fc3-384">Parameternaam</span><span class="sxs-lookup"><span data-stu-id="a8fc3-384">Parameter Name</span></span>    |    <span data-ttu-id="a8fc3-385">Vereist</span><span class="sxs-lookup"><span data-stu-id="a8fc3-385">Required</span></span>    |    <span data-ttu-id="a8fc3-386">Type</span><span class="sxs-lookup"><span data-stu-id="a8fc3-386">Type</span></span>    |    <span data-ttu-id="a8fc3-387">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a8fc3-388">executionId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-388">executionId</span></span>    |    <span data-ttu-id="a8fc3-389">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-389">No</span></span>    |    <span data-ttu-id="a8fc3-390">tekenreeks</span><span class="sxs-lookup"><span data-stu-id="a8fc3-390">string</span></span>    |    <span data-ttu-id="a8fc3-391">Filter om alleen details van rapporten op te halen met de executionId die in dit argument is opgegeven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="a8fc3-392">Meerdere executionIds kunnen worden opgegeven door ze te scheiden met een puntkomma ;".</span><span class="sxs-lookup"><span data-stu-id="a8fc3-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="a8fc3-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="a8fc3-393">executionStatus</span></span>    |    <span data-ttu-id="a8fc3-394">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-394">No</span></span>    |    <span data-ttu-id="a8fc3-395">Tekenreeks/enum</span><span class="sxs-lookup"><span data-stu-id="a8fc3-395">String/enum</span></span>    |    <span data-ttu-id="a8fc3-396">Filter om alleen details van rapporten met de executionStatus in dit argument op te halen.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="a8fc3-397">Geldige waarden zijn: `Pending` `Running` , en `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="a8fc3-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="a8fc3-398">De standaardwaarde is `Completed`.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="a8fc3-399">Meerdere statussen kunnen worden opgegeven door ze te scheiden met een puntkomma ;".</span><span class="sxs-lookup"><span data-stu-id="a8fc3-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="a8fc3-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="a8fc3-400">getLatestExecution</span></span>    |    <span data-ttu-id="a8fc3-401">Nee</span><span class="sxs-lookup"><span data-stu-id="a8fc3-401">No</span></span>    |    <span data-ttu-id="a8fc3-402">booleaans</span><span class="sxs-lookup"><span data-stu-id="a8fc3-402">boolean</span></span>    |    <span data-ttu-id="a8fc3-403">De API retournt gegevens over de meest recente uitvoering.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="a8fc3-404">Deze parameter is standaard ingesteld op true.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="a8fc3-405">Als u ervoor kiest om de waarde van deze parameter als onwaar door te geven, retourneert de API de uitvoerings-exemplaren van de afgelopen 90 dagen.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="a8fc3-406">Voorbeeld van nettolading van aanvraag</span><span class="sxs-lookup"><span data-stu-id="a8fc3-406">Sample Request Payload</span></span>

<span data-ttu-id="a8fc3-407">Geen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="a8fc3-408">Voorbeeldreactie</span><span class="sxs-lookup"><span data-stu-id="a8fc3-408">Sample Response</span></span>

<span data-ttu-id="a8fc3-409">De nettolading van het antwoord is als volgt gestructureerd:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="a8fc3-410">Responscodes: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a8fc3-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a8fc3-411">Voorbeeld van nettolading van antwoord:</span><span class="sxs-lookup"><span data-stu-id="a8fc3-411">Response payload example:</span></span>

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

<span data-ttu-id="a8fc3-412">Zodra de uitvoering van het rapport is voltooid, wordt de `Completed` uitvoeringsstatus weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="a8fc3-413">U kunt het rapport downloaden door de URL in de te `reportAccessSecureLink` selecteren.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="a8fc3-414">Woordenlijst</span><span class="sxs-lookup"><span data-stu-id="a8fc3-414">Glossary</span></span>

<span data-ttu-id="a8fc3-415">Belangrijkste definities van elementen in het antwoord.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="a8fc3-416">Parameter</span><span class="sxs-lookup"><span data-stu-id="a8fc3-416">Parameter</span></span>    |    <span data-ttu-id="a8fc3-417">Beschrijving</span><span class="sxs-lookup"><span data-stu-id="a8fc3-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a8fc3-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-418">ExecutionId</span></span>    |    <span data-ttu-id="a8fc3-419">Universally Unique Identifier (UUID) van het uitvoerings exemplaar</span><span class="sxs-lookup"><span data-stu-id="a8fc3-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="a8fc3-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="a8fc3-420">ReportId</span></span>    |    <span data-ttu-id="a8fc3-421">Rapport-id die is gekoppeld aan het uitvoerings exemplaar</span><span class="sxs-lookup"><span data-stu-id="a8fc3-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="a8fc3-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="a8fc3-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="a8fc3-423">Terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="a8fc3-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="a8fc3-424">RecurrenceCount</span></span>    |    <span data-ttu-id="a8fc3-425">Aantal terugkeerpatroon dat is opgegeven tijdens het maken van het rapport</span><span class="sxs-lookup"><span data-stu-id="a8fc3-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="a8fc3-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a8fc3-426">CallbackUrl</span></span>    |    <span data-ttu-id="a8fc3-427">Callback-URL die is gekoppeld aan het uitvoeringsin exemplaar</span><span class="sxs-lookup"><span data-stu-id="a8fc3-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="a8fc3-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a8fc3-428">CallbackMethod</span></span>    |    <span data-ttu-id="a8fc3-429">Callback-methode die is gekoppeld aan het uitvoeringsin exemplaar</span><span class="sxs-lookup"><span data-stu-id="a8fc3-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="a8fc3-430">Indeling</span><span class="sxs-lookup"><span data-stu-id="a8fc3-430">Format</span></span>    |    <span data-ttu-id="a8fc3-431">Indeling van het gegenereerde bestand aan het einde van de uitvoering</span><span class="sxs-lookup"><span data-stu-id="a8fc3-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="a8fc3-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="a8fc3-432">ExecutionStatus</span></span>    |    <span data-ttu-id="a8fc3-433">Status van het exemplaar van de uitvoering van het rapport.</span><span class="sxs-lookup"><span data-stu-id="a8fc3-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="a8fc3-434">Geldige waarden zijn: `Pending` `Running` , , `Paused` en `Completed`</span><span class="sxs-lookup"><span data-stu-id="a8fc3-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="a8fc3-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="a8fc3-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="a8fc3-436">Koppeling waarmee het rapport veilig kan worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="a8fc3-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="a8fc3-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="a8fc3-438">UTC-tijd waarna de rapportkoppeling verloopt in deze indeling: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="a8fc3-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="a8fc3-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="a8fc3-440">UTC-tijd waarop het rapport is gegenereerd in deze indeling: yyyy-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="a8fc3-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="a8fc3-441">Totaal aantal</span><span class="sxs-lookup"><span data-stu-id="a8fc3-441">TotalCount</span></span>    |    <span data-ttu-id="a8fc3-442">Aantal gegevenssets in de matrix Waarde</span><span class="sxs-lookup"><span data-stu-id="a8fc3-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="a8fc3-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-443">StatusCode</span></span>    |    <span data-ttu-id="a8fc3-444">Resultaatcode</span><span class="sxs-lookup"><span data-stu-id="a8fc3-444">Result Code</span></span> <br> <span data-ttu-id="a8fc3-445">De mogelijke waarden zijn 200, 400, 401, 403, 404 en 500</span><span class="sxs-lookup"><span data-stu-id="a8fc3-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="a8fc3-446">message</span><span class="sxs-lookup"><span data-stu-id="a8fc3-446">message</span></span>    |    <span data-ttu-id="a8fc3-447">Statusbericht van de uitvoering van de API</span><span class="sxs-lookup"><span data-stu-id="a8fc3-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="a8fc3-448">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="a8fc3-448">Next steps</span></span>

- <span data-ttu-id="a8fc3-449">Probeer de API's uit via de [Swagger API-URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="a8fc3-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="a8fc3-450">Uw eerste API-aanroep maken</span><span class="sxs-lookup"><span data-stu-id="a8fc3-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)