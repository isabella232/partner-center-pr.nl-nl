---
title: Aankondigingen van maart 2021
description: Aankondigingen van maart 2021 voor Microsoft Partner Center nieuwe mogelijkheden, promoties, aanbiedingen, markten of wijzigingen in bestaande aanbiedingen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328063"
---
# <a name="march-2021-announcements"></a>Aankondigingen van maart 2021

Deze pagina bevat de aankondigingen voor Microsoft Partner Center voor maart 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Gereedheid: wijzigingen in de validatie-API Cloud Solution Provider CSP-klantadres (CSP) worden in juni live uitgevoerd; testmogelijkheid nu beschikbaar

### <a name="categories"></a>Categorieën

- Datum: 2021-04-30
- Gereedheid

### <a name="summary"></a>Samenvatting

Om partners en klanten te helpen hun bedrijf te runnen op basis van vertrouwen, nodigen we partners uit om wijzigingen in de Adres-API valideren voor alle landen over de hele wereld te testen.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

CSP-partners voor directe factuur en indirecte providers die nieuwe klantadresgegevens maken of bijwerken.

### <a name="details"></a>Details

Microsoft wordt uitgevoerd op vertrouwen. We zetten ons in voor een compatibele, veilige en veilige methode voor validatie van klantadressen voor het uitvoeren van klantabonnementen in het CSP-programma. Vanaf 31 maart 2021 hebben we wijzigingen geïntroduceerd in de Adres-API valideren die we partners hebben uitgenodigd om te testen, voordat we live gaan met de wijzigingen in juni 2021.

Wijzigingen zijn alleen van invloed op de API Adres valideren. Api's voor klant- en update-factureringsprofiel maken worden niet beïnvloed.

Het antwoord retournt een van de volgende statusberichten:

| Status     | Beschrijving |    Aantal geretourneerde voorgestelde adressen |
|-------|---------------|-------------------|
|Geverifieerd verzendbaar | Het adres wordt geverifieerd en kan worden verzonden naar . | Enkelvoudig |
|Geverifieerd | Het adres wordt geverifieerd. | Enkelvoudig |
|Interactie vereist | Voorgesteld adres is aanzienlijk gewijzigd en moet worden bevestigd door de gebruiker. | Enkelvoudig |
|Gedeeltelijk straat | De opgegeven straat in het adres is gedeeltelijk en heeft meer informatie nodig. | Meerdere: maximaal drie |
|Gedeeltelijk locatie | De opgegeven locatie (gebouwnummer, suitenummer en andere) is gedeeltelijk en heeft meer informatie nodig. | Meerdere: maximaal drie |
|Meerdere | Er zijn meerdere velden die gedeeltelijk in het adres zijn (mogelijk ook gedeeltelijk en gedeeltelijk van de straat). | Meerdere: maximaal drie |
|Geen | Het adres is onjuist. | Geen |
|Niet gevalideerd | Het adres kan niet worden verzonden via het validatieproces. | Geen |

Amerikaanse postcodes retourneren 4 extra cijfers + koppeltekens, bijvoorbeeld 12345-6789.

Zodra een adres is verzonden voor validatie via de Validatieadres-API, wordt het volgende antwoordschema geretourneerd:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Bekijk dit voorbeeld van een antwoord. Houd er rekening mee dat voor de VS het antwoord een extra achtervoegsel van vier cijfers voor de postcode retourneert als u slechts vijf cijfers voor de postcode op geeft.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Volgende stappen

- Deel uw tenant-id voor de sandbox met de expert op het gebied van onderwerp (Ali Kunnenki) die moet worden opgenomen in de test flight, zodat u kunt beginnen met het voorbereiden van de update.

- Als u een CPV-oplossing (Panel Vendor) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Als u ondersteuning nodig hebt voor uw bewerkingen met Microsoft, kunt u contact op met de Yammer-groep voor ondersteuning van uw partner.

### <a name="change-log"></a>Wijzigingslogboek:

- 31 maart 2020: Oorspronkelijke publicatie

- 30 april 2021: Updates voor voorbeeldreactie en postcodedetails

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Nieuwe EAC-ervaring (Exchange-beheercentrum)

### <a name="categories"></a>Categorieën

- Datum: 2021-03-29
- Functies

### <a name="summary"></a>Samenvatting

Vanaf 27 april 2021 zal het Exchange-beheercentrum (EAC) een nieuwe ervaring uitrollen die de dagelijkse efficiëntie voor gebruikers verbetert.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Gedelegeerde beheerders die toegang hebben tot Exchange via Partner Center

### <a name="details"></a>Details

Vanaf 27 april 2021 worden partners die naar Exchange navigeren via Partner Center omgeleid naar de nieuwe EAC.

Deze nieuwe ervaring is momenteel beschikbaar als preview-versie en beheerders kunnen deze ervaring activeren door de schakelknop in de rechterbovenhoek in de klassieke EAC te selecteren. Ze kunnen ook naar de nieuwe EAC navigeren door de banner Nu proberen te selecteren die op alle pagina's wordt weergegeven.

