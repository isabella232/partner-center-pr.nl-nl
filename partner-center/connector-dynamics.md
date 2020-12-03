---
title: De connector voor het samen verkopen van Dynamics 365 CRM-partner centrum
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Synchroniseer verwijzingen in het partner centrum met de connector voor co-sell voor Dynamics 365 CRM. Verkopers kunnen vervolgens samen met micro soft verkopen binnen uw CRM-systemen.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556358"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="e04eb-104">Connector voor Dynamics 365-overzicht co-sell</span><span class="sxs-lookup"><span data-stu-id="e04eb-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="e04eb-105">Juiste rollen</span><span class="sxs-lookup"><span data-stu-id="e04eb-105">Appropriate roles</span></span>

- <span data-ttu-id="e04eb-106">Beheerder van verwijzingen</span><span class="sxs-lookup"><span data-stu-id="e04eb-106">Referrals admin</span></span>
- <span data-ttu-id="e04eb-107">Systeem beheerder of systeemaanpasser op de CRM</span><span class="sxs-lookup"><span data-stu-id="e04eb-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="e04eb-108">Met connector voor co-sell van partner Center kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="e04eb-109">Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="e04eb-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="e04eb-110">Gebruik de co-Connect connectors om een nieuwe verwijzing naar de verkoop te maken voor een micro soft-verkoper, referenties te ontvangen van de micro soft-verkoper, verwijzingen te accepteren/weigeren, afhandelings gegevens te wijzigen, zoals een deal waarde en een sluitings datum.</span><span class="sxs-lookup"><span data-stu-id="e04eb-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="e04eb-111">U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals.</span><span class="sxs-lookup"><span data-stu-id="e04eb-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="e04eb-112">U kunt al uw verwijzingen gebruiken binnen de CRM van uw keuze in plaats van in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e04eb-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="e04eb-113">De oplossing is gebaseerd op de micro soft-oplossing voor energie automatisering en maakt gebruik van partner Center-Api's.</span><span class="sxs-lookup"><span data-stu-id="e04eb-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="e04eb-114">Voordat u de vereisten installeert</span><span class="sxs-lookup"><span data-stu-id="e04eb-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="e04eb-115">**Onderwerpen**</span><span class="sxs-lookup"><span data-stu-id="e04eb-115">**Topics**</span></span>   |<span data-ttu-id="e04eb-116">**Details**</span><span class="sxs-lookup"><span data-stu-id="e04eb-116">**Details**</span></span>   |<span data-ttu-id="e04eb-117">**Koppelingen**</span><span class="sxs-lookup"><span data-stu-id="e04eb-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="e04eb-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="e04eb-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="e04eb-119">U hebt een geldige MPN-ID nodig</span><span class="sxs-lookup"><span data-stu-id="e04eb-119">You need a valid MPN ID</span></span>|<span data-ttu-id="e04eb-120">Toevoegen aan [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="e04eb-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="e04eb-121">Klaar voor de verkoop</span><span class="sxs-lookup"><span data-stu-id="e04eb-121">Cosell ready</span></span>|<span data-ttu-id="e04eb-122">Uw IP/Services-oplossing moet samen worden verkocht.</span><span class="sxs-lookup"><span data-stu-id="e04eb-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="e04eb-123">Verkopen met micro soft</span><span class="sxs-lookup"><span data-stu-id="e04eb-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="e04eb-124">Partnercentrum-account</span><span class="sxs-lookup"><span data-stu-id="e04eb-124">Partner Center account</span></span>|<span data-ttu-id="e04eb-125">De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling.</span><span class="sxs-lookup"><span data-stu-id="e04eb-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="e04eb-126">Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in partner centrum Portal kunt zien.</span><span class="sxs-lookup"><span data-stu-id="e04eb-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="e04eb-127">Uw account beheren</span><span class="sxs-lookup"><span data-stu-id="e04eb-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="e04eb-128">Gebruikers rollen voor het partner centrum</span><span class="sxs-lookup"><span data-stu-id="e04eb-128">Partner Center user roles</span></span>|<span data-ttu-id="e04eb-129">De werk nemer die de connectors installeert en gebruikt, moet een referentie beheerder zijn</span><span class="sxs-lookup"><span data-stu-id="e04eb-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="e04eb-130">Beheerdersrollen en -machtigingen toewijzen</span><span class="sxs-lookup"><span data-stu-id="e04eb-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="e04eb-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="e04eb-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="e04eb-132">De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser</span><span class="sxs-lookup"><span data-stu-id="e04eb-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="e04eb-133">Rollen toewijzen in Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="e04eb-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="e04eb-134">Stroom account voor energie automatisering</span><span class="sxs-lookup"><span data-stu-id="e04eb-134">Power Automate Flow Account</span></span>|<span data-ttu-id="e04eb-135">Een actief [geautomatiseerd](https://flow.microsoft.com) account voor het beheer van de CRM-systeem beheerder of het systeem.</span><span class="sxs-lookup"><span data-stu-id="e04eb-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="e04eb-136">Deze gebruiker moet zich ten minste één keer aanmelden bij Power voor het [automatiseren](https://flow.microsoft.com) van de installatie.</span><span class="sxs-lookup"><span data-stu-id="e04eb-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="e04eb-137">Synchronisatie van partner Center referrals voor Dynamics 365 (oplossing voor automatische stroom) installeren</span><span class="sxs-lookup"><span data-stu-id="e04eb-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="e04eb-138">Ga naar [Automatische stroom](https://flow.microsoft.com) en selecteer **omgevingen** in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="e04eb-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="e04eb-139">In deze stap ziet u de beschik bare CRM-exemplaren.</span><span class="sxs-lookup"><span data-stu-id="e04eb-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="e04eb-140">Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="e04eb-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="e04eb-141">Selecteer **oplossingen** op de linkernavigatiebalk.</span><span class="sxs-lookup"><span data-stu-id="e04eb-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="e04eb-142">Klik op de koppeling **Open AppSource** in het bovenste menu.</span><span class="sxs-lookup"><span data-stu-id="e04eb-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource openen":::

