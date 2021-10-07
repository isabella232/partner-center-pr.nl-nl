---
title: Marges ontdekken - commerciële marketplace
ms.topic: how-to
ms.date: 10/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Ontdek hoe Cloud Solution Provider (CSP)-partners Partner Center marges kunnen ontdekken die zijn geconfigureerd door ISV's (Independent Software Vendors).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8d7b5f077b3ea3f98f87121634427842db0a0f03
ms.sourcegitcommit: 77737d8f986a1afb3d923c130936e2f73ce07879
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/07/2021
ms.locfileid: "129661366"
---
# <a name="discover-margins-configured-by-independent-software-vendors-isvs"></a>Marges ontdekken die zijn geconfigureerd door onafhankelijke softwareleveranciers (ISV's)

**Juiste rollen:** Globale | Factureringsbeheerders | Beheeragent | Verkoopagent | Helpdeskagent

Onafhankelijke softwareleveranciers (ISV's) bieden mogelijk margekortingen voor sommige aanbiedingen op de commerciële marketplace aan specifieke Cloud Solution Providers (CSP's). Deze marges stimuleren CSP's om deze aanbiedingen aan hun klanten te verkopen.

> [!NOTE]
> De functie kortingen voor ISV-naar-CSP-marges is momenteel beschikbaar als openbare **preview** terwijl we feedback blijven verzamelen en de ervaringen blijven verbeteren.

## <a name="notes-about-the-public-preview"></a>Opmerkingen over de openbare preview

Met de marges van ISV naar CSP kan de ISV gerichte kortingen maken op specifieke CSP's. Deze mogelijkheid is nu beschikbaar, maar in openbare preview. Dit betekent dat de functie volledig functioneel en bruikbaar is terwijl we de algehele CSP Marketplace-ervaringen blijven verbeteren. De functie wordt niet meer in preview gedeclareerd als we de partnerervaring verbeteren. Er zijn geen specifieke tijdlijnen hiervoor en CSP-partners kunnen de kortingsfunctie gewoon blijven gebruiken.

### <a name="public-preview-improvement-areas"></a>Gebieden voor verbetering van openbare preview

