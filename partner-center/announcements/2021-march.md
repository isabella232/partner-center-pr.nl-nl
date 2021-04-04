---
title: Aankondigingen van maart 2021
description: Maart 2021 aankondigingen voor micro soft-partner centrum, inclusief nieuwe mogelijkheden, aanbiedingen, aanbiedingen, markten of wijzigingen in bestaande aanbiedingen.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 5b8c5f52207a7b9a49d07885a36b61486be45497
ms.sourcegitcommit: 60bbb8f4056120264b769f94431f84d86984c2e9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/03/2021
ms.locfileid: "106280867"
---
# <a name="march-2021-announcements"></a>Aankondigingen van maart 2021

Deze pagina bevat de aankondigingen voor het micro soft partner centrum voor maart 2021.

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a>Bijgewerkte CSP-klant adres validatie-API nu beschikbaar voor testen

### <a name="categories"></a>Categorieën

- Datum: 2021-03-31
- Functies

### <a name="summary"></a>Samenvatting

Als onderdeel van onze toezeg ging om partners en klanten te helpen hun bedrijf op basis van vertrouwen uit te voeren, zullen we wereld wijd partners uitnodigen om de wijzigingen in de ValidateAddress-API te testen.

### <a name="impacted-audience"></a>Doel groep

Alle CSP direct-factuur partners en indirecte providers die nieuwe klant adres gegevens maken of bijwerken

### <a name="details"></a>Details

Micro soft werkt op vertrouwen. We streven ernaar een compatibele, veilige en veilige methode te bieden voor het indienen van validatie van klant adressen voor het handelen van klant abonnementen in het CSP-programma. Vandaag 31 maart 2021 zijn er wijzigingen aangebracht in de ValidateAddress-API die u wilt uitnodigen om te testen voordat u live gaat met de wijzigingen in juni 2021. 

Houd er rekening mee dat deze wijzigingen alleen van invloed zijn op de ValidateAddress-API. CreateCustomer-en UpdateBillingProfile-Api's worden niet beïnvloed.

Het antwoord retourneert een van de volgende status berichten:

| Status | Beschrijving | Aantal voorgestelde opgehaalde adressen |
|----------|-------------|-------------------|
| VerifiedShippable | Adres wordt gecontroleerd en kan worden verzonden naar. | Enkelvoudig |
| Gegaan | Adres is geverifieerd. | Enkelvoudig |
| InteractionRequired | Aanbevolen adres (sen) is aanzienlijk gewijzigd en heeft de gebruikers bevestiging nodig. | Enkelvoudig |
| StreetPartial | De opgegeven straat in het adres is gedeeltelijk en er is meer informatie nodig. | Meerdere: Maxi maal drie|
| PremisesPartial | De opgegeven locatie (gebouw nummer, Suite nummer, enz.) is gedeeltelijk en er is meer informatie nodig. | Meerdere: Maxi maal drie |
| Meerdere | Er zijn meerdere velden die gedeeltelijk in het adres voor komen (mogelijk ook met StreetPartial en PremisesPartial). | Meerdere: Maxi maal drie |
| Geen | Adres is onjuist. | Geen |
| NotValidated | Het adres kan niet worden verzonden via het validatie proces.  | Geen |

Zodra een adres is verzonden om te worden gevalideerd via de ValidateAddress-API, wordt het volgende antwoord schema geretourneerd:

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

Bekijk dit voorbeeld antwoord. Houd er rekening mee dat voor de Verenigde Staten een extra achtervoegsel van vier cijfers voor de post code wordt geretourneerd als u slechts vijf cijfers invoert voor de post code.