Voordelen van de nieuwe EAC zijn onder andere:

- Er zijn inzichten, rapporten en waarschuwingsmechanismen toegevoegd voor e-mailstroomgerelateerde problemen. 

- Gepersonaliseerde dashboards om de productiviteit te verhogen.

Video's zijn beschikbaar in de sectie Training & guide over de nieuwe EAC-ervaring om **u** te helpen door de nieuwe ervaring te navigeren. Deze geven u een overzicht van hoe u de nieuwe portal het beste kunt gebruiken.

>[!NOTE]
>Met deze wijziging wordt de klassieke EAC-ervaring niet afgeschaft. U wordt ruim van tevoren op de hoogte gesteld voordat een wijziging wordt geïmplementeerd.

### <a name="next-steps"></a>Volgende stappen

- Bekijk de [bronnen over dit onderwerp,](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/)waar u schermopnamen van de nieuwe ervaring kunt bekijken.

- Deel deze informatie met de juiste belanghebbenden in uw organisatie. 

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze wijzigingen.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Introductie van de kalender voor productlancering

### <a name="categories"></a>Categorieën

- Datum: 2021-03-25
- Aanbiedingen | Moderne werkplek

### <a name="summary"></a>Samenvatting

In reactie op feedback van partners stroomlijnt Microsoft Operations de communicatie voor productlanceringen.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Cloud Solution Provider (CSP)-partners

### <a name="details"></a>Details

Microsoft streeft ernaar partnerervaringen voortdurend te verbeteren. We hebben van u feedback gekregen dat u te veel berichten van Microsoft hebt ontvangen, waaronder dubbele aankondigingen voor productlanceringen.

In reactie op uw feedback heeft Microsoft de gereedheidservaring voor productlanceringen voor nieuwe en bestaande aanbiedingen gestroomlijnd.

We bieden u nu één maandelijkse weergave van productlanceringen, gepubliceerd in de resourcegalerie Operations-gereedheid. Deze kalenderweergave [voor maandelijkse productlancering](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) vervangt afzonderlijke communicatie over productlancering in de resourcegalerie Operations-gereedheid en in Partner Center aankondigingen.

