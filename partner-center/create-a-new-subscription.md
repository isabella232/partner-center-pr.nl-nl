---
title: Klantabonnementen maken in Partner Center
ms.topic: how-to
ms.date: 08/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het verkopen van abonnementen aan uw klanten voor producten die zijn gepubliceerd door Microsoft en SaaS-producten die zijn gepubliceerd door ISV's van derden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 5276f5bcc201633865fd8f226d52630919530982
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458004"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Klantabonnementen maken, onderbreken of annuleren

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale | Helpdeskagent | Verkoopagent

Nadat u een record van uw klant in de Partner Center hebt gemaakt, kunt u ze abonnementen verkopen aan producten in de catalogus. Dit omvat producten die zijn gepubliceerd door Microsoft en SaaS-producten (Software as a Service) die door onafhankelijke onafhankelijke softwareleveranciers (ISV's) zijn gepubliceerd op de [commerciële marketplace.](https://azuremarketplace.microsoft.com/marketplace)

Sommige aanbiedingen zijn beperkt tot één abonnement per klant. Als u een lijst wilt bekijken met aanbiedingen die zijn beperkt, gaat u naar Partner Center pagina Prijzen en aanbiedingen.

>[!IMPORTANT]
> Als partner in het CSP-programma kunt u  SaaS-abonnementen op basis van licenties of SaaS-abonnementen met een datalicentie kopen bij **ISV-uitgevers** binnen Partner Center. Dit betekent dat u elke  SaaS-aanbieding op basis van licenties of naar [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gebruik kunt aanschaffen die de **ISV-uitgever** voor u beschikbaar heeft gesteld, inclusief exclusieve aanbiedingen waarvoor u toegang hebt. Als u andere commerciële marketplace-aanbiedingen van ISV's (zoals aanbiedingen op basis van gebruik met Betrekking tot Azure-toepassingen, containers of VM's) wilt kopen of beheren, moet u naar de [Azure Portal.](https://portal.azure.com/)

>[!NOTE]
>Alle datums en tijden in Partner Center worden opgegeven in de tijdstandaard Universal Time Coordinated (UTC). Dit kan tot 24 uur verschillen van uw lokale tijd.

## <a name="create-a-new-subscription"></a>Een nieuw abonnement maken

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer **Abonnement toevoegen.** Op **het tabblad Onlineservices** worden alle beschikbare Marketplace SaaS-aanbiedingen weergegeven.

4. Als u alleen bepaalde typen abonnementen wilt zien, maakt u selecties in de beschikbare filters:
   - **Publisher: kies** **Microsoft om alleen** aanbiedingen van Microsoft of **Partner** te bekijken om commerciële marketplace-producten te zien die zijn gepubliceerd door ISV's.
   - **Factureringstype:** selecteer het type abonnement dat u wilt gebruiken: **Licentie** of **Gebruik.** Zie [Facturering op basis van licenties](license-based-billing.md) voor informatie waarmee u kunt kiezen tussen de maandelijkse en jaarlijkse factureringsfrequentie.
   - **Categorie:** kies **Enterprise,** **Small Business** of **Trial.** Zie Proefversies van Microsoft-producten aanbieden voor [meer informatie over proefabonnementen.](offer-your-customers-trials-of-microsoft-products.md)

5. Selecteer de productabonnementen die u voor uw klant wilt kopen. De producten die u ziet, zijn afhankelijk van het type klantsegment (onderwijs, overheid, enzovoort) en de filters die u hebt toegepast. Sommige aanbiedingen die op de Marketplace worden weergegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner. Dit kan komen door:

   - De klant heeft al een abonnement op dat product en heeft er slechts één

   - Het abonnement van de klant is mogelijk tijdelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuw abonnement aan te schaffen.)

   - Voor ISV SaaS-aanbiedingen kunnen er enkele redenen zijn waarom de aanbieding niet beschikbaar is om te kopen: De ISV biedt mogelijk geen ondersteuning voor het land of de regio van de facturering van de klant; De ISV heeft er mogelijk voor gekozen om de aanbieding niet beschikbaar te maken via het CSP-programma; of de ISV heeft de aanbieding mogelijk uitsluitend [aan](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) bepaalde CSP-partners gedaan. De ISV-aanbieding is mogelijk ook niet transacteerbaar via de Partner Center (bijvoorbeeld containers of sommige aanbiedingen op basis van gebruik).  

6. Voer voor elk abonnement dat u wilt toevoegen het aantal licenties in (indien nodig) en selecteer **Toevoegen aan winkelwagen.**

7. Wanneer u klaar bent met het toevoegen van abonnementen, **selecteert u Uw** bestelling controleren en controleren.

8. Nadat u uw orders hebt gecontroleerd en klaar bent om deze abonnementen te kopen, selecteert u **Kopen.**

9. Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:

    - U kunt het abonnement controleren of bewerken door de abonnementsnaam te selecteren op de **pagina Abonnementen van die** klant. Hier kunt u invoeglicenties selecteren als deze beschikbaar zijn, het aantal licenties wijzigen of het abonnement opschorten.

    **Voor ISV SaaS-abonnementen (op basis van licenties en licenties) geldt het volgende:**
    - U ontvangt een koppeling naar de site van de ISV-uitgever. Deze koppeling helpt u bij het voltooien van de implementatie of het instellen van het account van het abonnement van de klant.
      
    >[!NOTE]
    > Noch u noch uw klant ontvangt een e-mailbericht met instructies voor het voltooien van het instellen/inrichten van het account voor dit type ISV-abonnement.)

    - Als uw abonnement wordt geleverd met een gratis proefversie van 30 dagen, wordt de gratis proefperiode automatisch toegepast. Als partner in het CSP-programma kunt u de gratis proefperiode voor aanbiedingen die u voor klanten aanschaft, niet in de weg staan. Zodra de gratis proefperiode is afgelopen, wordt de abonnementsperiode van start en wordt het abonnement omgezet in de betaalde status. Het abonnement wordt vervolgens automatisch vernieuwd volgens hetzelfde schema.
   
