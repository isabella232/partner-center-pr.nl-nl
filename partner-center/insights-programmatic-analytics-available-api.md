---
title: Lijst met API's voor toegang tot partnerinzichtgegevens
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Lijst met API's voor toegang tot partnerinzichtgegevens.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: cbd9f7fd08dfc4cfd247a0ed07a2c12845c5514c
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244893"
---
# <a name="available-apis-for-partner-insights-analytics"></a>Beschikbare API's voor analyse van partnerinzichten

Hieronder vindt u een lijst met API's voor analyse van partnerinzichten en de bijbehorende functies.

## <a name="dataset-pull-apis"></a>Pull-API's voor gegevenssets

***Tabel 1: Pull-API's voor gegevenssets***

| **API** | **Functionaliteit** |
| --- | --- |
| [Alle gegevenssets op halen](insights-programmatic-analytics-api-get-dataset.md) | Haalt alle beschikbare gegevenssets op. Gegevenssets maken een lijst van de tabellen, kolommen, metrische gegevens en tijdsbereiken. |
|||

## <a name="query-management-apis"></a>API's voor querybeheer

***Tabel 2: Api's voor querybeheer***

| **API** | **Functionaliteit** |
| --- | --- |
| [Rapportquery maken](insights-programmatic-access-paradigm.md#create-report-query-api) | Hiermee maakt u aangepaste query's die de gegevensset definiëren van waaruit kolommen en metrische gegevens moeten worden geëxporteerd. |
| [GET-rapportquery](insights-programmatic-analytics-api-get-report-queries.md) | Haalt alle query's op die beschikbaar zijn voor gebruik in rapporten. Haalt standaard alle systeem- en door de gebruiker gedefinieerde query's op. |
| [DELETE Report Query](insights-programmatic-analytics-api-delete-report-queries.md) | Hiermee verwijdert u door de gebruiker gedefinieerde query's. |
|||

## <a name="report-management-apis"></a>API's voor rapportbeheer

***Tabel 3: API's voor rapportbeheer***

| **API** | **Functionaliteit** |
| --- | --- |
| [Rapport maken](insights-programmatic-access-paradigm.md#create-report-api) | Een query wordt gepland om regelmatig te worden uitgevoerd. |
| [RAPPORTquery UITPROBEREN](insights-programmatic-analytics-api-try-report-queries.md) | Hiermee wordt een rapportquery-instructie uitgevoerd. Retourneert slechts 10 records die een partner kan gebruiken om te controleren of de gegevens zijn zoals verwacht. |
| [Rapport ophalen](insights-programmatic-analytics-api-get-report.md) | Haal alle rapporten op die zijn gepland. |
| [Rapport bijwerken](insights-programmatic-analytics-api-update-report.md) | Wijzig een rapportparameter. |
| [Rapport verwijderen](insights-programmatic-analytics-api-delete-report.md) | Hiermee verwijdert u alle records voor de uitvoering van het rapport en het rapport. |
| [Rapportuitvoeringen onderbreken](insights-programmatic-analytics-api-pause-report-executions.md) | Pauzeert de geplande uitvoering van rapporten. |
| [Rapportuitvoeringen hervatten](insights-programmatic-analytics-api-resume-report-executions.md) | Hervat de geplande uitvoering van een onderbroken rapport. |
|||

## <a name="report-execution-pull-apis"></a>Pull-API's voor rapportuitvoering

***Tabel 4: Pull-API's voor rapportuitvoering***

| **API** | **Functionaliteit** |
| --- | --- |
| [Rapportuitvoeringen krijgen](insights-programmatic-access-paradigm.md#get-report-execution-api) | Haal alle uitvoeringen op die voor een bepaald rapport zijn uitgevoerd. |
|||

## <a name="next-steps"></a>Volgende stappen

- U kunt de API's uitproberen via de [Swagger API-URL.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)