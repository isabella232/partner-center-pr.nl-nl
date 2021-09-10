---
title: Partner Center Insights Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Houd de gebruikers in uw bedrijf bij door gebruik te maken van gegevens over afzonderlijke training, voltooide modules, voltooide leertrajecten en meer.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b291ee52c9c6e72dc50aab9aa386177d9778cbd1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957130"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Analyserapporten Microsoft Learn gebruiken

**Juiste rollen:** globale | MPN-partnerbeheerder

Het [Microsoft Learn](/learn/) bevat informatie over de studenten in uw bedrijf, inclusief de modules die ze hebben voltooid en de leertrajecten die ze volgen. In het rapport wordt de status van elke afzonderlijke learner weergegeven. Globale beheerders en MPN-beheerders voor een bedrijf kunnen de gegevens bekijken.

## <a name="how-to-read-the-report"></a>Het rapport lezen

### <a name="summary-charts"></a>Samenvattingsdiagrammen

Deze grafieken geven een overzicht van het aantal en de maandelijkse cumulatieve trends voor getrainde individuen, voltooiingen van modules en leertrajecten.

**Aantal getrainde** personen: een telling van alle afzonderlijke studenten die ten minste één module hebben voltooid tijdens het geselecteerde datumbereik 

**Trend-minigrafiek getrainde personen:** het cumulatieve aantal actieve gebruikers per maand 

**Aantal module-voltooiingen:** aantal module-voltooiingen door de studenten in het bedrijf van de partner tijdens het geselecteerde datumbereik.
Als module 1 bijvoorbeeld wordt voltooid door 15 personen en module 2 door dezelfde 15 personen is voltooid, is het aantal voltooiingen van de module 30. De voltooiingsdatum van de module moet binnen het geselecteerde datumbereik vallen.

**Trend minigrafiek voor module-voltooiingen:** cumulatief aantal modules van maand tot maand 

**Learning voltooiingen** van het pad: aantal voltooiingen van Learning pad door de studenten in het bedrijf van de partner tijdens het geselecteerde datumbereik.
Als Learning pad 1 bijvoorbeeld door 20 personen wordt voltooid en het Learning-pad 'pad 2' is voltooid door dezelfde 20 personen, is het aantal voltooiingen van Learning-pad 40. De Learning van het pad moet binnen het geselecteerde datumbereik vallen.

**Learning trend minigrafiek** voor voltooiingen van het leertraject: cumulatief aantal maanden van voltooiingen van het leertraject 

### <a name="trained-individuals-monthly-trend"></a>De maandelijkse trend van getrainde personen

Deze gegevens zijn de trend van de gebruikers van uw bedrijf die een module voor het eerst in die maand hebben voltooid. 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal actieve studenten dat zich in die maand heeft geregistreerd (de eerste keer dat een module is voltooid). Dit is niet cumulatief.

### <a name="module-completions-monthly-trend"></a>Module-voltooiingen trend per maand

Deze gegevens zijn de trend van modules die gedurende die maand door alle gebruikers van uw bedrijf zijn voltooid. (niet cumulatief) 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal voltooiingen van de module in die maand. Dit is niet cumulatief.

### <a name="learning-path-completions-monthly-trend"></a>Learning maandelijkse trend voor voltooiing van het pad

Deze gegevens zijn de trend van leertrajecten die de gebruikers van uw bedrijf in die maand hebben voltooid. (niet cumulatief) 

**X-as** is maand voor het geselecteerde tijdfilter. 

**Y-as** is het aantal module-voltooiingen in die maand. Dit is niet cumulatief.

### <a name="learning-path-completion-tabs"></a>Learning tabbladen voor het voltooien van het pad

#### <a name="module-tab"></a>Tabblad Module

Dit tabblad bevat uitsplitsing van modules die in uw bedrijf zijn voltooid op de vijf belangrijkste modulenamen; het product waaraan de module is gekoppeld; en de gebruikersrol die relevant is voor de module.  

- Module-voltooiingsdiagram: uitsplitsing van de voltooiingen van de module (aantal weergegeven in de samenvattingssectie) op de modulenamen.

Het getal dat in het midden van de grafiek wordt weergegeven, is het totale aantal voltooide modules

- Voltooiingen per rol: uitsplitsing van de voltooiing van de module op de rol van de module. Als een module is gekoppeld aan meerdere rollen, wordt elk van de rollen toegevoegd aan het aantal module-voltooiingen.

Het getal dat in het midden van de grafiek wordt weergegeven, is het aantal afzonderlijke rollen voor de voltooiing van de module. 

