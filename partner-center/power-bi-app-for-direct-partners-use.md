---
title: Gebruik Partner Center Analytics voor Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het weergeven van uw zakelijke gegevens met behulp van Analyse-app van het Partnercentrum voor Power BI (voor directe partners in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855026"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Uw zakelijke gegevens weergeven met de Partner Center Analytics-app voor Microsoft Power BI



**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Verkoopagent | Beheeragent

## <a name="view-your-business-data"></a>Uw bedrijfsgegevens weergeven

Krijg een visuele weergave van uw zakelijke gegevens met de Analyse-app van het Partnercentrum voor Power BI, waaronder:

- Groei van uw klantenbestand, abonnementen en licenties

- Gebruik van Office 365-, Microsoft Dynamics- en Microsoft Azure producten

- Dagelijkse verbruikseenheden voor elke resource naar gebruik in elk Azure-abonnement voor de afgelopen 60 dagen

- Geschatte kosten (op basis van de meest recente tariefkaart)

- Mogelijkheid om gegevenssets te exporteren en aangepaste rapporten te maken, inclusief per klant.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Over de preview Partner Center versie van de app Partner Center Analytics

- Deze app is alleen voor directe partners in Cloud Solution Provider programma. Andere partners in CSP (indirecte resellers, bijvoorbeeld) kunnen zich niet aanmelden.

- Geschatte kosten zijn facturerings-/factuurgegevens vóór belasting en zijn niet juridisch binding. Geschatte kosten zijn alleen bedoeld om te worden gebruikt voor gegevensinzichten.

- Klantgegevens zijn gebaseerd op abonnementen. Klanten voor wie u onlangs accounts hebt gemaakt, maar die nog geen abonnementen hebben, worden niet opgenomen in tellingen.

- De geschatte kosten zijn gebaseerd op de meest recente tariefkaart, die is gebaseerd op CSP-prijzen.

- Dagen zijn kalenderdagen.

### <a name="business-insights-report"></a>Business Insights-rapport

- **Tenants van klanten:** aantal afzonderlijke Azure AD-tenants van klanten die abonnementen hebben aangeschaft

- **Nieuw (afgelopen 30 dagen)**: Nieuwe klanten hebben in de afgelopen 30 dagen ten minste één abonnement aanschaffen

- **Verloop (afgelopen 30 dagen)**: Klanten zonder abonnementen 'actief', 'in respijt' of 'uitgeschakeld'.

- **Nieuw (afgelopen 24 uur)**: Nieuwe klanten hebben in de afgelopen 24 uur ten minste één abonnement aanschaffen

- **Geschatte maandelijkse kosten in** de afgelopen 12 maanden: Trend in maand van geschatte factuurbedrag vóór belasting, samengevoegd maandelijks in de periode van de afgelopen 12 maanden

- **Geschatte kosten per product in** de afgelopen 12 maanden: verkochte producten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 12 maanden. Deze status geeft aan dat de belangrijkste producten de meeste omzet opleveren.

- **Klanten in de afgelopen 12** maanden: Trend van nieuwe klanten en verloopklanten per maand gedurende de periode van de afgelopen 12 maanden

- **Geschatte kosten per klant in** de afgelopen 12 maanden: Klanten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 12 maanden. Deze status geeft aan dat de belangrijkste klanten de meeste omzet genereren.

- **Aantal klanten per product:** verkochte producten gesorteerd op gekoppelde klanten. Deze status geeft de belangrijkste producten aan die aan de meeste klanten zijn verkocht.

### <a name="subscription-insights-report"></a>Abonnementsinzichten-rapport

- **Abonnementsstatus:**

- Actief: Abonnementen die behoren tot de status Actief of In respijtperiode

  - Tijdelijk: Abonnementen die behoren tot de status Uitgeschakeld

  - De-provisioned: Abonnementen die behoren tot de status 'de-provisioned' of 'expired'

- **Verloopstatus:**

  - Verlopen: Abonnementen die al zijn verlopen (waarbij de einddatum van het abonnement in het verleden ligt)

  - Verloopt na 30 dagen: Abonnementen die na 30 dagen verlopen (waarbij de einddatum van het abonnement na de volgende 30 dagen valt)

  - Verloopt binnen 30 dagen: Abonnementen die binnen de volgende 30 dagen verlopen (waarbij de einddatum van het abonnement tussen vandaag en de volgende 30 dagen ligt)

- **Totaal aantal abonnementen:** Abonnementen met de status Actief, In respijtperiode of Uitgeschakeld

- **Nieuw (afgelopen 30 dagen)**: Nieuwe abonnementen die zijn gekocht door klanten in de afgelopen 30 dagen

- **Nieuw (afgelopen 24 uur)**: Nieuwe abonnementen die zijn gekocht door klanten in de afgelopen 24 uur

- **Verloopt over 30 dagen:** abonnementen die binnen de komende 30 dagen verlopen

- **Verloop (afgelopen 30 dagen)**: Abonnementen die de inrichting in de afgelopen 30 dagen zijn beëindigd of tijdelijk zijn beëindigd (uitgeschakeld)

- **Distributie op abonnementstypen:**% distributie van het totale aantal abonnementen op basis van licenties en abonnementstypen op basis van gebruik

- **Aantal actieve abonnementen per product:** verkochte producten gesorteerd op aantal actieve abonnementen

- **Abonnementen in de afgelopen 12** maanden: trend van maand tot maand voor nieuwe abonnementen en verloopabonnementen die maandelijks zijn samengevoegd in de afgelopen 12 maanden

- **Details van klantabonnement:** gedetailleerde weergave van de klanten, abonnementen en aanbiedingen

### <a name="license-insights-report"></a>License Insights-rapport:

- **Totaal aantal licenties:** totaal aantal licenties dat is geaggregeerd voor alle op licenties gebaseerde abonnementen

- **Nieuw (afgelopen 30 dagen)**: Optelling van licentie in de afgelopen 30 dagen

- **Verloop (afgelopen 30 dagen)**: Licentievermindering binnen de afgelopen 30 dagen

- **Nieuw (afgelopen 24 uur)**: Optelling van licenties in de afgelopen 24 uur

- **Licenties in de afgelopen 90** dagen: de trend van maandelijkse toevoegingen en verlagingen van licenties die maandelijks zijn geaggregeerd in de afgelopen 90 dagen

- **Aantal actieve licenties per product:** verkochte producten gesorteerd op aantal actieve licenties

- **Aantal actieve licenties per klant:** klanten gesorteerd op aantal actieve licenties

- **Gebeurtenisdetails** van klantlicenties in de afgelopen 90 dagen: gedetailleerde weergave van de klanten, abonnementen en abonnementsgebeurtenissen, waaronder gebeurtenisdatum, gebeurtenisnaam, hoeveelheid en wijziging in hoeveelheid.

### <a name="licenses-usage-report"></a>Gebruiksrapport licenties:

- **Licenties die zijn toegewezen per product:** verkochte producten gesorteerd op aantal licentietoewijzingen

- **Licenties die worden gebruikt door product:** Verkochte producten gesorteerd op aantal licenties

- **Klantdistributie van toegewezen** licenties: % distributie van het totale aantal klanten, opgesplitst in buckets van 20% bereik op licentietoewijzing %

- **Klantdistributie van licenties in gebruik:**% distributie van het totale aantal klanten, opgesplitst in buckets van 20% bereik op licentiegebruik %

- **Licenties die zijn toegewezen door de klant:** gedetailleerde weergave van verkochte licenties en licenties die zijn toegewezen door klanten en producten

- **Licenties die door de klant worden gebruikt:** gedetailleerde weergave van verkochte licenties en licenties die worden gebruikt door klanten en producten

### <a name="azure-insights-report"></a>Azure Insights-rapport:

- Op gebruik gebaseerde klanten in de afgelopen **12** maanden: Trend van maandelijks nieuwe op gebruik gebaseerde klanten en op basis van verloop van gebruik gebaseerde klanten die maandelijks zijn geaggregeerd in de periode van de afgelopen 12 maanden

- Abonnementen op basis van gebruik in de afgelopen **12** maanden: trend van maand tot maand voor nieuwe op gebruik gebaseerde abonnementen en abonnementen op basis van verloop, maandelijks samengevoegd in de periode van de afgelopen 12 maanden

- **Geschatte gebruikskosten** per klant in de afgelopen 60 dagen: op gebruik gebaseerde klanten gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de afgelopen 60 dagen. Deze status geeft aan dat de belangrijkste klanten op basis van gebruik de meeste omzet genereren

- **Geschatte gebruikskosten per** categorie gedurende de afgelopen 60 dagen: Metercategorieën van op gebruik gebaseerde abonnementen gesorteerd op geschatte factuurbedrag vóór belasting, geaggregeerd in de periode van de afgelopen 60 dagen.

- **Geschatte gebruikskosten per** abonnement gedurende de afgelopen 60 dagen: Abonnementen op basis van gebruik op basis van geschatte factuurbedragen vóór belasting, geaggregeerd in de afgelopen 60 dagen.

- **Geschatte gebruikskosten van de klant op uitgavenbudget:** Klanten gesorteerd op percentage van hun huidige gebruiksbestedingsbudget dat de drempelwaarde overschrijdt (100%).

### <a name="azure-resource-usage-report"></a>Rapport azure-resourcegebruik:

- **Gebruik van Azure-resources per dag** voor de geselecteerde periode: dagelijkse verbruikseenheden voor elke resource naar gebruik in elk abonnement op basis van gebruik voor de geselecteerde periode in de afgelopen 60 dagen.

- **Geschatte gebruikskosten van Azure-resources** voor de geselecteerde periode: Geschatte kosten op basis van de kaart met het meest recente tarief voor elke resource naar gebruik in elk abonnement op basis van gebruik voor de geselecteerde periode in de afgelopen 60 dagen. 

## <a name="next-steps"></a>Volgende stappen

- [Partner Center Analytics voor Power BI-app](power-bi-app-for-direct-partners.md)

- [Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Partner Center Analytics-app voor Microsoft Power BI installeren en preview bekijken)
