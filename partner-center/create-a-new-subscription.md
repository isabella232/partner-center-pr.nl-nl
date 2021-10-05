---
title: Klantabonnementen maken in Partner Center
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het verkopen van abonnementen aan uw klanten voor producten die zijn gepubliceerd door Microsoft en SaaS-producten die zijn gepubliceerd door ISV's van derden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 1a2e13bf45b10bebe6ab0492ac059dc1d6a6c0ca
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452410"
---
# <a name="manage-customer-subscriptions"></a>Klantabonnementen beheren

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale beheerder | Helpdeskagent | Verkoopagent

Nadat u een record van uw klant in de Partner Center, kunt u ze abonnementen verkopen aan producten in de catalogus. Dit omvat producten die zijn gepubliceerd door Microsoft en SaaS-producten (Software as a Service) die door onafhankelijke onafhankelijke softwareleveranciers (ISV's) zijn gepubliceerd op [de commerciële marketplace.](https://azuremarketplace.microsoft.com/marketplace)

Sommige aanbiedingen zijn beperkt tot één abonnement per klant. Als u een lijst wilt bekijken met aanbiedingen die zijn beperkt, gaat u naar Partner Center pagina Prijzen en aanbiedingen.

> [!IMPORTANT]
> Als partner in het CSP-programma kunt u  SaaS-abonnementen op basis van licenties of saaS-abonnementen met datalicenties aanschaffen bij **ISV-uitgevers** binnen Partner Center. Dit betekent dat u elke  SaaS-aanbieding op basis van licenties of naar [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gebruik kunt aanschaffen die de **ISV-uitgever** voor u beschikbaar heeft gesteld, inclusief exclusieve aanbiedingen waarvoor u toegang hebt. Als u andere commerciële marketplace-aanbiedingen van ISV's wilt kopen of beheren (zoals aanbiedingen op basis van gebruik met betrekking tot Azure-toepassingen, containers of VM's), gaat u [naar de Azure Portal.](https://portal.azure.com/)

> [!NOTE]
> Alle datums en tijden in Partner Center worden opgegeven in de UTC-tijdstandaard (Universal Time Coordinated). Dit kan tot 24 uur verschillen van uw lokale tijd.

## <a name="create-a-new-subscription"></a>Een nieuw abonnement maken

> [!NOTE]
> Zie Voor meer informatie over de werkruimte-interface [Getting around Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Werkruimtenweergave](#tab/workspaces-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard)de **tegel Klanten** en selecteer vervolgens de klant in de lijst Klant.

2. Selecteer **Abonnement toevoegen.** Op **het tabblad Onlineservices** worden alle beschikbare Marketplace SaaS-aanbiedingen weergegeven.

3. Als u alleen bepaalde typen abonnementen wilt zien, maakt u selecties in de beschikbare filters:
   - **Publisher:** kies **Microsoft als** u alleen aanbiedingen van Microsoft of **Partner** wilt zien om commerciële marketplace-producten te zien die zijn gepubliceerd door ISV's.
   - **Factureringstype:** selecteer het type abonnementsfacturering dat u wilt gebruiken: **Licentie** of **Gebruik.** Zie [Facturering op basis van licenties](license-based-billing.md) voor informatie waarmee u kunt kiezen tussen de maandelijkse en jaarlijkse factureringsfrequentie.
   - **Categorie:** kies **Enterprise,** **Small Business** of **Trial.** Zie Proefversies van Microsoft-producten aanbieden voor [meer informatie over proefabonnementen.](offer-your-customers-trials-of-microsoft-products.md)

4. Selecteer de productabonnementen die u voor uw klant wilt kopen. De producten die u ziet, zijn afhankelijk van het type klantsegment (onderwijs, overheid, enzovoort) en de filters die u hebt toegepast. Sommige aanbiedingen die op de Marketplace worden weergegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner. Dit kan de volgende zijn:
   - De klant heeft al een abonnement op dat product en er is er slechts één toegestaan
   - Het abonnement van de klant is mogelijk tijdelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuw abonnement aan te schaffen.)
   - Voor ISV SaaS-aanbiedingen kunnen er enkele redenen zijn waarom de aanbieding niet beschikbaar is om te kopen: De ISV biedt mogelijk geen ondersteuning voor het factureringsland of de regio van de klant; De ISV heeft er mogelijk voor gekozen om de aanbieding niet beschikbaar te maken via het CSP-programma; of kan de ISV de aanbieding uitsluitend hebben [gedaan](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) aan bepaalde CSP-partners. De ISV-aanbieding is mogelijk ook niet transacteerbaar via de Partner Center (bijvoorbeeld containers of sommige aanbiedingen op basis van gebruik).  

5. Voer voor elk abonnement dat u wilt toevoegen het aantal licenties in (indien nodig) en selecteer **Toevoegen aan winkelwagen.**

6. Wanneer u klaar bent met het toevoegen van abonnementen, **selecteert u Controleren** en uw bestelling controleren.

7. Nadat u uw orders hebt gecontroleerd en klaar bent om deze abonnementen aan te schaffen, selecteert u **Kopen.**

8. Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:

    - U kunt het abonnement controleren of bewerken door de abonnementsnaam te selecteren op de pagina **Abonnementen van die** klant. Hier kunt u invoeglicenties selecteren als deze beschikbaar zijn, het aantal licenties wijzigen of het abonnement opschorten.

    **Voor ISV SaaS-abonnementen (op basis van licenties en naar licentie) geldt het volgende:**
    - U ontvangt een koppeling naar de site van de ISV-uitgever. Deze koppeling helpt u bij het voltooien van de implementatie of het instellen van het account van het abonnement van de klant.

    > [!NOTE]
    > Noch u noch uw klant ontvangt een e-mail met instructies voor het voltooien van het instellen/inrichten van het account voor dit type ISV-abonnement.)

    - Als uw abonnement wordt geleverd met een gratis proefversie van 30 dagen, wordt de gratis proefperiode automatisch toegepast. Als partner in het CSP-programma kunt u de gratis proefperiode voor aanbiedingen die u voor klanten koopt niet in de weg staan. Zodra de gratis proefperiode is afgelopen, begint de abonnementsperiode en wordt het abonnement omgezet in de betaalde status. Het abonnement wordt vervolgens automatisch vernieuwd volgens hetzelfde schema.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard) **klanten** en selecteer vervolgens de klant in de lijst Klant.

