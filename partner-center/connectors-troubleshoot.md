---
title: Problemen met connectors voor verwijzingen voor co-verkoop oplossen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
description: Meer informatie over antwoorden op veelvoorkomende vragen over het gebruik van connectors voor co-verkoop. Lees deze veelgestelde vragen over het oplossen van problemen met connectors voor co-sell.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 5143d8e779332fd7df1ebeb3b5175658a0190f4b
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957040"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Problemen met connectors voor verwijzingen voor co-verkoop oplossen

**Van toepassing op**: Dynamics 365 CRM | Salesforce CRM

**Juiste rollen:** Beheerdersrollen voor verwijzingen | Systeembeheerder of systeembeheerder op de CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Vragen en antwoorden over vereisten

1. Kunt u een oplossing voor verwijzingsconnectoren voor proefversies voor co-verkoop gebruiken voor uw omgeving?

Als u in de test-/faseringsomgeving bent, kunt u kiezen voor een proefoplossing. De betaalde versie van de connectors is beschikbaar in AppSource op US$ 15/maand. Met de betaalde verbinding krijgt u 10.000 API-aanroepen per dag. De connectors zijn wrappers boven op Partner Center verwijzings-API's. Wanneer de connectoroplossingen worden  uitgevoerd  voor een gebeurtenis maken of bijwerken voor de verkoopkansen aan de Partner Center of crm-zijde, wordt er een API-aanroep uitgevoerd.

2. Welke rol hebt u nodig om secties te maken in een CRM-omgeving?

Gebruikers die systeembeheerders of systeem customizers zijn, kunnen wijzigingen voor iedereen toepassen. Alle app-gebruikers kunnen het systeem echter personaliseren en zelfs een deel van hun aanpassingen delen met anderen. 

3. Hebben partnerverkopers speciale rollen nodig om aan deze Partner Center?
 
Aan partnerverkopers moet de rol Verwijzingsbeheerder zijn toegewezen. Zie Overzicht van machtigingen [voor meer informatie.](create-user-accounts-and-set-permissions.md)

4. Welke velden moeten eerst worden ingesteld in uw CRM-omgeving? 

• Zorg ervoor dat uw valuta geschikt is voor uw locatie en zich nauwkeurig in uw CRM-omgeving bevindt. • Uw verkoopteam moet in uw CRM-omgeving worden vermeld als CRM-gebruikers.

5. Welke vereisten zijn vereist voor het maken Power Automate omgeving?

Als u de Power Automate wilt gebruiken, hebt u het volgende nodig:

- Een Power Automate is vereist.
- Er is minimaal 1 GB opslagruimte vereist.

6.  Hebt u een Dynamics 365-abonnement nodig om de oplossing Salesforce Connectors te kunnen gebruiken?

De Salesforce Connector-oplossing is van het type Dynamics Flow dat synchronisatie met andere CRM-systemen ondersteunt. Voor de oplossing hoeft u geen Dynamics 365-exemplaar of een abonnement te hebben. Tijdens het installeren van de Salesforce-oplossing kan er een vervolgkeuzekeuze met een bestaande CDS-omgeving in uw bedrijf worden weergegeven. U moet die omgeving selecteren. Als u de fout 'Kan geen Dynamics 365-organisatie vinden die is verbonden met een aangemelde gebruiker' krijgt, moet u bovendien een nieuwe omgeving voor de connector maken.

## <a name="questions-and-answers-about-configuration"></a>Vragen en antwoorden over configuratie

1. Wat moet u doen als u de volgende fout tegen komt tijdens het activeren van stromen in Power Automate Platform?

Fout: Aanvraag voor Azure Resource Manager mislukt met fout: {"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'. 

Volg deze stappen voor probleemoplossing:

- Verwijder de CDS-verbinding en maak de CDS-verbindingen opnieuw.
- De onderliggende stroom in- en uitschakelen 
- Verwijder de oplossing en installeer de oplossing opnieuw. 

2.  Wat moet u doen als u de fout 'Aanmelden' ziet tijdens het toevoegen van een Partner Center-connector in Power Automate Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Foutbericht waarin aanmelding is vereist.":::

Volg deze probleemoplossingsstap:

- Gebruik uw Partner Center om u eenmaal aan te melden bij de stroomomgeving (flow.microsoft.com).


3. Wat moet u doen als u de volgende fout krijgt tijdens het activeren van de Partner Center crm-stroom in Power Automate Platform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Foutbericht dat updates vereist.":::

Volg deze stappen voor probleemoplossing:

- Activeer eerst de volgende twee onderliggende stromen voordat u de Partner Center crm-stroom activeert.
      - Partner Center to CRM - Helper (Insider Preview)
      - Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)

4. Wat moet u doen wanneer u geen verbindingen met de stroom kunt toevoegen wanneer u de stroom probeert te bewerken?

U voegt verbindingen toe aan de stroom terwijl de stroom wordt uitgevoerd en u voegt aan elke stroom afzonderlijk toe.  Als het dialoogvenster voor het toevoegen van verbindingen niet automatisch wordt geopend tijdens het bewerken van de stroom, kunt u elk van de stappen en substappen van de stromen afzonderlijk bewerken.

- Selecteer elke stroom en bewerk ze afzonderlijk.
- Vouw alle stappen in de stroom uit 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Stappen die verbindingen nodig hebben.":::

- Selecteer de stappen waarin u een waarschuwingspictogram ziet waarin u wordt gevraagd om verbindingen te koppelen en verbindingen toe te voegen. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Bewerk de stroom stap voor stap.":::


5. Wat moet u doen als de stromen van de oplossing Voor verwijzingen voor co-verkoop niet worden aan zet?