5. <span data-ttu-id="e04eb-144">Zoek naar **Partner Center referrals connectors voor Dynamics365** in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="e04eb-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="e04eb-145">Klik op de knop **nu downloaden** en vervolgens op **door gaan**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="e04eb-146">Hiermee opent u de pagina waar u de CRM-omgeving (Dynamics 365) kunt selecteren om de toepassing te installeren.</span><span class="sxs-lookup"><span data-stu-id="e04eb-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="e04eb-147">Ga akkoord met de voor waarden.</span><span class="sxs-lookup"><span data-stu-id="e04eb-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="e04eb-148">Vervolgens gaat u naar de pagina **uw oplossingen beheren** .</span><span class="sxs-lookup"><span data-stu-id="e04eb-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="e04eb-149">Navigeer naar partner Center referrals met behulp van de pijl knoppen aan de onderkant van de pagina.</span><span class="sxs-lookup"><span data-stu-id="e04eb-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="e04eb-150">**Geplande installatie** moet naast Partner Center referrals-oplossing worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="e04eb-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="e04eb-151">De installatie duurt 10-15 minuten.</span><span class="sxs-lookup"><span data-stu-id="e04eb-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="e04eb-152">Zodra de installatie is voltooid, gaat u terug naar [energie automatisering](https://flow.microsoft.com) en selecteert u **oplossingen** vanuit het navigatie gebied links.</span><span class="sxs-lookup"><span data-stu-id="e04eb-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="e04eb-153">U ziet dat **Partner Center referrals synchronisatie voor Dynamics 365** beschikbaar is in de lijst met oplossingen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="e04eb-154">Selecteer de **synchronisatie van partner Center referrals voor Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="e04eb-155">De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar:</span><span class="sxs-lookup"><span data-stu-id="e04eb-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Beschik bare CRMS":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="e04eb-157">Best practice: test voordat u live gaat</span><span class="sxs-lookup"><span data-stu-id="e04eb-157">Best practice: test before you go live</span></span>