2. Selecteer **Abonnement toevoegen.** Op **het tabblad Onlineservices** worden alle beschikbare Marketplace SaaS-aanbiedingen weergegeven.

3. Als u alleen bepaalde typen abonnementen wilt zien, maakt u selecties in de beschikbare filters:
   - **Publisher:** kies **Microsoft als** u alleen aanbiedingen van Microsoft of **Partner** wilt zien om commerciële marketplace-producten te zien die zijn gepubliceerd door ISV's.
   - **Factureringstype:** selecteer het type abonnementsfacturering dat u wilt gebruiken: **Licentie** of **Gebruik.** Zie [Facturering op basis van licenties](license-based-billing.md) voor informatie waarmee u kunt kiezen tussen de maandelijkse en jaarlijkse factureringsfrequentie.
   - **Categorie:** kies **Enterprise,** **Small Business** of **Trial.** Zie Proefversies van Microsoft-producten aanbieden voor [meer informatie over proefabonnementen.](offer-your-customers-trials-of-microsoft-products.md)

4. Selecteer de productabonnementen die u voor uw klant wilt kopen. De producten die u ziet, zijn afhankelijk van het type klantsegment (onderwijs, overheid, enzovoort) en de filters die u hebt toegepast. Sommige aanbiedingen die op de Marketplace worden weergegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner. Dit kan de volgende zijn:
   - De klant heeft al een abonnement op dat product en er is er slechts één toegestaan
   - Het abonnement van de klant is mogelijk tijdelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuw abonnement aan te schaffen.)
   - Voor ISV SaaS-aanbiedingen kunnen er enkele redenen zijn waarom de aanbieding niet beschikbaar is om te kopen: De ISV biedt mogelijk geen ondersteuning voor het factureringsland of de regio van de klant; De ISV heeft er mogelijk voor gekozen om de aanbieding niet beschikbaar te maken via het CSP-programma; of kan de ISV de aanbieding uitsluitend hebben [gedaan](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) aan bepaalde CSP-partners. De ISV-aanbieding is mogelijk ook niet transacteerbaar via de Partner Center (bijvoorbeeld containers of sommige aanbiedingen op basis van gebruik).  

