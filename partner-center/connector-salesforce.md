---
title: De connector voor co-sell voor Salesforce CRM Partner Center
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Synchroniseer uw verwijzingen in Partner Center met uw Salesforce CRM. Verkopers kunnen vervolgens samen met Microsoft verkopen vanuit uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 4a98bd2e98aa1533806205179812af6507b2a2af
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957079"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connector voor co-verkoop voor Salesforce CRM - overzicht

**Juiste rollen:** Beheerdersrollen voor verwijzingen | Systeembeheerder of systeem aanpassen op het CRM

Partner Center connector voor co-verkoop kunnen uw verkopers samen met Microsoft verkopen vanuit uw CRM-systemen. Ze moeten niet worden getraind voor het gebruik van Partner Center om deals voor co-verkoop te beheren. Met behulp van de connectors voor co-verkoop kunt u een nieuwe verwijzing voor co-verkoop maken om een Microsoft-verkoper te betrekken, verwijzingen van de Microsoft-verkoper te ontvangen, verwijzingen te accepteren/weigeren, dealgegevens zoals dealwaarde en einddatum te wijzigen.  U kunt ook updates ontvangen van de Microsoft-verkopers over deze deals voor co-verkoop. U kunt al uw verwijzingen laten werken binnen het CRM van uw keuze in plaats van in Partner Center.

De oplossing is gebaseerd op Microsoft Power Automate Solution en maakt gebruik van Partner Center API's.

## <a name="before-you-install---pre-requisites"></a>Voordat u installeert - vereisten

