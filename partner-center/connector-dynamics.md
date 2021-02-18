---
title: De connector voor het samen verkopen van Dynamics 365 CRM-partner centrum
ms.topic: how-to
ms.date: 02/16/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniseer verwijzingen in het partner centrum met de connector voor co-sell voor Dynamics 365 CRM. Verkopers kunnen vervolgens samen met micro soft verkopen binnen uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: e465130b96886cf2bb77bcd94f56c1a12545a5d5
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645706"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Connector voor Dynamics 365-overzicht co-sell

### <a name="appropriate-roles"></a>Juiste rollen

- Beheerder van verwijzingen
- Systeem beheerder of systeemaanpasser op de CRM

Met connector voor co-sell van partner Center kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen. Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop. Gebruik de co-Connect connectors om een nieuwe verwijzing naar de verkoop te maken voor een micro soft-verkoper, referenties te ontvangen van de micro soft-verkoper, verwijzingen te accepteren/weigeren, afhandelings gegevens te wijzigen, zoals een deal waarde en een sluitings datum. U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals. U kunt al uw referenties beheren in de CRM van uw keuze in plaats van in het partner centrum. 

De oplossing is gebaseerd op de micro soft-oplossing voor energie automatisering en maakt gebruik van partner Center-Api's.

## <a name="before-you-install---pre-requisites"></a>Voordat u de vereisten installeert

