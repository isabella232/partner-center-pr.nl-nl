---
title: Partner Center Insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Houd de gebruikers in uw bedrijf bij door gebruik te maken van gegevens over afzonderlijke training, voltooide modules, voltooide leertrajecten en meer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 132583352e1697a2f9dfa624eb9532692be6d734
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152627"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>In Microsoft Learn analytics-rapport ziet u de status van studenten in uw bedrijf

**Juiste rollen:** globale | MPN-partnerbeheerder

Het Microsoft Learn bevat informatie over de studenten in uw bedrijf, inclusief de modules die ze hebben voltooid en de leertrajecten die ze volgen. In het rapport wordt de status van elke afzonderlijke learner weergegeven. De globale beheerder en de MPN-beheerder voor uw bedrijf kunnen de gegevens bekijken.

## <a name="how-to-read-the-report"></a>Het rapport lezen

### <a name="summary-charts"></a>Samenvattingsdiagrammen

Deze grafieken geven een overzicht van het aantal en de maandelijkse cumulatieve trends voor getrainde personen, voltooiing van modules en leertrajecten.


**Aantal getrainde** personen: een telling van alle afzonderlijke studenten die ten minste één module hebben voltooid tijdens het geselecteerde datumbereik 

**Trend-minigrafiek getrainde personen:** het cumulatieve aantal actieve studenten per maand 

**Aantal module-voltooiingen:** aantal module-voltooiingen door de studenten in het bedrijf van de partner tijdens het geselecteerde datumbereik.
Als 'Module 1' bijvoorbeeld wordt voltooid door 15 personen en module 2 is voltooid door dezelfde 15 personen, is het aantal voltooiingen van de module 30. De voltooiingsdatum van de module moet binnen het geselecteerde datumbereik vallen.

**Module-voltooiingen trend-minigrafiek:** cumulatief aantal modules per maand 

**Aantal voltooiingen van leertraject:** aantal voltooiingen van leertrajecten door de studenten in het bedrijf van de partner tijdens het geselecteerde datumbereik.
Als het leertraject 'Pad 1' bijvoorbeeld wordt voltooid door 20 personen en het leertraject 'pad 2' is voltooid door dezelfde 20 personen, is het aantal voltooiingen van het leertraject 40. De voltooiingsdatum van het leertraject moet binnen het geselecteerde datumbereik vallen.

**Trend minigrafiek** voor voltooiing van leertraject: cumulatief aantal van de maand tot de voltooiing van het leertraject 

### <a name="trained-individuals-monthly-trend"></a>De maandelijkse trend van getrainde personen

Deze gegevens zijn de trend van de gebruikers van uw bedrijf die een module voor het eerst in die maand hebben voltooid. 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal actieve studenten dat zich in die maand heeft geregistreerd (de eerste keer dat een module is voltooid). Dit is niet cumulatief.

### <a name="module-completions-monthly-trend"></a>Module-voltooiingen trend per maand

Deze gegevens zijn de trend van modules die gedurende die maand door alle gebruikers van uw bedrijf zijn voltooid. (niet cumulatief) 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal voltooiingen van de module in die maand. Dit is niet cumulatief.

### <a name="learning-path-completions-monthly-trend"></a>De maandelijkse trend voor voltooiing van het leertraject

Deze gegevens zijn de trend van leertrajecten die de gebruikers van uw bedrijf in die maand hebben voltooid. (niet cumulatief) 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal module-voltooiingen in die maand. Dit is niet cumulatief.

### <a name="learning-path-completion-tabs"></a>Tabbladen voor het voltooien van leertrajecten 

**Tabblad Module**

Dit tabblad bevat uitsplitsing van modules die in uw bedrijf zijn voltooid op de namen van de vijf belangrijkste modules; het product waaraan de module is gekoppeld; en de gebruikersrol die relevant is voor de module.  

- Module-voltooiingen-donutgrafiek: uitsplitsing van de module-voltooiingen (aantal weergegeven in de samenvattingssectie) op de modulenamen.

Het getal dat in het midden van de grafiek wordt weergegeven, is het totale aantal voltooide modules

- Voltooiingen per rol: uitsplitsing van de module-voltooiingen op de rol van de module. Als een module is gekoppeld aan meerdere rollen, wordt elk van de rollen toegevoegd aan het aantal module-voltooiingen.

