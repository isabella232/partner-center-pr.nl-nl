---
title: Migreren vanaf partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe micro soft-partners kunnen migreren van partner Sales Connect (PSC) naar partner centrum en om deals te maken of te beheren die door micro soft-verkopers worden verzonden.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: bbd2d1035bdcde691b0db620949d0e973667627b
ms.sourcegitcommit: 351c7ff4e6ebbb615a00190b2310156381f9cf03
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/07/2020
ms.locfileid: "96776901"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Overzicht van het samen werken in Partner Center (PC) voor partners die worden gemigreerd vanuit partner Sales Connect (PSC)

**Juiste rollen**

- Accountbeheerder
- Beheerder van verwijzingen
- Partner Sales Connect (PSC)-verkoper
- Partner Sales Connect (PSC)-beheerder
- Manager van partner Sales Connect (PSC)

In dit artikel worden partners begeleid bij het migreren van partner Sales Connect naar het partner centrum, zodat ze gezamenlijk verkoop contracten kunnen blijven maken en beheren in het partner centrum.

Zoals u weet, zal uw bedrijf na 31 maart 2021 geen toegang meer hebben tot PSC. U kunt echter nog steeds alles vinden wat u in het partner centrum wilt doen, zoals het maken van trans acties voor de verkoop, het beheren van uw deals en het handelen op deals die door micro soft-verkopers naar u worden verzonden.

Er zijn echter ook verschillen. De volgende richt lijnen kunnen u helpen om uw overgang naar partner Center soepeler en eenvoudiger te maken.

>[!Important]
> Als u hier bent, omdat u een banner in PSC hebt gezien over de migratie, bent u op de juiste plaats. Deze hand leiding is niet van toepassing op de oplossings beoordeling (SA) en OEM IOT-partners die hun deals in PSC beheren.

## <a name="before-you-move-things-you-need-to-know"></a>Wat u moet weten voordat u verdergaat

### <a name="if-you-are-a-psc-admin"></a>Als u een PSC-beheerder bent

