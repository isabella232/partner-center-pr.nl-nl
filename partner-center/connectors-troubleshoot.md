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
ms.openlocfilehash: b8977f7c602b8587a619236b37a760a55bf87e53
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354539"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="f0f57-104">Problemen oplossen met referrals connectors</span><span class="sxs-lookup"><span data-stu-id="f0f57-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="f0f57-105">**Van toepassing op:**</span><span class="sxs-lookup"><span data-stu-id="f0f57-105">**Applies to:**</span></span>

- <span data-ttu-id="f0f57-106">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="f0f57-106">Dynamics 365 CRM</span></span>
- <span data-ttu-id="f0f57-107">Sales Force CRM</span><span class="sxs-lookup"><span data-stu-id="f0f57-107">Salesforce CRM</span></span>

<span data-ttu-id="f0f57-108">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="f0f57-108">**Appropriate roles**</span></span>

- <span data-ttu-id="f0f57-109">Beheerder van verwijzingen</span><span class="sxs-lookup"><span data-stu-id="f0f57-109">Referrals admin</span></span>
- <span data-ttu-id="f0f57-110">Systeem beheerder of systeemaanpasser op de CRM</span><span class="sxs-lookup"><span data-stu-id="f0f57-110">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="f0f57-111">Vragen en antwoorden over vereisten</span><span class="sxs-lookup"><span data-stu-id="f0f57-111">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="f0f57-112">Kunt u gebruikmaken van de connectors oplossing voor het gebruik van een proef abonnement voor uw omgeving?</span><span class="sxs-lookup"><span data-stu-id="f0f57-112">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="f0f57-113">Als u zich in de test-of faserings omgeving bevindt, kunt u kiezen voor een proef oplossing.</span><span class="sxs-lookup"><span data-stu-id="f0f57-113">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="f0f57-114">De betaalde versie van de connectors is beschikbaar in AppSource voor ons $15/maand.</span><span class="sxs-lookup"><span data-stu-id="f0f57-114">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="f0f57-115">Met de betaalde verbinding krijgt u dagelijks 10K API-aanroepen per dag.</span><span class="sxs-lookup"><span data-stu-id="f0f57-115">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="f0f57-116">De connectors zijn wrappers boven op Partner Center-Referral-Api's.</span><span class="sxs-lookup"><span data-stu-id="f0f57-116">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="f0f57-117">Wanneer de connector oplossingen worden uitgevoerd voor een gebeurtenis **maken** of **bijwerken** voor de mogelijkheden van het partner centrum of de CRM-kant, wordt een API-aanroep uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="f0f57-117">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="f0f57-118">Welke rol hebt u nodig voor het maken van secties in een CRM-omgeving?</span><span class="sxs-lookup"><span data-stu-id="f0f57-118">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="f0f57-119">Gebruikers die systeem beheerders of systeemaanpassers zijn, kunnen wijzigingen voor iedereen Toep assen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-119">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="f0f57-120">Alle app-gebruikers kunnen het systeem echter personaliseren en hun aanpassingen zelfs delen met anderen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-120">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="f0f57-121">Hebben partner verkopers speciale rollen nodig voor het werken met partner Center?</span><span class="sxs-lookup"><span data-stu-id="f0f57-121">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="f0f57-122">Partner verkopers moeten de rol ' verwijzingen beheerder ' toewijzen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-122">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="f0f57-123">Raadpleeg het volgende [machtigingen overzicht) (create-user-accounts-and-set-permissions) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f0f57-123">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="f0f57-124">Welke velden moeten eerst in uw CRM-omgeving worden ingesteld?</span><span class="sxs-lookup"><span data-stu-id="f0f57-124">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="f0f57-125">• Zorg ervoor dat uw valuta geschikt is voor uw locatie en correct in uw CRM-omgeving is.</span><span class="sxs-lookup"><span data-stu-id="f0f57-125">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="f0f57-126">• Uw verkoop team moet worden vermeld in uw CRM-omgeving als CRM-gebruikers.</span><span class="sxs-lookup"><span data-stu-id="f0f57-126">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="f0f57-127">Welke vereisten zijn er vereist voor het automatisch maken van een omgeving?</span><span class="sxs-lookup"><span data-stu-id="f0f57-127">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="f0f57-128">U hebt het volgende nodig om de omgeving voor het automatiseren van de Power te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="f0f57-128">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="f0f57-129">Er is een energiebeheer licentie vereist.</span><span class="sxs-lookup"><span data-stu-id="f0f57-129">A Power Automate license is required.</span></span>
- <span data-ttu-id="f0f57-130">Er is mini maal 1 GB opslag vereist.</span><span class="sxs-lookup"><span data-stu-id="f0f57-130">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="f0f57-131">Hebt u een Dynamics 365-abonnement nodig om Sales Force connectors-oplossing te gebruiken?</span><span class="sxs-lookup"><span data-stu-id="f0f57-131">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="f0f57-132">De oplossing voor de Sales Force-connector is van het type ' Dynamics flow ' dat synchronisatie met andere CRM-systemen ondersteunt.</span><span class="sxs-lookup"><span data-stu-id="f0f57-132">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="f0f57-133">Voor de oplossing is geen Dynamics 365-exemplaar of een abonnement vereist.</span><span class="sxs-lookup"><span data-stu-id="f0f57-133">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="f0f57-134">Tijdens de installatie van de Sales Force-oplossing kan er een vervolg keuzelijst met de bestaande CDS-omgeving in uw bedrijf worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="f0f57-134">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="f0f57-135">U moet die omgeving selecteren.</span><span class="sxs-lookup"><span data-stu-id="f0f57-135">You need to select that environment.</span></span> <span data-ttu-id="f0f57-136">Als u bovendien de fout ' kan geen Dynamics 365-organisatie vinden die is verbonden met een aangemelde gebruiker ' krijgt, moet u een nieuwe omgeving maken voor de connector.</span><span class="sxs-lookup"><span data-stu-id="f0f57-136">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="f0f57-137">Vragen en antwoorden over configuratie</span><span class="sxs-lookup"><span data-stu-id="f0f57-137">Questions and answers about configuration</span></span>