5. Voer voor elk abonnement dat u wilt toevoegen het aantal licenties in (indien nodig) en selecteer **Toevoegen aan winkelwagen.**

6. Wanneer u klaar bent met het toevoegen van abonnementen, **selecteert u Controleren** en uw bestelling controleren.

7. Nadat u uw orders hebt gecontroleerd en klaar bent om deze abonnementen aan te schaffen, selecteert u **Kopen.**

8. Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:

    - U kunt het abonnement controleren of bewerken door de abonnementsnaam te selecteren op de pagina **Abonnementen van die** klant. Hier kunt u invoeglicenties selecteren als deze beschikbaar zijn, het aantal licenties wijzigen of het abonnement opschorten.

    **Voor ISV SaaS-abonnementen (op basis van licenties en naar licentie) geldt het volgende:**
    - U ontvangt een koppeling naar de site van de ISV-uitgever. Deze koppeling helpt u bij het voltooien van de implementatie of het instellen van het account van het abonnement van de klant.

    > [!NOTE]
    > Noch u noch uw klant ontvangt een e-mail met instructies voor het voltooien van het instellen/inrichten van het account voor dit type ISV-abonnement.)

    - Als uw abonnement wordt geleverd met een gratis proefversie van 30 dagen, wordt de gratis proefperiode automatisch toegepast. Als partner in het CSP-programma kunt u de gratis proefperiode voor aanbiedingen die u voor klanten koopt niet in de weg staan. Zodra de gratis proefperiode is afgelopen, begint de abonnementsperiode en wordt het abonnement omgezet in de betaalde status. Het abonnement wordt vervolgens automatisch vernieuwd volgens hetzelfde schema.

* * *

## <a name="update-subscriptions-with-add-ons"></a>Abonnementen bijwerken met invoegtoepassingen

Als de klant een invoegabonnement wil aanschaffen, moet deze eerst een actief basisabonnement hebben.  U kunt invoegtoepassingen niet aanschaffen via de catalogus.

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Onder de **sectie Status** vindt u een lijst met beschikbare invoegtoepassingen voor het abonnement.  

5. Werk het aantal licenties voor elke vereiste invoeg-invoeging bij. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

De mogelijkheid om invoegtoepassingen aan te schaffen via Partner Center is alleen beschikbaar voor directe factuur- en indirecte providers.
Alleen in aanmerking komende invoegtoepassingen worden weergegeven op basis van de basisvereisten en regionale beschikbaarheid. Raadpleeg de aanbiedingsmatrix voor cloud resellers voor meer informatie over prijzen en aanbiedingen. Als u het basisabonnement onderbreekt, worden ook alle bijbehorende invoegtoepassingen onderbroken.