|**Onderwerpen**|**Details**|**Koppelingen**|
|--------------|--------------------|------|
|Microsoft Partner Network-id |U hebt een geldige MPN-id nodig|Lid worden van [MPN](https://partner.microsoft.com/)|
|Gereed voor co-verkoop|Uw IP/Services-oplossing moet klaar zijn voor co-verkoop.|[Verkopen met Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Partnercentrum-account|De MPN-id die is gekoppeld aan Partner Center tenant moet gelijk zijn aan de MPN-id die is gekoppeld aan uw oplossing voor co-verkoop. Controleer of u uw verwijzingen voor co-verkoop kunt zien in Partner Center portal voordat u de connectors implementeert.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Partner Center gebruikersrollen|De werknemer die de connectors gaat installeren en gebruiken, moet een verwijzingsbeheerder zijn|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|De CRM-gebruikersrol is Systeembeheerder of Systeem aanwijzer|[Rollen toewijzen in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow account|Maak een nieuwe productieomgeving met een database voor testen, fasering en productie. Als u een bestaande productieomgeving met een database hebt, kan deze opnieuw worden gebruikt. De gebruiker die de connectoroplossing gaat installeren, moet een Power Automate hebben en toegang tot deze omgeving hebben. U kunt de voortgang controleren en meer informatie in de [Power Automate](https://flow.microsoft.com/) als de installatie mislukt. Selecteer **Geschiedenis bekijken onder** **Oplossingen**.|[Omgeving maken of beheren](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installatie van Salesforce-pakket voor aangepaste Microsoft-velden

Als u de verwijzingen wilt synchroniseren tussen Partner Center salesforce en Salesforce CRM, moet Power Automate oplossing duidelijk microsoft-specifieke verwijzingsvelden identificeren. Deze afbakening biedt verkopers van partners de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.

1. Activeer notities in Salesforce **en** voeg deze toe aan de lijst met verkoopkansen. [Verwijzing](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Activeer **opportunity-teams** door de volgende stappen uit te voeren:
    - Gebruik in Setup het vak **Snel zoeken om** opportunity team-Instellingen.
    - Definieer de instellingen naar behoefte. [Verwijzing](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Installeer in Salesforce aangepaste velden en objecten met behulp van het [installatieprogramma voor pakketten.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Gebruik dit installatieprogramma om het pakket in elk bedrijf te installeren.

    >[!NOTE]
    >Als u in een sandbox installeert, moet u het eerste gedeelte van de URL vervangen door `http://test.salesforce.com` .

1. Voeg in Salesforce Microsoft-oplossingen toe aan de lijst met betrekking **tot** kansen. Nadat u de sleutelsleutel hebt **toegevoegd, selecteert u het** pictogram en de eigenschappen bijwerken

## <a name="best-practice-test-before-you-go-live"></a>Best Practice: Testen voordat u live gaat

Voordat u de oplossing installeert, configureert en Power Automate in de productieomgeving, moet u de oplossing testen op een faserings-CRM-exemplaar.

- Installeer Microsoft Power Automate-oplossing in een faseringsomgeving/CRM-exemplaar.

- Maak een kopie van de oplossing en voer uw configuratie en Power Automate stroomaanpassingen uit in de faseringsomgeving.

- Test de oplossing op een faserings-/CRM-exemplaar.

- Importeer bij succes als een beheerde oplossing naar het productie-exemplaar.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Synchronisatie Partner Center verwijzingen voor Salesforce CRM installeren

1. Ga naar [Power Automate](https://flow.microsoft.com) en selecteer **Omgevingen** in de rechterbovenhoek. Hier ziet u de beschikbare CRM-exemplaren.

1. Selecteer het juiste CRM-exemplaar in de vervolgkeuzelijst in de rechterbovenhoek.

1. Selecteer **Oplossingen** in de linkernavigatiebalk.

1. Selecteer de **koppeling AppSource** openen in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Open AppSource.":::

1. Zoek in **Partner Center naar verwijzingenconnectoren voor Salesforce** in het pop-upscherm.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Schermopname van Nu krijgen.":::

1. Selecteer de **knop Nu krijgen** en selecteer vervolgens **Doorgaan.**

1. Selecteer op de volgende pagina de Salesforce CRM-omgeving om de toepassing te installeren. Ga akkoord met de voorwaarden.

1. U wordt vervolgens omgeleid naar de **pagina Uw oplossingen** beheren.  Navigeer naar Partner Center met behulp van de pijlknoppen onderaan de pagina. **De geplande installatie** wordt weergegeven naast Partner Center oplossing Verwijzingen. De installatie duurt 10-15 minuten.

1. Nadat de installatie is voltooid, gaat u terug naar [Power Automate](https://flow.microsoft.com) en selecteert **u Oplossingen** in het linkernavigatiegebied. U ziet **Partner Center verwijzingssynchronisatie** voor Salesforce nu beschikbaar is in de lijst oplossingen.

1. Selecteer **Partner Center Verwijzingssynchronisatie voor Salesforce**. De volgende Power Automate en entiteiten zijn beschikbaar:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce-stromen.":::

## <a name="configure-the-solution"></a>De oplossing configureren

1. Nadat u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Power Automate](https://flow.microsoft.com/).

1. Selecteer in **de** vervolgkeuzehoek Omgevingen in de rechterbovenhoek het CRM-exemplaar waarin u de oplossing Power Automate geïnstalleerd.

1. U moet verbindingen maken die de drie gebruikersaccounts koppelen:

   - Partner Center gebruiker met beheerdersreferenties voor verwijzingen
   - Partnercentrum-gebeurtenissen
   - CRM-beheerder met de Power Automate in de oplossing

   1. Selecteer **Verbindingen in** de linkernavigatiebalk en selecteer Partner Center oplossing **Verwijzingen** in de lijst.

   1. Maak een verbinding door Een **verbinding maken te selecteren.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Schermopname van Een verbinding maken.":::

   1. Zoek naar **Partner Center (preview)** in de zoekbalk in de rechterbovenhoek.

   1. Maak een verbinding voor uw Partner Center met de rol referenties van verwijzingsbeheerder.

   1. Maak vervolgens een verbinding Partner Center gebeurtenissen voor uw Partner Center met de referenties van verwijzingenbeheerder.

   1. Maak een verbinding voor Salesforce voor de CRM-beheerder.
  
   1. Maak een verbinding voor Microsoft Dataverse voor de CRM-beheerder.

   1. Nadat u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Schermopname die laat zien hoe u verbindingen kunt observeren.":::

### <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar **de pagina** Oplossingen en selecteer **Standaardoplossing.** Selecteer **Verbindingsverwijzing (preview) door** op Alle **te klikken.**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Schermopname van Het bewerken van de verbindingen.":::

1. Bewerk elk van de verbindingen afzonderlijk door het pictogram met het beletselteken te selecteren. Voeg de relevante verbindingen toe.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Schermopname die laat zien hoe u connectors kunt bewerken.":::

1. Schakel de stromen in de volgende volgorde in:
   - Partner Center webhookregistratie (Insider Preview)
   - [Aanpassen] Create or Get Details from Salesforce
   - Een co-sell-Referral-Salesforce voor Partner Center (Insider Preview)
   - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)  
   - Partner Center naar Salesforce (Insider Preview)
   - Salesforce naar Partner Center (Insider Preview)
   - Salesforce-mogelijkheden om Partner Center (Insider Preview)
   - Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-API's gebruiken om te registreren voor resourcewijzigingsgebeurtenissen

U kunt de webhook PARTNER CENTER-API's gebruiken om te registreren voor resourcewijzigingsgebeurtenissen. Deze wijzigingsgebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Selecteer **Partner Center Salesforce CRM (Insider Preview)**.

1. Selecteer het **pictogram Bewerken** en selecteer Wanneer **een HTTP-aanvraag wordt ontvangen.**

1. Selecteer het **pictogram Kopiëren** om de opgegeven **HTTP POST-URL te kopiëren.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Schermopname die laat zien hoe u de URL kopieert.":::

1. Selecteer de **Partner Center webhookregistratie (Insider Preview) Power Automate** selecteer vervolgens **Uitvoeren.**

1. Zorg ervoor dat **het venster Stroom** uitvoeren wordt geopend in het rechterdeelvenster en selecteer **Doorgaan.**

1. Voer de volgende details in:

   - **Http Trigger-eindpunt:** deze URL is uit een eerdere stap gekopieerd.
   - **Gebeurtenissen die moeten worden** geregistreerd: selecteer alle beschikbare gebeurtenissen **(** verwijzing gemaakt, **verwijzing** bijgewerkt, **related-referral-created** en **related-referral-updated).**
   - **Bestaande trigger-eindpunten overschrijven indien aanwezig?**: Ja. Er kan slechts één URL worden geregistreerd voor een bepaalde webhookgebeurtenis.

1. Selecteer **Stroom uitvoeren** en selecteer vervolgens **Done.**

De webhook kan nu luisteren naar gebeurtenissen, deze maken en bijwerken.

## <a name="customize-synchronization-steps"></a>Synchronisatiestappen aanpassen

CRM-systemen zijn zeer aangepast en u kunt de Power Automate aanpassen op basis van uw CRM-installatie. Wanneer verwijzingen voor co-verkoop worden gesynchroniseerd tussen Partner Center en uw CRM-systeem, worden de velden die zijn [](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)gesynchroniseerd op de Partner Center-pc vermeld in de handleiding aangepaste veldtoewijzing .

Volg de handleiding voor veldtoewijzing en pas indien nodig de juiste wijzigingen aan in **[Aanpassen]** Create or Get Details from Salesforce or environment variables (Details maken of gegevens op halen uit Salesforce of omgevingsvariabelen). Werk geen andere stromen in de Power Automate bij, omdat dit van invloed kan zijn op toekomstige oplossingsupgrades.

De volgende aanpassingen zijn beschikbaar:

- **Vinkje weergeven in** de naam van de kans: standaard wordt een vinkje weergegeven naast de naam van de kans om aan te geven dat de synchronisatie tussen Partner Center en Salesforce CRM is geslaagd. Op dezelfde manier wordt er een kruis markering weergegeven als de synchronisatie mislukt. Als u wilt voorkomen dat er een vinkje of kruisval in de naam van de kans wordt toegevoegd, stelt u de huidige waarde van het vinkje Weergeven in de omgevingsvariabele naam van de kans **in** op Nee.

- **Fasenaam:**

  - **Actieve fasenaam:** dit is de fase in de verkooppijplijn van een verkoopkans in Salesforce.  Het vertegenwoordigt een actieve fase en is gelijk aan een verwijzing met de status Geaccepteerd in Partner Center. Dit kan de volgende fase in de verkooppijplijn zijn na de fase on-hold. Als de verkoopfase van verkoopkans uit de on-hold fase wordt verplaatst naar de actieve fase, wordt de verwijzing in Partner Center en worden de wijzigingen gesynchroniseerd.

  - **Naam van de fase in de wacht:** naam van de fase in de verkooppijplijn van een verkoopkans in Salesforce. Het vertegenwoordigt een fase in de wacht. Nieuwe verwijzingen voor co-verkoop die worden gedeeld door Microsoft en die nog niet zijn geaccepteerd, worden ingesteld op deze fase in Salesforce. Wijzigingen die zijn aangebracht in een mogelijkheid terwijl deze in de wachtfase is, worden niet gesynchroniseerd met Partner Center. Als de verkoopfase van een verkoopkans uit deze on-hold fase wordt verplaatst, wordt de verwijzing in Partner Center en worden de wijzigingen gesynchroniseerd.

- **Landcode klantaccount:** het is verplicht om een tweeletterig landnummer (ISO 3166) op te geven wanneer u een nieuwe verwijzing maakt. Standaard wordt de landcode gesynchroniseerd naar en van het veld **BillingCountry** van het account in Salesforce. Als u een ander veld in Salesforce hebt om de landcode te synchroniseren vanuit:

  - Voor een niet-lookup landcodeveld in het account dat een tweeletterig code bevat:

    - Werk de **veldnaam voor het landnummer van** het klantaccount bij in de Salesforce-omgevingsvariabele met de veldnaam van het CRM. Zorg ervoor dat u de naam van het veld op geeft, niet de weergavenaam.

    - Bewerk **[Aanpassen] Maak** of haal details op uit Salesforce en ga  naar Klantaccount maken of krijgen **in CRM-actie** om een landwaarde toe te wijzen aan het juiste veld in het CRM. Verwijder ook de **waardetoewijzing Land** uit de **BillingCountry.**

  - Voor een opzoekveld voor landcode in het account:

    - Voeg een nieuw aangepast veld toe aan het account en vul het automatisch in met een tweeletterig landnummer (ISO 3166) op basis van de waarde die is geselecteerd in het opzoekveld en vice versa.

    - Volg de voorgaande stappen voor het veld nonlookup country code om een nieuw aangepast veld te synchroniseren van het CRM naar en van Partner Center.

- **Dealwaarde:** standaard wordt de dealwaarde van Partner Center gesynchroniseerd naar en van **Bedrag** in het CRM. Als u een ander veld in de CRM hebt voor de dealwaarde om te synchroniseren vanuit:

  - Werk de **veldnaam dealwaarde** in de Salesforce-omgevingsvariabele bij met de veldnaam van het CRM. Zorg ervoor dat u de naam van het veld op geeft, niet de weergavenaam.

  - Bewerk **[Aanpassen]** Maak of Haal details op uit Salesforce en  ga naar  Kans **maken** of bijwerken in CRM en werk zowel Een nieuwe kans maken als Bestaande kansen bijwerken bij om de **DealValue** toe te wijzen aan het juiste veld in Salesforce.

- **Valutacode dealwaarde:** naam van het valutacodeveld voor de dealwaarde in Salesforce. Deze veld-API-naam wordt gebruikt om de valutacode voor de dealwaarde van de kans op te halen bij het maken of bijwerken van een verwijzing in Microsoft Partner Center. Als het valutacodeveld voor de dealwaarde anders is dan het standaardveld **CurrencyIsoCode,** werkt u de huidige waarde van deze omgevingsvariabele bij.

  - Werk de **valutanaam van de dealwaarde** bij in de Salesforce-omgevingsvariabele met de veldnaam van het CRM. Zorg ervoor dat u de naam van het veld op geeft, niet de weergavenaam.

  - Bewerk **[Aanpassen]** Maak of haal details op uit Salesforce en ga naar Create or **update opportunity** in CRM (Een nieuwe kans maken of bijwerken) en werk zowel de acties Create a new **opportunity** (Een nieuwe kans maken) als Update **existing opportunity** actions (Bestaande kansen bijwerken) bij om **DealValueCurrency** toe te wijzen aan het juiste veld in Salesforce.

- **Verkoopkans voor co-verkoop** synchroniseren: als deze is ingesteld op **Ja,** worden alleen de mogelijkheden voor co-verkoop en het delen van pijplijnen gesynchroniseerd van Partner Center naar Salesforce. Als dit is **ingesteld op nee,** worden leads, co-sell en mogelijkheden voor het delen van pijplijnen gesynchroniseerd van Partner Center naar Salesforce. Deze variabele heeft geen invloed op de verkoopkansen die worden gesynchroniseerd van Salesforce naar Partner Center.

## <a name="update-environment-variable"></a>Omgevingsvariabele bijwerken

De waarde van een omgevingsvariabele bijwerken:

1. Ga naar de **pagina Oplossingen** en selecteer **Standaardoplossing.** Selecteer **Omgevingsvariabele** door **Alle te selecteren.**

1. Selecteer de omgevingsvariabele voor de waarde die moet worden bijgewerkt en selecteer **Bewerken** met behulp van het pictogram met het beletselteken.

1. Huidige **waarde bijwerken** (standaardwaarde niet **bijwerken)** met behulp van de **optie Nieuwe waarde** en de waarde op te geven. De waarde moet overeenkomen met het gegevenstype van de variabele. Het gegevenstype Ja of Nee accepteert bijvoorbeeld de waarde Ja of Nee.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Schermopname van Omgevingsvariabelen bijwerken.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-end bi-directional co-sell verwijzingssynchronisatie

Nadat u de Power Automate-oplossing hebt geïnstalleerd, geconfigureerd en aangepast, kunt u testen op synchronisatie van verwijzingen voor co-verkoop tussen Salesforce CRM en Partner Center.

### <a name="pre-requisites"></a>Vereisten

Als u de verwijzingen in Partner Center Salesforce CRM wilt synchroniseren, moet de Power Automate-oplossing microsoftspecifieke verwijzingsvelden duidelijk afbakenen. Deze identificatie biedt uw verkopersteams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.

Er is een set aangepaste velden beschikbaar als onderdeel van Partner Center de entiteit Verwijzingensynchronisatie voor Salesforce **CRM-oplossingskans.** Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden **voor** de mogelijkheid.

De volgende aangepaste velden moeten deel uitmaken van de CRM-sectie:

- **Synchroniseren met Partner Center:** of de kans moet worden gesynchroniseerd met Partner Center. De waarde van dit veld is standaard Nee en moet expliciet worden ingesteld op Ja door uw verkoper om een verkoopkans met Microsoft te delen. Voor nieuwe verwijzingen die worden gedeeld Partner Center CRM wordt deze veldwaarde ingesteld op Ja.

- **Verwijzings-id:** een veld met alleen-lezen-id's voor Microsoft Partner Center verwijzing.

- **Verwijzingskoppeling:** een alleen-lezen koppeling naar de verwijzing in Microsoft Partner Center.

- **Hoe kan Microsoft helpen:** Hulp vereist van Microsoft voor de verwijzing. Als u een verwijzing voor co-verkoop wilt maken, selecteert u de juiste hulp die Microsoft nodig heeft. Een klantcontact moet worden gekoppeld aan de mogelijkheid om een verwijzing voor co-verkoop te maken. Als u een verwijzing voor niet-co-verkoop wilt maken, selecteert u dit veld niet. Een verwijzing naar een niet-co-verkoop kan op elk gewenst moment worden geconverteerd naar een verwijzing voor co-verkoop door de juiste optie voor hulp te selecteren.

- **Zichtbaarheid Partner Center Microsoft-verwijzing:** selecteer zichtbaarheid voor de Partner Center verwijzing. Door het zichtbaar te maken voor Microsoft-verkopers, kan een verwijzing voor niet-co-verkoop worden geconverteerd naar co-verkoop. Wanneer Microsoft Help vereist is, is de verwijzing standaard zichtbaar voor Microsoft-verkopers. Nadat dit veld als zichtbaar is gemarkeerd, kan het niet meer worden teruggedraaid.

- **Microsoft CRM:** wanneer er een verwijzing voor co-verkoop wordt gemaakt en geaccepteerd door Microsoft, wordt dit veld gevuld met de CRM-id van Microsoft.

- **Microsoft Partner Center Solutions:** een aangepast object om oplossingen die klaar zijn voor co-verkoop of Microsoft-oplossingen te koppelen aan de verkoopkans. Een of meer oplossingen kunnen worden toegevoegd aan of verwijderd uit de mogelijkheid. Het is verplicht om ten minste één kant-en-klaar co-verkoopoplossing of Microsoft-oplossing aan de verkoopkans toe te voegen voordat u deze met Microsoft deelt. Als u dit object wilt koppelen aan de mogelijkheid, moet u **het formulier Opportunity** in het CRM bijwerken.

- **Controle:** een alleen-lezen audittrail voor synchronisatie met Partner Center verwijzingen

### <a name="scenarios"></a>SCENARIO 'S

1. Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en wordt gesynchroniseerd in Partner Center:

   1. Meld u aan bij uw Salesforce CRM-omgeving met een gebruiker die zichtbaarheid heeft in de **sectie Opportunity** van het CRM.

   1. Zorg ervoor dat de sectie **Microsoft Partner Center** aanwezig is wanneer u een nieuwe kans maakt in **de** Salesforce CRM-omgeving.

   1. Verkoopkansen die zijn gesynchroniseerd met Partner Center worden geïdentificeerd met ✔ pictogram in Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Schermopname van de Salesforce-omgeving.":::

   1. Als u deze mogelijkheid wilt synchroniseren met Microsoft Partner Center, moet u de volgende velden instellen in de kaartweergave:

      - **Hoe kan Microsoft helpen?**: als u een verwijzing voor co-verkoop wilt maken, selecteert u een geschikte Help-optie.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Schermopname die laat zien hoe u de juiste velden in de kaartweergave op kunt halen.":::

      - **Synchroniseren met Partner Center:** Ja
      - **Contactpersoon voor klant:** als u een verwijzing voor co-verkoop wilt maken, voegt u een klantcontact toe aan de verkoopkans.
      - **Microsoft Solutions:** als u een verwijzing met Microsoft wilt delen, voegt u een geldige oplossing voor co-verkoop of Microsoft-oplossingen toe aan de verkoopkans.

   1. Nadat u de optie Synchroniseren **met** Partner Center hebt ingesteld op **Ja,** tien minuten wachten, meld u zich aan bij uw Partner Center account. Uw verwijzingen worden gesynchroniseerd met Salesforce CRM en Verwijzingskoppeling wordt ingevuld. Als er een fout is opgetreden, wordt het veld Controle gevuld met foutgegevens.

   1. Wanneer de optie Synchroniseren met **Partner Center** is ingesteld op Ja, worden de wijzigingen gesynchroniseerd met uw Partner Center salesforce-account als u de kans in Salesforce CRM bij werkt.

2. Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in Microsoft Partner Center en gesynchroniseerd in de Salesforce CRM-omgeving:

    1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).

    1. Selecteer **Verwijzingen in** het menu aan de linkerkant.

    1. Maak een nieuwe verwijzing voor co-Partner Center door te klikken op de optie Nieuwe deal.

    1. Meld u aan bij uw Salesforce CRM-omgeving.

    1. Navigeer **naar Verkoopkansen openen.** De verwijzing die is gemaakt in Microsoft Partner Center is nu gesynchroniseerd in Salesforce CRM.

    1. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de details van de kaartweergave ingevuld.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Schermopname van de salesforce-kansenpagina.":::

>[!NOTE]
>**Hebt u hulp nodig bij de implementatie?**
>Voor hulp bij de implementatie van uw verwijzingsconnector voor co-verkoop kunt u contact op nemen met een technische partnerconsultant. Ze kunnen ondersteuning bieden bij de implementatie en best practices voor een geslaagde implementatie.
>
>Zie How to Submit a technical presales and deployment services request (Een aanvraag voor technische [presales-](technical-benefits.md) en implementatieservices indienen) voor meer informatie

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)

- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)

- [Partnercentrum-webhooks](/partner-center/develop/partner-center-webhooks)
