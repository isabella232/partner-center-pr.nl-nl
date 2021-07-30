---
title: Klantabonnementen maken in Partner Center
ms.topic: how-to
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het verkopen van abonnementen aan uw klanten voor producten die zijn gepubliceerd door Microsoft en SaaS-producten die zijn gepubliceerd door ISV's van derden.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 199e3dc42a0aa46c3e743e9e6fcb0ed585cd0303
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114838016"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Klantabonnementen maken, onderbreken of annuleren

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale beheerders | Helpdeskagent | Verkoopagent

Nadat u een record van uw klant in de Partner Center hebt gemaakt, kunt u ze abonnementen verkopen aan producten in de catalogus. Dit omvat producten die zijn gepubliceerd door Microsoft en SaaS-producten (Software as a Service) die door onafhankelijke onafhankelijke softwareleveranciers (ISV's) zijn gepubliceerd op [de commerciële marketplace.](https://azuremarketplace.microsoft.com/marketplace)

Sommige aanbiedingen zijn beperkt tot één abonnement per klant. Als u een lijst wilt bekijken met aanbiedingen die beperkt zijn, gaat u naar Partner Center pagina Met prijzen en aanbiedingen.

>[!IMPORTANT]
> Als partner in het CSP-programma kunt u  SaaS-abonnementen op basis van licenties of SaaS-abonnementen met een datalicentie kopen bij **ISV-uitgevers** binnen Partner Center. Dit betekent dat u elke  SaaS-aanbieding op basis van licenties of naar [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) gebruik kunt aanschaffen die de **ISV-uitgever** voor u beschikbaar heeft gesteld, inclusief exclusieve aanbiedingen waarvoor u toegang hebt. Als u andere commerciële marketplace-aanbiedingen van ISV's wilt kopen of beheren (zoals aanbiedingen op basis van gebruik met Betrekking tot Azure-toepassingen, containers of VM's), moet u naar de [Azure Portal.](https://portal.azure.com/)

>[!NOTE]
>Alle datums en tijden in Partner Center worden opgegeven in de UTC-tijdstandaard (Universal Time Coordinated). Dit kan tot 24 uur verschillen van uw lokale tijd.

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

    **Voor ISV SaaS-abonnementen (op basis van licenties en naar licentie) geldt het volgende:**
    - U ontvangt een koppeling naar de site van de ISV-uitgever. Deze koppeling helpt u bij het voltooien van de implementatie of het instellen van het account van het abonnement van de klant.
      
    >[!NOTE]
    > Noch u noch uw klant ontvangt een e-mailbericht met instructies voor het voltooien van het instellen/inrichten van het account voor dit type ISV-abonnement.)

    - Als uw abonnement wordt geleverd met een gratis proefversie van 30 dagen, wordt de gratis proefperiode automatisch toegepast. Als partner in het CSP-programma kunt u de gratis proefperiode voor aanbiedingen die u voor klanten aanschaft, niet in de weg staan. Zodra de gratis proefperiode is afgelopen, begint de abonnementsperiode en wordt het abonnement omgezet in de betaalde status. Het abonnement wordt vervolgens automatisch vernieuwd volgens hetzelfde schema.
   
## <a name="update-subscriptions-with-add-ons"></a>Abonnementen bijwerken met invoegtoepassingen 

Als de klant een invoegaankoop wilt aanschaffen, moet deze eerst een actief basisabonnement hebben.  U kunt invoegtoepassingen niet aanschaffen via de catalogus.

1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)

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

1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Kies **Onderbroken** bij **Status**. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd, of 90 dagen plus het aantal dagen tussen het moment dat het account is geopend en de eerste factureringsperiode (maximaal 120 dagen).

Wanneer u een abonnement onder de  knop Tijdelijk opschorten ziet, wordt aangegeven wanneer het abonnement automatisch verloopt als u het abonnement niet opnieuw activeren. 

>[!NOTE]
>CSP-abonnementen hebben geen verlopen periode (zoals web-directe abonnementen) waarin de services nog steeds werken, maar het abonnement geen factureringskosten genereert. CSP-abonnementen zijn actief of tijdelijk (of volledig verwijderd).

### <a name="cancel-a-subscription"></a>Een abonnement annuleren

U kunt SaaS-abonnementen op basis van licenties van ISV-uitgevers van derden annuleren binnen de Partner Center [commerciële marketplace.](csp-commercial-marketplace-overview.md) Zolang u binnen de annuleringsperiode annuleert, ontvangt u een volledige restitutie.

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

1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Zoek het abonnement dat u wilt annuleren.

4. Selecteer annuleren **in** de kolom **Status.** Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Als er een dialoogvenster wordt weergegeven, vult u relevante gegevens in en selecteert u **Verzenden.**

6. Selecteer Ja, annuleren om de annulering **te bevestigen.**

> [!NOTE]
> U kunt er ook voor kiezen om een abonnement Azure Marketplace annuleren met behulp van API's. Zie Een abonnement op Azure Marketplace [annuleren om dit te doen.](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Kiezen of u een abonnement op de commerciële marketplace automatisch wilt verlengen

Actieve abonnementen zijn standaard ingesteld om automatisch te worden verlengd wanneer de abonnementsperiode verloopt. Voor [abonnementen op commerciële marketplace-producten](csp-commercial-marketplace-overview.md)kunt u ervoor kiezen om het abonnement niet automatisch te verlengen.

Als u wilt voorkomen dat een actief abonnement op de commerciële marketplace automatisch wordt verlengd:

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer **Abonnementen**. Hier worden alle op licenties gebaseerde abonnementen vermeld die u voor de klant hebt aangeschaft.

4. Selecteer in **de** kolom Abonnement het abonnement dat u wilt wijzigen.

5. Zoek op de pagina met abonnementsdetails **de sectie Status** en vink het selectievakje Automatisch **verlengen** uit.

6. Selecteer **Indienen**.

## <a name="next-steps"></a>Volgende stappen

- [Commerciële marketplace-producten kopen voor uw klanten](csp-commercial-marketplace-purchase.md)

- [Commerciële marketplace-producten voor uw klanten beheren](csp-commercial-marketplace-manage.md)

- [Overzicht van commerciële marketplace](csp-commercial-marketplace-overview.md)