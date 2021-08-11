---
title: Veelvoorkomende vragen voor programmatische toegang tot partnerinzichten
description: Krijg antwoorden op veelgestelde vragen over toegang tot partnerinzichtgegevens via API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5edfc720f2f9014d7532935fcfadc64260f721f7af57eda81994c710b6492df9
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115692361"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Veelgestelde vragen over programmatische toegang tot analysegegevens

In dit artikel worden veelgestelde vragen beantwoord over het programmatisch openen van partnerinzichtgegevens in Partner Center.

## <a name="api-responses"></a>API-antwoorden

Wat zijn de verschillende scenario's waarin ik een ander API-antwoord dan 200 (Geslaagd) kan ontvangen?

In deze tabel worden de API-antwoorden beschreven en wat u moet doen als u ze ontvangt.

|    Foutbeschrijving     |    Foutcode     |    Problemen oplossen     |
|    ----    |    ----    |    ----    |
|    Niet geautoriseerd     |    401     |    Dit is een verificatie-uitzondering. Controleer de juistheid van het Azure Active Directory (AAD)-token. Het AAD-token is 60 minuten geldig, waarna u het AAD-token opnieuw moet maken.     |
|    Ongeldige tabelnaam     |    400     |    De naam van de gegevensset is onjuist. Controleer de naam van de gegevensset opnieuw door de API Alle gegevenssets op te halen aan te roepen.     |
|    Onjuiste kolomnaam     |    400     |    De naam van de kolom in de query is onjuist. Controleer de kolomnaam opnieuw door de API Alle gegevenssets op te halen aan te roepen of door te verwijzen naar de kolomnamen in de gegevensdefinities    |
|    Null of ontbrekende waarde     |    400     |    Mogelijk ontbreken verplichte parameters als onderdeel van de nettolading van de aanvraag van de API.     |
|    Ongeldige rapportparameters     |    400     |    Zorg ervoor dat de rapportparameters juist zijn. U kunt bijvoorbeeld een waarde van minder dan 4 opgeven voor parameter RecurrenceInterval.     |
|    Terugkeerpatrooninterval moet tussen 4 en 2160 zijn     |    400     |    Zorg ervoor dat de waarde van de aanvraagparameter RecurrenceInterval tussen 4 en 2160 ligt.     |
|    Ongeldige QueryId     |    400     |    Controleer de gegenereerde QueryId opnieuw.     |
|    Ongeldige rapportparameters voor het maken- Begintijd van rapport moet ten minste 4 uur vanaf de huidige UTC-tijd zijn     |    400     |    De parameter Begintijd als onderdeel van de nettolading van de aanvraag mag niet in het verleden zijn. De begintijd van het rapport moet ten minste 4 uur vanaf de huidige UTC-tijd zijn.     |
|    Aangevraagde waarde 'tekenreeks' niet gevonden     |    400     |    Controleer of u de aanvraagparameters of `callbackurl` -indeling hebt bijgewerkt.     |
|    Er is geen item gevonden met opgegeven filters.     |    404     |    Controleer de parameter reportID die wordt gebruikt in de API Rapportuitvoeringen krijgen.     |
|    Er zijn geen uitvoeringen opgetreden voor de opgegeven filtervoorwaarden. Controleer de reportId of executionId en open de API opnieuw na de geplande uitvoeringstijd van het rapport     |    404     |    Zorg ervoor dat de reportId juist is. Open de API opnieuw na de geplande uitvoeringstijd van het rapport, zoals opgegeven in de nettolading van de aanvraag.     |
|    Er is een interne fout opgetreden tijdens het maken van een rapport. Correlatie-id <>     |    500     |    Zorg ervoor dat de datumnotatie voor de velden *StartTime,* *QueryStartTime* en *QueryEndTime* juist is.     |
|    Service niet beschikbaar    |    500     |    Als u continu een service ontvangt die niet beschikbaar is (5xx-fout), opent u een ondersteuningsticket.    |
|        |        |        |

## <a name="no-records"></a>Geen records

Ik ontvang API-antwoord 200 wanneer ik het rapport download van de beveiligde locatie. Waarom krijg ik geen records?
Controleer of de tekenreeks in de query een van de toegestane waarden voor de kolomkop heeft. Met deze query worden bijvoorbeeld nul resultaten retourneren:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

In dit voorbeeld zijn de toegestane waarden `IsDuplicateRowForPGA` voor 0 of 1. Raadpleeg de [gegevensdefinities](insights-data-definitions.md) voor alle mogelijke waarden voor de verschillende kolommen.