- Voltooiingen per product: uitsplitsing van de voltooiingen van de module op het product waar de module aan is toegesneden. Als een module is gekoppeld aan meerdere producten, wordt elk van de producten toegevoegd aan het aantal module-voltooiingen.    

Het getal dat in het midden van de grafiek wordt weergegeven, is het aantal afzonderlijke producten voor de voltooiing van de module.  

#### <a name="learning-path-tab"></a>Learning tabblad Pad

Dit tabblad bevat een overzicht van de leertrajecten die in uw bedrijf zijn voltooid op de vijf belangrijkste modulenamen; het product waar het leertraject aan is toegesneden; en de rol die relevant is voor dit leertraject.  

- Learning voltooiingsgrafiek paden: uitsplitsing van Learning voltooiingen van het pad (aantal weergegeven in de samenvattingssectie) op naam.

- Voltooiingen per rol: uitsplitsing van de voltooiingen van de leertrajecten op rol. Als een module is gekoppeld aan meerdere rollen, wordt elk van de rollen toegevoegd aan het aantal module-voltooiingen.

- Voltooiingen per product: uitsplitsing van de voltooiingen van de leertrajecten op product waaraan het leertraject is toegesneden. Als een module is gekoppeld aan meerdere producten, wordt elk van de producten toegevoegd aan het aantal module-voltooiingen.

### <a name="completions-by-learning-individuals"></a>Voltooiingen door individuen te leren

Hier vindt u de getrainde gebruikers in uw bedrijf en details van hun voltooide modules en leertrajecten.

Microsoft Learn identificeert studenten met een gebruikersobject-id. Op het **tabblad Modules** worden alle studenten gesorteerd op de voltooide modules. Ze worden weergegeven met hun Microsoft Learn gebruikersnaam, object-id en aantal modules. U kunt zoeken met behulp van gebruikersnaam. 

Op het **tabblad Learning** paden worden alle studenten weergegeven, gesorteerd op voltooide leertrajecten, met de weergavenaam van de leerder, de object-id en het aantal modules.

Ga als volgende te werk om de details van een gebruiker op te halen met behulp van de gebruikersobject-id: 

1. Meld u aan [bij Graph Explorer.](https://developer.microsoft.com/graph/graph-explorer ) (U moet de globale beheerder zijn van de Azure AD-tenant van uw bedrijf.)

2. Kopieer de gebruikersobject-id naar het [gebied dat](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) is gemarkeerd in Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Veelgestelde vragen

1. Ik kan de Learn-details van mijn bedrijf niet zien.

   Dit rapport is beschikbaar voor partners met een account in Partner Center. Als u zich nog steeds Partner Membership Center, kunt u dit rapport niet zien.

2. Wie in mijn bedrijf kan dit rapport bekijken? 

   De globale beheerder en de MPN-beheerder kunnen het rapport bekijken.

3. Hoe kan ik ervoor zorgen dat al onze gebruikers hun Microsoft Learn koppelen aan hun Partner Center account?

   *Nadat de globale beheerder* een nieuwe gebruiker heeft toegevoegd, moet die gebruiker naar [Microsoft Learn](/learn/) gaan om zijn zakelijke account of werkaccount van Azure Active Directory (AD) te koppelen aan zijn Learn-account. Dit zorgt ervoor dat Insights Learning juiste cursussen en vaardigheden worden weergegeven op het tabblad.
   
   De gebruiker moet:
   
   1. Meld u [aan Microsoft Learn](/learn/).
   2. Selecteer de profielafbeelding en selecteer vervolgens **Mijn profiel**.
   3. Selecteer **Instellingen**.
   4. Voeg **onder Accountbeheer** het werkaccount toe onder **Gekoppelde accounts.**

4. Kan ik alle gebruikers van het bedrijf zien die zich aanmelden bij Microsoft Learn in dit rapport met een MSA-account?

   Op dit moment kunt u dit het beste doen door deze gebruikers toe te voegen aan uw Azure AD-tenant en ze vervolgens toe te voegen aan Partner Center, zodat ze hun Microsoft Learn-account kunnen koppelen via **Mijn profiel** in Partner Center. 

   Voor gebruikers die alleen hun MSA-account gebruiken voor training, kan het Microsoft Learn-team in de nabije toekomst hun werke-mail koppelen aan hun Microsoft Learn-profiel. 

## <a name="next-steps"></a>Volgende stappen

Zie voor meer rapporten [Partner Center Insights.](partner-center-insights.md)

>[!NOTE] 
> U kunt de onbewerkte gegevens voor dit rapport downloaden uit de sectie Rapporten downloaden in Insights dashboard. [Meer informatie](insights-download-reports.md) 
