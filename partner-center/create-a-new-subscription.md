---
title: Klant abonnementen maken in het partner centrum
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het verkopen van uw klanten abonnementen voor producten die door micro soft zijn gepubliceerd, evenals SaaS-producten die zijn gepubliceerd door onafhankelijke software fabrikanten.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528584"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Klantabonnementen maken, onderbreken of annuleren

**Van toepassing op**

- Partnercentrum
- Partner centrum voor Microsoft Cloud voor de Amerikaanse overheid
- CSP-partners

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Globale beheerder
- Helpdesk medewerker
- Verkoop agent

Nadat u een record van uw klant in het partner centrum hebt gemaakt, kunt u deze abonnementen verkopen aan producten in de catalogus. Dit geldt ook voor producten die door micro soft worden gepubliceerd, evenals SaaS-producten (Software as a Service) die door onafhankelijke software leveranciers (Isv's) van derden naar de [commerciële Marketplace](https://azuremarketplace.microsoft.com/marketplace)worden gepubliceerd.

Sommige aanbiedingen zijn beperkt tot één abonnement per klant. Ga naar de pagina prijzen en aanbiedingen van het partner centrum om een lijst weer te geven van welke aanbiedingen zijn beperkt.

> [!IMPORTANT]
> Als partner in het CSP-programma kunt u alleen SaaS-abonnementen op **basis van licenties** kopen van ISV-uitgevers in het partner centrum. Dit betekent dat u een **op licenties gebaseerde SaaS-** aanbieding kunt kopen die de ISV-Uitgever voor u beschikbaar heeft gesteld, met inbegrip van [exclusieve aanbiedingen](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) waartoe u toegang hebt. Ga naar de [Azure-beheer Portal](https://portal.azure.com/)om andere commerciële Marketplace-aanbiedingen van onafhankelijke software leveranciers te kopen of beheren (zoals **op gebruik gebaseerde** , gecontroleerde of op verbruiks gebaseerde aanbiedingen voor Azure-toepassingen, containers of vm's). Zie [commerciële Marketplace-producten kopen](csp-commercial-marketplace-purchase.md)voor meer informatie.

## <a name="create-a-new-subscription"></a>Een nieuw abonnement maken

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Selecteer **abonnement toevoegen** . Op het tabblad **Online Services** worden alle beschik bare SaaS-aanbiedingen voor Marketplace weer gegeven.

4. Als u alleen bepaalde typen abonnementen wilt zien, selecteert u de gewenste opties in de beschik bare filters:
   - **Uitgever** : Kies **micro soft** om alleen aanbiedingen van micro soft of **partner** te bekijken voor commerciële Marketplace-producten die door isv's worden gepubliceerd.
   - **Facturerings type** : Selecteer het type abonnement facturering dat u wilt gebruiken: **licentie** of **gebruik** . Zie [factuur op basis van licenties](license-based-billing.md) voor informatie die u kan helpen bij het bepalen van de maandelijkse en jaarlijkse facturerings frequentie.
   - **Categorie** : Kies **Enter prise** , **Small Business** of **proef versie** . Zie voor meer informatie over proef abonnementen [uw klanten een proef versie van micro soft-producten aanbieden](offer-your-customers-trials-of-microsoft-products.md).

5. Selecteer de product abonnementen die u wilt kopen voor uw klant. De producten die u ziet, zijn afhankelijk van het type klant segment (onderwijs, overheid enz.) en de filters die u hebt toegepast. Sommige aanbiedingen die op Marketplace worden weer gegeven, zijn mogelijk niet altijd beschikbaar voor een specifieke klant of een specifieke CSP-partner. Dit kan een van de volgende zijn:

   - De klant heeft al een abonnement op dat product en is slechts toegestaan

   - Het abonnement van de klant is mogelijk opgeschort (in dit geval kunt u het abonnement opnieuw activeren in plaats van een nieuwe te kopen.)

   - Voor ISV SaaS-aanbiedingen kunnen er een paar redenen zijn waarom de aanbieding niet beschikbaar is voor aankoop: de ISV biedt mogelijk geen ondersteuning voor het factuur land of de regio van de klant. de ISV heeft mogelijk ervoor gekozen om de aanbieding niet beschikbaar te stellen via het CSP-programma; het is ook mogelijk dat de ISV de aanbieding [exclusief](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) heeft gemaakt voor bepaalde CSP-partners. De ISV-aanbieding kan ook niet worden verwerkt via het partner centrum (bijvoorbeeld containers of bepaalde op gebruik gebaseerde aanbiedingen).  

6. Voer het aantal licenties (indien nodig) in voor elk abonnement dat u wilt toevoegen en selecteer **toevoegen aan winkel wagen** .

7. Wanneer u klaar bent met het toevoegen van abonnementen, selecteert u uw bestelling **controleren** en controleren.

8. Wanneer u uw orders hebt gecontroleerd en u klaar bent om deze abonnementen te kopen, selecteert u **kopen** .

9. Nadat u een abonnement voor een klant hebt gekocht, gebeurt het volgende:

    - U kunt het abonnement bekijken of bewerken door de naam van het abonnement te selecteren op de pagina **abonnementen** van die klant. Hier kunt u licenties voor invoeg toepassingen selecteren als er een beschikbaar is, het aantal licenties wijzigen of het abonnement opschorten.

    **Voor ISV SaaS-abonnementen (op basis van licenties):**
    - U ontvangt een koppeling naar de site van de ISV-Uitgever. Deze koppeling helpt u bij het volt ooien van de implementatie of het instellen van het account voor het abonnement van de klant.
      
    >[!NOTE]
    > U en uw klant ontvangen geen e-mail bericht met instructies voor het volt ooien van het account dat is ingesteld/inrichten voor dit type ISV-abonnement.)

    - Als uw abonnement wordt geleverd met een gratis proef versie van 30 dagen, wordt de gratis proef periode automatisch toegepast. Als partner in het CSP-programma kunt u de gratis proef periode van aanbiedingen die u aanschaft voor klanten niet kwijt schelden. Zodra de gratis proef periode is afgelopen, wordt de abonnements termijn gestart en wordt het abonnement omgezet in de betaalde status. Het abonnement wordt vervolgens automatisch verlengd volgens hetzelfde schema.
   
## <a name="update-subscriptions-with-add-ons"></a>Abonnementen bijwerken met invoegtoepassingen 

Als u een invoegtoepassing wilt kopen, moet de klant eerst een actief basisabonnement hebben.  U kunt invoegtoepassingen niet aanschaffen via de catalogus.

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Onder de sectie **status** ziet u een lijst met beschik bare invoeg toepassingen voor het abonnement.  

5. Werk het aantal licenties voor elke vereiste invoeg toepassing bij. Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

De mogelijkheid om invoeg toepassingen te kopen via partner centrum is alleen beschikbaar voor directe factuur-en indirecte providers.
Alleen in aanmerking komende invoeg toepassingen worden weer gegeven op basis van de basis vereisten en regionale Beschik baarheid. Raadpleeg de aanbiedingsmatrix voor cloudresellers voor meer informatie over prijzen en aanbiedingen.  Als u het basisabonnement onderbreekt, worden ook alle bijbehorende invoegtoepassingen onderbroken.

Begindatums voor invoegtoepassingen worden afgestemd met het basisabonnement en de kosten worden berekend op basis van de begindatum van de kosten en de einddatum van de kosten met pro rata kosten op de eerste factuur. Zie voor meer informatie [facturering op basis van licenties](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Een abonnement opschorten of annuleren

Partners kunnen een abonnement opschorten of annuleren indien dit wordt aangevraagd door de klant of in gevallen van niet-betaling of fraude.

### <a name="suspend-a-subscription"></a>Een abonnement opschorten

Wanneer u de status van een abonnement wijzigt in **opgeschort** , kunnen gebruikers zich niet aanmelden of hebben geen toegang tot services.

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Kies het abonnement dat u wilt beheren.

4. Kies **Onderbroken** bij **Status** . Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Alle gegevens worden verwijderd, tenzij het abonnement binnen 90 dagen opnieuw wordt geactiveerd 90, plus het aantal dagen tussen het tijdstip waarop het account is geopend en de eerste facturerings periode (Maxi maal 120 dagen).

Wanneer u een abonnement uitbreekt, wordt de datum weer gegeven die u onder de **onderbroken** knop ziet wanneer het abonnement automatisch verloopt als u het niet opnieuw activeert. 

### <a name="cancel-a-subscription"></a>Een abonnement annuleren

U hebt de mogelijkheid om op licenties gebaseerde SaaS-abonnementen te annuleren vanuit ISV-uitgevers van derden binnen de [commerciële Marketplace](csp-commercial-marketplace-overview.md)van partner Center. Zolang u de annulerings periode hebt geannuleerd, ontvangt u een volledige terugbetaling.

Voor ISV-aanbiedingen worden maandelijks gefactureerd:

- Als u minder dan 24 uur annuleert nadat u de order hebt geplaatst, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 24 uur annuleert nadat u de order hebt geplaatst, wordt de annulering gepland om te worden uitgevoerd bij het vernieuwen.

Voor aanbiedingen die jaarlijks worden gefactureerd:

- Als u minder dan 14 dagen na het plaatsen van de bestelling annuleert, ontvangt u een volledig tegoed op de volgende factuur.

- Als u later dan 14 dagen na het plaatsen van de order annuleert, wordt de annulering gepland om te worden uitgevoerd bij het vernieuwen.

Nadat deze peri Oden zijn afgelopen, ziet u niet langer de optie om het abonnement te annuleren.

> [!NOTE]
> Op basis van gebruik en meting van de ISV-services van derden (die bijvoorbeeld virtuele machines of containers gebruiken) komen niet in aanmerking voor retour. Op gebruik gebaseerde services kunnen niet worden ingericht als een annulerings methode. Omdat kosten worden gefactureerd na gebruik, komen deze services niet in aanmerking voor een restitutie.

Ga als volgt te werk om een SaaS-abonnement op basis van een licentie van een ISV-uitgever te annuleren:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Zoek het abonnement dat u wilt annuleren.

4. Selecteer **Annuleren** in de kolom **status** . Kies vervolgens **Verzenden** om de wijzigingen vast te leggen.

5. Als er een dialoog venster wordt weer gegeven, vult u de relevante gegevens in en selecteert u vervolgens **verzenden** .

6. Selecteer **Ja, annuleren** om de annulering te bevestigen.

> [!NOTE]
> U kunt er ook voor kiezen om een Azure Marketplace-abonnement te annuleren met behulp van Api's. Zie [een abonnement op Azure Marketplace annuleren](/partner-center/develop/cancel-an-azure-marketplace-subscription)als u dit wilt doen.

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Kies of u automatisch een abonnement op commerciële Marketplace wilt vernieuwen

Actieve abonnementen zijn standaard ingesteld om automatisch te worden verlengd wanneer de abonnementsperiode verloopt. Voor [abonnementen op commerciële Marketplace-Producten](csp-commercial-marketplace-overview.md)kunt u ervoor kiezen om het abonnement optioneel niet automatisch te vernieuwen.

Als u wilt voor komen dat een actief abonnement op commerciële Marketplace automatisch wordt vernieuwd:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Selecteer **Abonnementen** . Hier vindt u een overzicht van de op licenties gebaseerde abonnementen die u hebt aangeschaft voor de klant.

4. Selecteer in de kolom **abonnement** het abonnement dat u wilt wijzigen.

5. Zoek op de pagina abonnements Details het gedeelte **status** en schakel het selectie vakje **automatisch verlengen** uit.

6. Selecteer **Indienen** .

## <a name="next-steps"></a>Volgende stappen

- [Commerciële Marketplace-producten kopen voor uw klanten](csp-commercial-marketplace-purchase.md)

- [Commerciële Marketplace-Producten voor uw klanten beheren](csp-commercial-marketplace-manage.md)

- [Overzicht van commerciële Marketplace](csp-commercial-marketplace-overview.md)