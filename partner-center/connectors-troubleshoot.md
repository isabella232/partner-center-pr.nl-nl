---
title: Problemen met connectors voor verwijzingen voor co-verkoop oplossen
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over antwoorden op veelvoorkomende vragen over het gebruik van connectors voor co-verkoop. Lees deze veelgestelde vragen over het oplossen van problemen met connectors voor co-sell.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276924"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="1df82-104">Problemen met connectors voor verwijzingen voor co-verkoop oplossen</span><span class="sxs-lookup"><span data-stu-id="1df82-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="1df82-105">**Van toepassing op**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1df82-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="1df82-106">**Juiste rollen:** beheerdersrollen voor verwijzingen | Systeembeheerder of systeembeheerder op de CRM</span><span class="sxs-lookup"><span data-stu-id="1df82-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="1df82-107">Vragen en antwoorden over vereisten</span><span class="sxs-lookup"><span data-stu-id="1df82-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="1df82-108">Kunt u een oplossing voor verwijzingsconnectoren voor proefversies voor co-verkoop gebruiken voor uw omgeving?</span><span class="sxs-lookup"><span data-stu-id="1df82-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="1df82-109">Als u in de test-/faseringsomgeving bent, kunt u kiezen voor een proefoplossing.</span><span class="sxs-lookup"><span data-stu-id="1df82-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="1df82-110">De betaalde versie van de connectors is beschikbaar in AppSource op US$ 15/maand.</span><span class="sxs-lookup"><span data-stu-id="1df82-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="1df82-111">Met de betaalde verbinding krijgt u 10.000 API-aanroepen per dag.</span><span class="sxs-lookup"><span data-stu-id="1df82-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="1df82-112">De connectors zijn wrappers boven op Partner Center verwijzings-API's.</span><span class="sxs-lookup"><span data-stu-id="1df82-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="1df82-113">Wanneer de connectoroplossingen worden  uitgevoerd voor een create- of **updategebeurtenis** voor de verkoopkansen aan Partner Center of crm-zijde, wordt er een API-aanroep uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="1df82-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="1df82-114">Welke rol hebt u nodig om secties te maken in een CRM-omgeving?</span><span class="sxs-lookup"><span data-stu-id="1df82-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="1df82-115">Gebruikers die systeembeheerders of systeem customizers zijn, kunnen wijzigingen voor iedereen toepassen.</span><span class="sxs-lookup"><span data-stu-id="1df82-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="1df82-116">Alle app-gebruikers kunnen het systeem echter personaliseren en zelfs een deel van hun aanpassingen delen met anderen.</span><span class="sxs-lookup"><span data-stu-id="1df82-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="1df82-117">Hebben partnerverkopers speciale rollen nodig om aan een Partner Center?</span><span class="sxs-lookup"><span data-stu-id="1df82-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="1df82-118">Aan partnerverkopers moet de rol Verwijzingsbeheerder zijn toegewezen.</span><span class="sxs-lookup"><span data-stu-id="1df82-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="1df82-119">Zie Overzicht van machtigingen [voor meer informatie.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="1df82-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="1df82-120">Welke velden moeten eerst worden ingesteld in uw CRM-omgeving?</span><span class="sxs-lookup"><span data-stu-id="1df82-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="1df82-121">• Zorg ervoor dat uw valuta geschikt is voor uw locatie en zich nauwkeurig in uw CRM-omgeving bevindt.</span><span class="sxs-lookup"><span data-stu-id="1df82-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="1df82-122">• Uw verkoopteam moet in uw CRM-omgeving worden vermeld als CRM-gebruikers.</span><span class="sxs-lookup"><span data-stu-id="1df82-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="1df82-123">Welke vereisten zijn vereist voor het maken Power Automate omgeving?</span><span class="sxs-lookup"><span data-stu-id="1df82-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="1df82-124">Als u de Power Automate wilt gebruiken, hebt u het volgende nodig:</span><span class="sxs-lookup"><span data-stu-id="1df82-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="1df82-125">Een Power Automate is vereist.</span><span class="sxs-lookup"><span data-stu-id="1df82-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="1df82-126">Er is minimaal 1 GB opslagruimte vereist.</span><span class="sxs-lookup"><span data-stu-id="1df82-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="1df82-127">Hebt u een Dynamics 365-abonnement nodig om de oplossing Salesforce Connectors te kunnen gebruiken?</span><span class="sxs-lookup"><span data-stu-id="1df82-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="1df82-128">De Salesforce Connector-oplossing is van het type Dynamics Flow dat synchronisatie met andere CRM-systemen ondersteunt.</span><span class="sxs-lookup"><span data-stu-id="1df82-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="1df82-129">Voor de oplossing hoeft u geen Dynamics 365-exemplaar of een abonnement te hebben.</span><span class="sxs-lookup"><span data-stu-id="1df82-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="1df82-130">Tijdens het installeren van de Salesforce-oplossing kan er een vervolgkeuzekeuze met een bestaande CDS-omgeving in uw bedrijf worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="1df82-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="1df82-131">U moet die omgeving selecteren.</span><span class="sxs-lookup"><span data-stu-id="1df82-131">You need to select that environment.</span></span> <span data-ttu-id="1df82-132">Als u de fout 'Kan geen Dynamics 365-organisatie vinden die is verbonden met een aangemelde gebruiker' krijgt, moet u bovendien een nieuwe omgeving voor de connector maken.</span><span class="sxs-lookup"><span data-stu-id="1df82-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="1df82-133">Vragen en antwoorden over configuratie</span><span class="sxs-lookup"><span data-stu-id="1df82-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="1df82-134">Wat moet u doen als u de volgende fout tegen komt tijdens het activeren van stromen in Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="1df82-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="1df82-135">Fout: Aanvraag voor Azure Resource Manager mislukt met fout: {"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could be found."}}'.</span><span class="sxs-lookup"><span data-stu-id="1df82-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="1df82-136">Volg deze stappen voor probleemoplossing:</span><span class="sxs-lookup"><span data-stu-id="1df82-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1df82-137">Verwijder de CDS-verbinding en maak de CDS-verbindingen opnieuw.</span><span class="sxs-lookup"><span data-stu-id="1df82-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="1df82-138">De onderliggende stroom in- en uitschakelen</span><span class="sxs-lookup"><span data-stu-id="1df82-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="1df82-139">Verwijder de oplossing en installeer de oplossing opnieuw.</span><span class="sxs-lookup"><span data-stu-id="1df82-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="1df82-140">Wat moet u doen als u de fout 'Aanmelden' ziet tijdens het toevoegen van een Partner Center-connector in Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="1df82-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Foutbericht waarin aanmelding is vereist.":::