<span data-ttu-id="e04eb-158">Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test.</span><span class="sxs-lookup"><span data-stu-id="e04eb-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="e04eb-159">Installeer de oplossing voor het automatiseren van micro soft power op een staging-omgeving/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="e04eb-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="e04eb-160">Maak een kopie van de oplossing en voer uw configuratie uit en Automatiseer de stroom aanpassingen in de faserings omgeving.</span><span class="sxs-lookup"><span data-stu-id="e04eb-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="e04eb-161">Test de oplossing op een staging/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="e04eb-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="e04eb-162">Importeer bij geslaagd als beheerde oplossing naar het productie-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="e04eb-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="e04eb-163">De oplossing configureren</span><span class="sxs-lookup"><span data-stu-id="e04eb-163">Configure the solution</span></span>

1. <span data-ttu-id="e04eb-164">Wanneer u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Automatische stroom](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="e04eb-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="e04eb-165">Selecteer in de vervolg keuzelijst **omgevingen** in de rechter BOVENHOEK het CRM-exemplaar waarop u de oplossing voor het automatiseren van energie beheer hebt geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="e04eb-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="e04eb-166">U moet verbindingen maken die de drie gebruikers accounts koppelen:</span><span class="sxs-lookup"><span data-stu-id="e04eb-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="e04eb-167">Partner centrum-gebruiker met referrals beheerders referenties</span><span class="sxs-lookup"><span data-stu-id="e04eb-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="e04eb-168">Partnercentrum-gebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="e04eb-168">Partner Center Events</span></span>

   - <span data-ttu-id="e04eb-169">CRM-beheerder met de stroom voor het automatiseren van stromen in de oplossing.</span><span class="sxs-lookup"><span data-stu-id="e04eb-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="e04eb-170">Selecteer **verbindingen** in de linkernavigatiebalk en selecteer de oplossing Partner Center referrals in de lijst.</span><span class="sxs-lookup"><span data-stu-id="e04eb-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="e04eb-171">Maak een verbinding door te klikken op **een verbinding maken**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Verbinding maken":::

      3. <span data-ttu-id="e04eb-173">Zoek naar **Partner Center referrals (preview)** in de zoek balk in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="e04eb-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="e04eb-174">Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="e04eb-175">Maak vervolgens een verbinding met de partner centrum-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de beheerder.</span><span class="sxs-lookup"><span data-stu-id="e04eb-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="e04eb-176">Maak een verbinding voor Common Data Service (huidige omgeving) voor de gebruiker van de CRM-beheerder.</span><span class="sxs-lookup"><span data-stu-id="e04eb-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="e04eb-177">Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:</span><span class="sxs-lookup"><span data-stu-id="e04eb-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Verbindingen":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="e04eb-179">De verbindingen bewerken</span><span class="sxs-lookup"><span data-stu-id="e04eb-179">Edit the connections</span></span>

1. <span data-ttu-id="e04eb-180">Ga terug naar de pagina **oplossingen** en selecteer **standaard oplossing**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="e04eb-181">Selecteer **verbindings verwijzing (preview)** door te klikken op **alle**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Verbinding maken":::

2. <span data-ttu-id="e04eb-183">Bewerk elk van de verbindingen één voor één door het pictogram drie punten te selecteren.</span><span class="sxs-lookup"><span data-stu-id="e04eb-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="e04eb-184">Voeg de relevante verbindingen toe.</span><span class="sxs-lookup"><span data-stu-id="e04eb-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Verbindingen vermeld"::: 

3.  <span data-ttu-id="e04eb-186">Schakel de stromen in de volgende volg orde in:</span><span class="sxs-lookup"><span data-stu-id="e04eb-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="e04eb-187">Inschrijving van partner Center-webhooks (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-188">Een verwijzing naar een co-sell maken – Dynamics 365 naar partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-189">Partner centrum referentie-updates voor micro soft-verkoop naar Dynamics 365 (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-190">Partner centrum voor Dynamics 365 (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-191">Dynamics 365 naar partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-192">Dynamics 365-opportunity naar partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="e04eb-193">Dynamics 365 micro soft Solutions to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="e04eb-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="e04eb-194">Webhook-Api's gebruiken om te registreren voor bron wijzigings gebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="e04eb-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="e04eb-195">Met de webhook-Api's van partner Center kunt u zich registreren voor bron wijzigings gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="e04eb-196">Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.</span><span class="sxs-lookup"><span data-stu-id="e04eb-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="e04eb-197">Als u uw URL wilt registreren, selecteert u stroom voor het automatiseren van de data **Center-webhook-registratie (Insider preview)** .</span><span class="sxs-lookup"><span data-stu-id="e04eb-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="e04eb-198">Verbindingen toevoegen voor een partner centrum-gebruiker (a.) met referrals beheerders referenties (b.) partner Center-gebeurtenissen zoals hieronder gemarkeerd</span><span class="sxs-lookup"><span data-stu-id="e04eb-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="e04eb-200">Wanneer u deze updates maakt, ziet u</span><span class="sxs-lookup"><span data-stu-id="e04eb-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="e04eb-202">Sla de wijzigingen op en selecteer **inschakelen**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="e04eb-203">Voer de volgende stappen uit om het partner centrum-webhooks in te scha kelen voor het Luis teren naar gebeurtenis wijzigingen:</span><span class="sxs-lookup"><span data-stu-id="e04eb-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="e04eb-204">Selecteer **partner centrum voor Dynamics 365 (Insider preview)**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="e04eb-205">Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="e04eb-206">Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.</span><span class="sxs-lookup"><span data-stu-id="e04eb-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL kopiëren":::

8. <span data-ttu-id="e04eb-208">Selecteer nu de stroom voor het automatiseren van partner Center-webhooks (Insider preview) en selecteer **uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="e04eb-209">Zorg ervoor dat het venster stroom uitvoeren wordt geopend in het rechterdeel venster en klik op **door gaan**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="e04eb-210">Voer de volgende details in:</span><span class="sxs-lookup"><span data-stu-id="e04eb-210">Enter the following details:</span></span>

    1. <span data-ttu-id="e04eb-211">**Http-trigger eindpunt**: URL gekopieerd uit eerdere stap</span><span class="sxs-lookup"><span data-stu-id="e04eb-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="e04eb-212">**Te registreren gebeurtenissen**: ' verwijzing-gemaakt ' en ' referentie-bijgewerkt '</span><span class="sxs-lookup"><span data-stu-id="e04eb-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="e04eb-213">**Bestaande trigger eindpunten overschrijven indien aanwezig**: Ja (Hiermee worden alle bestaande eind punten overschreven.)</span><span class="sxs-lookup"><span data-stu-id="e04eb-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="e04eb-214">Selecteer **uitvoeren** en selecteer vervolgens **gereed.**</span><span class="sxs-lookup"><span data-stu-id="e04eb-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="e04eb-215">De webhook kan nu Luis teren om gebeurtenissen te maken en bij te werken.</span><span class="sxs-lookup"><span data-stu-id="e04eb-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="e04eb-216">Synchronisatie stappen aanpassen</span><span class="sxs-lookup"><span data-stu-id="e04eb-216">Customize synchronization steps</span></span>

<span data-ttu-id="e04eb-217">Als er verwijzingen naar links worden gesynchroniseerd tussen partner centrum en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-PC hier vermeld.</span><span class="sxs-lookup"><span data-stu-id="e04eb-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="e04eb-218">Vaak worden de CRM-systemen zeer aangepast.</span><span class="sxs-lookup"><span data-stu-id="e04eb-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="e04eb-219">U kunt de stroom voor het automatiseren van stromen aanpassen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="e04eb-220">Volg de instructies in de hand leiding voor de veld toewijzing en breng zo nodig de juiste wijzigingen aan in de stappen van de stroom automatische stromen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="e04eb-221">Micro soft partner Centers naar CRM-toewijzingen worden gegeven, maar op basis van uw CRM-omgeving kunt u ervoor kiezen om de velden verder aan te passen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="e04eb-222">Meerdere stappen van elk van de energiebeheer stromen kunnen worden aangepast op basis van uw behoeften.</span><span class="sxs-lookup"><span data-stu-id="e04eb-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="e04eb-223">Hier volgen enkele voor beelden van beschik bare aanpassingen:</span><span class="sxs-lookup"><span data-stu-id="e04eb-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="e04eb-224">Als u de velden voor de gebeurtenissen maken of bijwerken in het partner centrum wilt aanpassen aan CRM Referral-synchronisatie:</span><span class="sxs-lookup"><span data-stu-id="e04eb-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="e04eb-225">a.</span><span class="sxs-lookup"><span data-stu-id="e04eb-225">a.</span></span> <span data-ttu-id="e04eb-226">Selecteer partner centrum voor Dynamics 365 (Insider preview) of partner centrum naar Sales Force (Insider preview).</span><span class="sxs-lookup"><span data-stu-id="e04eb-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="e04eb-227">b.</span><span class="sxs-lookup"><span data-stu-id="e04eb-227">b.</span></span> <span data-ttu-id="e04eb-228">Selecteer **bewerken** om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="e04eb-229">c.</span><span class="sxs-lookup"><span data-stu-id="e04eb-229">c.</span></span> <span data-ttu-id="e04eb-230">Selecteer **(bereik) de lead of de opportuniteit synchroniseren**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="e04eb-231">Als u CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen wilt aanpassen, selecteert u **of het een nieuwe gedeelde verkoop kans is en klikt u vervolgens** op.</span><span class="sxs-lookup"><span data-stu-id="e04eb-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="e04eb-232">Selecteer de substap **als** dit het geval is en vouw vervolgens **een nieuwe opportuniteit maken in het CRM** uit.</span><span class="sxs-lookup"><span data-stu-id="e04eb-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="e04eb-233">U kunt de toewijzingen in deze sectie bewerken met de gids voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="e04eb-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="e04eb-234">d.</span><span class="sxs-lookup"><span data-stu-id="e04eb-234">d.</span></span> <span data-ttu-id="e04eb-235">Voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor update gebeurtenissen, klikt u op de stap (bereik) synchroniseren van de lead of de verkoop kans.</span><span class="sxs-lookup"><span data-stu-id="e04eb-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="e04eb-236">e.</span><span class="sxs-lookup"><span data-stu-id="e04eb-236">e.</span></span> <span data-ttu-id="e04eb-237">Selecteer **deze optie als het een update is voor een verkoop kans en klik vervolgens**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="e04eb-238">Selecteer de substap **Indien ja** en vouw vervolgens uit **als het verschil tussen de objecten verkoop kansen in partner centrum en CRM**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="e04eb-239">f.</span><span class="sxs-lookup"><span data-stu-id="e04eb-239">f.</span></span> <span data-ttu-id="e04eb-240">Selecteren **als ja** , gevolgd door **bestaande verkoop kans bijwerken**</span><span class="sxs-lookup"><span data-stu-id="e04eb-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="e04eb-241">De velden voor CRM naar PC Referral Synchronization voor update gebeurtenissen aanpassen:</span><span class="sxs-lookup"><span data-stu-id="e04eb-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="e04eb-242">a.</span><span class="sxs-lookup"><span data-stu-id="e04eb-242">a.</span></span> <span data-ttu-id="e04eb-243">Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="e04eb-244">b.</span><span class="sxs-lookup"><span data-stu-id="e04eb-244">b.</span></span> <span data-ttu-id="e04eb-245">Selecteer **(bereik) de opportuniteit synchroniseren**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="e04eb-246">c.</span><span class="sxs-lookup"><span data-stu-id="e04eb-246">c.</span></span> <span data-ttu-id="e04eb-247">Als u de CRM-veld toewijzingen voor update gebeurtenissen wilt aanpassen, selecteert u **of er verschillen zijn tussen de objecten leads in partner centrum en CRM**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="e04eb-248">d.</span><span class="sxs-lookup"><span data-stu-id="e04eb-248">d.</span></span> <span data-ttu-id="e04eb-249">Selecteer de substap **als ja** en vouw vervolgens de stap **een referral met verkoopkansgegevens bijwerken** uit.</span><span class="sxs-lookup"><span data-stu-id="e04eb-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="e04eb-250">U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="e04eb-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="e04eb-251">De velden voor CRM naar PC Referral-synchronisatie aanpassen voor het maken van gebeurtenissen?</span><span class="sxs-lookup"><span data-stu-id="e04eb-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="e04eb-252">a.</span><span class="sxs-lookup"><span data-stu-id="e04eb-252">a.</span></span> <span data-ttu-id="e04eb-253">Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="e04eb-254">b.</span><span class="sxs-lookup"><span data-stu-id="e04eb-254">b.</span></span> <span data-ttu-id="e04eb-255">Selecteer **(bereik) het synchroniseren van verwijzingen.**</span><span class="sxs-lookup"><span data-stu-id="e04eb-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="e04eb-256">c.</span><span class="sxs-lookup"><span data-stu-id="e04eb-256">c.</span></span> <span data-ttu-id="e04eb-257">Selecteer **micro soft Referral maken** voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="e04eb-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="e04eb-258">U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="e04eb-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="e04eb-259">Er zijn twee omgevings variabelen gemaakt:</span><span class="sxs-lookup"><span data-stu-id="e04eb-259">There are two environment variables created:</span></span>

- <span data-ttu-id="e04eb-260">Vinkje: geeft aan of u een vinkje zou moeten hebben naast de verkoop kansen die in twee richtingen tussen partner centrum en Dynamics 365 CRM worden gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="e04eb-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="e04eb-261">Alleen verkoop kansen synchroniseren: geeft aan of u alleen verkoop kansen wilt synchroniseren.</span><span class="sxs-lookup"><span data-stu-id="e04eb-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="e04eb-262">U kunt ervoor kiezen de standaard waarde voor de omgevings variabelen te bewerken.</span><span class="sxs-lookup"><span data-stu-id="e04eb-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Invoervak voor standaard waarden":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="e04eb-264">End-to-end-synchronisatie van Referral-verkoop referenties</span><span class="sxs-lookup"><span data-stu-id="e04eb-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="e04eb-265">Zodra u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Dynamics 365 en partner centrum.</span><span class="sxs-lookup"><span data-stu-id="e04eb-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="e04eb-266">Vereisten</span><span class="sxs-lookup"><span data-stu-id="e04eb-266">Pre-requisites</span></span>

<span data-ttu-id="e04eb-267">Voor het synchroniseren van de verwijzingen tussen partner centrum en Dynamics 365 CRM, is de oplossing voor het automatiseren van de stroom een duidelijke verwijzings velden van micro soft.</span><span class="sxs-lookup"><span data-stu-id="e04eb-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="e04eb-268">Met deze identificatie kunnen uw verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.</span><span class="sxs-lookup"><span data-stu-id="e04eb-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="e04eb-269">Een set aangepaste velden is beschikbaar als onderdeel van de entiteit **verkoop kans** .</span><span class="sxs-lookup"><span data-stu-id="e04eb-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="e04eb-270">Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .</span><span class="sxs-lookup"><span data-stu-id="e04eb-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="e04eb-271">De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:</span><span class="sxs-lookup"><span data-stu-id="e04eb-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="e04eb-272">**Synchroniseren met partner centrum**: of u de mogelijkheid wilt synchroniseren met micro soft Partner Center</span><span class="sxs-lookup"><span data-stu-id="e04eb-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="e04eb-273">**Verwijzings-id**: een veld met alleen-lezen-id voor micro soft Partner Center Referral</span><span class="sxs-lookup"><span data-stu-id="e04eb-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="e04eb-274">**Verwijzings koppeling**: een alleen-lezen koppeling naar de verwijzing in het micro soft partner centrum</span><span class="sxs-lookup"><span data-stu-id="e04eb-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="e04eb-275">**Hoe kan ik Help** van micro soft helpen?: micro soft vereist voor de verwijzing</span><span class="sxs-lookup"><span data-stu-id="e04eb-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="e04eb-276">**Producten**: lijst met producten die zijn gekoppeld aan deze verkoop kans</span><span class="sxs-lookup"><span data-stu-id="e04eb-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="e04eb-277">**Controle**: een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen</span><span class="sxs-lookup"><span data-stu-id="e04eb-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="e04eb-278">Werk het verkoopkansformulier in Dynamics 365 CRM bij met oplossingen voor het veld Products.</span><span class="sxs-lookup"><span data-stu-id="e04eb-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulier Verkoop kans":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a><span data-ttu-id="e04eb-281">DENKBAAR</span><span class="sxs-lookup"><span data-stu-id="e04eb-281">SCENARIOS:</span></span>

1. <span data-ttu-id="e04eb-282">Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en gesynchroniseerd in partner centrum:</span><span class="sxs-lookup"><span data-stu-id="e04eb-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="e04eb-283">Meld u aan bij uw Dynamics 365 CRM-omgeving met een zicht baarheid in het gedeelte **verkoop kansen** van de CRM.</span><span class="sxs-lookup"><span data-stu-id="e04eb-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="e04eb-284">Zorg ervoor dat de volgende sectie aanwezig is wanneer u een ' nieuwe mogelijkheid ' in de Dynamics 365-omgeving maakt</span><span class="sxs-lookup"><span data-stu-id="e04eb-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sectie voor beeld van verkoop kansen met informatie over micro soft Partner Center in Dynamics 365.":::

   3. <span data-ttu-id="e04eb-286">Als u deze mogelijkheid wilt synchroniseren met micro soft Partner Center, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:</span><span class="sxs-lookup"><span data-stu-id="e04eb-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="e04eb-287">**Synchroniseren met partner centrum**: Ja</span><span class="sxs-lookup"><span data-stu-id="e04eb-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="e04eb-288">**Hoe kan micro soft u helpen?**: Selecteer een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="e04eb-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sectie voor beeld van verkoop kansen in Dynamics 365 waarin de Help-opties van micro soft Partner Center worden weer gegeven naast een veld met de naam hoe kan micro soft u helpen?":::

      - <span data-ttu-id="e04eb-290">**Producten**: oplossings-id's van het product</span><span class="sxs-lookup"><span data-stu-id="e04eb-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="e04eb-291">Zodra de opportuniteit is gemaakt in Dynamics 365 met **synchronisatie met** de optie voor Partner Center is ingesteld op **Ja**, wacht u 10 minuten en meldt u zich aan bij uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="e04eb-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="e04eb-292">Uw verwijzingen worden gesynchroniseerd met Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e04eb-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="e04eb-293">Voor een verkoop kans waarvoor de optie ' synchroniseren met partner centrum ' is ingesteld op ' ja ' en u de verkoop kans bijwerkt in Dynamics 365 CRM, worden de wijzigingen ook gesynchroniseerd in uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="e04eb-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="e04eb-294">Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="e04eb-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="e04eb-295">Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in micro soft Partner Center en gesynchroniseerd in de Dynamics 365-omgeving:</span><span class="sxs-lookup"><span data-stu-id="e04eb-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="e04eb-296">Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="e04eb-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="e04eb-297">Selecteer **verwijzingen** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="e04eb-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="e04eb-298">Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door te klikken op de optie nieuwe deal.</span><span class="sxs-lookup"><span data-stu-id="e04eb-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="e04eb-299">Meld u aan bij uw Dynamics 365 CRM-omgeving.</span><span class="sxs-lookup"><span data-stu-id="e04eb-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="e04eb-300">Navigeer naar **Open verkoop kansen**.</span><span class="sxs-lookup"><span data-stu-id="e04eb-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="e04eb-301">De verwijzing die is gemaakt in het micro soft Partner Center is nu gesynchroniseerd in Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="e04eb-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="e04eb-302">Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.</span><span class="sxs-lookup"><span data-stu-id="e04eb-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e04eb-303">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="e04eb-303">Next steps</span></span>

- [<span data-ttu-id="e04eb-304">Leads beheren</span><span class="sxs-lookup"><span data-stu-id="e04eb-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="e04eb-305">Collectieve-verkoopkansen beheren</span><span class="sxs-lookup"><span data-stu-id="e04eb-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="e04eb-306">Meer informatie over het platform van micro soft voor energie automatisering?</span><span class="sxs-lookup"><span data-stu-id="e04eb-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="e04eb-307">Partner centrum-webhooks</span><span class="sxs-lookup"><span data-stu-id="e04eb-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)