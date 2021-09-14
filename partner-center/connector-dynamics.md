---
title: De connector voor co-verkoop voor Dynamics 365 CRM Partner Center
description: Synchroniseer verwijzingen in Partner Center met uw connector voor co-verkoop voor Dynamics 365 CRM. U kunt vervolgens samen met Microsoft verkopen vanuit uw CRM-systeem.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 798a8a7d26480e8a1fc23bca3af45bd6a0e44778
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244971"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Overzicht van de connector voor co-sell voor Dynamics 365 CRM

**Juiste rollen:** Beheerdersrechten voor verwijzingen | Systeembeheerder of systeem aanpassen op het CRM

Partner Center connectors voor co-verkoop kunnen uw verkopers samen met Microsoft verkopen vanuit uw CRM-systemen (Customer Relationship System). Ze moeten niet worden getraind voor het gebruik van Partner Center om deals voor co-verkoop te beheren. Gebruik de connectors voor co-verkoop om een nieuwe verwijzing voor co-verkoop te maken naar:

- Een Microsoft-verkoper betrekken
- Verwijzingen ontvangen van de Microsoft-verkoper
- Verwijzingen accepteren of weigeren
- Dealgegevens wijzigen, zoals dealwaarde en einddatum 
 
U kunt ook updates ontvangen van de Microsoft-verkopers over deze deals voor co-verkoop. U kunt al uw verwijzingen beheren in het CRM van uw keuze in plaats van in Partner Center.

De oplossing is gebaseerd op Power Automate en maakt gebruik van Partner Center API's.

## <a name="prerequisites"></a>Vereisten

Voordat u de oplossing installeert, moet u ervoor zorgen dat u aan de volgende vereisten voldoet.