<span data-ttu-id="1df82-142">Volg deze probleemoplossingsstap:</span><span class="sxs-lookup"><span data-stu-id="1df82-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="1df82-143">Gebruik uw Partner Center om u eenmaal aan te melden bij de stroomomgeving (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="1df82-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="1df82-144">Wat moet u doen als u de volgende foutmelding krijgt tijdens het activeren van de Partner Center crm-stroom in Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="1df82-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Foutbericht dat updates vereist.":::

<span data-ttu-id="1df82-146">Volg deze stappen voor probleemoplossing:</span><span class="sxs-lookup"><span data-stu-id="1df82-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="1df82-147">Activeer eerst de volgende twee onderliggende stromen voordat u de Partner Center crm-stroom activeert.</span><span class="sxs-lookup"><span data-stu-id="1df82-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="1df82-148">Partner Center to CRM - Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="1df82-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="1df82-150">Wat moet u doen wanneer u geen verbindingen met de stroom kunt toevoegen wanneer u de stroom probeert te bewerken?</span><span class="sxs-lookup"><span data-stu-id="1df82-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="1df82-151">U voegt verbindingen toe aan de stroom terwijl de stroom wordt uitgevoerd en u voegt aan elke stroom afzonderlijk toe.</span><span class="sxs-lookup"><span data-stu-id="1df82-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="1df82-152">Als het dialoogvenster voor het toevoegen van verbindingen niet automatisch wordt geopend tijdens het bewerken van de stroom, kunt u elk van de stappen en substappen van de stromen afzonderlijk bewerken.</span><span class="sxs-lookup"><span data-stu-id="1df82-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="1df82-153">Selecteer elke stroom en bewerk ze afzonderlijk.</span><span class="sxs-lookup"><span data-stu-id="1df82-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="1df82-154">Vouw alle stappen in de stroom uit</span><span class="sxs-lookup"><span data-stu-id="1df82-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Stappen die verbindingen nodig hebben.":::

- <span data-ttu-id="1df82-156">Selecteer de stappen waarin u een waarschuwingspictogram ziet waarin u wordt gevraagd om verbindingen te koppelen en verbindingen toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="1df82-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Bewerk de stroom stap voor stap.":::


