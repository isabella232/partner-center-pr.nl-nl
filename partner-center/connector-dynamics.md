---
title: De connector voor het samen verkopen van Dynamics 365 CRM-partner centrum
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniseer uw referenties in Partner Center met uw connector voor co-sell voor Dynamics 365 CRM. Verkopers kunnen vervolgens samen met micro soft verkopen binnen uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947736"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Connector voor Dynamics 365-overzicht co-sell

### <a name="appropriate-roles"></a>Juiste rollen

- Beheerder van verwijzingen
- Systeem beheerder of systeemaanpasser op de CRM

Met connector voor co-sell van partner Center kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen. Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop. Gebruik de co-Connect connectors om een nieuwe verwijzing naar de verkoop te maken voor een micro soft-verkoper, referenties te ontvangen van de micro soft-verkoper, verwijzingen te accepteren/weigeren, afhandelings gegevens te wijzigen, zoals een deal waarde en een sluitings datum. U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals. U kunt al uw verwijzingen gebruiken binnen de CRM van uw keuze in plaats van in het partner centrum. 

De oplossing is gebaseerd op de micro soft-oplossing voor energie automatisering en maakt gebruik van partner Center-Api's.

## <a name="before-you-install---pre-requisites"></a>Voordat u de vereisten installeert

|**Onderwerpen**   |**Details**   |**Koppelingen**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |U hebt een geldige MPN-ID nodig|Toevoegen aan [MPN](https://partner.microsoft.com/)|
|Klaar voor de verkoop|Uw IP/Services-oplossing moet samen worden verkocht.|[Verkopen met micro soft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercentrum-account|De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling. Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in partner centrum Portal kunt zien.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Gebruikers rollen voor het partner centrum|De werk nemer die de connectors installeert en gebruikt, moet een referentie beheerder zijn|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser|[Rollen toewijzen in Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Stroom account voor energie automatisering|Een actief [geautomatiseerd](https://flow.microsoft.com) account voor het beheer van de CRM-systeem beheerder of het systeem. Deze gebruiker moet zich ten minste één keer aanmelden bij Power voor het [automatiseren](https://flow.microsoft.com) van de installatie.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Synchronisatie van partner Center referrals voor Dynamics 365 (oplossing voor automatische stroom) installeren

1. Ga naar [Automatische stroom](https://flow.microsoft.com) en selecteer **omgevingen** in de rechter bovenhoek. In deze stap ziet u de beschik bare CRM-exemplaren.

2. Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.

3. Selecteer **oplossingen** op de linkernavigatiebalk.

4. Klik op de koppeling **Open AppSource** in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource openen":::

5. Zoek naar **Partner Center referrals connectors voor Dynamics365** in het pop-upvenster.  

6. Klik op de knop **nu downloaden** en vervolgens op **door gaan**.

7. Hiermee opent u de pagina waar u de CRM-omgeving (Dynamics 365) kunt selecteren om de toepassing te installeren.  Ga akkoord met de voor waarden.

8. Vervolgens gaat u naar de pagina **uw oplossingen beheren** .  Navigeer naar partner Center referrals met behulp van de pijl knoppen aan de onderkant van de pagina. **Geplande installatie** moet naast Partner Center referrals-oplossing worden weer gegeven. De installatie duurt 10-15 minuten. 

9. Zodra de installatie is voltooid, gaat u terug naar [energie automatisering](https://flow.microsoft.com) en selecteert u **oplossingen** vanuit het navigatie gebied links. U ziet dat **Partner Center referrals synchronisatie voor Dynamics 365** beschikbaar is in de lijst met oplossingen.

10. Selecteer de **synchronisatie van partner Center referrals voor Dynamics 365**. De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Beschik bare CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>Best practice: test voordat u live gaat

Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test.

- Installeer de oplossing voor het automatiseren van micro soft power op een staging-omgeving/CRM-exemplaar.
- Maak een kopie van de oplossing en voer uw configuratie uit en Automatiseer de stroom aanpassingen in de faserings omgeving.
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

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Verbinding maken":::

      3. Zoek naar **Partner Center referrals (preview)** in de zoek balk in de rechter bovenhoek.

      4. Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.

      5. Maak vervolgens een verbinding met de partner centrum-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de beheerder.

      6. Maak een verbinding voor Common Data Service (huidige omgeving) voor de gebruiker van de CRM-beheerder.
       
     
      7. Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Verbindingen":::
   
## <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar de pagina **oplossingen** en selecteer **standaard oplossing**. Selecteer **verbindings verwijzing (preview)** door te klikken op **alle**.

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Verbinding maken":::

2. Bewerk elk van de verbindingen één voor één door het pictogram drie punten te selecteren. Voeg de relevante verbindingen toe.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Verbindingen vermeld"::: 

3.  Schakel de stromen in de volgende volg orde in:
- Inschrijving van partner Center-webhooks (Insider preview)
- Een verwijzing naar een co-sell maken – Dynamics 365 naar partner Center (Insider preview)
- Partner centrum referentie-updates voor micro soft-verkoop naar Dynamics 365 (Insider preview)
- Partner centrum voor Dynamics 365 (Insider preview)
- Dynamics 365 naar partner Center (Insider preview)
- Dynamics 365-opportunity naar partner Center (Insider preview)
- Dynamics 365 micro soft Solutions to Partner Center (Insider preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-Api's gebruiken om te registreren voor bron wijzigings gebeurtenissen

Met de webhook-Api's van partner Center kunt u zich registreren voor bron wijzigings gebeurtenissen. Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Als u uw URL wilt registreren, selecteert u stroom voor het automatiseren van de data **Center-webhook-registratie (Insider preview)** .

2. Verbindingen toevoegen voor een partner centrum-gebruiker (a.) met referrals beheerders referenties (b.) partner Center-gebeurtenissen zoals hieronder gemarkeerd

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Wanneer u deze updates maakt, ziet u

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Sla de wijzigingen op en selecteer **inschakelen**.

   Voer de volgende stappen uit om het partner centrum-webhooks in te scha kelen voor het Luis teren naar gebeurtenis wijzigingen:

5. Selecteer **partner centrum voor Dynamics 365 (Insider preview)**.

6. Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen**.

7. Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL kopiëren":::

8. Selecteer nu de stroom voor het automatiseren van partner Center-webhooks (Insider preview) en selecteer **uitvoeren**.

9. Zorg ervoor dat het venster stroom uitvoeren wordt geopend in het rechterdeel venster en klik op **door gaan**.

10. Voer de volgende details in:

    1. **Http-trigger eindpunt**: URL gekopieerd uit eerdere stap

    2. **Te registreren gebeurtenissen**: ' verwijzing-gemaakt ' en ' referentie-bijgewerkt '

    3. **Bestaande trigger eindpunten overschrijven indien aanwezig**: Ja (Hiermee worden alle bestaande eind punten overschreven.)

11. Selecteer **uitvoeren** en selecteer vervolgens **gereed.**

De webhook kan nu Luis teren om gebeurtenissen te maken en bij te werken.

## <a name="customize-synchronization-steps"></a>Synchronisatie stappen aanpassen

Als er verwijzingen naar links worden gesynchroniseerd tussen partner centrum en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-PC hier vermeld.

Vaak worden de CRM-systemen zeer aangepast. U kunt de stroom voor het automatiseren van stromen aanpassen. Volg de instructies in de hand leiding voor de veld toewijzing en breng zo nodig de juiste wijzigingen aan in de stappen van de stroom automatische stromen.  Micro soft partner Centers naar CRM-toewijzingen worden gegeven, maar op basis van uw CRM-omgeving kunt u ervoor kiezen om de velden verder aan te passen.

Meerdere stappen van elk van de energiebeheer stromen kunnen worden aangepast op basis van uw behoeften. Hier volgen enkele voor beelden van beschik bare aanpassingen:

1. Als u de velden voor de gebeurtenissen maken of bijwerken in het partner centrum wilt aanpassen aan CRM Referral-synchronisatie: 

    a. Selecteer partner centrum voor Dynamics 365 (Insider preview) of partner centrum naar Sales Force (Insider preview).

    b. Selecteer **bewerken** om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

    c. Selecteer **(bereik) de lead of de opportuniteit synchroniseren**.

2. Als u CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen wilt aanpassen, selecteert u **of het een nieuwe gedeelde verkoop kans is en klikt u vervolgens** op. Selecteer de substap **als** dit het geval is en vouw vervolgens **een nieuwe opportuniteit maken in het CRM** uit. U kunt de toewijzingen in deze sectie bewerken met de gids voor veld toewijzing.

    d. Voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor update gebeurtenissen, klikt u op de stap (bereik) synchroniseren van de lead of de verkoop kans.

    e. Selecteer **deze optie als het een update is voor een verkoop kans en klik vervolgens**. Selecteer de substap **Indien ja** en vouw vervolgens uit **als het verschil tussen de objecten verkoop kansen in partner centrum en CRM**.  

    f. Selecteren **als ja** , gevolgd door **bestaande verkoop kans bijwerken**

3. De velden voor CRM naar PC Referral Synchronization voor update gebeurtenissen aanpassen:

    a. Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

    b. Selecteer **(bereik) de opportuniteit synchroniseren**.

    c. Als u de CRM-veld toewijzingen voor update gebeurtenissen wilt aanpassen, selecteert u **of er verschillen zijn tussen de objecten leads in partner centrum en CRM**. 

    d. Selecteer de substap **als ja** en vouw vervolgens de stap **een referral met verkoopkansgegevens bijwerken** uit.

   U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.

4. De velden voor CRM naar PC Referral-synchronisatie aanpassen voor het maken van gebeurtenissen?

   a. Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

   b. Selecteer **(bereik) het synchroniseren van verwijzingen.**

   c. Selecteer **micro soft Referral maken** voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen.

   U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.

Er zijn twee omgevings variabelen gemaakt:

- Vinkje: geeft aan of u een vinkje zou moeten hebben naast de verkoop kansen die in twee richtingen tussen partner centrum en Dynamics 365 CRM worden gesynchroniseerd.

- Alleen verkoop kansen synchroniseren: geeft aan of u alleen verkoop kansen wilt synchroniseren.

U kunt ervoor kiezen de standaard waarde voor de omgevings variabelen te bewerken.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Invoervak voor standaard waarden":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-end-synchronisatie van Referral-verkoop referenties

Zodra u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Dynamics 365 en partner centrum.

### <a name="pre-requisites"></a>Vereisten

Voor het synchroniseren van de verwijzingen tussen partner centrum en Dynamics 365 CRM, is de oplossing voor het automatiseren van de stroom een duidelijke verwijzings velden van micro soft. Met deze identificatie kunnen uw verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.

Een set aangepaste velden is beschikbaar als onderdeel van de entiteit **verkoop kans** . Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .

De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:

- **Synchroniseren met partner centrum**: of u de mogelijkheid wilt synchroniseren met micro soft Partner Center

- **Verwijzings-id**: een veld met alleen-lezen-id voor micro soft Partner Center Referral

- **Verwijzings koppeling**: een alleen-lezen koppeling naar de verwijzing in het micro soft partner centrum

- **Hoe kan ik Help** van micro soft helpen?: micro soft vereist voor de verwijzing

- **Producten**: lijst met producten die zijn gekoppeld aan deze verkoop kans

- **Controle**: een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen

Werk het verkoopkansformulier in Dynamics 365 CRM bij met oplossingen voor het veld Products.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulier Verkoop kans":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>DENKBAAR

1. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en gesynchroniseerd in partner centrum:

   1. Meld u aan bij uw Dynamics 365 CRM-omgeving met een zicht baarheid in het gedeelte **verkoop kansen** van de CRM.

   2. Zorg ervoor dat de volgende sectie aanwezig is wanneer u een ' nieuwe mogelijkheid ' in de Dynamics 365-omgeving maakt

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sectie voor beeld van verkoop kansen met informatie over micro soft Partner Center in Dynamics 365.":::

   3. Als u deze mogelijkheid wilt synchroniseren met micro soft Partner Center, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:

      - **Synchroniseren met partner centrum**: Ja

      - **Hoe kan micro soft u helpen?**: Selecteer een van de volgende opties:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sectie voor beeld van verkoop kansen in Dynamics 365 waarin de Help-opties van micro soft Partner Center worden weer gegeven naast een veld met de naam hoe kan micro soft u helpen?":::

      - **Producten**: oplossings-id's van het product

   4. Zodra de opportuniteit is gemaakt in Dynamics 365 met **synchronisatie met** de optie voor Partner Center is ingesteld op **Ja**, wacht u 10 minuten en meldt u zich aan bij uw partner centrum-account. Uw verwijzingen worden gesynchroniseerd met Dynamics 365.

   5. Voor een verkoop kans waarvoor de optie ' synchroniseren met partner centrum ' is ingesteld op ' ja ' en u de verkoop kans bijwerkt in Dynamics 365 CRM, worden de wijzigingen ook gesynchroniseerd in uw partner centrum-account.

   6. Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Dynamics 365.

2. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in micro soft Partner Center en gesynchroniseerd in de Dynamics 365-omgeving:

   1. Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).

   2. Selecteer **verwijzingen** in het menu aan de linkerkant.

   3. Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door te klikken op de optie nieuwe deal.

   4. Meld u aan bij uw Dynamics 365 CRM-omgeving.

   5. Navigeer naar **Open verkoop kansen**. De verwijzing die is gemaakt in het micro soft Partner Center is nu gesynchroniseerd in Dynamics 365 CRM.

   6. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)

- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)

- [Meer informatie over het platform van micro soft voor energie automatisering?](/power-automate/)

- [Partner centrum-webhooks](/partner-center/develop/partner-center-webhooks)