A. In Power Automate moet u stromen in de volgende volgorde bewerken en bijwerken om de juiste verbindingen te gebruiken:

- Partner Center webhookregistratie (Insider Preview)
- Verwijzing voor co-verkoop maken - Salesforce naar Partner Center (Insider Preview)
- Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)
- Partner Center naar Salesforce (Insider Preview)
- Salesforce naar Partner Center (Insider Preview)
- Salesforce-mogelijkheden om Partner Center (Insider Preview)
- Salesforce Microsoft Solutions to Partner Center (Insider Preview)

 B. Selecteer voor elk stroom de **optie Alleen gebruikers** uitvoeren. Selecteer **Verbinding gebruiken in** plaats van Opgegeven door **alleen-uitvoeren gebruiker.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Een stroom activeren.":::


C. Activeer de onderstaande stromen:

 - Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)

- Salesforce naar Partner Center (Insider Preview)

    
D. Activeer alle resterende stromen.

E. Selecteer uitvoeren Partner Center Flow-webhookregistratie.  Geef de **HTTP-URL op** van de eerste actie in **Partner Center salesforce-stroom.** Selecteer alle vier de opties onder **Gebeurtenissen om te registreren** en selecteer **Ja** bij Overschrijven.

## <a name="questions-and-answers-about-runmaintenance"></a>Vragen en antwoorden over uitvoeren/onderhoud

1. Hoe kunt u fouten oplossen tijdens het uitvoeren Power Automate stroom?

Raadpleeg Stroomfouten herstellen om ervoor te zorgen dat Power Automate stromen worden uitgevoerd zoals u verwacht en fouten tijdens de uitvoering [kunt oplossen.](/power-automate/fix-flow-failures)

2. Wat moet u doen als u verwijzingen ziet die niet goed zijn gesynchroniseerd in Partner Center CRM-omgeving?
 
Selecteer Controleren om de status van verwijzingssynchronisatie **te bepalen.** 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Verwijzingen synchroniseren.":::

Zorg ervoor dat aan de volgende voorwaarden wordt voldaan:

- Oplossings-id wordt geleverd als onderdeel van de mogelijkheid.

- Landcode van twee letters is vereist.

- Wanneer Hulp van Microsoft wordt geselecteerd voor de mogelijkheid, zijn contactgegevens van klanten vereist.

3. Hoe kunt u ervoor zorgen dat een verwijzing in twee richtingen wordt gesynchroniseerd?

Voer de volgende stappen uit:

- Verkopers van partners moeten ervoor  zorgen dat ze de optie Synchroniseren met Partner Center hebben ingeschakeld in de crm-sectie.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Zorg ervoor dat Synch is ingeschakeld.":::

- Verkopers moeten een omzet- en einddatum verstrekken bij het kwalificeren van een lead.

- Als de CRM-id  wordt  opgegeven in de fase voor het maken of bijwerken van een verkoopkans, maar een leadkans met die id niet wordt gevonden in CRM, wordt bijwerken of maken genegeerd.

- Zorg ervoor dat het veld verwijzingsvaluta is geconfigureerd in de Salesforce-omgeving. 

4. Wat moet u doen als de verbinding met de connector wordt verbroken en u een verwijzingssynchronisatie mist?

Hier volgen enkele van de opties die u kunt uitproberen:

- Controleer of de gebruikersnaam of het wachtwoord is verlopen voor de Partner Center gebruiker met beheerdersrollen voor verwijzingen.

- U kunt naar de niet-gesynchroniseerde mogelijkheid gaan, een kleine update maken en kijken of de verwijzing is gesynchroniseerd.

- Als de stromen zijn uitgevoerd en zijn mislukt, selecteert u de stroom en dient u de mislukte run opnieuw in.

5. Wat moet u doen wanneer er fouten optreden met toegang geweigerd?

Zorg ervoor dat de juiste rollen bestaan

- De rol verwijzingsbeheerder voor Partner Center verkoper 
 
- De rol Systeembeheerder of Systeem aanpassen voor uw CRM-exemplaar

- Zorg ervoor dat de gebruiker Power Automate flow-account zich ten minste één keer van tevoren https://flow.microsoft.com aanmeldt

6. Als u ziet dat de landcode **van het klantaccount** ontbreekt tijdens het maken van een verkoopkans voor co-verkoop, wat moet u dan doen?

U moet de tweeletterig ISO-landcode toevoegen aan het klantaccount in CRM.

7. Wat moet u doen als u de fout ziet dat oplossings-id **is vereist bij** het maken van een verkoopkans voor co-verkoop?

Als u een verwijzing voor co-verkoop wilt maken, hebt u een oplossing nodig die gereed is voor co-verkoop door Microsoft. 

8. Wat moet u doen wanneer er kansen voor co-verkoop worden gemaakt in Partner Center die niet zijn gesynchroniseerd met CRM, ook al zijn er geen stroomfouten?

Ga als volgt te werk:

- Nadat u een nieuwe deal voor co-verkoop in Partner Center hebt gemaakt, controleert u of Partner Center naar de Dynamics 365-stroom wordt aangeroepen (deze kan meerdere keren worden aangeroepen).

- Als de stroom wordt aangeroepen, controleert u alle aangeroepen stromen en identificeert u de stroomuit voer die het CRM zou bijwerken. U kunt de acties volgen en controleren of het CRM is bijgewerkt of dat er een probleem is aangetroffen.

- Controleer **Nieuwe deal** in Partner Center om te zien of deze wordt gevuld met crm-id.

- Zorg ervoor dat de deal niet per ongeluk wordt gesloten als **Gewonnen** of Verloren **in** Partner Center.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)
 
- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)
