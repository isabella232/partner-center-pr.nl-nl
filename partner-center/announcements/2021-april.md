---
title: Aankondigingen van april 2021
description: Aankondigingen van april 2021 voor Microsoft Partner Center met inbegrip van nieuwe mogelijkheden, promoties, aanbiedingen, markten of wijzigingen in bestaande aanbiedingen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-action-center
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 31f6fadc0eb25b899bc2dee3a0475daf17c54c2c
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841756"
---
# <a name="april-2021-announcements"></a>Aankondigingen van april 2021

Deze pagina bevat de aankondigingen voor Microsoft Partner Center voor april 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Gereedheid: De validatie-API voor CSP-klantadressen wordt live in juni bijgewerkt; testmogelijkheid nu beschikbaar

### <a name="categories"></a>Categorieën

- Datum: 2021-04-30
- Gereedheid

### <a name="summary"></a>Samenvatting

Om partners en klanten te helpen hun bedrijf te runnen op basis van vertrouwen, nodigen we partners uit om wijzigingen in de Adres-API valideren voor alle landen over de hele wereld te testen.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

CSP-partners voor directe factuur en indirecte providers die nieuwe adresgegevens van bestaande klanten maken of bijwerken

### <a name="details"></a>Details

Microsoft wordt uitgevoerd op vertrouwen. We zetten ons in voor een compatibele, veilige en veilige methode voor validatie van klantadressen voor het transacteren van klantabonnementen in het CSP-programma. Vanaf 31 maart 2021 zijn er wijzigingen aangebracht in de Adres-API valideren. We nodigen partners uit om de API vóór de go-live eind juni 2021 te testen. 

Houd er rekening mee dat deze wijzigingen alleen van invloed zijn op de ADRES-API valideren. Api's voor klant- en updateprofiel maken worden niet beïnvloed. Hoewel het voorgestelde adres momenteel niet hoeft te worden gebruikt met de API Klant maken, wordt dit ten zeerste aanbevolen.

Het antwoord retournt een van de volgende statusberichten:

| Status     | Beschrijving |    Aantal geretourneerde voorgestelde adressen |
|-------|---------------|-------------------|
|Geverifieerd verzendbaar | Het adres wordt geverifieerd en kan worden verzonden naar . | Enkelvoudig |
|Geverifieerd | Het adres wordt geverifieerd. | Enkelvoudig |
|Interactie vereist | Voorgesteld adres is aanzienlijk gewijzigd en er is een gebruikersbevestiging nodig. | Enkelvoudig |
|Gedeeltelijk straat | De opgegeven straat in het adres is gedeeltelijk en heeft meer informatie nodig. | Meerdere, maximaal drie |
|Gedeeltelijk lokaal | De opgegeven locatie (gebouwnummer, suitenummer en andere) is gedeeltelijk en heeft meer informatie nodig. | Meerdere, maximaal drie |
|Meerdere | Er zijn meerdere velden die gedeeltelijk in het adres zijn (mogelijk ook gedeeltelijk en gedeeltelijk van de straat). | Meerdere, maximaal drie |
|Geen | Het adres is onjuist. | Geen |
|Niet gevalideerd | Het adres kan niet worden verzonden via het validatieproces. | Geen |

Amerikaanse postcodes retourneren nog eens vier cijfers + afbreekstreetine, bijvoorbeeld 12345-6789.

### <a name="next-steps"></a>Volgende stappen