- Beschikbaarheid van AppSource-aanbiedingen: Sommige CSP Marketplace-aanbiedingen, voornamelijk AppSource-aanbiedingen, nemen meer tijd in de tijd om te integreren en beschikbaar te maken in de Partner Center. Sommige partners zijn mogelijk op zoek naar AppSource-aanbiedingen, maar moeten mogelijk wachten tot ze beschikbaar zijn. Naarmate de tijd vergaat, Partner Center team verbeteringen aanbrengen in de latentie tussen het moment waarop een ISV een aanbieding maakt en wanneer deze beschikbaar is.
- Marges worden momenteel gedefinieerd als percentagekortingen op een CSP Marketplace-product-SKU. In de toekomst zijn er streven om het prijspunt te integreren in toekomstige prijslijsten. Tot dit gebeurt, kunnen partners de product-SKU in de margelijst (en bijbehorende API's) koppelen aan de product-SKU's voor de marketplace-prijslijst om kostenbedragen te voorspellen.
- Sommige Marketplace-aanbiedingen met een proefversie ingeschakeld, niet gerelateerd aan margekortingen, worden in de marketplace-bladerervaring als **$.00-bedragen** aangeboden. Partners moeten zorgvuldig begrijpen dat deze proefversies aan het einde van hun termijn worden verlengd tot betaalde bedragen. 
- Exclusieve aanbiedingen zijn mogelijk beschikbaar voor partners. Deze staan momenteel niet in de marketplace-prijslijsten. Tot die tijd moeten partners de prijzen voor hen vinden met behulp van de marketplace-bladerervaring voor het product dat ze willen kopen.

## <a name="view-margins-in-partner-center"></a>Marges in de Partner Center

Een CSP kan marges weergeven die ISV's voor deze marges hebben geconfigureerd op de pagina marges:

> [!NOTE]
> Zie Getting around Partner Center voor meer informatie [over de werkruimte-interface.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Werkruimteweergave](#tab/workspaces-view)

1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard) selecteer de **tegel** Prijzen.

2. Selecteer **Marges.** Partners zien een lijst met Marketplace-aanbiedingen waar ISV's marges voor hebben geconfigureerd.

3. CSP-partners kunnen door de lijst  met beschikbare marges bladeren of de gegevens downloaden in een door komma's scheidingstekens.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Meld u Partner Center [dashboard aan](https://partner.microsoft.com/dashboard)en selecteer **CSP** in het navigatiemenu aan de linkerkant.

2. Selecteer **Verkopen,** gevolgd door **Marges**. Partners zien een lijst met Marketplace-aanbiedingen waar ISV's marges voor hebben geconfigureerd.

3. CSP-partners kunnen door de lijst  met beschikbare marges bladeren of de gegevens downloaden in een door komma's scheidingstekens.

* * *

## <a name="margins-overview"></a>Overzicht van marges

ISV's die relaties met CSP-partners tot stand hebben gebracht, willen mogelijk margekortingen bieden om de CSP-partner te stimuleren de aanbiedingen aan hun klanten te verkopen. In dergelijke gevallen onderhandelt de CSP-partner vaak over een marge met een ISV of kan de ISV een marge bieden zonder overleg met een CSP-partner. De ISV kan een marge bieden voor aanbiedingen op basis van licenties of op basis van verbruik. Op verbruik gebaseerde marges zijn alleen van toepassing op de ISV-producten, niet op Azure-verbruiksproducten waar het ISV-product mee kan werken.

## <a name="margins-and-pricing"></a>Marges en prijzen

De Partner Center marketplace bevat de oorspronkelijke CSP-prijzen voor aanbiedingen. Prijslijsten voor de CSP Marketplace worden gedeeld met alle partners en bevatten retailprijzen. Partners passen vervolgens de korting voor het margepercentage toe op de product-SKU die ze willen kopen om inzicht te krijgen in de uiteindelijke prijs van het item voordat ze het kopen. CSP-partners zien ook retailprijzen in het Prijzenblad van Azure via de Azure Portal (alleen voor producten op basis van verbruik). Ze zien ook details van de marge die naar hen is uitgebreid in dit prijzenblad. 

## <a name="purchasing-offers"></a>Aanbiedingen kopen

CSP-partners verkrijgen hun geconfigureerde marge door simpelweg de Marketplace-aanbieding in [Partner Center](https://partner.microsoft.com) te kopen of het product te implementeren vanuit de Microsoft [Azure Portal](https://portal.azure.com). De vertransactiesde partner ontvangt de margekorting zonder dat er nog een stap moet worden onderverded. Partners kunnen zich niet voor de marge uit- en uit- als de ISV deze heeft geconfigureerd voor de CSP. De korting wordt toegepast.

Marges zijn van toepassing op elke transactie die de partner uitvoert en van toepassing op een van hun klanten. De CSP-partner hoeft geen voorstel te accepteren en is niet verplicht om een ISV-aanbieding te transactiseren, maar als dit het geval is en ze een marge hebben, wordt deze automatisch toegepast. 

## <a name="margins-and-indirect-resellers"></a>Marges en indirecte resellers

Marges worden alleen beschikbaar gesteld aan partners die worden gefactureerd door Microsoft, partners zoals indirecte providers en partners voor directe factuur. Een ISV kan een marge niet rechtstreeks aan een indirecte reseller verstrekken, maar de indirecte provider kan besluiten om een marge door te geven aan de indirecte reseller. Indirecte providers kunnen ervoor kiezen om de marge door te geven aan hun indirecte reseller, maar dat is niet verplicht. 

## <a name="terms-and-billing"></a>Voorwaarden en facturering

Partners kunnen controleren of de marge is toegepast op aanbiedingen op basis van verbruik met behulp van de Azure Cost Management-functies in de Azure Portal. Partners kunnen controleren of de marge is toegepast op aanbiedingen op basis van licenties door hun afstemmingsbestand aan het einde van hun factureringscyclus te controleren.

Elke marge heeft een begin- en einddatum. De prijsvermindering op basis van de margekorting wordt toegepast op de termijn van de aankoop. Een partner kan dezelfde aanbieding na de periode opnieuw inkopen om een nieuwe termijn met marge te krijgen. Met verlengingen wordt de marge toegepast als de verlenging binnen de begin- en einddatum van de marge wordt toegepast. Einddatums voor een marge worden altijd uitgelijnd met het einde van de maand. 

## <a name="margins-for-metered-billing"></a>Marges voor facturering naar data

Sommige CSP-producten worden met facturering naar gebruik gebruikt. Als de CSP-partner seats verhoogt voor aanbiedingen met facturering naar gebruik, blijven de prijzen voor het op rechten gebaseerde gedeelte van de kosten de korting behouden tot het einde van de jaarlijkse abonnementsperiode, maar blijft de marge die wordt toegepast op de prijs voor de facturering naar gebruik niet behouden na de eindperiode van de marge. De tijdelijke oplossing hier is dat ISV's een nieuwe marge voor die CSP-partner maken tot het einde van de abonnementsperiode. 

## <a name="margins-notifications"></a>Meldingen over marges

Er wordt geen proactieve melding verzonden, tenzij de ISV via e-mail contact op neemt met de CSP en bevestigt dat de marge is uitgebreid. De CSP-partner kan alle beschikbare marges weergeven via het tabblad Marges in de Partner Center.   

### <a name="recon-files"></a>Bestanden opnieuw configureren

De **CSP-partner** vindt details van de marges die zijn uitgebreid in het reconbestand Terugkerende en eenmalige aankopen zodra deze zijn gegenereerd. Belangrijke gegevens in het reconbestand om marges uit te leggen:

- UnitPrice blijft volgens de prijs die is ingesteld door de ISV.  

- EffectiveUnitPrice toont de prijs nadat de marge is toegepast.  

- PriceAdjustmentDescription bevat details over hoeveel van een marge aan de CSP-partner is verstrekt. 

## <a name="discover-and-operationalize-margins-using-the-partner-center-apis"></a>Marges ontdekken en operationeel maken met behulp van Partner Center API's

Partners kunnen de gebruikersinterface Partner Center of API's gebruiken om beschikbare marges weer te geven of te exporteren.

### <a name="apis-to-retrieve-margins"></a>API's voor het ophalen van marges

Partners kunnen de gegevens operationeel maken door de onderstaande API's aan te roepen. Elk van deze API's retourneert een lijst met marges waar de partner toegang toe heeft, gedefinieerd door de ISV. Beide API's retourneren dezelfde gegevens.

- [Met Marges op halen](/partner-center/develop/get-margins) worden gegevens in API-resultaatindeling

- [Met Marges downloaden](/partner-center/develop/download-margins) worden gegevens in een door komma's scheidingstekens

### <a name="apis-to-discover-marketplace-offers"></a>API's voor het ontdekken van Marketplace-aanbiedingen

CSP-programmapartners kunnen ook API's gebruiken om een lijst met beschikbare marges te retourneren. In aanmerking komende aanbiedingen zijn alleen die SaaS ISV-aanbiedingen die beschikbaar zijn voor de partner om te verkopen via Partner Center marketplace. Partners kunnen een lijst met Marketplace SaaS-aanbiedingen krijgen door een lijst met [aanbiedingen voor een markt te verkrijgen.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

CSP-partners kunnen de Partner Center-API's gebruiken om de lijst met transacteerbare SaaS-aanbiedingen (Software-as-a-Service) op te halen en orders voor hun klanten in te dienen. Zie Een abonnement maken voor [commerciële marketplace-producten voor meer informatie.](/partner-center/develop/create-subscription-azure-marketplace-products)

CSP-partners kunnen de Azure Portal UX gebruiken om alle Marketplace-aanbiedingen weer te geven. Ze kunnen de volgende API's gebruiken om de lijst met marketplace-VM-aanbiedingen op te halen en orders voor hun klanten in te dienen.  
- [VM's: Een lijst met VM's met API's](/azure/virtual-machines/windows/cli-ps-findimage)
- [VM's: Aankoop-API's (CLI, PowerShell, ARM)](/azure/virtual-machines/linux/quick-create-cli) 

Er is geen filter in de Azure Portal voor aanbiedingen die zijn gekozen om te worden verkocht via CSP. Partners moeten de prijslijst bekijken om te begrijpen welke aanbiedingen via CSP kunnen worden getransacteerd. Er zijn momenteel geen Azure Portal beschikbaar voor het transacten van SaaS- of Managed Application Marketplace-aanbiedingen. 

Lees Overzicht van commerciële marketplace voor meer informatie over de CSP-ervaring in [de marketplace.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Volgende stappen

- [Overzicht van commerciële marketplace](csp-commercial-marketplace-overview.md)
- [Aanbiedingen voor commerciële marketplace kopen](csp-commercial-marketplace-purchase.md)
- [Handleiding voor CSP-incentive](https://aka.ms/partnerincentives)