| Onderwerpen   | Details   | Koppelingen   |
|--------------|--------------------|------|
| Microsoft Partner Network-id (MPN) |U hebt een geldige MPN-id nodig. | [Deelnemen aan het partnernetwerk](https://partner.microsoft.com/) |
| Gereed voor co-verkoop|Uw IP/Services-oplossing moet klaar zijn voor co-verkoop. | [Verkopen met Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft) |
| Partnercentrum-account | De MPN-id die is gekoppeld aan Partner Center tenant moet gelijk zijn aan de MPN-id die is gekoppeld aan uw oplossing voor co-verkoop. Controleer of u uw verwijzingen voor co-verkoop kunt zien in de Partner Center portal voordat u de connectors implementeert. | [Uw account beheren](create-user-accounts-and-set-permissions.md) |
| Partner Center gebruikersrollen | De werknemer die de connectors gaat installeren en gebruiken, moet een verwijzingsbeheerder zijn.|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md) |
| Dynamics 365 CRM|De CRM-gebruikersrol is Systeembeheerder of Systeem aanwijzer.|[Rollen toewijzen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization) |
| Power Automate flow-account|Maak een nieuwe productieomgeving met een database voor testen, fasering en productie. Als u een bestaande productieomgeving met een database hebt, kan deze opnieuw worden gebruikt. De gebruiker die de connectoroplossing gaat installeren, moet een licentie voor Power Automate en toegang tot deze omgeving hebben. U kunt de voortgang controleren en meer informatie in de [Power Automate](https://flow.microsoft.com/) als de installatie mislukt. Selecteer **Geschiedenis bekijken onder** **Oplossingen**. | [Omgeving maken of beheren](/power-platform/admin/create-environment#create-an-environment-with-a-database) |

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Synchronisatie Partner Center verwijzingen installeren voor Dynamics 365 (Power Automate oplossing)

1. Ga naar [Power Automate](https://flow.microsoft.com)en selecteer **Omgevingen** in de rechterbovenhoek. In deze stap ziet u de beschikbare CRM-exemplaren.

2. Selecteer het juiste CRM-exemplaar in de vervolgkeuzelijst in de rechterbovenhoek.

3. Selecteer **Oplossingen** aan de linkerkant.

4. Selecteer de **koppeling AppSource** openen in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Schermopname van Open AppSource.":::

5. Zoek naar **Partner Center connectors voor Dynamics 365** in het pop-upscherm.  

6. Selecteer de **knop Nu krijgen** en selecteer vervolgens **Doorgaan.**

7. Er wordt een pagina weergegeven waar u de CRM-omgeving (Dynamics 365) kunt selecteren om de toepassing te installeren. Ga akkoord met de voorwaarden.

8. U kunt de voortgang controleren en als de installatie mislukt, kunt u meer informatie vinden in Power Automate door Geschiedenis bekijken te selecteren **onder** **Oplossingen**.

9. Nadat de installatie is voltooid, gaat u terug [naar Power Automate](https://flow.microsoft.com) selecteert u **Oplossingen** aan de linkerkant. **Partner Center Verwijzingssynchronisatie voor Dynamics 365** is nu beschikbaar in de **lijst oplossingen.**

10. Selecteer **Partner Center Verwijzingssynchronisatie voor Dynamics 365.** De volgende Power Automate en entiteiten zijn beschikbaar.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Schermopname met beschikbare CRM's.":::

## <a name="test-before-you-go-live"></a>Testen voordat u live gaat

Voordat u de oplossing installeert, configureert en Power Automate in de productieomgeving, test u de oplossing op een faserings-CRM-exemplaar. U moet het volgende doen:

- Installeer de Power Automate oplossing op een CRM-exemplaar van een faseringsomgeving.
- Configureer en pas de Power Automate oplossing in een faseringsomgeving aan.
- Test de oplossing op een faserings-CRM-exemplaar.
- Na een geslaagde test importeert u als een beheerde oplossing naar het productie-exemplaar.

## <a name="configure-the-solution"></a>De oplossing configureren

1. Nadat u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Power Automate](https://flow.microsoft.com/).

2. Selecteer in **de** vervolgkeuzelijst Omgevingen in de rechterbovenhoek het CRM-exemplaar waarop u de oplossing Power Automate geïnstalleerd.

3. U moet verbindingen maken die de drie gebruikersaccounts koppelen:

   - Partner Center gebruiker met beheerdersreferenties voor verwijzingen
   - Partnercentrum-gebeurtenissen
   - CRM-beheerder met de Power Automate in de oplossing

   a. Selecteer **Verbindingen aan** de linkerkant en selecteer Partner Center oplossing **Verwijzingen** in de lijst.

   b. Maak een verbinding door Een **verbinding maken te selecteren.**

      :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Schermopname van Een verbinding maken.":::

   c. Zoek naar **Partner Center verwijzingen (preview)** in de zoekbalk in de rechterbovenhoek.

   d. Maak een verbinding voor uw Partner Center met de referentiesrol Van verwijzingsbeheerder.

   e. Maak vervolgens een verbinding Partner Center gebeurtenissen voor uw Partner Center met de referenties van de verwijzingsbeheerder.

   f. Maak een verbinding voor Common Data Service (huidige omgeving) voor de CRM-beheerder.
     
   g. Nadat u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Schermopname van verbindingen.":::

## <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar **de pagina** Oplossingen en selecteer **Standaardoplossing.** Selecteer **Verbindingsverwijzing (preview) door** **Alle te selecteren.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Schermopname van Het bewerken van de verbindingen.":::

2. Bewerk elk van de verbindingen afzonderlijk door het pictogram met het beletselteken te selecteren. Voeg de relevante verbindingen toe.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Schermopname van de vermelde verbindingen.":::

3. Ga terug  naar de pagina Oplossingen, selecteer **Partner Center Verwijzingensynchronisatie voor Dynamics 365** en schakel de stroom in door het beletselteken naast elke stroom in de volgende volgorde te selecteren. Zie Aanpassingsstappen en Stappen voor probleemoplossing als u problemen ondervindt tijdens het [in-/uit-zetten van de stroom.](connectors-troubleshoot.md) [](connector-dynamics.md#customize-synchronization-steps)

   Schakel de stromen in de volgende volgorde in:

   a. Partner Center webhookregistratie (Insider Preview)
   
   b. [Aanpassen] Details maken of op halen uit dynamics 365-stroom
   
   c. Verwijzing voor co-verkoop maken : Dynamics 365 naar Partner Center (Insider Preview)
   
   d. Partner Center naar Dynamics 365 - Helper (Insider Preview)
   
   e. Partner Center Microsoft Co-sell Verwijzingsupdates voor Dynamics 365 (Insider Preview)
   
   f. Partner Center naar Dynamics 365 (Insider Preview)
   
   g. Dynamics 365 to Partner Center (Insider Preview)
   
   h. Dynamics 365 Opportunity to Partner Center (Insider Preview)
   
   i. Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-API's gebruiken om te registreren voor resourcewijzigingsgebeurtenissen

U kunt de api'Partner Center webhook gebruiken om u te registreren voor gebeurtenissen voor resourcewijziging. Deze wijzigingsgebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Selecteer **Partner Center Dynamics 365 (Insider Preview)**.

2. Selecteer het **pictogram** Bewerken en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen.**

3. Selecteer het **pictogram Kopiëren** om de opgegeven HTTP POST-URL te kopiëren.

   :::image type="content" source="images/webhook-video.gif" alt-text="Schermopname van het gebruik van webhooks om resourcewijzigingen te registreren.":::

4. Selecteer de **Partner Center webhookregistratie (Insider Preview) Power Automate** selecteer vervolgens **Uitvoeren.**

5. Zorg ervoor dat **het venster Stroom** uitvoeren wordt geopend in het rechterdeelvenster en selecteer **Doorgaan.**

6. Voer de volgende details in:

   - **Http Trigger-eindpunt:** deze URL is uit een eerdere stap gekopieerd.
   - **Te registreren gebeurtenissen:** selecteer alle beschikbare gebeurtenissen ( verwijzing **gemaakt,** **verwijzing bijgewerkt,** **related-referral-created** en **related-referral-updated).**
   - **Bestaande trigger-eindpunten overschrijven, indien aanwezig?**: Ja. Er kan slechts één URL worden geregistreerd voor een bepaalde webhookgebeurtenis.

7. Selecteer **Stroom uitvoeren** en selecteer vervolgens **Done.**

De webhook kan nu luisteren naar gebeurtenissen, deze maken en bijwerken.

## <a name="customize-synchronization-steps"></a>Synchronisatiestappen aanpassen

CRM-systemen zijn zeer aangepast en u kunt de Power Automate aanpassen op basis van uw CRM-configuratie. Wanneer verwijzingen voor co-verkoop worden gesynchroniseerd tussen Partner Center en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-pc weergegeven in de handleiding voor aangepaste [veldtoewijzing.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)

Volg de handleiding voor veldtoewijzing en, indien nodig, de juiste wijzigingen aan te brengen in [Aanpassen] Maken of Details op halen uit **Dynamics 365-stroom-** of omgevingsvariabelen. Werk geen andere stromen in de Power Automate bij omdat dit van invloed kan zijn op toekomstige oplossingsupgrades.

De volgende aanpassingen zijn beschikbaar:

- **Vinkje weergeven in** de naam van de kans: standaard wordt er een vinkje weergegeven naast de naam van de kans om aan te geven dat de synchronisatie tussen Partner Center en Dynamics 365 CRM is geslaagd. Op dezelfde manier wordt er een kruis markering weergegeven als de synchronisatie mislukt. Stel de huidige waarde van het vinkje Weergeven **in** de omgevingsvariabele naam van de kansnaam in op Nee om te voorkomen dat er een vinkje of kruisval in de naam van de kans wordt toegevoegd.
- **Dealwaarde:** standaard wordt de dealwaarde van Partner Center gesynchroniseerd naar en `estimatedvalue` van in het CRM. Als u een ander veld in het CRM hebt om de dealwaarde te synchroniseren vanuit:

  - Werk de **veldnaam dealwaarde** in de Dynamics 365-omgevingsvariabele bij met de veldnaam van het CRM. Zorg ervoor dat u de naam van het veld op geeft, niet de weergavenaam.
  - Bewerk [Aanpassen] Maak of haal details op uit de **Dynamics 365-stroom,** ga  naar Kans maken of bijwerken **in** CRM en werk Een nieuwe kans maken en Bestaande kansenacties bijwerken bij om de **waarde DealValue** toe te wijzen aan het juiste veld in het CRM.  Verwijder ook de **toewijzing DealValue** uit het **veld Geschatte** omzet.

- **Landcode van klantaccount:** u moet een tweeletterig landnummer (ISO 3166) verstrekken wanneer u een nieuwe verwijzing maakt. Standaard wordt de landcode gesynchroniseerd naar en van het veld address1_country **account** in het CRM. Als u een ander veld in het CRM hebt om de landcode te synchroniseren vanuit:

  - Voor een niet-lookup landnummerveld in het account dat  een tweeletterig code bevat, moet u de veldnaam voor de landcode van het klantaccount bijwerken in de Dynamics 365-omgevingsvariabele met de veldnaam van het CRM. Zorg ervoor dat u de naam van het veld op geeft, niet de weergavenaam. Bewerk [Aanpassen] Maak of haal details op uit **de Dynamics 365-stroom** en  ga naar Klantaccount maken of krijgen **in** de CRM-actie om een landwaarde toe te wijzen aan het juiste veld in het CRM. Verwijder ook de **waardetoewijzing Land** uit het **veld Adres 1: Land/regio.**

  - Voeg voor een veld op basis van opzoeklandcode in het account een nieuw aangepast veld toe aan het account en vul het automatisch in met een tweeletterig landnummer (ISO 3166) op basis van de waarde die is geselecteerd in het opzoekveld en vice versa. Volg de voorgaande stappen voor het veld nonlookup country code om een nieuw aangepast veld te synchroniseren van het CRM naar en van Partner Center.

- **Opportunity-velden:** als er verplichte velden **in** Opportunity moeten worden ingevuld, bewerkt u **[Aanpassen] Create or Get Details from Dynamics 365 flow** en gaat u naar Create or update **opportunity** in the CRM (Een nieuwe kans-actie maken) om waarden toe te wijzen aan de verplichte velden op basis van uw zakelijke vereisten. 
- **Leadvelden:** als er verplichte velden in **Lead** zijn die moeten worden ingevuld, bewerkt **u [Aanpassen] Create or Get Details from Dynamics 365 flow** en gaat u naar Create or update **lead** in the CRM (Lead maken of bijwerken) en werkt u Create a new lead action (Een nieuwe **leadactie** maken) bij om waarden toe te wijzen aan de verplichte velden op basis van uw bedrijfsvereisten.
- **Klantaccount:** wanneer een nieuwe verwijzing vanuit Partner Center wordt gesynchroniseerd met het CRM, probeert de Power Automate-oplossing te zoeken naar een bestaand account in het CRM met behulp van de bedrijfsnaam en postcode van de klant. Als er geen klantaccount wordt gevonden, wordt er een nieuw klantaccount gemaakt in het CRM. Als u de zoekcriteria en details voor het maken van nieuwe account wilt bijwerken, bewerkt u [Aanpassen] Maken of Details op halen uit **de Dynamics 365-stroom** en gaat u naar Klantaccount maken **of** krijgen in de CRM- en Klantaccountactie **maken.**

## <a name="update-environment-variable"></a>Omgevingsvariabele bijwerken

De waarde van een omgevingsvariabele bijwerken:

1. Ga naar de **pagina Oplossingen** en selecteer **Standaardoplossing.** Selecteer **Omgevingsvariabele** door **Alle te selecteren.**

2. Selecteer de omgevingsvariabele voor de waarde die moet worden bijgewerkt en selecteer **Bewerken** met behulp van het beletselteken.

3. Werk **de huidige waarde** bij (werk de **standaardwaarde niet bij** met behulp van de optie Nieuwe **waarde** en geef de waarde op. De waarde moet overeenkomen met het gegevenstype van de variabele. Het gegevenstype Ja of Nee accepteert bijvoorbeeld de waarde Ja of Nee.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Schermopname van Omgevingsvariabelen bijwerken.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Verwijzingssynchronisatie van end-to-end bidirectionele co-verkoop

Nadat u de Power Automate-oplossing hebt geïnstalleerd, geconfigureerd en aangepast, kunt u testen op synchronisatie van verwijzingen voor co-verkoop tussen Dynamics 365 en Partner Center.

### <a name="prerequisites"></a>Vereisten

Om de verwijzingen in Partner Center en Dynamics 365 CRM te synchroniseren, wordt in de Power Automate-oplossing duidelijk de microsoft-specifieke verwijzingsvelden afgebakend. Deze identificatie geeft uw verkopersteams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.

Er wordt een set aangepaste velden en objecten toegevoegd als onderdeel van de installatie van de oplossing. Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden **voor** kansen.

De volgende aangepaste velden moeten deel uitmaken van de CRM-sectie:

- **Synchroniseren met Partner Center:** of de kans moet worden gesynchroniseerd met Partner Center. De waarde van dit veld is standaard Nee en moet expliciet worden ingesteld op Ja door uw verkoper om een verkoopkans met Microsoft te delen. Voor nieuwe verwijzingen die worden gedeeld Partner Center CRM wordt deze veldwaarde ingesteld op Ja.
- **Verwijzings-id:** een veld alleen-lezen-id voor de Partner Center verwijzing.
- **Verwijzingskoppeling:** een alleen-lezenkoppeling naar de verwijzing in Partner Center.
- **Hoe kan Microsoft u helpen?**: Hulp vereist van Microsoft voor de verwijzing. Als u een verwijzing voor co-verkoop wilt maken, selecteert u de juiste hulp die Microsoft nodig heeft. Een contactpersoon van een klant moet worden gekoppeld aan de mogelijkheid om een verwijzing voor co-verkoop te maken. Als u een verwijzing voor niet-co-verkoop wilt maken, selecteert u dit veld niet. Een verwijzing voor niet-co-verkoop kan op elk gewenst moment worden geconverteerd naar een verwijzing voor co-verkoop door de gewenste optie voor hulp te selecteren.
- **Zichtbaarheid van Partner Center Microsoft-verwijzing:** selecteer zichtbaarheid voor de Partner Center verwijzing. Door deze zichtbaar te maken voor Microsoft-verkopers, kan een verwijzing voor niet-co-verkoop worden geconverteerd naar co-verkoop. Wanneer Microsoft Help vereist is, is de verwijzing standaard zichtbaar voor Microsoft-verkopers. Nadat dit veld als zichtbaar is gemarkeerd, kan het niet worden teruggedraaid.
- **Microsoft CRM-id:** wanneer er een verwijzing voor co-verkoop wordt gemaakt en geaccepteerd door Microsoft, wordt dit veld gevuld met de CRM-id van Microsoft.
- **Producten: verouderd:** gebruik dit veld niet en voeg het niet toe aan de CRM-sectie. Deze is alleen beschikbaar voor achterwaartse compatibiliteit. Gebruik Partner Center oplossingen.
- **Controleren:** een alleen-lezen audittrail voor synchronisatie met Partner Center verwijzingen.
- **Microsoft Partner Center Solutions:** een aangepast object om oplossingen die gereed zijn voor co-verkoop of Microsoft-oplossingen te koppelen aan de verkoopkans. Een of meer oplossingen kunnen worden toegevoegd aan of verwijderd uit de mogelijkheid. Het is verplicht om ten minste één kant-en-klaar oplossing voor co-verkoop of Microsoft aan de verkoopkans toe te voegen voordat u deze met Microsoft deelt. Als u dit object wilt koppelen aan de mogelijkheid, moet u het formulier **Opportunity** in het CRM bijwerken.

  Selecteer het juiste tabblad op het formulier **Opportunity** en voeg een subraster toe zoals hier wordt weergegeven.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Schermopname van het formulier Opportunity.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Schermopname van Microsoft Solutions.":::

- Nadat u Microsoft-oplossingen hebt toevoegen, kunt u de oplossingsdetails voor co-verkoop vooraf invult, zodat uw verkopers deze niet hoeven toe te voegen. Als u een nieuw oplossingsdetail wilt toevoegen, gaat u naar het object  Microsoft Solution Details in het CRM en selecteert u **Record toevoegen** om één vermelding toe te voegen of gebruikt u Excel uploaden om meerdere vermeldingen toe te voegen.

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="Schermopname met details van nieuwe Microsoft-oplossing.":::

### <a name="scenarios"></a>Scenario's

1. Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in het CRM en wordt gesynchroniseerd in Partner Center:

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving met de gebruiker die zichtbaarheid heeft in de **sectie Opportunity** van het CRM.

   1. Zorg ervoor dat de **sectie Microsoft Partner Center** aanwezig is wanneer u een nieuwe kans maakt in de Dynamics 365-omgeving.

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="Schermopname van Nieuwe kans.":::

   1. Als u deze mogelijkheid wilt synchroniseren met Partner Center, moet u de volgende velden instellen in de kaartweergave:

      - **Hoe kan Microsoft u helpen?**: als u een verwijzing voor co-verkoop wilt maken, selecteert u een geschikte Help-optie.

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="Schermopname die laat zien hoe u de juiste velden in de kaartweergave op kunt halen.":::

      - **Klantcontact:** als u een verwijzing voor co-verkoop wilt maken, voegt u een contactpersoon van een klant toe aan de verkoopkans.
      - **Synchroniseren met Partner Center:** Ja.
      - **Microsoft Solutions:** als u een verwijzing met Microsoft wilt delen, voegt u een geldige, kant-en-klaar oplossing voor co-verkoop of Microsoft-oplossing toe aan de verkoopkans.

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="Schermopname met oplossings-id.":::

   1. Nadat de kans is gemaakt in Dynamics 365, met de optie Synchroniseren **Partner Center** ingesteld op Ja, wacht u 10 minuten. Meld u vervolgens aan bij uw Partner Center account. Uw verwijzingen worden gesynchroniseerd met Dynamics 365 en **Verwijzings-id**. **Verwijzingskoppeling** wordt ingevuld. Als er een fout is opgetreden, wordt het **veld** Controle gevuld met foutgegevens.

      1. Voor een kans waarin de optie Synchroniseren met **Partner Center** is ingesteld op Ja, worden de wijzigingen in uw Partner Center-account gesynchroniseerd als u de mogelijkheid in Dynamics 365 CRM bij Partner Center bijgewerkt.

      1. Verkoopkansen die zijn gesynchroniseerd met Partner Center worden geïdentificeerd met ✔ in Dynamics 365.

1. Verwijzingssynchronisatie wanneer de verwijzing wordt gemaakt of bijgewerkt in Partner Center en gesynchroniseerd in de Dynamics 365-omgeving:

   1. Meld u aan bij uw Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).

   1. Selecteer **Verwijzingen in** het menu links.

   1. Maak een nieuwe verwijzing voor co-verkoop vanuit Partner Center door de optie **Nieuwe deal te** selecteren.

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving.

   1. Ga naar **Open verkoopkansen.** De verwijzing die is gemaakt in Partner Center is nu gesynchroniseerd in Dynamics 365 CRM.

   1. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de details van de kaartweergave ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)
- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
- [Meer informatie over het Microsoft Power Automate platform](/power-automate/)
- [Partnercentrum-webhooks](/partner-center/develop/partner-center-webhooks)
