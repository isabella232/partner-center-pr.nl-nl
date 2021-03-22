---
title: De connector voor het samen verkopen van Dynamics 365 CRM-partner centrum
description: Synchroniseer verwijzingen in het partner centrum met de connector voor co-sell voor Dynamics 365 CRM. U kunt vervolgens samen met micro soft verkopen in uw CRM-systeem.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768768"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Connector voor Dynamics 365 CRM-overzicht co-sell

### <a name="appropriate-roles"></a>Juiste rollen

- Beheerder van verwijzingen
- Systeem beheerder of systeemaanpasser op de CRM

Met connectors voor het verkopen van partners kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen. Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop. Gebruik de co-Connect connectors om een nieuwe verwijzing naar de verkoop te maken voor een micro soft-verkoper, referenties te ontvangen van de micro soft-verkoper, verwijzingen te accepteren of te weigeren, en de deal gegevens te wijzigen, zoals de deal waarde en de sluitings datum. U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals. U kunt al uw referenties beheren in de CRM van uw keuze in plaats van in het partner centrum.

De oplossing is gebaseerd op het automatiseren van de functies en maakt gebruik van partner Center-Api's.

## <a name="prerequisites"></a>Vereisten

Voordat u de oplossing installeert, moet u ervoor zorgen dat aan de volgende vereisten wordt voldaan.