Begindatums voor invoegtoepassingen worden afgestemd met het basisabonnement en de kosten worden berekend op basis van de begindatum van de kosten en de einddatum van de kosten met pro rata kosten op de eerste factuur. Zie Op licenties gebaseerde facturering [voor meer informatie.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Een abonnement opzeggen of annuleren

Partners kunnen een abonnement opzeggen of annuleren als dit wordt aangevraagd door de klant, of in geval van niet-vooruitbetaling of fraude.

### <a name="suspend-a-subscription"></a>Een abonnement opschorten

Wanneer u de status van een abonnement wijzigt in **Tijdelijk,** kunnen gebruikers zich niet aanmelden of toegang krijgen tot services.

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Kies **Onderbroken** bij **Status**. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd, of 90 dagen plus het aantal dagen tussen het moment dat het account is geopend en de eerste factureringsperiode (maximaal 120 dagen).

Wanneer u een abonnement onder de  knop Tijdelijk opzegt, wordt aangegeven wanneer het abonnement automatisch verloopt als u het abonnement niet opnieuw activeren. 

> [!NOTE]
> CSP-abonnementen hebben geen verlopen periode (zoals web-directe abonnementen) waarin de services nog steeds werken, maar het abonnement geen factureringskosten genereert. CSP-abonnementen zijn actief of tijdelijk (of volledig verwijderd).

> [!NOTE]
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Als u nieuwe commerce-abonnementen wilt opschorten of nieuwe handelsabonnementen opnieuw wilt activeren, maakt u een serviceaanvraag en neem contact op met de ondersteuning.


### <a name="cancel-a-subscription"></a>Een abonnement annuleren

U kunt SaaS-abonnementen op basis van licenties annuleren van ISV-uitgevers van derden binnen de Partner Center [commerciële marketplace.](csp-commercial-marketplace-overview.md) Zolang u binnen de annuleringsperiode annuleert, ontvangt u een volledige restitutie.

Voor ISV-aanbiedingen die maandelijks worden gefactureerd:

- Als u minder dan 24 uur na het plaatsen van de order annuleert, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 24 uur na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.

Voor aanbiedingen die jaarlijks worden gefactureerd:

- Als u minder dan 14 dagen na het plaatsen van de order annuleert, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 14 dagen na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.

Nadat deze perioden zijn afgelopen, ziet u niet langer de optie om het abonnement te annuleren.

> [!NOTE]
> ISV-services van derden (die bijvoorbeeld virtuele machines of containers gebruiken) op basis van gebruik en naar gebruik komen niet in aanmerking voor retournering. Op gebruik gebaseerde services kunnen worden verwijderd als annuleringsmethode. Omdat de kosten na gebruik worden gefactureerd, komen deze services niet in aanmerking voor restitutie.

Ga als volgt te werk om een SaaS-abonnement op basis van een licentie van een ISV-uitgever te annuleren:

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Zoek het abonnement dat u wilt annuleren.

4. Selecteer annuleren **in** de kolom **Status.** Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Als er een dialoogvenster wordt weergegeven, vult u alle relevante gegevens in en selecteert u **Verzenden.**

6. Selecteer Ja, annuleren om de annulering **te bevestigen.**

> [!NOTE]
> U kunt er ook voor kiezen om een abonnement Azure Marketplace annuleren met behulp van API's. Zie Een abonnement op Azure Marketplace [annuleren om dit te doen.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

## <a name="suspend-or-cancel-a-new-commerce-subscription"></a>Een nieuw commerce-abonnement opzeggen of annuleren

### <a name="suspend-a-new-commerce-subscription"></a>Een nieuw commerce-abonnement opschorten

> [!NOTE]
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

In het geval van niet-betaling van de klant, ook wel het 'dunningscenario' genoemd, kunnen partners hun abonnement onderbreken en hervatten om de toegang van de klant tot de services van het abonnement onmiddellijk te blokkeren.

Partners kunnen een abonnement op elk moment onderbreken en hervatten zonder opzegging. De facturering van partners wordt echter voortgezet tijdens de opzegging. 

Als de abonnementen van de klant worden onderbroken, wordt de mogelijkheid om zich aan te melden en hun services te gebruiken uitgeschakeld totdat het abonnement wordt hervat. Alle gegevens die betrekking hebben op het abonnement worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd.

U kunt een abonnement onderbreken met behulp van Partner Center:

1. Ga naar de abonnementspagina van de klant en selecteer het abonnement dat u wilt onderbreken.

2. Selecteer het **keuzerondje** Suspend.

3. Selecteer OK in het **pop-updialoogvenster.**

4. Het abonnement heeft nu een onderbroken status en de partner wordt nog steeds gefactureerd voor het abonnement.

Onderbreken is omkeerbaar via Partner Center gebruikersinterface of API's waarmee de toegang van een klant tot de services van een abonnement onmiddellijk wordt hersteld.

> [!IMPORTANT]
> Als u een abonnement onderpauzeert, worden alle instellingen voor automatisch verlengen uitgeschakeld en worden eventuele bestaande geplande wijzigingen verwijderd. Het onderbreken van een abonnement heeft alleen invloed op de toegang tot de service van de klant en de facturering van de partner blijft in de onderbroken status.

### <a name="cancel-a-new-commerce-subscription"></a>Een nieuw commerce-abonnement annuleren

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Voor nieuwe commerceaanbiedingen kunnen partners hun abonnement opzeggen met een pro **72-restitutie** binnen de eerste 72 uur voor elke periode **(proration berekend per dag).**  

Na 72 uur is annulering niet meer beschikbaar en wordt de partner gefactureerd voor de volledige termijn, zelfs als de klant niet meer betaalt voor of het abonnement gebruikt (van toepassing op een factureringsplan).

Wanneer een annulering is voltooid, heeft de klant onmiddellijk geen toegang meer tot de service en kan de service niet worden hersteld. De status van het abonnement kan niet worden hersteld.  

Als er halverwege de termijn licenties worden toegevoegd, is hetzelfde beleid van 72 uur van toepassing op het verminderen van extra licenties. Het verminderen van het aantal toegevoegde licenties moet worden uitgevoerd via **ondersteuningsaanvragen.**

## <a name="subscription-renewals"></a>Abonnementsvernieuwingen

> [!NOTE]
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Actieve abonnementen zijn standaard ingesteld om automatisch te worden verlengd wanneer de abonnementsperiode verloopt. Voor [abonnementen op commerciële marketplace-producten](csp-commercial-marketplace-overview.md)of nieuwe commerce-abonnementen kunt u ervoor kiezen om het abonnement niet automatisch te verlengen.

Als u wilt voorkomen dat een actief abonnement op de commerciële marketplace of nieuwe commerce-abonnementen automatisch wordt verlengd:

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer **Abonnementen**. Hier worden alle op licenties gebaseerde abonnementen vermeld die u voor de klant hebt aangeschaft.

4. Selecteer in **de** kolom Abonnement het abonnement dat u wilt wijzigen.

5. Zoek op de pagina met abonnementsdetails **de sectie Status** en vink het selectievakje Automatisch **verlengen** uit.

6. Selecteer **Indienen**.

### <a name="manage-new-commerce-renewals-with-scheduled-changes"></a>Nieuwe handelsvernieuwingen beheren met geplande wijzigingen

> [!NOTE]
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Sommige wijzigingen in abonnementen kunnen alleen aan het einde van een termijn plaatsvinden. Deze wijzigingen kunnen worden gepland zodat ze gemakkelijk aan het einde van de term worden toegepast. Voorbeelden van wijzigingen die moeten worden gepland:

- licentiekortingen
- Wijzigingen in factureringsperiode
- Wijzigingen in factureringsfrequentie

Andere wijzigingen, zoals upgrades of licentieverhogingen, kunnen tijdens de periode worden toegepast.

Planningswijzigingen vinden plaats bij verlenging wanneer het abonnement wordt verlengd voor de volgende termijn.

Vereisten voor geplande wijzigingen:

- Abonnement is actief 
- Automatisch verlengen is aan
- SKU moet in aanmerking komen voor een upgrade

Een nieuwe wijziging plannen bij verlenging:

1. Meld u aan bij Partner Center dashboard.

2. Kies een **klant** in de lijst met klanten.

3. Kies het abonnement dat u wilt beheren.

4. Selecteer **Vernieuwingen beheren.**

5. Selecteer een andere Waardewijziging voor SKU, hoeveelheid, termijn of factureringsfrequentie:

   - **Huidig** is de huidige waarde van het abonnement

   - **Wijzigen** in is de laatst opgeslagen waarde die u wilt toepassen bij verlenging van het nieuwe abonnement

6. Selecteer **Indienen**.

7. De wijzigingen vinden plaats bij verlenging.

Partners hebben toegang tot **Vernieuwingen beheren om** bestaande geplande wijziging weer te geven, bij te werken of te verwijderen.

> [!NOTE]
> - Proefversies worden aan het einde van de proefperiode standaard ge converteerd naar de betaalde equivalente SKU.
> - Als het aantal licenties voor geplande SKU-upgrades niet wordt gewijzigd, wordt het opnieuw toewijzen van gebruikerslicenties automatisch uitgevoerd, anders moet dit handmatig worden uitgevoerd.
> - Opgeslagen geplande wijzigingen worden verwijderd als er op de korte termijn updates worden doorgevoerd in het abonnement.

Opgeslagen geplande wijzigingen worden verwijderd wanneer de volgende wijzigingen op de korte termijn worden aangebracht:  

- Automatisch verlengen is uitgeschakeld 
- Hoeveelheid wordt gewijzigd 
- Abonnement is geannuleerd 
- SKU is bijgewerkt 
- De proefversie wordt geconverteerd 

## <a name="upgrades-in-new-commerce-subscriptions"></a>Upgrades in nieuwe commerce-abonnementen

Voor nieuwe handel betekent een upgrade van het ene betaalde abonnement naar het andere. Met nieuwe upgrades van betaalde naar betaalde commerce kan de klant onmiddellijk een upgrade uitvoeren van de huidige SKU naar een upgrade met toegevoegde services. 

Partners kunnen selecteren naar welk abonnement ze een upgrade willen uitvoeren bij het configureren van het aantal licenties. Partners kunnen een nieuw **abonnement** selecteren of een **bestaand abonnement** selecteren als dit in aanmerking komt voor de upgrade. 

Upgrades kunnen uit twee typen bestaan: **Volledige upgrade** en **Gedeeltelijke upgrade.**

> [!NOTE]
> - Upgrades kunnen worden gepland aan het einde van een termijn of kunnen halverwege de termijn worden gestart.
> - Als u een upgrade op de korte termijn start, worden bestaande geplande upgrades verwijderd.
> - Upgrades kunnen alleen worden gestart vanuit abonnementen met de **status** Actief.

### <a name="full-upgrades"></a>Volledige upgrades

Een volledige upgrade is een in-place upgrade, wat betekent dat alle of meer licenties worden bijgewerkt. In dit geval blijft de abonnements-id hetzelfde en worden er automatisch licenties toegewezen. Als de klant de doel-SKU echter al heeft aangeschaft bij een andere partner of kanaal via een verouderd kanaal, is handmatige toewijzing nodig. Als handmatige toewijzing nodig is, ziet de partner een waarschuwingsbericht in Partner Center waarin staat dat de licenties handmatig moeten worden toegewezen. 

### <a name="partial-upgrades"></a>Gedeeltelijke upgrades

Met gedeeltelijke upgrades kan een partner bepaalde licenties van de ene SKU naar de andere aanwijzen. Met de vorige upgradefunctionaliteit in traditionele abonnementen op basis van licenties konden alleen alle licenties worden bijgewerkt. Nieuwe handel stelt een partner in staat om bepaalde licenties op hun gemak te verplaatsen. Dit geeft de partner meer controle over het beheren van upgrades, zodat ze sommige gebruikers naar een nieuwe SKU kunnen verplaatsen zonder ze allemaal te verplaatsen.

Details van gedeeltelijke upgrade:

- Deze optie is gedeeltelijk gedefinieerd als het aantal upgradelicenties kleiner is dan het oorspronkelijke abonnement.
- Een nieuw abonnement dat is gemaakt tijdens een gedeeltelijke upgrade, heeft dezelfde einddatums als het abonnement waar de upgrade van afkomstig is.

## <a name="increasing-and-reducing-licenses-in-new-commerce-subscriptions"></a>Licenties in nieuwe commerce-abonnementen verhogen en verminderen

Het aantal licenties voor  een abonnement kan op elk moment worden verhoogd, met factureringscorrecties die worden weergegeven in het volgende factuur- en afstemmingsbestand. 

Het aantal licenties voor een abonnement kan worden **verlaagd:**
- alleen binnen de eerste 72 uur nadat de abonnementsorder voor het eerst is **geplaatst of vernieuwd.** 
- via klantondersteuning binnen 72 uur, voor licenties die **zijn toegevoegd op de tussentijdse termijn**

Een afname van het aantal licenties binnen de eerste 72 uur van een abonnementsperiode (na de initiële aankoop of verlenging) kan worden gedaan via selfservice in Partner Center of via de API.

Een afname van het aantal licenties dat op de korte termijn is toegevoegd, kan alleen worden uitgevoerd via klantondersteuning, binnen de eerste 72 uur.

In beide gevallen van licentievermindering krijgt u een restitutie voor het volledige bedrag **minus pro-rated** bedrag voor de dagen dat u het abonnement hebt gebruikt   **(proration berekend per dag).** 

Als er meer **dan 72** uur zijn verstreken sinds de abonnementsorder is  geplaatst of er extra licenties zijn toegevoegd, kan het aantal licenties niet worden verlaagd tot het volgende annuleringsvenster bij verlenging.

## <a name="switching-billing-plans"></a>Schakelen tussen factureringsplannen

Partners hebben de flexibiliteit om hun factureringsplan en factureringsperiode samen te schakelen. Ze hebben ook de mogelijkheid om alleen hun factureringsplan halverwege de termijn over te schakelen, zonder de factureringsperiode helemaal opnieuw in te stellen.

### <a name="just-changing-billing-frequency-scheduled-change"></a>Alleen de factureringsfrequentie wijzigen (geplande wijziging)

Partners kunnen alleen het factureringsplan via Partner Center in slechts enkele stappen wijzigen, die van kracht worden in de volgende factureringscyclus:

1. Ga naar de abonnementspagina van de klant en selecteer het abonnement dat u wilt wijzigen.

2. Selecteer de **koppeling Factureringsfrequentie** beheren.

3. Er wordt een zijpaneel geopend met de huidige factureringsfrequentie en een vervolgkeuzevenster met de opties om de frequentie in te wijzigen.

4. Zodra een nieuwe waarde is geselecteerd, worden de nieuwe factureringswijzigingen doorgevoerd in de **volgende** factureringscyclus (GEEN onmiddellijke wijziging).

### <a name="changing-billing-frequency-along-with-billing-term-and-other-fields-immediate-change"></a>Factureringsfrequentie wijzigen, samen met factureringsperiode en andere velden (onmiddellijke wijziging)

De partner kan de factureringsfrequentie, samen met de factureringstermijn en andere velden, ook via de Partner Center wijzigen, waardoor een onmiddellijke wijziging wordt veroorzaakt:

1. Ga naar de abonnementspagina van de klant en selecteer het abonnement dat u wilt wijzigen.

2. Wijzig de duur van de term door een optie in de vervolgkeuzeoptie te selecteren. Hiermee opent u een andere vervolgkeuze voor het wijzigen van de factureringsfrequentie.

3. Selecteer een andere factureringsfrequentie in de vervolgkeuzekeuze.

4. Zodra u de wijzigingen hebt aangebracht en op Verzenden hebt geklikt, worden de nieuwe factureringswijzigingen onmiddellijk **doorgevoerd.**

## <a name="next-steps"></a>Volgende stappen

- [Commerciële marketplace-producten kopen voor uw klanten](csp-commercial-marketplace-purchase.md)

- [Commerciële marketplace-producten voor uw klanten beheren](csp-commercial-marketplace-manage.md)

- [Overzicht van commerciële marketplace](csp-commercial-marketplace-overview.md)
