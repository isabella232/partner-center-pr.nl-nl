---
title: Migratie van Partner Sales Verbinding maken (PSC) voor IOT-partners
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Meer informatie over hoe Microsoft IOT-partners kunnen migreren van Partner Sales Verbinding maken (PSC) naar Partner Center maken of beheren van deals.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/07/2021
ms.openlocfilehash: 1850ffe388349cdb7e4c685e5db0004d74735e80
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101647"
---
# <a name="guide-to-create-and-manage-iot-deals-in-partner-center-pc-for-iot-partners-migrating-from-partner-sales-connect-psc"></a>Handleiding voor het maken en beheren van IOT-deals in Partner Center (PC) voor IOT-partners die migreren vanuit Partner Sales Verbinding maken (PSC)

**Juiste rollen:** Accountbeheerder | Beheerdersrechten voor verwijzingen | Verkoper-Verbinding maken (PSC) van partnerverkoop | Partner Sales Verbinding maken (PSC) admin | Partner Sales Verbinding maken (PSC) deal manager

In dit artikel vindt u richtlijnen voor IOT-partners die migreren van Partner Sales Verbinding maken (PSC) naar Partner Center (PC), zodat ze deals kunnen blijven maken en beheren in Partner Center.

>[!Note]
> Deze handleiding is **alleen van toepassing voor IOT-zakelijke partners die** hun deals beheren in PSC.

