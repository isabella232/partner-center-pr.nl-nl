---
title: Lijst met API's voor toegang tot partnerinzichtgegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lijst met API's voor toegang tot partnerinzichtgegevens.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376573"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="e3b00-103">Beschikbare API's voor analyse van partnerinzichten</span><span class="sxs-lookup"><span data-stu-id="e3b00-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="e3b00-104">Hieronder vindt u de lijst met API's voor analyse van partnerinzichten en de bijbehorende functies.</span><span class="sxs-lookup"><span data-stu-id="e3b00-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="e3b00-105">Pull-API's voor gegevenssets</span><span class="sxs-lookup"><span data-stu-id="e3b00-105">Dataset pull APIs</span></span>

<span data-ttu-id="e3b00-106">***Tabel 1: Pull-API's voor gegevenssets***</span><span class="sxs-lookup"><span data-stu-id="e3b00-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="e3b00-107">**API**</span><span class="sxs-lookup"><span data-stu-id="e3b00-107">**API**</span></span> | <span data-ttu-id="e3b00-108">**Functionaliteit**</span><span class="sxs-lookup"><span data-stu-id="e3b00-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="e3b00-109">Alle gegevenssets op halen</span><span class="sxs-lookup"><span data-stu-id="e3b00-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="e3b00-110">Haalt alle beschikbare gegevenssets op.</span><span class="sxs-lookup"><span data-stu-id="e3b00-110">Gets all the available datasets.</span></span> <span data-ttu-id="e3b00-111">Gegevenssets maken een lijst van de tabellen, kolommen, metrische gegevens en tijdsbereiken.</span><span class="sxs-lookup"><span data-stu-id="e3b00-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="e3b00-112">API's voor querybeheer</span><span class="sxs-lookup"><span data-stu-id="e3b00-112">Query management APIs</span></span>

<span data-ttu-id="e3b00-113">***Tabel 2: Api's voor querybeheer***</span><span class="sxs-lookup"><span data-stu-id="e3b00-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="e3b00-114">**API**</span><span class="sxs-lookup"><span data-stu-id="e3b00-114">**API**</span></span> | <span data-ttu-id="e3b00-115">**Functionaliteit**</span><span class="sxs-lookup"><span data-stu-id="e3b00-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="e3b00-116">Rapportquery maken</span><span class="sxs-lookup"><span data-stu-id="e3b00-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="e3b00-117">Hiermee maakt u aangepaste query's die de gegevensset definiëren van waaruit kolommen en metrische gegevens moeten worden geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="e3b00-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="e3b00-118">GET-rapportquery</span><span class="sxs-lookup"><span data-stu-id="e3b00-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="e3b00-119">Haalt alle query's op die beschikbaar zijn voor gebruik in rapporten.</span><span class="sxs-lookup"><span data-stu-id="e3b00-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="e3b00-120">Haalt standaard alle systeem- en door de gebruiker gedefinieerde query's op.</span><span class="sxs-lookup"><span data-stu-id="e3b00-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="e3b00-121">DELETE Report Query</span><span class="sxs-lookup"><span data-stu-id="e3b00-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="e3b00-122">Hiermee verwijdert u door de gebruiker gedefinieerde query's.</span><span class="sxs-lookup"><span data-stu-id="e3b00-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="e3b00-123">API's voor rapportbeheer</span><span class="sxs-lookup"><span data-stu-id="e3b00-123">Report management APIs</span></span>

<span data-ttu-id="e3b00-124">***Tabel 3: API's voor rapportbeheer***</span><span class="sxs-lookup"><span data-stu-id="e3b00-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="e3b00-125">**API**</span><span class="sxs-lookup"><span data-stu-id="e3b00-125">**API**</span></span> | <span data-ttu-id="e3b00-126">**Functionaliteit**</span><span class="sxs-lookup"><span data-stu-id="e3b00-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="e3b00-127">Rapport maken</span><span class="sxs-lookup"><span data-stu-id="e3b00-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="e3b00-128">Een query wordt gepland om regelmatig te worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="e3b00-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="e3b00-129">RAPPORTquery UITPROBEREN</span><span class="sxs-lookup"><span data-stu-id="e3b00-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="e3b00-130">Hiermee wordt een query-instructie rapport uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="e3b00-130">Executes a Report query statement.</span></span> <span data-ttu-id="e3b00-131">Retourneert slechts 10 records die een partner kan gebruiken om te controleren of de gegevens zijn zoals verwacht.</span><span class="sxs-lookup"><span data-stu-id="e3b00-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="e3b00-132">Rapport ophalen</span><span class="sxs-lookup"><span data-stu-id="e3b00-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="e3b00-133">Haal alle rapporten op die zijn gepland.</span><span class="sxs-lookup"><span data-stu-id="e3b00-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="e3b00-134">Rapport bijwerken</span><span class="sxs-lookup"><span data-stu-id="e3b00-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="e3b00-135">Wijzig een rapportparameter.</span><span class="sxs-lookup"><span data-stu-id="e3b00-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="e3b00-136">Rapport verwijderen</span><span class="sxs-lookup"><span data-stu-id="e3b00-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="e3b00-137">Hiermee verwijdert u alle records voor de uitvoering van het rapport en het rapport.</span><span class="sxs-lookup"><span data-stu-id="e3b00-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="e3b00-138">Rapportuitvoeringen onderbreken</span><span class="sxs-lookup"><span data-stu-id="e3b00-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="e3b00-139">Pauzeert de geplande uitvoering van rapporten.</span><span class="sxs-lookup"><span data-stu-id="e3b00-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="e3b00-140">Rapportuitvoeringen hervatten</span><span class="sxs-lookup"><span data-stu-id="e3b00-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="e3b00-141">Hervat de geplande uitvoering van een onderbroken rapport.</span><span class="sxs-lookup"><span data-stu-id="e3b00-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="e3b00-142">Pull-API's voor rapportuitvoering</span><span class="sxs-lookup"><span data-stu-id="e3b00-142">Report execution pull APIs</span></span>

<span data-ttu-id="e3b00-143">***Tabel 4: Pull-API's voor rapportuitvoering***</span><span class="sxs-lookup"><span data-stu-id="e3b00-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="e3b00-144">**API**</span><span class="sxs-lookup"><span data-stu-id="e3b00-144">**API**</span></span> | <span data-ttu-id="e3b00-145">**Functionaliteit**</span><span class="sxs-lookup"><span data-stu-id="e3b00-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="e3b00-146">Rapportuitvoeringen krijgen</span><span class="sxs-lookup"><span data-stu-id="e3b00-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="e3b00-147">Haal alle uitvoeringen op die voor een bepaald rapport zijn uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="e3b00-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="e3b00-148">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="e3b00-148">Next steps</span></span>

- <span data-ttu-id="e3b00-149">U kunt de API's uitproberen via de [Swagger API-URL.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="e3b00-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>