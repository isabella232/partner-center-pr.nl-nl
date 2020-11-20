---
title: De co-sell connector voor Sales Force CRM Partner Center
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniseer uw referenties in Partner Center met uw Sales Force-CRM. Verkopers kunnen vervolgens samen met micro soft verkopen binnen uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947848"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connector voor Sales Force-verkoop-overzicht

### <a name="appropriate-roles"></a>Juiste rollen

- Beheerder van verwijzingen
- Systeem beheerder of systeemaanpasser op de CRM

Met connector voor co-sell van partner Center kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen. Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop. Met de co-Connect oren kunt u een nieuwe verwijzing naar een mede verkoop maken om contact op te nemen met een micro soft-verkoper, verwijzingen te ontvangen van de micro soft-verkoper, verwijzingen te accepteren/weigeren, afhandelings gegevens te wijzigen, zoals de deal waarde en de sluitings datum.  U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals. U kunt al uw referenties gebruiken terwijl u werkt in de CRM van uw keuze in plaats van in het partner centrum. 

De oplossing is gebaseerd op de micro soft-oplossing voor energie automatisering en maakt gebruik van partner Center-Api's.

## <a name="before-you-install---pre-requisites"></a>Voordat u de vereisten installeert

|**Onderwerpen**   |**Details**   |**Koppelingen**   |
|--------------|--------------------|------|
|Microsoft Partner Network-ID |U hebt een geldige MPN-ID nodig|Toevoegen aan [MPN](https://partner.microsoft.com/)|
|Klaar voor samen verkopen|Uw IP/Services-oplossing moet samen worden verkocht.|[Verkopen met micro soft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercentrum-account|De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling. Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in partner centrum Portal kunt zien.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Gebruikers rollen voor het partner centrum|De werk nemer die de connectors installeert en gebruikt, moet een referentie beheerder zijn|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)|
|Sales Force CRM|De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser|[Rollen toewijzen in Sales Force CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Stroom account voor energie automatisering|Een actief [geautomatiseerd](https://flow.microsoft.com) account voor het beheer van de CRM-systeem beheerder of het systeem. Deze gebruiker moet zich ten minste één keer aanmelden bij Power voor het [automatiseren](https://flow.microsoft.com) van de installatie.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installatie van Sales Force-pakket voor aangepaste micro soft-velden 

Voor het synchroniseren van de verwijzingen tussen partner centrum en Sales Force CRM, moet de oplossing voor het automatiseren van micro soft specifieke Referral-velden duidelijk identificeren. Deze afbakening biedt partner verkopers teams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.

1. Activeer in Sales Force de **notities** en voeg deze toe aan de lijst met aan verkoop kansen gerelateerde. 
[Verwijzing](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Activeer **verkoop kansen teams** door de volgende stappen uit te voeren: 
    - In Setup gebruikt u het vak **Snelzoeken** om de instellingen van het Opportunity team te vinden.
    - Definieer de instellingen waar nodig.
[Verwijzing](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Onder Sales Force installeert u aangepaste velden en objecten met behulp van Package Installer hieronder.
  
Ga [hier](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) om het pakket te installeren in een bedrijf:


Opmerking: als u in een sandbox installeert, moet u het eerste deel van de URL vervangen door http://test.salesforce.com

4. Voeg in Sales Force micro soft-oplossingen toe aan de lijst met **kansen** die hieraan zijn gerelateerd. Nadat deze is toegevoegd, klikt u op het **moersleutel** pictogram en werkt u de eigenschappen bij

## <a name="best-practice-test-before-you-go-live"></a>Best practice: test voordat u live gaat

Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test.

- Installeer de oplossing voor het automatiseren van micro soft power op een staging-omgeving/CRM-exemplaar.

- Maak een kopie van de oplossing en voer uw configuratie uit en Automatiseer de stroom aanpassingen in de faserings omgeving.

- Test de oplossing op een staging/CRM-exemplaar.

- Importeer bij geslaagd als een beheerde oplossing naar het productie-exemplaar.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Synchronisatie van partner Center referrals voor Sales Force CRM installeren

1. Ga naar [Automatische stroom](https://flow.microsoft.com) en selecteer **omgevingen** in de rechter bovenhoek. Hiermee worden de beschik bare exemplaren van CRM weer gegeven.

2. Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.

3. Selecteer **oplossingen** op de linkernavigatiebalk.

4. Klik op de koppeling **Open AppSource** in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource openen":::

5. Zoek naar **Partner Center referrals connectors voor Sales Force** in het pop-upvenster.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Klik op de knop **nu downloaden** en vervolgens op **door gaan**.

7. Hiermee opent u de pagina waar u de Sales Force CRM-omgeving kunt selecteren om de toepassing te installeren.  Ga akkoord met de voor waarden.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Beschik bare CRMS":::

8. Vervolgens gaat u naar de pagina **uw oplossingen beheren** .  Navigeer naar partner Center referrals met behulp van de pijl knoppen aan de onderkant van de pagina. **Geplande installatie** moet naast Partner Center referrals-oplossing worden weer gegeven. De installatie duurt 10-15 minuten.

9. Zodra de installatie is voltooid, gaat u terug naar [energie automatisering](https://flow.microsoft.com) en selecteert u **oplossingen** vanuit het navigatie gebied links. U ziet dat **Partner Center referrals synchronisatie voor Sales Force** beschikbaar is in de lijst met oplossingen.

10. Selecteer **Partner Center referrals synchronisatie voor Sales Force**. De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Sales Force-stromen":::



## <a name="configure-the-solution"></a>De oplossing configureren

1. Wanneer u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Automatische stroom](https://flow.microsoft.com/).

2. Selecteer in de vervolg keuzelijst **omgevingen** in de rechter BOVENHOEK het CRM-exemplaar waarop u de oplossing voor het automatiseren van energie beheer hebt geïnstalleerd.
3. U moet verbindingen maken waarmee de drie gebruikers accounts worden gekoppeld:
    - Partner centrum-gebruiker met referrals beheerders referenties
    - Partnercentrum-gebeurtenissen
    - CRM-beheerder met de stroom voor het automatiseren van stromen in de oplossing.
4. Selecteer **verbindingen** in de linkernavigatiebalk en selecteer de oplossing Partner Center referrals in de lijst.

5. Maak een verbinding door te klikken op **een verbinding maken**.

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Verbinding maken":::

- Zoek naar partner Center referrals (preview) in de zoek balk in de rechter bovenhoek.

- Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.

-  Maak vervolgens een verbinding met de partner centrum-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de beheerder.

- Maak een verbinding voor Sales Force voor de CRM-beheerders gebruiker.

-  Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Verbindingen observeren":::

### <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar de pagina oplossingen en selecteer **standaard oplossing**.  Selecteer **verbindings verwijzing (preview)** door te klikken op **alle**.
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Connector bewerking starten":::

2. Bewerk elk van de verbindingen één voor één door het pictogram drie punten te selecteren. Voeg de relevante verbindingen toe.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Connectors bewerken":::

3. Schakel de stromen in de volgende volg orde in:

- Inschrijving van partner Center-webhooks (Insider preview)
- Een verwijzing naar een gezamenlijk verkoop object maken-Sales Force to Partner Center (Insider preview)
- Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)
- Partner centrum naar Sales Force (Insider preview)
- Sales Force to Partner Center (Insider preview)
- Sales Force to Partner Center (Insider preview)
- Sales Force Micro Solutions to Partner Center (Insider preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-Api's gebruiken om te registreren voor bron wijzigings gebeurtenissen

Met de webhook-Api's van partner Center kunt u zich registreren voor bron wijzigings gebeurtenissen. Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Als u uw URL wilt registreren, selecteert u stroom voor het automatiseren van de data **Center-webhook-registratie (Insider preview)** .

2. Verbindingen toevoegen voor een partner centrum-gebruiker (a.) met referrals beheerders referenties (b.) partner Center-gebeurtenissen zoals hieronder gemarkeerd

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. Wanneer u deze updates maakt, ziet u

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Sla de wijzigingen op en selecteer **inschakelen**.

   Voer de volgende stappen uit om het partner centrum-webhooks in staat te stellen om te Luis teren naar gebeurtenis wijzigingen:

5. Selecteer **partner centrum naar Sales Force CRM (Insider preview)**.

6. Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen**.

7. Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL kopiëren":::

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

   1. Selecteer partner centrum naar Sales Force CRM (Insider preview).

   2. Selecteer **bewerken** om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

   3. Selecteer **(bereik) de lead of de opportuniteit synchroniseren**.

2. Als u CRM-veld toewijzingen voor het maken van gebeurtenissen wilt aanpassen, selecteert u **of het een nieuwe gedeelde verkoop kans is en klikt u vervolgens** op. Selecteer de substap **Indien ja** en vouw vervolgens **een nieuwe opportuniteit maken in het CRM** uit. U kunt de toewijzingen in deze sectie bewerken met de gids voor veld toewijzing.

   1. Als u CRM-veld toewijzingen voor update gebeurtenissen wilt aanpassen, klikt u op de stap (bereik) synchroniseren van de lead of de verkoop kans.

   2. Selecteer **deze optie als het een update is voor een verkoop kans en klik vervolgens**. Selecteer de substap **Indien ja** en vouw vervolgens uit **als het verschil tussen de objecten verkoop kansen in partner centrum en CRM**.  

   3. Selecteren **als ja** , gevolgd door **bestaande verkoop kans bijwerken**

3. De velden voor CRM naar PC Referral Synchronization voor update gebeurtenissen aanpassen:

   1. Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

   2. Selecteer **(bereik) de opportuniteit synchroniseren**.

   3. Voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding veld Toewijzingen) voor update gebeurtenissen, selecteert u **of er verschil is tussen de objecten leads in Partner Center en CRM**.

   4. Selecteer de substap **als ja** en vouw vervolgens de stap **een referral met verkoopkansgegevens bijwerken** uit.

   U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.

4. De velden voor CRM naar PC Referral-synchronisatie aanpassen voor het maken van gebeurtenissen?

   1. Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.

   2. Selecteer **(bereik) het synchroniseren van verwijzingen.**

   3. Selecteer **micro soft Referral maken** voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen.

U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>End-to-end-synchronisatie van Referral-verkoop referenties

Zodra u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Sales Force CRM en partner Center.

### <a name="pre-requisites"></a>Vereisten

Voor de synchronisatie van de verwijzingen tussen partner centrum en Sales Force CRM moet de oplossing voor het automatiseren van micro soft-specifieke Referral-velden duidelijk worden afgebakend. Met deze identificatie kunnen verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.

Een set aangepaste velden is beschikbaar als onderdeel van partner Center referrals synchronisatie voor de Sales Force CRM **Solution-** entiteit. Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .

De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:

- **Synchroniseren met partner centrum**: of u de mogelijkheid wilt synchroniseren met micro soft Partner Center

- **Verwijzings-id**: een veld met alleen-lezen-id voor micro soft Partner Center Referral

- **Verwijzings koppeling**: een alleen-lezen koppeling naar de verwijzing in het micro soft partner centrum

- **Hoe kan ik micro soft helpen**: Help vereist van micro soft voor de verwijzing

- **Producten**: lijst met producten die zijn gekoppeld aan deze verkoop kans

- **Controle**: een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen

### <a name="scenarios"></a>DENKBAAR

1. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en gesynchroniseerd in partner centrum:

   1. Meld u aan bij uw Sales Force CRM-omgeving met een zicht baarheid in het gedeelte **verkoop kansen** van de CRM.

   2. Zorg ervoor dat de volgende sectie aanwezig is wanneer u een nieuwe kans maakt in de Sales Force CRM-omgeving

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Sales Force-omgeving":::

   3. Als u deze mogelijkheid wilt synchroniseren met micro soft Partner Center, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:

       - "Synchroniseren met partner centrum": Ja
       - "How can micro soft Help?": Selecteer een van de volgende opties:
       - Producten: oplossings-Id's van het product

   4. Wanneer u de optie  **synchronisatie van verkoop kansen met partner Center** hebt ingesteld op **Ja**, wacht u 10 minuten en meldt u zich aan bij uw partner centrum-account. Uw verwijzingen worden gesynchroniseerd met Sales Force CRM.

   5. Wanneer de optie ' synchroniseren met partner centrum ' is ingesteld op ' ja ' en u de opportuniteit bijwerkt in Sales Force CRM, worden de wijzigingen gesynchroniseerd met uw partner centrum-account.

   6. Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Sales Force CRM.

2. Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in micro soft Partner Center en gesynchroniseerd in de Sales Force CRM-omgeving:

    1. Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).

    2. Selecteer **verwijzingen** in het menu aan de linkerkant.

    3. Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door te klikken op de optie nieuwe deal.

    4. Meld u aan bij uw Sales Force CRM-omgeving.

    5. Navigeer naar **Open verkoop kansen**. De verwijzing die is gemaakt in het micro soft Partner Center is nu gesynchroniseerd in Sales Force CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Scherm Sales Force-verkoop kans":::

    6. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)

- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)

- [Partner centrum-webhooks](/partner-center/develop/partner-center-webhooks)