|**Onderwerpen**   |**Details**   |**Koppelingen**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID (MPN) |U hebt een geldige MPN-ID nodig.|[Neem lid van het partner netwerk](https://partner.microsoft.com/)|
|Klaar voor samen verkopen|Uw IP/Services-oplossing moet samen worden verkocht.|[Verkopen met micro soft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnercentrum-account|De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling. Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in de partner centrum-Portal kunt zien.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Gebruikers rollen voor het partner centrum|De werk nemer die de connectors installeert en gebruikt, moet een verwijzings beheerder zijn.|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser.|[Rollen toewijzen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Stroom account voor energie automatisering|Maak een nieuwe productie omgeving met een Data Base voor testen, fase ring en productie. Als u een bestaande productie omgeving met een Data Base hebt, kan deze opnieuw worden gebruikt. De gebruiker die de connector oplossing gaat installeren, moet beschikken over een automatische licentie en toegang tot deze omgeving. Als de installatie mislukt, kunt u de voortgang controleren en meer informatie krijgen in de [automatische energie](https://flow.microsoft.com/) registratie. Selecteer **Geschiedenis bekijken** onder **oplossingen**.|[Omgeving maken of beheren](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Synchronisatie van partner Center referrals voor Dynamics 365 (oplossing voor automatische stroom) installeren

1. Ga naar [energie automatisering](https://flow.microsoft.com)en selecteer in de rechter bovenhoek de optie **omgevingen** . In deze stap ziet u de beschik bare CRM-exemplaren.

1. Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.

1. Selecteer **oplossingen** aan de linkerkant.

1. Selecteer de koppeling **Open AppSource** in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Scherm opname van open AppSource.":::

1. Zoek naar **Partner Center referrals connectors voor Dynamics 365** in het pop-upvenster.  

1. Selecteer de knop **nu downloaden** en selecteer vervolgens **door gaan**.

1. Er wordt een pagina weer gegeven waar u de CRM-omgeving (Dynamics 365) kunt selecteren om de toepassing te installeren. Ga akkoord met de voor waarden.

1. U kunt de voortgang bewaken en, als de installatie mislukt, kunt u meer details in energie automatisering krijgen door onder **oplossingen** de optie **geschiedenis weer te geven** .

1. Nadat de installatie is voltooid, gaat u terug naar [automatische energie](https://flow.microsoft.com) en selecteert u **oplossingen** aan de linkerkant. De **synchronisatie van partner Center referrals voor Dynamics 365** is nu beschikbaar in de lijst met **oplossingen** .

1. Selecteer de **synchronisatie van partner Center referrals voor Dynamics 365**. De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Scherm opname waarin de beschik bare CRMs wordt weer gegeven.":::

## <a name="test-before-you-go-live"></a>Testen voordat u live gaat

Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test. U moet het volgende doen:

- Installeer de oplossing voor het automatiseren van energie beheer op een staging Environment CRM-exemplaar.
- De oplossing voor energie automatisering configureren en aanpassen in een faserings omgeving.
- Test de oplossing op een staging CRM-exemplaar.
- Na een geslaagde test kunt u importeren als een beheerde oplossing naar het productie-exemplaar.

## <a name="configure-the-solution"></a>De oplossing configureren

1. Nadat u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Automatische stroom](https://flow.microsoft.com/).

1. Selecteer in de vervolg keuzelijst **omgevingen** in de rechter BOVENHOEK het CRM-exemplaar waarop u de oplossing voor het automatiseren van energie beheer hebt geïnstalleerd.

1. U moet verbindingen maken die de drie gebruikers accounts koppelen:

   - Partner centrum-gebruiker met referrals beheerders referenties
   - Partnercentrum-gebeurtenissen
   - CRM-beheerder met de stroom voor het automatiseren van stromen in de oplossing

   1. Selecteer **verbindingen** aan de linkerkant en selecteer de oplossing **Partner Center referrals** in de lijst.

   1. Maak een verbinding door **een verbinding maken** te selecteren.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Scherm opname van een verbinding maken.":::

   1. Zoek naar **Partner Center referrals (preview)** in de zoek balk in de rechter bovenhoek.

   1. Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.

   1. Maak vervolgens een verbinding met de Partner Center-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de referentie beheerder.

   1. Maak een verbinding voor Common Data Service (huidige omgeving) voor de gebruiker van de CRM-beheerder.
     
   1. Nadat u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Scherm opname van verbindingen.":::

## <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar de pagina **oplossingen** en selecteer **standaard oplossing**. Selecteer **verbindings verwijzing (preview)** door **alle** te selecteren.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Scherm afbeelding waarin de verbindingen worden bewerkt.":::

1. Bewerk elk van de verbindingen één voor één door het pictogram met het weglatings teken te selecteren. Voeg de relevante verbindingen toe.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Scherm opname van de weer gegeven verbindingen.":::

1.  Ga terug naar de pagina **oplossingen** , selecteer **synchronisatie van partner Center referrals voor Dynamics 365** en schakel de stroom in door het pictogram met het weglatings teken naast elke stroom in de volgende reeks te selecteren. Zie [aanpassings stappen](connector-dynamics.md#customize-synchronization-steps) en [stappen voor probleem oplossing](connectors-troubleshoot.md)als u problemen ondervindt tijdens het inschakelen van de stroom.

Schakel de stromen in de volgende volg orde in:

- Inschrijving van partner Center-webhooks (Insider preview)
- Een verwijzing naar een co-sell maken – Dynamics 365 naar partner Center (Insider preview)
- Aanpassen Gegevens maken of ophalen uit Dynamics 365 flow
- Partner centrum voor Dynamics 365-helper (Insider preview)
- Partner centrum referentie-updates voor micro soft-verkoop naar Dynamics 365 (Insider preview)
- Partner centrum voor Dynamics 365 (Insider preview)
- Dynamics 365 naar partner Center (Insider preview)
- Dynamics 365-opportunity naar partner Center (Insider preview)
- Dynamics 365 micro soft Solutions to Partner Center (Insider preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-Api's gebruiken om te registreren voor bron wijzigings gebeurtenissen

U kunt de webhook-Api's van partner Center gebruiken om te registreren voor bron wijzigings gebeurtenissen. Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Selecteer **partner centrum voor Dynamics 365 (Insider preview)**.

1. Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen**.

1. Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.

   :::image type="content" source="images/webhook-video.gif" alt-text="Scherm opname van het gebruik van webhooks om resource wijzigingen te registreren.":::

1. Selecteer de stroom voor het automatiseren van de **Partner Center-webhook (Insider preview)** en selecteer vervolgens **uitvoeren**.

1. Zorg ervoor dat het venster **stroom uitvoeren** wordt geopend in het rechterdeel venster en selecteer **door gaan**.

1. Voer de volgende details in:

   - **Http-trigger eindpunt**: deze URL is uit een eerdere stap gekopieerd.
   - **Te registreren gebeurtenissen**: Selecteer alle beschik bare gebeurtenissen (door **verwijzing gemaakt**, **verwijzing-bijgewerkt**, **gerelateerde-verwijzing-gemaakt** en **gerelateerde-Referral-bijgewerkt**).
   - **Bestaande trigger eindpunten overschrijven indien aanwezig?**: Ja. Er kan slechts één URL worden geregistreerd voor een bepaalde webhook-gebeurtenis.

1. Selecteer **Run flow** en selecteer vervolgens **gereed.**

De webhook kan nu naar gebeurtenissen Luis teren, maken en bijwerken.

## <a name="customize-synchronization-steps"></a>Synchronisatie stappen aanpassen

CRM-systemen zijn zeer aangepast en u kunt de energiebeheer oplossing aanpassen op basis van uw CRM-installatie. Wanneer verwijzingen naar de verkoop worden gesynchroniseerd tussen het partner centrum en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-PC weer gegeven in de [hand leiding voor aangepaste veld toewijzing](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Volg de hand leiding voor de veld toewijzing en wijzig indien nodig de juiste wijzigingen in **[aanpassen] Create of Get details van Dynamics 365 flow** of omgevings variabelen. Werk geen andere stromen bij in de oplossing voor het automatiseren van de energie, omdat deze invloed kan hebben op toekomstige oplossings upgrades.

De volgende aanpassingen zijn beschikbaar:

- **Selectie vakje voor de naam van de opportunity inschakelen**: standaard wordt een vinkje weer gegeven naast de naam van de opportuniteit om aan te geven dat de synchronisatie tussen partner centrum en Dynamics 365 CRM met succes wordt uitgevoerd. Op dezelfde manier wordt een kruis markering weer gegeven als de synchronisatie mislukt. Als u wilt voor komen dat de naam van de verkoop kans wordt gecontroleerd of gemarkeerd, stelt u de huidige waarde van het **selectie vakje weer geven in de omgevings variabele Opportunity naam in** op Nee.
- **Deal waarde**: standaard wordt de deal waarde van partner Center gesynchroniseerd van en naar **ESTIMATEDVALUE** in de CRM. Als u een ander veld in de CRM hebt voor de deal waarde om te synchroniseren vanaf:

  - Werk de naam van het veld **deal waarde** bij in de omgevings variabele Dynamics 365 met de naam van het CRM-veld. Zorg ervoor dat u de naam van het veld opgeeft, niet de weergave naam.
  - Bewerken **[aanpassen] Maak of ontvang Details van de Dynamics 365-stroom** en ga naar de **verkoop kans maken of bijwerken** in CRM en update **Maak een nieuwe kans** en **werk de bestaande opportuniteits** acties bij om de **DealValue** -waarde toe te wijzen aan het juiste veld in het CRM. Verwijder ook de toewijzing **DealValue** uit het veld **geschatte omzet** .

- **Land code klant account**: het is verplicht een land code van twee letters (ISO 3166) op te geven wanneer u een nieuwe verwijzing maakt. De land code wordt standaard gesynchroniseerd van en naar het **address1_country** veld van het account in de CRM. Als u een ander veld in de CRM hebt voor de land code waarvan u wilt synchroniseren:

   - Voor een niet-opzoek veld land code in het account dat een code van twee letters bevat:
     - Werk de naam van het veld **land code van het klant account** in de Dynamics 365-omgevings variabele met de naam van het CRM-veld in. Zorg ervoor dat u de naam van het veld opgeeft, niet de weergave naam.
     - Bewerken **[aanpassen] Maak of ontvang Details van de Dynamics 365-stroom** en ga naar een **klant account maken of ophalen** in de CRM-actie om een **land** waarde toe te wijzen aan het juiste veld in het CRM. Verwijder ook de toewijzing van de **land** waarde uit het veld **adres 1: land/regio** .

   - Voor een veld op basis van opzoek code in het account:
     - Voeg een nieuw aangepast veld toe aan het account en vul het automatisch in met een land code van twee letters (ISO 3166) op basis van de waarde die is geselecteerd in het veld op basis van zoek opdrachten en omgekeerd.
     - Volg de bovenstaande stappen voor het veld niet-opzoek land code om een nieuw aangepast veld te synchroniseren vanuit CRM naar en van partner centrum.

- **Opportuniteits velden**: als er verplichte velden in de **Opportunity** moeten worden ingevuld, bewerkt u **[aanpassen] maken of ophalen van de Dynamics 365-stroom** en gaat u naar een **verkoop kans maken of bijwerken** in de CRM-en update **maakt u een nieuwe opportuniteits actie** om waarden toe te wijzen aan de verplichte velden op basis van uw bedrijfs vereisten.
- **Velden voor lead**: als er verplichte velden aanwezig zijn in de **lead** die moet worden gevuld, bewerken **[aanpassen] maken of ophalen van de Dynamics 365-stroom** en gaat u naar een **lead maken of bijwerken** in de CRM en update **maakt u een nieuwe lead-actie** om waarden toe te wijzen aan de verplichte velden op basis van uw bedrijfs vereisten.
- **Klant account**: wanneer een nieuwe verwijzing wordt gesynchroniseerd van het partner centrum naar de CRM, wordt in de oplossing voor het automatiseren van energie beheer gezocht naar een bestaand account in de CRM met behulp van de bedrijfs naam en post code van de klant. Als er er geen wordt gevonden, wordt er een nieuw klant account gemaakt in de CRM. Als u de zoek criteria en nieuwe Details voor het maken van het account wilt bijwerken, bewerkt u **[aanpassen] maken of ophalen van de Dynamics 365-stroom** en gaat u naar **klant account maken of ophalen** in de CRM- **account actie** voor het maken van een klant.

## <a name="update-environment-variable"></a>Omgevings variabele bijwerken

De waarde van een omgevings variabele bijwerken:

1. Ga naar de pagina **oplossingen** en selecteer **standaard oplossing**. Selecteer **omgevings variabele** door **alle** te selecteren.

1. Selecteer de omgevings variabele voor de waarde die moet worden bijgewerkt en selecteer **bewerken** met behulp van het pictogram met het weglatings teken.

1. **Huidige waarde** bijwerken (de **standaard waarde** niet bijwerken) met behulp van de optie **nieuwe waarde** en de waarde opgeven. De waarde moet overeenkomen met het gegevens type van de variabele. Bijvoorbeeld: het gegevens type Ja of Nee accepteert ofwel de waarde Ja of Nee.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Scherm opname van de weer gave van omgevings variabelen voor updates.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>End-to-end bidirectionele verwijzings synchronisatie voor samen verkoop

Nadat u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Dynamics 365 en partner centrum.

### <a name="prerequisites"></a>Vereisten

Voor het synchroniseren van de verwijzingen tussen partner centrum en Dynamics 365 CRM, is de oplossing voor het automatiseren van de stroom een duidelijke verwijzings velden van micro soft. Met deze identificatie kunnen uw verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.

Er wordt een set aangepaste velden en objecten toegevoegd als onderdeel van de oplossings installatie. Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .

De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:

- **Synchroniseren met partner centrum**: of u de opportuniteit synchroniseert met het partner centrum. De waarde van dit veld is standaard Nee en moet expliciet worden ingesteld op Ja door uw verkoper om een verkoop kans met micro soft te delen. Voor nieuwe verwijzingen die worden gedeeld door het partner centrum naar CRM, wordt deze veld waarde ingesteld op Ja.
- **Verwijzings-id**: een veld met de id alleen-lezen voor de referral van het partner centrum.
- **Verwijzings koppeling**: een alleen-lezen koppeling naar de verwijzing in het partner centrum.
- **Hoe kan ik Help** van micro soft helpen bij het aanwijzen van de verwijzing. Als u een verwijzing naar een mede verkoop wilt maken, selecteert u de juiste Help van micro soft. Een contact persoon van de klant moet zijn gekoppeld aan de mogelijkheid om een verwijzing naar een gezamenlijk verkoop te maken. Als u een verwijzing naar een niet-gezamenlijk verkoop wilt maken, selecteert u dit veld niet. Een verwijzing naar een niet-gezamenlijk verkoop kan op elk gewenst moment worden geconverteerd naar een verwijzing naar een gezamenlijk verkoop punt door de juiste optie voor Help vereist te selecteren.
- **Zicht baarheid van micro soft Partner Center-Referral**: Selecteer zicht baarheid voor de referral van het partner centrum. Als je het object zichtbaar maakt voor verkopers van micro soft, wordt een verwijzing naar een niet-gezamenlijk verkoop object mogelijk geconverteerd naar co-sell. Wanneer micro soft Help is vereist, is de verwijzing standaard zichtbaar voor verkopers van micro soft. Nadat dit veld is gemarkeerd als zichtbaar, kan het niet worden hersteld.
- **Micro soft CRM-id**: wanneer een verwijzing naar een gezamenlijk verkoop wordt gemaakt en geaccepteerd door micro soft, wordt dit veld gevuld met de CRM-id van micro soft.
- **Producten: verouderd**: gebruik dit veld niet of Voeg het toe aan de sectie CRM. Het is alleen beschikbaar voor compatibiliteit met eerdere versies. Gebruik in plaats daarvan Partner Center-oplossingen.
- **Controle**: een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen.
- **Micro soft Partner Center-oplossingen**: een aangepast object voor het koppelen van kant-en-klare oplossingen en micro soft-oplossingen met de kans. Er kunnen een of meer oplossingen worden toegevoegd aan of verwijderd uit de verkoop kans. Het is verplicht om ten minste één kant-en-klare oplossing toe te voegen aan de verkoop kans voordat u deze deelt met micro soft. Als u dit object aan de verkoop kans wilt koppelen, werkt u het **verkoopkansformulier** in de CRM bij.

  Selecteer het juiste tabblad in het **verkoopkansformulier** en voeg een subraster toe, zoals hier wordt weer gegeven.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Scherm opname van het formulier Verkoop kans.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Scherm opname van micro soft-oplossingen.":::

- Nadat u micro soft-oplossingen hebt toegevoegd, kunt u de details van de kant-en-klare oplossing vooraf invullen zodat uw verkopers deze niet hoeven toe te voegen. Als u een nieuwe oplossings detail wilt toevoegen, gaat u naar het object micro soft Solution Details in het CRM en selecteert u **record toevoegen** om één item toe te voegen of **Excel-upload** gebruiken om meerdere vermeldingen toe te voegen.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Scherm afbeelding met nieuwe Details van de micro soft-oplossing.":::

### <a name="scenarios"></a>Scenario's

1. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in de CRM en gesynchroniseerd in partner centrum:

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving met de gebruiker met zicht baarheid in het gedeelte **verkoop kansen** van de CRM.

   1. Zorg ervoor dat de sectie **micro soft Partner Center** aanwezig is wanneer u een nieuwe opportuniteit maakt in de Dynamics 365-omgeving.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Scherm opname waarin nieuwe kansen worden weer gegeven.":::

   1. Als u deze verkoop kans met partner centrum wilt synchroniseren, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:

      - **Hoe kan ik hulp krijgen?**: als u een verwijzing naar een gezamenlijk verkoop punt wilt maken, selecteert u de gewenste optie.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Scherm afbeelding die laat zien hoe u de juiste velden kunt ophalen in de kaart weergave.":::

      - **Contact persoon** van de klant: als u een verwijzing naar een mede verkoop wilt maken, voegt u een contact persoon voor klanten toe aan de verkoop kans.
      - **Synchroniseren met partner centrum**: Ja.
      - **Micro soft-oplossingen**: als u een verwijzing met micro soft wilt delen, moet u een geldige oplossing voor samen verkoop van ready of micro soft toevoegen aan de verkoop kans.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Scherm opname van de oplossings-ID.":::

   1. Nadat de opportunity is gemaakt in Dynamics 365 en de optie **synchroniseren met partner Center** is ingesteld op Ja, wacht u 10 minuten. Meld u vervolgens aan bij uw partner centrum-account. Uw verwijzingen worden gesynchroniseerd met Dynamics 365 en de **verwijzings-id**. **Verwijzings koppeling** wordt gevuld. Als er een fout optreedt, wordt het **controle** veld ingevuld met fout gegevens.
     
    1. Op dezelfde manier wordt voor een verkoop kans waarvoor de optie voor de **Partner Center** is ingesteld op Ja, de wijzigingen worden gesynchroniseerd in uw partner centrum-account als u de opportuniteit bijwerkt in Dynamics 365 CRM.

    1. Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Dynamics 365.

1. Referentie synchronisatie wanneer de referral wordt gemaakt of bijgewerkt in het partner centrum en wordt gesynchroniseerd in de Dynamics 365-omgeving:

   1. Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).

   1. Selecteer **verwijzingen** in het menu links.

   1. Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door de optie **nieuwe deal** te selecteren.

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving.

   1. Ga naar **Open verkoop kansen**. De verwijzing die is gemaakt in Partner Center is nu gesynchroniseerd in Dynamics 365 CRM.

   1. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)
- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
- [Meer informatie over het micro soft-platform voor energie automatisering](/power-automate/)
- [Partnercentrum-webhooks](/partner-center/develop/partner-center-webhooks)
