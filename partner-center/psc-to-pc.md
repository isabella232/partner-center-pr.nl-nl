---
title: Migreren vanuit Partner Sales Verbinding maken (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Meer informatie over hoe Microsoft-partners kunnen migreren van Partner Sales Verbinding maken (PSC) naar Partner Center maken of beheren van deals die door Microsoft-verkopers worden verzonden.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.date: 09/08/2021
ms.openlocfilehash: 96106dd84d4889c9165daf41385d1092361101c4
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128359496"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Handleiding voor co-verkoop in Partner Center (PC) voor partners die migreren van Partner Sales Verbinding maken (PSC)

**Juiste rollen:** Accountbeheerder | Beheerdersaccounts voor verwijzingen | Verkoper van Verbinding maken (PSC) van partner | Beheerders van Verbinding maken (PSC) | Partner Sales Verbinding maken (PSC) deal manager

Dit artikel bevat richtlijnen voor partners die migreren van Partner Sales Verbinding maken (PSC) naar Partner Center (PC), zodat ze deals voor co-verkoop kunnen blijven maken en beheren in Partner Center.

> [!NOTE]
> Als u hier bent omdat u een banner in PSC over de migratie hebt gezien, bent u op de juiste plaats. Deze handleiding is niet van toepassing op Solution Assessment (SA) en OEM-licentieverleningspartners die hun deals beheren in PSC.

> [!IMPORTANT]
> Vanaf 1 april 2021 kan uw bedrijf geen deals meer maken of bewerken in PSC. **U kunt nog steeds de bestaande dealsgegevens downloaden met behulp van de bulkexportfunctie in PSC. U kunt ook [openstaande deals migreren van](psc-to-pc.md#psc-deals-migration) PSC naar Partner Center na deze datum.**
> 
> Als er deals zijn waar u actief aan werkt die in aanmerking komende oplossingen voor IP-co-verkoop incentive bevatten, hebt u twee opties:
> 
> 1. Markeer de deal als gewonnen en voltooi de dealregistratie in PSC vóór 31 maart 2021.
> 2. [Migreert de deals](psc-to-pc.md#psc-deals-migration) Partner Center zodat u meer tijd hebt om aan de deal te werken en de registratie van de deal te starten.

Hoewel uw bedrijf na 30 april 2021 geen toegang meer heeft tot PSC, vindt u nog steeds alles wat u wilt doen in Partner Center, zoals het maken van deals voor co-verkoop, het beheren van uw deals en het handelen op deals die door verkopers van Microsoft naar u zijn verzonden.

Er zijn echter wel verschillen. De volgende richtlijnen kunnen helpen om uw overgang naar Partner Center en eenvoudiger te maken.

## <a name="things-to-know-before-moving"></a>Dingen die u moet weten voordat u gaat verplaatsen

### <a name="if-you-are-a-psc-admin"></a>Als u een PSC-beheerder bent

- U hebt een e-mailadres van het werk nodig om u aan te melden [bij Partner Center](https://partner.microsoft.com/).
- Stel uw account in met behulp van de Partner Center [accountbeheerder](permissions-overview.md).
- In dit document leest u hoe u in Partner Center kunt verkopen.
- Stel gebruikersaccounts in Partner Center voor al uw PSC-gebruikers (beheerders-, dealbeheer- en verkoperrollen) en wijs deze verwijzingsbeheerdersrollen [toe.](permissions-overview.md)

>[!IMPORTANT]
> Zorg ervoor dat Microsoft Partner Network-id (MPN) die wordt weergegeven in de PSC-banner beschikbaar is in de lijst met MPN-locaties in Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Afbeelding van de PSC-banner waar de partners de MPN-id kunnen vinden.":::

 Als u wilt controleren of de MPN-id wordt weergegeven als een Partner Center MPN-locatie, meld u zich aan bij het [Partner Center-dashboard](https://partner.microsoft.com/dashboard)en selecteert u **Instellingen** (het tandwielpictogram) rechtsboven in het scherm, gevolgd door **Account Instellingen**. Selecteer in het linkernavigatiemenu op  het tweede niveau Locaties om de lijst met alle MPN-ID's en locaties weer te geven die zijn gekoppeld aan het Partner Center account.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Als u een PSC-dealmanager of verkoper bent

- U hebt een e-mailadres van het werk nodig om u aan te melden bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)
- Als u een niet-werkaccount in PSC gebruikt of als uw werke-mail voor een ander bedrijf is dan het partnerbedrijf, neem dan contact op met uw PSC-beheerder voor hulp bij het instellen van het account.
- Neem contact op met uw PSC-beheerder Partner Center account is ingesteld, ongeacht het account dat u gebruikt om u aan te melden bij PSC.
- Controleer of u toegang hebt tot Partner Center en de sectie Verwijzingen.
- Lees dit document voor meer informatie over de werkstromen en de wijzigingen in Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Als beheerder in PSC zijn dit de volgende stappen

Selecteer in Partner Center linkernavigatiemenu **de optie Verwijzingen.** Controleer of u toegang hebt tot de pagina Verwijzingen.

  >[!Note]
  > Mogelijk moet u zich bij uw Partner Center en weer aanmelden om uw referenties te vernieuwen voor toegang tot de verwijzingenpagina's.

**Als** u de optie  Verwijzingen niet ziet in het Partner Center-menu of de pagina's met verwijzingen, neem dan contact op met de [accountbeheerder](permissions-overview.md) van uw bedrijf en vraag deze om u toegang te geven tot de optie Verwijzingen en het bijbehorende gebied.

Ga als volgende te werk om de accountbeheerder van uw bedrijf te vinden:

1. Selecteer **Accountinstellingen** in het tandwielpictogram rechtsboven in Partner Center dashboard.

1. Selecteer **Gebruikersbeheer in** het navigatiemenu links op het tweede niveau.

1. Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst** Filter. Wijzig de optie in **Accountbeheerder**.

   Op de pagina worden alle accountbeheerders met hun respectieve e-mailadressen weergegeven. Stuur een e-mail naar een van deze en vraag deze om de beheerdersrol verwijzingen toe te wijzen voor uw werkaccount.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Afbeelding van de accountbeheerders op de pagina Gebruikersbeheer van partnerinstellingen.":::

>[!Important]
>- Als uw rol alleen betrekking heeft op het beheren van gebruikers in PSC, vraagt u de accountbeheerder van uw bedrijf u de [rol van accountbeheerder](permissions-overview.md#manage-mpn-membership-and-your-company) toe te wijzen in Partner Center. 
>- Als uw rol ook het beheren van kansen voor co-verkoop omvat, vraagt u om de beheerdersrol [verwijzingen toegewezen te](permissions-overview.md#manage-referrals) krijgen.
> - Het is een goed idee om ook één lead voor wijzigingsbeheer te benoemen bij de PSC-beheerders. Zo voorkomt u dat alle PSC-beheerders afzonderlijk contact moeten maken met Partner Center accountbeheerders. In plaats daarvan kan de lead voor wijzigingsbeheer de primaire persoon zijn die met de Partner Center accountbeheerder werkt.

## <a name="user-migration"></a>Gebruikersmigratie

Nadat u uw account hebt ingesteld in Partner Center, gebruikt u de wizard gebruikersmigratie op de pagina verkoopkansen om automatisch Partner Center toewijzen aan werknemers van uw bedrijf.

>[!Note]
> Gebruikersmigratie kan alleen worden uitgevoerd door [accountbeheerders](permissions-overview.md#manage-mpn-membership-and-your-company) van uw bedrijf. Als u niet de rol van accountbeheerder hebt, zoek dan een accountbeheerder die u kan helpen bij het instellen van de gebruikersaccounts met behulp van de wizard gebruikersmigratie.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Afbeelding van de wizard gebruikersmigratie.":::

Accountbeheerders zien een koppeling naar de wizard psc-gebruikersmigratie op de pagina voor verkoopkansen naast de verwijzingenhandleiding. Ze kunnen de gebruikersmigratie initiëren door de koppeling te selecteren. Beheerders kunnen de koppeling selecteren om de gebruikersmigratie te starten. Ze kunnen deze gebruikersmigratiestap meerdere keren uitvoeren totdat aan alle gebruikers de juiste rollen zijn toegewezen in Partner Center.

De gebruikersmigratietabel heeft de volgende details:

- Gebruikersaccount: e-mail-id van de werknemer
- PSC-partneraccount: het account waaraan de werknemer is gekoppeld in PSC
- PSC-gebruikersrol: een van de drie rollen die zijn toegewezen aan in PSC.
- MPN-locatie van PC: de locatie waarvoor de gebruiker relevante Partner Center (pc)-rollen krijgt. De MPN van het PSC-partneraccount wordt gebruikt om de equivalente MPN-locatie in de Partner Center om machtigingen toe te wijzen. De hele organisatie geeft de mpn-id van de vOrg aan.
- Pc-gebruikersrol: aan werknemers worden rollen toegewezen op basis van hun PSC-gebruikersrollen. Beheerders in PSC krijgen de beheerdersrollen Verwijzingen toegewezen in Partner Center. Aan verkoper wordt de gebruikersrol verwijzingen toegewezen in Partner Center. Meer informatie over de Partner Center-rollen en wat gebruikers met deze rollen kunnen doen in Partner Center in de sectie Verwijzingen beheren van Gebruikersrollen en -machtigingen toewijzen voor de gebruikers van een bedrijf die [in Partner Center.](permissions-overview.md#manage-referrals)
- PC AAD-tenant: de Microsoft Azure Active Directory (Azure AD)-tenant waaraan de gebruikers zijn toegewezen in Partner Center
- Status: er zijn drie mogelijke statussen voor de status van de migratie
    - **Niet gemigreerd:** aan de gebruiker zijn geen Partner Center toegewezen
    - **Gemigreerd:** de gebruiker is gemigreerd met de relevante rol die is toegewezen, zoals wordt weergegeven in de tabel
    - **Fout:** de migratie kan niet worden voltooid vanwege een fout

Soms kan de migratie mislukken en leiden tot fouten. Hier zijn enkele redenen waarom een migratie een fout kan veroorzaken en enkele manieren om het probleem op te lossen:

1. De PSC-gebruikers gebruiken mogelijk een niet-werkaccount.

2. De PSC-gebruiker gebruikt mogelijk een account uit een ander domein dan het account dat u gebruikt in Partner Center.

   Als u fouten met betrekking tot scenario 1 en 2 wilt oplossen, vraagt u de gebruiker zich aan te melden bij Partner Center met het werkaccount dat is gekoppeld aan uw Azure AD-tenant. Uw [globale beheerder](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) kan u helpen.
   
   Uw globale beheerder zoeken: 
   - Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard) selecteer **Accountinstellingen** in het tandwielpictogram rechtsboven.
   - Selecteer **Gebruikersbeheer in** de linkernavigatiebalk op het tweede niveau.
   - Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst Filter** en wijzig de optie in **Globale beheerder.** Op de pagina worden vervolgens alle globale beheerders met hun respectieve e-mailadressen weergegeven. Vraag een van deze om de rol van verwijzingsbeheerder voor uw werkaccount toe te wijzen.
   
      De globale beheerder kan een nieuw gebruikersaccount maken in uw Azure AD-tenant of gastgebruikerstoegang toewijzen aan de andere domeinaccountgebruikers. Zodra de accounts zijn ingesteld voor alle PSC-dealmanagers en -gebruikers, moeten ze zich aanmelden bij Partner Center, **Verwijzingen** selecteren in het navigatiemenu aan de linkerkant en bevestigen dat ze de pagina Verwijzingen kunnen zien.

3. De gebruiker heeft al een verwijzingsrol toegewezen in Partner Center.
    - U kunt de bestaande rol van de gebruiker controleren. Selecteer in de rechterbovenhoek van Partner Center selecteer **Instellingen** (het tandwielpictogram) en vervolgens **Accountinstellingen.** Wanneer u een tweede linkernavigatiemenu ziet, selecteert u **Gebruikersbeheer** en zoekt u naar de gebruiker.

## <a name="psc-deals-migration"></a>Migratie van PSC-deals

Nadat u de gebruikersmigratie hebt voltooid, gebruikt u de migratiewizard voor deals op de pagina mogelijkheden voor co-verkoop om alle in aanmerking komende openstaande deals van PSC naar een Partner Center. **De migratiekoppeling naar deals is alleen zichtbaar voor verwijzingsbeheerders met het hele organisatiebereik in Partner Center.** Rechtsboven op de pagina Collectieve verkoopkansen verschijnt een koppeling met de naam **PSC-dealmigratie**. Hiermee wordt de wizard Dealmigratie geopend.

Lees deze sectie voordat u de dealmigratie start.

**Komt in aanmerking voor migratie**

Slechts enkele deals komen in aanmerking voor migratie van PSC naar Partner Center. Deze migratiewizard is gebouwd om partners te helpen hun deals te Partner Center waar ze nog steeds actief met hun klanten werken om de deal te sluiten. **Alleen deals met een open status die zijn gemaakt op 1 januari 2020 met geldige partneraccountgegevens (geldige MPN-id) en die geen dealregistratie ondergaan, komen in aanmerking voor migratie.**

**Komt niet in aanmerking voor migratie**

- Deals voor oplossingsevaluatie komen niet in aanmerking voor dealmigratie
- Zakelijke deals met OEM-licenties komen niet in aanmerking voor dealmigratie
- Een deal die is gemarkeerd als gewonnen in PSC, komt niet in aanmerking voor migratie. Dealregistratie als deze in aanmerking komt voor de deals die zijn gemarkeerd als gewonnen, moet worden voltooid in PSC.

## <a name="pre-requisites-for-deal-migration"></a>Vereisten voor dealmigratie

Voordat u begint met de dealmigratie Partner Center, volgt u de onderstaande instructies om de deals in PSC in te stellen voor een geslaagde migratie.

1. Alle leden van het verkoopteam in uw bedrijf die aan de openstaande deals werken, worden op de hoogte gesteld van deze migratie.
2. De leden van het verkoopteam zijn getraind om Partner Center te gebruiken voor dealbeheer.
3. De deals bevatten alle vereiste informatie, zoals hieronder wordt beschreven.
    - Bedrijfsgegevens van klant, inclusief naam en adres
    - Contactgegevens van de klant als het een deal voor co-verkoop is
    - Ten minste één oplossing
    - Ten minste één teamlid met alle details: voornaam, achternaam, e-mail-id en telefoonnummer
    - Dealwaarde
    - Geschatte einddatum deal
    - Partnernotities

U kunt de mogelijkheden voor bulksgewijs downloaden en uploaden in PSC gebruiken om alle ontbrekende details in de deal toe te voegen voor alle in aanmerking komende deals.

>[!Note]
> De dealmigratie slaagt zelfs als niet aan de bovenstaande vereisten wordt voldaan. U kunt de status van de deal echter niet wijzigen als een van de hierboven genoemde vereiste velden in Partner Center niet beschikbaar zijn. Vervolgens moet u alle vereiste gegevens invoeren die ontbreken in de deals in Partner Center aan de slag te gaan. **Het wordt ten zeerste aangeraden om de in aanmerking komende deals in PSC op te schonen voordat u deze migreert naar Partner Center.**

De dealmigratie in Partner Center is gebouwd als een ervaring met één klik. U hoeft alleen maar de knop **'Deals migreren' te selecteren** zodra uw bedrijf klaar is om de in aanmerking komende deals te migreren. **U kunt de deals die u wilt migreren vanuit PSC niet kiezen. Als u geen deals wilt migreren naar Partner Center, verplaatst u deze naar de gesloten status in PSC voordat u de migratie start.**

>[!Note]
> Nadat de migratie is geïnitieerd, kan het tot 24 uur duren voordat **de deals zijn gemigreerd.**

Zodra de migratie is voltooid, is de status van het bannerbericht gewijzigd, met een koppeling naar het migratierapport. Download het rapport om de details weer te geven van deals die zijn gemigreerd van PSC naar Partner Center.

Het rapport bevat de onderstaande details.

1. **Partner Center engagement-id:** de unieke id in Partner Center voor alle deals in een overeenkomst. Er zijn twee deals: één voor de partner en één voor Microsoft bij een overeenkomst voor co-verkoop in Partner Center.
2. **Partner Center verwijzings-id:** de unieke id in Partner Center voor de deal die bij de partner hoort.
3. **Dealnaam:** id die is opgegeven voor de deal in PSC.
4. **PSC-deal-id:** de unieke id in PSC voor de deal.
5. **Fouten:** om aan te geven of er een fout is opgetreden tijdens het migreren van een specifieke deal.

Alle deals die zijn gemigreerd, zijn niet zichtbaar in PSC. U kunt blijven werken aan de gemigreerde deals in Partner Center waaronder het voltooien van dealregistratie in Partner Center. Er worden geen wijzigingen aangebracht in de interacties met de Microsoft-verkopers voor deals voor co-verkoop.

Deals die vanuit PSC worden gemigreerd, zijn beschikbaar op de tabbladen Inkomende en Uitgaande op basis van de bron van de deal. Alle deals die door uw bedrijf worden gedeeld, zijn beschikbaar op het tabblad Uitgaand en door Microsoft geïnitieerde deals zijn beschikbaar op het tabblad Binnenkomende Partner Center. Er zijn twee soorten deals die na de migratie worden gemaakt.

1. **Deals voor co-verkoop:** deals die zijn gemarkeerd als co-sell in PSC, worden gemaakt als deals voor co-verkoop in Partner Center.
2. **Door partners geleide deals:** deals die niet zijn gemarkeerd als co-sell, worden gemaakt als door partners geleide deals in Partner Center. Door partners geleide deals zijn zichtbaar voor Microsoft-verkopers en kunnen worden geüpgraded naar deals voor co-verkoop voordat de terminaltoestand wordt bereikt (gewonnen, verloren). Bovendien komen door partners geleide deals in aanmerking voor dealregistratie als er een oplossing is die in aanmerking komt voor een incentive in de deal.

>[!Important]
> Als er fouten zijn waardoor sommige deals niet kunnen worden gemigreerd, kunt u de dealmigratie opnieuw starten door te klikken op de knop **Deals migreren.** Deze functie wordt alleen ingeschakeld als er nog enkele in aanmerking komende deals moeten worden gemigreerd. Dit is ook handig als u zich in de overgangsfase waar een aantal nieuwe deals worden gemaakt in PSC na het initiëren van de dealmigratie.

Zodra alle deals zijn gemigreerd, wordt er een banner weergegeven met 'Geen **deals** om te migreren' met de knop **'Deals** migreren' **uitgeschakeld.**

Gebruik na het voltooien van de gebruikersmigratie en/of dealmigratie de volgende richtlijnen om de migratiestrategie te bepalen:

Als uw bedrijf een Partner Development Manager (PDM) heeft: wanneer uw Partner Center-account is ingesteld en uw gebruikers zijn overgeschoven en rollen en machtigingen hebben, kunt u uw co-verkoopactiviteiten verplaatsen naar Partner Center. Informeer de PDM om over te schakelen in plaats van te wachten tot de deadline van de migratie is voltooid, waardoor al uw nieuwe deals naar de Partner Center.

>[!Note]
>Zodra u deze overstap hebt gemaakt, kunt u alleen reageren op de bestaande actieve deals in PSC. U kunt geen nieuwe deals maken en geen deals ontvangen van Microsoft-verkopers in PSC.

Als uw bedrijf geen PDM heeft: zorg ervoor dat alle gebruikersaccounts zijn ingesteld en geverifieerd door alle gebruikers. U ontvangt een melding via een e-mail en een banner in PSC met betrekking tot de exacte datum waarop u kunt beginnen met de co-verkoop in Partner Center. Houd er wel voor dat u nog steeds de bestaande actieve deals in PSC moet beheren.

>[!Important]
> U hebt tot 30 april 2021 de tijd om de deals te registreren die zijn gemarkeerd als gewonnen.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Volgende stappen voor PSC-beheerders, PSC-dealmanagers en PSC-verkopers

Meer informatie over co-sell in Partner Center.
Dit is een belangrijke stap, waarmee u wordt voorbereid op co-verkoop in Partner Center. Krijg inzicht in de werkstromen en de wijzigingen in Partner Center, zodat u meteen effectief samen kunt verkopen. Begin met het volledig lezen van dit document. Er is ook een goede set resources beschikbaar in de galerie [met de ervaring voor co-sell.](https://aka.ms/cosellexperience)

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Belangrijke verschillen tussen PSC- en Partner Center werkstromen

|**Scenario**|**Verkoopcijfers van Verbinding maken**|**Partnercentrum**|
|-----|:-----|:-----|
|Gebruikersrollen|PSC heeft beheerders-, dealmanager- en verkoperrollen.|Partner Center heeft alleen de [rol verwijzingsbeheerder](permissions-overview.md#manage-referrals) die zowel lees- als schrijfmachtigingen biedt voor alle deals.|
|Microsoft uitnodigen voor een deal voor co-verkoop|Geïnitieerd door Microsoft-verkoper, is er geen expliciete vraag door de partner.|De partner moet een expliciete [aanvraag indienen](manage-co-sell-opportunities.md#add-solutions) als er verkopershulp van Microsoft nodig is voor een deal. Microsoft Verkoper heeft een optie om de aanvraag te weigeren.|
|Vervaldatum|Er is geen concept van het verlopen van een deal.|Binnenkomende deals van partners verlopen binnen 14 dagen als ze niet worden geaccepteerd door de partner. Hetzelfde geldt voor uitgaande deals van partners, waarbij ze de status Verlopen kunnen krijgen als de Microsoft-verkoper er over 14 dagen geen actie op ondergaat.|
|Microsoft-verkopersgegevens|Zichtbaar zodra er een deal wordt gemaakt.|Microsoft-verkopersgegevens worden alleen gedeeld met partner als de verkoper expliciet de uitnodiging voor co-verkoop van partner accepteert.|
|[Privépijplijn](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Niet beschikbaar.|Partners kunnen hun pijplijn delen zonder microsoft-verkopers meer inzicht te geven.|
|Oplossingen|Oplossingen die tot slechts één prijslijst behoren, kunnen worden toegevoegd aan een deal.|Partner kan oplossingen [toevoegen die](manage-co-sell-opportunities.md#add-solutions) deel uitmaken van de volgende lijsten. a) Hun eigen oplossingen b) Oplossingen uit de catalogus van Microsoft (vergelijkbaar met de rol van transactiedeal in PSC) en c) oplossingen voor co-verkoop van andere externe partners (vergelijkbaar met de rol ISV Deal in PSC).|
|Toewijzing van deal|Alleen de toegewezen verkoper kan de deals bekijken en er actie op ondernemen.|Teamleden kunnen worden toegevoegd aan een deal om de personen op te geven die aan een deal werken. Andere verwijzingsbeheerders kunnen deze deals niet bekijken of er actie op onder de weg staan.|
|Klantorganisatie|Vrije tekstinvoer.|U kunt de [klantorganisatie doorzoeken](manage-co-sell-opportunities.md#select-your-customer) op de [D&B-database](https://www.dnb.com/) door slechts een paar tekens te typen. De juridische naam en het juridische adres worden automatisch ingevuld op basis van de keuze.|
|Contactpersoon van klant|Niet verplicht.|Niet verplicht voor het delen van privépijplijnen. Vereist als Microsoft-verkoper wordt uitgenodigd voor deelname aan een aanvraag voor co-verkoop.|
|Openbare API|Niet beschikbaar.|[Openbare API](/partner/develop/referrals) voor het programmatisch beheren Partner Center verwijzingen.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Wijs de velden in PSC toe aan de bijbehorende velden in Partner Center

In deze sectie worden geselecteerde schermopnamen (of 'kaarten') voor PSC vergeleken met de bijbehorende weergave in de sectie Partner Center verkoopkansen.

Op elk paar schermopnamen ziet u genummerde, gele of rode cirkels:

- **Wat betekenen gele cirkels?** Genummerde, gele cirkels worden eerst weergegeven op elke PSC-schermopname. Vervolgens ziet u een begeleidende Partner Center schermopname met veel van dezelfde cijfers.

   Als u wilt zien hoe elk veld of kenmerk in PSC wordt gerelateerd aan het equivalent in Partner Center, koppelt u de genummerde cirkels aan elkaar in de twee gerelateerde schermopnamen. Koppel bijvoorbeeld de genummerde, gele '1' in de eerste PSC-schermopname aan de genummerde, gele '1' in de tweede, Partner Center schermopname eronder.

- **Wat betekent een rode cirkel?** Als u op één schermopname een rode cirkel ziet, geeft dit aan dat het PSC-veld niet beschikbaar is in Partner Center.

PsC-naar-Partner Center veldtoewijzingen worden weergegeven voor de volgende gebieden:

1. PSC-startpagina die is Partner Center standaardweergave voor verkoopkansen
1. PSC-rasterweergave die is Partner Center dealweergave
1. Details van PSC-deal die zijn Partner Center de detailweergave van de deal
1. PsC-weergave Producten toevoegen die is Partner Center weergave Oplossingen toevoegen
1. PsC-gebruikersbeheerweergave die is Partner Center de weergave gebruikersbeheer
1. Toewijzingsweergave van PSC-gebruikersrol die is Partner Center de toewijzingsweergave van de rol
1. PSC-meldingen weergeven die zijn Partner Center de weergave meldingen

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - PSC-startpagina die is Partner Center standaardweergave voor verkoopkansen

Vergelijk de overeenkomende, genummerde cirkels tussen de bovenste PSC-schermopname en Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend Partner Center veld.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Afbeelding van de veldtoewijzingen tussen de startpagina van Partner Sales Verbinding maken en de standaardweergave van kansen voor co-verkoop in Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - PSC-rasterweergave die is Partner Center dealweergave

Vergelijk de overeenkomende, genummerde cirkels tussen de bovenste PSC-schermopname en Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend Partner Center veld.  

> [!NOTE]
> Andere overwegingen worden onder de schermopnamen weergegeven.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Afbeelding van de veldtoewijzingen tussen de rasterweergave Partner Sales Verbinding maken (PSC) en de weergave Partner Center deal." lightbox="images/pscmigration/grid-view-expanded.png":::

**Speciale overwegingen:**

- Er is geen lijstweergave in Partner Center zoals die van PSC.  Alle deals worden vermeld op basis van de meest recente ontvangen of gemaakte datum met de klantgegevens en het type deal. De eerste deal in de weergave is standaard geselecteerd. De meeste waarden die worden weergegeven in de PSC-tabelindeling zijn beschikbaar in de detailweergave van de deal in Partner Center.
- Dealrol is geen vereist veld in Partner Center. Deze wordt niet weergegeven of vastgelegd in een van de werkstromen. Deze wordt automatisch aan de verkoperszijde van Microsoft afgeleid op basis van de oplossingen die aan de deal zijn toegevoegd.
- De datum van laatste wijziging wordt niet weergegeven op de pagina met verwijzingsdetails in Partner Center. Partners kunnen de sorteerfunctionaliteit gebruiken om de deals te sorteren op basis van de laatste bijgewerkte datum.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - Details van PSC-deal die is Partner Center

Vergelijk de overeenkomende, genummerde cirkels in de bovenste schermopname (PSC) met de Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend veld of overeenkomend gebied in Partner Center.

> [!NOTE]
> Andere overwegingen worden onder de schermopnamen weergegeven.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Afbeelding van de veldtoewijzingen tussen de weergave details van de psc-deal (Partner Sales Verbinding maken) en de weergave Partner Center dealdetails." lightbox="images/pscmigration/deal-details-expanded.png":::

**Speciale overwegingen:**

- Partners kunnen een deal bewerken door de knop Bewerken te selecteren in de detailweergave van de partnerdeal (6). Zodra de knop Bewerken is geselecteerd, kunnen alle velden worden bewerkt. Vervolgens hebt u de mogelijkheid om de bewerkingen die zijn aangebracht aan de deal op te slaan of te annuleren.
- Er is geen optie om de deal te sluiten als duplicaat in Partner Center.
- Klantresultaat is niet beschikbaar in Partner Center. Alle details met betrekking tot interacties van klanten kunnen worden bijgewerkt in de sectie Notities in Partner Center.
- Geschatte einddatum van oplossing is alleen beschikbaar voor OEM IOT-deals in Partner Center. Deze informatie wordt niet weergegeven voor andere dealtypen.
- Licentieprogramma is niet vereist in Partner Center. Deze informatie wordt automatisch afgeleid op basis van de oplossingen die in de deal zijn geselecteerd.

>[!Note]
>Een deal die als gewonnen of verloren is gemarkeerd, kan later niet meer worden bewerkt. Wees voorzichtig bij het verplaatsen van een deal naar een van deze terminale staten.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - PSC-weergave 'Producten toevoegen' die is Partner Center weergave 'Oplossingen toevoegen'

Vergelijk de overeenkomende, genummerde cirkels in de bovenste schermopname (PSC) met de Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend veld of overeenkomend gebied in Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Afbeelding met de veldtoewijzingen tussen de weergave Producten toevoegen Verbinding maken Partner Sales Verbinding maken (PSC) en de weergave Partner Center oplossingen toevoegen." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - Gebruikersbeheer in PSC versus Partner Center

Vergelijk de overeenkomende, genummerde cirkels in de bovenste schermopname (PSC) met de Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend veld of overeenkomend gebied in Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Afbeelding van de veldtoewijzingen tussen de startpagina voor gebruikersbeheer van Partner Sales Verbinding maken (PSC) en de pagina Partner Center gebruikersbeheer in het gebied Accountinstellingen."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - Toewijzing van gebruikersrol in PSC versus Partner Center

Vergelijk de overeenkomende, genummerde cirkels in de bovenste schermopname (PSC) met de Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend veld of overeenkomend gebied in Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Afbeelding van de veldtoewijzingen tussen de roltoewijzingsweergave Partner Sales Verbinding maken (PSC) en de Partner Center roltoewijzingsweergave." lightbox="images/pscmigration/roles-expanded.png":::

**Speciale overwegingen:**

- De equivalente rol voor PSC-beheerder is de accountbeheerdersrol in Partner Center.
- Er is slechts één rol in Partner Center voor het beheren van een deal voor co-verkoop. Deze rol is de rol van verwijzingsbeheerder.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - Meldingen in PSC versus Partner Center

Vergelijk de overeenkomende, genummerde cirkels in de bovenste schermopname (PSC) met de Partner Center schermopname eronder. Overeenkomende getallen geven aan waar u de PSC-gerelateerde functie of het kenmerk kunt vinden in Partner Center. Rode cirkels geven aan dat er geen overeenkomend veld of overeenkomend gebied in Partner Center.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Afbeelding van de toewijzing tussen de PSC-meldingen (Partner Sales Verbinding maken) en de weergave Partner Center meldingen."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Over van PSC naar Partner Center - Veelgestelde vragen

In de volgende secties worden veelgestelde vragen over de migratie beantwoord.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - Wat moet ik doen als ik geen toegang heb tot Partner Center?

U kunt contact opnemen met uw beheerders die worden vermeld op de pagina Geen toegang om de rollen toegewezen te krijgen. U hebt de [verwijzingsbeheerdersrol nodig](permissions-overview.md#manage-referrals) voor de lees- en schrijfmachtiging in de sectie verwijzingen. Als u alleen zakelijke profielen beheert, hebt u de beheerdersrol bedrijfsprofiel nodig in Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Afbeelding van de ervaring geen toegang in Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - Wie mij toegang verlenen tot de sectie Verwijzingen in Partner Center?

Uw [accountbeheerder](permissions-overview.md#manage-mpn-membership-and-your-company) kan u toegang verlenen tot het tabblad Verwijzingen. Als u de accountbeheerder wilt zoeken, selecteert u **Accountinstellingen** in het tandwielpictogram rechtsboven in Partner Center [dashboard.](https://partner.microsoft.com/dashboard) Selecteer vervolgens **Gebruikersbeheer in** de linkernavigatiebalk op het tweede niveau. Selecteer bovenaan de lijst met gebruikers de **vervolgkeuzelijst Filter** en wijzig de optie in **accountbeheerder**. Op de pagina worden alle accountbeheerders met hun respectieve e-mailadressen weergegeven. Vraag een van deze om de rol van verwijzingsbeheerder voor uw werkaccount toe te wijzen.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3: de knop +nieuwe deal wordt grijs voor ons account. Wat moet ik doen om deals te maken?

Dit gebeurt alleen als er geen oplossingen voor co-verkoop zijn gekoppeld aan de MPN-organisatie die u gebruikt in Partner Center. Neem contact op met uw PDM om de MPN-id van uw oplossingen te corrigeren of maak een ondersteuningsticket met het probleem , 'Knop Nieuwe deal wordt grijs gemaakt na PSC-migratie'.

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - Kan ik deals toewijzen aan een specifieke persoon van onze organisatie, zoals PSC?

U kunt teamleden toewijzen aan een specifieke deal. Het blokkeert niet dat andere verwijzingsbeheerders deze deals kunnen bekijken of gebruiken.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Is er een weergave van alle deals die aan mij zijn toegewezen?

U kunt de functie Favorieten gebruiken. Dit is een tabblad op gebruikersniveau. U kunt alle deals die aan u zijn toegewezen markeren als favorieten om snel toegang te krijgen tot de deals.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Is er een alleen-lezenweergave voor de deals?

Nee, er is geen alleen-lezen weergave van de deals in de sectie verwijzingen. Alle verwijzingsbeheerders hebben volledige lees- en schrijftoegang tot alle deals.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Hoe kan ik een deal registreren nadat deze is markeert als gewonnen?

Als de deal voldoet aan de onderstaande criteria, wordt een pop-up weergegeven om dealregistratie [te starten.](./register-deals.md)

- Er is een oplossing die in aanmerking komt voor een incentive, gekoppeld aan de deal.
- Microsoft-verkoper wordt uitgenodigd om deel te nemen aan de deal of ze hebben u uitgenodigd voor de deal.
- Microsoft-kaart heeft de status Geaccepteerd of Gewonnen in Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8: er wordt een foutbericht weergegeven wanneer ik de knop +Nieuwe dealregistratie selecteer in de sectie Dealregistratie. Hoe kan ik mijn deals registreren?

De **knop +Nieuwe dealregistratie** wordt alleen gebruikt door de partners die zijn geregistreerd in het ISV Connect-programma voor het registreren van een deal zonder bijbehorende verkoopkans in Partner Center. Voor het registreren van deals met een verkoopkans wordt een pop-up weergegeven wanneer de deal is gemarkeerd als gewonnen en als deze voldoet aan de criteria voor dealregistratie.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - Is het toevoegen van een klantorganisatie verplicht?

Ja, het toevoegen van [een klantorganisatie](./manage-co-sell-opportunities.md#select-your-customer) is verplicht in Partner Center. Zoek eerst naar de locatie waar de klant zich bevindt. Op basis van de details die u hebt; U kunt specifiek zijn, zoals de exacte naam van het gebouw of alleen de plaatsdetails opgeven. De organisatiezoekactie haalt alle juridische entiteiten op die overeenkomen met de naam die u hebt invoeren, zodat u geen adresgegevens hoeft in te voeren. Alle gegevens worden automatisch ingevuld op basis van de geselecteerde organisatie.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - Zijn contactgegevens van klanten verplicht?

Dit is afhankelijk van [het type deal](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) dat u maakt. Als u alleen uw pijplijn deelt en geen hulp nodig hebt van de microsoft-verkooporganisatie, kunt u ervoor kiezen geen contactgegevens van klanten op te geven. Als u een co-verkoop waarbij u actief hulp nodig hebt van De verkoper van Microsoft, moet u de contactgegevens van de klant verstrekken. U moet expliciete toestemming van de klant krijgen voordat u een aanvraag voor co-verkoop maakt in Partner Center.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - Hoeveel oplossingen kan ik toevoegen aan een deal?

U kunt maximaal 50 oplossingen (vergelijkbaar met 'producten' in PSC) toevoegen aan een deal. In tegenstelling tot PSC kunt u oplossingen combineren van uw eigen oplossingen die in aanmerking komen voor co-verkoop, SKU's van Microsoft en andere oplossingen die in aanmerking komen voor co-verkoop van derden. Er hoeft geen deal-rol te worden geselecteerd of beschikbaar te zijn in Partner Center. Voor Microsoft-SKU's kunt u eventueel hoeveelheid en prijs toevoegen voor elke SKU die aan de deal wordt toegevoegd.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - Wanneer krijg ik informatie over de verkopergegevens van Microsoft nadat ik een deal heb gemaakt?

Microsoft-verkopers worden pas toegewezen nadat ze voldoen aan de exacte helpvereiste die is vermeld tijdens het maken van de deal met de relevante verkoper-persona aan de zijde van Microsoft. Zelfs na de toewijzing hebben Microsoft-verkopers de mogelijkheid om de uitnodiging voor co-verkoop te accepteren of af te wijzen. Alleen als een uitnodiging voor co-verkoop wordt geaccepteerd door een verkoper, wordt de deal bijgewerkt met de contactgegevens van de Microsoft-verkoper. De SLA voor Microsoft-verkopers om actie te ondernemen op de deal is 14 dagen. Het is dezelfde SLA die partners hebben om actie te ondernemen op de deal voordat deze de status Verlopen heeft.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - Waar vind ik de id van de kans?

De kans-id in PSC is hetzelfde als de deal-id in Partner Center. U vindt de deal-id naast de dealnaam wanneer u een deal opent.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - Hoe kan mijn PDM toegang krijgen tot Partner Center?

Partner Center zijn niet rechtstreeks toegankelijk voor uw PDA's, in tegenstelling tot PSC. Er zijn meerdere opties voor het inschakelen van die mogelijkheid, die hieronder worden vermeld.

- OCP Insights: als PDM's alleen de deals en de bijbehorende voortgang bekijken, kunnen ze de OCP-portal (One Commercial Partner) Insights gebruiken om de weergave van uw organisatie op te halen. Dit is een intern hulpprogramma en alleen beschikbaar voor PDM's. OCP-inzichten zijn niet beschikbaar voor gebruikers van uw bedrijf.
- Gastgebruiker in Partner Center: u kunt uw PDM-account toevoegen als gastgebruiker in Partner Center en de rol van verwijzingsbeheerder aan hen toewijzen, zodat ze verwijzingen kunnen bekijken en erop kunnen @microsoft.com reageren.
- Een [nieuwe](./create-user-accounts-and-set-permissions.md#add-a-new-user) gebruiker maken in uw tenant: u kunt een nieuwe gebruiker maken in uw eigen tenant en deze gegevens delen met de PDM, zodat ze verwijzingen kunnen bekijken en erop kunnen reageren die vergelijkbaar zijn met andere verwijzingsgebruikers in uw account.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>De juiste MPN-id zoeken als uw account in PSC niet is gekoppeld aan een geldige MPN

Als u hier bent omdat u een banner in PSC hebt gezien met de melding 'PSC invalid MPN ID association problem', bent u op de juiste plaats. Uw account is mogelijk om de volgende redenen gekoppeld aan een ongeldige MPN-id

- Uw bedrijf heeft geen Partner Center account.
- Uw PDM heeft een fout gemaakt tijdens het invoeren van de MPN-id van uw account in de interne systemen die uw PSC-account koppelen aan uw Partner Center-account (MPN-id).
- Uw bedrijf heeft de migratie van Partner Membership Center (PMC) naar Partner Center.

Zoek eerst de juiste MPN-id door de onderstaande stappen uit te voeren.

1. Meld u aan bij [uw Partner Center account](https://partner.microsoft.com/dashboard).
2. Gebruik de richtlijnen in de [documentatie over accountinstellingen om](./partner-center-account-setup.md#locate-your-mpn-id) de MPN-id te vinden.

Hieronder ziet u een schermopname met de exacte locatie waar u uw MPN Partner Center-id kunt vinden.

:::image type="content" source="images/pscmigration/finding-mpn-id.png" alt-text="Afbeelding van de accountinstellingen waar de partner de MPN-id kan vinden."  lightbox="images/pscmigration/finding-mpn-id.png":::

- Als u een PDM hebt, vraagt u deze om uw MPN-id te corrigeren met de juiste MPN-id van uw Partner Center account.
- Als u geen PDM hebt, stuurt u een e-mail naar het adres in de PSC-banner met zowel de PSC-accountgegevens die worden weergegeven in de PSC-banner als de juiste MPN-id van uw Partner Center-account.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Resources om u te helpen bij het maken en beheren van uw deals in Partner Center

Als u de Help-onderwerpen over co-sell nog niet hebt gelezen, helpen de volgende bronnen u bij het beheren van deals in Partner Center.

|**Om dit te doen**   |**Leest u**   |
|-----------------------|:-----------------------|
|Informatie over de tabbladen en navigatie op de pagina Kansen voor co-verkoop|[Navigeren door de sectie voor co-verkoop](./manage-co-sell-opportunities.md)|
|Een klantorganisatie selecteren in de D&B-lijst |[Uw klant selecteren](./manage-co-sell-opportunities.md#select-your-customer)|
|De velden in de sectie dealdetails wijzigen|[Details van deal](./manage-co-sell-opportunities.md#deal-details)|
|Uw teamleden toevoegen aan een dealteam|[Uw werknemers toevoegen](./manage-co-sell-opportunities.md#add-team-members)|
|Reageren op een deal voor co-verkoop|[Deals voor co-verkoop beheren](./manage-co-sell-opportunities.md#respond-to-a-co-sell-opportunity)
|Registreer deals die u hebt gewonnen in Partner Center |[Een nieuwe deal registreren](./register-deals.md)
|Verwijzingsinzichten verkrijgen en ontdekken hoe uw verwijzingen het doen |[Verwijzingsinzichten](./referral-insights.md)
|Bedrijfsprofiel maken en beheren|[Bedrijfsprofielen beheren](./create-a-marketing-profile.md)
|Leads beheren voor uw bedrijfsprofiel |[Leads beheren](./manage-leads.md)|

## <a name="next-steps"></a>Volgende stappen


- [Partner sales Verbinding maken to Partner Center workbook](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) - workbook to align partners's sales processes and roles with new sales processes via Partner Center vs. Partner Sales Verbinding maken.
- [Partner Center handleiding voor co-verkoop:](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) richtlijnen voor het identificeren van een operationeel model via Partner Center voor het beheren van leads of kansen voor co-verkoop en het registreren van deals.
- [De stapel voor](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) verwijzingsbeheer: stapsgewijs gevisualiseerde instructies voor het beheren van leads en kansen voor co-verkoop via Partner Center.
- [Publiceren en beheren in](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) de commerciële marketplace: stapsgewijs gevisualiseerde instructies voor het maken, beheren en publiceren van aanbiedingen via Partner Center in de commerciële marketplace.
