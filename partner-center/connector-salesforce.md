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
ms.openlocfilehash: 4b3817dafbd05edf0c50b062b52ac4814c767d04
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92528685"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="59c2f-104">Connector voor Sales Force-verkoop-overzicht</span><span class="sxs-lookup"><span data-stu-id="59c2f-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="59c2f-105">Juiste rollen</span><span class="sxs-lookup"><span data-stu-id="59c2f-105">Appropriate roles</span></span>

- <span data-ttu-id="59c2f-106">Beheerder van verwijzingen</span><span class="sxs-lookup"><span data-stu-id="59c2f-106">Referrals admin</span></span>
- <span data-ttu-id="59c2f-107">Systeem beheerder of systeemaanpasser op de CRM</span><span class="sxs-lookup"><span data-stu-id="59c2f-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="59c2f-108">Met connector voor co-sell van partner Center kunnen uw verkopers samen werken met micro soft binnen uw CRM-systemen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="59c2f-109">Ze hoeven niet te worden getraind om gebruik te kunnen maken van het partner centrum voor het beheren van trans acties met co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="59c2f-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="59c2f-110">Met de co-Connect oren kunt u een nieuwe verwijzing naar een mede verkoop maken om contact op te nemen met een micro soft-verkoper, verwijzingen te ontvangen van de micro soft-verkoper, verwijzingen te accepteren/weigeren, afhandelings gegevens te wijzigen, zoals de deal waarde en de sluitings datum.</span><span class="sxs-lookup"><span data-stu-id="59c2f-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="59c2f-111">U kunt ook updates van de micro soft-verkopers ontvangen op deze mede koop-deals.</span><span class="sxs-lookup"><span data-stu-id="59c2f-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="59c2f-112">U kunt al uw referenties gebruiken terwijl u werkt in de CRM van uw keuze in plaats van in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="59c2f-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="59c2f-113">De oplossing is gebaseerd op de micro soft-oplossing voor energie automatisering en maakt gebruik van partner Center-Api's.</span><span class="sxs-lookup"><span data-stu-id="59c2f-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="59c2f-114">Voordat u de vereisten installeert</span><span class="sxs-lookup"><span data-stu-id="59c2f-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="59c2f-115">**Onderwerpen**</span><span class="sxs-lookup"><span data-stu-id="59c2f-115">**Topics**</span></span>   |<span data-ttu-id="59c2f-116">**Details**</span><span class="sxs-lookup"><span data-stu-id="59c2f-116">**Details**</span></span>   |<span data-ttu-id="59c2f-117">**Koppelingen**</span><span class="sxs-lookup"><span data-stu-id="59c2f-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="59c2f-118">Microsoft Partner Network-ID</span><span class="sxs-lookup"><span data-stu-id="59c2f-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="59c2f-119">U hebt een geldige MPN-ID nodig</span><span class="sxs-lookup"><span data-stu-id="59c2f-119">You need a valid MPN ID</span></span>|<span data-ttu-id="59c2f-120">Toevoegen aan [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="59c2f-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="59c2f-121">Klaar voor samen verkopen</span><span class="sxs-lookup"><span data-stu-id="59c2f-121">Co-sell ready</span></span>|<span data-ttu-id="59c2f-122">Uw IP/Services-oplossing moet samen worden verkocht.</span><span class="sxs-lookup"><span data-stu-id="59c2f-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="59c2f-123">Verkopen met micro soft</span><span class="sxs-lookup"><span data-stu-id="59c2f-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="59c2f-124">Partnercentrum-account</span><span class="sxs-lookup"><span data-stu-id="59c2f-124">Partner Center account</span></span>|<span data-ttu-id="59c2f-125">De MPN-ID die is gekoppeld aan de Partner Center-Tenant, moet gelijk zijn aan de MPN-ID die is gekoppeld aan uw oplossing voor co-selling.</span><span class="sxs-lookup"><span data-stu-id="59c2f-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="59c2f-126">Controleer voordat u de connectors implementeert of u de referenties voor samen verkopen in partner centrum Portal kunt zien.</span><span class="sxs-lookup"><span data-stu-id="59c2f-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="59c2f-127">Uw account beheren</span><span class="sxs-lookup"><span data-stu-id="59c2f-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="59c2f-128">Gebruikers rollen voor het partner centrum</span><span class="sxs-lookup"><span data-stu-id="59c2f-128">Partner Center user roles</span></span>|<span data-ttu-id="59c2f-129">De werk nemer die de connectors installeert en gebruikt, moet een referentie beheerder zijn</span><span class="sxs-lookup"><span data-stu-id="59c2f-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="59c2f-130">Beheerdersrollen en -machtigingen toewijzen</span><span class="sxs-lookup"><span data-stu-id="59c2f-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="59c2f-131">Sales Force CRM</span><span class="sxs-lookup"><span data-stu-id="59c2f-131">Salesforce CRM</span></span>|<span data-ttu-id="59c2f-132">De rol van CRM-gebruiker is systeem beheerder of systeemaanpasser</span><span class="sxs-lookup"><span data-stu-id="59c2f-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="59c2f-133">Rollen toewijzen in Sales Force CRM</span><span class="sxs-lookup"><span data-stu-id="59c2f-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="59c2f-134">Stroom account voor energie automatisering</span><span class="sxs-lookup"><span data-stu-id="59c2f-134">Power Automate Flow Account</span></span>|<span data-ttu-id="59c2f-135">Een actief [geautomatiseerd](https://flow.microsoft.com) account voor het beheer van de CRM-systeem beheerder of het systeem.</span><span class="sxs-lookup"><span data-stu-id="59c2f-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="59c2f-136">Deze gebruiker moet zich ten minste één keer aanmelden bij Power voor het [automatiseren](https://flow.microsoft.com) van de installatie.</span><span class="sxs-lookup"><span data-stu-id="59c2f-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="59c2f-137">Installatie van Sales Force-pakket voor aangepaste micro soft-velden</span><span class="sxs-lookup"><span data-stu-id="59c2f-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="59c2f-138">Voor het synchroniseren van de verwijzingen tussen partner centrum en Sales Force CRM, moet de oplossing voor het automatiseren van micro soft specifieke Referral-velden duidelijk identificeren.</span><span class="sxs-lookup"><span data-stu-id="59c2f-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="59c2f-139">Deze afbakening biedt partner verkopers teams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.</span><span class="sxs-lookup"><span data-stu-id="59c2f-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="59c2f-140">Activeer in Sales Force de **notities** en voeg deze toe aan de lijst met aan verkoop kansen gerelateerde.</span><span class="sxs-lookup"><span data-stu-id="59c2f-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="59c2f-141">Verwijzing</span><span class="sxs-lookup"><span data-stu-id="59c2f-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="59c2f-142">Activeer **verkoop kansen teams** door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="59c2f-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="59c2f-143">In Setup gebruikt u het vak **Snelzoeken** om de instellingen van het Opportunity team te vinden.</span><span class="sxs-lookup"><span data-stu-id="59c2f-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="59c2f-144">Definieer de instellingen waar nodig.</span><span class="sxs-lookup"><span data-stu-id="59c2f-144">Define the settings as needed.</span></span>
[<span data-ttu-id="59c2f-145">Verwijzing</span><span class="sxs-lookup"><span data-stu-id="59c2f-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="59c2f-146">Onder Sales Force installeert u aangepaste velden en objecten met behulp van Package Installer hieronder.</span><span class="sxs-lookup"><span data-stu-id="59c2f-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="59c2f-147">Ga [hier](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) om het pakket te installeren in een bedrijf:</span><span class="sxs-lookup"><span data-stu-id="59c2f-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="59c2f-148">Opmerking: als u in een sandbox installeert, moet u het eerste deel van de URL vervangen door http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="59c2f-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="59c2f-149">Voeg in Sales Force micro soft-oplossingen toe aan de lijst met **kansen** die hieraan zijn gerelateerd.</span><span class="sxs-lookup"><span data-stu-id="59c2f-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="59c2f-150">Nadat deze is toegevoegd, klikt u op het **moersleutel** pictogram en werkt u de eigenschappen bij</span><span class="sxs-lookup"><span data-stu-id="59c2f-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="59c2f-151">Best practice: test voordat u live gaat</span><span class="sxs-lookup"><span data-stu-id="59c2f-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="59c2f-152">Voordat u de oplossing voor het automatiseren van energie op de productie omgeving installeert, configureert en bijwerkt, moet u ervoor zorgen dat u de oplossing op een staging CRM-exemplaar test.</span><span class="sxs-lookup"><span data-stu-id="59c2f-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="59c2f-153">Installeer de oplossing voor het automatiseren van micro soft power op een staging-omgeving/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="59c2f-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="59c2f-154">Maak een kopie van de oplossing en voer uw configuratie uit en Automatiseer de stroom aanpassingen in de faserings omgeving.</span><span class="sxs-lookup"><span data-stu-id="59c2f-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="59c2f-155">Test de oplossing op een staging/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="59c2f-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="59c2f-156">Importeer bij geslaagd als een beheerde oplossing naar het productie-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="59c2f-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="59c2f-157">Synchronisatie van partner Center referrals voor Sales Force CRM installeren</span><span class="sxs-lookup"><span data-stu-id="59c2f-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="59c2f-158">Ga naar [Automatische stroom](https://flow.microsoft.com) en selecteer **omgevingen** in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="59c2f-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="59c2f-159">Hiermee worden de beschik bare exemplaren van CRM weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="59c2f-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="59c2f-160">Selecteer het juiste CRM-exemplaar in de vervolg keuzelijst in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="59c2f-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="59c2f-161">Selecteer **oplossingen** op de linkernavigatiebalk.</span><span class="sxs-lookup"><span data-stu-id="59c2f-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="59c2f-162">Klik op de koppeling **Open AppSource** in het bovenste menu.</span><span class="sxs-lookup"><span data-stu-id="59c2f-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource openen":::

5. <span data-ttu-id="59c2f-164">Zoek naar **Partner Center referrals connectors voor Sales Force** in het pop-upvenster.</span><span class="sxs-lookup"><span data-stu-id="59c2f-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="59c2f-166">Klik op de knop **nu downloaden** en vervolgens op **door gaan** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-166">Click the **Get it now** button and then **Continue** .</span></span>

7. <span data-ttu-id="59c2f-167">Hiermee opent u de pagina waar u de Sales Force CRM-omgeving kunt selecteren om de toepassing te installeren.</span><span class="sxs-lookup"><span data-stu-id="59c2f-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="59c2f-168">Ga akkoord met de voor waarden.</span><span class="sxs-lookup"><span data-stu-id="59c2f-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Beschik bare CRMS":::

8. <span data-ttu-id="59c2f-170">Vervolgens gaat u naar de pagina **uw oplossingen beheren** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="59c2f-171">Navigeer naar partner Center referrals met behulp van de pijl knoppen aan de onderkant van de pagina.</span><span class="sxs-lookup"><span data-stu-id="59c2f-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="59c2f-172">**Geplande installatie** moet naast Partner Center referrals-oplossing worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="59c2f-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="59c2f-173">De installatie duurt 10-15 minuten.</span><span class="sxs-lookup"><span data-stu-id="59c2f-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="59c2f-174">Zodra de installatie is voltooid, gaat u terug naar [energie automatisering](https://flow.microsoft.com) en selecteert u **oplossingen** vanuit het navigatie gebied links.</span><span class="sxs-lookup"><span data-stu-id="59c2f-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="59c2f-175">U ziet dat **Partner Center referrals synchronisatie voor Sales Force** beschikbaar is in de lijst met oplossingen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="59c2f-176">Selecteer **Partner Center referrals synchronisatie voor Sales Force** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-176">Select **Partner Center Referrals Synchronization for Salesforce** .</span></span> <span data-ttu-id="59c2f-177">De volgende stroom voor het automatiseren van stromen en entiteiten zijn beschikbaar:</span><span class="sxs-lookup"><span data-stu-id="59c2f-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Sales Force-stromen":::



## <a name="configure-the-solution"></a><span data-ttu-id="59c2f-179">De oplossing configureren</span><span class="sxs-lookup"><span data-stu-id="59c2f-179">Configure the solution</span></span>

1. <span data-ttu-id="59c2f-180">Wanneer u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug naar [Automatische stroom](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="59c2f-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="59c2f-181">Selecteer in de vervolg keuzelijst **omgevingen** in de rechter BOVENHOEK het CRM-exemplaar waarop u de oplossing voor het automatiseren van energie beheer hebt geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="59c2f-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="59c2f-182">U moet verbindingen maken waarmee de drie gebruikers accounts worden gekoppeld:</span><span class="sxs-lookup"><span data-stu-id="59c2f-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="59c2f-183">Partner centrum-gebruiker met referrals beheerders referenties</span><span class="sxs-lookup"><span data-stu-id="59c2f-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="59c2f-184">Partnercentrum-gebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="59c2f-184">Partner Center Events</span></span>
    - <span data-ttu-id="59c2f-185">CRM-beheerder met de stroom voor het automatiseren van stromen in de oplossing.</span><span class="sxs-lookup"><span data-stu-id="59c2f-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="59c2f-186">Selecteer **verbindingen** in de linkernavigatiebalk en selecteer de oplossing Partner Center referrals in de lijst.</span><span class="sxs-lookup"><span data-stu-id="59c2f-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="59c2f-187">Maak een verbinding door te klikken op **een verbinding maken** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-187">Create a connection by clicking **Create a connection** .</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Verbinding maken":::

- <span data-ttu-id="59c2f-189">Zoek naar partner Center referrals (preview) in de zoek balk in de rechter bovenhoek.</span><span class="sxs-lookup"><span data-stu-id="59c2f-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="59c2f-190">Maak een verbinding voor uw partner centrum-gebruiker met de referenties van de beheerder van verwijzingen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="59c2f-191">Maak vervolgens een verbinding met de partner centrum-gebeurtenissen voor uw partner centrum-gebruiker met de referenties van de beheerder.</span><span class="sxs-lookup"><span data-stu-id="59c2f-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="59c2f-192">Maak een verbinding voor Common Data Service (huidige omgeving) voor de gebruiker van de CRM-beheerder.</span><span class="sxs-lookup"><span data-stu-id="59c2f-192">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="59c2f-193">Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:</span><span class="sxs-lookup"><span data-stu-id="59c2f-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Verbindingen observeren":::

### <a name="edit-the-connections"></a><span data-ttu-id="59c2f-195">De verbindingen bewerken</span><span class="sxs-lookup"><span data-stu-id="59c2f-195">Edit the connections</span></span>

1. <span data-ttu-id="59c2f-196">Ga terug naar de pagina oplossingen en selecteer **standaard oplossing** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-196">Return to the Solutions page and select **Default Solution** .</span></span>  <span data-ttu-id="59c2f-197">Selecteer **verbindings verwijzing (preview)** door te klikken op **alle** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-197">Select **Connection Reference (preview)** by clicking **All** .</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Connector bewerking starten":::

2. <span data-ttu-id="59c2f-199">Bewerk elk van de verbindingen één voor één door het pictogram drie punten te selecteren.</span><span class="sxs-lookup"><span data-stu-id="59c2f-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="59c2f-200">Voeg de relevante verbindingen toe.</span><span class="sxs-lookup"><span data-stu-id="59c2f-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Connectors bewerken":::

3. <span data-ttu-id="59c2f-202">Schakel de stromen in de volgende volg orde in:</span><span class="sxs-lookup"><span data-stu-id="59c2f-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="59c2f-203">Inschrijving van partner Center-webhooks (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-204">Een verwijzing naar een gezamenlijk verkoop object maken-Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-205">Partner centrum referentie-updates voor micro soft-verkoop naar Sales Force (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-206">Partner centrum naar Sales Force (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-207">Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-208">Sales Force to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59c2f-209">Sales Force Micro Solutions to Partner Center (Insider preview)</span><span class="sxs-lookup"><span data-stu-id="59c2f-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="59c2f-210">Webhook-Api's gebruiken om te registreren voor bron wijzigings gebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="59c2f-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="59c2f-211">Met de webhook-Api's van partner Center kunt u zich registreren voor bron wijzigings gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="59c2f-212">Deze wijzigings gebeurtenissen worden als HTTP-berichten naar uw URL verzonden.</span><span class="sxs-lookup"><span data-stu-id="59c2f-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="59c2f-213">Als u uw URL wilt registreren, selecteert u stroom voor het automatiseren van de data **Center-webhook-registratie (Insider preview)** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="59c2f-214">Verbindingen toevoegen voor een partner centrum-gebruiker (a.) met referrals beheerders referenties (b.) partner Center-gebeurtenissen zoals hieronder gemarkeerd</span><span class="sxs-lookup"><span data-stu-id="59c2f-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger":::

3. <span data-ttu-id="59c2f-216">Wanneer u deze updates maakt, ziet u</span><span class="sxs-lookup"><span data-stu-id="59c2f-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="59c2f-218">Sla de wijzigingen op en selecteer **inschakelen** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-218">Save your changes and select **Turn on** .</span></span>

   <span data-ttu-id="59c2f-219">Voer de volgende stappen uit om het partner centrum-webhooks in staat te stellen om te Luis teren naar gebeurtenis wijzigingen:</span><span class="sxs-lookup"><span data-stu-id="59c2f-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="59c2f-220">Selecteer **partner centrum naar Sales Force CRM (Insider preview)** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-220">Select **Partner Center to Salesforce CRM (Insider Preview)** .</span></span>

6. <span data-ttu-id="59c2f-221">Selecteer het **bewerkings** pictogram en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-221">Select the **Edit** icon and select **When a HTTP request is received** .</span></span>

7. <span data-ttu-id="59c2f-222">Selecteer het **Kopieer** pictogram om de gegeven HTTP post-URL te kopiëren.</span><span class="sxs-lookup"><span data-stu-id="59c2f-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL kopiëren":::

8. <span data-ttu-id="59c2f-224">Selecteer nu de stroom voor het automatiseren van partner Center-webhooks (Insider preview) en selecteer **uitvoeren** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run** .</span></span>

9. <span data-ttu-id="59c2f-225">Zorg ervoor dat het venster stroom uitvoeren wordt geopend in het rechterdeel venster en klik op **door gaan** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue** .</span></span>

10. <span data-ttu-id="59c2f-226">Voer de volgende details in:</span><span class="sxs-lookup"><span data-stu-id="59c2f-226">Enter the following details:</span></span>

    1. <span data-ttu-id="59c2f-227">**Http-trigger eindpunt** : URL gekopieerd uit eerdere stap</span><span class="sxs-lookup"><span data-stu-id="59c2f-227">**Http Trigger Endpoint** : URL copied from earlier step</span></span>

    2. <span data-ttu-id="59c2f-228">**Te registreren gebeurtenissen** : ' verwijzing-gemaakt ' en ' referentie-bijgewerkt '</span><span class="sxs-lookup"><span data-stu-id="59c2f-228">**Events to Register** : "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="59c2f-229">**Bestaande trigger eindpunten overschrijven indien aanwezig** : Ja (Hiermee worden alle bestaande eind punten overschreven.)</span><span class="sxs-lookup"><span data-stu-id="59c2f-229">**Overwrite existing trigger endpoints if present** : Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="59c2f-230">Selecteer **uitvoeren** en selecteer vervolgens **gereed.**</span><span class="sxs-lookup"><span data-stu-id="59c2f-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="59c2f-231">De webhook kan nu Luis teren om gebeurtenissen te maken en bij te werken.</span><span class="sxs-lookup"><span data-stu-id="59c2f-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="59c2f-232">Synchronisatie stappen aanpassen</span><span class="sxs-lookup"><span data-stu-id="59c2f-232">Customize synchronization steps</span></span>

<span data-ttu-id="59c2f-233">Als er verwijzingen naar links worden gesynchroniseerd tussen partner centrum en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op de Partner Center-PC hier vermeld.</span><span class="sxs-lookup"><span data-stu-id="59c2f-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="59c2f-234">Vaak worden de CRM-systemen zeer aangepast.</span><span class="sxs-lookup"><span data-stu-id="59c2f-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="59c2f-235">U kunt de stroom voor het automatiseren van stromen aanpassen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="59c2f-236">Volg de instructies in de hand leiding voor de veld toewijzing en breng zo nodig de juiste wijzigingen aan in de stappen van de stroom automatische stromen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="59c2f-237">Micro soft partner Centers naar CRM-toewijzingen worden gegeven, maar op basis van uw CRM-omgeving kunt u ervoor kiezen om de velden verder aan te passen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="59c2f-238">Meerdere stappen van elk van de energiebeheer stromen kunnen worden aangepast op basis van uw behoeften.</span><span class="sxs-lookup"><span data-stu-id="59c2f-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="59c2f-239">Hier volgen enkele voor beelden van beschik bare aanpassingen:</span><span class="sxs-lookup"><span data-stu-id="59c2f-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="59c2f-240">Als u de velden voor de gebeurtenissen maken of bijwerken in het partner centrum wilt aanpassen aan CRM Referral-synchronisatie:</span><span class="sxs-lookup"><span data-stu-id="59c2f-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="59c2f-241">Selecteer partner centrum naar Sales Force CRM (Insider preview).</span><span class="sxs-lookup"><span data-stu-id="59c2f-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="59c2f-242">Selecteer **bewerken** om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="59c2f-243">Selecteer **(bereik) de lead of de opportuniteit synchroniseren** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-243">Select **(Scope) Synchronize the lead or opportunity** .</span></span>

2. <span data-ttu-id="59c2f-244">Als u CRM-veld toewijzingen voor het maken van gebeurtenissen wilt aanpassen, selecteert u **of het een nieuwe gedeelde verkoop kans is en klikt u vervolgens** op.</span><span class="sxs-lookup"><span data-stu-id="59c2f-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then** .</span></span> <span data-ttu-id="59c2f-245">Selecteer de substap **Indien ja** en vouw vervolgens **een nieuwe opportuniteit maken in het CRM** uit.</span><span class="sxs-lookup"><span data-stu-id="59c2f-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM** .</span></span> <span data-ttu-id="59c2f-246">U kunt de toewijzingen in deze sectie bewerken met de gids voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="59c2f-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="59c2f-247">Als u CRM-veld toewijzingen voor update gebeurtenissen wilt aanpassen, klikt u op de stap (bereik) synchroniseren van de lead of de verkoop kans.</span><span class="sxs-lookup"><span data-stu-id="59c2f-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="59c2f-248">Selecteer **deze optie als het een update is voor een verkoop kans en klik vervolgens** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-248">Select **If it’s an update to an opportunity, then** .</span></span> <span data-ttu-id="59c2f-249">Selecteer de substap **Indien ja** en vouw vervolgens uit **als het verschil tussen de objecten verkoop kansen in partner centrum en CRM** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then** .</span></span>  

   3. <span data-ttu-id="59c2f-250">Selecteren **als ja** , gevolgd door **bestaande verkoop kans bijwerken**</span><span class="sxs-lookup"><span data-stu-id="59c2f-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="59c2f-251">De velden voor CRM naar PC Referral Synchronization voor update gebeurtenissen aanpassen:</span><span class="sxs-lookup"><span data-stu-id="59c2f-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="59c2f-252">Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="59c2f-253">Selecteer **(bereik) de opportuniteit synchroniseren** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-253">Select **(Scope) Synchronize the opportunity** .</span></span>

   3. <span data-ttu-id="59c2f-254">Voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding veld Toewijzingen) voor update gebeurtenissen, selecteert u **of er verschil is tussen de objecten leads in Partner Center en CRM** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then** .</span></span>

   4. <span data-ttu-id="59c2f-255">Selecteer de substap **als ja** en vouw vervolgens de stap **een referral met verkoopkansgegevens bijwerken** uit.</span><span class="sxs-lookup"><span data-stu-id="59c2f-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data** .</span></span>

   <span data-ttu-id="59c2f-256">U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="59c2f-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="59c2f-257">De velden voor CRM naar PC Referral-synchronisatie aanpassen voor het maken van gebeurtenissen?</span><span class="sxs-lookup"><span data-stu-id="59c2f-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="59c2f-258">Selecteer **bewerken**  om de stroom voor het automatiseren van de stroom te bewerken/aan te passen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="59c2f-259">Selecteer **(bereik) het synchroniseren van verwijzingen.**</span><span class="sxs-lookup"><span data-stu-id="59c2f-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="59c2f-260">Selecteer **micro soft Referral maken** voor het aanpassen van CRM-veld toewijzingen (op basis van de hand leiding voor veld Toewijzingen) voor het maken van gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="59c2f-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral** .</span></span>

<span data-ttu-id="59c2f-261">U kunt de toewijzingen in deze sectie bewerken op basis van de hand leiding voor veld toewijzing.</span><span class="sxs-lookup"><span data-stu-id="59c2f-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="59c2f-262">End-to-end-synchronisatie van Referral-verkoop referenties</span><span class="sxs-lookup"><span data-stu-id="59c2f-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="59c2f-263">Zodra u de oplossing voor het automatiseren van de stroom hebt geïnstalleerd, geconfigureerd en aangepast, kunt u de synchronisatie van verwijzingen naar verkoop kansen testen tussen Sales Force CRM en partner Center.</span><span class="sxs-lookup"><span data-stu-id="59c2f-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="59c2f-264">Vereisten</span><span class="sxs-lookup"><span data-stu-id="59c2f-264">Pre-requisites</span></span>

<span data-ttu-id="59c2f-265">Voor de synchronisatie van de verwijzingen tussen partner centrum en Sales Force CRM moet de oplossing voor het automatiseren van micro soft-specifieke Referral-velden duidelijk worden afgebakend.</span><span class="sxs-lookup"><span data-stu-id="59c2f-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="59c2f-266">Met deze identificatie kunnen verkopers teams bepalen welke verwijzingen ze willen delen met micro soft voor co-selling.</span><span class="sxs-lookup"><span data-stu-id="59c2f-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="59c2f-267">Een set aangepaste velden is beschikbaar als onderdeel van partner Center referrals synchronisatie voor de Sales Force CRM **Solution-** entiteit.</span><span class="sxs-lookup"><span data-stu-id="59c2f-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="59c2f-268">Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden voor **verkoop kansen** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="59c2f-269">De volgende aangepaste velden moeten deel uitmaken van de sectie CRM:</span><span class="sxs-lookup"><span data-stu-id="59c2f-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="59c2f-270">**Synchroniseren met partner centrum** : of u de mogelijkheid wilt synchroniseren met micro soft Partner Center</span><span class="sxs-lookup"><span data-stu-id="59c2f-270">**Sync with Partner Center** : Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="59c2f-271">**Verwijzings-id** : een veld met alleen-lezen-id voor micro soft Partner Center Referral</span><span class="sxs-lookup"><span data-stu-id="59c2f-271">**Referral Identifier** : A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="59c2f-272">**Verwijzings koppeling** : een alleen-lezen koppeling naar de verwijzing in het micro soft partner centrum</span><span class="sxs-lookup"><span data-stu-id="59c2f-272">**Referral Link** : A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="59c2f-273">**Hoe kan ik micro soft helpen** : Help vereist van micro soft voor de verwijzing</span><span class="sxs-lookup"><span data-stu-id="59c2f-273">**How can Microsoft help** : Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="59c2f-274">**Producten** : lijst met producten die zijn gekoppeld aan deze verkoop kans</span><span class="sxs-lookup"><span data-stu-id="59c2f-274">**Products** : List of products associated with this opportunity</span></span>

- <span data-ttu-id="59c2f-275">**Controle** : een audit trail met alleen-lezen voor synchronisatie met partner Center-verwijzingen</span><span class="sxs-lookup"><span data-stu-id="59c2f-275">**Audit** : A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="59c2f-276">DENKBAAR</span><span class="sxs-lookup"><span data-stu-id="59c2f-276">SCENARIOS:</span></span>

1. <span data-ttu-id="59c2f-277">Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en gesynchroniseerd in partner centrum:</span><span class="sxs-lookup"><span data-stu-id="59c2f-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="59c2f-278">Meld u aan bij uw Sales Force CRM-omgeving met een zicht baarheid in het gedeelte **verkoop kansen** van de CRM.</span><span class="sxs-lookup"><span data-stu-id="59c2f-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="59c2f-279">Zorg ervoor dat de volgende sectie aanwezig is wanneer u een nieuwe kans maakt in de Sales Force CRM-omgeving</span><span class="sxs-lookup"><span data-stu-id="59c2f-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Sales Force-omgeving":::

   3. <span data-ttu-id="59c2f-281">Als u deze mogelijkheid wilt synchroniseren met micro soft Partner Center, moet u ervoor zorgen dat u de volgende velden in de kaart weergave instelt:</span><span class="sxs-lookup"><span data-stu-id="59c2f-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="59c2f-282">"Synchroniseren met partner centrum": Ja</span><span class="sxs-lookup"><span data-stu-id="59c2f-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="59c2f-283">"How can micro soft Help?": Selecteer een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="59c2f-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="59c2f-284">Producten: oplossings-Id's van het product</span><span class="sxs-lookup"><span data-stu-id="59c2f-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="59c2f-285">Wanneer u de optie  **synchronisatie van verkoop kansen met partner Center** hebt ingesteld op **Ja** , wacht u 10 minuten en meldt u zich aan bij uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="59c2f-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes** , wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="59c2f-286">Uw verwijzingen worden gesynchroniseerd met Sales Force CRM.</span><span class="sxs-lookup"><span data-stu-id="59c2f-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="59c2f-287">Wanneer de optie ' synchroniseren met partner centrum ' is ingesteld op ' ja ' en u de opportuniteit bijwerkt in Sales Force CRM, worden de wijzigingen gesynchroniseerd met uw partner centrum-account.</span><span class="sxs-lookup"><span data-stu-id="59c2f-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="59c2f-288">Verkoop kansen die zijn gesynchroniseerd met partner Center worden aangeduid met ✔ pictogram in Sales Force CRM.</span><span class="sxs-lookup"><span data-stu-id="59c2f-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="59c2f-289">Verwijzings synchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in micro soft Partner Center en gesynchroniseerd in de Sales Force CRM-omgeving:</span><span class="sxs-lookup"><span data-stu-id="59c2f-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="59c2f-290">Meld u aan bij uw partner Center- [dash board](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="59c2f-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="59c2f-291">Selecteer **verwijzingen** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="59c2f-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="59c2f-292">Maak een nieuwe verwijzing naar een mede verkoop van het partner centrum door te klikken op de optie nieuwe deal.</span><span class="sxs-lookup"><span data-stu-id="59c2f-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="59c2f-293">Meld u aan bij uw Sales Force CRM-omgeving.</span><span class="sxs-lookup"><span data-stu-id="59c2f-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="59c2f-294">Navigeer naar **Open verkoop kansen** .</span><span class="sxs-lookup"><span data-stu-id="59c2f-294">Navigate to **Open Opportunities** .</span></span> <span data-ttu-id="59c2f-295">De verwijzing die is gemaakt in het micro soft Partner Center is nu gesynchroniseerd in Sales Force CRM.</span><span class="sxs-lookup"><span data-stu-id="59c2f-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Scherm Sales Force-verkoop kans":::

    6. <span data-ttu-id="59c2f-297">Wanneer u een gesynchroniseerde verwijzing selecteert, worden de kaart weergave Details ingevuld.</span><span class="sxs-lookup"><span data-stu-id="59c2f-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="59c2f-298">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="59c2f-298">Next steps</span></span>

- [<span data-ttu-id="59c2f-299">Leads beheren</span><span class="sxs-lookup"><span data-stu-id="59c2f-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="59c2f-300">Collectieve-verkoopkansen beheren</span><span class="sxs-lookup"><span data-stu-id="59c2f-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="59c2f-301">Partner centrum-webhooks</span><span class="sxs-lookup"><span data-stu-id="59c2f-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)