1. <span data-ttu-id="f0f57-138">Wat moet u doen als u de volgende fout melding krijgt bij het activeren van stromen in het energiebeheer platform?</span><span class="sxs-lookup"><span data-stu-id="f0f57-138">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="f0f57-139">Fout: de aanvraag voor het Azure Resource Manager is mislukt met de volgende fout: {"Error": {"code": "WorkflowTriggerNotFound", "Message": "de trigger ' e14d00f1-1fdf-4b1b-AAAC-54a5064093d3 ' van de werk stroom kan niet worden gevonden.}}.</span><span class="sxs-lookup"><span data-stu-id="f0f57-139">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="f0f57-140">Volg deze stappen voor probleem oplossing:</span><span class="sxs-lookup"><span data-stu-id="f0f57-140">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="f0f57-141">Verwijder de CDS-verbinding en maak de CDS-verbindingen opnieuw.</span><span class="sxs-lookup"><span data-stu-id="f0f57-141">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="f0f57-142">Onderliggende stroom in-en uitschakelen</span><span class="sxs-lookup"><span data-stu-id="f0f57-142">Turn the child flow off and on</span></span> 
- <span data-ttu-id="f0f57-143">Verwijder de oplossing en installeer vervolgens de oplossing opnieuw.</span><span class="sxs-lookup"><span data-stu-id="f0f57-143">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="f0f57-144">Wat moet u doen als u de fout melding meldt bij het toevoegen van een partner Center-connector in het geautomatiseerde platform?</span><span class="sxs-lookup"><span data-stu-id="f0f57-144">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Fout bericht waarvoor aanmelding is vereist":::

<span data-ttu-id="f0f57-146">Volg deze stappen voor probleem oplossing:</span><span class="sxs-lookup"><span data-stu-id="f0f57-146">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="f0f57-147">Gebruik de referenties van uw partner centrum om u eenmaal aan te melden bij de stroom omgeving (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="f0f57-147">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="f0f57-148">Wat moet u doen als de volgende fout wordt weer gegeven tijdens het activeren van het partner centrum naar CRM-stroom in het geautomatiseerde platform?</span><span class="sxs-lookup"><span data-stu-id="f0f57-148">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Fout bericht dat updates vereist":::

<span data-ttu-id="f0f57-150">Volg deze stappen voor probleem oplossing:</span><span class="sxs-lookup"><span data-stu-id="f0f57-150">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="f0f57-151">Activeer eerst de volgende twee onderliggende stromen voordat u het partner centrum naar CRM-stroom activeert.</span><span class="sxs-lookup"><span data-stu-id="f0f57-151">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="f0f57-152">Partner centrum voor CRM-helper (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-152">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="f0f57-153">Partner centrum micro soft-referentie-updates verkopen aan CRM (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-153">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="f0f57-154">Wat moet u doen als u geen verbindingen kunt toevoegen aan de stroom wanneer u de stroom probeert te bewerken?</span><span class="sxs-lookup"><span data-stu-id="f0f57-154">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="f0f57-155">U voegt verbindingen toe aan de stroom terwijl de stroom wordt uitgevoerd. u kunt elke stroom afzonderlijk toevoegen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-155">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="f0f57-156">Als het dialoog venster voor het toevoegen van verbindingen niet automatisch wordt geopend tijdens het bewerken van de stroom, kunt u elk van de stappen en substappen van de stromen afzonderlijk bewerken.</span><span class="sxs-lookup"><span data-stu-id="f0f57-156">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="f0f57-157">Selecteer elke stroom en bewerk ze afzonderlijk.</span><span class="sxs-lookup"><span data-stu-id="f0f57-157">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="f0f57-158">Alle stappen in de stroom uitvouwen</span><span class="sxs-lookup"><span data-stu-id="f0f57-158">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Stappen die verbindingen nodig hebben":::

- <span data-ttu-id="f0f57-160">Selecteer de stappen waarin een waarschuwings pictogram wordt weer gegeven om verbindingen te koppelen en verbindingen toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-160">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Stap per stap voor het bewerken van de stroom":::


5. <span data-ttu-id="f0f57-162">Wat moet u doen als de stromen van de connectors oplossing voor het samen verkopen van verwijzingen niet worden ingeschakeld?</span><span class="sxs-lookup"><span data-stu-id="f0f57-162">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="f0f57-163">A.</span><span class="sxs-lookup"><span data-stu-id="f0f57-163">A.</span></span> <span data-ttu-id="f0f57-164">In energie automatisering moet u stromen bewerken in de volgende volg orde en deze bijwerken om de juiste verbindingen te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="f0f57-164">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="f0f57-165">Inschrijving van partner Center-webhooks (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-165">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-166">Een verwijzing naar een gezamenlijk verkoop object maken-Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-166">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-167">Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-167">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-168">Partner centrum naar Sales Force (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-168">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-169">Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-169">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-170">Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-170">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f0f57-171">Sales Force Micro Solutions to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-171">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="f0f57-172">B.</span><span class="sxs-lookup"><span data-stu-id="f0f57-172">B.</span></span> <span data-ttu-id="f0f57-173">Selecteer voor elke stroom de optie **alleen gebruikers uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="f0f57-173">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="f0f57-174">Selecteer **verbinding gebruiken** in plaats van **via alleen-uitvoeren gebruiker**.</span><span class="sxs-lookup"><span data-stu-id="f0f57-174">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Een stroom activeren":::


<span data-ttu-id="f0f57-176">C.</span><span class="sxs-lookup"><span data-stu-id="f0f57-176">C.</span></span> <span data-ttu-id="f0f57-177">Activeer deze hieronder vermelde stromen:</span><span class="sxs-lookup"><span data-stu-id="f0f57-177">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="f0f57-178">Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-178">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="f0f57-179">Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="f0f57-179">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="f0f57-180">D.</span><span class="sxs-lookup"><span data-stu-id="f0f57-180">D.</span></span> <span data-ttu-id="f0f57-181">Alle resterende stromen activeren.</span><span class="sxs-lookup"><span data-stu-id="f0f57-181">Activate all the remaining flows.</span></span>

<span data-ttu-id="f0f57-182">E.</span><span class="sxs-lookup"><span data-stu-id="f0f57-182">E.</span></span> <span data-ttu-id="f0f57-183">Selecteer bij stroom Partner Center-webhook registratie **uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="f0f57-183">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="f0f57-184">Geef de **http-URL** op van de eerste actie in **Partner Center naar Sales Force** -stroom.</span><span class="sxs-lookup"><span data-stu-id="f0f57-184">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="f0f57-185">Selecteer alle vier de opties onder **gebeurtenissen die u wilt registreren** en selecteer **Ja** voor overschrijven.</span><span class="sxs-lookup"><span data-stu-id="f0f57-185">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="f0f57-186">Vragen en antwoorden over uitvoeren/onderhoud</span><span class="sxs-lookup"><span data-stu-id="f0f57-186">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="f0f57-187">Hoe kunt u problemen oplossen wanneer er fouten optreden tijdens het automatiseren van de stroom?</span><span class="sxs-lookup"><span data-stu-id="f0f57-187">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="f0f57-188">Raadpleeg [stroom fouten oplossen](/power-automate/fix-flow-failures)om ervoor te zorgen dat uw stroom stromen automatisch worden uitgevoerd zoals verwacht en problemen tijdens de uitvoering kunnen oplossen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-188">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="f0f57-189">Wat moet u doen als er verwijzingen worden weer geven die niet juist zijn gesynchroniseerd in een partner centrum of een CRM-omgeving?</span><span class="sxs-lookup"><span data-stu-id="f0f57-189">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="f0f57-190">Selecteer **audit** om de status van de verwijzings synchronisatie te bepalen.</span><span class="sxs-lookup"><span data-stu-id="f0f57-190">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Verwijzingen synchroniseren":::

<span data-ttu-id="f0f57-192">Zorg ervoor dat aan de volgende voor waarden wordt voldaan:</span><span class="sxs-lookup"><span data-stu-id="f0f57-192">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="f0f57-193">De oplossings-ID is opgenomen als onderdeel van de verkoop kans.</span><span class="sxs-lookup"><span data-stu-id="f0f57-193">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="f0f57-194">Land code van twee letters is vereist.</span><span class="sxs-lookup"><span data-stu-id="f0f57-194">Two letter country code is required.</span></span>

- <span data-ttu-id="f0f57-195">Wanneer u hulp van micro soft hebt geselecteerd voor de opportuniteit, is contact gegevens van de klant vereist.</span><span class="sxs-lookup"><span data-stu-id="f0f57-195">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="f0f57-196">Hoe kunt u ervoor zorgen dat een verwijzing twee richtingen synchroniseert?</span><span class="sxs-lookup"><span data-stu-id="f0f57-196">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="f0f57-197">Voer de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="f0f57-197">Do the following steps:</span></span>

- <span data-ttu-id="f0f57-198">Partner verkopers moeten ervoor zorgen dat de optie **synchronisatie met partner Center** is ingeschakeld in de sectie CRM.</span><span class="sxs-lookup"><span data-stu-id="f0f57-198">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Zorg ervoor dat u synch hebt ingeschakeld":::

- <span data-ttu-id="f0f57-200">Verkopers moeten een omzet en een afsluitings datum opgeven bij het kwalificeren van een potentiële klant.</span><span class="sxs-lookup"><span data-stu-id="f0f57-200">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="f0f57-201">Als de CRM-ID wordt weer gegeven in de fase **maken** of **bijwerken** van de verkoop kans, maar er geen lead opportuniteit met die id is gevonden in CRM, wordt het bijwerken of maken genegeerd.</span><span class="sxs-lookup"><span data-stu-id="f0f57-201">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="f0f57-202">Zorg ervoor dat het veld referentie valuta is geconfigureerd in de Sales Force-omgeving.</span><span class="sxs-lookup"><span data-stu-id="f0f57-202">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="f0f57-203">Wat moet u doen als de connector wordt losgekoppeld en u geen verwijzings synchronisatie meer hebt.</span><span class="sxs-lookup"><span data-stu-id="f0f57-203">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="f0f57-204">Hier volgen enkele van de opties die u kunt uitproberen:</span><span class="sxs-lookup"><span data-stu-id="f0f57-204">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="f0f57-205">Controleer of de gebruikers naam of het wacht woord voor de partner centrum-gebruiker is verlopen met de rollen beheerder van verwijzing.</span><span class="sxs-lookup"><span data-stu-id="f0f57-205">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="f0f57-206">U kunt naar de niet-gesynchroniseerde verkoop kans gaan, een kleine update maken en bekijken of de verwijzing is gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="f0f57-206">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="f0f57-207">Als de stromen zijn uitgevoerd en mislukt, selecteert u de stroom en verzendt u de uitgevoerde bewerking opnieuw.</span><span class="sxs-lookup"><span data-stu-id="f0f57-207">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="f0f57-208">Wat moet u doen wanneer u geen toegang krijgt tot fouten?</span><span class="sxs-lookup"><span data-stu-id="f0f57-208">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="f0f57-209">Controleer of de juiste rollen bestaan</span><span class="sxs-lookup"><span data-stu-id="f0f57-209">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="f0f57-210">Rol van verwijzings beheerder voor Partner Center-verkoper</span><span class="sxs-lookup"><span data-stu-id="f0f57-210">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="f0f57-211">De rol systeem beheerder of systeemaanpasser op uw CRM-exemplaar</span><span class="sxs-lookup"><span data-stu-id="f0f57-211">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="f0f57-212">Zorg ervoor dat de gebruiker die het stroom account energie automatiseert, https://flow.microsoft.com ten minste één keer vooraf meldt</span><span class="sxs-lookup"><span data-stu-id="f0f57-212">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="f0f57-213">Wat moet u doen als u ziet dat de **land code van het klant account** ontbreekt tijdens het maken van een mede verkoop kans.</span><span class="sxs-lookup"><span data-stu-id="f0f57-213">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="f0f57-214">U moet de ISO-land code van twee letters toevoegen aan het klant account in CRM.</span><span class="sxs-lookup"><span data-stu-id="f0f57-214">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="f0f57-215">Wat moet u doen als u de fout melding ziet dat de **oplossings-id is vereist** tijdens het maken van een verkoop kans op verkoop?</span><span class="sxs-lookup"><span data-stu-id="f0f57-215">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="f0f57-216">Voor het maken van een verwijzing naar een mede verkoop, hebt u een micro soft-oplossing voor een kant-en-klare verkoop nodig.</span><span class="sxs-lookup"><span data-stu-id="f0f57-216">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="f0f57-217">Wat moet u doen wanneer u verkoop kansen die zijn gemaakt in het partner centrum, ziet die niet zijn gesynchroniseerd met CRM, zelfs als er geen stroom fouten zijn:</span><span class="sxs-lookup"><span data-stu-id="f0f57-217">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="f0f57-218">Ga als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="f0f57-218">Do the following:</span></span>

- <span data-ttu-id="f0f57-219">Nadat u een nieuwe mede verkochte deal in het partner centrum hebt gemaakt, controleert u of het partner centrum voor Dynamics 365 stroom wordt aangeroepen (het kan meerdere keren worden opgeroepen).</span><span class="sxs-lookup"><span data-stu-id="f0f57-219">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="f0f57-220">Als de stroom wordt aangeroepen, controleert u alle aanroepen van stromen en identificeert u de stroom uitvoering waarmee de CRM wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="f0f57-220">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="f0f57-221">U kunt de acties volgen en controleren of er een probleem is opgetreden bij het bijwerken van het CRM.</span><span class="sxs-lookup"><span data-stu-id="f0f57-221">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="f0f57-222">Controleer de *nieuwe deal*\* in het partner centrum om te zien of deze wordt gevuld met CRM-id.</span><span class="sxs-lookup"><span data-stu-id="f0f57-222">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="f0f57-223">Zorg ervoor dat de deal niet per ongeluk is gesloten als "gewonnen" of "verloren" in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="f0f57-223">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f0f57-224">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="f0f57-224">Next steps</span></span>

- [<span data-ttu-id="f0f57-225">Leads beheren</span><span class="sxs-lookup"><span data-stu-id="f0f57-225">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="f0f57-226">Collectieve-verkoopkansen beheren</span><span class="sxs-lookup"><span data-stu-id="f0f57-226">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