- U hebt een werk-e-mail nodig om u aan te melden bij het [partner centrum](https://partner.microsoft.com/).
- Stel uw account in met behulp van de [account beheerder](permissions-overview.md)van het partner centrum.
- Lees dit document voor meer informatie over het samen verkopen van het partner centrum.
- Stel gebruikers accounts in het partner centrum in voor al uw PSC-gebruikers (admin, deals Manager en verkopers rollen) en wijs ze toe aan [referentie beheerders rollen](permissions-overview.md).

>[!IMPORTANT]
> Zorg ervoor dat de MPN-ID die wordt weer gegeven in de banner PSC beschikbaar is in de lijst met MPN-locaties in het partner centrum.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-ID kunnen vinden.":::

 Als u wilt controleren of de MPN-ID wordt weer gegeven als een partner centrum MPN-locatie, meldt u zich aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum en selecteert u **instellingen** (het tandwiel pictogram) in de rechter bovenhoek van het scherm, gevolgd door **account instellingen**. Selecteer in het menu van het tweede niveau links navigeren **locaties** om de lijst met alle MPN-id's en locaties te zien die zijn gekoppeld aan het partner centrum-account.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Als u een PSC voor de deal Manager of verkoper bent

- U hebt een werk-e-mail nodig om u aan te melden bij het [dash board](https://partner.microsoft.com/dashboard)van de Partner Center.
- Als u een niet-werk account gebruikt in PSC of uw zakelijke e-mail adres is voor een ander bedrijf dan het partner bedrijf, neemt u contact op met uw PSC-beheerder voor meer informatie over het instellen van accounts.
- Neem contact op met uw PSC-beheerder als uw partner centrum-account is ingesteld, ongeacht het account dat u gebruikt om u aan te melden bij PSC.
- Controleer of u toegang hebt tot partner centrum en de sectie referrals.
- Lees dit document om inzicht te krijgen in de werk stromen en de wijzigingen in partner centrum.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als beheerder in PSC zijn dit de volgende stappen

Selecteer de optie **verwijzingen** in het navigatie menu van het partner centrum. Controleer of u toegang hebt tot de pagina's met verwijzingen.

  >[!Note]
  > Mogelijk moet u zich afmelden bij Partner Center en u vervolgens weer aanmelden om uw referenties voor toegang tot de pagina's met verwijzingen te vernieuwen.

Als de optie **verwijzingen** niet wordt weer geven in het menu van het partner centrum of aan de pagina met verwijzingen, neemt u contact op met de [account beheerder](permissions-overview.md) van uw bedrijf en vraagt u om u toegang te geven tot de opties voor **verwijzingen** en het bijbehorende gebied.

De account beheerder van uw bedrijf zoeken:

1. Selecteer **account instellingen** in het tandwiel pictogram rechtsboven in het dash board van de partner centrum.

1. Selecteer **gebruikers beheer** in het navigatie menu van het tweede niveau links.

1. Selecteer boven aan de lijst met gebruikers de vervolg keuzelijst **filter** . Wijzig de optie in **account beheerder**.

   Op de pagina worden alle account beheerders weer gegeven met hun respectieve e-mail adressen. E-mail een van de gebruikers en vraag hen om de beheerdersrol voor uw werk account toe te wijzen.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Afbeelding van de account beheerder op de pagina partner instellingen gebruikers beheer.":::

>[!Important]
>- Als uw rol alleen het beheer van gebruikers in PSC omvat, vraagt u de account beheerder van uw bedrijf om u de rol [account beheerder](permissions-overview.md#manage-mpn-membership-and-your-company) toe te wijzen in het partner centrum. 
>- Als uw rol ook mogelijkheden voor het beheren van co-verkoop omvat, moet u [de beheerdersrol](permissions-overview.md#manage-referrals) toewijzen.
> - Het is een goed idee om ook een lead voor veranderingen beheer te benoemen onder de PSC-beheerders. Als u dit doet, voor komt u dat alle PSC-beheerders afzonderlijk kunnen worden bereikt door account beheerders van het partner centrum. In plaats daarvan kan de lead voor veranderingen beheer de primaire persoon zijn die werkt met de account beheerder van het partner centrum.

## <a name="user-migration"></a>Gebruikers migratie

Nadat u uw account in partner centrum hebt ingesteld, gebruikt u de wizard Gebruikers migreren op de pagina verkoop kansen om het automatisch toe te wijzen van partner centrum rollen aan werk nemers van uw bedrijf.

>[!Note]
> Gebruikers migratie kan alleen worden uitgevoerd door [account beheerders](permissions-overview.md#manage-mpn-membership-and-your-company) van uw bedrijf. Als u de rol account beheerder niet hebt, kunt u een account beheerder vinden die u kan helpen bij het instellen van de gebruikers accounts met behulp van de wizard gebruikers migratie. De functionaliteit voor gebruikers migratie is vanaf 18 november 2020 beschikbaar.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Afbeelding van de wizard gebruikers migratie.":::

Account beheerders zien een koppeling van de wizard PSC-gebruikers migratie op de pagina mogelijkheden voor samen verkoop naast de hand leiding voor verwijzingen. Ze kunnen de gebruikers migratie initiëren door de koppeling te selecteren. Beheerders kunnen de koppeling selecteren om de gebruikers migratie te initiëren. Ze kunnen deze gebruikers migratie stap meerdere keren uitvoeren totdat alle gebruikers de juiste rollen hebben toegewezen in het partner centrum.

De tabel gebruikers migratie bevat de volgende details:

- Gebruikers account: e-mail-ID van de werk nemer
- PSC-partner account: het account waaraan de werk nemer is gekoppeld in PSC
- PSC-gebruikersrol: een van de drie rollen die zijn toegewezen aan in PSC.
- Locatie van de PC-MPN: de locatie waarvoor de gebruiker relevante PC-rollen krijgt. Het account van de PSC-partner MPN wordt gebruikt om de equivalente MPN locatie in het partner centrum te vinden om machtigingen toe te wijzen. De hele organisatie geeft de vOrg MPN-ID aan.
- PC-gebruikersrol: werk nemers krijgen rollen toegewezen op basis van hun PSC-gebruikers rollen. Aan de beheerder in PSC worden de beheerders rollen voor verwijzingen toegewezen in de PC. Aan de verkoper wordt de gebruikersrol referrals toegewezen in PC. Meer informatie over de PC-rollen en wat gebruikers met deze rollen in [Partner Center kunnen](permissions-overview.md#manage-referrals) doen
- PC AAD-Tenant-de Tenant waaraan de gebruikers zijn toegewezen in het partner centrum
- Status: er zijn drie mogelijke statussen van de migratie
    - **Niet gemigreerd** : er is geen PC-verwijzings functie toegewezen aan de gebruiker
    - **Gemigreerd** : de gebruiker is gemigreerd met de relevante rol die is toegewezen, zoals weer gegeven in de tabel
    - **Fout** -kan de migratie niet volt ooien omdat er een fout is opgetreden

Soms kan de migratie mislukken en resulteert dit in fouten. Hier volgen enkele redenen waarom een migratie een fout kan veroorzaken en een aantal manieren om het probleem op te lossen:

1. De PSC-gebruikers gebruiken mogelijk een niet-werk account.

2. De PSC-gebruiker maakt mogelijk gebruik van een account uit een ander domein dan dat u gebruikt in het partner centrum.

   Vraag de gebruiker zich aan te melden bij het partner centrum met hun werk account dat aan uw Azure AD-Tenant is gekoppeld om fouten met betrekking tot de scenario's 1 en 2 op te lossen. Uw [globale beheerder](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan u helpen.
   
   Uw globale beheerder vinden: 
   - Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard) van de partner centrum en selecteer **account instellingen** in het tandwiel pictogram in de rechter bovenhoek.
   - Selecteer **gebruikers beheer** op de navigatie balk links op het tweede niveau.
   - Selecteer boven aan de lijst met gebruikers de vervolg keuzelijst **filter** en wijzig de optie in **globale beheerder**. Op de pagina worden vervolgens alle globale beheerders weer gegeven met hun respectievelijke e-mail adressen. Vraag een van hen om de rol van verwijzings beheerder voor uw werk account toe te wijzen.
   
      De globale beheerder kan een nieuw gebruikers account maken in uw Azure AD-Tenant of toegang tot de gast gebruiker toewijzen aan de andere gebruikers van het domein account. Zodra de accounts voor alle PSC-deal managers en-gebruikers zijn ingesteld, moeten ze zich aanmelden bij het partner centrum, **verwijzingen** selecteren in het navigatie menu en bevestigen dat ze de pagina met verwijzingen kunnen zien.

3. De gebruiker heeft al een referral-rol toegewezen in het partner centrum.
    - U kunt de bestaande rol van de gebruiker controleren. Selecteer in de rechter bovenhoek van partner Center **instellingen** (het tandwiel pictogram) en vervolgens de **account instellingen**. Wanneer u een tweede navigatie menu ziet, selecteert u **gebruikers beheer** en zoekt u naar de gebruiker.

Nadat u de gebruikers migratie hebt voltooid, gebruikt u de volgende richt lijnen om de migratie strategie te bepalen:

Als uw bedrijf een partner Development Manager (PDM) heeft: wanneer uw partner centrum-account is ingesteld en uw gebruikers over rollen en machtigingen beschikken, kunt u uw activiteiten naar het partner centrum verplaatsen. Informeer de PDM om de switch te laten wachten tot de deadline voor de migratie is voltooid, waardoor al uw nieuwe deals in het partner centrum kunnen stromen.

>[!Note]
>Zodra u deze switch hebt gemaakt, kunt u alleen op de bestaande actieve deals in PSC reageren. U kunt geen nieuwe deals maken en geen deals ontvangen van micro soft-verkopers in PSC.

Als uw bedrijf geen PDM heeft, moet u ervoor zorgen dat alle gebruikers accounts zijn ingesteld en geverifieerd door alle gebruikers. U wordt gewaarschuwd via een e-mail en een banner in PSC met betrekking tot de exacte datum waarop u in het partner centrum gezamenlijk kunt beginnen met verkopen. Houd er rekening mee dat u nog steeds de bestaande actieve deals in PSC moet beheren.

>[!Important]
>Actieve deals worden niet gemigreerd naar de PC. U hebt tot 31 maart 2021 de deals te sluiten en te registreren.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Volgende stappen voor PSC-beheerders, PSC-deal managers en PSC-verkopers

Meer informatie over het samen verkopen in Partner Center.
Dit is een belang rijke stap, waarmee u wordt voor bereid op het samen verkopen van het partner centrum. Krijg inzicht in de werk stromen en de wijzigingen in Partner Center zodat u meteen direct kunt verkopen. Lees eerst dit document. Er is ook een goede set resources beschikbaar in de [Galerie met ervaring voor gezamenlijk gebruik](https://aka.ms/cosellexperience).

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

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>De velden in PSC toewijzen aan de overeenkomende velden in het partner centrum

In deze sectie worden de geselecteerde scherm opnamen die worden weer gegeven voor PSC, vergeleken met de overeenkomende weer gave in de sectie verkoop kansen voor het partner centrum.

U ziet genummerde, gele of rode cirkels op elk paar scherm opnamen:

- **Wat betekenen de gele cirkels?** Genummerde, gele cirkels worden eerst op elke PSC-scherm afbeelding weer gegeven. Vervolgens vindt u een scherm opname van het Companion-partner centrum dat veel van dezelfde getallen bevat.

   Als u wilt zien hoe elk veld of kenmerk in PSC wordt toegewezen aan de tegen hanger in het partner centrum, moet u de genummerde cirkels combi neren in de twee gerelateerde scherm afbeeldingen. U kunt bijvoorbeeld het genummerde, gele ' 1 ' in de eerste, PSC-scherm afbeelding, de genummerde, gele ' 1 ' in de tweede, afbeelding van het partner centrum eronder, vergelijken.

- **Wat betekent een rode cirkel?** Als er een rode cirkel op één scherm afbeelding wordt weer gegeven, betekent dit dat het PSC-veld niet beschikbaar is in het partner centrum.

De veld toewijzingen van het programma PSC-to-Partner Center worden weer gegeven voor de volgende gebieden:

1. Start pagina van PSC toegewezen aan de standaard weergave voor de verkoop kansen van het partner centrum
1. Weer gave van een PSC-raster dat is gekoppeld aan de deal weergave van het partner centrum
1. Details van de weer gave van de PSC-deal die is toegewezen aan de Partner Center-detail weergave Details
1. Aan het partner centrum gekoppelde product weergave toevoegen
1. Weer gave voor PSC-gebruikers beheer toegewezen aan de gebruikers beheer weergave van het partner centrum
1. Toewijzings weergave van de PSC-gebruikersrol toegewezen aan de weer gave van de roltoewijzing van de Partner Center
1. Weer gave van PSC-meldingen die is toegewezen aan de weer gave meldingen in het partner centrum

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-start pagina van PSC toegewezen aan de standaard weergave voor de verkoop kansen van het partner centrum

Vergelijk de overeenkomende, genummerde cirkels tussen de bovenste PSC-scherm afbeelding en de screen shot van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend Partner Center-veld is.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Afbeelding met de veld Toewijzingen tussen de start pagina van partner Sales Connect en de standaard weergave van verkoop kansen in het partner centrum." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2: de raster weergave van een PSC die is toegewezen aan de deal weergave van het partner centrum

Vergelijk de overeenkomende, genummerde cirkels tussen de bovenste PSC-scherm afbeelding en de screen shot van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend Partner Center-veld is.  

> [!NOTE]
> Andere overwegingen worden weer gegeven onder de scherm opnamen.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Afbeelding met de veld Toewijzingen tussen de weer gave van de partner Sales Connect (PSC) en de deal weergave van het partner centrum." lightbox="images/pscmigration/grid-view-expanded.png":::

**Speciale overwegingen:**

- Er is geen lijst weergave in het partner centrum, zoals die van PSC.  Alle deals worden weer gegeven op basis van de laatst ontvangen of gemaakte datum met de klant gegevens en het type van de deal. De eerste deal in de weer gave is standaard geselecteerd. De meeste waarden die worden weer gegeven in de indeling van de PSC-tabel zijn beschikbaar in de detail weergave van de deal in de PC.
- De rol van deal is geen vereist veld in de PC. Het wordt niet weer gegeven of vastgelegd in een van de werk stromen. Deze wordt automatisch afgeleid van de micro soft-verkoper, gebaseerd op de oplossingen die zijn toegevoegd aan de deal.
- De datum van laatste wijziging wordt niet weer gegeven op de pagina met referentie Details van de PC. Partners kunnen de sorteer functionaliteit gebruiken om de deals te sorteren op basis van de datum waarop het laatst is bijgewerkt.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-de weer gave met details van de PSC-deal die is toegewezen aan het partner centrum

Vergelijk de overeenkomende, genummerde cirkels op de bovenste scherm opname met de scherm afbeelding van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend veld of gebied in het partner centrum is.

> [!NOTE]
> Andere overwegingen worden weer gegeven onder de scherm opnamen.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Afbeelding met de veld Toewijzingen tussen de weer gave Details van de partner Sales Connect (PSC) en de weer gave Details van het partner centrum." lightbox="images/pscmigration/deal-details-expanded.png":::

**Speciale overwegingen:**

- Partners kunnen een deal bewerken door de knop bewerken te selecteren in de detail weergave van de partner (6). Zodra de knop bewerken is geselecteerd, worden alle velden bewerkbaar. U hebt de mogelijkheid om de wijzigingen in de deal op te slaan of te annuleren.
- Er is geen optie voor het sluiten van de deal als duplicaat in partner centrum.
- Het resultaat van de klant is niet beschikbaar in het partner centrum. Alle informatie met betrekking tot klant interacties kan worden bijgewerkt in het gedeelte Notities van de PC.
- De geschatte Sluitings datum van de oplossing is alleen beschikbaar voor OEM IOT-deals in het partner centrum. Deze informatie wordt niet weer gegeven voor andere typen deals.
- Licentie programma is niet vereist op de PC. Deze informatie wordt automatisch uitgesteld op basis van de oplossingen die zijn geselecteerd in de deal.

>[!Note]
>Een deal die is gemarkeerd als gewonnen of verloren kan later niet worden bewerkt. Wees voorzichtig tijdens het verplaatsen van een deal naar een van deze Terminal statussen.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-weer gave producten toevoegen aan de weer gave oplossingen toevoegen van het partner centrum

Vergelijk de overeenkomende, genummerde cirkels op de bovenste scherm opname met de scherm afbeelding van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend veld of gebied in het partner centrum is.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Afbeelding van de veld Toewijzingen tussen de weer gave partner Sales Connect (PSC) voor het toevoegen van producten en de weer gave oplossingen toevoegen aan partner centrum." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-gebruikers beheer in PSC versus partner centrum

Vergelijk de overeenkomende, genummerde cirkels op de bovenste scherm opname met de scherm afbeelding van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend veld of gebied in het partner centrum is.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Afbeelding van de weer gave van de veld Toewijzingen tussen de partner Sales Connect (PSC) User Management Home en de pagina weergave van het partner centrum-gebruikers beheer in het gebied account instellingen."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-gebruikersrol toewijzing in PSC versus partner centrum

Vergelijk de overeenkomende, genummerde cirkels op de bovenste scherm opname met de scherm afbeelding van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend veld of gebied in het partner centrum is.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Afbeelding van de veld Toewijzingen tussen de toewijzings weergave van de rol partner Sales Connect (PSC) en de weer gave van de roltoewijzing van de Partner Center." lightbox="images/pscmigration/roles-expanded.png":::

**Speciale overwegingen:**

- De overeenkomstige rol voor de PSC-beheerder is de rol account beheerder in het partner centrum.
- Er is slechts één rol in het partner centrum voor het beheer van de verkoop van trans acties. Deze rol is de rol van verwijzings beheerder.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-meldingen in PSC versus partner centrum

Vergelijk de overeenkomende, genummerde cirkels op de bovenste scherm opname met de scherm afbeelding van het partner centrum eronder. Overeenkomende aantallen geven aan waar u de aan de PSC gerelateerde functie of het kenmerk kunt vinden in het partner centrum. Rode cirkels geven aan dat er geen overeenkomend veld of gebied in het partner centrum is.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Afbeelding van de toewijzing tussen de PSC-meldingen (partner Sales Connect) en de weer gave meldingen in het partner centrum."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Overstappen van PSC naar partner Center: veelgestelde vragen

De volgende secties beantwoorden Veelgestelde vragen over de migratie.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1: wat moet ik doen als ik geen toegang heb tot het partner centrum?

U kunt contact opnemen met uw beheerders die worden vermeld op de pagina ' geen toegang ' om de toegewezen rollen te krijgen. U hebt de rol van [verwijzings beheerder](permissions-overview.md#manage-referrals) nodig voor lees-en schrijf machtigingen onder het gedeelte referrals. Als u alleen zakelijke profielen beheert, hebt u de rol bedrijfs profiel beheerder nodig in het partner centrum.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Afbeelding van de ervaring van geen toegang in het partner centrum.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-wie kan me toegang verlenen tot de sectie referrals in Partner Center?

Uw [account beheerder](permissions-overview.md#manage-mpn-membership-and-your-company) kan u toegang verlenen tot het tabblad verwijzingen. Als u uw account beheerder wilt vinden, selecteert u **account instellingen** in het tandwiel pictogram rechtsboven in het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum. Selecteer vervolgens **gebruikers beheer** op de navigatie balk links op het tweede niveau. Selecteer boven aan de lijst met gebruikers de vervolg keuzelijst **filter** en wijzig de optie in **account beheerder**. Op de pagina worden alle account beheerders weer gegeven met hun respectieve e-mail adressen. Vraag een van hen om de rol van verwijzings beheerder voor uw werk account toe te wijzen.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-de knop + nieuwe deal is voor ons account grijs weer gegeven. Wat moet ik doen om te beginnen met het maken van deals?

Dit gebeurt alleen als er geen oplossingen voor samen verkoop zijn gekoppeld aan de MPN-organisatie die u in partner centrum gebruikt. Neem contact op met uw PDM om de MPN-ID van uw oplossingen te corrigeren of een ondersteunings ticket te maken waarin het probleem wordt vermeld.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4: kan ik deals toewijzen aan een specifieke persoon van onze organisatie, zoals een PSC?

U kunt team leden toewijzen aan een specifieke deal. Het blokkeert niet dat andere referentie beheerders deze deals kunnen bekijken of ermee handelen.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-is er een overzicht van alle aan mij toegewezen deals?

U kunt de functie Favorieten gebruiken. Dit is een tabblad op gebruikers niveau. U kunt alle deals markeren die aan u zijn toegewezen als favorieten om snel toegang te krijgen tot de deals.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-is er een weer gave met het kenmerk alleen-lezen voor de deals?

Nee, er is geen weer gave met het kenmerk alleen-lezen van de deals in het gedeelte referrals. Alle referentie beheerders hebben volledige lees-en schrijf toegang tot alle deals.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-Hoe kan ik een deal registreren nadat deze is gemarkeerd als binnengehaald?

Als de deal aan de onderstaande criteria voldoet, wordt er een pop-up weer gegeven om de [registratie van deals](./register-deals.md)te starten.

- Er is een stimulans die in aanmerking komt voor een oplossing die aan de deal is gekoppeld.
- De verkoper van micro soft wordt uitgenodigd om deel te nemen aan de deal of u hebt aan de deal uitgenodigd.
- Micro soft Card heeft de status geaccepteerd of gewonnen in het partner centrum.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8: er verschijnt een fout bericht wanneer ik de knop + nieuwe deal registratie Selecteer in de sectie deals registratie. Hoe kan ik mijn deals registreren?

De knop **+ nieuwe deal registratie** wordt alleen gebruikt door de partners die zijn geregistreerd in het ISV Connect-programma voor het registreren van een deal zonder een bijbehorende verkoop kans in het partner centrum. Voor het registreren van deals met een verkoop kans wordt er een pop-upvenster weer gegeven wanneer de deal is gemarkeerd als gewonnen en als deze voldoet aan de criteria voor registratie van deals.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-een klant organisatie toevoegen verplicht?

Ja, het toevoegen van een [klant organisatie](./manage-co-sell-opportunities.md#select-your-customer) is verplicht in het partner centrum. Eerst zoekt u naar de locatie waar de klant zich bevindt. Op basis van de details die u hebt. u kunt ook de exacte naam van het gebouw opgeven, of alleen informatie geven over de plaats. Met de zoek actie van de organisatie worden alle juridische entiteiten opgehaald die overeenkomen met de naam die u invoert, zodat u geen adres gegevens hoeft in te voeren. Alle details worden automatisch ingevuld op basis van de geselecteerde organisatie.

### <a name="10---are-customer-contact-details-mandatory"></a>10-zijn contact gegevens van de klant verplicht?

Is afhankelijk van het [type deal](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) dat u maakt. Als u uw pijp lijn hebt gedeeld en geen hulp nodig hebt van de verkoop organisatie van micro soft, kunt u ervoor kiezen om geen contact gegevens van de klant te geven. Als je mede verkocht bent waar je momenteel hulp van micro soft-verkopers zoekt, moet je de contact gegevens van de klant opgeven. U moet een expliciete toestemming van de klant krijgen voordat u een aanvraag voor verkopen maakt in het partner centrum.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-hoeveel oplossingen kan ik aan een deal toevoegen?

U kunt Maxi maal 50 oplossingen (vergelijkbaar met ' Products ' in PSC) aan een deal toevoegen. In tegens telling tot PSC kunt u oplossingen combi neren van uw eigen oplossingen die in aanmerking komen voor de eerste partij, micro soft-Sku's en andere derden die in aanmerking komende oplossingen hebben. Er is geen rol van deals die in partner centrum moet worden geselecteerd of beschikbaar moeten zijn. Voor micro soft Sku's kunt u eventueel hoeveelheid en prijs toevoegen voor elke SKU die wordt toegevoegd aan de deal.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12: Wanneer krijg ik meer informatie over de micro soft-verkopergegevens na het maken van een deal?

Micro soft-verkopers worden alleen toegewezen nadat ze overeenkomen met de exacte Help vereisten die zijn opgegeven tijdens het maken van de deal met de relevante verkopers medewerker aan de kant van micro soft. Zelfs na toewijzing heeft micro soft-verkopers een optie om de uitnodiging voor co-sell te accepteren of af te wijzen. Alleen als een mede-verkoop uitnodiging wordt geaccepteerd door een verkoper, wordt de deal bijgewerkt met de contact gegevens van de verkoper van micro soft. De SLA voor verkopers van micro soft om op de deal te handelen is 14 dagen. Het is dezelfde SLA die partners nodig hebben om te reageren op de deal voordat deze de status verlopen heeft bereikt.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-waar vind ik de opportuniteits-ID?

De kans-ID in PSC is hetzelfde als de deal-ID in de PC. U kunt de deal-ID naast de naam van de deal vinden wanneer u een wille keurige deal opent.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-Hoe kan mijn PDM toegang krijgen tot de PC?

Het partner centrum is niet rechtstreeks toegankelijk via uw PDMs, zoals bij een PSC. Er zijn meerdere opties om die mogelijkheid in te scha kelen, zoals hieronder wordt vermeld.

- OCP Insights: als PDMs alleen de deals en de voortgang die eraan zijn gerelateerd weer geven, kunnen ze gebruikmaken van de OCP Insights-Portal om uw organisatie weergave te krijgen. Dit is een intern hulp programma dat alleen beschikbaar is voor PDMs. U ziet dat OCP Insights niet beschikbaar is voor de gebruikers van uw bedrijf.
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

## <a name="next-steps"></a>Volgende stappen

Volg deze aanvullende bronnen:

- [Partner Sales Connect to Partner Center](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -werkmap: werk boek om verkoop processen en-rollen van partners uit te lijnen met nieuwe verkoop processen via partner Center versus verkoop verbinding met partner.
- [Gebruiks richtlijnen](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) voor de IT-afdeling van partners: richt lijnen voor het identificeren van een besturings model via partner centrum voor het beheren van leads of het verkopen van verkoop kansen en het registreren van deals.
- [Dek over verwijzings beheer](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -gevisualiseerde stapsgewijze instructies voor het beheren van leads en verkoop kansen via partner centrum.
- [Publiceer en beheer in de](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) stapsgewijze instructie voor het maken, beheren en publiceren van aanbiedingen via het partner centrum in de commerciële Marketplace.