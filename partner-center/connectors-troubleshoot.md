---
title: Problemen oplossen met referrals connectors
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over antwoorden op veelgestelde vragen over het gebruik van connectors voor co-verkoop. Lees deze veelgestelde vragen over het oplossen van problemen met het verkopen van co-Connect oren.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92528683"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Problemen oplossen met referrals connectors

**Van toepassing op:**

- Partnercentrum
- Dynamics 365 CRM
- Sales Force CRM

**Juiste rollen**

- Beheerder van verwijzingen
- Systeem beheerder of systeemaanpasser op de CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Vragen en antwoorden over vereisten

1. Kunt u gebruikmaken van de connectors oplossing voor het gebruik van een proef abonnement voor uw omgeving?

Als u zich in de test-of faserings omgeving bevindt, kunt u kiezen voor een proef oplossing. De betaalde versie van de connectors is beschikbaar in AppSource voor ons $15/maand. Met de betaalde verbinding krijgt u dagelijks 10K API-aanroepen per dag. De connectors zijn wrappers boven op Partner Center-Referral-Api's. Wanneer de connector oplossingen worden uitgevoerd voor een gebeurtenis **maken** of **bijwerken** voor de mogelijkheden van het partner centrum of de CRM-kant, wordt een API-aanroep uitgevoerd.

2. Welke rol hebt u nodig voor het maken van secties in een CRM-omgeving?

Gebruikers die systeem beheerders of systeemaanpassers zijn, kunnen wijzigingen voor iedereen Toep assen. Alle app-gebruikers kunnen het systeem echter personaliseren en hun aanpassingen zelfs delen met anderen. 

3. Hebben partner verkopers speciale rollen nodig voor het werken met partner Center?
 
Partner verkopers moeten de rol ' verwijzingen beheerder ' toewijzen. Raadpleeg het volgende [machtigingen overzicht) (create-user-accounts-and-set-permissions) voor meer informatie.

4. Welke velden moeten eerst in uw CRM-omgeving worden ingesteld? 

• Zorg ervoor dat uw valuta geschikt is voor uw locatie en correct in uw CRM-omgeving is. • Uw verkoop team moet worden vermeld in uw CRM-omgeving als CRM-gebruikers.

5. Welke vereisten zijn er vereist voor het automatisch maken van een omgeving?

U hebt het volgende nodig om de omgeving voor het automatiseren van de Power te gebruiken:

- Er is een energiebeheer licentie vereist.
- Er is mini maal 1 GB opslag vereist.

6.  Hebt u een Dynamics 365-abonnement nodig om Sales Force connectors-oplossing te gebruiken?

De oplossing voor de Sales Force-connector is van het type ' Dynamics flow ' dat synchronisatie met andere CRM-systemen ondersteunt. Voor de oplossing is geen Dynamics 365-exemplaar of een abonnement vereist. Tijdens de installatie van de Sales Force-oplossing kan er een vervolg keuzelijst met de bestaande CDS-omgeving in uw bedrijf worden weer gegeven. U moet die omgeving selecteren. Als u bovendien de fout ' kan geen Dynamics 365-organisatie vinden die is verbonden met een aangemelde gebruiker ' krijgt, moet u een nieuwe omgeving maken voor de connector.

## <a name="questions-and-answers-about-configuration"></a>Vragen en antwoorden over configuratie

1. Wat moet u doen als u de volgende fout melding krijgt bij het activeren van stromen in het energiebeheer platform?