## <a name="update-subscriptions-with-add-ons"></a>Abonnementen bijwerken met invoegtoepassingen 

Als de klant een invoegaankoop wilt aanschaffen, moet deze eerst een actief basisabonnement hebben.  U kunt invoegtoepassingen niet aanschaffen via de catalogus.

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Onder de **sectie Status** vindt u een lijst met beschikbare invoegtoepassingen voor het abonnement.  

5. Werk het aantal licenties voor elke vereiste invoeging bij. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

De mogelijkheid om invoegtoepassingen te kopen via Partner Center is alleen beschikbaar voor directe factuur- en indirecte providers.
Alleen in aanmerking komende invoegtoepassingen worden weergegeven op basis van de basisvereisten en regionale beschikbaarheid. Raadpleeg de aanbiedingsmatrix voor cloud resellers voor meer informatie over prijzen en aanbiedingen. Als u het basisabonnement onderbreekt, worden ook alle bijbehorende invoegtoepassingen onderbroken.

Begindatums voor invoegtoepassingen worden afgestemd met het basisabonnement en de kosten worden berekend op basis van de begindatum van de kosten en de einddatum van de kosten met pro rata kosten op de eerste factuur. Zie Op licenties gebaseerde facturering [voor meer informatie.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Een abonnement opschorten of annuleren

Partners kunnen een abonnement opzeggen of annuleren als dit wordt aangevraagd door de klant, of in het geval van niet-vooruitbetaling of fraude.

### <a name="suspend-a-subscription"></a>Een abonnement opschorten

Wanneer u de status van een abonnement wijzigt in **Tijdelijk,** kunnen gebruikers zich niet aanmelden of toegang krijgen tot services.

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Kies **Onderbroken** bij **Status**. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd, of 90 dagen plus het aantal dagen tussen het moment dat het account is geopend en de eerste factureringsperiode (maximaal 120 dagen).

Wanneer u een abonnement onder de  knop Tijdelijk opschorten ziet, wordt aangegeven wanneer het abonnement automatisch verloopt als u het abonnement niet opnieuw activeren. 

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Als u nieuwe commerce-abonnementen wilt opschorten of nieuwe commerce-abonnementen opnieuw wilt activeren, maakt u een serviceaanvraag en neem contact op met de ondersteuning. 

Self-serve opschorten en opnieuw activeren vanuit Partner Center dashboard en API's zijn mogelijk in de toekomst beschikbaar.

> [!NOTE]
> CSP-abonnementen hebben geen verlopen periode (zoals web-directe abonnementen) waarin de services nog steeds werken, maar het abonnement geen factureringskosten genereert. CSP-abonnementen zijn actief of tijdelijk (of volledig verwijderd).

### <a name="cancel-a-subscription"></a>Een abonnement annuleren

U kunt op licenties gebaseerde SaaS-abonnementen van ISV-uitgevers van derden annuleren binnen de Partner Center [commerciële marketplace.](csp-commercial-marketplace-overview.md) Zolang u binnen de annuleringsperiode annuleert, ontvangt u een volledige restitutie.

Voor ISV-aanbiedingen die maandelijks worden gefactureerd:

- Als u minder dan 24 uur na het plaatsen van de order annuleert, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 24 uur na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.

Voor aanbiedingen die jaarlijks worden gefactureerd:

- Als u minder dan 14 dagen na het plaatsen van de bestelling annuleert, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 14 dagen na het plaatsen van de order annuleert, wordt de annulering gepland bij verlenging.

Nadat deze perioden zijn afgelopen, ziet u niet langer de optie om het abonnement te annuleren.

> [!NOTE]
> ISV-services van derden (die bijvoorbeeld gebruikmaken van virtuele machines of containers) op basis van gebruik en naar gebruik, komen niet in aanmerking voor retournering. Op gebruik gebaseerde services kunnen worden gede inrichting als annuleringsmethode. Omdat kosten na gebruik worden gefactureerd, komen deze services niet in aanmerking voor restitutie.

Ga als volgt te werk om een SaaS-abonnement op basis van een licentie van een ISV-uitgever te annuleren:

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Zoek het abonnement dat u wilt annuleren.

4. Selecteer annuleren **in** de kolom **Status.** Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Als er een dialoogvenster wordt weergegeven, vult u relevante gegevens in en selecteert u **Verzenden.**

6. Selecteer Ja, annuleren om de annulering **te bevestigen.**

> [!NOTE]
> U kunt er ook voor kiezen om een abonnement Azure Marketplace met behulp van API's. Zie Een abonnement op Azure Marketplace [annuleren om dit te doen.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="cancel-a-new-commerce-subscription"></a>Een nieuw commerce-abonnement annuleren

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Voor nieuwe commerceaanbiedingen kunt u het abonnement op elk moment vóór de toezeggingsperiode opzeggen. Wanneer u een abonnement annuleert, verliest de klant onmiddellijk toegang tot de service. De toegang kan niet worden hersteld na annulering. De volgende annuleringsopties zijn beschikbaar voor een partner nadat het abonnement is aangeschaft: 

- Binnen 24 uur na de begindatum van het abonnement: u kunt het hele abonnement binnen de eerste 24 uur opzeggen voor volledige restitutie.  
- Binnen 30 dagen na de begindatum van het abonnement: u kunt het hele abonnement binnen de eerste 30 dagen annuleren. U krijgt een restitutie voor het volledige bedrag minus het pro-rated bedrag voor de dagen dat u het abonnement hebt gebruikt.
- Na 30 dagen na de begindatum van het abonnement: u kunt het abonnement niet annuleren.

### <a name="pause-and-resume-a-new-commerce-subscriptions"></a>Een nieuw commerce-abonnement onderbreken en hervatten 

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

In het geval van niet-betaling van de klant, ook wel het 'dunningscenario' genoemd, kunnen partners hun abonnement onderbreken en hervatten om de toegang van de klant tot de services van het abonnement onmiddellijk te blokkeren.

Als de abonnementen van de klant worden onderbroken, wordt de mogelijkheid om zich aan te melden en hun services te gebruiken uitgeschakeld totdat het abonnement wordt hervat.   

U kunt een abonnement onderbreken met behulp van Partner Center:

1. Ga naar de abonnementspagina van de klant en selecteer het abonnement dat u wilt onderbreken

2. Selecteer het **keuzerondje** Suspend

3. Lees de pop-up modaal en selecteer **OK**

4. Het abonnement heeft nu een onderbroken status en de partner wordt nog steeds gefactureerd voor het abonnement

Onderbreken is een herstelbare status via Partner Center gebruikersinterface of API's waarmee de toegang van een klant tot de services van een abonnement onmiddellijk wordt hersteld. 

>[!IMPORTANT] 
> Als u een abonnement onderpauzeert, worden alle instellingen voor automatisch verlengen uitgeschakeld en worden eventuele bestaande wijzigingen verwijderd. Het aanbieden van een subscriptoin heeft alleen invloed op de toegang tot de service van de klant. De facturering van de partner blijft in de onderbroken status.

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription-or-a-new-commerce-subscription"></a>Kies of u een abonnement op de commerciële marketplace of een nieuw commerce-abonnement automatisch wilt verlengen

> [!Note] 
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

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Sommige wijzigingen in abonnementen kunnen alleen aan het einde van een termijn plaatsvinden. Deze wijzigingen kunnen worden gepland zodat ze gemakkelijk aan het einde van de term worden toegepast. Voorbeelden van wijzigingen die moeten worden gepland:

- SKU downgrades
- Kortingen van de seat
- Wijzigingen in verschillende voorwaarden
- Wijzigingen in factureringsfrequentie

Andere wijzigingen, zoals upgrades of toename van de seat, kunnen tijdens de periode worden toegepast.

Planningswijzigingen vinden plaats bij verlenging wanneer het abonnement wordt verlengd voor de volgende termijn.

Vereisten voor geplande wijzigingen:

- Abonnement is actief 
- Automatisch verlengen is aan
- SKU moet in aanmerking komen voor een upgrade voor geplande upgrades

Een nieuwe wijziging plannen bij verlenging

1. Meld u aan bij Partner Center dashboard.

2. Kies een **klant** in de lijst met klanten.

3. Kies het abonnement dat u wilt beheren.

4. Selecteer **Vernieuwingen beheren.**

5. Selecteer een andere Waardewijziging voor SKU, hoeveelheid, termijn of factureringsfrequentie:

   - **Current** is de huidige waarde van het abonnement 

   - **Wijzigen** in is de laatst opgeslagen waarde die u wilt toepassen bij verlenging van het nieuwe abonnement 

6. Selecteer **Verzenden**

7. De wijzigingen vinden plaats bij verlenging. 

Partners hebben toegang tot **Vernieuwingen beheren om** bestaande geplande wijziging weer te geven, bij te werken of te verwijderen.

> [!Note] 
>- Proefversies zijn standaard ingesteld op conversie naar de betaalde SKU aan het einde van hun termijn. 
>- Voor geplande SKU-upgrades/downgrades moet het opnieuw toewijzen van gebruikerslicenties handmatig worden uitgevoerd.
>- Opgeslagen geplande wijzigingen worden verwijderd als de volgende updates op de korte termijn worden doorgevoerd in het abonnement.

### <a name="partial-upgrades-in-new-commerce-subscriptions"></a>Gedeeltelijke upgrades in nieuwe commerce-abonnementen

> [!Note] 
> Nieuwe commercewijzigingen zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Met gedeeltelijke upgrades kan een partner bepaalde licenties van de ene SKU naar de andere aanwijzen. Bij de vorige upgrade in traditionele abonnementen op basis van licenties konden alleen alle licenties worden bijgewerkt. Nieuwe handel stelt een partner in staat om bepaalde licenties op hun gemak te verplaatsen. Hierdoor heeft de partner meer controle over het beheer van upgrades, waardoor sommige gebruikers naar een nieuwe SKU kunnen worden verplaatst zonder ze allemaal te verplaatsen. 

Gedeeltelijke upgrades kunnen aan het einde van een termijn worden gepland of op de korte termijn worden gestart. 

Gedeeltelijke upgradedetails:

- Gedefinieerd als gedeeltelijk als het aantal upgradelicenties anders is dan het initiële abonnement.
- Als u een upgrades op de korte termijn start, worden bestaande geplande upgrades verwijderd.
- Upgrades kunnen alleen worden gestart vanuit abonnementen met de **status** Actief.
- Een nieuw abonnement dat is gemaakt tijdens het upgraden, heeft dezelfde einddatums als het abonnement waar de upgrade van afkomstig is.

Partners hebben toegang tot het abonnement waarvoor ze een upgrade willen uitvoeren bij het configureren van het aantal licenties en het abonnement waarvoor ze een upgrade willen uitvoeren. Partners kunnen een nieuw **abonnement** selecteren of een bestaand abonnement selecteren.

## <a name="next-steps"></a>Volgende stappen

- [Commerciële marketplace-producten kopen voor uw klanten](csp-commercial-marketplace-purchase.md)

- [Commerciële marketplace-producten voor uw klanten beheren](csp-commercial-marketplace-manage.md)

- [Overzicht van commerciële marketplace](csp-commercial-marketplace-overview.md)
