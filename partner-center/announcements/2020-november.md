---
title: November 2020-aankondigingen
description: Mede delingen van november 2020 voor het micro soft-partner centrum, inclusief nieuwe mogelijkheden, aanbiedingen, aanbiedingen, markten of wijzigingen in bestaande aanbiedingen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691296"
---
# <a name="november-2020-announcements"></a>November 2020-aankondigingen

Op deze pagina vindt u informatie over de aankondigingen voor het micro soft partner centrum voor november 2020.

2020 aankondigingen: [april](2020-april.md)juni tot en met september tot en met  |  [May](2020-may.md)  |  [June](2020-june.md)  |  [July](2020-july.md)  |  [August](2020-august.md)  |  [September](2020-september.md)  |  [oktober](2020-October.md) | Maand

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>Wijzigingen in de facturerings valuta van de partner van de EU/EVA voor nieuwe Commerce aanbiedingen.  

### <a name="categories"></a>Categorieën
- Datum 2020-11-17
- Functies

### <a name="impacted-audience"></a>Doel groep  

Partners die communiceren via het programma Cloud solution provider in de regio EU/EVA 

### <a name="summary"></a>Samenvatting 

In de regio Europese Unie (EU)/European Free Trade Association (EVA) zal alle nieuwe Commerce aanbiedingen in het Cloud Solution Provider-programma de facturerings locatie van de partner gebruiken in plaats van de facturerings locatie van de klant. Dit betekent dat partners door micro soft worden gefactureerd op basis van hun locatie valuta, niet op de locatie valuta van de klant. Dit gebeurt in twee fasen: 

- **Fase 1: nieuwe klanten die een nieuwe Commerce-aanbieding kopen in CSP**

Vanaf januari 2021 worden partners die nieuwe klanten hebben, nieuwe Commerce aanbiedingen in rekening gebracht voor die aankopen in de valuta van de partner locatie. Partners met bestaande klanten die al nieuwe Commerce-aanbiedingen in CSP hebben gekocht, worden in de valuta van de facturerings locatie van de klant gefactureerd tijdens deze fase. 

 

- **Fase 2: bestaande klanten die een nieuwe Commerce-aanbieding in CSP hebben gekocht vóór 1 januari 2021** 

De volgende fase 1 en tijdens het kalender jaar 2021, micro soft zet de facturering van nieuwe Commerce-aanbiedingen voor partners met bestaande klanten over, die een nieuwe Commerce-aanbieding in CSP heeft gekocht vóór 2021 januari, van klant locatie valuta tot partner locatie valuta. Partners worden vooraf op de hoogte gesteld voordat deze wijziging wordt geïmplementeerd.  

>Eraan Deze wijziging is alleen van invloed op de facturerings valuta van de partner en niet op de prijzen van nieuwe Commerce-aanbiedingen in CSP. 

De nieuwe Commerce-aanbiedingen in het bereik voor deze wijziging zijn: Azure-abonnementen die deel uitmaken van een Azure-abonnement, Azure-reserve ringen, Server abonnementen, permanente software en micro soft Commercial Marketplace-aankopen in het Cloud Solution Provider-programma.

### <a name="partner-benefits"></a>Voor delen van partner  

- Deze update vermindert de complexiteit en de overhead met de facturering in meerdere valuta in de regio EU/EVA voor de nieuwe Commerce ervaring.  

- Partners ontvangen een geconsolideerde factuur in één valuta en ontvangen geen factuur meer voor elke locatie valuta van de klant. 

- Belonings uitbetalingen worden in dezelfde valuta als de factuur valuta van de partner.

- Partners zien een gereduceerde facturerings complexiteit die wordt veroorzaakt door het factureren van meerdere valuta's, waarmee tijd en resources worden vrijgemaakt die momenteel zijn gekoppeld aan het afstemmen van accounts. 

- Voor partners die nog geen nieuwe Commerce-aanbiedingen hebben toegepast, wordt deze wijziging afgestemd op het vorige partner-facturerings model, waardoor partners de nieuwe Commerce-ervaring in CSP gemakkelijker kunnen overstappen. 

### <a name="resources"></a>Resources 

