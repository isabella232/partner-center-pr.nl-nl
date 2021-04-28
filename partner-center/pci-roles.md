---
title: Partner Center op rollen gebaseerde toegang tot Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de specifieke rollen die nodig zijn voor het bekijken Partner Center Insights-rapporten. Dit zijn onder andere de rollen Executive Report Viewer en Report Viewer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120780"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Op rollen gebaseerd toegangsbeheer voor het Partner Center Insights-dashboard

**Juiste rollen**

- Globale beheerder
- Beheeragent
- Rapportviewer
- Rapportviewer voor leidinggevenden

Het dashboard Insights gebruikt twee nieuwe rollen in Partner Center toegang van werknemers tot de rapporten te beheren: Executive Report Viewer en Report Viewer.  Gebruikers met de rol Executive Report Viewer hebben toegang tot alle rapportagegegevenssets, terwijl gebruikers met de rol Rapportviewer geen toegang hebben tot gevoelige gegevenssets zoals omzet en persoonlijke gegevens van klanten/werknemers.  

Net als bij Partner Center rollen, kan de globale beheerder of de accountbeheerder gebruikers toewijzen aan deze rollen op de pagina Gebruikersbeheer. De rollen kunnen van toepassing zijn voor het hele bedrijf of voor specifieke MPN-locaties. Rollen die zijn toegewezen voor specifieke MPN-locatie(s) beperken de gebruiker tot het weergeven van rapportagegegevens die alleen zijn gekoppeld aan de geselecteerde MPN-locatie(s). Partner kan een of meer locaties selecteren in de onderstaande weergave.

:::image type="content" source="images/pci/roles.png" alt-text="Toont locatiespecifieke instellingen Partner Center Insights-rollen voor Rapportviewer en Executive Report Viewer.":::

>[!Note]
> Gebruikers die vanaf 20 januari 2020 MPN-beheerders zijn, worden automatisch toegevoegd aan de bedrijfsbrede rol Executive **Report Viewer** voor alle locaties voor die tenant. Deze gebruikers hebben dus toegang tot de rapporten als executive rapportviewer zonder expliciete actie die is vereist door de globale beheerder of accountbeheerder. De globale beheerders en accountbeheerders kunnen de automatisch toegewezen rollen van deze gebruikers overschrijven om hun mogelijkheden verder te vergroten of te beperken.

## <a name="next-steps"></a>Volgende stappen

- Meer informatie over [Partner Center en de](partner-center-insights.md) verschillende rapporten.
