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
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="9c553-104">Connector voor co-verkoop voor Salesforce CRM - overzicht</span><span class="sxs-lookup"><span data-stu-id="9c553-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="9c553-105">**Juiste rollen:** Beheerdersrollen voor verwijzingen | Systeembeheerder of systeem aanpassen op het CRM</span><span class="sxs-lookup"><span data-stu-id="9c553-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="9c553-106">Partner Center connector voor co-verkoop kunnen uw verkopers samen met Microsoft verkopen vanuit uw CRM-systemen.</span><span class="sxs-lookup"><span data-stu-id="9c553-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="9c553-107">Ze moeten niet worden getraind voor het gebruik van Partner Center om deals voor co-verkoop te beheren.</span><span class="sxs-lookup"><span data-stu-id="9c553-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="9c553-108">Met behulp van de connectors voor co-verkoop kunt u een nieuwe verwijzing voor co-verkoop maken om een Microsoft-verkoper te betrekken, verwijzingen van de Microsoft-verkoper te ontvangen, verwijzingen te accepteren/weigeren, dealgegevens zoals dealwaarde en einddatum te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="9c553-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="9c553-109">U kunt ook updates ontvangen van de Microsoft-verkopers over deze deals voor co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="9c553-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="9c553-110">U kunt al uw verwijzingen laten werken binnen het CRM van uw keuze in plaats van in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9c553-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="9c553-111">De oplossing is gebaseerd op Microsoft Power Automate Solution en maakt gebruik van Partner Center API's.</span><span class="sxs-lookup"><span data-stu-id="9c553-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="9c553-112">Voordat u installeert - vereisten</span><span class="sxs-lookup"><span data-stu-id="9c553-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="9c553-113">**Onderwerpen**</span><span class="sxs-lookup"><span data-stu-id="9c553-113">**Topics**</span></span>   |<span data-ttu-id="9c553-114">**Details**</span><span class="sxs-lookup"><span data-stu-id="9c553-114">**Details**</span></span>   |<span data-ttu-id="9c553-115">**Koppelingen**</span><span class="sxs-lookup"><span data-stu-id="9c553-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="9c553-116">Microsoft Partner Network-id</span><span class="sxs-lookup"><span data-stu-id="9c553-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="9c553-117">U hebt een geldige MPN-id nodig</span><span class="sxs-lookup"><span data-stu-id="9c553-117">You need a valid MPN ID</span></span>|<span data-ttu-id="9c553-118">Lid worden van [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="9c553-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="9c553-119">Gereed voor co-verkoop</span><span class="sxs-lookup"><span data-stu-id="9c553-119">Co-sell ready</span></span>|<span data-ttu-id="9c553-120">Uw IP/Services-oplossing moet klaar zijn voor co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="9c553-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="9c553-121">Verkopen met Microsoft</span><span class="sxs-lookup"><span data-stu-id="9c553-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="9c553-122">Partnercentrum-account</span><span class="sxs-lookup"><span data-stu-id="9c553-122">Partner Center account</span></span>|<span data-ttu-id="9c553-123">De MPN-id die is gekoppeld aan Partner Center tenant, moet gelijk zijn aan de MPN-id die is gekoppeld aan uw oplossing voor co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="9c553-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="9c553-124">Controleer of u uw verwijzingen voor co-verkoop kunt zien in Partner Center portal voordat u de connectors implementeert.</span><span class="sxs-lookup"><span data-stu-id="9c553-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="9c553-125">Uw account beheren</span><span class="sxs-lookup"><span data-stu-id="9c553-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9c553-126">Partner Center gebruikersrollen</span><span class="sxs-lookup"><span data-stu-id="9c553-126">Partner Center user roles</span></span>|<span data-ttu-id="9c553-127">De werknemer die de connectors gaat installeren en gebruiken, moet een verwijzingsbeheerder zijn</span><span class="sxs-lookup"><span data-stu-id="9c553-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="9c553-128">Beheerdersrollen en -machtigingen toewijzen</span><span class="sxs-lookup"><span data-stu-id="9c553-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="9c553-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9c553-129">Salesforce CRM</span></span>|<span data-ttu-id="9c553-130">De CRM-gebruikersrol is Systeembeheerder of Systeem aanwijzer</span><span class="sxs-lookup"><span data-stu-id="9c553-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="9c553-131">Rollen toewijzen in Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="9c553-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="9c553-132">Power Automate Flow-account</span><span class="sxs-lookup"><span data-stu-id="9c553-132">Power Automate Flow Account</span></span>|<span data-ttu-id="9c553-133">Een actief [Power Automate](https://flow.microsoft.com) account voor de crm-systeembeheerder of systeem aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9c553-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="9c553-134">Deze gebruiker moet zich ten [minste Power Automate](https://flow.microsoft.com) vóór de installatie aanmelden.</span><span class="sxs-lookup"><span data-stu-id="9c553-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="9c553-135">Installatie van Salesforce-pakket voor aangepaste Microsoft-velden</span><span class="sxs-lookup"><span data-stu-id="9c553-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="9c553-136">Als u de verwijzingen wilt synchroniseren tussen Partner Center salesforce en Salesforce CRM, Power Automate oplossing duidelijk Microsoft-specifieke verwijzingsvelden identificeren.</span><span class="sxs-lookup"><span data-stu-id="9c553-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="9c553-137">Deze afbakening biedt verkopers van partners de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="9c553-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="9c553-138">Activeer notities in Salesforce **en** voeg deze toe aan de lijst met verkoopkansen.</span><span class="sxs-lookup"><span data-stu-id="9c553-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="9c553-139">Verwijzing</span><span class="sxs-lookup"><span data-stu-id="9c553-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="9c553-140">Activeer **opportunity-teams** door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="9c553-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="9c553-141">Gebruik in Setup het vak **Snel zoeken om** de instellingen van het opportunity team te vinden.</span><span class="sxs-lookup"><span data-stu-id="9c553-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="9c553-142">Definieer de instellingen naar behoefte.</span><span class="sxs-lookup"><span data-stu-id="9c553-142">Define the settings as needed.</span></span>
[<span data-ttu-id="9c553-143">Verwijzing</span><span class="sxs-lookup"><span data-stu-id="9c553-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="9c553-144">Installeer in Salesforce aangepaste velden en objecten met behulp van het [installatieprogramma voor pakketten.](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)</span><span class="sxs-lookup"><span data-stu-id="9c553-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="9c553-145">Gebruik dit om het pakket in elk bedrijf te installeren.</span><span class="sxs-lookup"><span data-stu-id="9c553-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="9c553-146">Als u in een sandbox installeert, moet u het eerste gedeelte van de URL vervangen door http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="9c553-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="9c553-147">Voeg in Salesforce Microsoft-oplossingen toe aan de lijst met betrekking **tot** kansen.</span><span class="sxs-lookup"><span data-stu-id="9c553-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="9c553-148">Nadat u de sleutelsleutel hebt **toegevoegd, selecteert u het** pictogram en de eigenschappen bijwerken</span><span class="sxs-lookup"><span data-stu-id="9c553-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="9c553-149">Best Practice: Testen voordat u live gaat</span><span class="sxs-lookup"><span data-stu-id="9c553-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="9c553-150">Voordat u de oplossing installeert, configureert en Power Automate in de productieomgeving, moet u de oplossing testen op een faserings-CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="9c553-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="9c553-151">Installeer Microsoft Power Automate-oplossing in een faseringsomgeving/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="9c553-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="9c553-152">Maak een kopie van de oplossing en voer uw configuratie en Power Automate stroomaanpassingen uit in de faseringsomgeving.</span><span class="sxs-lookup"><span data-stu-id="9c553-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="9c553-153">Test de oplossing op een faserings-/CRM-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="9c553-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="9c553-154">Importeer bij succes als een beheerde oplossing naar het productie-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="9c553-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="9c553-155">Synchronisatie Partner Center verwijzingen voor Salesforce CRM installeren</span><span class="sxs-lookup"><span data-stu-id="9c553-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="9c553-156">Ga naar [Power Automate](https://flow.microsoft.com) en selecteer **Omgevingen** in de rechterbovenhoek.</span><span class="sxs-lookup"><span data-stu-id="9c553-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="9c553-157">Hier ziet u de beschikbare CRM-exemplaren.</span><span class="sxs-lookup"><span data-stu-id="9c553-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="9c553-158">Selecteer het juiste CRM-exemplaar in de vervolgkeuzehoek in de rechterbovenhoek.</span><span class="sxs-lookup"><span data-stu-id="9c553-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="9c553-159">Selecteer **Oplossingen** in de linkernavigatiebalk.</span><span class="sxs-lookup"><span data-stu-id="9c553-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="9c553-160">Selecteer de **koppeling AppSource** openen in het bovenste menu.</span><span class="sxs-lookup"><span data-stu-id="9c553-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource.":::

5. <span data-ttu-id="9c553-162">Zoek in **Partner Center naar verwijzingenconnectoren voor Salesforce** in het pop-upscherm.</span><span class="sxs-lookup"><span data-stu-id="9c553-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="9c553-164">Selecteer de **knop Nu krijgen** en vervolgens **Doorgaan.**</span><span class="sxs-lookup"><span data-stu-id="9c553-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="9c553-165">Hiermee opent u de pagina waar u de Salesforce CRM-omgeving kunt selecteren om de toepassing te installeren.</span><span class="sxs-lookup"><span data-stu-id="9c553-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="9c553-166">Ga akkoord met de voorwaarden.</span><span class="sxs-lookup"><span data-stu-id="9c553-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="Beschikbare CRM's.":::

8. <span data-ttu-id="9c553-168">U wordt vervolgens omgeleid naar de **pagina Uw oplossingen** beheren.</span><span class="sxs-lookup"><span data-stu-id="9c553-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="9c553-169">Navigeer naar Partner Center met behulp van de pijlknoppen onderaan de pagina.</span><span class="sxs-lookup"><span data-stu-id="9c553-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="9c553-170">**De geplande installatie** wordt weergegeven naast Partner Center oplossing Verwijzingen.</span><span class="sxs-lookup"><span data-stu-id="9c553-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="9c553-171">De installatie duurt 10-15 minuten.</span><span class="sxs-lookup"><span data-stu-id="9c553-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="9c553-172">Zodra de installatie is voltooid, gaat u terug [naar Power Automate](https://flow.microsoft.com) en selecteert **u Oplossingen** in het navigatiegedeelte aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="9c553-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="9c553-173">U ziet **Partner Center verwijzingssynchronisatie** voor Salesforce beschikbaar is in de lijst oplossingen.</span><span class="sxs-lookup"><span data-stu-id="9c553-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="9c553-174">Selecteer **Partner Center Verwijzingssynchronisatie voor Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="9c553-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="9c553-175">De volgende Power Automate en entiteiten zijn beschikbaar:</span><span class="sxs-lookup"><span data-stu-id="9c553-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce-stromen.":::



## <a name="configure-the-solution"></a><span data-ttu-id="9c553-177">De oplossing configureren</span><span class="sxs-lookup"><span data-stu-id="9c553-177">Configure the solution</span></span>

1. <span data-ttu-id="9c553-178">Nadat u de oplossing in uw CRM-exemplaar hebt geïnstalleerd, gaat u terug [naar Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="9c553-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="9c553-179">Selecteer in **de** vervolgkeuzehoek Omgevingen in de rechterbovenhoek het CRM-exemplaar waarin u de oplossing Power Automate geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="9c553-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="9c553-180">U moet verbindingen maken die de drie gebruikersaccounts koppelen:</span><span class="sxs-lookup"><span data-stu-id="9c553-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="9c553-181">Partner Center gebruiker met beheerdersreferenties voor verwijzingen</span><span class="sxs-lookup"><span data-stu-id="9c553-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="9c553-182">Partnercentrum-gebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="9c553-182">Partner Center Events</span></span>
    - <span data-ttu-id="9c553-183">CRM-beheerder met de Power Automate stromen in de oplossing.</span><span class="sxs-lookup"><span data-stu-id="9c553-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="9c553-184">Selecteer **Verbindingen in** de linkernavigatiebalk en selecteer de oplossing Partner Center verwijzingen in de lijst.</span><span class="sxs-lookup"><span data-stu-id="9c553-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="9c553-185">Maak een verbinding door op Een verbinding **maken te klikken.**</span><span class="sxs-lookup"><span data-stu-id="9c553-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Verbinding maken.":::

- <span data-ttu-id="9c553-187">Zoek naar Partner Center (preview) in de zoekbalk in de rechterbovenhoek.</span><span class="sxs-lookup"><span data-stu-id="9c553-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="9c553-188">Maak een verbinding voor uw Partner Center met de referentiesrol Van verwijzingsbeheerder.</span><span class="sxs-lookup"><span data-stu-id="9c553-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="9c553-189">Maak vervolgens een verbinding Partner Center gebeurtenissen voor uw Partner Center met de referenties van verwijzingenbeheerder.</span><span class="sxs-lookup"><span data-stu-id="9c553-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="9c553-190">Maak een verbinding voor Salesforce voor de CRM-beheerder.</span><span class="sxs-lookup"><span data-stu-id="9c553-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="9c553-191">Zodra u alle verbindingen hebt toegevoegd, ziet u de volgende verbindingen in uw omgeving:</span><span class="sxs-lookup"><span data-stu-id="9c553-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Bekijk de verbindingen.":::

### <a name="edit-the-connections"></a><span data-ttu-id="9c553-193">De verbindingen bewerken</span><span class="sxs-lookup"><span data-stu-id="9c553-193">Edit the connections</span></span>

1. <span data-ttu-id="9c553-194">Ga terug naar de pagina Oplossingen en selecteer **Standaardoplossing.**</span><span class="sxs-lookup"><span data-stu-id="9c553-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="9c553-195">Selecteer **Verbindingsverwijzing (preview) door** op Alle **te klikken.**</span><span class="sxs-lookup"><span data-stu-id="9c553-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Begin met het bewerken van de connector.":::

2. <span data-ttu-id="9c553-197">Bewerk elk van de verbindingen afzonderlijk door het pictogram met drie punten te selecteren.</span><span class="sxs-lookup"><span data-stu-id="9c553-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="9c553-198">Voeg de relevante verbindingen toe.</span><span class="sxs-lookup"><span data-stu-id="9c553-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Connectors bewerken.":::

3. <span data-ttu-id="9c553-200">Schakel de stromen in de volgende volgorde in:</span><span class="sxs-lookup"><span data-stu-id="9c553-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="9c553-201">Partner Center webhookregistratie (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="9c553-202">Verwijzing voor co-verkoop maken - Salesforce naar Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c553-203">Partner Center Microsoft Co-sell Verwijzingsupdates voor Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="9c553-204">Partner Center naar Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="9c553-205">Salesforce naar Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c553-206">Salesforce Opportunity to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="9c553-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="9c553-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="9c553-208">Webhook-API's gebruiken om te registreren voor resourcewijzigingsgebeurtenissen</span><span class="sxs-lookup"><span data-stu-id="9c553-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="9c553-209">Met Partner Center webhook-API's kunt u zich registreren voor gebeurtenissen voor resourcewijziging.</span><span class="sxs-lookup"><span data-stu-id="9c553-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="9c553-210">Deze wijzigingsgebeurtenissen worden als HTTP-berichten naar uw URL verzonden.</span><span class="sxs-lookup"><span data-stu-id="9c553-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="9c553-211">Als u uw URL wilt registreren, selecteert Partner Center de stroom **Webhook-registratie (Insider Preview)** Power Automate registreren.</span><span class="sxs-lookup"><span data-stu-id="9c553-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="9c553-212">Voeg verbindingen toe voor (a.) Partner Center gebruiker met beheerdersreferenties (b.) voor verwijzingen Partner Center Gebeurtenissen zoals hieronder is gemarkeerd</span><span class="sxs-lookup"><span data-stu-id="9c553-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Trigger.":::

3. <span data-ttu-id="9c553-214">Wanneer u deze updates aan het maken bent, ziet u</span><span class="sxs-lookup"><span data-stu-id="9c553-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="9c553-216">Sla uw wijzigingen op en selecteer **In- of uit.**</span><span class="sxs-lookup"><span data-stu-id="9c553-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="9c553-217">Voer de Partner Center uit om webhooks te laten luisteren naar gebeurteniswijzigingen:</span><span class="sxs-lookup"><span data-stu-id="9c553-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="9c553-218">Selecteer **Partner Center Salesforce CRM (Insider Preview)**.</span><span class="sxs-lookup"><span data-stu-id="9c553-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="9c553-219">Selecteer het **pictogram** Bewerken en selecteer **Wanneer een HTTP-aanvraag wordt ontvangen.**</span><span class="sxs-lookup"><span data-stu-id="9c553-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="9c553-220">Selecteer het **pictogram Kopiëren** om de opgegeven HTTP POST-URL te kopiëren.</span><span class="sxs-lookup"><span data-stu-id="9c553-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Kopieer de URL.":::

8. <span data-ttu-id="9c553-222">Selecteer nu de stroom Partner Center webhookregistratie (Insider Preview) Power Automate selecteer **Uitvoeren.**</span><span class="sxs-lookup"><span data-stu-id="9c553-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="9c553-223">Zorg ervoor dat het venster Stroom uitvoeren wordt geopend in het rechterdeelvenster en selecteer **Doorgaan.**</span><span class="sxs-lookup"><span data-stu-id="9c553-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="9c553-224">Voer de volgende details in:</span><span class="sxs-lookup"><span data-stu-id="9c553-224">Enter the following details:</span></span>

    1. <span data-ttu-id="9c553-225">**Http Trigger-eindpunt:** URL die u uit een eerdere stap hebt gekopieerd</span><span class="sxs-lookup"><span data-stu-id="9c553-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="9c553-226">**Gebeurtenissen die moeten worden** geregistreerd: 'verwijzing gemaakt' en 'verwijzing bijgewerkt'</span><span class="sxs-lookup"><span data-stu-id="9c553-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="9c553-227">**Overschrijf bestaande trigger-eindpunten indien aanwezig:** Ja (hiermee worden alle bestaande eindpunten overschreven.)</span><span class="sxs-lookup"><span data-stu-id="9c553-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="9c553-228">Selecteer **Uitvoeren** en selecteer vervolgens **Done.**</span><span class="sxs-lookup"><span data-stu-id="9c553-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="9c553-229">De webhook kan nu luisteren naar het maken en bijwerken van gebeurtenissen.</span><span class="sxs-lookup"><span data-stu-id="9c553-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="9c553-230">Synchronisatiestappen aanpassen</span><span class="sxs-lookup"><span data-stu-id="9c553-230">Customize synchronization steps</span></span>

<span data-ttu-id="9c553-231">Wanneer verwijzingen voor co-verkoop worden gesynchroniseerd tussen Partner Center en uw CRM-systeem, worden de velden die zijn gesynchroniseerd op Partner Center pc hier vermeld.</span><span class="sxs-lookup"><span data-stu-id="9c553-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="9c553-232">CRM-systemen zijn vaak zeer aangepast.</span><span class="sxs-lookup"><span data-stu-id="9c553-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="9c553-233">U kunt de Power Automate aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9c553-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="9c553-234">Volg de handleiding voor veldtoewijzing en indien nodig de juiste wijzigingen aan te brengen in de stappen van de Power Automate stromen.</span><span class="sxs-lookup"><span data-stu-id="9c553-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="9c553-235">Microsoft Partner Centers naar CRM-toewijzingen worden aangeboden, maar op basis van uw CRM-omgeving kunt u ervoor kiezen om de velden verder aan te passen.</span><span class="sxs-lookup"><span data-stu-id="9c553-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="9c553-236">Meerdere stappen van elk van de Power Automate stromen kunnen worden aangepast op basis van uw behoeften.</span><span class="sxs-lookup"><span data-stu-id="9c553-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="9c553-237">Hier volgen enkele voorbeelden van beschikbare aanpassingen:</span><span class="sxs-lookup"><span data-stu-id="9c553-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="9c553-238">De velden voor het maken of bijwerken van gebeurtenissen in de Partner Center crm-verwijzingssynchronisatie aanpassen:</span><span class="sxs-lookup"><span data-stu-id="9c553-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="9c553-239">Selecteer Partner Center Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="9c553-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="9c553-240">Selecteer **Bewerken om** de stroom van de Power Automate bewerken/aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9c553-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="9c553-241">Selecteer **(Bereik) Synchroniseer de lead of kans**.</span><span class="sxs-lookup"><span data-stu-id="9c553-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="9c553-242">Als u CRM-veldtoewijzingen voor het maken van gebeurtenissen wilt aanpassen, selecteert u Als het de nieuwe **gedeelde kans is, selecteert u vervolgens**.</span><span class="sxs-lookup"><span data-stu-id="9c553-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="9c553-243">Selecteer de substap zo **ja** en vouw vervolgens Een nieuwe kans maken **in crm uit.**</span><span class="sxs-lookup"><span data-stu-id="9c553-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="9c553-244">U kunt de toewijzingen in deze sectie bewerken met behulp van de Handleiding voor veldtoewijzing.</span><span class="sxs-lookup"><span data-stu-id="9c553-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="9c553-245">Als u CRM-veldtoewijzingen voor updategebeurtenissen wilt aanpassen, selecteert u de stap '(Bereik) De lead of kans synchroniseren'.</span><span class="sxs-lookup"><span data-stu-id="9c553-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="9c553-246">Selecteer **Als het een update van een kans is, dan**.</span><span class="sxs-lookup"><span data-stu-id="9c553-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="9c553-247">Selecteer de substap **zo ja** en vouw vervolgens If difference uit tussen de **opportunity-objecten in Partner Center CRM en vervolgens**.</span><span class="sxs-lookup"><span data-stu-id="9c553-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="9c553-248">Selecteer **Indien ja gevolgd** door Bestaande kans **bijwerken**</span><span class="sxs-lookup"><span data-stu-id="9c553-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="9c553-249">De velden voor VERWIJZINGssynchronisatie van CRM naar pc aanpassen voor updategebeurtenissen:</span><span class="sxs-lookup"><span data-stu-id="9c553-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="9c553-250">Selecteer **Bewerken om**  de stroom van de Power Automate bewerken/aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9c553-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9c553-251">Selecteer **(Bereik) Synchroniseer de kans**.</span><span class="sxs-lookup"><span data-stu-id="9c553-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="9c553-252">Voor het aanpassen van CRM-veldtoewijzingen (op basis van de handleiding voor veldtoewijzingen) voor updategebeurtenissen selecteert u Als er verschil is tussen de **leadobjecten in Partner Center en CRM, selecteert u vervolgens**.</span><span class="sxs-lookup"><span data-stu-id="9c553-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="9c553-253">Selecteer de substap zo **ja** en vouw vervolgens de stap **Een verwijzing bijwerken met opportunity data uit.**</span><span class="sxs-lookup"><span data-stu-id="9c553-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="9c553-254">U kunt de toewijzingen in deze sectie bewerken op basis van de Handleiding voor veldtoewijzing.</span><span class="sxs-lookup"><span data-stu-id="9c553-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="9c553-255">Wilt u de velden voor verwijzingssynchronisatie van CRM naar pc's aanpassen voor het maken van gebeurtenissen?</span><span class="sxs-lookup"><span data-stu-id="9c553-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="9c553-256">Selecteer **Bewerken om**  de stroom van de Power Automate bewerken/aanpassen.</span><span class="sxs-lookup"><span data-stu-id="9c553-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="9c553-257">Selecteer **(Bereik) Verwijzingen synchroniseren.**</span><span class="sxs-lookup"><span data-stu-id="9c553-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="9c553-258">Selecteer Microsoft-verwijzing maken voor het aanpassen van CRM-veldtoewijzingen (op basis van de handleiding voor veldtoewijzingen) voor **het maken van gebeurtenissen.**</span><span class="sxs-lookup"><span data-stu-id="9c553-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="9c553-259">U kunt de toewijzingen in deze sectie bewerken op basis van de Handleiding voor veldtoewijzing.</span><span class="sxs-lookup"><span data-stu-id="9c553-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="9c553-260">Verwijzingssynchronisatie van end-to-end bi-directionele co-verkoop</span><span class="sxs-lookup"><span data-stu-id="9c553-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="9c553-261">Nadat u de Power Automate-oplossing hebt geïnstalleerd, geconfigureerd en aangepast, kunt u testen op synchronisatie van verwijzingen voor co-verkoop tussen Salesforce CRM en Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9c553-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="9c553-262">Vereisten</span><span class="sxs-lookup"><span data-stu-id="9c553-262">Pre-requisites</span></span>

<span data-ttu-id="9c553-263">Als u de verwijzingen tussen Partner Center salesforce en Salesforce CRM wilt synchroniseren, moet Power Automate oplossing microsoftspecifieke verwijzingsvelden duidelijk afbakenen.</span><span class="sxs-lookup"><span data-stu-id="9c553-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="9c553-264">Deze identificatie biedt uw verkopersteams de mogelijkheid om te bepalen welke verwijzingen ze willen delen met Microsoft voor co-verkoop.</span><span class="sxs-lookup"><span data-stu-id="9c553-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="9c553-265">Er is een set aangepaste velden beschikbaar als onderdeel van Partner Center de entiteit Verwijzingensynchronisatie voor Salesforce **CRM-oplossingskans.**</span><span class="sxs-lookup"><span data-stu-id="9c553-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="9c553-266">Een CRM-beheerder moet een afzonderlijke CRM-sectie maken met de aangepaste velden **voor** kansen.</span><span class="sxs-lookup"><span data-stu-id="9c553-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="9c553-267">De volgende aangepaste velden moeten deel uitmaken van de CRM-sectie:</span><span class="sxs-lookup"><span data-stu-id="9c553-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="9c553-268">**Synchroniseren met Partner Center:** of de kans moet worden gesynchroniseerd met Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9c553-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="9c553-269">**Verwijzings-id:** een veld met alleen-lezen-id's voor Microsoft Partner Center verwijzing</span><span class="sxs-lookup"><span data-stu-id="9c553-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="9c553-270">**Verwijzingskoppeling:** een alleen-lezenkoppeling naar de verwijzing in Microsoft Partner Center</span><span class="sxs-lookup"><span data-stu-id="9c553-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="9c553-271">**Hoe kan Microsoft helpen:** Hulp vereist van Microsoft voor de verwijzing</span><span class="sxs-lookup"><span data-stu-id="9c553-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="9c553-272">**Producten:** lijst met producten die zijn gekoppeld aan deze kans</span><span class="sxs-lookup"><span data-stu-id="9c553-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="9c553-273">**Controleren:** een alleen-lezen audittrail voor synchronisatie met Partner Center verwijzingen</span><span class="sxs-lookup"><span data-stu-id="9c553-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="9c553-274">Scenario 's:</span><span class="sxs-lookup"><span data-stu-id="9c553-274">SCENARIOS:</span></span>

1. <span data-ttu-id="9c553-275">Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in CRM en wordt gesynchroniseerd in Partner Center:</span><span class="sxs-lookup"><span data-stu-id="9c553-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="9c553-276">Meld u aan bij uw Salesforce CRM-omgeving met de gebruiker die inzicht heeft in de **sectie Opportunity** van het CRM.</span><span class="sxs-lookup"><span data-stu-id="9c553-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="9c553-277">Zorg ervoor dat de volgende sectie aanwezig is wanneer u een nieuwe kans maakt in de Salesforce CRM-omgeving</span><span class="sxs-lookup"><span data-stu-id="9c553-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce-omgeving.":::

   3. <span data-ttu-id="9c553-279">Als u deze mogelijkheid wilt synchroniseren met Microsoft Partner Center, moet u de volgende velden instellen in de kaartweergave:</span><span class="sxs-lookup"><span data-stu-id="9c553-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="9c553-280">"Synchroniseren met Partner Center": Ja</span><span class="sxs-lookup"><span data-stu-id="9c553-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="9c553-281">"Hoe kan Microsoft u helpen?": Selecteer een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="9c553-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="9c553-282">Producten: Oplossings-ID's van het product</span><span class="sxs-lookup"><span data-stu-id="9c553-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="9c553-283">Nadat u de optie Synchroniseren  **met** een Partner Center ingesteld op **Ja,** 10 minuten wachten, aanmelden bij uw Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="9c553-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="9c553-284">Uw verwijzingen worden gesynchroniseerd met Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c553-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="9c553-285">Wanneer de optie Synchroniseren met Partner Center is ingesteld op Ja. Als u de kans in Salesforce CRM bij werkt, worden de wijzigingen gesynchroniseerd met uw Partner Center account.</span><span class="sxs-lookup"><span data-stu-id="9c553-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="9c553-286">Verkoopkansen die zijn gesynchroniseerd met Partner Center worden geïdentificeerd met ✔icon in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c553-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="9c553-287">Verwijzingssynchronisatie wanneer verwijzing wordt gemaakt of bijgewerkt in Microsoft Partner Center en gesynchroniseerd in de Salesforce CRM-omgeving:</span><span class="sxs-lookup"><span data-stu-id="9c553-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="9c553-288">Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard/home)</span><span class="sxs-lookup"><span data-stu-id="9c553-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="9c553-289">Selecteer **Verwijzingen in** het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="9c553-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="9c553-290">Maak een nieuwe verwijzing voor co-verkoop vanuit Partner Center door te klikken op de optie Nieuwe deal.</span><span class="sxs-lookup"><span data-stu-id="9c553-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="9c553-291">Meld u aan bij uw Salesforce CRM-omgeving.</span><span class="sxs-lookup"><span data-stu-id="9c553-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="9c553-292">Navigeer **naar Open Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="9c553-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="9c553-293">De verwijzing die is gemaakt in Microsoft Partner Center is nu gesynchroniseerd in Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="9c553-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce-kansscherm.":::

    6. <span data-ttu-id="9c553-295">Wanneer u een gesynchroniseerde verwijzing selecteert, worden de details van de kaartweergave ingevuld.</span><span class="sxs-lookup"><span data-stu-id="9c553-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9c553-296">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="9c553-296">Next steps</span></span>

- [<span data-ttu-id="9c553-297">Leads beheren</span><span class="sxs-lookup"><span data-stu-id="9c553-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="9c553-298">Collectieve-verkoopkansen beheren</span><span class="sxs-lookup"><span data-stu-id="9c553-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="9c553-299">Partnercentrum-webhooks</span><span class="sxs-lookup"><span data-stu-id="9c553-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