Lees de informatie over dit onderwerp in de [Operations Gallery] ( https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ op de website van micro soft partner.  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>API-beperking naar partners die partner Center-Api's aanroepen

### <a name="categories"></a>Categorieën

- Datum 2020-11-17
- Functies

### <a name="summary"></a>Samenvatting

Micro soft introduceert de API-beperking tot partners die partner Center-Api's aanroepen voor een meer consistente prestaties binnen een bepaalde periode.

### <a name="impacted-audience"></a>Doel groep

Partners die communiceren via het Cloud Solution Provider-programma

### <a name="details"></a>Details

Micro soft implementeert de API-beperking in Q1 2021 om een meer consistente prestaties te bieden binnen een tijds spanne voor partners die de Api's van het partner centrum aanroepen. Met beperking wordt het aantal aanvragen voor een service binnen een bepaalde periode beperkt om te voor komen dat bronnen worden overmatigd. Wanneer een drempel waarde wordt overschreden, zal het partner centrum gedurende een bepaalde periode alle verdere aanvragen van die client kunnen beperken.  

### <a name="partner-benefits"></a>Voor delen van partner 

Het partner centrum is ontworpen om een groot aantal aanvragen af te handelen, maar als er veel aanvragen worden gedaan door een aantal partners, helpt het beperken van de optimale prestaties en betrouw baarheid van alle partners. Het zorgt voor minimale downtime. Door het grote aantal aanvragen te verminderen, kunnen we ervoor zorgen dat de prestaties van alle partners consistent zijn. 


### <a name="apis-to-be-throttled"></a>Api's die moeten worden beperkt

|**Bewerking**|**Documentatie voor Partnercentrum**|
|-------------------------|----------------------------------|
|{baseURL}/v1/Customers/{customer_id}/Subscriptions|[Alle abonnementen van een klant ophalen](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}|[Een abonnement op de ID ophalen](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/Customers/{customer_id}/orders||[Alle bestellingen van een klant ophalen](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/Customers/{customer_id}/orders/{order_id}|[Een order op basis van ID ophalen](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/Customers/{customer_id}/orders/{order_id}/provisioningstatus|[De inrichtings status van het abonnement ophalen](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}|[Orders beheren en een abonnement beheren](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/addons|[Een lijst met invoeg toepassingen voor een abonnement ophalen](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/azureEntitlements|[Een lijst met Azure-rechten voor een abonnement ophalen](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/Customers/{customer_id}/Subscriptions/{subscription_id}/registrationstatus|[Registratie status van abonnement ophalen](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/customers/{customer-tenant-id}/transfers|[Alle overdrachten van een klant ophalen](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{upgrade-id}/status|[Upgrade status van product ophalen](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions|[Een lijst met aanbiedingen voor proef conversie ophalen](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

Deze aankondiging is erop gericht partners te voorzien van vroegtijdige kennis van de komende wijzigingen, waardoor ze kunnen voorbereiden. We raden u ten zeerste aan om partners vertrouwd te raken met deze Api's en overweeg de API voor het activiteiten logboek te gebruiken voor meer efficiëntie en om te voor komen dat deze wordt beperkt. Raadpleeg de informatie in [API Throttle-richt lijnen](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance)voor meer informatie over deze functie. 

### <a name="next-steps"></a>Volgende stappen

Bekijk de [richt lijnen](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance)voor het beperken van de API en neem de nodige maat regelen. 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>409 fouten vanwege dubbele MCA-aanvragen

### <a name="categories"></a>Categorieën

- Datum 2020-11-16
- Functies

### <a name="context"></a>Context

- In februari moesten partners de micro soft-klant overeenkomst ondertekenen (MCuA). Dit was een migratie van de vorige Microsoft Cloud Agreement (MCA). 
- Als onderdeel van deze wijzigings partner werden de partners gevraagd om de overeenkomst type parameter op te geven, zoals [hier](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)wordt beschreven.

### <a name="what-happened-next"></a>Wat is er nu gebeurd:

- Niet alle partners hebben de parameter aanvraag opgenomen in de implementatie. Micro soft heeft de MCA naar deze partners geretourneerd.
- De partner verzendt de handtekening aanvraag vervolgens opnieuw naar de klant en stuurt de MCA naar micro soft. 
- De duplicatie heeft invloed op de mogelijkheid van micro soft om service te bieden aan partners.
- In september 2020 hebben we een melding verzonden naar partners via Yammer in meerdere forums, waardoor de para meter wordt door gegeven aan partners. Micro soft kan de dubbele waarden niet meer accepteren en er worden 409-fouten weer gegeven.

>[Opmerking] Dit is geen nieuwe contract-en API-wijziging voor partners.

- In oktober hebben we nauw samengewerkt met partners die de meeste dubbele aanvragen hadden om het probleem op te lossen.
- Op dit moment wordt aan partners geadviseerd en worden er persoonlijke e-mail berichten verzonden naar de tien misleidende partijen, om hun aanvragen te beoordelen en aan ons te vragen, zodat we het probleem kunnen helpen testen en oplossen.
- Op 10 november 2020 hebben we het accepteren van duplicaten gestopt, en partners die de para meters niet hebben gecorrigeerd, heeft 409 fouten aangetroffen.
- Nadat de wijziging is teruggedraaid, worden er geen dubbele items geaccepteerd. 
- Op 14 januari 2021 worden er echter geen dubbele items meer geaccepteerd. Op deze manier kunnen partners meer tijd aanpassingen aan hun einde aanbrengen. We hebben al een melding ontvangen van een partner dat ze een update willen implementeren op 11/16 waarop we nauw met hen kunnen werken.
- Wij vragen u om de partners te helpen bij het testen door hun tenants toe te voegen aan een vlucht met de wijzigingen zodat de update van de oplossing naar verwachting werkt.



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>Testen beschikbaar: verbeteringen in het partner centrum-API en de gebruikers interface (UI) voor het onderwijs klant validatie proces

### <a name="categories"></a>Categorieën

- Datum 2020-11-10
- Mogelijkheden | Efficiëntie van schijf & schalen

### <a name="impacted-audience"></a>Doel groep

Partners die academische aanbiedingen verkopen via het programma Cloud Solution Provider (CSP).

### <a name="summary"></a>Samenvatting

Testen is nu beschikbaar voor partner centrum API-updates en UI-uitbrei dingen voor het trainings proces van het onderwijs klant.

### <a name="details"></a>Details

Micro soft werkt op vertrouwen. We streven ernaar een compatibele, veilige en veilige methode voor klant validatie te bieden voor het handelen van studie aanbiedingen in het CSP-programma. Als onderdeel hiervan introduceren we de API van partner Center en de verbeteringen van de gebruikers interface in het tweede kwar taal van dit boek jaar (FY21 Q2). Deze uitbrei dingen zullen duidelijkheid en zicht baarheid toevoegen aan het validatie proces van de klant, evenals de mogelijkheid om nauw keurige gegevens in te voeren, waardoor de klant validatie is voltooid.

**Verbeteringen in het partner centrum**

- Nieuwe Api's voor het ophalen en plaatsen van kwalificaties om nauw keurige gegevens invoer te ondersteunen en het validatie proces van het onderwijs klant door micro soft te verbeteren.

- UI-verbeteringen ter ondersteuning van nauw keurige gegevens invoer en verbeteren het validatie proces van het onderwijs klant door micro soft.

Testen.

Om een beter inzicht te krijgen in de Api's en gegevens invoer die vereist zijn voor een succes volle klant validatie, kunnen partners deze verbeteringen vanaf oktober 2020 testen. We geven binnenkort meer informatie over de exacte timing en hoe ze kunnen deel nemen. De bestaande partner Center-Api's worden vóór het einde van FY21 Q2 afgetrokken. Op dat moment moet u overstappen op de nieuwe partner centrum-Api's.

   - Testen van de beschik bare partner test datums van 1 oktober tot 2 december 2020. Partners die willen deel nemen, moeten de test handleiding voor het onderwijs van de klanten van het partner centrum downloaden voor het voorbereiden, registreren en wat ze kunnen verwachten tijdens de test fase.

**Library-en Museum-klanten**

Naast deze verbeteringen, zijn we enthousiast om dat in FY21 Q2 aan te kondigen, kunnen we prijzen voor het onderwijs van bibliotheken en Museum inschakelen, waardoor de Education-klanten met wie u de CSP-aanbiedingen kunt maken, worden uitgebreid.

Micro soft behoudt zich het recht voor om de status van een klant of voorgestelde klant als een bevoegd onderwijs gebruiker te controleren. Raadpleeg de [gebruikers vereisten](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7) voor het onderwijs recht op het onderwijs voor volledige informatie.

## <a name="next-steps"></a>Volgende stappen

Bekijk de nieuwe gebruikers interface-en API-wijzigingen van het partner centrum en de test handleiding in het trainings proces voor de verbetering van de inhouds validatie van het IT- [partner centrum](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

• Meld u aan om te kunnen deel nemen aan testen. (Zie de [test handleiding](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) voor meer informatie.) 

• Zorg ervoor dat uw organisatie vertrouwd is met de [gebruikers vereisten voor het onderwijs](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)recht op het onderwijs. 

• Deel deze informatie met de juiste teams binnen uw organisatie, samen met uw wederverkopers om hen te helpen deze wijzigingen voor te bereiden.



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>Inhoud van commerciële licentie partners uitbreiden in de galerie met Operations Readiness

### <a name="categories"></a>Categorieën

- Datum: 2020-11-5
- Functies

### <a name="summary"></a>Samenvatting

Vanaf november 5 2020 wordt de inhoud van de commerciële licentie partner van partner University ook beschikbaar gesteld in de galerie met Operations Readiness.

### <a name="impacted-audience"></a>Doel groep

Commerciële partners

### <a name="details"></a>Details

Vanaf 5 november 2020 wordt de inhoud van de commerciële licentie partner van partner University ook beschikbaar gesteld in de galerie met Operations Readiness. Dit consolideert de bestaande operationele en commerciële licentie partner om inhoud te starten in de galerie met Operations Readiness met onze bedoelende commerciële licentie partner-inhoud van partner University. Zo beschikt u met partners over een naadloze ervaring voor de gereedheid. De volgende verzamelingen zijn toegevoegd aan de galerie met Operations Readiness:

- [Microsoft Azure-aanbiedingen en licenties](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [Commerciële licentie verlening: CSP-Spotlight-oproep](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [Commerciële licentie verlening-oproep voor licentie-updates](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie met alle relevante contact personen in uw organisatie.

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5"></a>Micro soft teams kamers Premium SKU starten

### <a name="categories"></a>Categorieën

- Datum: 2020-11-3
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

Micro soft teams kamers Premium SKU voor micro soft teams via het programma Cloud Solution Provider (CSP) is nu beschikbaar.

### <a name="impacted-audience"></a>Doel groep

Alle partners communiceren via het CSP-programma (Cloud Solution Provider)

### <a name="details"></a>Details

De nieuwe micro soft teams-kamers Premium SKU voor micro soft teams-kamers is nu beschikbaar voor klanten die een CSP aanschaffen via USD50 per apparaat per product. De micro soft teams kamers Premium SKU is een alternatief voor de standaard-SKU van micro soft teams-kamers (voorheen een licentie voor Vergader ruimte genoemd). Deze SKU bevat alles in de standaard aanbieding, zoals de vereiste licenties voor micro soft teams, Skype voor bedrijven online en intune-beheer. De aanbieding biedt ook telefoon systeem, dat nodig is voor de integratie van open bare telefoonnet werk (openbaar geschakelde telefonie) en audio vergaderingen, indien beschikbaar. 

Met de Premium-aanbieding hebben klanten toegang tot de nieuw gepubliceerde micro soft teams-kamers beheerde services, waar experts het beheer en de activiteiten voor Vergader ruimten namens de klant afhandelen. Met deze Cloud service voor IT-beheer en-bewaking blijven de apparaten van micro soft teams en hun rand apparatuur up-to-date en beveiligd. Ze zijn ook proactief bewaakt en beheerd, en onderhouden een omgeving die is geoptimaliseerd voor een goede ervaring in de kamer.

#### <a name="released-at-launch"></a>Vrijgegeven bij het starten

   |****|**Micro soft teams kamers Standard USD15-apparaat per maand**|**Micro soft teams kamers Premium USD50-apparaat per maand**|
   |-------------------|:------|:------|
   |Skype voor Bedrijven|Ja| |
   |Microsoft Teams|Ja|Ja|
   |Telefoon systeem|Ja|Ja|
   |Audio vergaderingen|Ja|Ja|
   |Microsoft Intune|Ja|Ja|
   | |Micro soft teams-kamers standaard USD15 per apparaat per maand|Micro soft teams kamers Premium USD50 per apparaat per maand|
   |Beheerde services van micro soft teams-kamers| |Ja|
   |Wereld wijde Beschik baarheid|Ja|In geselecteerde markten|

#### <a name="microsoft-teams-rooms-managed-services"></a>Beheerde services van micro soft teams-kamers

- Proactieve beheer: zakelijke (24x7x365 beheer van uw room-systemen, waaronder patches, configuratie beheer en meer.
• Realtime controle en analyse van de hoofd oorzaak: bewaking en detectie met door micro soft gecooerdineerde incident beheer reacties, in combi natie met de klant, indien nodig. Met de mobiele app kunt u op de hoogte blijven van waarschuwingen.
- Beheerde updates: beheer en levering van toepassingen, Windows KB en firmware-updates.
- Beveiliging tegen beveiligings Risico's: beveiliging tegen beveiligings Risico's via micro soft Defender Advanced Threat Protection.
- Klanten ondersteuning: zakelijke (24x7x365-ticket ondersteuning via ons speciaal Service Operations Center met ondersteunings incidenten voor niet-geautomatiseerde aanvragen. Gedetailleerd toegangs beheer op basis van rollen.
- Inzichten en aanbevelingen: geaggregeerde inzichten in klanten en rapporten over de gezondheid van de kamer, de inventaris, het gebruik, online vergaderingen en de trends van het incident.

#### <a name="offer-details"></a>Details van aanbieding

   |**Naam van aanbieding**|**Aanbiedings-id**|**Materiaal-ID**|
   |-------------------|:------|:------|
   |Teams kamers Premium|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Teams kamers Premium (VS en CAN)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Teams kamers Premium voor faculteiten|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>Volgende stappen

- Bekijk de nieuwe aanbieding en de geografische Beschik baarheid daarvan de veelgestelde [vragen (FAQ)]().
- Vertrouwd raken met de nieuwe aanbieding en de geografische Beschik baarheid. 
- Meer informatie over micro soft-kamers en gerelateerde aanbiedingen in [micro soft-team kamers](https://rooms.microsoft.com/).
- Gebruik de [partner gids teams](https://aka.ms/teamscallingmeetingsguide) om uw prak tijken te ontwikkelen met teams in Vergader ruimten en maak een verkoop klare aanbieding.
- Raadpleeg de [Veelgestelde vragen over de micro soft teams-kamers](https://aka.ms/PartnerMTRFAQ) voor meer informatie over de product oplossing en-services. 
- Deel deze informatie met alle contact personen in uw organisatie en begrijp de verkoop kansen en cross-sell-mogelijkheden.

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>Nieuwe micro soft teams Advanced Communications-Sku's voor Government Community Cloud (GCC) binnenkort beschikbaar

### <a name="categories"></a>Categorieën

- Datum: 2020-11-2
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

De nieuwe SKU voor het toevoegen van geavanceerde communicatie voor micro soft teams in GCC is beschikbaar vanaf 1 december 2020.

### <a name="impacted-audience"></a>Doel groep

Alle partners communiceren via het CSP-programma (Cloud Solution Provider)

### <a name="details"></a>Details

De nieuwe geavanceerde invoeg toepassing voor communicatie voor micro soft teams in GCC is nu beschikbaar op USD12 per gebruiker per maand. De add-on Sku's kunnen worden aangeschaft op een andere Microsoft 365 suite die micro soft teams bevat. Geavanceerde communicatie biedt een nieuwe set mogelijkheden voor grote vergaderingen, communicatie beleid, integraties en geavanceerde hulpprogram ma's voor IT-beheer. 

#### <a name="offer-details"></a>Details van aanbieding

   |**Naam van aanbieding**|**Aanbiedings-id**|**Materiaal-ID**|
   |-------------------|:------|:------|
   |Geavanceerde communicatie voor GCC|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>Veelgestelde vragen 

**Wat is geavanceerde communicatie?** Met deze nieuwe invoeg toepassing voor micro soft-teams kunnen klanten hun communicatie-ervaring verder verbeteren. Het kan worden aangeschaft boven op elke Microsoft 365 SKU waarop ze zijn geabonneerd.

**Hoeveel kost het?** De commerciële ERP is USD12 per gebruiker per maand.

**Welke klanten kunnen de invoeg toepassing aanschaffen?** GCC-klanten kunnen de invoeg toepassing kopen.

**Hoe kan het worden gekocht?** De invoeg toepassing kan worden aangeschaft via Enterprise Agreement, Enterprise Agreement-abonnement, inschrijving voor onderwijs oplossingen, CSP of Web direct.

**Waar kan de verkoop worden verkocht?** Het kan worden verkocht in de Amerikaanse markt.

**Wat zijn de vereisten?** Alle Microsoft 365-of Office 365-pakketten die micro soft teams bevatten, kunnen deze invoeg toepassing bevatten.

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie met de relevante contact personen in uw organisatie en begrijp inzicht in de verkoop kansen voor verkopen en cross-selling. Raadpleeg de sectie resources van de [partner handleiding voor teams](https://aka.ms/teamscallingmeetingsguide).

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365: onlangs gelanceerde en aanstaande nieuwe aanbiedingen en producten

### <a name="categories"></a>Categorieën

- Datum: 2020-11-2
- Aanbiedingen/markten

### <a name="impacted-audience"></a>Doel groep

Directe providers, indirecte providers en indirecte wederverkopers

### <a name="details"></a>Details

#### <a name="new-offers"></a>Nieuwe aanbiedingen

Op 1 november 2020 heeft micro soft Dynamics 365-project bewerkingen uitgebracht en wordt Dynamics 365 project Service Automation (PSA) voor commerciële klanten verwijderd. Deze communicatie bevat aanvullende informatie over de toewijzing van het gebruik van de rechten van de oplossing van deze start en van de Inge sloten aanbiedingen van een nieuwe onafhankelijke software leverancier (ISV).

#### <a name="project-operations-isv-embed-offers"></a>Project bewerkingen ISV-invoeg aanbiedingen

Op 1 november 2020 heeft micro soft drie extra ingebouwde ISV-aanbiedingen van 36-maand voor Dynamics 365 uitgebracht voor project bewerkingen voor klanten van de Cloud Solution Provider (CSP). Zie het tabblad project bewerkingen in het [Dynamics CSP Offers-November 2020 Excel-document](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls) voor de SKU-gegevens.

#### <a name="project-operations-dual-use-rights-mapping"></a>Project bewerkingen Dual-Use Rights mapping

In de volgende tabel vindt u informatie over de on-premises toewijzing van Dynamics 365 dual use-rechten voor de project bewerkingen:

   |**Aanbieding voor D365-bewerkingen**|**D365 on-premises toewijzing van rechten voor twee gebruik**|
   |-------------------|:------|
   |Aanbieding voor D365-bewerkingen|D365 on-premises toewijzing van rechten voor twee gebruik|
   |D365-project bewerkingen|D365 for Operations, on-premises (AX-Server) met behulp van de Dyn365 project Operations SKU (109108477)|
   |D365-project bewerkingen bijvoegen|D365 for Operations, on-premises (AX-Server) met behulp van de Dyn365 project Operations SKU (109108477)|
   |D365 Finance with project Operations|D365 for Operations, on-premises (AX-Server) met behulp van de Dyn365 project Operations SKU (109108477)|
   |D365-Financiën zijn gekoppeld aan project bewerkingen|D365 for Operations, on-premises (AX-Server) met behulp van de Dyn365 project Operations SKU (109108477)|
   |D365 Unified Operations: activity with project Operations|D365 for Operations, on-premises (AX-Server) met behulp van de Dyn365 project Operations SKU (109108477)|

#### <a name="previously-announced"></a>Eerder aangekondigd

Op 1 november 2020 heeft micro soft de volgende nieuwe en bijgewerkte aanbiedingen en producten voor de Dynamics 365-en Power-platforms voor CSP uitgebracht:

- Dynamics 365 Customer Voice GEBRUIKERSABONNEMENTSLICENTIES 

Controleer het tabblad project bewerkingen in het [Excel-document van de Dynamics CSP Offers-November 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls) voor de details van de aanbiedings-id.

Meer informatie vindt u op de start pagina van micro soft Dynamics 365 Customer Voice.

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie met de relevante personen in uw organisatie.

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>Introductie van Microsoft 365 Businesse stem voor non-profit organisaties

### <a name="categories"></a>Categorieën

- Datum: 2020-11-2
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

Op 1 2020 november heeft micro soft nieuwe Sku's geïntroduceerd voor Microsoft 365 Businesse Voice voor non-profit organisaties.

### <a name="impacted-audience"></a>Doel groep

Directe providers, indirecte providers en indirecte wederverkopers

### <a name="details"></a>Details

Op 1 november 2020 heeft micro soft nieuwe Sku's voor zakelijke Voice geïntroduceerd. De volledige suite is beschikbaar in Canada, het Verenigd Konink rijk en de Verenigde Staten. Zakelijke stem zonder gespreks plan is beschikbaar in alle andere markten. 

Microsoft 365 Business Voice is een op de cloud gebaseerd telefoon systeem voor kleine en middel grote bedrijven die zijn ingebouwd in Office 365. Het toevoegen van een zakelijke stem aan het Office 365-abonnement van een klant levert een alles-in-één oplossing voor communicatie en samen werking met aanroepen, chatten en vergaderingen in één toepassing, micro soft teams.

Raadpleeg de prijs lijst voor prijs informatie.

Microsoft 365 Business stem kan worden toegevoegd aan de volgende abonnementen voor Maxi maal 300 gebruikers:

- Office 365: Business Essentials, Business Premium, a1, E1, a3 en E3
- Microsoft 365: Business, a3 en E3


### <a name="next-steps"></a>Volgende stappen

- Lees de informatie in de prijs lijst voor beeld en deel de gegevens met alle relevante contact personen in uw organisatie. 
- Bekijk alle gereedheids materialen in de resource galerie voor de Cloud Solution Provider-programma-updates: [introductie van Microsoft 365 Business stem voor kleine en middel grote bedrijven](https://partner.microsoft.com/resources/collection/m365-voice-smb#/). 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>De aanbieding van de Cloud Solution Provider (CSP) voor Microsoft 365 Business Voice is nu beschikbaar

### <a name="categories"></a>Categorieën

- Datum: 2020-11-2
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

Prijzen voor kortingen die beschikbaar zijn voor nieuwe abonnementen en verlengingen van Microsoft 365 Business stem met oproep plan en Microsoft 365 Business spraak zonder abonnement.

### <a name="impacted-audience"></a>Doel groep

Alle partners communiceren via het CSP-programma

### <a name="details"></a>Details

Met ingang van 1 november 2020 tot en met 30 april 2021, nieuwe en vernieuwings abonnementen van Microsoft 365 Business Voice met oproep plan en Microsoft 365 Business spraak zonder oproepings plan zijn de prijzen voor kortingen van toepassing. Microsoft 365 Business spraak met een gespreks plan is gedurende 12 maanden onderhevig aan een korting van 25 procent en Microsoft 365 Business stem zonder oproep plan wordt gedurende 12 maanden onderhevig aan een korting van 33 procent. 

#### <a name="offer-details"></a>Details van aanbieding

   |**Naam van aanbieding**|**Aanbiedings-id**|**Materiaal-ID**|
   |-------------------|:------|:------|
   |Aanbieding voor Microsoft 365 Business stem-acceptatie|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Aanbieding voor Microsoft 365 Business stem-acceptatie|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Aanbieding voor Microsoft 365 Business Voice (Verenigde Staten)|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Promotie van de acceptatie van het Microsoft 365 Business stem (zonder oproep)|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Promotie van de acceptatie van het Microsoft 365 Business stem (zonder oproep)|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Promotie van de acceptatie van het Microsoft 365 Business stem (zonder oproep)|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |Microsoft 365 Business stem (zonder abonnement) voor een promotie met Amerikaanse goed keuring|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

Deze aanbiedingen zijn van invloed op de volgende klanten:

- Net nieuwe klant tenants
- Bestaande tenants van klanten die geen actieve of recent geannuleerde abonnement hebben (binnen de laatste 30 dagen) bij een zakelijke Voice-of audio conferencing-licentie op CSP, Web direct of een ander micro soft-commercieel kanaal

#### <a name="additional-resources"></a>Aanvullende bronnen

- Ga naar de [pagina Microsoft 365 Business Voice-partner](https://www.microsoft.com/microsoft-365/partners/businessvoice) voor meer informatie over zakelijke Voice. 
- Meer informatie over deze promotie vindt u in de [Veelgestelde vragen](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo)over gerelateerde partners.

### <a name="next-steps"></a>Volgende stappen

- Raadpleeg deze vergadering en deel deze informatie met alle relevante contact personen in uw organisatie.
- Neem deze acties op in uw Microsoft 365 verkoop bewegingen.
- Bespreek de klanten over de waarde van het toevoegen van zakelijke stem aan teams. 

________________