>[!Important]
> Vanaf 15 augustus 2021 kan uw bedrijf geen deals maken of bewerken in PSC. **U kunt de bestaande deals nog steeds downloaden met behulp van de bulkexportfunctie in PSC. U kunt ook [openstaande deals migreren van](partner-sales-connect-to-partner-center-iot.md#psc-deals-migration) PSC naar Partner Center na deze datum.**

Zoals u weet, **heeft uw bedrijf na 30 augustus 2021** geen toegang meer tot PSC. U vindt echter nog steeds alles wat u wilt doen in Partner Center, zoals het maken en beheren van deals.

Er zijn echter wel verschillen. De volgende richtlijnen kunnen u helpen uw overgang naar Partner Center soepeler en eenvoudiger te maken.

## <a name="before-you-move-things-you-need-to-know"></a>Voordat u overstapt, moet u weten wat u moet weten

### <a name="if-you-are-a-psc-admin"></a>Als u een PSC-beheerder bent

- U hebt een e-mailadres van uw werk nodig om u aan te [melden bij Partner Center.](https://partner.microsoft.com/)
- Stel uw account in met behulp van Partner Center [accountbeheerder](permissions-overview.md).
- Meer informatie over het maken en beheren van IOT-deals in Partner Center u dit document leest.
- Stel gebruikersaccounts in Partner Center voor al uw PSC-gebruikers (beheerders-, dealbeheer- en verkoperrollen) en wijs ze de gebruikersrollen verwijzingsbeheerder of [verwijzingsgebruikers toe.](permissions-overview.md)

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Als u een PSC-dealmanager of verkoper bent

- U hebt een e-mailadres van uw werk nodig om u aan te melden bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)
- Als u een niet-werkaccount in PSC gebruikt of als uw werk-e-mailadres voor een ander bedrijf is dan het partnerbedrijf, neem dan contact op met uw PSC-beheerder voor hulp bij het instellen van het account.
- Neem contact op met uw PSC-beheerder Partner Center account is ingesteld, ongeacht het account dat u gebruikt om u aan te melden bij PSC.
- Controleer of u toegang hebt tot Partner Center en de sectie Verwijzingen.
- Lees dit document voor meer informatie over de werkstromen en de wijzigingen in Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als beheerder in PSC zijn dit de volgende stappen

Selecteer in Partner Center linkernavigatiemenu de **optie** Verwijzingen. Controleer of u toegang hebt tot de pagina Kansen voor co-verkoop.

  >[!Note]
  > Mogelijk moet u zich bij de Partner Center aanmelden om uw referenties te vernieuwen voor toegang tot de verwijzingenpagina's.

**Als** u de optie  Verwijzingen niet ziet in het Partner Center-menu of de pagina's met betrekking tot verwijzingen, neem dan contact op met de [accountbeheerder](permissions-overview.md) van uw bedrijf en vraag deze om u toegang te geven tot de optie Verwijzingen en het bijbehorende gebied.

De accountbeheerder van uw bedrijf zoeken:

1. Selecteer **Accountinstellingen** in het tandwielpictogram rechtsboven in Partner Center dashboard.

1. Selecteer **Gebruikersbeheer in** het navigatiemenu aan de linkerkant op het tweede niveau.

1. Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst** Filter. Wijzig de optie in **Accountbeheerder**.

   Op de pagina worden alle accountbeheerders met hun respectieve e-mailadressen weergegeven. Stuur een e-mail naar een van deze en vraag deze om de beheerdersrol verwijzingen toe te wijzen voor uw werkaccount.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Afbeelding van de accountbeheerders op de pagina Gebruikersbeheer van partnerinstellingen.":::

>[!Important]
>- Als uw rol alleen betrekking heeft op het beheren van gebruikers in PSC, vraagt u de accountbeheerder van uw bedrijf u de [rol van accountbeheerder](permissions-overview.md#manage-mpn-membership-and-your-company) toe te wijzen in Partner Center volgens het beleid van uw bedrijf.
>- Als uw rol ook het beheren van ioT-deals omvat, vraagt u om waar nodig de gebruikersrol verwijzingenbeheerder of verwijzingen toegewezen te krijgen. [](permissions-overview.md#manage-referrals)
> - Het is een goed idee om ook één lead voor wijzigingsbeheer te benoemen onder de PSC-beheerders. Zo voorkomt u dat alle PSC-beheerders afzonderlijk contact moeten maken met Partner Center accountbeheerders. In plaats daarvan kan de lead voor wijzigingsbeheer de primaire persoon zijn die met de Partner Center accountbeheerder werkt.

## <a name="user-migration"></a>Gebruikersmigratie

Nadat u uw account in Partner Center hebt ingesteld, gebruikt u de wizard gebruikersmigratie op de pagina verkoopkansen om automatisch Partner Center-rollen toe te wijzen aan werknemers van uw bedrijf.

>[!Note]
> Gebruikersmigratie kan alleen worden uitgevoerd door [accountbeheerders](permissions-overview.md#manage-mpn-membership-and-your-company) van uw bedrijf. Als u niet de rol van accountbeheerder hebt, zoek dan een accountbeheerder die u kan helpen bij het instellen van de gebruikersaccounts met behulp van de wizard gebruikersmigratie.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Afbeelding van de wizard gebruikersmigratie.":::

Accountbeheerders zien een koppeling naar de wizard PSC-gebruikersmigratie op de pagina verkoopkansen naast de handleiding voor verwijzingen. Ze kunnen de gebruikersmigratie initiëren door de koppeling te selecteren. Beheerders kunnen de koppeling selecteren om de gebruikersmigratie te starten. Ze kunnen deze gebruikersmigratiestap meerdere keren uitvoeren totdat aan alle gebruikers de juiste rollen zijn toegewezen in Partner Center.

De gebruikersmigratietabel heeft de volgende details:

- Gebruikersaccount: e-mail-id van de werknemer
- PSC-partneraccount: het account waaraan de werknemer is gekoppeld in PSC
- PSC-gebruikersrol: een van de drie rollen die zijn toegewezen in PSC.
- PC MPN-locatie: de locatie waarvoor de gebruiker relevante Partner Center (PC)-rollen krijgt. Het MPN van het PSC-partneraccount wordt gebruikt om de equivalente MPN-locatie in de Partner Center om machtigingen toe te wijzen. De hele organisatie geeft de MPN-id van de vOrg aan.
- Pc-gebruikersrol: aan werknemers worden rollen toegewezen op basis van hun PSC-gebruikersrollen. Beheerders in PSC krijgen de beheerdersrollen Verwijzingen toegewezen in Partner Center. Aan de verkoper wordt de gebruikersrol verwijzingen toegewezen in Partner Center. Meer informatie over de Partner Center rollen en wat gebruikers met deze rollen kunnen doen in Partner Center [hier](permissions-overview.md#manage-referrals)
- PC AAD-tenant: de Microsoft Azure Active Directory (Azure AD)-tenant waaraan de gebruikers zijn toegewezen in Partner Center
- Status: er zijn drie mogelijke statussen voor de status van de migratie
    - **Niet gemigreerd:** de gebruiker heeft geen Partner Center toegewezen aan verwijzingen
    - **Gemigreerd:** de gebruiker is gemigreerd en de relevante rol is toegewezen, zoals wordt weergegeven in de tabel
    - **Fout:** de migratie kan niet worden voltooid vanwege een fout

Soms kan de migratie mislukken en leiden tot fouten. Hier zijn enkele redenen waarom een migratie een fout kan veroorzaken en enkele manieren om het probleem op te lossen:

1. De PSC-gebruikers gebruiken mogelijk een niet-werkaccount.

2. De PSC-gebruiker gebruikt mogelijk een account uit een ander domein dan het account dat u in de Partner Center.

   Als u fouten met betrekking tot scenario 1 en 2 wilt oplossen, vraagt u de gebruiker om zich aan te melden bij Partner Center met behulp van het werkaccount dat is gekoppeld aan uw Azure AD-tenant. Uw [globale beheerder](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan u helpen.
   
   Uw globale beheerder zoeken: 
   1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard) selecteer **Accountinstellingen** in het tandwielpictogram rechtsboven.
   2. Selecteer **Gebruikersbeheer** in de linkernavigatiebalk op het tweede niveau.
   3. Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst Filter** en wijzig de optie in **Globale beheerder.** Op de pagina worden vervolgens alle globale beheerders met hun respectieve e-mailadressen weergegeven. Vraag een van deze om de rol van verwijzingsbeheerder voor uw werkaccount toe te wijzen.
   
      De globale beheerder kan een nieuw gebruikersaccount maken in uw Azure AD-tenant of gastgebruikerstoegang toewijzen aan de andere domeinaccountgebruikers. Zodra de accounts zijn ingesteld voor alle PSC-dealmanagers en -gebruikers, moeten  ze zich aanmelden bij Partner Center, Verwijzingen selecteren in het navigatiemenu aan de linkerkant en bevestigen dat ze de pagina Verwijzingen kunnen zien.

3. De gebruiker heeft al een verwijzingsrol toegewezen in Partner Center.
    - U kunt de bestaande rol van de gebruiker controleren. Selecteer in de rechterbovenhoek Partner Center de **Instellingen** (het tandwielpictogram) en vervolgens **Accountinstellingen.** Wanneer u een tweede linkernavigatiemenu ziet, selecteert u **Gebruikersbeheer en** zoekt u naar de gebruiker.

## <a name="psc-deals-migration"></a>Migratie van PSC-deals

Nadat u de gebruikersmigratie hebt voltooid, gebruikt u de wizard dealsmigratie op de pagina verkoopkansen om alle in aanmerking komende openstaande deals van PSC naar een Partner Center. **De migratiekoppeling naar deals is alleen zichtbaar voor de verwijzingsbeheerders met het volledige organisatiebereik in Partner Center.** Rechtsboven op de pagina Collectieve verkoopkansen verschijnt een koppeling met de naam **PSC-dealmigratie**. Hiermee wordt de wizard Dealmigratie geopend.

Lees deze sectie voordat u begint met de dealmigratie.

**Komt in aanmerking voor migratie**

Slechts enkele deals komen in aanmerking voor migratie van PSC naar Partner Center. Deze migratiewizard is gebouwd om partners te helpen hun deals te Partner Center waar ze nog steeds actief samenwerken met hun klanten om de deal te sluiten. **Alleen deals met een open status die zijn gemaakt op 1 januari 2020 met geldige partneraccountgegevens (geldige MPN-id) komen in aanmerking voor migratie.**

## <a name="pre-requisites-for-deal-migration"></a>Vereisten voor dealmigratie

Voordat u begint met de dealmigratie Partner Center, volgt u de onderstaande instructies om de deals in PSC in te stellen voor een geslaagde migratie.

- Alle leden van het verkoopteam in uw bedrijf die aan de openstaande deals werken, worden op de hoogte gesteld van deze migratie.
- De leden van het verkoopteam zijn getraind om Partner Center te gebruiken voor dealbeheer.
- De deals bevatten alle vereiste informatie, zoals hieronder wordt beschreven.
    - Bedrijfsgegevens van klant, inclusief naam en adres
    - Ten minste één oplossing
    - Ten minste één teamlid met alle details: voornaam, achternaam, e-mail-id en telefoonnummer
    - Dealwaarde
    - Geschatte einddatum deal
    - Partnernotities

U kunt de mogelijkheden voor bulksgewijs downloaden en uploaden in PSC gebruiken om alle ontbrekende details in de deal toe te voegen voor alle in aanmerking komende deals.

>[!Note]
> De dealmigratie slaagt zelfs als niet aan de bovenstaande vereisten wordt voldaan. U kunt de status van de deal echter niet wijzigen als een van de hierboven genoemde vereiste velden in Partner Center niet beschikbaar zijn. Vervolgens moet u alle vereiste gegevens invoeren die ontbreken in de deals in Partner Center u gewenste gegevens kunt gaan gebruiken. **Het wordt ten zeerste aangeraden om de in aanmerking komende deals in PSC op te schonen voordat u deze migreert naar Partner Center.**

De dealmigratie in Partner Center is gebouwd als een ervaring met één klik. U hoeft alleen maar op de knop Deals **migreren te klikken** zodra uw bedrijf klaar is om de in aanmerking komende deals te migreren. **U kunt de deals die u wilt migreren vanuit PSC niet kiezen. Als u geen deals wilt migreren naar Partner Center, verplaatst u deze naar de gesloten status in PSC voordat u de migratie start.**

>[!Note]
> Nadat de migratie is geïnitieerd, kan het tot 24 uur duren voordat **de deals zijn gemigreerd.**

Zodra de migratie is voltooid, is de status van het bannerbericht gewijzigd, met een koppeling naar het migratierapport. Download het rapport om de details weer te geven van deals die zijn gemigreerd van PSC naar Partner Center.

Het rapport bevat de onderstaande details.

- **Partner Center engagement-id:** de unieke id in Partner Center voor alle deals in een overeenkomst. Er zijn twee deals: één voor de partner en één voor Microsoft bij een overeenkomst voor co-verkoop in Partner Center.
- **Partner Center verwijzings-id:** de unieke id in Partner Center voor de deal die bij de partner hoort.
- **Dealnaam:** id die is opgegeven voor de deal in PSC.
- **PSC-deal-id:** de unieke id in PSC voor de deal.
- **Fouten:** om aan te geven of er een fout is opgetreden tijdens het migreren van een specifieke deal.

Alle deals die zijn gemigreerd, zijn niet zichtbaar in PSC. U kunt blijven werken aan de gemigreerde deals in Partner Center.

Deals die zijn gemigreerd vanuit PSC zijn beschikbaar op het tabblad Uitgaand van de pagina Verkoopkansen voor co-verkoop. Alle deals worden gemaakt als door partners geleide deals. Ze zijn zichtbaar voor Microsoft-verkopers.

>[!Important]
> Als er fouten zijn waardoor sommige deals niet kunnen worden gemigreerd, kunt u de dealmigratie opnieuw starten door te klikken op de knop **Deals migreren.** Deze functie wordt alleen ingeschakeld als er nog enkele in aanmerking komende deals moeten worden gemigreerd. Dit is ook handig als u zich in de overgangsfase waar een aantal nieuwe deals worden gemaakt in PSC na het initiëren van de dealmigratie.

Zodra alle deals zijn gemigreerd, wordt er een banner weergegeven met 'Geen **deals** om te migreren' met de knop **'Deals** migreren' **uitgeschakeld.**

## <a name="next-steps"></a>Volgende stappen

Meer informatie over het maken en beheren van IOT-deals in Partner Center.
Dit is een belangrijke stap, waarmee u wordt voorbereid op het beheer van IOT-deals in Partner Center. Krijg inzicht in de werkstromen en de wijzigingen in Partner Center, zodat u effectief deals kunt maken en beheren. Begin met het volledig lezen van dit document.

## <a name="differences-between-psc-and-pc-workflows"></a>Verschillen tussen PSC- en PC-werkstromen

|**Scenario**|**Partnerverkoop Verbinding maken**|**Partnercentrum**|
|-----|:-----|:-----|
|Gebruikersrollen|PSC heeft beheerders-, dealmanager- en verkoperrollen.|Partner Center heeft [de rollen Verwijzingsbeheerder](permissions-overview.md#manage-referrals) en Verwijzingsgebruikers die zowel lees- als schrijfmachtigingen geven op basis van het locatiebereik.|
|Microsoft-verkopersgegevens|Zichtbaar zodra er een deal wordt gemaakt.|Microsoft-verkopersgegevens zijn niet zichtbaar voor partners, omdat het dealtype wordt geleid door een partner.
|Oplossingen|Elk aantal oplossingen kan worden toegevoegd aan de deal.|De partner kan maximaal 50 oplossingen toevoegen aan de deal.
|Toewijzing van deal|Alleen de toegewezen verkoper kan de deals bekijken en er actie op ondernemen.|Verwijzingsgebruikers die zijn toegevoegd aan de teamsectie van een deal kunnen de deal bekijken en er actie op ondernemen. Verwijzingsbeheerders voor de MPN-locatie waarvoor de deal is gemaakt, kunnen de deal bekijken en er actie op ondernemen.|
|Klantorganisatie|Vrije tekstinvoer.|U kunt de [klantorganisatie doorzoeken](manage-co-sell-opportunities.md#select-your-customer) op de [D&B-database](https://www.dnb.com/) door slechts een paar tekens te typen. De juridische naam en het juridische adres worden automatisch ingevuld op basis van de keuze.|

## <a name="moving-from-psc-to-pc---faq"></a>Over van PSC naar PC - Veelgestelde vragen

In de volgende secties worden veelgestelde vragen over de migratie beantwoord.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Wat moet ik doen als ik geen toegang heb tot Partner Center?

U kunt contact opnemen met uw beheerders die worden vermeld op de pagina Geen toegang om de rollen toegewezen te krijgen. U hebt de [verwijzingsbeheerdersrol nodig](permissions-overview.md#manage-referrals) voor de lees- en schrijfmachtiging in de sectie verwijzingen. Als u alleen zakelijke profielen beheert, hebt u de beheerdersrol bedrijfsprofiel nodig in het partnercentrum.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Afbeelding van de ervaring geen toegang in Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Wie mij toegang verlenen tot de sectie Verwijzingen in Partner Center?

Uw [accountbeheerder](permissions-overview.md#manage-mpn-membership-and-your-company) kan u toegang verlenen tot het tabblad Verwijzingen. Als u de accountbeheerder wilt zoeken, selecteert u **Accountinstellingen** in het tandwielpictogram rechtsboven in Partner Center [dashboard.](https://partner.microsoft.com/dashboard) Selecteer vervolgens **Gebruikersbeheer in** de linkernavigatiebalk op het tweede niveau. Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst Filter** en wijzig de optie in **accountbeheerder**. Op de pagina worden alle accountbeheerders met hun respectieve e-mailadressen weergegeven. Vraag een van deze om de rol van verwijzingsbeheerder voor uw werkaccount toe te wijzen.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3: de knop +nieuwe deal wordt grijs voor ons account. Wat moet ik doen om deals te maken?

Dit gebeurt alleen als de MPN-id die is gekoppeld aan uw account niet is ingeschakeld voor het maken van IOT-deals. Neem contact op met het IOT-bedrijfsteam via de e-mail die is verstrekt tijdens de trainingssessies of maak een ondersteuningsticket om uw MPN-id in te stellen voor IOT-deals.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - Kan ik deals toewijzen aan een specifieke persoon van onze organisatie, zoals PSC?

U kunt teamleden toewijzen aan een specifieke deal. Het blokkeert niet dat andere verwijzingsbeheerders deze deals kunnen bekijken of gebruiken.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Is er een weergave van alle deals die aan mij zijn toegewezen?

U kunt de functie Favorieten gebruiken. Dit is een tabblad op gebruikersniveau. U kunt alle deals die aan u zijn toegewezen markeren als favorieten om snel toegang te krijgen tot de deals.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Is er een alleen-lezen weergave voor de deals?

Nee, er is geen alleen-lezen weergave van de deals in de sectie verwijzingen.

### <a name="7---is-adding-a-customer-organization-mandatory"></a>7 - Is het toevoegen van een klantorganisatie verplicht?

Ja, het toevoegen van [een klantorganisatie](./manage-co-sell-opportunities.md#select-your-customer) is verplicht in Partner Center. Zoek eerst naar de locatie waar de klant zich bevindt. Op basis van de details die u hebt; U kunt specifieke details toevoegen, zoals de exacte naam van het gebouw of alleen de plaatsgegevens opgeven. De organisatiezoekactie haalt alle juridische entiteiten op die overeenkomen met de naam die u hebt invoeren, zodat u geen adresgegevens hoeft in te voeren. Alle gegevens worden automatisch ingevuld op basis van de geselecteerde organisatie.

### <a name="8---are-customer-contact-details-mandatory"></a>8 - Zijn contactgegevens van de klant verplicht?

Ja, contactgegevens van klanten zijn verplicht voor het maken van IOT-deals.

### <a name="9---how-many-solutions-can-i-add-to-a-deal"></a>9 - Hoeveel oplossingen kan ik toevoegen aan een deal?

U kunt maximaal 50 oplossingen (vergelijkbaar met 'producten' in PSC) toevoegen aan een deal. Zowel de hoeveelheid als de geschatte einddatum voor de oplossingen is verplicht en de geschatte einddatum van oplossingen moet eerder zijn dan de geschatte einddatum in de sectie details van de deal.

### <a name="10---where-can-i-find-the-opportunity-id"></a>10 - Waar vind ik de id van de kans?

De kans-id in PSC is hetzelfde als de verwijzings-id in Partner Center. U vindt de verwijzings-id naast de dealnaam wanneer u een deal opent.