Het getal dat wordt weergegeven in het midden van de grafiek is het aantal afzonderlijke rollen voor de voltooiing van de module. 

- Voltooiingen per product: uitsplitsing van de voltooiingen van de module op het product waar de module aan is toegesneden. Als een module is gekoppeld aan meerdere producten, wordt elk van de producten toegevoegd aan het aantal module-voltooiingen.    

Het getal dat in het midden van de grafiek wordt weergegeven, is het aantal afzonderlijke producten voor de voltooiing van de module.  

**Tabblad Leertraject**   

Dit tabblad bevat een uitsplitsing van de leertrajecten die in uw bedrijf zijn voltooid op de vijf belangrijkste modulenamen; het product waar het leertraject aan is toegesneden; en de rol die relevant is voor dit leertraject.  

- Cirkeldiagram met voltooiingen van leertrajecten: uitsplitsing van de voltooiingen van leertrajecten (aantal weergegeven in de samenvattingssectie) op naam.

- Voltooiingen per rol*: uitsplitsing van de voltooiingen van de leertrajecten op rol. Als een module is gekoppeld aan meerdere rollen, wordt elk van de rollen toegevoegd aan het aantal module-voltooiingen.

- Voltooiingen per product: uitsplitsing van de voltooiingen van de leertrajecten op product waaraan het leertraject is toegesneden. Als een module is gekoppeld aan meerdere producten, wordt elk van de producten toegevoegd aan het aantal module-voltooiingen.

### <a name="completions-by-learning-individuals"></a>Voltooiingen door individuen te leren

Hier vindt u de getrainde gebruikers in uw bedrijf en details van hun voltooide modules en leertrajecten.

Microsoft Learn identificeert studenten met een gebruikersobject-id. Op het **tabblad Modules** worden alle studenten gesorteerd op de voltooide modules. Ze worden weergegeven met hun Microsoft Learn gebruikersnaam, object-id en aantal modules. U kunt zoeken met behulp van gebruikersnaam. 

Op het **tabblad Leertrajecten** worden alle studenten weergegeven, gesorteerd op voltooide leertrajecten, met de weergavenaam van de learner, de object-id en het aantal modules.

De details van een gebruiker op te halen met behulp van de gebruikersobject-id: 

1. Meld u aan bij [Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) (U moet de globale beheerder zijn van de Azure AD-tenant van uw bedrijf.)

2. Kopieer de gebruikersobject-id naar het [gebied dat is gemarkeerd](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) in Graph Explorer. 

## <a name="faq"></a>Veelgestelde vragen

1. Ik kan de Leergegevens van mijn bedrijf niet zien.

Dit rapport is beschikbaar voor partners met een account in Partner Center. Als u zich nog steeds Partner Membership Center, kunt u dit rapport niet zien.

2.  Wie in ons bedrijf kan dit rapport bekijken? 

De globale beheerder en de MPN-beheerder kunnen het rapport bekijken.

3. Hoe kan ik ervoor zorgen dat al onze gebruikers hun Microsoft Learn koppelen aan hun Partner Center account?

Nadat de globale beheerder een nieuwe gebruiker heeft toegevoegd, moet die gebruiker naar de Mijn profiel **om** zijn of haar Microsoft Learn koppelen.

- Selecteer het **pictogram Uw account** in de rechterhoek van het dashboard en selecteer vervolgens **Mijn profiel**. 

-  Onder **Uw leerproces** kunnen gebruikers hun Microsoft Learning koppelen en hun Microsoft-account koppelen aan Partner University.

3. Kan ik alle gebruikers van het bedrijf zien die zich aanmelden bij Microsoft Learn in dit rapport met een MSA-account?

Op dit moment kunt u dit het beste doen door deze gebruikers toe te voegen aan uw Azure AD-tenant en ze vervolgens toe te voegen aan Partner Center, zodat ze hun Microsoft Learn-account via **Mijn profiel** in Partner Center. 

Voor gebruikers die hun MSA-account alleen gebruiken voor training, kan het Microsoft Learn-team in de nabije toekomst hun werke-mail koppelen aan hun Microsoft Learn-profiel. 

## <a name="next-steps"></a>Volgende stappen

Zie Insights voor [Partner Center rapporten.](partner-center-insights.md)

>[!NOTE] 
> U kunt de onbewerkte gegevens voor dit rapport downloaden via de sectie Rapporten downloaden in het Dashboard Inzichten. [Meer informatie](pci-download-reports.md) 