```csharp
// IAggregatePartner partnerOperations;
// string customerId;
// s{
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

- Deel uw Tenant-ID van de sandbox met onze deskundige expert (MKB), Ali Donkerkhaki, die in de test vlucht moet worden opgenomen, zodat u kunt beginnen met het voorbereiden van de update.

- Als u een CPV-oplossing (configuratie scherm) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Als u vragen hebt of ondersteuning nodig hebt voor uw bedrijfs activiteiten met micro soft, neem dan contact op met de Yammer-groep van uw partner ondersteuning.

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Nieuwe versie van het Exchange-beheer centrum (SBV)

### <a name="categories"></a>Categorieën

- Datum: 2021-03-29
- Functies

### <a name="summary"></a>Samenvatting

Vanaf 27 april 2021 wordt in het Exchange-beheer centrum (SBV) een nieuwe ervaring geïntroduceerd waarmee de dagelijkse efficiëntie voor gebruikers wordt verbeterd.

### <a name="impacted-audience"></a>Doel groep

Gedelegeerde beheerders hebben toegang tot Exchange via partner centrum

### <a name="details"></a>Details

Vanaf 27 april 2021 worden partners die navigeren naar Exchange via partner Center, omgeleid naar de nieuwe SBV.

Deze nieuwe ervaring is momenteel beschikbaar als preview-versie en beheerders kunnen deze ervaring activeren door de in de rechter bovenhoek van de klassieke SBV te selecteren. Ze kunnen ook naar de nieuwe SBV navigeren door de banner ' nu uitproberen ' te selecteren die op alle pagina's wordt weer gegeven.

De voor delen van de nieuwe SBV zijn onder andere:

- Er zijn inzichten, rapporten en waarschuwings mechanismen toegevoegd voor problemen met betrekking tot de mail stroom. 

- Persoonlijke Dash boards om de productiviteit te verg Roten.

Om u te helpen door de nieuwe ervaring, zijn er Video's beschikbaar in het gedeelte **Training & Guide** van de nieuwe SBV-ervaring. Op deze manier krijgt u een overzicht van hoe u de nieuwe portal het beste kunt gebruiken.

>[!NOTE]
>Met deze wijziging wordt de klassieke SBV-ervaring niet afgeschaft. Voordat u een wijziging implementeert, wordt u vooraf op de hoogte gebracht.

### <a name="next-steps"></a>Volgende stappen

- Bekijk de [bronnen over dit onderwerp](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), waar u scherm afbeeldingen van de nieuwe ervaring kunt weer geven.

- Deel deze informatie met de juiste belanghebbenden in uw organisatie. 

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze wijzigingen.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Micro soft Operations: introductie van de agenda voor product lancering

### <a name="categories"></a>Categorieën

- Datum: 2021-03-25
- Aanbiedingen | Moderne werk plek

### <a name="summary"></a>Samenvatting

In reactie op feedback van de partner stroomt micro soft-activiteiten de communicatie voor het starten van het product.

### <a name="impacted-audience"></a>Doel groep

CSP-partners (Cloud Solution Provider)

### <a name="details"></a>Details

Micro soft streeft ernaar om de partner ervaringen continu te verbeteren. We hadden feedback van u dat u te veel communicatie van micro soft hebt ontvangen, waaronder dubbele aankondigingen voor product lanceringen.

Als reactie op uw feedback heeft micro soft de gereedheids ervaring voor product lanceringen gestroomlijnd voor nieuwe en bestaande aanbiedingen.

We bieden u nu een enkele maandelijkse weer gave van product lanceringen, gepubliceerd in de resource galerie voor de gereedheids taken. In deze maandelijkse [weer gave voor het starten](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) van een product wordt de communicatie van afzonderlijke producten in de resource galerie voor Operations Readiness en in het partner centrum vervangen.

U hebt ook toegang tot deze [product lancerings agenda](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) vanuit [Community-verzamelingen](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [agenda weergaven](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated)en [CSP-nieuws brieven](https://partner.microsoft.com/resources/collection/csp-monthly-update#/). We sturen u een melding wanneer we de product lancerings agenda van elke maand publiceren met een aankondiging in de resource galerie voor de gereedheids taken.

U kunt nog steeds informatie vinden over nieuwe en bestaande aanbiedingen in de prijs lijst en prijs lijst wijzigings logboeken, evenals in product Blogs, licentie handleidingen en product marketing pagina's.

De wijziging is van toepassing op het starten van de volgende producten:

- On-premises Dynamics
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Server  
- Hulpprogramma's
- Teams en telecommunicatie

We blijven specifieke aankondigingen verzenden voor product lanceringen waarvoor Details van de gereedheids bewerkingen zijn vereist.

### <a name="next-steps"></a>Volgende stappen

Bekijk de bronnen over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor meer vragen over deze aanbiedingen.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Wijzigingen in de vereisten voor de CSP-klant voor bereiding

### <a name="categories"></a>Categorieën

- Datum: 2021-03-25
- Functies

### <a name="summary"></a>Samenvatting

Als onderdeel van onze toezeg ging om partners en klanten te helpen hun bedrijf op basis van vertrouwen uit te voeren, zullen we bijkomende klant gegevens aanvragen, met ingang van 25 maart 2021.

### <a name="impacted-audience"></a>Doel groep

Cloud Solution Provider (CSP) direct factuur partners en indirecte providers die nieuwe of bestaande klanten hebben in de landen die worden vermeld in de volgende sectie

### <a name="details"></a>Details

Micro soft werkt op vertrouwen. We streven ernaar een compatibele, veilige en veilige methode voor klant validatie te bieden voor het handelen van klant abonnementen in het CSP-programma. Op 25 maart 2021 worden de verbeteringen van de Partner Center API en gebruikers interface (UI) geïntroduceerd die van invloed zijn op partners die voldoen aan de volgende criteria:

1. De partner heeft een directe facturerings relatie met micro soft (wat betekent dat de partner een directe factuur partner of een indirecte provider is).

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

Partners die aan de criteria voldoen, moeten de **registratie-id** van een klant (ook wel de **organisatie Inn**) en het **telefoon nummer** van de klant indienen wanneer ze nieuwe klanten vrijgeven of bestaande klant gegevens wijzigen. Deze partners kunnen ook een optionele **middelste naam** voor de klant invoeren.

Houd er rekening mee dat wanneer u de registratie-ID van uw bedrijf toevoegt, u uw zakelijke belasting-ID moet gebruiken en niet de persoonlijke ID van de klant.

Partners die zaken doen met nieuwe of bestaande klanten in de volgende landen, hebben in november 2020 al geknoeid met een eerdere release.

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

Partners met klanten in de rest van de wereld hebben de mogelijkheid om op 25 maart 2021 de **registratie-id**, het **telefoon nummer** en de **middelste naam** van het bedrijf in te voeren als optionele Details.

### <a name="next-steps"></a>Volgende stappen

- Raadpleeg de technische documentatie en veelgestelde vragen in de [verzameling speciale partners](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) voor meer gedetailleerde richt lijnen.

- Bereid u voor op het opnemen van de wijzigingen met behulp van de partner centrum-API en webervaring. API/Sdk's zijn beschikbaar voor testen.

- Zorg ervoor dat u de aanvullende gegevens indient bij het voorbereiden van nieuwe klanten of het wijzigen van bestaande klant gegevens.

- Als u een CPV-oplossing (configuratie scherm) gebruikt, raadpleegt u uw CPV.

### <a name="questions"></a>Vragen?

Neem contact op met uw belasting adviseur of gemeentelijke belasting dienst als u vragen hebt met betrekking tot de juridische id (ook wel INN of TIN genoemd). Micro soft kan geen ondersteuning bieden voor belasting kwesties.

Als u ondersteuning nodig hebt in uw bewerkingen met micro soft, [opent u een service aanvraag](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correcties die zijn aangebracht in 1 maart 2021 lijst met permanente software prijzen

### <a name="categories"></a>Categorieën

- Datum: 2021-03-23
- Aanbiedingen/markten

### <a name="impacted-audience"></a>Doel groep

Indirecte providers en directe factuur partners die permanente software in het Cloud Solution Provider-programma worden toegepast 

### <a name="details"></a>Details

De lijst met prijzen voor permanente software die is gepost op 1 maart 2021 bevatte markten die daar niet had moeten zijn. De prijs lijst met permanente software is op 17 maart 2021 bijgewerkt met de correcties. Deze correcties zijn alleen van toepassing op:

- Product-ID: DF77X4D43RKT 
- Product naam: Windows 10 Home naar Pro-upgrade voor Microsoft 365 Business
- Verwijderde of niet-ondersteunde markten: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, LC, CM, CO, CR, CW, DO, DZ, EG, bijvoorbeeld, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, te maken, MA, MC, MD, & NG , NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW'S, AG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, MG, UY, UZ, VE, VN, YE, ZM, ZW

Deze wijzigingen zijn alleen van toepassing op het bovenstaande product. Andere producten hebben geen correcties. 

### <a name="next-steps-and-resources"></a>Volgende stappen en resources

- Partners die permanente software transacteren, moeten de meest recente prijs lijst met permanente software downloaden.
- Raadpleeg de [regio land codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) voor een beschrijvende toewijzing van de afkorting van twee letters aan landen.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> SDK-release op .NET Standard (v 1.17.0)

### <a name="categories"></a>Categorieën

- Datum: 2021-03-23

- Functies
 
### <a name="impacted-audience"></a>Doel groep

Directe factuur partners en indirecte providers die deel nemen aan het CSP-programma dat gebruikmaakt van de .NET SDK van het partner centrum.

### <a name="details"></a>Details

Vanaf maart 23 2020 kunnen partners beginnen met het downloaden van de versie van [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Micro soft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), samen met bijgewerkte voor beelden van het Public Partner Center SDK [github](https://github.com/Microsoft/Partner-Center-DotNet-Samples). Deze versie bevat updates voor de volgende methoden:

#### <a name="audit-updated-new-operation-types"></a>Controle bijgewerkt: nieuwe bewerkings typen

Er zijn nieuwe [bewerkings typen](https://docs.microsoft.com/partner-center/develop/auditing-resources) toegevoegd om te weten wanneer de door de klant goedgekeurde en BEËINDIGDe DAP is.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Controle bijgewerkt: nieuwe resource-en bewerkings typen

Er zijn nieuwe [resource-en bewerkings typen](https://docs.microsoft.com/partner-center/develop/auditing-resources) toegevoegd voor het ondersteunen van het scenario voor de Directory functie van klanten.

- Nieuw resource type "CustomerDirectoryRole"

- Bewerkings typen ' AddUserMember ' en ' RemoveUserMember '

#### <a name="sdk-updates-to-customer-accounts"></a>SDK-updates voor klant accounts

- Ondersteuning voor GET-/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- /Customers/{Customer-Tenant-id}/Qualifications ophalen

- POST/Customers/{customer_id}/Qualifications? code = {validationCode}

#### <a name="additional-changes"></a>Aanvullende wijzigingen

De volgende wijzigingen worden geïntroduceerd als onderdeel van nieuwe Commerce en zijn momenteel alleen beschikbaar via een uitnodiging voor partners die deel uitmaken van de M365/D365 nieuwe technische preview van Commerce-ervaring. Partners die geen deel uitmaken van de nieuwe technische preview van Commerce, mogen geen gevolgen ondervinden en moeten neerwaarts compatibel zijn.

- Wijzigingen in catalogus:

  - /Products/{product-id}/SKUs/{SKU-id} ophalen

- Kopen en beheren:
  - /Customers/{customerId}/subscriptions ophalen
  - /Customers/{customerId}/subscriptions/{subscriptionId} ophalen
  - PATCH/customers/{customerId}/subscriptions/{subscriptionId}
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities ophalen
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitions ophalen
  - /Customers/{customerId}/subscriptions/{subscriptionId}/transitions plaatsen

### <a name="next-steps"></a>Volgende stappen

- Down load de meest recente versie [MicrosoftPartnerCenter. NETSDK (NuGet Gallery | Micro soft. Store. PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- De GitHub-voor [beelden](https://github.com/Microsoft/Partner-Center-DotNet-Samples) downloaden en bekijken

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>CSP Commercial Marketplace-aanbieding en FY21 CSP-stimulansen voor in aanmerking komende aanbiedingen

### <a name="categories"></a>Categorieën

- Datum: 2021-03-18
- Functies

### <a name="impacted-audience"></a>Doel groep

Indirecte providers en directe factuur partners in het Cloud Solution Provider-programma 

### <a name="details"></a>Details

Indirecte providers en directe factuur partners in het Cloud Solution Provider-programma kunnen aanbiedingen van derden verkopen en een kortings stimulans verdienen voor elke in aanmerking komende trans acties van derden in Partner Center of de Azure Portal. De stimulans is in de vorm van een korting op gefactureerde verkoop voor de in aanmerking komende aanbiedingen en is **beschikbaar tot 30 juni 2021**.  

Blijf op de hoogte van deze CSP Commercial Marketplace en neem contact op met uw klanten om de juiste aanbiedingen te identificeren om hun voortdurende succes volle en digitale trans formatie mogelijk te maken.

We werken samen met Independent Software Vendors (Isv's) om de nieuwste IaaS-en SaaS-oplossingen op de markt te brengen voor klanten van micro soft. ISV-uitgevers hebben de mogelijkheid om verkoop van hun aanbiedingen in te scha kelen via het micro soft partner Channel. Onze aanbiedingen die in aanmerking komen voor een stimulans, worden onderverdeeld in twee categorieën:

- Selecteer SaaS en IaaS aanbiedingen van derden met Azure IP co-sell gemotiveerd-status. 

- SaaS-toepassingen die zijn geïntegreerd met teams of ten minste twee Microsoft 365 productiviteits-apps, zoals Power Point, Word, Excel, Outlook of share point.

### <a name="next-steps-and-resources"></a>Volgende stappen en resources

- Meer informatie over het verdienen van [partner prikkels](https://partner.microsoft.com/membership/partner-incentives) voor het verkopen van in aanmerking komende Marketplace-apps de in aanmerking komende apps. Nieuwe aanbiedingen worden maandelijks toegevoegd.  
- [Resources voor directe factuur bronnen van Cloud Solution Provider](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Bronnen voor het stimuleren van indirecte providers van Cloud Solution Provider](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Neem deze [presentatie](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) door om meer te weten te komen over het verkopen van de apps voor commerciële Marketplace. Bekijk [hier](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/)meer informatie. 
- Verken de catalogus met commerciële Marketplace in [partner centrum](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) of [Azure Portal](https://ms.portal.azure.com/#home)
- [Api's](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) gebruiken om apps te integreren in de Marketplace van uw bedrijf
- Neem contact op met Isv's waarmee u zaken wilt doen
- Indirecte providers moeten integreren met behulp van Api's en richt lijnen voor gids waarop apps worden verkocht

### <a name="questions"></a>Vragen?  

Raadpleeg [dit artikel](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) voor een overzicht van de commerciële Marketplace in het partner centrum.

Als u aanvullende hulp nodig hebt, kunt u een ondersteunings aanvraag maken in het partner centrum. Meer informatie vindt u in [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1) .

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Naam en vereiste update van Power BI Premium-aanbieding

### <a name="categories"></a>Categorieën

- Datum: 2021-03-18
- Functies

### <a name="summary"></a>Samenvatting

De laatste prijs lijst van 1 april 2021 wordt bijgewerkt om duidelijkheid toe te voegen aan de naam en/of vereiste informatie voor Power BI Premium per gebruiker.

### <a name="impacted-audience"></a>Doel groep

Directe en indirecte partners van Cloud Solution Provider (CSP)

### <a name="details"></a>Details

De laatste prijs lijst van 1 april 2021 wordt bijgewerkt om duidelijkheid toe te voegen aan de naam en/of vereiste informatie voor Power BI Premium per gebruiker.

Totdat de uiteindelijke prijs lijst is bijgewerkt, gebruikt u de informatie in deze sectie om te controleren of het juiste product is besteld.

In de volgende details worden de betreffende SKU en de vereiste details weer gegeven.

| Weergave naam aanbieding op 1 maart prijs lijst preview |  De weergave naam van de aanbieding is bijgewerkt op 1 april van de uiteindelijke prijs lijst| Aanbiedings-id |
| ------ | ----------- | ----------- |
| Power BI Premium per gebruikers Add-On (prijs van het non-profit personeel)  |  Power BI Premium per gebruiker Add-On **(Office)** (prijs van de non-profit organisatie)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Klanten moeten beschikken over een van de volgende vereisten om deze aanbieding aan te schaffen:

| Weergave naam van aanbieding | Aanbiedings-id |
| ------ | ----------- |
| Microsoft 365 E5 (prijs van het non-profit personeel)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 zonder audio conferencing (prijzen voor non-profit organisaties)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (prijs van het non-profit personeel)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Proef versie van Office 365 E5 (non-profit mede werkers)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 zonder audio conferencing (prijs stelling voor non-profit organisaties)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

Voor de volgende Power BI Premium aanbieding is een vereiste vereist voor aankoop:

| Weergave naam van aanbieding | Aanbiedings-id |
| ------ | ----------- |
|   Power BI Premium per gebruikers Add-On (prijs van het non-profit personeel)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Klanten moeten beschikken over deze vereiste om deze aanbieding aan te schaffen:

| Weergave naam van aanbieding | Aanbiedings-id |
| ------ |----------|
| Power BI Pro (prijs van de non-profit organisatie)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.  

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Prijzen updates van maart voor Microsoft 365 F3

### <a name="categories"></a>Categorieën

- Datum: 2021-03-16
- Aanbiedingen/markten

### <a name="summary"></a>Samenvatting

De prijzen voor een onjuiste prijs van maart 2021 zijn gecorrigeerd voor Microsoft 365 F3 Britse pond (GBP) en euro (EUR).

### <a name="impacted-audience"></a>Doel groep

Partners kopen Microsoft 365 F3 in GBP of EUR tussen 1 maart en 17 maart 2021 via het programma Cloud Solution Provider (CSP).

### <a name="details"></a>Details

Micro soft heeft onjuiste prijzen voor Microsoft 365 F3 opgelost. De onjuiste prijzen waren voor GBP en EUR en alleen voor aanbiedingen die zijn gekocht tussen 1 maart en 17 maart 2021. De aanbiedingen en valuta's die worden beïnvloed, worden hieronder weer gegeven. 

| Naam van aanbieding | Valuta | Aanbiedings-id | Materiaal-ID |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (liefdadigheids instelling) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (Commercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
De preview-versie van de licentie prijs lijsten van maart en april zijn bijgewerkt op 16 maart tot 17:00 uur Pacific (standaard tijd).

### <a name="next-steps"></a>Volgende stappen

- Partners moeten de huidige prijs lijsten op basis van licenties, zowel maart als de preview-versie van april, opnieuw downloaden, met deze prijs correcties, indien van toepassing.  
- Micro soft neemt via e-mail contact met betrokken partners in de komende weken om hen te informeren over de volgende stappen die betrekking hebben op het corrigeren van betrokken trans acties.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante CSP-Yammer-community's voor meer vragen.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> De naam van een rechts bedrijf bijwerken via partner centrum

### <a name="categories"></a>Categorieën

- Datum: 2021-03-16
- Efficiëntie van schijf & schalen

### <a name="summary"></a>Samenvatting

Met ingang van 2021, Microsoft Partner Network (MPN)-partners en Cloud Solution Provider (CSP) kunnen indirecte wederverkopers hun juridische bedrijfs naam bijwerken via partner centrum.

### <a name="impacted-audience"></a>Doel groep

MPN-partners en indirecte leveranciers van CSP'S (niet van toepassing op de CSP direct-factuur partners)

### <a name="details"></a>Details

Vanaf 2021 maart kunnen MPN-partners en indirecte leveranciers van CSP'S hun juridische bedrijfs naam via partner centrum bijwerken op een compatibele, op zichzelf gebaseerde manier. Met deze nieuwe functie hoeven partners niet langer een ondersteunings ticket van het partner centrum in te dienen om hun bedrijfs naam bij te werken. Dit bespaart een aanzienlijke hoeveelheid tijd voor partners wanneer deze activiteiten worden uitgevoerd. 

Zie [uw juridische zakelijke profiel bijwerken](../update-your-partner-profile.md#update-your-legal-business-profile)voor meer informatie.

>[!NOTE]
>Zorg ervoor dat de bedrijfs naam in uw juridisch bedrijfs profiel geen spel fouten en afkortingen bevat en exact overeenkomt met uw formele zakelijke registratie records voor bedrijven. Raadpleeg [uw organisatie profiel verifiëren](../update-your-partner-profile.md#update-your-legal-business-profile)voor meer informatie over het bijwerken van uw organisatie profiel.

### <a name="next-steps"></a>Volgende stappen

Deel deze informatie in uw organisatie zodat het juiste team hun processen kan controleren en bijwerken.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante CSP-Yammer-community's voor meer vragen.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Bijwerken naar de ontwikkeling van het programma voor Cloud Solution Provider (CSP) en Open License-programma wijzigingen

### <a name="categories"></a>Categorieën

- Datum: 2021-03-15
- Functies

### <a name="summary"></a>Samenvatting

Er zijn nieuwe aanbiedingen voor permanente software van de commerciële en publieke sector beschikbaar voor het programma van de Cloud Solution Provider (CSP), samen met wijzigingen in het open Licensing-programma.

### <a name="impacted-audience"></a>Doel groep

Commerciële distributeurs en beheerde wederverkopers die verkopen via het Open License-programma, evenals alle CSP-partners die gebruikmaken van permanente software

### <a name="details"></a>Details

In september 2020 heeft micro soft een reeks stappen [aangekondigd](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) in onze digitale trans formatie-reis om mogelijkheden uit te breiden naar partners in het CSP-programma, met inbegrip van de beschik baarheid van on-premises software voor partners. Met deze wijzigingen kunnen partners hun bedrijf groeien en hun bereik uitbreiden door gebruik te maken van software licenties in CSP. plaats ze in de Cloud-eerste wereld. Ze bieden klanten ook de mogelijkheid om over te stappen naar de Cloud en kunnen partners de flexibiliteit geven die nodig is voor klanten hybride Cloud omgevingen.

Ter voortzetting van deze digitale trans formatie kondigen we de volgende wijzigingen aan:

- 1 juli 2021: er worden geen nieuwe Sku's, producten of promoties toegevoegd aan de prijs lijst van het Open License-programma.

- 7 juli 2021: er worden twee commerciële aanbiedingen opgehaald, legitieme Windows-en Visual Studio Professional-producten en aanbiedingen voor open bare sectoren (overheid, onderwijs en non-profit [organisaties bekijken)](./2020-december.md#9)toegevoegd aan de lijst met door de CSP permanente software geprijsd.  De prijs lijst kan worden gevonden in het gedeelte software van de pagina [verkoop > prijzen &](https://partnercenter.microsoft.com/pcv/sales) in partner centrum en wordt op deze datum opnieuw gepubliceerd.

Zie de **volgende stappen** voor meer informatie over de ontwikkeling van het CSP-programma en het openen van het licentie programma.

### <a name="next-steps"></a>Volgende stappen

- CSP-programma evolutie: Bekijk de [permanente software in de gereedheids materialen van het Cloud Solution Provider-programma](https://partner.microsoft.com/resources/collection/software-in-csp#/) . Gebruik deze [gereedheids toewijzing](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) om snel de juiste informatie te vinden voor uw rol.

- Wijzigingen in het licentie programma openen: Bekijk de ontwikkeling van het [CSP-programma en Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) -programma wijzigingen gereedheids materialen. Gebruik deze [gereedheids toewijzing](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) om snel de juiste informatie te vinden voor uw rol.

### <a name="questions"></a>Vragen

Raadpleeg uw relevante CSP-Yammer-community's voor meer vragen.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Bijwerken naar een eerdere aankondiging: Premium-evaluaties, een invoeg toepassing voor nalevings beheer

### <a name="categories"></a>Categorieën

- Datum: 2021-03-15
- Uw bedrijf laten groeien

### <a name="summary"></a>Samenvatting

De proef aanbiedingen mogen niet worden vermeld op de prijs lijst en worden verwijderd.

### <a name="impacted-audience"></a>Doel groep

Partners die communiceren via de Cloud Solution Provider

### <a name="details"></a>Details

De proef aanbiedingen mogen niet zijn opgenomen in de prijs lijst. Deze worden verwijderd uit de prijs lijst van 1 mei 2021.

De oorspronkelijke aankondiging is [hier](./2021-february.md#4).

### <a name="additional-resources"></a>Aanvullende bronnen

- [Microsoft 365 E5 beveiliging en naleving](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Evaluaties bouwen en beheren in micro soft Compliance Manager-Microsoft 365 naleving](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources over dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migreer uw oplossingen van de ene commerciële partner (OCP) go-to-Market (GTM) naar de micro soft Commercial Marketplace

### <a name="categories"></a>Categorieën

- Datum: 2021-03-12
- Functies

### <a name="summary"></a>Samenvatting

Van 29 maart 2021 gaat u slechts een beperkt aantal GTM-functies (go-to-Market) van één commerciële partner (OCP) ervaren. We raden u aan uw oplossingen te migreren naar de commerciële Marketplace in Partner Center.

### <a name="impacted-audience"></a>Doel groep

Organisaties die samen verkopen met oplossingen in OCP GTM

### <a name="details"></a>Details

In december 2020 zijn we begonnen met onze reis van het micro soft OCP GTM-hulp programma naar de micro soft Commercial Marketplace in Partner Center. Met deze overgang worden de mogelijkheden van de commerciële Marketplace uitgevouwen, waar u uw oplossingen kunt presen teren aan miljoenen klanten, kansen delen met andere verkopers van micro soft en partners, en gezamenlijk innoverende oplossingen verkopen.

De volgende mijl paal in de overgang vindt plaats op 29 maart 2021. Dat is het geval wanneer u beperkte mogelijkheden van de OCP GTM gaat ervaren, waarbij sommige velden alleen-lezen worden. Als u momenteel mede-verkoop met oplossingen in OCP GTM, raden we u aan uw oplossingen naar de commerciële Marketplace te migreren om te profiteren van de mogelijkheden en uw publicatie ervaring te vereenvoudigen. 

Door over te stappen op de commerciële Marketplace is partner Center het primaire doel voor de publicatie-ervaring voor de co-verkoop. Het is waar u uw bedrijf kunt blijven uitbreiden door uw oplossingen te verbinden met onze gedeelde klanten via dezelfde kanalen en in-product ervaringen die we gebruiken voor micro soft-producten. Meer [informatie over de commerciële Marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Volgende stappen

- Als u uw oplossingen nog niet hebt verplaatst, volgt u de instructies in de [overgangs handleiding](/azure/marketplace/co-sell-solution-migration) of bekijkt u de [Stapsgewijze video zelf studie](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) voor het volt ooien van alle migratie activiteiten en het publiceren van uw oplossing (en) in de commerciële Marketplace.

- Voor vragen met betrekking tot de beperkte mogelijkheden in OCP GTM raadpleegt [u de vereisten voor samen verkoop om te publiceren in de veelgestelde vragen over micro soft Commercial Marketplace](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Zie de sectie "OCP GTM beperkte mogelijkheden vanaf 29 maart 2021.")

### <a name="questions"></a>Vragen?

Neem contact op met de [ondersteuning](https://partner.microsoft.com/support/?stage=1) als u vragen hebt of meer informatie nodig hebt.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>De nieuwe Commerce-ervaring in het Cloud Solution Provider-programma (CSP) voor Azure naar Rusland uitbreiden

### <a name="categories"></a>Categorieën

- Datum: 2021-03-10
- Functies

### <a name="impacted-audience"></a>Doel groep

Alle partners in Rusland communiceren via het CSP-programma (Cloud Solution Provider).

### <a name="details"></a>Details

Vanaf 10 2021 maart kunnen we de beschik baarheid van de **nieuwe Commerce-ervaring in CSP voor Azure in Rusland** aankondigen. Met deze ervaring kunt u de manier waarop klanten Azure-Services kopen en gebruiken, stroom lijnen en verbeteren. Het biedt ook partners in het CSP-programma een consistente weer gave van Azure-prijzen voor verkoop bewegingen, USD-prijzen voor globale consistentie, facturerings datum uitlijning en toegang tot Azure Cost Management.

### <a name="next-steps"></a>Volgende stappen

Er zijn verschillende bronnen beschikbaar die de nieuwe Azure commerce-ervaring introduceren en aanvullende informatie bieden. Zoek de meest recente Veelgestelde vragen, dekken, video en meer in de [resource galerie van het CSP-programma updates](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Licentie sleutel voor partner centrum-software en down loads

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

De functie voor het downloaden van partner centrum-software en de levering van licentie sleutels is opnieuw ingesteld.

### <a name="impacted-audience"></a>Doel groep

Alle leveranciers van Cloud Solution Providers (CSP) handelen permanente en server Subscription software orders via partner centrum

### <a name="details"></a>Details

Als reactie op feedback van de partner reactiveren de mogelijkheden van het Partner Center om software-en licentie sleutels te verkrijgen voor de bestellingen van permanente en server abonnementen. Het wordt teruggezet naar de vorige staat voordat deze werd verwijderd op 19 januari 2021. (Zie de [aankondiging](2020-september.md#17).)

Houd er rekening mee dat software licentie sleutels en download koppelingen waardevol en Maxi maal worden aangestuurd na intellectuele-eigendoms activa. Als ze worden gelekt, kunnen ze snel worden uitgeput met hun activerings limieten en een negatieve klant-en partner ervaring veroorzaken.

### <a name="next-steps"></a>Volgende stappen

Raadpleeg de volgende bronnen voor gebruiks instructies en belang rijke richt lijnen voor het distribueren van software sleutels:

- [On-premises software verkopen via het CSP-programma](../csp-on-premise-software.md)
- [Partner centrum-nieuwe Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Zie de sectie **richt lijnen voor het distribueren van software sleutels** .)

### <a name="questions"></a>Vragen?

Als u meer vragen over deze kennisgeving hebt, controleert u uw relevante Yammer-community's.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Uw deals migreren van partner Sales Connect (PSC) naar partner centrum

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

Partner Sales Connect (PSC) gaat over naar alleen-lezen toegang vanaf 31 maart 2021. Daarom raden we u aan om te beginnen met het migreren van uw deals van PSC naar partner Center.

### <a name="impacted-audience"></a>Doel groep

Partners met deals in PSC

### <a name="details"></a>Details

Als onderdeel van onze gedeelde betrokkenheid bij groei is **samen met micro soft** het pad te vinden dat u kunt **detecteren, uw expertise te leveren en uw klant footprint te verg Roten** voor positieve klant resultaten. Met een gemiddelde **duur van 3,5 keer sneller** dan normaal is het beheren van de ervaring voor samen werking in het partner centrum dat u kunt verkopen aan de directe klanten-, partner-en micro soft-verkopers kanalen, en uw volledige referentie pijplijn op één locatie te beheren.

**PSC** gaat over naar **alleen-lezen toegang** vanaf **31 maart 2021**. Daarom raden we u aan om uw overstap naar partner centrum te starten en de verbeteringen van deze functies te openen: 

- **Meer nauw keurige route ring** van de deals die u deelt met micro soft naar de juiste verkoper, op basis van het type hulp die u nodig hebt.
- **Validatie** van de geschiktheid van een trans actie voor in aanmerking komende oplossingen en om te voldoen aan de criteria van het ISV-verbindings programma, waardoor het goedkeurings proces en de uiteindelijke test voor de uitvoering (PoE) worden vereenvoudigd.
- **Naadloze gebruikers ervaring** voor het beheren van al uw verkoop kansen en verkoop gekwalificeerde leads op één plek.

Daarnaast hebben we onlangs nieuwe functies toegevoegd in het partner centrum om u te helpen bij het verplaatsen:

- [Bulk bewerkingen voor het samen verkopen van verkoop kansen](../bulk-operations.md)
- [Functie](../psc-to-pc.md) voor de migratie van deals (Zie de sectie **migratie van PSC-deals** .)

Met de ervaring voor de samen werking in Partner Center hebben uw verkoop teams meer tijd besteed aan het richten op nurturing-leads en-kansen, het sluiten van deals en het maken van blijvende klant relaties.

### <a name="next-steps"></a>Volgende stappen

Gebruik de [overgangs gids](../psc-to-pc.md) van het partner centrum om u te helpen bij de stappen voor het migreren van uw deals van PSC naar partner Center.

### <a name="questions"></a>Vragen?

Neem contact op met de [ondersteuning](https://partner.microsoft.com/support/?stage=1)voor meer vragen.

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nieuwe micro soft Dynamics 365-producten en aanbiedingen die beschikbaar zijn op 1 april 2021

### <a name="categories"></a>Categorieën

- Datum: 2021-03-04
- Functies

### <a name="summary"></a>Samenvatting

Op 1 april 2021 worden verschillende nieuwe producten en aanbiedingen voor het programma Cloud Solution Provider (CSP) gestart.

### <a name="impacted-audience"></a>Doel groep

Alle partners communiceren via het CSP-programma (Cloud Solution Provider)

### <a name="details"></a>Details

Op 1 april 2021 zal micro soft de volgende nieuwe producten en aanbiedingen starten:

- Power BI Premium per gebruiker
- GEBRUIKERSABONNEMENTSLICENTIES geo-en-segment uitbreiding van klant spraak en-marketing

**Power BI Premium per gebruiker**

Micro soft introduceert de eerste Power BI Premium aanbiedingen per gebruiker. Power BI Premium wordt momenteel alleen verkocht in een capaciteits constructie. Power BI Premium per gebruiker biedt toegang tot de mogelijkheden van ENTER prise business intelligence (BI) en analyse. De flexibele individuele seat-licentie is voor kleine en middel grote bedrijven.

Bekijk de [Details](/power-platform-release-plan/2020wave2/power-bi/planned-features) van de Power bi-release voor meer informatie over deze aanbieding.


**Details van aanbieding**

Houd er rekening mee dat de naam van de aanbieding iets anders is dan de prijs lijst preview.

| Naam van aanbieding | Aanbiedings-id |
| ------ |----------- |
| Power BI Premium per gebruiker | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium per gebruiker voor faculteiten | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium per gebruiker voor studenten | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium per gebruiker (prijs van de non-profit organisatie) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Power BI Premium per gebruikers Add-On | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Power BI Premium per gebruikers Add-On voor faculteiten | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Power BI Premium per gebruikers Add-On voor studenten | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Power BI Premium per gebruikers Add-On (prijs van het non-profit personeel) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**GEBRUIKERSABONNEMENTSLICENTIES geo-en-segment uitbreiding van klant spraak en-marketing**

Als follow-up van de GEBRUIKERSABONNEMENTSLICENTIES-aanbieding van december 2020 kunnen Dynamics 365-aanbiedingen voor klanten Voice en marketing zijn gewijzigd om nieuwe landen en meer non-profit en onderwijs-Sku's toe te voegen.

| Naam van aanbieding | Aanbiedings-id |
| ------ |----------- |
| Dynamics 365 Customer Voice GEBRUIKERSABONNEMENTSLICENTIES (non profit mede werkers prijs) | 7a8642a5-481e-4906-A642-b56dbeeb62a0 |
| Dynamics 365 Customer Voice GEBRUIKERSABONNEMENTSLICENTIES voor faculteiten | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Ga naar de volgende pagina's om meer te weten te komen over deze aanbiedingen:

- [Start pagina voor Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Start pagina voor Dynamics 365-marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Volgende stappen

Bekijk de resources in dit onderwerp en deel deze informatie met de juiste belanghebbenden in uw organisatie.  

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Micro soft Universal Print nu beschikbaar in sommige suites

### <a name="categories"></a>Categorieën

- Datum: 2021-03-33
- Functies

### <a name="summary"></a>Samenvatting

Micro soft Universal Print is beschikbaar voor Transact binnen select Microsoft 365 suites en als zelfstandige invoeg toepassing van 1 maart 2021.

### <a name="impacted-audience"></a>Doel groep

Alle partners communiceren via het CSP-programma (Cloud Solution Provider)

### <a name="details"></a>Details

[Universal Print](https://aka.ms/universalprint) is een Microsoft 365-afdruk service waarmee de nood zaak van on-premises afdruk servers wordt verwijderd en Windows-apparaten kunnen afdrukken naar door Azure geregistreerde printers. Deze is beschikbaar voor trans acties vanaf 1 maart 2021.

Werk nemers profiteren van afdrukloze afdrukken, gestroomlijnde op locatie gebaseerde printer detectie en een intuïtieve afdruk ervaring zonder leer curve. Apparaten die lid zijn van Azure Active Directory (Azure AD) gebruiken bestaande Azure AD-referenties om veilig af te drukken. Beheerders beheren afdrukken met behulp van de Azure Portal en kunnen eenvoudig printers verbinden met systeem eigen ondersteuning voor universeel afdrukken. Universeel afdrukken kan worden geïmplementeerd met niet-compatibele printers door gebruik te maken van Universal Print Connector software.

Universele afdrukken worden alsnog bij het starten van Windows E3, a3, E5 en A5 en Microsoft 365 BP, F3, E3, a3, E5 en A5.  

**Details van aanbieding**

Houd er rekening mee dat de naam van de aanbieding iets anders is dan de prijs lijst preview.

| Naam van aanbieding | Aanbiedings-id | Materiaal-ID |
| ------ |----------- |----------- |  
| Invoeg toepassing voor universeel afdruk volume (500-taken)-Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Invoeg toepassing voor universele afdruk volumes (500-taken) voor faculteiten-Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Invoeg toepassing voor universeel afdrukken van volumes (500-taken)-Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Invoeg toepassing voor universele afdruk volumes (500-taken) voor faculteiten-Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Volgende stappen

Raadpleeg de prijs lijst en het [universele afdruk overzicht](/universal-print/fundamentals/universal-print-whatis). Deel deze informatie met alle relevante contact personen in uw organisatie.

### <a name="questions"></a>Vragen?

Raadpleeg uw relevante Yammer-community's voor vragen over deze aanbiedingen.
