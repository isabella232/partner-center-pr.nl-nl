---
title: Partner Center Analytics voor Power BI gebruiken
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het weer geven van uw zakelijke gegevens met behulp van de Partner Center Analytics-App voor Power BI (voor rechtstreekse partners in CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633859"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Uw bedrijfs gegevens weer geven met de Partner Center Analytics-App voor micro soft Power BI



**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Verkoop agent
- Beheer agent

## <a name="view-your-business-data"></a>Uw zakelijke gegevens weer geven

Maak een visuele representatie van uw bedrijfs gegevens met de Partner Center Analytics-App voor Power BI, met inbegrip van:

- De groei van uw klanten basis, abonnementen en licenties

- Gebruik van Office 365-, micro soft Dynamics-en Microsoft Azure-producten

- Dagelijkse verbruiks eenheden voor elke resource met data limiet in elk Azure-abonnement gedurende de afgelopen 60 dagen

- Geschatte kosten (op basis van de meest recente tarieven kaart)

- De mogelijkheid om gegevens sets te exporteren en aangepaste rapporten te maken, inclusief per klant.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>De preview-versie van app Center Analytics-apps

- Deze app is alleen voor directe partners in het Cloud Solution Provider-programma. Andere partners in CSP (bijvoorbeeld indirecte wederverkopers) kunnen zich niet aanmelden.

- Alle geschatte kosten zijn facturen voor facturering/factuur vooraf en zijn niet juridisch bindend. Geschatte kosten zijn alleen bedoeld voor gebruik voor data Insights.

- Klant gegevens zijn gebaseerd op abonnementen. Klanten waarvoor u onlangs accounts hebt gemaakt, maar die nog geen abonnementen hebben, worden niet opgenomen in aantallen.

- De geschatte kosten zijn gebaseerd op de meest recente tarief kaart, die is gebaseerd op CSP-prijzen.

- Dagen zijn kalender dagen.

### <a name="business-insights-report"></a>Rapport van Business Insights

- **Tenants van klanten**: aantal afzonderlijke Azure AD-tenants van klanten die hebben gekochte abonnementen

- **Nieuw (afgelopen 30 dagen)**: nieuwe klanten die in de afgelopen 30 dagen ten minste één abonnement kopen

- **Verloop (afgelopen 30 dagen)**: klanten zonder ' Active ', ' in respijt ' of ' uitgeschakelde ' abonnementen

- **Nieuw (afgelopen 24 uur)**: nieuwe klanten hebben ten minste één abonnement in de afgelopen 24 uur kopen

- **Geschatte maandelijkse kosten gedurende de afgelopen 12 maanden**: maand over maand trend van het geschatte vooraf-BTW-factuur bedrag, geaggregeerd maandelijks voor de periode van afgelopen 12 maanden

- **Geschatte kosten per product gedurende een periode van 12 maanden**: verkochte producten, gesorteerd op basis van het geschatte bedrag vóór de BTW-factuur, geaggregeerd over de periode van de afgelopen 12 maanden. Deze status geeft aan dat de belangrijkste producten de meeste omzet.

- **Klanten in de afgelopen 12 maanden**: maand over maand trend van nieuwe klanten en verloop klanten die maandelijks zijn geaggregeerd over de periode van de afgelopen 12 maanden

- **Geschatte kosten per klant gedurende de afgelopen 12 maanden**: klanten gesorteerd op geschat bedrag factuur vooraf BTW, geaggregeerd over de periode van afgelopen 12 maanden. Deze status geeft aan dat de belangrijkste klanten de meeste omzet.

- **Aantal klanten per product**: verkochte producten gesorteerd op gekoppelde klanten. Deze status duidt op de belangrijkste producten die aan de meeste klanten worden verkocht.

### <a name="subscription-insights-report"></a>Rapport met abonnement Insights

- **Abonnements status**:

- Actief: abonnementen die horen bij de status ' actief ' of ' in de respijt periode '

  - Onderbroken: abonnementen die horen bij de status ' uitgeschakeld '

  - Niet-ingericht: abonnementen die horen bij de status ' niet-ingericht ' of ' verlopen '

- **Verloop status**:

  - Verlopen: abonnementen die al zijn verlopen (waarbij de eind datum van het abonnement in het verleden ligt)

  - Verlopen na 30 dagen: abonnementen die na 30 dagen verlopen (waarbij de eind datum van het abonnement na de volgende 30 dagen valt)

  - Verloopt over 30 dagen: abonnementen die binnen de komende 30 dagen verlopen (waarbij de eind datum van het abonnement tussen vandaag en de volgende 30 dagen ligt)

- **Totaal aantal abonnementen**: abonnementen in actief, in de respijt periode of de status uitgeschakeld

- **Nieuw (afgelopen 30 dagen)**: nieuwe abonnementen die klanten in de afgelopen 30 dagen zijn aangeschaft

- **Nieuw (afgelopen 24 uur)**: nieuwe abonnementen die klanten in de afgelopen 24 uur zijn aangeschaft

- **Verloopt over 30 dagen**: abonnementen die binnen de komende 30 dagen verlopen

- **Verloop (afgelopen 30 dagen)**: abonnementen die in de afgelopen 30 dagen zijn uitgezet of geblokkeerd (uitgeschakeld)

- **Distributie per abonnements** type:% distributie van het totale aantal abonnementen per licentie op basis van en op gebruik gebaseerd abonnement

- **Aantal actieve abonnementen per product**: verkochte producten gesorteerd op actief aantal abonnementen

- **Abonnementen over de afgelopen 12 maanden**: maand over maand trend van nieuwe abonnementen en verloop abonnementen die maandelijks worden geaggregeerd over de periode van afgelopen 12 maanden

- **Details van klant abonnement**: gedetailleerd overzicht van de klanten, abonnementen en aanbiedingen

### <a name="license-insights-report"></a>Licentie Insights-rapport:

- **Totale licenties**: totaal aantal licenties dat is geaggregeerd op alle abonnementen op basis van licenties

- **Nieuw (afgelopen 30 dagen)**: licentie toevoeging binnen de afgelopen 30 dagen

- **Verloop (laatste 30 dagen)**: licentie reductie binnen de afgelopen 30 dagen

- **Nieuw (afgelopen 24 uur)**: licentie toevoeging in de afgelopen 24 uur

- **Licenties gedurende de afgelopen 90 dagen**: maand over maand trend van licentie toevoegingen en kortingen die maandelijks worden geaggregeerd over de periode van afgelopen 90 dagen

- **Aantal actieve licenties per product**: verkochte producten gesorteerd op aantal actieve licenties

- **Aantal actieve licenties per klant**: klanten gesorteerd op aantal actieve licenties

- **Details van de klant licentie gebeurtenis gedurende de afgelopen 90 dagen**: gedetailleerde weer gave van de evenementen klanten, abonnementen en abonnementen, waaronder gebeurtenis datum, gebeurtenis naam, hoeveelheid en wijziging in hoeveelheid.

### <a name="licenses-usage-report"></a>Gebruiks rapport licenties:

- **Licenties die zijn toegewezen door product**: verkochte producten gesorteerd op aantal licenties toewijzingen

- **Licenties die worden gebruikt door product**: verkochte producten gesorteerd op aantal licenties gebruik

- **Klant distributie van verleende licenties**:% distributie van totaal aantal klanten verbroken in buckets van 20% bereik per licentie toewijzing%

- **Klant distributie van in gebruik** zijnde licenties:% distributie van totaal aantal klanten die zijn gebroken in buckets met een licentie gebruik%

- **Licenties die zijn toegewezen door de klant**: gedetailleerde weer gave van licenties die worden verkocht en licenties die zijn toegewezen door klanten en producten

- **Licenties die worden gebruikt door de klant**: gedetailleerde weer gave van licenties die worden verkocht en licenties die worden gebruikt door klanten en producten

### <a name="azure-insights-report"></a>Azure Insights-rapport:

- **Klanten op basis van gebruik gedurende de afgelopen 12 maanden**: maand over maand trend van nieuwe op gebruik gebaseerde klanten en klanten die zijn gebaseerd op het gebruik van getijden op basis van verbruik, zijn maandelijks geaggregeerd over de periode van de afgelopen 12 maanden

- **Op gebruik gebaseerde abonnementen gedurende de afgelopen 12 maanden**: maand over maand trend van nieuwe op gebruik gebaseerde abonnementen en gespreide, op basis van gebruik geplaatste abonnementen maandelijks voor de periode van afgelopen 12 maanden

- **Geschatte kosten voor gebruik door de klant gedurende de afgelopen 60 dagen**: op gebruik gebaseerde klanten, gesorteerd op geschat bedrag factuur vooraf BTW, geaggregeerd over de periode van afgelopen 60 dagen. Deze status geeft aan dat klanten op het hoogste gebruik de meeste omzet

- **Geschatte kosten van gebruik per categorie gedurende de afgelopen 60 dagen**: meter categorieën van op gebruik gebaseerde abonnementen, gesorteerd op het geschatte bedrag vóór de BTW-factuur, geaggregeerd over de periode van de afgelopen 60 dagen.

- **Geschatte kosten voor gebruik per abonnement gedurende de afgelopen 60 dagen**: op gebruik gebaseerde abonnementen op geraamde pre-BTW factuur bedrag, geaggregeerd over de periode van de afgelopen 60 dagen.

- **Geschatte gebruiks kosten van klanten per uitgaven budget**: klanten die zijn gesorteerd op percentage van hun huidige bestedings budget overschrijden de drempel waarde (100%).

### <a name="azure-resource-usage-report"></a>Azure resource gebruik-rapport:

- **Gebruik van Azure-resources per dag voor de geselecteerde periode**: dagelijks verbruiks eenheden voor elke resource met data limiet in elk op gebruik gebaseerd abonnement voor geselecteerde periode in de afgelopen 60 dagen.

- **Geschatte gebruiks kosten van Azure-resources voor de geselecteerde periode**: geschatte kosten op basis van de meest recente tarieven kaart voor elke resource met een licentie in elk op gebruik gebaseerd abonnement voor geselecteerde periode in de afgelopen 60 dagen. 

## <a name="next-steps"></a>Volgende stappen

- [Overzicht van partner Center Analytics for Power BI-app](power-bi-app-for-direct-partners.md)

- [Install and preview the Partner Center Analytics app for Microsoft Power BI](power-bi-app-for-direct-partners-install.md) (Partner Center Analytics-app voor Microsoft Power BI installeren en preview bekijken)