- Bekijk de technische documentatie en veelgestelde vragen in de [speciale partnerverzameling](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) voor meer gedetailleerde richtlijnen.
- Bereid u voor op het opnemen van de wijzigingen met behulp Partner Center API en webgebruikerservaring. 
- Deel uw tenant-id voor de sandbox met de expert op het gebied van onderwerp (Ali Wiltki) die moet worden opgenomen in de test flight, zodat u kunt beginnen met het voorbereiden van de update. 
- Als u een CPV-oplossing (Panel Vendor) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Als u ondersteuning nodig hebt voor uw bewerkingen met Microsoft, kunt u contact met uw partnerondersteuningsgroep Yammer of een [serviceaanvraag openen.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nieuwe locatie voor Partner Center API Swagger-documentatie

### <a name="categories"></a>Categorieën

- Datum: 2021-04-26
- Functies

### <a name="summary"></a>Samenvatting

Partner Center API Swagger-documenten zijn gemigreerd van de vorige [site voor Swagger-documentatie](https://apidocs.microsoft.com/services/partnercenter) naar een nieuwe [site met Swagger-documentatie.](/rest/api/partner-center-rest/)

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners voor directe factuur en indirecte providers die deelnemen aan het Cloud Solution Provider (CSP)-programma dat gebruik maakt van de Partner Center API's

### <a name="details"></a>Details

Vanaf 26 april 2021 bevindt de Partner Center API Swagger-documentatie, inclusief REST API-inhoud, zich op een [nieuwe site.](/rest/api/partner-center-rest/) De oude site is na enkele weken niet meer toegankelijk.

### <a name="benefits"></a>Voordelen

De Partner Center API Swagger-documentatie biedt de **functie Try It.** Als u deze functie wilt gebruiken, moet u een Bearer-token hebben, dat u kunt genereren door de stappen te volgen die worden vermeld in [Partner Center Verificatie.](/partner-center/develop/partner-center-authentication#app--user-authentication)

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie binnen uw organisatie, zodat het juiste team de processen kan controleren en bijwerken.

### <a name="questions"></a>Vragen?

Als u vragen hebt over deze aanbiedingen, controleert u uw relevante Yammer community's.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Cloud Solution Provider (CSP)-beleid voor de retourperiode van software en de vervaldatum van de downloadkoppeling

### <a name="categories"></a>Categorieën

- Datum: 2021-04-21
- Functies

### <a name="summary"></a>Samenvatting

Er zijn wijzigingen in het beleid voor de retourperiode van de CSP-software en het verlopen van de downloadkoppeling.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners die permanente software of aanbiedingen van softwareabonnementen in CSP af te betalen

### <a name="details"></a>Details

Let op de volgende belangrijke meldingen met betrekking tot permanente software- en softwareabonnementaankopen via Partner Center:

#### <a name="software-return-period-policy"></a>Beleid voor retourperiode van software

Vanaf 1 juni 2021 verandert de retourperiode voor softwareaanbiedingen in CSP, zoals vermeld in de Microsoft Partner-overeenkomst (MPA), van 60 dagen vanaf orderdatum in 30 dagen na orderdatum.

Nadat een order voor een softwareaanbieding is verzonden, hebben partners 30 dagen vanaf de orderdatum de tijd om wijzigingen in een dergelijke volgorde in te dienen:

- Elke doorlopende softwarelicentie die binnen de retourperiode van 30 dagen wordt geretourneerd, ontvangt een volledig tegoed van de betaalde aankoopprijs.

- Elk softwareabonnementsproduct dat binnen de retourperiode van 30 dagen wordt geretourneerd, ontvangt een prorated tegoed van de betaalde aankoopprijs.

Dit bericht is een vervolg op onze e-mailberichten die op december 2020 en april 2021 naar alle CSP-partners zijn verzonden met betrekking tot de retourperiode en andere updates voor de MPA. Raadpleeg deze kennisgevingen voor meer informatie over wijzigingen die van invloed zijn op de MPA.

#### <a name="software-download-link-expiry"></a>Het downloaden van software verloopt

Vanaf 3 juni 2021 hebben de software downloadkoppelingen voor continue software- en softwareabonnementproductaankopen via Partner Center een vervaldatum van vijf dagen vanaf de eerste download. De verloopperiode is van toepassing op alle aankopen vóór 3 juni 2021, en op of na 3 juni 2021.

### <a name="next-steps"></a>Volgende stappen

Bekijk de [CSP-retourperiode en veelgestelde](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf)vragen over het verlopen van de downloadkoppeling en informeer alle juiste teams binnen uw organisatie over deze wijzigingen:

### <a name="questions"></a>Vragen?

Als u vragen hebt over deze aanbiedingen, controleert u uw relevante Yammer community's.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Licentieprogramma openen: resellers overstappen naar het Cloud Solution Provider (CSP)-programma

### <a name="categories"></a>Categorieën

- Datum: 2021-04-19
- Uw bedrijf laten groeien

### <a name="summary"></a>Samenvatting

Deze communicatie laat zien hoe u zich voorbereidt op de wijzigingen die binnenkort worden doorgevoerd in het Open Licensing-programma.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

CSP- en Open License-partners

### <a name="details"></a>Details

In 2020 heeft [Microsoft](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) aangekondigd dat doorlopende softwarelicenties breed beschikbaar zullen zijn voor partners en klanten via het Cloud Solution Provider (CSP)-programma. De eerste mijlpaal is bereikt in januari 2021, toen commerciële doorlopende softwareaanbiedingen beschikbaar werden. De volgende belangrijke mijlpaal vindt plaats in juli 2021, wanneer aanbiedingen voor openbare [sectoren](https://aka.ms/openlicensepublicsector) beschikbaar komen. We [hebben](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) ook gecommuniceerd dat met ingang van 1 januari 2022 geen nieuwe softwarelicentieaankopen of verlengingen van Software Assurance of onlineservices kunnen worden gedaan via het Open License-programma.

De overgang van permanente software naar het CSP-programma in de nieuwe commerce-ervaring helpt partners om de mogelijkheden voor het aanbieden van diverse oplossingen en beheerde services uit te breiden. Dit versnelt ook de overgang van klanten naar de cloud.  Om een soepele overgang te garanderen voor zowel onze partners als klanten, hebben we deze aanpassingen en materialen aangebracht om deze digitale transformatie te versnellen:

#### <a name="april-2021"></a>April 2021

[Nu beschikbaar:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)Open overgangsmateriaal voor licentie-naar-CSP voor resellers

#### <a name="july-2021"></a>Juli 2021

##### <a name="csp"></a>CSP

- 1 juli: Permanente softwarelicenties beschikbaar voor klanten in de publieke sector

- 7 juli: Visual Studio Pro en Get Genuine Windows licentie voor doorlopende overeenkomst voor software die beschikbaar is voor alle segmenten

##### <a name="open-value"></a>Waarde openen

- 1 juli: Aanvullende SKU's beschikbaar in het Open Value-programma voor onderwijs en non-profitorganisaties, met vergelijkbare aanbiedingen als het Open License-programma

##### <a name="open-license"></a>Licentie openen

- 1 juli: Microsoft zal geen nieuwe aanbiedingen meer starten in het programma Open License.

#### <a name="january-2022"></a>Januari 2022

- 1 januari: er kunnen geen nieuwe aankopen of verlengingen worden gedaan via het programma Open License

### <a name="next-steps"></a>Volgende stappen

#### <a name="csp-indirect-providers"></a>Indirecte CSP-providers

Gebruik de komende maanden om resellers met een open licentie te helpen zich in het CSP-programma te houden door evenementen van de partner-community te bezoeken en het overgangsmateriaal Open License-to-CSP voor resellers te gebruiken:

- [Open licentie-naar-CSP-overgangsmateriaal voor resellers:](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)aanpasbare overzichtspresentatie, e-mailsjabloon, onboardinghandleiding voor indirecte CSP-resellers en meer om u te helpen de acceptatie voor uw wederverkopers op schaal te stimuleren.

- [CSP Partner Community-gebeurtenissen die](https://globalpbocomm.eventbuilder.com/GlobalCSP) worden gehost door Microsoft Business Operations.  Neem deel aan de verschillende sessies om de basisbeginselen van CSP (basisprincipes van CSP) te leren of blijf up-to-date en stel vragen over Software in CSP (Q&A Sessions).

- (Binnenkort) Trainingssessie voor indirecte CSP-resellers die worden gehost door Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Licentie-resellers openen

- Als uw organisatie momenteel niet is ingeschreven bij het CSP-programma, neem dan contact op met uw distributeur voor informatie over hoe u aan de slag kunt gaan. Verbinding maken hier met een indirecte [provider](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).

- Als uw organisatie al is ingeschreven bij het CSP-programma, kunt u hier meer informatie vinden over continue software in [CSP.](https://partner.microsoft.com/resources/collection/software-in-csp)

### <a name="questions"></a>Vragen?

Voor meer vragen over deze aanbiedingen, controleert u uw relevante Yammer community's.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Nu live: Globale handleiding voor promotie-gereedheid

### <a name="categories"></a>Categorieën

- Datum: 2021-04-16
- Functies

### <a name="summary"></a>Samenvatting

Gereedheid starten heeft een nieuwe algemene handleiding voor [gereedheid voor promotie gepubliceerd](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in de operations-gereedheid-resourcegalerie. Deze handleiding biedt een geconsolideerde weergave van alle actieve [wereldwijde promoties.](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/)

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle volumelicenties (VL), Dynamics Price List (DPL) en Cloud Solution Provider (CSP)-partners

### <a name="details"></a>Details

Microsoft-partners hebben met ons gedeeld dat ze een geconsolideerde weergave moeten bieden van alle wereldwijde promoties met ondersteunende details. U wilde deze geconsolideerde handleiding gebruiken om promoties te gebruiken met het vertrouwen dat alle beschikbare informatie gemakkelijk toegankelijk is op een centrale en handige locatie.

Vanaf april 2021 werkt Microsoft deze handleiding maandelijks bij en is deze beschikbaar in een speciale global promo readiness Guide-verzameling in de resourcegalerie van Operations Readiness.

Koppelingen naar deze handleiding worden ook opgenomen in de volgende verzamelingen:

- [Start de agendaverzameling](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), die een gecentraliseerde weergave biedt van toekomstige wijzigingen en lanceringen.

- [Communityverzamelingen,](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)die ondersteunende materialen bevatten voor onze maandelijkse partnergesprekken, waarbij toekomstige wijzigingen en actuele onderwerpen van operationele interesse worden belicht.

- [Partner-nieuwsbrieven,](https://partner.microsoft.com/resources/collection/csp-monthly-update#/)zoals maandelijkse update van CSP

Als een maandelijkse herinnering publiceren we ook een Partner Center aankondiging met elk nieuw probleem van de algemene handleiding voor promotie-gereedheid.

### <a name="next-steps"></a>Volgende stappen

Aan het begin van elke maand vindt u de meest recente algemene handleiding voor [gereedheid](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) voor promotie in de [resourcegalerie van Operations Readiness.](https://partner.microsoft.com/resources)

Deel deze informatie met de juiste contactpersonen in uw organisatie en laat ons weten hoe nuttig de handleiding is via de pagina 'Was deze pagina nuttig?' aan het einde van elke pagina.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Update en Cloud Solution Provider van de CSP-community van april

### <a name="categories"></a>Categorieën

- Datum: 2021-04-16
- Community | Uitnodigingen en herinneringen

### <a name="summary"></a>Samenvatting

Resources van de CSP-community zijn op aanvraag beschikbaar en worden maandelijks bijgewerkt om u op de hoogte te houden en u voor te bereiden op veranderingen in het CSP-programma.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Directe CSP-factuurpartners en indirecte providers

### <a name="details"></a>Details

Deze maand bevatten de resources de volgende belangrijke onderwerpen:

- [Wijzigingen in het CSP-programma en open license-programma bijwerken](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Wijzigingen in de onboardingvereisten voor CSP-klanten in bepaalde regio's](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nieuwe indeling voor de nieuwe PDF-factuur voor commerce in het CSP-programma](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

In de [CSP-communityverzameling](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/)vindt u het volgende:

- De downloadbare [CSP Monthly Update-nieuwsbrief,](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global)waarin recente CSP-aankondigingen, updates, gebeurtenissen en herinneringen worden samengevoegd in een eenvoudig te lezen document.

- De [aankondigings agenda van de CSP,](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021)die een tijdlijnweergave biedt van toekomstige wijzigingen die van invloed zijn op het programma.

- De nieuwe [kalender voor productlancering,](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf)waar u toekomstige productlanceringen en -aanbiedingen kunt bekijken.

- [CSP start updatebronnen](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) met eenvoudig te gebruiken inhoud over belangrijke operationele wijzigingen.

- [Vernieuwingen en herinneringen over](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) belangrijke CSP-onderwerpen die interesse en query's ontvangen.

#### <a name="csp-community-call-qas"></a>CSP Community Call Q&As

Community Call Q&As zijn beschikbaar om u te helpen met vragen met betrekking tot toekomstige wijzigingen. Registreer u nu voor CSP Community Call Q&Zoals die plaatsvinden in april, mei en juni. Deze zijn gericht op de meest recente lanceringen, belangrijke vernieuwingen en herinneringen.

[Registreer u hier.](https://globalpbocomm.eventbuilder.com/GlobalCSP)

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources van de community en registreer u voor de Q-&A.

Om ervoor te zorgen dat u het meeste uit de Community Call Q&A kunt halen, bekijkt u de inhoud van de community op aanvraag en dient u uw vragen maximaal 48 uur vóór de oproep in.

### <a name="questions"></a>Vragen?

De maandelijkse CSP Community Call Q&A is de beste plek voor vragen met betrekking tot wijzigingen in het CSP-programma. Bekijk elke maand het materiaal en dien uw vragen van tevoren in, zodat we de sessie kunnen besteden aan de onderwerpen die voor u het belangrijkst zijn.

Neem contact op met ondersteuning voor [meer informatie.](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Laatste herinnering: afschaffing van de GET-kwalificatie op 6 mei 2021

### <a name="categories"></a>Categorieën

- Datum: 2021-05-04

- Functies

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners die academicus, non-profit en Government Community Cloud (GCC) verkopen via het Cloud Solution Provider-programma met behulp van de Partner Center-API

### <a name="details"></a>Details

Deze aankondiging is een vervolg op de verbeteringen Partner Center [in december zijn uitgebracht.](./2020-december.md#1) Als onderdeel van deze release zijn nieuwe API's voor GET- en POST-kwalificaties geïmplementeerd. Als gevolg hiervan wordt de bestaande GET-kwalificatie op 6 mei **2021** ingetrokken. Op dat moment moet u zijn overstappen op het gebruik van de nieuwe POST Partner Center API's. Met de nieuwe POST-API's kunt u Education-aanbiedingen aanschaffen, terwijl u met de nieuwe GET-API's vooraf gekwalificeerde non-profit- en GCC-aanbiedingen kunt aanschaffen.

### <a name="next-steps"></a>Volgende stappen

- **Werk bij naar de nieuwe API's** voor een geslaagde en tijdige overgang.

- **Bekijk de nieuwe api Partner Center wijzigingen en** handleiding in de Operations Readiness-resources: verbeteringen Partner Center [Education-klantvalidatieproces.](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

- Deel deze informatie met de juiste teams binnen uw organisatie en met uw wederverkopers om hen te helpen zich voor te bereiden op deze wijzigingen.

### <a name="questions"></a>Vragen?

Voor vragen met betrekking tot deze melding kunt u contact opnemen [met Partner Center ondersteuning.](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals)

### <a name="change-log"></a>Wijzigingenlogboek

- 4 mei 2021: Laatste herinnering van aanstaande afschaffing van GET-kwalificatie

- 9 april 2021: Herinnering aan aanstaande afschaffing van GET-kwalificatie 

- Februari: Bijgewerkte tijdlijnen voor het aftrekken van GET-& PUT-kwalificaties

- Januari: Herinnering aan aanstaande afschaffingen van GET-& PUT-kwalificaties

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nieuwe indeling voor de nieuwe PDF-factuur voor commerce in CSP

### <a name="categories"></a>Categorieën

- Datum: 2021-04-05
- Functies

### <a name="summary"></a>Samenvatting

Microsoft introduceert een nieuwe indeling voor de nieuwe PDF-factuur voor commerce in het Cloud Solution Provider-programma (CSP) om factureringsgegevens weer te geven op productdetails in plaats van SKU-beschrijving.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners die het CSP-programma gebruiken

### <a name="details"></a>Details

Vanaf mei 2021 introduceert Microsoft een nieuwe indeling voor de nieuwe PDF-factuur voor commerce in het CSP-programma om factureringsgegevens weer te geven op productdetails in plaats van SKU-beschrijving. Met deze nieuwe update aggregeren we de regelitems op producttype terwijl elk product op een afzonderlijke regel wordt weergegeven.

Partners zullen deze wijziging van kracht zien in hun factuur van mei voor de factureringsperiode tussen 1 april 2021 en 30 april 2021. De betrokken aanbiedingen zijn Microsoft Azure gereserveerde instantie, Azure-abonnementen (Azure-abonnement) en Marketplace.

Alle credit-rebill-aanvragen die worden gedaan nadat de factuurindeling is bijgewerkt, worden gegenereerd in de nieuwe indeling.

#### <a name="partner-benefits"></a>Voordelen van partners

Deze update biedt de volgende verbeteringen in de factureringservaring voor partners:

- Gereduceerde factuurgrootte met behoud van kritieke gegevens

- Afstemming van de indeling op de industriestandaarden voor compacte en gebruiksvriendelijke facturen 

De volgende elementen worden niet beïnvloed:

- Pagina factureringsoverzicht op de FACTUUR-PDF

- Bestaande facturerings-API's

- Afstemmingsbestanden (Recon-bestanden kunnen worden gebruikt voor het ophalen van gedetailleerde gegevens.) 

- Facturen voor gebruiks- en licentiekosten

### <a name="next-steps"></a>Volgende stappen

Lees de informatie over dit onderwerp in de [resourcegalerie Operations Readiness](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) op de website van de Microsoft-partner. Voor meer informatie over facturerings- en belastingonderwerpen, waaronder factureringsresources, facturen, CSP-facturering en belastingen, gaat u naar de sectie Facturering [in](../billing.md) Partner Center.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Wijzigingen in de onboardingvereisten Cloud Solution Provider de klant (CSP)

### <a name="categories"></a>Categorieën

- Datum: 2021-04-02
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

Als onderdeel van onze toezegging om partners en klanten te helpen hun bedrijf te runnen op basis van vertrouwen, vragen we aanvullende klantgegevens aan, met ingang van 25 maart 2021.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

CSP-partners voor directe factuur en indirecte providers die nieuwe of bestaande klanten hebben in de landen die in de volgende sectie worden vermeld

### <a name="details"></a>Details

Microsoft wordt uitgevoerd op vertrouwen. We zetten ons in voor een compatibele, veilige en veilige methode voor klantvalidatie voor het transacteren van klantabonnementen in het CSP-programma. Op 25 maart 2021 introduceren we verbeteringen in Partner Center API en gebruikersinterface (UI) die van invloed zijn op partners die aan beide van de volgende criteria voldoen:

- De partner heeft een directe factureringsrelatie met Microsoft (wat betekent dat de partner een partner voor directe facturering of een indirecte provider is).

- De partner doet zaken met nieuwe of bestaande klanten in de volgende landen:

    - Thailand
    - Vietnam
    - Turkije
    - Polen
    - Zuid-Afrika
    - India
    - Brazilië
    - Irak
    - Myanmar
    - Zuid-Soedan
    - Saoedi-Arabië
    - Verenigde Arabische Emiraten
    - Venezuela

Partners die aan de criteria voldoen, moeten de bedrijfsregistratie-id (ook wel de INN van de organisatie van de klant genoemd) en het telefoonnummer van een klant indienen wanneer ze de volgende keer een abonnement voor die klant bijwerken of maken. Deze partners kunnen ook een optionele middelste naam voor de klant invoeren.

Houd er rekening mee dat wanneer u uw bedrijfsregistratie-id toevoegt, u uw zakelijke btw-id moet gebruiken en niet de persoonlijke id van de klant.

Partners die zaken doen met nieuwe of bestaande klanten in de volgende landen, hebben al een eerdere versie van november 2020 in gebruik.

- Armenië
- Azerbeidzjan
- Belarus
- Hongarije
- Kazachstan
- Kirgistan
- Moldavië
- Rusland
- Tadzjikistan
- Oekraïne
- Oezbekistan

Partners met klanten in de rest van de wereld kunnen eind maart 2021 de bedrijfsregistratie-id, het telefoonnummer en de middelste naam voor klanten invoeren als optionele gegevens.

### <a name="next-steps"></a>Volgende stappen

- Bekijk de technische documentatie en veelgestelde vragen in de speciale [partnerverzameling](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) voor meer gedetailleerde richtlijnen.
- Bereid u voor op het opnemen van de wijzigingen Partner Center api en webgebruikerservaring. API's/SDK's zijn beschikbaar voor testen.
- Zorg ervoor dat u de aanvullende gegevens indient bij het onboarden van nieuwe klanten of het wijzigen van bestaande klantgegevens.
- Als u een CPV-oplossing (Panel Vendor) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Neem contact op met uw belastingadviseur of lokale belasting kantoor als u vragen hebt met betrekking tot de registratie-id van het bedrijf (ook wel INN of TIN genoemd). Microsoft kan geen richtlijnen geven over belastingzaken.

Als u ondersteuning nodig hebt voor uw bewerkingen met Microsoft, opent u een [serviceaanvraag.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Productlanceringen en aanbiedingen van deze maand weergeven

### <a name="categories"></a>Categorieën

- Datum: 2021-04-01
- Functies
 
### <a name="summary"></a>Samenvatting

De kalender voor productlancering van april 2021 is nu gepubliceerd.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle partners die het programma Cloud Solution Provider (CSP)

### <a name="details"></a>Details

De kalender voor productlancering van [april](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) 2021 is nu beschikbaar in de resourcegalerie Operations-gereedheid. Bekijk hier de komende productlanceringen en aanbiedingen.

### <a name="next-steps"></a>Volgende stappen

Bekijk de [kalender voor productlancering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/)en deel de informatie met de juiste belanghebbenden in uw organisatie.  

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante community's voor meer vragen over Yammer aanbiedingen.