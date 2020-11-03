---
title: Migreren vanaf partner Sales Connect (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe micro soft-partners kunnen migreren van partner Sales Connect (PSC) naar partner centrum en om deals te maken of te beheren die door micro soft-verkopers worden verzonden.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528484"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Overzicht van het samen werken in Partner Center (PC) voor partners die worden gemigreerd vanuit partner Sales Connect (PSC)

**Van toepassing op**

- Partnercentrum

**Juiste rollen**

- Accountbeheerder
- Beheerder van verwijzingen
- Partner Sales Connect (PSC)-verkoper
- Partner Sales Connect (PSC)-beheerder
- Manager van partner Sales Connect (PSC)

Zoals u weet, verliest uw bedrijf geen toegang tot de PSC post van 31 december 2020. U vindt hier echter alles wat u wilt doen om trans acties te maken, uw deals te beheren en te handelen op deals die door micro soft-verkopers naar u worden verzonden in het partner centrum. Er zijn echter ook verschillen en de volgende richt lijnen helpen u bij het maken van de overgang naar het vloeiender en direct sturen van uw overstap naar partner Center.

>[!Important]
> Als u hier bent, omdat u een banner in PSC hebt gezien over de migratie, bent u op de juiste plaats. Deze hand leiding is niet van toepassing op de oplossings beoordeling (SA) en OEM IOT-partners die hun deals in PSC beheren.

## <a name="before-you-move-things-you-need-to-know"></a>Wat u moet weten voordat u verdergaat

### <a name="if-you-are-psc-admin"></a>Als u een PSC-beheerder bent

- U hebt een werk-e-mail nodig om u aan te melden bij het [partner centrum](https://partner.microsoft.com/).
- Stel uw account in met behulp van de [account beheerder](permissions-overview.md)van het partner centrum.
- Lees dit document voor meer informatie over het samen verkopen van het partner centrum.
- Stel gebruikers accounts in het partner centrum in voor al uw PSC-gebruikers (admin, deals Manager en verkopers rollen) en wijs ze toe aan [referentie beheerders rollen](permissions-overview.md).

>[!Important]
> Zorg ervoor dat de MPN-ID die wordt weer gegeven in de banner PSC beschikbaar is in de lijst met MPN-locaties in partner centrum. U kunt in het partner centrum controleren door naar ' account instellingen ' en '[locaties](manage-locations.md)' te gaan om de lijst te vinden van alle MPNs die zijn gekoppeld aan het partner centrum-account.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Als u PSC voor deals of de verkoper bent

- U hebt een werk-e-mail nodig om u aan te melden bij het [partner centrum](https://partner.microsoft.com/).
- Als u een niet-werk account gebruikt in PSC of uw zakelijke e-mail adres is voor een ander bedrijf dan het partner bedrijf, neemt u contact op met uw PSC-beheerder voor meer informatie over het instellen van accounts.
- Neem contact op met uw PSC-beheerder als uw partner centrum-account is ingesteld, ongeacht het account dat u gebruikt om u aan te melden bij PSC.
- Controleer of u toegang hebt tot partner centrum en de sectie referrals.
- Lees dit document om inzicht te krijgen in de werk stromen en de wijzigingen in partner centrum.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als beheerder in PSC zijn dit de volgende stappen

Als u het tabblad verwijzingen niet ziet:

- De [globale beheerder](permissions-overview.md) van uw bedrijf kan u toegang verlenen tot het tabblad verwijzingen. Als u uw globale beheerder wilt vinden, gaat u naar partner instellingen van het tandwiel pictogram rechtsboven in het partner centrum. Selecteer de pagina gebruikers beheer in het tweede niveau van de linker navigatie balk. Klik op de vervolg keuzelijst met ' alle gebruikers ' in de rechter bovenhoek van de pagina en wijzig in ' globale beheerders '. Op de pagina worden vervolgens alle globale beheerders weer gegeven met hun respectievelijke e-mail-Id's. Neem contact op met de IT-afdeling om toegang te krijgen tot referentie beheerders voor uw werk account.

>[!Important]
> Als uw rol alleen gebruikers beheert in PSC, kunt u de rol [account beheerder](permissions-overview.md#manage-mpn-membership-and-your-company) in het partner centrum krijgen. Als uw rol ook het beheren van mogelijkheden voor co-sell omvat, moet u de beheerdersrol van [referrals](permissions-overview.md#manage-referrals) ophalen. U kunt ook een wijzigings beheer kwalificeren tussen de PSC-Administrators om met de account beheerder van het partner centrum te werken in plaats van alle PSC-beheerders die afzonderlijk aan de account beheerders op de computer zijn gekoppeld.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

- Ga naar het tabblad Verwijzingen in het navigatie deel venster links en controleer of u toegang hebt tot de pagina's.

>[!Note]
> Mogelijk moet u zich afmelden bij Partner Center en u vervolgens weer aanmelden om uw referenties voor toegang tot de pagina's met verwijzingen te vernieuwen.

Nadat u uw account hebt ingesteld in Partner Center,

- Nodig alle gebruikers die een rol ' deals Manager ' of ' verkoper ' hebben in de volgende stap in het partner centrum.
- De [account beheerder](permissions-overview.md#manage-mpn-membership-and-your-company) die u heeft geholpen bij het openen van verwijzingen, kan alle gebruikers uitnodigen.
- Vraag de account beheerder tijdens het uitnodigen van de gebruikers om de rol van [verwijzings beheerder](permissions-overview.md#manage-referrals) toe te wijzen.
- Sommige PSC-gebruikers gebruiken mogelijk een niet-werk account of een account uit een ander domein dan dat u in het partner centrum gebruikt. Al deze gebruikers moeten zich aanmelden bij het partner centrum met hun werk account dat aan uw Azure AD-Tenant is gekoppeld. Uw [globale beheerder](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan u hierbij helpen. Als u uw globale beheerder wilt vinden, gaat u naar partner instellingen van het tandwiel pictogram rechtsboven in het partner centrum. Klik op de pagina gebruikers beheer in het tweede niveau van de linker navigatie balk. Klik op de vervolg keuzelijst met ' alle gebruikers ' in de rechter bovenhoek van de pagina en wijzig in ' globale beheerders '.
- De globale beheerder kan een nieuw gebruikers account maken in uw Azure AD-Tenant of toegang tot de gast gebruiker toewijzen aan de andere gebruikers van het domein account.
- Zodra de accounts zijn ingesteld voor alle PSC-beheer en-gebruikers, moet u zich aanmelden bij het partner centrum. Ga naar het tabblad Referral in het linkernavigatievenster en controleer of ze de pagina referrals kunnen zien.

Als uw bedrijf een PDM heeft: wanneer uw partner centrum-account is ingesteld en uw gebruikers over rollen en machtigingen beschikken, kunt u uw activiteiten naar het partner centrum verplaatsen. Informeer de PDM om de switch te laten wachten tot de deadline voor de migratie is voltooid, waardoor al uw nieuwe deals in het partner centrum kunnen stromen.
>[!Note]
>Zodra u deze switch hebt gemaakt, kunt u alleen op de bestaande actieve deals in PSC reageren. U kunt geen nieuwe deals maken en geen deals ontvangen van micro soft-verkopers in PSC.

Als uw bedrijf geen PDM heeft, moet u ervoor zorgen dat alle gebruikers accounts zijn ingesteld en geverifieerd door alle gebruikers. U wordt gewaarschuwd via een e-mail en een banner in PSC met betrekking tot de exacte datum waarop u in het partner centrum gezamenlijk kunt beginnen met verkopen. Houd er rekening mee dat u nog steeds de bestaande actieve deals in PSC moet beheren.

>[!Important]
>Actieve deals worden niet gemigreerd naar de PC. U hebt tot en met 31 december 2020 de deals te sluiten en te registreren.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Volgende stappen voor PSC-beheerders, PSC-deal managers en PSC-verkopers

Meer informatie over het samen verkopen in Partner Center.
Dit is een belang rijke stap, waarmee u wordt voor bereid op het samen verkopen van het partner centrum. Krijg inzicht in de werk stromen en de wijzigingen in Partner Center, zodat u effectief gezamenlijk kunt verkopen per dag. Lees eerst dit document. Er is ook een goede set resources beschikbaar in de [Galerie met ervaring voor gezamenlijk gebruik](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Belangrijkste verschillen tussen PSC-en PC-werk stromen

|**Scenario**|**Partner verkoop verbinding**|**Partnercentrum**|
|-----|:-----|:-----|
|Gebruikersrollen|PSC heeft beheerder, beheer van deals en verkopers rollen.|PC heeft alleen een rol voor [verwijzings beheerder](permissions-overview.md#manage-referrals) die lees-en schrijf machtigingen voor alle deals biedt.|
|Micro soft wordt uitgenodigd voor een mede verkochte deal|Gestart door micro soft-verkopers is er geen expliciete vraag naar een partner.|De partner moet een [expliciete aanvraag](manage-co-sell-opportunities.md#add-solutions) indienen als een micro soft-verkoper hulp nodig heeft voor een deal. De verkoper van micro soft heeft een optie om de aanvraag af te wijzen.|
|Vervaldatum|Er is geen concept van het verlopen van een deal.|Binnenkomende deals voor partners verlopen in 14 dagen als ze niet worden geaccepteerd door de partner. Hetzelfde geldt voor uitgaande deals van partners, waar ze in verlopen kunnen gaan als de verkoper van micro soft in 14 dagen geen actie onderneemt.|
|Micro soft-verkopers gegevens|Zichtbaar zodra een deal wordt gemaakt.|De verkopergegevens van micro soft worden alleen met de partner gedeeld als de verkoper de uitnodiging voor co-sell van de partner expliciet aanvaardt.|
|[Persoonlijke pijp lijn](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Niet beschikbaar.|Partners kunnen hun pijp lijn delen zonder dat ze zichtbaar zijn voor micro soft-verkopers.|
|Oplossingen|Oplossingen die tot slechts één prijs lijst behoren, kunnen worden toegevoegd aan een deal.|Partner kan [oplossingen](manage-co-sell-opportunities.md#add-solutions) toevoegen die deel uitmaken van de volgende lijsten. a) zijn oplossingen van de eerste partij van micro soft (vergelijkbaar met de rol Trans Action-deal in PSC) en c) oplossingen voor co-selling van andere partners van derden (vergelijkbaar met de functie ISV-deal in PSC).|
|Toewijzing van deals|Alleen toegewezen verkoper kan de deals bekijken en er actie op ondernemen.|Team leden kunnen worden toegevoegd aan een deal om de personen op te geven die aan een deal werken, maar er is geen blok kering van andere referentie beheerders om deze deals te bekijken of te verwerken.|
|Klant organisatie|Invoer van tekst in het vrije formulier.|U kunt de organisatie van de [klant](manage-co-sell-opportunities.md#select-your-customer) zoeken op basis van de [D&B-data base](https://www.dnb.com/) door slechts enkele tekens te typen. De juridische naam en het adres worden automatisch ingevuld op basis van de keuze.|
|Contact persoon van de klant|Niet verplicht.|Niet verplicht voor het delen van persoonlijke pijp lijnen. Vereist als de verkoper van micro soft is uitgenodigd om deel te nemen aan een mede-verkoop aanvraag.|
|Open bare API|Niet beschikbaar.|[Open bare API](/partner/develop/referrals) voor het programmatisch beheren van partner Center-verwijzingen.|

## <a name="psc-and-partner-center-field-mapping"></a>Toewijzing van PSC-en partner centrum velden

In deze sectie vindt u de exacte toewijzing van kenmerken tussen de PSC en het partner centrum. Elk scherm in PSC wordt vergeleken met de relevante weer gave in het gedeelte mogelijkheden voor co-sell in Partner Center. 

>[!Note]
>Volg de getallen op de gele bellen in de scherm afbeeldingen van PSC om het equivalente kenmerk in het partner centrum te vinden. De rode bellen geven aan dat de gearchiveerde niet beschikbaar is in het partner centrum.

**Start pagina van PSC en standaard weergave van de verkoop kansen in het partner centrum**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**Weer gave van een PSC-raster en de weer gave van het partner centrum**

- Er is geen lijst weergave in het partner centrum, zoals die van PSC.  Alle deals worden weer gegeven op basis van de laatst ontvangen of gemaakte datum met de klant gegevens en het type van de deal. De eerste deal in de weer gave is standaard geselecteerd. De meeste waarden die worden weer gegeven in de indeling van de PSC-tabel zijn beschikbaar in de detail weergave van de deal in de PC.
- De rol van deal is geen vereist veld in de PC. Deze wordt niet weer gegeven en niet vastgelegd in een van de werk stromen. Deze wordt automatisch afgeleid van de micro soft-verkoper, gebaseerd op de oplossingen die zijn toegevoegd aan de deal.
- De datum van laatste wijziging wordt niet weer gegeven op de pagina met referentie Details van de PC. Partners kunnen de sorteer functionaliteit gebruiken om de deals te sorteren op basis van de datum waarop het laatst is bijgewerkt.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**Weer gave Details van deal in PSC en partner Center**

- Partners kunnen een deal bewerken door te klikken op de knop bewerken in de detail weergave van de partner, (6). Nadat u op de knop bewerken hebt geklikt, kunt u alle velden bewerkbaar maken met de optie om de wijzigingen in de deal op te slaan of te annuleren.
- Er is geen optie voor het sluiten van de deal als duplicaat in partner centrum.
- Het resultaat van de klant is niet beschikbaar in het partner centrum. Alle informatie met betrekking tot klant interacties kan worden bijgewerkt in het gedeelte Notities van de PC.
- De geschatte Sluitings datum van de oplossing is alleen beschikbaar voor OEM IOT-deals in het partner centrum. Het wordt niet weer gegeven voor andere typen deals.
- Licentie programma is niet vereist op de PC. Het wordt automatisch uitgesteld op basis van de oplossingen die zijn geselecteerd in de deal.

>[!Note]
>Alle deals die zijn gemarkeerd als gewonnen of verloren kunnen niet worden bewerkt. Wees voorzichtig tijdens het verplaatsen van een deal naar een van deze Terminal statussen.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**De weer gave voor het toevoegen van producten en het partner centrum ' oplossingen toevoegen '**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**Gebruikers beheer in PSC en partner Center**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**Gebruikersrol toewijzing in PSC en partner centrum**

- De overeenkomstige rol voor de PSC-beheerder is de rol account beheerder in het partner centrum.
- Er is slechts één rol in het partner centrum voor het delen van het beheer van de verkoop. Dit is de rol van verwijzings beheerder.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

**Meldingen in PSC en partner centrum**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Overstappen van PSC naar partner Center: veelgestelde vragen

**Eerste. Wat moet ik doen als ik geen toegang heb tot het partner centrum?**

U kunt contact opnemen met uw beheerders die worden vermeld op de pagina ' geen toegang ' om de toegewezen rollen te krijgen. U hebt de rol '[verwijzings beheerder](permissions-overview.md#manage-referrals)' nodig voor lees-en schrijf machtigingen onder het gedeelte referrals. Als u alleen zakelijke profielen beheert, hebt u de rol ' bedrijfs profiel beheerder ' nodig in het partner centrum.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden." mag alleen worden gebruikt door de partners die zijn geregistreerd in het ISV Connect-programma voor het registreren van een deal zonder een bijbehorende verkoop kans in het partner centrum. Voor het registreren van deals met een verkoop kans wordt er een pop-upvenster weer gegeven wanneer de deal is gemarkeerd als gewonnen en als deze voldoet aan de criteria voor registratie van deals.

**Q9. Is het toevoegen van een klant organisatie verplicht?**

Ja, het toevoegen van een [klant organisatie](./manage-co-sell-opportunities.md#select-your-customer) is verplicht in het partner centrum. Eerst zoekt u naar de locatie waar de klant zich bevindt. Op basis van de details die u hebt. u kunt ook de exacte naam van het gebouw opgeven, of alleen informatie geven over de plaats. Met de zoek actie van de organisatie worden alle juridische entiteiten opgehaald die overeenkomen met de naam die u invoert, zodat u geen adres gegevens hoeft in te voeren. Alle details worden automatisch ingevuld op basis van de geselecteerde organisatie.

**Q10. Zijn de contact gegevens van de klant verplicht?**

Is afhankelijk van het [type deal](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) dat u maakt. Als u uw pijp lijn hebt gedeeld en geen hulp nodig hebt van de verkoop organisatie van micro soft, kunt u ervoor kiezen om geen contact gegevens van de klant te geven. Als je mede verkocht bent waar je momenteel hulp van micro soft-verkopers zoekt, moet je de contact gegevens van de klant opgeven. U moet een expliciete toestemming van de klant krijgen voordat u een aanvraag voor verkopen maakt in het partner centrum.

**Q11. Hoeveel oplossingen kan ik toevoegen aan een deal?**

U kunt Maxi maal 50 oplossingen (vergelijkbaar met ' Products ' in PSC) aan een deal toevoegen. In tegens telling tot PSC kunt u oplossingen combi neren van uw eigen oplossingen die in aanmerking komen voor de eerste partij, micro soft-Sku's en andere derden die in aanmerking komende oplossingen hebben. Er is geen rol van deals die in partner centrum moet worden geselecteerd of beschikbaar moeten zijn. Voor micro soft Sku's kunt u eventueel hoeveelheid en prijs toevoegen voor elke SKU die wordt toegevoegd aan de deal.

**Q12. Wanneer krijg ik meer informatie over de micro soft-verkopergegevens na het maken van een deal?**

Micro soft-verkopers worden alleen toegewezen nadat ze overeenkomen met de exacte Help vereisten die zijn opgegeven tijdens het maken van de deal met de relevante verkopers medewerker aan de kant van micro soft. Zelfs na toewijzing heeft micro soft-verkopers een optie om de uitnodiging voor co-sell te accepteren of af te wijzen. Alleen als een mede-verkoop uitnodiging wordt geaccepteerd door een verkoper, wordt de deal bijgewerkt met de contact gegevens van de verkoper van micro soft. De SLA voor verkopers van micro soft om op de deal te handelen is 14 dagen. Het is dezelfde SLA die partners nodig hebben om te reageren op de deal voordat deze de status verlopen heeft bereikt.

**Q13. Waar kan ik de opportuniteits-ID vinden?**

De kans-ID in PSC is hetzelfde als de deal-ID in de PC. U kunt de deal-ID naast de naam van de deal vinden wanneer u een wille keurige deal opent.

**Q14. Hoe kan mijn PDM toegang krijgen tot de PC?**

Het partner centrum is niet rechtstreeks toegankelijk via uw PDMs, zoals bij een PSC. Er zijn meerdere opties om die mogelijkheid in te scha kelen, zoals hieronder wordt vermeld.

- OCP Insights: als PDMs alleen de & deals bekijken die aan hen zijn gerelateerd, kunnen ze gebruikmaken van de OCP Insights-Portal om uw organisatie weergave te krijgen. Dit is een intern hulp programma dat alleen beschikbaar is voor PDMs. U ziet dat OCP Insights niet beschikbaar is voor de gebruikers van uw bedrijf.
- Gast gebruiker in Partner Center: u kunt uw PDM- @microsoft.com account toevoegen als gast gebruiker in Partner Center en hieraan een rol voor verwijzings beheerder toewijzen, zodat deze verwijzingen kunnen weer geven en er acties op worden uitgevoerd.
- Een [nieuwe gebruiker](./create-user-accounts-and-set-permissions.md#add-a-new-user) maken in uw Tenant: u kunt een nieuwe gebruiker maken in uw eigen Tenant en deze gegevens delen met de PDM, zodat ze kunnen worden weer gegeven en er kan worden gereageerd op verwijzingen die vergelijkbaar zijn met andere referral-gebruikers in uw account.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Resources die u helpen bij het maken en beheren van uw deals in Partner Center

Als u de Help-onderwerpen voor co-verkopen nog niet hebt gelezen, kunt u met de volgende resources deals beheren in Partner Center.

|**Om dit te doen**   |**Leest u**   |
|-----------------------|:-----------------------|
|Informatie over de tabbladen en navigatie op de pagina mogelijkheden voor co-verkoop|[Navigeren in de sectie co-sell](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Een klant organisatie selecteren in de lijst D&B |[Selecteer uw klant](./manage-co-sell-opportunities.md#select-your-customer)|
|De velden wijzigen in de sectie Details van deal|[Details van deal](./manage-co-sell-opportunities.md#deal-details)|
|Uw team leden toevoegen aan een deal team|[Uw werk nemers toevoegen](./manage-co-sell-opportunities.md#add-team-members)|
|Reageren op een mede verkochte deal|[Verkoop contracten beheren](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Deals registreren die u hebt gewonnen in het partner centrum |[Een nieuwe deal registreren](./register-deals.md)
|Verwijzings inzichten ophalen en nagaan hoe uw verwijzingen worden uitgevoerd |[Verwijzingsinzichten](./referral-insights.md)
|Een bedrijfs profiel maken en beheren|[Bedrijfsprofielen beheren](./create-a-marketing-profile.md)
|Leads voor uw bedrijfs profiel beheren |[Leads beheren](./manage-leads.md)|

## <a name="additional-resources"></a>Aanvullende bronnen

- [Partner Sales Connect to Partner Center](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -werkmap: werk boek om verkoop processen en-rollen van partners uit te lijnen met nieuwe verkoop processen via partner Center versus verkoop verbinding met partner.
- [Gebruiks richtlijnen](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) voor de IT-afdeling van partners: richt lijnen voor het identificeren van een besturings model via partner centrum voor het beheren van leads of het verkopen van verkoop kansen en het registreren van deals.
- [Dek over verwijzings beheer](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -gevisualiseerde stapsgewijze instructies voor het beheren van leads en verkoop kansen via partner centrum.
- [Publiceer en beheer in de](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) stapsgewijze instructie voor het maken, beheren en publiceren van aanbiedingen via het partner centrum in de commerciële Marketplace.
