---
title: De connector voor co-sell voor Salesforce CRM Partner Center
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniseer uw verwijzingen in Partner Center met uw Salesforce CRM. Verkopers kunnen vervolgens samen met Microsoft verkopen vanuit uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276974"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Connector voor co-verkoop voor Salesforce CRM - overzicht

**Juiste rollen:** Beheerdersrollen voor verwijzingen | Systeembeheerder of systeem aanpassen op het CRM

Partner Center connector voor co-verkoop kunnen uw verkopers samen met Microsoft verkopen vanuit uw CRM-systemen. Ze moeten niet worden getraind voor het gebruik van Partner Center om deals voor co-verkoop te beheren. Met behulp van de connectors voor co-verkoop kunt u een nieuwe verwijzing voor co-verkoop maken om een Microsoft-verkoper te betrekken, verwijzingen van de Microsoft-verkoper te ontvangen, verwijzingen te accepteren/weigeren, dealgegevens zoals dealwaarde en einddatum te wijzigen.  U kunt ook updates ontvangen van de Microsoft-verkopers over deze deals voor co-verkoop. U kunt al uw verwijzingen laten werken binnen het CRM van uw keuze in plaats van in Partner Center. 

De oplossing is gebaseerd op Microsoft Power Automate Solution en maakt gebruik van Partner Center API's.

## <a name="before-you-install---pre-requisites"></a>Voordat u installeert - vereisten