Fout: de aanvraag voor het Azure Resource Manager is mislukt met de volgende fout: {"Error": {"code": "WorkflowTriggerNotFound", "Message": "de trigger ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 ' van de werk stroom kan niet worden gevonden.}}. 

Volg deze stappen voor probleem oplossing:

- Verwijder de CDS-verbinding en maak de CDS-verbindingen opnieuw.
- Onderliggende stroom in-en uitschakelen 
- Verwijder de oplossing en installeer vervolgens de oplossing opnieuw. 

2.  Wat moet u doen als u de fout melding meldt bij het toevoegen van een partner Center-connector in het geautomatiseerde platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::

Volg deze stappen voor probleem oplossing:

- Gebruik de referenties van uw partner centrum om u eenmaal aan te melden bij de stroom omgeving (flow.microsoft.com).


3. Wat moet u doen als de volgende fout wordt weer gegeven tijdens het activeren van het partner centrum naar CRM-stroom in het geautomatiseerde platform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::

Volg deze stappen voor probleem oplossing:

- Activeer eerst de volgende twee onderliggende stromen voordat u het partner centrum naar CRM-stroom activeert.
      - Partner centrum voor CRM-helper (Insider preview)
      - Partner centrum micro soft-referentie-updates verkopen aan CRM (Insider preview)

4. Wat moet u doen als u geen verbindingen kunt toevoegen aan de stroom wanneer u de stroom probeert te bewerken?

U voegt verbindingen toe aan de stroom terwijl de stroom wordt uitgevoerd. u kunt elke stroom afzonderlijk toevoegen.  Als het dialoog venster voor het toevoegen van verbindingen niet automatisch wordt geopend tijdens het bewerken van de stroom, kunt u elk van de stappen en substappen van de stromen afzonderlijk bewerken.

- Selecteer elke stroom en bewerk ze afzonderlijk.
- Alle stappen in de stroom uitvouwen 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::

- Selecteer de stappen waarin een waarschuwings pictogram wordt weer gegeven om verbindingen te koppelen en verbindingen toe te voegen. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::


5. Wat moet u doen als de stromen van de connectors oplossing voor het samen verkopen van verwijzingen niet worden ingeschakeld?

A. In energie automatisering moet u stromen bewerken in de volgende volg orde en deze bijwerken om de juiste verbindingen te gebruiken:

- Inschrijving van partner Center-webhooks (Insider preview)
- Een verwijzing naar een gezamenlijk verkoop object maken-Sales Force to Partner Center (Insider preview)
- Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)
- Partner centrum naar Sales Force (Insider preview)
- Sales Force to Partner Center (Insider preview)
- Sales Force to Partner Center (Insider preview)
- Sales Force Micro Solutions to Partner Center (Insider preview)

 B. Selecteer voor elke stroom de optie **alleen gebruikers uitvoeren** . Selecteer **verbinding gebruiken** in plaats van **via alleen-uitvoeren gebruiker** .  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::


C. Activeer deze hieronder vermelde stromen:

 - Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)

- Sales Force to Partner Center (Insider preview)

    
D. Alle resterende stromen activeren.

E. Selecteer bij stroom Partner Center-webhook registratie **uitvoeren** . Geef de **http-URL** op van de eerste actie in **Partner Center naar Sales Force** -stroom. Selecteer alle vier de opties onder **gebeurtenissen die u wilt registreren** en selecteer **Ja** voor overschrijven.

## <a name="questions-and-answers-about-runmaintenance"></a>Vragen en antwoorden over uitvoeren/onderhoud

1. Hoe kunt u problemen oplossen wanneer er fouten optreden tijdens het automatiseren van de stroom?

Raadpleeg [stroom fouten oplossen](/power-automate/fix-flow-failures)om ervoor te zorgen dat uw stroom stromen automatisch worden uitgevoerd zoals verwacht en problemen tijdens de uitvoering kunnen oplossen.

2. Wat moet u doen als er verwijzingen worden weer geven die niet juist zijn gesynchroniseerd in een partner centrum of een CRM-omgeving?
 
Selecteer **audit** om de status van de verwijzings synchronisatie te bepalen. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::

Zorg ervoor dat aan de volgende voor waarden wordt voldaan:

- De oplossings-id is opgenomen als onderdeel van de verkoop kans.

- Land code van twee letters is vereist.

- Wanneer u hulp van micro soft hebt geselecteerd voor de opportuniteit, is contact gegevens van de klant vereist.

3. Hoe kunt u ervoor zorgen dat een verwijzing twee richtingen synchroniseert?

Voer de volgende stappen uit:

- Partner verkopers moeten ervoor zorgen dat de optie **synchronisatie met partner Center** is ingeschakeld in de sectie CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Fout bericht waarvoor aanmelding is vereist" in het partner centrum.

## <a name="next-steps"></a>Volgende stappen

- [Leads beheren](manage-leads.md)
 
- [Collectieve-verkoopkansen beheren](manage-co-sell-opportunities.md)