U kunt deze productlancering [ook openen vanuit](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [communityverzamelingen,](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) [agendaweergaven](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)en [CSP-nieuwsbrieven.](https://partner.microsoft.com/resources/collection/csp-monthly-update#/) We stellen u op de hoogte wanneer we elke maand de kalender voor productlancering publiceren met een aankondiging in de resourcegalerie Voor Operations-gereedheid.

U kunt nog steeds informatie over nieuwe en bestaande aanbiedingen vinden in de logboeken prijzenlijstvoorbeeld en prijslijstwijziging, evenals in productblogs, licentiehandleidingen en productmarketingpagina's.

De wijziging is van toepassing op lanceringen voor de volgende producten:

- Dynamics on-premises
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- Hulpprogramma's
- Teams en Telco

We blijven specifieke aankondigingen verzenden voor productlanceringen waarvoor details over operations-gereedheid zijn vereist.

### <a name="next-steps"></a>Volgende stappen

Lees de bronnen over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor meer vragen over deze aanbiedingen.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Wijzigingen in onboardingvereisten voor CSP-klanten

### <a name="categories"></a>Categorieën

- Datum: 2021-03-25
- Functies

### <a name="summary"></a>Samenvatting

Als onderdeel van onze toezegging om partners en klanten te helpen hun bedrijf te runnen op basis van een vertrouwensrelatie, vragen we aanvullende klantgegevens aan, met ingang van 25 maart 2021.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Cloud Solution Provider (CSP) directe factuurpartners en indirecte providers die nieuwe of bestaande klanten hebben in de landen die in de volgende sectie worden vermeld

### <a name="details"></a>Details

Microsoft wordt uitgevoerd op vertrouwen. We zetten ons in voor een compatibele, veilige en veilige methode voor klantvalidatie voor het transacteren van klantabonnementen in het CSP-programma. Op 25 maart 2021 introduceren we verbeteringen van Partner Center API en gebruikersinterface (UI) die van invloed zijn op partners die aan beide van de volgende criteria voldoen:

1. De partner heeft een directe factureringsrelatie met Microsoft (wat betekent dat de partner een directe factureringspartner of een indirecte provider is).

2. De partner doet zaken met nieuwe of bestaande klanten in de volgende landen:

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

Partners die aan de criteria voldoen, moeten de bedrijfsregistratie-id **(ook** wel **inN** van de organisatie van de klant genoemd) en het telefoonnummer van een klant indienen wanneer ze nieuwe klanten onboarden of bestaande klantgegevens wijzigen.  Deze partners kunnen ook een optionele **middelste naam** voor de klant invoeren.

Houd er rekening mee dat wanneer u uw bedrijfsregistratie-id toevoegt, u uw zakelijke btw-id moet gebruiken en niet de persoonlijke id van de klant.

Partners die zaken doen met nieuwe of bestaande klanten in de volgende landen, hebben al een eerdere release in november 2020 in gebruik.

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

Partners met klanten in de rest van de wereld kunnen op 25 maart 2021 de  bedrijfsregistratie-id, het telefoonnummer en de middelste naam voor klanten invoeren als optionele details.  

### <a name="next-steps"></a>Volgende stappen

- Bekijk de technische documentatie en veelgestelde vragen in de [speciale partnerverzameling](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) voor meer gedetailleerde richtlijnen.

- Bereid u voor op het opnemen van de wijzigingen met behulp Partner Center API en webgebruikerservaring. API/SDK's zijn beschikbaar om te testen.

- Zorg ervoor dat u de aanvullende gegevens indient bij het onboarden van nieuwe klanten of het wijzigen van bestaande klantgegevens.

- Als u een CPV-oplossing (Panel Vendor) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Neem contact op met uw belastingadviseur of lokale belasting kantoor als u vragen hebt met betrekking tot de juridische id (ook wel INN of TIN genoemd). Microsoft kan geen richtlijnen geven over belastingzaken.

Als u ondersteuning nodig hebt bij uw bewerkingen met Microsoft, [opent u een serviceaanvraag.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8)

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correcties aangebracht in de prijslijst met doorlopende software van 1 maart 2021

### <a name="categories"></a>Categorieën

- Datum: 2021-03-23
- Aanbiedingen/markten

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Indirecte providers en directe factuurpartners die permanente software in het Cloud Solution Provider gebruiken 

### <a name="details"></a>Details

De prijslijst voor permanente software die op 1 maart 2021 werd gepost, bevatte markten die daar niet hadden mogen zijn. De prijslijst voor permanente software is bijgewerkt op 17 maart 2021 met de correcties. Deze correcties zijn alleen van toepassing op:

- Product-id: DF77X4D43RKT 
- Productnaam: Windows 10 Home pro-upgrade voor Microsoft 365 Business
- Verwijderde of niet-ondersteunde markten: AE, AF, AL, AM, AO, BA, BB, BD, WAS, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, JR, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Deze wijzigingen zijn alleen van toepassing op het bovenstaande product. Andere producten hadden geen correcties. 

### <a name="next-steps-and-resources"></a>Volgende stappen en resources

- Partners die permanente software gebruiken, moeten de meest recente lijst met doorlopende softwareprijzen downloaden.
- Raadpleeg de [landcodes van](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) de regio voor een vriendelijke toewijzing van de afkorting van twee letters aan landen.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-release op .NET Standard (v1.17.0)

### <a name="categories"></a>Categorieën

- Datum: 2021-03-23

- Functies
 
### <a name="impacted-audience"></a>Beïnvloede doelgroep

Directe factuurpartners en indirecte providers die deelnemen aan het CSP-programma dat de .NET-SDK Partner Center gebruiken.

### <a name="details"></a>Details

Vanaf 23 maart 2020 kunnen partners beginnen met het downloaden van de versie van [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), samen met bijgewerkte openbare Partnercentrum-SDK [GitHub-voorbeelden.](https://github.com/Microsoft/Partner-Center-DotNet-Samples) Deze versie bevat updates voor de volgende methoden:

#### <a name="audit-updated-new-operation-types"></a>Controle bijgewerkt: nieuwe bewerkingstypen

Nieuwe [bewerkingstypen toegevoegd om](https://docs.microsoft.com/partner-center/develop/auditing-resources) te weten wanneer de klant DAP heeft goedgekeurd en beëindigd.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Controle bijgewerkt: Nieuwe resource- en bewerkingstypen

Er zijn nieuwe [resource- en bewerkingstypen toegevoegd](https://docs.microsoft.com/partner-center/develop/auditing-resources) voor de ondersteuning van het scenario van de klantdirectory-rol.

- Nieuw resourcetype CustomerDirectoryRole

- Bewerkingstypen 'AddUserMember' en 'RemoveUserMember'

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-updates voor klantaccounts

- Ondersteuning voor GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/kwalificaties

- POST /customers/{customer_id}/kwalificaties?code={validationCode}

#### <a name="additional-changes"></a>Aanvullende wijzigingen

De volgende wijzigingen worden geïntroduceerd als onderdeel van New Commerce en zijn momenteel alleen beschikbaar via uitnodiging voor partners die deel uitmaken van de technische preview van de M365/D365 New Commerce-ervaring. Partners die geen deel uitmaken van de technical preview van New Commerce, mogen geen gevolgen merken en moeten achterwaarts compatibel zijn.

- Cataloguswijzigingen:

  - GET /products/{product-id}/skus/{sku-id}

- Kopen en beheren:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Volgende stappen

- Download de nieuwste versie [van MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- De [GitHub-voorbeelden downloaden en bekijken](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Aanbieding voor commerciële CSP-marketplace en FY21 CSP-incentives voor in aanmerking komende aanbiedingen

### <a name="categories"></a>Categorieën

- Datum: 2021-03-18
- Functies

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Indirecte providers en directe factuurpartners in het Cloud Solution Provider programma 

### <a name="details"></a>Details

Indirecte providers en directe factuurpartners in het Cloud Solution Provider-programma kunnen aanbiedingen van derden verkopen en een grote incentive verdienen voor elke in aanmerking komende aanbieding van derden die in Partner Center of de Azure Portal. De incentive heeft de vorm van een auto op gefactureerde verkoop voor de in aanmerking komende aanbiedingen en is beschikbaar tot en met **30 juni 2021.**  

Blijf hieronder meer te weten over deze commerciële marketplace-aanbieding voor CSP en neem vandaag nog contact op met uw klanten om de juiste aanbiedingen te identificeren om hun succes en digitale transformatie mogelijk te maken.

We werken samen met Onafhankelijke softwareleveranciers (ISV's) om de nieuwste IaaS- en SaaS-oplossingen op de markt te brengen voor Microsoft-klanten. ISV-uitgevers kunnen de verkoop van hun aanbiedingen via het Microsoft-partnerkanaal inschakelen. Onze aanbiedingen die in aanmerking komen voor een incentive kunnen worden onderverdeeld in twee categorieën:

- Selecteer SaaS- en IaaS-aanbiedingen van derden met een azure IP-gecentraliseerde status voor co-verkoop. 

- SaaS-toepassingen die zijn geïntegreerd met Teams of ten minste twee Microsoft 365 productiviteits-apps, zoals PowerPoint, Word, Excel, Outlook of SharePoint.

### <a name="next-steps-and-resources"></a>Volgende stappen en resources

- Meer informatie over het verdienen [van Partner Incentives voor](https://partner.microsoft.com/membership/partner-incentives) het verkopen van in aanmerking komende Marketplace-apps aan apps die in aanmerking komen voor incentives. Nieuwe aanbiedingen worden maandelijks toegevoegd.  
- [Cloud Solution Provider directe factuur voor incentive-resources van partners](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Cloud Solution Provider indirect provider incentive resources](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Bekijk deze [presentatie voor](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) meer informatie over het verkopen van de commerciële marketplace-apps. Bekijk hier aanvullende [bronnen.](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) 
- De catalogus met commerciële marketplaces verkennen in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) of [Azure Portal](https://ms.portal.azure.com/#home)
- [API's gebruiken](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) om apps te integreren in de marketplace van uw bedrijf
- Contact op met ISV's met wie u geïnteresseerd bent om zaken te doen
- Indirecte providers moeten integreren met behulp van API's en resellers begeleiden over welke apps moeten worden verkocht

### <a name="questions"></a>Vragen?  

Raadpleeg dit [artikel voor](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) een overzicht van de commerciële marketplace in Partner Center.

Als u aanvullende hulp nodig hebt, kunt u een ondersteuningsaanvraag maken in Partner Center. Meer informatie op [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Power BI Premium naamgeving van aanbieding en vereiste update

### <a name="categories"></a>Categorieën

- Datum: 2021-03-18
- Functies

### <a name="summary"></a>Samenvatting

De lijst met definitieve prijzen van 1 april 2021 wordt bijgewerkt om duidelijkheid te geven over de naamgevings- en/of vereiste informatie voor de Power BI Premium per gebruiker.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Cloud Solution Provider directe en indirecte partners (CSP)

### <a name="details"></a>Details

De definitieve prijslijst van 1 april 2021 wordt bijgewerkt om de naamgevings- en/of vereiste informatie voor de Power BI Premium per gebruiker toe te voegen.

Totdat de uiteindelijke prijslijst is bijgewerkt, gebruikt u de informatie in deze sectie om ervoor te zorgen dat het juiste product is besteld.

In de volgende details worden de betrokken SKU en de vereiste details bewaarde.

| Weergavenaam van aanbieding in de preview-versie van de prijslijst van 1 maart |  Weergavenaam van aanbieding bijgewerkt op definitieve prijslijst van 1 april| Aanbiedings-id |
| ------ | ----------- | ----------- |
| Power BI Premium per Add-On (non-profit personeel prijzen)  |  Power BI Premium per gebruiker Add-On **(Office)** (non-profit personeel prijzen)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Klanten moeten een van de volgende vereisten hebben om deze aanbieding te kopen:

| Weergavenaam van aanbieding | Aanbiedings-id |
| ------ | ----------- |
| Microsoft 365 E5 (non-profit personeel prijzen)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 zonder audiovergaderingen (non-profit personeel prijzen)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (non-profit personeel prijzen)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Proefversie van Office 365 E5 (non-profit personeel)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 zonder audiovergaderingen (non-profit personeel prijzen)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Voor de Power BI Premium aanbieding is een vereiste voor aankoop vereist:

| Weergavenaam van aanbieding | Aanbiedings-id |
| ------ | ----------- |
|   Power BI Premium per Add-On (non-profit personeel prijzen)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Klanten moeten deze vereiste hebben om deze aanbieding te kunnen kopen:

| Weergavenaam van aanbieding | Aanbiedings-id |
| ------ |----------|
| Power BI Pro (non-profit personeel prijzen)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.  

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Prijsupdates van maart voor Microsoft 365 F3

### <a name="categories"></a>Categorieën

- Datum: 2021-03-16
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

Onjuiste prijzen van maart 2021 zijn gecorrigeerd voor Microsoft 365 F3 British Pond (GBP) en Euro (EURO).

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners kopen Microsoft 365 F3 in GBPs of EURO tussen 1 maart en 17 maart 2021 via het programma Cloud Solution Provider (CSP).

### <a name="details"></a>Details

Microsoft heeft onjuiste prijzen voor de Microsoft 365 F3 opgelost. De onjuiste prijzen waren voor GBP en EUR en alleen voor aanbiedingen die zijn aangeschaft tussen 1 maart en 17 maart 2021. De beïnvloede aanbiedingen en valuta's worden hieronder vermeld. 

| Naam van aanbieding | Valuta | Aanbiedings-id | Materiaal-id |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (Nederland) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (commercieel) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
De prijslijsten voor de preview-versie van de licentiebasis van maart en april zijn bijgewerkt op 16 maart 17:00 pacific (standaardtijd).

### <a name="next-steps"></a>Volgende stappen

- Partners moeten de huidige prijslijsten op basis van licenties, zowel maart als de preview van april, opnieuw downloaden met deze prijscorrecties, indien van toepassing.  
- Microsoft neemt de komende weken via e-mail contact op met betrokken partners om hen te informeren over de volgende stappen met betrekking tot het corrigeren van betrokken transacties.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante CSP Yammer-community's voor meer vragen.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Werk de naam van een juridisch bedrijf bij via Partner Center

### <a name="categories"></a>Categorieën

- Datum: 2021-03-16
- Efficiëntie verhogen & schalen

### <a name="summary"></a>Samenvatting

Vanaf maart 2021 kunnen Microsoft Partner Network(MPN)-partners en indirecte Cloud Solution Provider-resellers (CSP) hun juridische bedrijfsnaam bijwerken via Partner Center.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

MPN-partners en indirecte CSP-resellers (niet van toepassing op CSP-partners voor directe factuur)

### <a name="details"></a>Details

Vanaf maart 2021 kunnen MPN-partners en indirecte CSP-resellers hun juridische bedrijfsnaam bijwerken via Partner Center op een compatibele, self-serve manier. Met deze nieuwe functie hoeven partners geen ondersteuningsticket meer in te dienen Partner Center hun bedrijfsnaam bij te werken. Dit bespaart partners een aanzienlijke hoeveelheid tijd bij het uitvoeren van deze activiteiten. 

Zie Uw juridische bedrijfsprofiel bijwerken [voor meer informatie.](../update-your-partner-profile.md#update-your-legal-business-profile)

>[!NOTE]
>Zorg ervoor dat de bedrijfsnaam in uw juridische bedrijfsprofiel vrij is van spelfouten en afkortingen en exact overeenkomt met uw formele zakelijke registratierecords. Raadpleeg Uw organisatieprofiel verifiëren voor meer informatie over het bijwerken [van uw organisatieprofiel.](../update-your-partner-profile.md#update-your-legal-business-profile)

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie binnen uw organisatie, zodat het juiste team de processen kan controleren en bijwerken.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante CSP Yammer-community's voor meer vragen.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Bijwerken naar Cloud Solution Provider programma-ontwikkeling (CSP) en wijzigingen in open licentieprogramma's

### <a name="categories"></a>Categorieën

- Datum: 2021-03-15
- Functies

### <a name="summary"></a>Samenvatting

Er komen nieuwe doorlopende softwareaanbiedingen voor commerciële en openbare sectoren naar het Cloud Solution Provider-programma (CSP), samen met wijzigingen in het Open Licensing-programma.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Commerciële distributeurs en beheerde resellers die verkopen via het Open License-programma, evenals alle CSP-partners die permanente software verkopen

### <a name="details"></a>Details

In september 2020 heeft [Microsoft](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) een reeks stappen aangekondigd in ons digitale transformatietraject om de mogelijkheden voor partners in het CSP-programma uit te breiden, waaronder de beschikbaarheid van on-premises software voor partners. Dankzij deze wijzigingen kunnen partners hun bedrijf laten groeien en hun bereik uitbreiden door gebruik te maken van softwarelicenties in CSP en deze te positioneren voor succes in de cloud-first wereld van vandaag. Ze bieden ook mogelijkheden voor de overgangen van klanten naar de cloud en bieden partners de flexibiliteit die nodig is voor hybride cloudomgevingen van klanten.

In het vervolg van deze digitale transformatie kondigen we de volgende wijzigingen aan:

- 1 juli 2021: Er worden geen nieuwe SKU's, producten of promoties toegevoegd aan de prijslijst Open License-programma.

- 7 juli 2021: Twee commerciële aanbiedingen, Get Genuine Windows en Visual Studio Professional, en aanbiedingen voor openbare sectoren (overheid, onderwijs en non-profit – zie aankondiging [)](./2020-december.md#9)worden toegevoegd aan de prijslijst voor door CSP's voortgezette software.  De prijslijst vindt u in de sectie Software van de pagina [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) in Partner Center en wordt op deze datum opnieuw gepubliceerd.

Zie volgende stappen hieronder voor meer informatie over de wijzigingen in het CSP-programma en de wijzigingen in het Open **License-programma.**

### <a name="next-steps"></a>Volgende stappen

- Ontwikkeling van het CSP-programma: Bekijk de Software voor het doorlopende [programma in Cloud Solution Provider gereedheidsmateriaal](https://partner.microsoft.com/resources/collection/software-in-csp#/) voor het programma. Gebruik deze [gereedheidskaart om](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) snel de juiste informatie voor uw rol te vinden.

- Wijzigingen in het Open License-programma: Controleer de [ontwikkeling van het CSP-programma en het Open License-programma om](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) gereedheidsmaterialen te wijzigen. Gebruik deze [gereedheidskaart om](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) snel de juiste informatie voor uw rol te vinden.

### <a name="questions"></a>Vragen

Raadpleeg uw relevante CSP Yammer-community's voor meer vragen.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Update naar een eerdere aankondiging: Premium Assessments, een invoegaanvoeging voor Compliance Manager

### <a name="categories"></a>Categorieën

- Datum: 2021-03-15
- Uw bedrijf laten groeien

### <a name="summary"></a>Samenvatting

De proefaanbiedingen mogen niet worden vermeld in de prijslijst en worden verwijderd.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners die via een Cloud Solution Provider

### <a name="details"></a>Details

De proefaanbiedingen mogen niet zijn opgenomen in de prijslijst. Deze worden verwijderd uit de prijslijst van 1 mei 2021.

De oorspronkelijke aankondiging staat [hier.](./2021-february.md#4)

### <a name="additional-resources"></a>Aanvullende bronnen

- [Microsoft 365 E5-beveiliging en -naleving](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Evaluaties bouwen en beheren in Microsoft Compliance Manager - Microsoft 365 Compliance](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Volgende stappen

Lees de bronnen over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Uw oplossingen migreren van ONE Commercial Partner (OCP) go-to-market (GTM) naar de commerciële marketplace van Microsoft

### <a name="categories"></a>Categorieën

- Datum: 2021-03-12
- Functies

### <a name="summary"></a>Samenvatting

Vanaf 29 maart 2021 krijgt u te maken met beperkte MOGELIJKHEDEN van OCP (One Commercial Partner) voor go-to-market (GTM). We raden u aan om uw oplossingen te migreren naar de commerciële marketplace in Partner Center.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Organisaties die samen verkopen met oplossingen in OCP GTM

### <a name="details"></a>Details

In december 2020 zijn we begonnen met het traject van het Microsoft OCP GTM-hulpprogramma naar de commerciële marketplace van Microsoft in Partner Center. Deze overgang breidt de mogelijkheden van de commerciële marketplace uit, waar u uw oplossingen kunt presenteren aan miljoenen klanten, tweerichtingsmogelijkheden kunt delen met andere Microsoft- en partnerverkopers en gezamenlijk innovatieve oplossingen kunt verkopen.

De volgende mijlpaal in de overgang vindt plaats op 29 maart 2021. Op dat moment krijgt u te maken met beperkte OCP GTM-mogelijkheden, met een aantal velden die alleen-lezen worden. Als u momenteel samen met oplossingen in OCP GTM werkt, raden we u aan om uw oplossingen te migreren naar de commerciële marketplace om te profiteren van de mogelijkheden en uw publicatie-ervaring te vereenvoudigen. 

Als u overstapt op de commerciële marketplace Partner Center de primaire bestemming voor publicatie bij co-verkoop. Hier kunt u uw bedrijf blijven groeien door uw oplossingen te verbinden met onze gedeelde klanten via dezelfde kanalen en productervaringen die we voor Microsoft-producten gebruiken. [Meer informatie over de commerciële marketplace.](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/)

### <a name="next-steps"></a>Volgende stappen

- Als u uw oplossingen nog niet hebt verplaatst, volgt u [](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) de instructies in de overgangshandleiding of bekijkt u de stapsgewijs videozelfstudie om alle migratieactiviteiten te voltooien en te beginnen met het publiceren van uw oplossing(en) in de commerciële marketplace. [](/azure/marketplace/co-sell-solution-migration)

- Als u vragen hebt over de beperkte mogelijkheden in OCP GTM, bekijkt u de veelgestelde vragen over de commerciële marketplace van Microsoft om de vereisten voor [co-verkoop te bekijken.](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf) (Zie de sectie 'Beperkte mogelijkheden van OCP GTM vanaf 29 maart 2021.)

### <a name="questions"></a>Vragen?

Neem contact [op](https://partner.microsoft.com/support/?stage=1) met ondersteuning als u vragen hebt of meer informatie nodig hebt.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>De nieuwe commerce-ervaring in het Cloud Solution Provider (CSP)-programma voor Azure uitbreiden naar Rusland

### <a name="categories"></a>Categorieën

- Datum: 2021-03-10
- Functies

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle partners in Rusland die via het Cloud Solution Provider (CSP)-programma werken.

### <a name="details"></a>Details

Vanaf 10 maart 2021 kondigen we met trots de beschikbaarheid aan van de nieuwe **commerce-ervaring in CSP voor Azure in Rusland.** Deze ervaring stroomlijnt en verbetert de manier waarop klanten Azure-services kopen en gebruiken. Het biedt partners in het CSP-programma ook een consistente weergave van De prijzen van Azure voor verkoopmotie, prijzen voor USD voor wereldwijde consistentie, afstemming van factureringsdatums en toegang tot Azure Cost Management.

### <a name="next-steps"></a>Volgende stappen

Er zijn verschillende resources beschikbaar met de nieuwe Azure Commerce-ervaring en aanvullende informatie. U vindt de meest recente veelgestelde vragen, stapels, video en meer in de [resourcegalerie voor updates van het CSP-programma.](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/)

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Partner Center softwarelicentiesleutel en downloadafhandeling

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

De Partner Center downloaden van software en de uitvoering van licentiesleutels is hersteld.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle Cloud Solution Provider (CSP)-partners die softwareorders voor permanent gebruik en serverabonnementen uitvoeren via Partner Center

### <a name="details"></a>Details

In reactie op feedback van partners geven we opnieuw aan Partner Center om software- en licentiesleutels te verkrijgen voor permanente softwareorders en softwareorders voor serverabonnementen. Deze wordt hersteld naar de vorige staat voordat deze op 19 januari 2021 wordt verwijderd. (Zie de [aankondiging](2020-september.md#17).)

Houd er rekening mee dat softwarelicentiesleutels en downloadkoppelingen waardevolle en zeer aangevraagde intellectueel eigendomsactiva zijn. Als deze worden gelekt, kunnen ze snel worden verwijderd van hun activeringslimieten en een negatieve klant- en partnerervaring veroorzaken.

### <a name="next-steps"></a>Volgende stappen

Bekijk de volgende bronnen voor gebruiksinstructies en belangrijke richtlijnen voor de distributie van softwaresleutels:

- [On-premises software verkopen via het CSP-programma](../csp-on-premise-software.md)
- [Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Zie de sectie Guidance on Software Key Distribution(Richtlijnen voor distributie van **softwaresleutels))**

### <a name="questions"></a>Vragen?

Als u meer vragen over deze kennisgeving hebt, controleert u uw relevante Yammer-community's.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Uw deals migreren van Partner Sales Connect (PSC) naar Partner Center

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

Partner Sales Connect (PSC) gaat vanaf 31 maart 2021 over op alleen-lezentoegang. Daarom raden we u aan te beginnen met het migreren van uw deals van PSC naar Partner Center.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Partners met deals in PSC

### <a name="details"></a>Details

Als onderdeel van onze gedeelde toezegging voor groei is **co-verkoop** met Microsoft het pad voor u om te worden **ontdekt,** uw expertise te leveren en uw klantenvoetafdruk te vergroten voor positieve resultaten van klanten. Met een gemiddelde deal die **3,5** keer sneller is dan normaal, kunt u met het beheer van uw ervaring voor co-verkoop in Partner Center verkopen via de directe klant- en partner- en Microsoft-verkoperkanalen en uw volledige verwijzingspijplijn op één locatie beheren.

**PSC** wordt vanaf **31 maart 2021** overgeplaatst naar **alleen-lezentoegang.** Daarom raden we u aan om te beginnen met uw overstap naar Partner Center en toegang te krijgen tot deze verbeteringen: 

- **Nauwkeurigere routering** van de deals die u met Microsoft deelt naar de juiste verkoper, op basis van het type hulp dat u nodig hebt.
- **Maak vooraf een deal** met validatie van geschiktheid voor oplossingen die in aanmerking komen voor een incentive en om te voldoen aan de criteria van het ISV Connect-programma, wat het goedkeuringsproces en de definitieve POE-attestatie (Proof of Execution) vereenvoudigt.
- **Naadloze gebruikerservaring** voor het beheren van al uw kansen voor co-verkoop en gekwalificeerde verkoopkansen op één plek.

We hebben onlangs ook nieuwe functies toegevoegd aan Partner Center om u te helpen bij uw overstap:

- [Bulkbewerkingen voor kansen voor co-verkoop](../bulk-operations.md)
- [Functie voor dealmigratie](../psc-to-pc.md) (zie de sectie **Migratie van PSC-deals.)**

Met behulp van de ervaring voor co-verkoop in Partner Center hebben uw verkoopteams meer tijd om zich te richten op het stimuleren van leads en verkoopkansen, het sluiten van deals en het creëren van blijvende klantrelaties.

### <a name="next-steps"></a>Volgende stappen

Gebruik de Partner Center [om](../psc-to-pc.md) u te helpen bij het migreren van uw deals van PSC naar Partner Center.

### <a name="questions"></a>Vragen?

Neem contact op met ondersteuning voor verdere [vragen.](https://partner.microsoft.com/support/?stage=1)

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nieuwe Microsoft Dynamics 365-producten en -aanbiedingen beschikbaar op 1 april 2021

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

Op 1 april 2021 start Microsoft verschillende nieuwe producten en aanbiedingen voor het programma Cloud Solution Provider (CSP).

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle partners die het programma Cloud Solution Provider (CSP)

### <a name="details"></a>Details

Op 1 april 2021 start Microsoft de volgende nieuwe producten en aanbiedingen:

- Power BI Premium per gebruiker
- Geo- en segmentuitbreiding voor Customer Voice en Marketing USL

**Power BI Premium per gebruiker**

Microsoft introduceert de eerste aanbiedingen per gebruiker Power BI Premium gebruikersaanbiedingen. Power BI Premium wordt momenteel alleen verkocht in een capaciteits constructie. Power BI Premium per gebruiker biedt toegang tot enterprise business intelligence (BI) en analysemogelijkheden. De flexibele licentieverlening voor individuele licenties is geschikt voor kleine en middelgrote bedrijven.

Bekijk de [Power BI van de release](/power-platform-release-plan/2020wave2/power-bi/planned-features) voor meer informatie over deze aanbieding.


**Aanbiedingsdetails**

Houd er rekening mee dat de naam van de aanbieding enigszins afwijkt van de preview-versie van de prijslijst.

| Naam van aanbieding | Aanbiedings-id |
| ------ |----------- |
| Power BI Premium per gebruiker | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium per gebruiker voor onderwijsmedewerkers | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium per gebruiker voor studenten | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium per gebruiker (non-profit personeel prijzen) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium per gebruiker Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium per gebruiker Add-On voor onderwijsmedewerkers | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium per gebruiker Add-On voor studenten | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium per Add-On (non-profit personeel prijzen) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**UsL geo- en segmentuitbreiding voor Customer Voice en Marketing**

Als vervolg op de lancering van december 2020 zijn de USL-aanbiedingen voor Dynamics 365 Customer Voice en Marketing gewijzigd om nieuwe landen en meer non-profit- en onderwijs-SKU's toe te voegen.

| Naam van aanbieding | Aanbiedings-id |
| ------ |----------- |
| Dynamics 365 Customer Voice USL (Non-profit personeel prijzen) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice USL for Faculty | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Ga naar de volgende pagina's voor meer informatie over deze aanbiedingen:

- [Startpagina van Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Startpagina voor Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.  

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Microsoft Universeel afdrukken nu beschikbaar in sommige suites

### <a name="categories"></a>Categorieën

- Datum: 2021-03-33
- Functies

### <a name="summary"></a>Samenvatting

Microsoft Universeel afdrukken is vanaf 1 maart 2021 beschikbaar voor transact binnen bepaalde Microsoft 365-suites en als zelfstandige invoegactie.

### <a name="impacted-audience"></a>Beïnvloede doelgroep

Alle partners die het programma Cloud Solution Provider (CSP)

### <a name="details"></a>Details

[Universeel afdrukken](https://aka.ms/universalprint) is een Microsoft 365 afdrukservice waarmee on-premises afdrukservers niet meer nodig zijn en Windows-apparaten kunnen afdrukken naar bij Azure geregistreerde printers. Deze is beschikbaar voor transact vanaf 1 maart 2021.

Werknemers profiteren van afdrukken zonder stuurprogramma, gestroomlijnde locatiegebaseerde printerdetectie en een intuïtieve afdrukervaring zonder leercurve. Apparaten die zijn verbonden met Azure Active Directory (Azure AD) gebruiken bestaande Azure AD-referenties om veilig af te drukken. Beheerders beheren afdrukken met behulp van de Azure Portal en kunnen printers eenvoudig verbinden met systeemeigen ondersteuning voor Universeel afdrukken. Universeel afdrukken kunnen worden geïmplementeerd met niet-compatibele printers met behulp van connector voor Universeel afdrukken-software.

Universeel afdrukken wordt bij de start van Windows E3, A3, E5 en A5 en Microsoft 365 BP, F3, E3, A3, E5 en A5 ingevuld.  

**Aanbiedingsdetails**

Houd er rekening mee dat de naam van de aanbieding enigszins afwijkt van de preview-versie van de prijslijst.

| Naam van aanbieding | Aanbiedings-id | Materiaal-id |
| ------ |----------- |----------- |  
| Universeel afdrukken volume-invoeging (500 taken) - Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Universeel afdrukken volume-invoeging (500 taken) voor onderwijsmedewerkers - Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Universeel afdrukken volume-invoeg-on (500 taken) - Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Universeel afdrukken volume-invoeging (500 taken) voor onderwijsmedewerkers - Windows   |  d0862f05-80f5-4fd4-8432-fe72ddd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Volgende stappen

Vertrouwd raken met de prijslijst en het Universeel afdrukken [overzicht](/universal-print/fundamentals/universal-print-whatis). Deel deze informatie met alle juiste contactpersonen in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen.