|**Onderwerpen**   |**Details**   |**Koppelingen**   |
|--------------|--------------------|------|
|Microsoft Partner Network-id |U hebt een geldige MPN-id nodig|Lid worden van [MPN](https://partner.microsoft.com/)|
|Gereed voor co-verkoop|Uw IP/Services-oplossing moet klaar zijn voor co-verkoop.|[Verkopen met Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Partnercentrum-account|De MPN-id die is gekoppeld aan Partner Center tenant, moet gelijk zijn aan de MPN-id die is gekoppeld aan uw oplossing voor co-verkoop. Controleer of u uw verwijzingen voor co-verkoop kunt zien in Partner Center portal voordat u de connectors implementeert.|[Uw account beheren](create-user-accounts-and-set-permissions.md)|
|Partner Center gebruikersrollen|De werknemer die de connectors gaat installeren en gebruiken, moet een verwijzingsbeheerder zijn|[Beheerdersrollen en -machtigingen toewijzen](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|De CRM-gebruikersrol is Systeembeheerder of Systeem aanwijzer|[Rollen toewijzen in Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow-account|Een actief [Power Automate](https://flow.microsoft.com) account voor de crm-systeembeheerder of systeem aanpassen. Deze gebruiker moet zich ten [minste Power Automate](https://flow.microsoft.com) vóór de installatie aanmelden.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Installatie van Salesforce-pakket voor aangepaste Microsoft-velden 

Als u de verwijzingen wilt synchroniseren tussen Partner Center salesforce en Salesforce CRM, Power Automate oplossing duidelijk Microsoft-specifieke verwijzingsvelden identificeren. Deze afbakening biedt verkopers van partners de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.

1. Activeer notities in Salesforce **en** voeg deze toe aan de lijst met verkoopkansen. 
[Verwijzing](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Activeer **opportunity-teams** door de volgende stappen uit te voeren: 
    - Gebruik in Setup het vak **Snel zoeken om** de instellingen van het opportunity team te vinden.
    - Definieer de instellingen naar behoefte.
[Verwijzing](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Installeer in Salesforce aangepaste velden en objecten met behulp van het [installatieprogramma voor pakketten.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV) Gebruik dit om het pakket in elk bedrijf te installeren.

>[!NOTE]
>Als u in een sandbox installeert, moet u het eerste gedeelte van de URL vervangen door http://test.salesforce.com

4. Voeg in Salesforce Microsoft-oplossingen toe aan de lijst met betrekking **tot** kansen. Nadat u de sleutelsleutel hebt **toegevoegd, selecteert u het** pictogram en de eigenschappen bijwerken

## <a name="best-practice-test-before-you-go-live"></a>Best Practice: Testen voordat u live gaat

Voordat u de oplossing installeert, configureert en Power Automate in de productieomgeving, moet u de oplossing testen op een faserings-CRM-exemplaar.

- Installeer Microsoft Power Automate-oplossing in een faseringsomgeving/CRM-exemplaar.

- Maak een kopie van de oplossing en voer uw configuratie en Power Automate stroomaanpassingen uit in de faseringsomgeving.

- Test de oplossing op een faserings-/CRM-exemplaar.

- Importeer bij succes als een beheerde oplossing naar het productie-exemplaar.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Synchronisatie Partner Center verwijzingen voor Salesforce CRM installeren

1. Ga naar [Power Automate](https://flow.microsoft.com) en selecteer **Omgevingen** in de rechterbovenhoek. Hier ziet u de beschikbare CRM-exemplaren.

2. Selecteer het juiste CRM-exemplaar in de vervolgkeuzehoek in de rechterbovenhoek.

3. Selecteer **Oplossingen** in de linkernavigatiebalk.

4. Selecteer de **koppeling AppSource** openen in het bovenste menu.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource.":::

5. Zoek in **Partner Center naar verwijzingenconnectoren voor Salesforce** in het pop-upscherm.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. Selecteer de **knop Nu krijgen** en vervolgens **Doorgaan.**

7. Hiermee opent u de pagina waar u de Salesforce CRM-omgeving kunt selecteren om de toepassing te installeren.  Ga akkoord met de voorwaarden.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Beschikbare CRM's.":::

8. U wordt vervolgens omgeleid naar de **pagina Uw oplossingen** beheren.  Navigeer naar Partner Center met behulp van de pijlknoppen onderaan de pagina. **De geplande installatie** wordt weergegeven naast Partner Center oplossing Verwijzingen. De installatie duurt 10-15 minuten.

9. Zodra de installatie is voltooid, gaat u terug [naar Power Automate](https://flow.microsoft.com) en selecteert **u Oplossingen** in het navigatiegedeelte aan de linkerkant. U ziet **Partner Center verwijzingssynchronisatie** voor Salesforce beschikbaar is in de lijst oplossingen.

10. Selecteer **Partner Center Verwijzingssynchronisatie voor Salesforce**. De volgende Power Automate en entiteiten zijn beschikbaar:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-stromen.":::



## <a name="configure-the-solution"></a>De oplossing configureren

1. Nadat u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug [naar Power Automate](https://flow.microsoft.com/).

2. Selecteer in **de** vervolgkeuzehoek Omgevingen in de rechterbovenhoek het CRM-exemplaar waarin u de oplossing Power Automate geïnstalleerd.
3. U moet verbindingen maken die de drie gebruikersaccounts koppelen:
    - Partner Center gebruiker met beheerdersreferenties voor verwijzingen
    - Partnercentrum-gebeurtenissen
    - CRM-beheerder met de Power Automate stromen in de oplossing.
4. Selecteer **Verbindingen in** de linkernavigatiebalk en selecteer de oplossing Partner Center verwijzingen in de lijst.

5. Maak een verbinding door op Een verbinding **maken te klikken.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Verbinding maken.":::

- Zoek naar Partner Center (preview) in de zoekbalk in de rechterbovenhoek.

- Maak een verbinding voor uw Partner Center met de referentiesrol Van verwijzingsbeheerder.

-  Maak vervolgens een verbinding Partner Center gebeurtenissen voor uw Partner Center met de referenties van verwijzingenbeheerder.

- Maak een verbinding voor Salesforce voor de CRM-beheerder.

-  Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Bekijk de verbindingen.":::

### <a name="edit-the-connections"></a>De verbindingen bewerken

1. Ga terug naar de pagina Oplossingen en selecteer **Standaardoplossing.**  Selecteer **Verbindingsverwijzing (preview) door** op Alle **te klikken.**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Begin met het bewerken van de connector.":::

2. Bewerk elk van de verbindingen afzonderlijk door het pictogram met drie punten te selecteren. Voeg de relevante verbindingen toe.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Connectors bewerken.":::

3. Schakel de stromen in de volgende volgorde in:

- Partner Center webhookregistratie (Insider Preview)
- Verwijzing voor co-verkoop maken - Salesforce naar Partner Center (Insider Preview)
- Partner Center Microsoft Co-sell Verwijzingsupdates voor Salesforce (Insider Preview)
- Partner Center naar Salesforce (Insider Preview)
- Salesforce naar Partner Center (Insider Preview)
- Salesforce Opportunity to Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook-API's gebruiken om te registreren voor resourcewijzigingsgebeurtenissen

Met Partner Center webhook-API's kunt u zich registreren voor gebeurtenissen voor resourcewijziging. Deze wijzigingsgebeurtenissen worden als HTTP-berichten naar uw URL verzonden.

1. Als u uw URL wilt registreren, selecteert Partner Center de stroom **Webhook-registratie (Insider Preview)** Power Automate registreren.

2. Voeg verbindingen toe voor (a.) Partner Center gebruiker met beheerdersreferenties (b.) voor verwijzingen Partner Center Gebeurtenissen zoals hieronder is gemarkeerd

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger.":::

3. Wanneer u deze updates aan het maken bent, ziet u

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. Sla uw wijzigingen op en selecteer **In- of uit.**

   Voer de Partner Center uit om webhooks te laten luisteren naar gebeurteniswijzigingen:

5. Selecteer **Partner Center Salesforce CRM (Insider Preview)**.

6. Selecteer het **pictogram** Bewerken en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen.**

7. Selecteer het **pictogram Kopiëren** om de opgegeven HTTP POST-URL te kopiëren.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieer de URL.":::

8. Selecteer nu de stroom Partner Center webhookregistratie (Insider Preview) Power Automate selecteer **Uitvoeren.**

9. Zorg ervoor dat het venster Stroom uitvoeren wordt geopend in het rechterdeelvenster en selecteer **Doorgaan.**

10. Voer de volgende details in:

    1. **Http Trigger-eindpunt:** URL die u uit een eerdere stap hebt gekopieerd

    2. **Gebeurtenissen die moeten worden** geregistreerd: 'verwijzing gemaakt' en 'verwijzing bijgewerkt'

    3. **Overschrijf bestaande trigger-eindpunten indien aanwezig:** Ja (hiermee worden alle bestaande eindpunten overschreven.)

11. Selecteer **Uitvoeren** en selecteer vervolgens **Done.**

De webhook kan nu luisteren naar het maken en bijwerken van gebeurtenissen.

## <a name="customize-synchronization-steps"></a>Synchronisatiestappen aanpassen

Wanneer verwijzingen voor co-verkoop worden gesynchroniseerd tussen Partner Center en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op Partner Center pc hier vermeld.

CRM-systemen zijn vaak zeer aangepast. U kunt de Power Automate aanpassen. Volg de handleiding voor veldtoewijzing en indien nodig de juiste wijzigingen aan te brengen in de stappen van de Power Automate stromen.  Microsoft Partner Centers naar CRM-toewijzingen worden aangeboden, maar op basis van uw CRM-omgeving kunt u ervoor kiezen om de velden verder aan te passen.

Meerdere stappen van elk van de Power Automate stromen kunnen worden aangepast op basis van uw behoeften. Hier volgen enkele voorbeelden van beschikbare aanpassingen:

1. De velden voor het maken of bijwerken van gebeurtenissen in de Partner Center crm-verwijzingssynchronisatie aanpassen:

   1. Selecteer Partner Center Salesforce CRM (Insider Preview).

   2. Selecteer **Bewerken om** de stroom van de Power Automate bewerken/aanpassen.

   3. Selecteer **(Bereik) Synchroniseer de lead of kans**.

2. Als u CRM-veldtoewijzingen voor het maken van gebeurtenissen wilt aanpassen, selecteert u Als het de nieuwe **gedeelde kans is, selecteert u vervolgens**. Selecteer de substap zo **ja** en vouw vervolgens Een nieuwe kans maken **in crm uit.** U kunt de toewijzingen in deze sectie bewerken met behulp van de Handleiding voor veldtoewijzing.

   1. Als u CRM-veldtoewijzingen voor updategebeurtenissen wilt aanpassen, selecteert u de stap '(Bereik) De lead of kans synchroniseren'.

   2. Selecteer **Als het een update van een kans is, dan**. Selecteer de substap **zo ja** en vouw vervolgens If difference uit tussen de **opportunity-objecten in Partner Center CRM en vervolgens**.  

   3. Selecteer **Indien ja gevolgd** door Bestaande kans **bijwerken**

3. De velden voor VERWIJZINGssynchronisatie van CRM naar pc aanpassen voor updategebeurtenissen:

   1. Selecteer **Bewerken om**  de stroom van de Power Automate bewerken/aanpassen.

   2. Selecteer **(Bereik) Synchroniseer de kans**.

   3. Voor het aanpassen van CRM-veldtoewijzingen (op basis van de handleiding voor veldtoewijzingen) voor updategebeurtenissen selecteert u Als er verschil is tussen de **leadobjecten in Partner Center en CRM, selecteert u vervolgens**.

   4. Selecteer de substap zo **ja** en vouw vervolgens de stap **Een verwijzing bijwerken met opportunity data uit.**

   U kunt de toewijzingen in deze sectie bewerken op basis van de Handleiding voor veldtoewijzing.

4. Wilt u de velden voor verwijzingssynchronisatie van CRM naar pc's aanpassen voor het maken van gebeurtenissen?

   1. Selecteer **Bewerken om**  de stroom van de Power Automate bewerken/aanpassen.

   2. Selecteer **(Bereik) Verwijzingen synchroniseren.**

   3. Selecteer Microsoft-verwijzing maken voor het aanpassen van CRM-veldtoewijzingen (op basis van de handleiding voor veldtoewijzingen) voor **het maken van gebeurtenissen.**

U kunt de toewijzingen in deze sectie bewerken op basis van de Handleiding voor veldtoewijzing.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Verwijzingssynchronisatie van end-to-end bi-directionele co-verkoop

Nadat u de Power Automate-oplossing hebt geïnstalleerd, geconfigureerd en aangepast, kunt u testen op synchronisatie van verwijzingen voor co-verkoop tussen Salesforce CRM en Partner Center.

### <a name="pre-requisites"></a>Vereisten

Als u de verwijzingen tussen Partner Center salesforce en Salesforce CRM wilt synchroniseren, moet Power Automate oplossing microsoftspecifieke verwijzingsvelden duidelijk afbakenen. Deze identificatie biedt uw verkopersteams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.

Er is een set aangepaste velden beschikbaar als onderdeel van Partner Center de entiteit Verwijzingensynchronisatie voor Salesforce **CRM-oplossingskans.** Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden **voor** kansen.

De volgende aangepaste velden moeten deel uitmaken van de CRM-sectie:

- **Synchroniseren met Partner Center:** of de kans moet worden gesynchroniseerd met Microsoft Partner Center

- **Verwijzings-id:** een veld met alleen-lezen-id's voor Microsoft Partner Center verwijzing

- **Verwijzingskoppeling:** een alleen-lezenkoppeling naar de verwijzing in Microsoft Partner Center

- **Hoe kan Microsoft helpen:** Hulp vereist van Microsoft voor de verwijzing

- **Producten:** lijst met producten die zijn gekoppeld aan deze kans

- **Controleren:** een alleen-lezen audittrail voor synchronisatie met Partner Center verwijzingen

### <a name="scenarios"></a>Scenario 's:

1. Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en wordt gesynchroniseerd in Partner Center:

   1. Meld u aan bij uw Salesforce CRM-omgeving met de gebruiker die inzicht heeft in de **sectie Opportunity** van het CRM.

   2. Zorg ervoor dat de volgende sectie aanwezig is wanneer u een nieuwe kans maakt in de Salesforce CRM-omgeving

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-omgeving.":::

   3. Als u deze mogelijkheid wilt synchroniseren met Microsoft Partner Center, moet u de volgende velden instellen in de kaartweergave:

       - "Synchroniseren met Partner Center": Ja
       - "Hoe kan Microsoft u helpen?": Selecteer een van de volgende opties:
       - Producten: Oplossings-ID's van het product

   4. Nadat u de optie Synchroniseren  **met** een Partner Center ingesteld op **Ja,** 10 minuten wachten, aanmelden bij uw Partner Center account. Uw verwijzingen worden gesynchroniseerd met Salesforce CRM.

   5. Wanneer de optie Synchroniseren met Partner Center is ingesteld op Ja. Als u de kans in Salesforce CRM bij werkt, worden de wijzigingen gesynchroniseerd met uw Partner Center account.

   6. Verkoopkansen die zijn gesynchroniseerd met Partner Center worden geïdentificeerd met ✔icon in Salesforce CRM.

2. Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in Microsoft Partner Center en gesynchroniseerd in de Salesforce CRM-omgeving:

    1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard/home)

    2. Selecteer **Verwijzingen in** het menu aan de linkerkant.

    3. Maak een nieuwe verwijzing voor co-verkoop vanuit Partner Center door te klikken op de optie Nieuwe deal.

    4. Meld u aan bij uw Salesforce CRM-omgeving.

    5. Navigeer **naar Open Opportunities**. De verwijzing die is gemaakt in Microsoft Partner Center is nu gesynchroniseerd in Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-kansscherm.":::

    6. Wanneer u een gesynchroniseerde verwijzing selecteert, worden de details van de kaartweergave ingevuld.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)

- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)

- [Partnercentrum-webhooks](/partner-center/develop/partner-center-webhooks)