|**Onderwerpen**   |**Details**   |**Koppelingen**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |U hebt een geldige MPN-ID nodig|Toevoegen aan [MPN](https://partner.microsoft.com/)|
|Klaar voor de verkoop|Uw IP/Services-oplossing moet samen worden verkocht.|[Verkopen met micro soft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercentrum-account|De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling. Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in partner centrum Portal kunt zien.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Gebruikers rollen voor het partner centrum|De werk nemer die de connectors installeert en gebruikt, moet een referentie beheerder zijn|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser|[Rollen toewijzen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Stroom account voor energie automatisering|Maak een nieuwe productie omgeving met een Data Base voor testen/fase ring en productie. Als u een bestaande productie omgeving met Data Base hebt, kunt u deze opnieuw gebruiken. Gebruiker die connector oplossing gaat installeren, moet beschikken over een automatische licentie en toegang tot deze omgeving. U kunt de voortgang controleren en meer Details ophalen. als de installatie mislukt [, klikt u op geschiedenis](https://flow.microsoft.com/) weer geven onder oplossingen.|[Omgeving maken of beheren](https://docs.microsoft.com/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Synchronisatie van partner Center referrals voor Dynamics 365 (oplossing voor automatische stroom) installeren

1. Ga naar [Automatische stroom](https://flow.microsoft.com) en selecteer **omgevingen** in de rechter bovenhoek. In deze stap ziet u de beschik bare CRM-exemplaren.

2. Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.

3. Selecteer **oplossingen** op de linkernavigatiebalk.

4. Klik op de koppeling **Open AppSource** in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource openen":::

5. Zoek naar **Partner Center referrals connectors voor Dynamics365** in het pop-upvenster.  

6. Klik op de knop **nu downloaden** en vervolgens op **door gaan**.

7. Hiermee opent u de pagina waar u de CRM-omgeving (Dynamics 365) kunt selecteren om de toepassing te installeren.  Ga akkoord met de voor waarden.

8. U kunt de voortgang controleren en meer Details ophalen. als de installatie mislukt, klikt u op **geschiedenis weer geven** onder **oplossingen**.
 

9. Zodra de installatie is voltooid, gaat u terug naar [energie automatisering](https://flow.microsoft.com) en selecteert u **oplossingen** vanuit het navigatie gebied links. U ziet dat **Partner Center referrals synchronisatie voor Dynamics 365** beschikbaar is in de lijst met oplossingen.

10. Selecteer de **synchronisatie van partner Center referrals voor Dynamics 365**. De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Beschik bare CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Best practice: test voordat u live gaat

Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test.

- Installeer de oplossing voor het automatiseren van micro soft power op een staging-omgeving/CRM-exemplaar.
- Configureer en pas de micro soft-oplossing voor het automatiseren van energie aan in faserings omgeving.
- Test de oplossing op een staging/CRM-exemplaar. 
- Importeer bij geslaagd als beheerde oplossing naar het productie-exemplaar. 

## <a name="configure-the-solution"></a>De oplossing configureren

1. Wanneer u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Automatische stroom](https://flow.microsoft.com/).


2. Selecteer in de vervolg keuzelijst **omgevingen** in de rechter BOVENHOEK het CRM-exemplaar waarop u de oplossing voor het automatiseren van energie beheer hebt geïnstalleerd.

3. U moet verbindingen maken die de drie gebruikers accounts koppelen:

   - Partner centrum-gebruiker met referrals beheerders referenties

   - Partnercentrum-gebeurtenissen

   - CRM-beheerder met de stroom voor het automatiseren van stromen in de oplossing.

      1. Selecteer **verbindingen** in de linkernavigatiebalk en selecteer de oplossing Partner Center referrals in de lijst.

      2. Maak een verbinding door te klikken op **een verbinding maken**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Verbinding maken":::

      3. Zoek naar **Partner Center referrals (preview)** in de zoek balk in de rechter bovenhoek.

      4. Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.

      5. Maak vervolgens een verbinding met de partner centrum-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de beheerder.

      6. Maak een verbinding voor Common Data Service (huidige omgeving) voor de gebruiker van de CRM-beheerder.
     
      7. Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Verbindingen":::
   
## <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar de pagina **oplossingen** en selecteer **standaard oplossing**. Selecteer **verbindings verwijzing (preview)** door te klikken op **alle**.

:::image type="content" source="images/cosellconnectors/dynamics-3.png" alt-text="Verbinding maken":::

2. Bewerk elk van de verbindingen één voor één door het pictogram drie punten te selecteren. Voeg de relevante verbindingen toe.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Verbindingen vermeld"::: 

3.  Ga terug naar de pagina oplossingen, selecteer de synchronisatie van partner Center referrals voor Dynamics 365 en schakel de stroom in door te klikken op het pictogram drie punten naast elke stroom in de volgende reeks. Zie [aanpassings stappen](connector-dynamics.md#customize-synchronization-steps) en [stappen voor probleem oplossing](connectors-troubleshoot.md)als u problemen ondervindt bij het inschakelen van de stroom. 

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

Met de webhook-Api's van partner Center kunt u zich registreren voor bron wijzigings gebeurtenissen. Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Selecteer **partner centrum voor Dynamics 365 (Insider preview)**.

2. Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen**.

3. Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL kopiëren":::

4. Selecteer nu de stroom voor het automatiseren van partner Center-webhooks (Insider preview) en selecteer **uitvoeren**.

5. Zorg ervoor dat het venster stroom uitvoeren wordt geopend in het rechterdeel venster en klik op **door gaan**.

6. Voer de volgende details in:

   - **Http-trigger eindpunt**: URL gekopieerd uit eerdere stap

   - **Te registreren gebeurtenissen**: Selecteer alle beschik bare gebeurtenissen (' Referral-created ', ' Referral-updated ', ' Verwante-Referral-created ', ' gerelateerde-Referral-bijgewerkt ')

   -**Bestaande trigger eindpunten overschrijven indien aanwezig**: Ja het is belang rijk te weten dat er slechts één URL kan worden geregistreerd voor een bepaalde webhook-gebeurtenis. Het is belang rijk te weten dat er slechts één URL kan worden geregistreerd voor een bepaalde webhook-gebeurtenis. 

7. Selecteer **uitvoeren** en selecteer vervolgens **gereed.**

De webhook kan nu Luis teren om gebeurtenissen te maken en bij te werken.

## <a name="customize-synchronization-steps"></a>Synchronisatie stappen aanpassen

CRM-systemen zijn zeer aangepast en u kunt de energiebeheer oplossing aanpassen op basis van uw CRM-installatie.  Wanneer verwijzingen naar links worden gesynchroniseerd tussen partner centrum en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-PC weer gegeven in de [hand leiding voor aangepaste veld toewijzing](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Volg de hand leiding voor de veld toewijzing en wijzig indien nodig de juiste wijzigingen in **[aanpassen] Create of Get details van Dynamics 365 flow**  of omgevings variabelen. Het is raadzaam om geen andere stromen bij te werken in de oplossing voor het automatiseren van de oplossing, omdat deze invloed kan hebben op upgrades van toekomstige oplossingen. 

Hier volgen de beschik bare aanpassingen:

- Selectie vakje Opportunity naam: standaard wordt een vinkje weer gegeven naast naam van opportuniteit om aan te geven dat de synchronisatie tussen partner centrum en Dynamics 365 CRM met succes wordt uitgevoerd. Op dezelfde manier wordt een kruis markering weer gegeven als de synchronisatie mislukt. Als u wilt voor komen dat de naam van de verkoop kans wordt gecontroleerd of door gegeven, stelt u de huidige waarde van het selectie vakje voor de weergave naam van de verkoop kans in op Nee.

- Deal waarde: standaard wordt de deal waarde van partner Center gesynchroniseerd van en naar **estimatedvalue** in CRM. Als u een ander veld in CRM hebt voor het afhandelen van waarde om te synchroniseren vanaf:

    a.    De naam van het veld deal waarde bijwerken in de Dynamics 365-omgevings variabele met de naam van het CRM-veld. Houd er rekening mee dat u de naam van het veld niet de weergave naam moet opgeven.

    b.    Bewerken **[aanpassen] Maak of ontvang Details van de Dynamics 365-stroom**  en navigeer naar een opportuniteit **maken of bijwerken** in CRM en update **Maak een nieuwe kans** en **werk de bestaande opportuniteits** acties bij om **DealValue** waarde toe te wijzen aan het juiste veld in CRM. Verwijder ook de **toewijzing DealValue** uit het veld **geschatte omzet** .

- Land code klant account: het is verplicht een land code van twee letters (ISO 3166) op te geven bij het maken van een nieuwe verwijzing. De land code wordt standaard gesynchroniseerd van en van het address1_country veld van het account in CRM. Als u een ander veld in CRM hebt voor de land code waarvan u wilt synchroniseren:

   a.    Voor een niet-opzoek veld land code in account met code van twee letters:

   - De land code veld naam van het klant account bijwerken in de Dynamics 365-omgevings variabele met de naam van het CRM-veld. Houd er rekening mee dat u de naam van het veld niet de weergave naam moet opgeven.

   - Bewerken **[aanpassen] Maak of ontvang Details van de Dynamics 365-stroom**  en navigeer naar het maken of ophalen van klant account in CRM-actie om land waarde toe te wijzen aan het juiste veld in CRM. Verwijder ook de waarde toewijzing van het land uit adres 1: veld land/regio.

   b.    Voor een veld voor een land code op basis van een zoek opdracht in account:

   - Voeg een nieuw aangepast veld toe aan het account en vul het automatisch in met een land code van twee letters (ISO 3166) op basis van de waarde die is geselecteerd in het veld op basis van zoek opdrachten en vice versa.

   - Volg de bovenstaande stappen voor een niet-opzoek land code veld om een nieuw aangepast veld van CRM naar en van het partner centrum te synchroniseren.

- Opportuniteits velden: als er verplichte velden in de verkoop kans moeten worden ingevuld **[aanpassen] maken of ophalen van de Dynamics 365-stroom**  en navigeert u naar een **opportuniteit maken of bijwerken** in CRM en update **maakt u een nieuwe opportuniteits actie** om waarden toe te wijzen aan de verplichte velden op basis van uw bedrijfs vereisten.

- Velden voor potentiële klanten: als er verplichte velden in de lead moeten worden ingevuld **[aanpassen] maken of ophalen van de Dynamics 365-stroom**  en navigeert u naar **maken of bijwerken** van de lead in CRM en update maakt u **een nieuwe lead actie** om waarden toe te wijzen aan de verplichte velden op basis van uw bedrijfs vereisten.

- Klant account: wanneer een nieuwe verwijzing wordt gesynchroniseerd van het partner centrum naar CRM, probeert de oplossing voor het automatiseren van energie te zoeken naar een bestaand account in CRM met behulp van de bedrijfs naam en post code van de klant. Als er geen wordt gevonden, wordt er een nieuw klant account gemaakt in CRM. Als u de zoek criteria en Details van het maken van nieuwe accounts wilt bijwerken, bewerkt u **[aanpassen] maken of ophalen van de Dynamics 365-stroom** en navigeert u naar het **maken of ophalen van een klant account** in CRM en het maken van de actie voor een **klant account**.

## <a name="update-environment-variable"></a>Omgevings variabele bijwerken

De waarde van een omgevings variabele bijwerken:

1. Ga naar de pagina **oplossingen** en selecteer **standaard oplossing**. Selecteer **omgevings variabele** door te klikken op alle.

2. Selecteer de omgevings variabele voor de waarde die moet worden bijgewerkt en klik op **bewerken** met behulp van drie puntjes.

3. Update **huidige waarde** (niet bijwerken standaard waarde) met de optie **nieuwe waarde** en geef de waarde op. De waarde moet overeenkomen met het gegevens type van de variabele voor bijvoorbeeld Ja/Nee-gegevens type accepteert ofwel ja of Nee.

:::image type="content" source="images/cosellconnectors/dynamics-5.png" alt-text="Invoervak voor standaard waarden":::

- End-to-end-synchronisatie van Referral-verkoop referenties

Zodra u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Dynamics 365 en partner centrum.

### <a name="pre-requisites"></a>Vereisten

Voor het synchroniseren van de verwijzingen tussen partner centrum en Dynamics 365 CRM, is de oplossing voor het automatiseren van de stroom een duidelijke verwijzings velden van micro soft. Met deze identificatie kunnen uw verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.

Er wordt een set aangepaste velden en objecten toegevoegd als onderdeel van de oplossings installatie. Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .

De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:

- **Synchroniseren met partner centrum**: of u de mogelijkheid wilt synchroniseren met micro soft Partner Center. De waarde van dit veld is standaard Nee en moet expliciet worden ingesteld op Ja door uw verkoper om een verkoop kans met micro soft te delen. Voor nieuwe verwijzingen die worden gedeeld door het partner centrum naar CRM, wordt deze veld waarde ingesteld op Ja.

- **Verwijzings-id**: een veld met alleen-lezen-id voor micro soft Partner Center Referral

- **Verwijzings koppeling**: een alleen-lezen koppeling naar de verwijzing in het micro soft partner centrum
- **Hoe kan ik Help** van micro soft helpen bij het aanwijzen van de verwijzing. Als u een verwijzing naar een mede verkoop wilt maken, selecteert u de juiste Help van micro soft. Een contact persoon van de klant moet zijn gekoppeld aan de mogelijkheid om een verwijzing naar een gezamenlijk verkoop te maken. Als u een verwijzing naar een niet-co-sell wilt maken, schakelt u dit veld uit. Een verwijzing naar een niet-gezamenlijk verkoop kan op elk gewenst moment worden geconverteerd naar een verwijzing naar de verkoop.

- **Zicht baarheid van micro soft Partner Center-Referral**: Selecteer zicht baarheid voor micro soft Partner Center Referral. Als u het zichtbaar maakt voor verkopers van micro soft, kan een niet-verkoop verwijzing worden geconverteerd naar co-sell. Wanneer micro soft Help is vereist, is Referral standaard zichtbaar voor micro soft-verkopers. Dit veld kan niet worden teruggedraaid als dit is gemarkeerd als zichtbaar.

- **Micro soft CRM-id**: wanneer een verwijzing naar een gezamenlijk verkoop wordt gemaakt en geaccepteerd door micro soft, wordt dit veld gevuld met de CRM-id van micro soft.

- **Producten: verouderd** : gebruik dit veld niet of Voeg het niet toe aan de sectie CRM. het is alleen beschikbaar voor achterwaartse compatibiliteit. Gebruik in plaats daarvan oplossingen van micro soft Partner Center.

- **Controle**: een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen

- **Micro soft Partner Center-oplossingen**: een aangepast object voor het koppelen van kant-en-klare oplossingen en micro soft-oplossingen met de kans. Een of meer oplossingen kunnen worden toegevoegd en/of uit de opportuniteit worden verwijderd. Het is verplicht om ten minste één kant-en-klare oplossing toe te voegen aan de verkoop kans voordat u deze deelt met micro soft. Als u dit object aan de verkoop kansen wilt koppelen, werkt u het formulier Verkoop kans bij in CRM:

  Selecteer het juiste tabblad in het formulier Verkoop kans en voeg een subraster toe, zoals hieronder wordt weer gegeven:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Formulier Verkoop kans":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Nadat u micro soft-oplossingen hebt toegevoegd, kunt u de details van kant-en-klare oplossingen vooraf invullen, zodat uw verkopers deze niet hoeven toe te voegen. Als u een nieuwe oplossings detail wilt toevoegen, gaat u naar micro soft Solution Details object in CRM en klikt u op **record toevoegen** om één item toe te voegen of **Excel-upload** gebruiken om meerdere vermeldingen toe te voegen.

:::image type="content" source="images/dynamic-1a.png" alt-text="Details van oplossing":::

### <a name="scenarios"></a>DENKBAAR

1. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en gesynchroniseerd in partner centrum:

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving met een zicht baarheid in het gedeelte **verkoop kansen** van de CRM.

   2. Zorg ervoor dat het gedeelte van het micro soft Partner Center aanwezig is wanneer u een nieuwe kans maakt in de Dynamics 365-omgeving

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nieuwe kans"::: 

   3. Als u deze verkoop kans met partner centrum wilt synchroniseren, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:

      - **Hoe kan ik hulp krijgen?**: als u een verwijzing naar de verkoop wilt maken, selecteert u een geschikte optie voor de Help.

         :::image type="content" source="images/dynamic-3a.png" alt-text="De juiste velden ophalen in de kaart weergave":::

      - **Contact persoon** van de klant: als u een verwijzing naar de verkoop wilt maken, voegt u een contact persoon van de klant toe aan de opportuniteit.
      - **Synchroniseren met partner centrum**: Ja

      - Micro soft-oplossingen: als u een verwijzing met micro soft wilt delen, voegt u een geldige oplossing voor het samen voegen van de verkoop gereed of micro soft toe.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Id van de oplossing":::

   4. Zodra de opportuniteit is gemaakt in Dynamics 365 met synchronisatie met de optie voor Partner Center is ingesteld op Ja, wacht u 10 minuten en meldt u zich aan bij uw partner centrum-account. Uw verwijzingen worden gesynchroniseerd met Dynamics 365 en de verwijzings-id. Verwijzings koppeling wordt gevuld. Als er een fout optreedt, wordt het controle veld ingevuld met fout gegevens.
     
    5. Voor een verkoop kans waarvoor de optie ' synchroniseren met partner centrum ' is ingesteld op ' ja ' en u de verkoop kans bijwerkt in Dynamics 365 CRM, worden de wijzigingen ook gesynchroniseerd in uw partner centrum-account.

    6. Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Dynamics 365.

2. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in micro soft Partner Center en gesynchroniseerd in de Dynamics 365-omgeving:

   1. Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).

   2. Selecteer **verwijzingen** in het menu aan de linkerkant.

   3. Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door de optie  **nieuwe deal** te selecteren.

   4. Meld u aan bij uw Dynamics 365 CRM-omgeving.

   5. Navigeer naar **Open verkoop kansen**. De verwijzing die is gemaakt in het micro soft Partner Center is nu gesynchroniseerd in Dynamics 365 CRM.

   6. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)

- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)

- [Meer informatie over het platform van micro soft voor energie automatisering?](/power-automate/)

- [Partnercentrum-webhooks](/partner-center/develop/partner-center-webhooks)