5. <span data-ttu-id="1df82-158">Wat moet u doen als de stromen van de oplossing Voor verwijzingen voor co-verkoop niet worden aan zet?</span><span class="sxs-lookup"><span data-stu-id="1df82-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="1df82-159">A.</span><span class="sxs-lookup"><span data-stu-id="1df82-159">A.</span></span> <span data-ttu-id="1df82-160">In Power Automate moet u stromen in de volgende volgorde bewerken en bijwerken om de juiste verbindingen te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="1df82-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="1df82-161">Partner Center webhookregistratie (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="1df82-162">Verwijzing voor co-verkoop maken - Salesforce naar Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1df82-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1df82-164">Partner Center naar Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="1df82-165">Salesforce naar Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1df82-166">Salesforce-mogelijkheden om Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="1df82-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="1df82-168">B.</span><span class="sxs-lookup"><span data-stu-id="1df82-168">B.</span></span> <span data-ttu-id="1df82-169">Selecteer voor elk stroom de **optie Alleen gebruikers** uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="1df82-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="1df82-170">Selecteer **Verbinding gebruiken in** plaats van Opgegeven door **alleen-uitvoeren gebruiker.**</span><span class="sxs-lookup"><span data-stu-id="1df82-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Een stroom activeren.":::


<span data-ttu-id="1df82-172">C.</span><span class="sxs-lookup"><span data-stu-id="1df82-172">C.</span></span> <span data-ttu-id="1df82-173">Activeer de onderstaande stromen:</span><span class="sxs-lookup"><span data-stu-id="1df82-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="1df82-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="1df82-175">Salesforce naar Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="1df82-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="1df82-176">D.</span><span class="sxs-lookup"><span data-stu-id="1df82-176">D.</span></span> <span data-ttu-id="1df82-177">Activeer alle resterende stromen.</span><span class="sxs-lookup"><span data-stu-id="1df82-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="1df82-178">E.</span><span class="sxs-lookup"><span data-stu-id="1df82-178">E.</span></span> <span data-ttu-id="1df82-179">Selecteer uitvoeren Partner Center Flow-webhookregistratie. </span><span class="sxs-lookup"><span data-stu-id="1df82-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="1df82-180">Geef de **HTTP-URL van** de eerste actie in Partner Center **naar de Salesforce-stroom.**</span><span class="sxs-lookup"><span data-stu-id="1df82-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="1df82-181">Selecteer alle vier de opties onder **Gebeurtenissen om te registreren** en selecteer **Ja** bij Overschrijven.</span><span class="sxs-lookup"><span data-stu-id="1df82-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="1df82-182">Vragen en antwoorden over uitvoeren/onderhoud</span><span class="sxs-lookup"><span data-stu-id="1df82-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="1df82-183">Hoe kunt u fouten oplossen tijdens het uitvoeren Power Automate stroom?</span><span class="sxs-lookup"><span data-stu-id="1df82-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="1df82-184">Raadpleeg Stroomfouten herstellen om ervoor te zorgen dat Power Automate stromen worden uitgevoerd zoals u verwacht en fouten tijdens de uitvoering [kunt oplossen.](/power-automate/fix-flow-failures)</span><span class="sxs-lookup"><span data-stu-id="1df82-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="1df82-185">Wat moet u doen als u verwijzingen ziet die niet goed zijn gesynchroniseerd in Partner Center crm-omgeving?</span><span class="sxs-lookup"><span data-stu-id="1df82-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="1df82-186">Selecteer Controleren om de status van verwijzingssynchronisatie **te bepalen.**</span><span class="sxs-lookup"><span data-stu-id="1df82-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Verwijzingen synchroniseren.":::

<span data-ttu-id="1df82-188">Zorg ervoor dat aan de volgende voorwaarden wordt voldaan:</span><span class="sxs-lookup"><span data-stu-id="1df82-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="1df82-189">Oplossings-id wordt geleverd als onderdeel van de mogelijkheid.</span><span class="sxs-lookup"><span data-stu-id="1df82-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="1df82-190">Landcode van twee letters is vereist.</span><span class="sxs-lookup"><span data-stu-id="1df82-190">Two letter country code is required.</span></span>

- <span data-ttu-id="1df82-191">Wanneer Hulp van Microsoft wordt geselecteerd voor de mogelijkheid, zijn contactgegevens van klanten vereist.</span><span class="sxs-lookup"><span data-stu-id="1df82-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="1df82-192">Hoe kunt u ervoor zorgen dat een verwijzing in twee richtingen wordt gesynchroniseerd?</span><span class="sxs-lookup"><span data-stu-id="1df82-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="1df82-193">Voer de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="1df82-193">Do the following steps:</span></span>

- <span data-ttu-id="1df82-194">Verkopers van partners moeten ervoor zorgen dat ze de optie Synchroniseren met **Partner Center** hebben ingeschakeld in de crm-sectie.</span><span class="sxs-lookup"><span data-stu-id="1df82-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Zorg ervoor dat Synch is ingeschakeld.":::

- <span data-ttu-id="1df82-196">Verkopers moeten een omzet- en einddatum verstrekken bij het kwalificeren van een lead.</span><span class="sxs-lookup"><span data-stu-id="1df82-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="1df82-197">Als de CRM-id  wordt  opgegeven in de fase voor het maken of bijwerken van een verkoopkans, maar een leadkans met die id niet wordt gevonden in CRM, wordt het bijwerken of maken genegeerd.</span><span class="sxs-lookup"><span data-stu-id="1df82-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="1df82-198">Zorg ervoor dat het veld verwijzingsvaluta is geconfigureerd in de Salesforce-omgeving.</span><span class="sxs-lookup"><span data-stu-id="1df82-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="1df82-199">Wat moet u doen als de verbinding met de connector wordt verbroken en u een verwijzingssynchronisatie mist?</span><span class="sxs-lookup"><span data-stu-id="1df82-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="1df82-200">Hier volgen enkele van de opties die u kunt uitproberen:</span><span class="sxs-lookup"><span data-stu-id="1df82-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="1df82-201">Controleer of de gebruikersnaam of het wachtwoord is verlopen voor de Partner Center gebruiker met beheerdersrollen voor verwijzingen.</span><span class="sxs-lookup"><span data-stu-id="1df82-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="1df82-202">U kunt naar de niet-gesynchroniseerde mogelijkheid gaan, een kleine update maken en kijken of de verwijzing is gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="1df82-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="1df82-203">Als de stromen zijn uitgevoerd en zijn mislukt, selecteert u de stroom en dient u de mislukte run opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="1df82-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="1df82-204">Wat moet u doen wanneer er fouten optreden met toegang geweigerd?</span><span class="sxs-lookup"><span data-stu-id="1df82-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="1df82-205">Zorg ervoor dat de juiste rollen bestaan</span><span class="sxs-lookup"><span data-stu-id="1df82-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="1df82-206">De rol van verwijzingsbeheerder voor Partner Center verkoper</span><span class="sxs-lookup"><span data-stu-id="1df82-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="1df82-207">De rol Systeembeheerder of Systeem aanpassen voor uw CRM-exemplaar</span><span class="sxs-lookup"><span data-stu-id="1df82-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="1df82-208">Zorg ervoor dat de Power Automate flow-account van tevoren https://flow.microsoft.com ten minste één keer aanmeldt</span><span class="sxs-lookup"><span data-stu-id="1df82-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="1df82-209">Als u ziet dat de landcode **van het klantaccount** ontbreekt tijdens het maken van een verkoopkans voor een co-verkoop, wat moet u dan doen?</span><span class="sxs-lookup"><span data-stu-id="1df82-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="1df82-210">U moet de tweeletterig ISO-landcode toevoegen aan het klantaccount in CRM.</span><span class="sxs-lookup"><span data-stu-id="1df82-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="1df82-211">Wat moet u doen als u de fout ziet dat oplossings-id **is vereist bij** het maken van een verkoopkans voor co-verkoop?</span><span class="sxs-lookup"><span data-stu-id="1df82-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="1df82-212">Als u een verwijzing voor co-verkoop wilt maken, hebt u een oplossing nodig die gereed is voor co-verkoop door Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1df82-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="1df82-213">Wat moet u doen wanneer u kansen voor co-verkoop ziet die zijn gemaakt in Partner Center die niet zijn gesynchroniseerd met CRM, ook al zijn er geen stroomfouten?</span><span class="sxs-lookup"><span data-stu-id="1df82-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="1df82-214">Ga als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="1df82-214">Do the following:</span></span>

- <span data-ttu-id="1df82-215">Nadat u een nieuwe deal voor co-verkoop in Partner Center hebt gemaakt, controleert u of Partner Center naar de Dynamics 365-stroom wordt aangeroepen (deze kan meerdere keren worden aangeroepen).</span><span class="sxs-lookup"><span data-stu-id="1df82-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="1df82-216">Als de stroom wordt aangeroepen, controleert u alle aangeroepen stromen en identificeert u de stroomuit voer die het CRM zou bijwerken.</span><span class="sxs-lookup"><span data-stu-id="1df82-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="1df82-217">U kunt de acties volgen en controleren of het CRM is bijgewerkt of dat er een probleem is aangetroffen.</span><span class="sxs-lookup"><span data-stu-id="1df82-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="1df82-218">Controleer **Nieuwe deal** in Partner Center om te zien of deze wordt gevuld met crm-id.</span><span class="sxs-lookup"><span data-stu-id="1df82-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="1df82-219">Zorg ervoor dat de deal niet per ongeluk wordt gesloten als **Gewonnen** of Verloren **in** Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1df82-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1df82-220">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="1df82-220">Next steps</span></span>

- [<span data-ttu-id="1df82-221">Leads beheren</span><span class="sxs-lookup"><span data-stu-id="1df82-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="1df82-222">Collectieve-verkoopkansen beheren</span><span class="sxs-lookup"><span data-stu-id="1df82-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
