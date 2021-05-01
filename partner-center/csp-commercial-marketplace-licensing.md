---
title: Licenties beheren in Marketplace-aanbiedingen
ms.topic: how-to
ms.date: 04/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het instellen en beheren van licenties voor uw aanbiedingen op de commerciële marketplace van ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3b2281696a2fe69253cd033eb2a7eef7fb3046f3
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284887"
---
# <a name="manage-licensing-in-marketplace-offers"></a><span data-ttu-id="808ec-103">Licenties beheren in Marketplace-aanbiedingen</span><span class="sxs-lookup"><span data-stu-id="808ec-103">Manage licensing in marketplace offers</span></span>

<span data-ttu-id="808ec-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="808ec-104">**Appropriate roles**</span></span>

- <span data-ttu-id="808ec-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="808ec-105">Global admin</span></span>
- <span data-ttu-id="808ec-106">Accountbeheerder</span><span class="sxs-lookup"><span data-stu-id="808ec-106">Account admin</span></span>

<span data-ttu-id="808ec-107">In dit artikel wordt beschreven hoe u een aanbieding in Partner Center instelt, deze beschikbaar maakt in Microsoft AppSource en vervolgens licenties voor die aanbieding beheert.</span><span class="sxs-lookup"><span data-stu-id="808ec-107">This article walks you through the process of setting up an offer in Partner Center, making it available in Microsoft AppSource, and then managing licenses for that offer.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="808ec-108">De mogelijkheden in dit artikel zijn momenteel beschikbaar als openbare preview.</span><span class="sxs-lookup"><span data-stu-id="808ec-108">The capabilities in this article are currently in Public Preview.</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="808ec-109">Voordat u begint</span><span class="sxs-lookup"><span data-stu-id="808ec-109">Before you begin</span></span>

<span data-ttu-id="808ec-110">Voordat u met dit proces begint, moet u vertrouwd raken met de onderstaande informatie.</span><span class="sxs-lookup"><span data-stu-id="808ec-110">Before beginning this process, you should familiarize yourself with the information below.</span></span>

### <a name="review-the-azure-marketplace-documentation"></a><span data-ttu-id="808ec-111">Bekijk de Azure Marketplace documentatie</span><span class="sxs-lookup"><span data-stu-id="808ec-111">Review the Azure Marketplace documentation</span></span>

<span data-ttu-id="808ec-112">De onderstaande artikelen bevatten informatie die u moet kennen voordat u doorgaat.</span><span class="sxs-lookup"><span data-stu-id="808ec-112">The articles below contain information you should know before continuing.</span></span> 

- [<span data-ttu-id="808ec-113">Een Dynamics 365 for Customer Engagement- en PowerApps-aanbieding maken</span><span class="sxs-lookup"><span data-stu-id="808ec-113">Create a Dynamics 365 for Customer Engagement & PowerApps offer</span></span>](https://docs.microsoft.com/azure/marketplace/dynamics-365-customer-engage-offer-setup)
- [<span data-ttu-id="808ec-114">Een commerciële marketplace-account maken in Partner Center</span><span class="sxs-lookup"><span data-stu-id="808ec-114">Create a commercial marketplace account in Partner Center</span></span>](https://docs.microsoft.com/azure/marketplace/create-account)

### <a name="create-your-offer-id"></a><span data-ttu-id="808ec-115">Uw aanbiedings-id maken</span><span class="sxs-lookup"><span data-stu-id="808ec-115">Create your Offer ID</span></span>

<span data-ttu-id="808ec-116">In de onderstaande procedures wordt u gevraagd een aanbiedings-id in te voeren.</span><span class="sxs-lookup"><span data-stu-id="808ec-116">In the procedures below, you’ll be prompted to enter an Offer ID.</span></span> <span data-ttu-id="808ec-117">Neem nu even de tijd om een geschikte aanbiedings-id te vinden, waarbij u rekening houdt met de volgende punten:</span><span class="sxs-lookup"><span data-stu-id="808ec-117">Take some time now to come up with a suitable Offer ID, keeping in mind the following points:</span></span>

- <span data-ttu-id="808ec-118">Deze id is zichtbaar voor klanten in het webadres voor de Marketplace-aanbieding en Azure Resource Manager sjablonen, indien van toepassing.</span><span class="sxs-lookup"><span data-stu-id="808ec-118">This ID is visible to customers in the web address for the marketplace offer and Azure Resource Manager templates, if applicable.</span></span>
- <span data-ttu-id="808ec-119">De aanbiedings-id in combinatie met de uitgevers-id moet minder dan 40 tekens lang zijn.</span><span class="sxs-lookup"><span data-stu-id="808ec-119">The Offer ID combined with the Publisher ID must be under 40 characters in length.</span></span>
- <span data-ttu-id="808ec-120">Gebruik alleen kleine letters en cijfers.</span><span class="sxs-lookup"><span data-stu-id="808ec-120">Use only lowercase letters and numbers.</span></span> <span data-ttu-id="808ec-121">De aanbiedings-id kan afbreekstreepingstekens en onderstrepingstekens bevatten, maar geen spaties.</span><span class="sxs-lookup"><span data-stu-id="808ec-121">The Offer ID can include hyphens and underscores, but no spaces.</span></span> <span data-ttu-id="808ec-122">Als uw uitgevers-id bijvoorbeeld testpublisherid is en u test-offer-1 in voert, is het webadres van de aanbieding https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1 .</span><span class="sxs-lookup"><span data-stu-id="808ec-122">For example, if your Publisher ID is testpublisherid and you enter test-offer-1, the offer web address will be https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1.</span></span>
- <span data-ttu-id="808ec-123">Deze id kan niet worden gewijzigd nadat u Maken **hebt geselecteerd.**</span><span class="sxs-lookup"><span data-stu-id="808ec-123">This ID can't be changed after you select **Create**.</span></span>

### <a name="create-your-offer-alias"></a><span data-ttu-id="808ec-124">Uw aanbiedingsalias maken</span><span class="sxs-lookup"><span data-stu-id="808ec-124">Create your Offer alias</span></span>

<span data-ttu-id="808ec-125">De alias Aanbieding is de naam die wordt gebruikt voor de aanbieding in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="808ec-125">The Offer alias is the name used for the offer in Partner Center.</span></span> <span data-ttu-id="808ec-126">U hebt ook een geschikte alias voor de aanbieding nodig die de onderstaande richtlijnen volgt:</span><span class="sxs-lookup"><span data-stu-id="808ec-126">You’ll also need an appropriate Offer alias that follows the guidelines below:</span></span>

- <span data-ttu-id="808ec-127">Deze naam wordt niet gebruikt in de marketplace en verschilt van de naam van de aanbieding en andere waarden die aan klanten worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="808ec-127">This name isn't used in the marketplace and is different from the offer name and other values shown to customers.</span></span>
- <span data-ttu-id="808ec-128">Deze naam kan niet worden gewijzigd nadat u Maken hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="808ec-128">This name can't be changed after you select Create.</span></span>

## <a name="create-your-offer"></a><span data-ttu-id="808ec-129">Uw aanbieding maken</span><span class="sxs-lookup"><span data-stu-id="808ec-129">Create your offer</span></span>

<span data-ttu-id="808ec-130">De eerste stap in het licentieproces is het maken van uw aanbieding op de commerciële marketplace.</span><span class="sxs-lookup"><span data-stu-id="808ec-130">The first step in the licensing process is to create your commercial marketplace offer.</span></span> 

1. <span data-ttu-id="808ec-131">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="808ec-131">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="808ec-132">Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**</span><span class="sxs-lookup"><span data-stu-id="808ec-132">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="808ec-133">Selecteer bovenaan de pagina Overzicht de optie Nieuwe **aanbieding** en selecteer vervolgens **Dynamics 365 for Customer Engagement & PowerApps.**</span><span class="sxs-lookup"><span data-stu-id="808ec-133">At the top of the Overview page, select **New offer**, and then select **Dynamics 365 for Customer Engagement & PowerApps**.</span></span>
4. <span data-ttu-id="808ec-134">Voer de **aanbiedings-id en** **aanbiedingsalias in** die u eerder hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="808ec-134">Enter the **Offer ID** and **Offer alias** you created earlier.</span></span>
5. <span data-ttu-id="808ec-135">Selecteer **Maken om** de aanbieding te genereren en door te gaan.</span><span class="sxs-lookup"><span data-stu-id="808ec-135">Select **Create** to generate the offer and continue.</span></span>
6. <span data-ttu-id="808ec-136">Kies uw licentieopties.</span><span class="sxs-lookup"><span data-stu-id="808ec-136">Choose your licensing options.</span></span>

    - <span data-ttu-id="808ec-137">Als u licentiebeheer voor uw aanbieding wilt inschakelen, selecteert u **App-licentiebeheer via Microsoft inschakelen.**</span><span class="sxs-lookup"><span data-stu-id="808ec-137">To enable license management for your offer, select **Enable app license management through Microsoft**.</span></span> <span data-ttu-id="808ec-138">Dit is een een time-instelling en u kunt deze niet meer wijzigen nadat uw aanbieding is gepubliceerd.</span><span class="sxs-lookup"><span data-stu-id="808ec-138">This is a one-time setting, and you can’t change it once your offer is published.</span></span>

    - <span data-ttu-id="808ec-139">U kunt klanten ook in staat stellen om de basisfunctionaliteit van uw app uit te voeren zonder licentie en Premium-functies uit te voeren zodra ze een licentie hebben aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="808ec-139">You can also enable customers to run your app’s base functionality without a license, and run premium features once they’ve purchased a license.</span></span> <span data-ttu-id="808ec-140">Als u dit wilt doen, **selecteert u Klanten toestaan mijn app te installeren, zelfs als er geen licenties zijn toegewezen.**</span><span class="sxs-lookup"><span data-stu-id="808ec-140">To do this, select **Allow customers to install my app even if licenses are not assigned**.</span></span>

    - <span data-ttu-id="808ec-141">Als u niet wilt dat licentiebeheer voor uw aanbieding is ingeschakeld, selecteert u Nu downloaden **(gratis)**, **Gratis** proefversie of **Neem contact met mij op.**</span><span class="sxs-lookup"><span data-stu-id="808ec-141">If you don’t want your offer to have license management enabled, select **Get it now (Free)**, **Free trial**, or **Contact me**.</span></span>

## <a name="create-your-plan"></a><span data-ttu-id="808ec-142">Uw plan maken</span><span class="sxs-lookup"><span data-stu-id="808ec-142">Create your plan</span></span>

<span data-ttu-id="808ec-143">In deze stappen definieert u het plan of de plannen die u wilt inschakelen voor uw aanbieding.</span><span class="sxs-lookup"><span data-stu-id="808ec-143">In these steps you’ll define the plan or plans you want to enable for your offer.</span></span>

1. <span data-ttu-id="808ec-144">Selecteer in het navigatiemenu aan de **linkerkant Overzicht plannen** en selecteer **vervolgens Nieuw plan maken.**</span><span class="sxs-lookup"><span data-stu-id="808ec-144">On the left navigation menu, select **Plan overview**, and then select **Create new plan**.</span></span>
2. <span data-ttu-id="808ec-145">Voer een **plan-id** en **plannaam in** en selecteer **vervolgens Maken.**</span><span class="sxs-lookup"><span data-stu-id="808ec-145">Enter a **Plan ID** and **Plan name**, and then select **Create**.</span></span>
3. <span data-ttu-id="808ec-146">Voer op **de pagina Abonnementsvermelding** de beschrijving van uw abonnement **in.**</span><span class="sxs-lookup"><span data-stu-id="808ec-146">On the **Plan listing** page, enter your **Plan description**.</span></span>
4. <span data-ttu-id="808ec-147">Als u de beschrijving wilt opslaan en later wilt voltooien, **selecteert u Concept opslaan.**</span><span class="sxs-lookup"><span data-stu-id="808ec-147">To save the description and finish later, select **Save draft**.</span></span>

5. <span data-ttu-id="808ec-148">Wanneer u klaar bent, selecteert u **Controleren en publiceren.**</span><span class="sxs-lookup"><span data-stu-id="808ec-148">When you’re finished, select **Review and publish**.</span></span> <span data-ttu-id="808ec-149">De plangegevens worden nu weergegeven op appsource.microsoft.com aanbiedingsvermelding (sectie abonnementen).</span><span class="sxs-lookup"><span data-stu-id="808ec-149">The plan information will now be displayed on appsource.microsoft.com under offer listing (plans section).</span></span>

6. <span data-ttu-id="808ec-150">Nadat u alle plannen voor deze aanbieding hebt gemaakt, moet u de service-id van elk plan kopiëren.</span><span class="sxs-lookup"><span data-stu-id="808ec-150">After you’ve created all of the plans for this offer, you’ll need to copy each plan’s Service ID.</span></span> <span data-ttu-id="808ec-151">Selecteer **Bovenaan de pagina** Abonnementsvermelding de optie Planoverzicht.</span><span class="sxs-lookup"><span data-stu-id="808ec-151">Select **Plan overview** at the top of the Plan listing page.</span></span> <span data-ttu-id="808ec-152">Kopieer de service-id voor elk plan naar een veilige locatie.</span><span class="sxs-lookup"><span data-stu-id="808ec-152">Copy the Service ID for each plan to a safe location.</span></span>

## <a name="add-service-ids-to-your-solution"></a><span data-ttu-id="808ec-153">Service-ID's toevoegen aan uw oplossing</span><span class="sxs-lookup"><span data-stu-id="808ec-153">Add Service IDs to your solution</span></span>

<span data-ttu-id="808ec-154">De volgende stap is het bijwerken van uw oplossing door de service-ID's toe te voegen voor elk plan dat u zojuist hebt gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="808ec-154">The next step is to update your solution by adding the Service IDs for each plan that you just copied.</span></span> <span data-ttu-id="808ec-155">Zie Create an [AppSource Package for your solution (Een AppSource-pakket maken voor uw oplossing) voor hulp hiervoor.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)</span><span class="sxs-lookup"><span data-stu-id="808ec-155">For guidance on this, see [Create an AppSource Package for your solution](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource).</span></span>

## <a name="upload-your-package-and-publish-your-offer"></a><span data-ttu-id="808ec-156">Uw pakket uploaden en uw aanbieding publiceren</span><span class="sxs-lookup"><span data-stu-id="808ec-156">Upload your package and publish your offer</span></span>

1. <span data-ttu-id="808ec-157">Selecteer commerciële marketplace in het navigatiedeelvenster **aan de linkerkant** en selecteer **vervolgens Technische configuratie.**</span><span class="sxs-lookup"><span data-stu-id="808ec-157">On the left navigation pane, select **Commercial Marketplace**, and then select **Technical configuration**.</span></span>
2. <span data-ttu-id="808ec-158">Selecteer **onder Basislicentiemodel** de optie **Gebruiker**.</span><span class="sxs-lookup"><span data-stu-id="808ec-158">Under **Base License Model**, select **User**.</span></span>
3. <span data-ttu-id="808ec-159">Voer **onder CRM-pakket** de URL van uw pakketlocatie in.</span><span class="sxs-lookup"><span data-stu-id="808ec-159">Under **CRM Package**, enter the URL of your package location.</span></span>
4. <span data-ttu-id="808ec-160">Gebruik de andere tabbladen in het linkernavigatievenster om andere vereiste gegevens in te voeren.</span><span class="sxs-lookup"><span data-stu-id="808ec-160">Use the other tabs on the left navigation pane to enter any other required information.</span></span> <span data-ttu-id="808ec-161">Wanneer u klaar bent, selecteert u **Controleren en publiceren.**</span><span class="sxs-lookup"><span data-stu-id="808ec-161">When you’re done, select **Review and publish**.</span></span>

<span data-ttu-id="808ec-162">Nadat u de aanbieding hebt gepubliceerd, controleren en verifiëren we uw gegevens.</span><span class="sxs-lookup"><span data-stu-id="808ec-162">After you publish the offer, we’ll review and verify your information.</span></span> <span data-ttu-id="808ec-163">Als er problemen zijn met dit proces, stellen we u hiervan op de hoogte.</span><span class="sxs-lookup"><span data-stu-id="808ec-163">If there are any issues with this process, we’ll notify you.</span></span> <span data-ttu-id="808ec-164">Wanneer alle problemen zijn opgelost, ontvangt u een melding dat uw aanbieding beschikbaar is in AppSource.</span><span class="sxs-lookup"><span data-stu-id="808ec-164">When all issues have been resolved, you’ll get a notification that your offer is available in AppSource.</span></span> <span data-ttu-id="808ec-165">Op dat moment kunt u het live maken.</span><span class="sxs-lookup"><span data-stu-id="808ec-165">At that point you can make it live.</span></span>

## <a name="make-your-offer-live-in-partner-center"></a><span data-ttu-id="808ec-166">Uw aanbieding live maken in Partner Center</span><span class="sxs-lookup"><span data-stu-id="808ec-166">Make your offer live in Partner Center</span></span>

<span data-ttu-id="808ec-167">De onderstaande procedure laat u zien hoe u uw aanbieding live kunt maken in AppSource.</span><span class="sxs-lookup"><span data-stu-id="808ec-167">The procedure below walks you through the process of making your offer live in AppSource.</span></span> <span data-ttu-id="808ec-168">Zie Inleiding tot aanbiedingsopties voor meer informatie [over dit proces.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)</span><span class="sxs-lookup"><span data-stu-id="808ec-168">To learn more about this process, see [Introduction to listing options](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type).</span></span>

>[!NOTE]
><span data-ttu-id="808ec-169">Nadat u uw aanbieding hebt gepubliceerd, duurt het 4-6 uur om live te gaan.</span><span class="sxs-lookup"><span data-stu-id="808ec-169">Once you publish your offer, it will take 4-6 hours to go live.</span></span>

1. <span data-ttu-id="808ec-170">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="808ec-170">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="808ec-171">Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**</span><span class="sxs-lookup"><span data-stu-id="808ec-171">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="808ec-172">Zoek op **de** pagina Overzicht de aanbieding die u zoekt.</span><span class="sxs-lookup"><span data-stu-id="808ec-172">On the **Overview** page, find the offer you’re looking for.</span></span> <span data-ttu-id="808ec-173">Aanbiedingen die gereed zijn om te worden gepubliceerd, hebben de status **Preview**.</span><span class="sxs-lookup"><span data-stu-id="808ec-173">Offers ready to be published will have a status of **Preview**.</span></span> <span data-ttu-id="808ec-174">Selecteer de aanbieding.</span><span class="sxs-lookup"><span data-stu-id="808ec-174">Select the offer.</span></span>
4. <span data-ttu-id="808ec-175">Selecteer op **de overzichtspagina** van de aanbieding **de optie Live gaan.**</span><span class="sxs-lookup"><span data-stu-id="808ec-175">On the **Offer overview** page, select **Go live**.</span></span>
<span data-ttu-id="808ec-176">De aanbieding is over 4-6 uur live.</span><span class="sxs-lookup"><span data-stu-id="808ec-176">The offer will be live in 4-6 hours.</span></span>
5. <span data-ttu-id="808ec-177">Als u uw aanbiedingsvermelding op AppSource wilt zien, selecteert u de **koppeling AppSource** onder aan de **overzichtspagina van de** aanbieding.</span><span class="sxs-lookup"><span data-stu-id="808ec-177">To see your offer listing on AppSource, select the **AppSource** link at the bottom of the **Offer overview** page.</span></span>

    - <span data-ttu-id="808ec-178">**Voor aanbiedingen met licentie:** als voor uw aanbieding een licentiecontrole is vereist, kunnen gebruikers alleen een lead invoeren door op **Contact** opnemen te klikken, zodat u met hen kunt communiceren.</span><span class="sxs-lookup"><span data-stu-id="808ec-178">**For license-enabled offers**: If your offer requires a license check, users will only be able to enter a lead by clicking **Contact Me**, so that you can communicate with them.</span></span>

    - <span data-ttu-id="808ec-179">**Voor aanbiedingen met licentie** met een gratis installatieoptie: als voor uw aanbieding  geen licentiecontrole is vereist, zien beheerders de knop Nu downloaden naast **Contact opnemen.**</span><span class="sxs-lookup"><span data-stu-id="808ec-179">**For license-enabled offers with free installation option**: If your offer does not require a license check, admin users will see a **Get It Now** button in addition to **Contact Me**.</span></span> <span data-ttu-id="808ec-180">Gebruikers die uw gratis installatieoptie willen proberen, moeten klikken op Nu **downloaden.** Dit brengt hen bij het installeren van de aanbieding in Power Platform Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="808ec-180">Users who want to try your free installation option should click **Get It Now**, which will bring them to install the offer on Power Platform Admin Center.</span></span> <span data-ttu-id="808ec-181">Gebruikers kunnen Contact **opnemen nog steeds gebruiken** als ze vragen hebben of als ze willen upgraden naar een betaald abonnement.</span><span class="sxs-lookup"><span data-stu-id="808ec-181">Users can still use **Contact Me** if they have any questions, or if they want to upgrade to a paid plan.</span></span>

## <a name="register-isv-connect-deal-in-dealreg"></a><span data-ttu-id="808ec-182">ISV Connect-deal registreren in DealReg</span><span class="sxs-lookup"><span data-stu-id="808ec-182">Register ISV Connect deal in DealReg</span></span>

<span data-ttu-id="808ec-183">De volgende stap is het registreren van uw deal.</span><span class="sxs-lookup"><span data-stu-id="808ec-183">The next step is to register your deal.</span></span> <span data-ttu-id="808ec-184">Zie Uw deals registreren [om dit te doen.](https://docs.microsoft.com/partner-center/register-deals)</span><span class="sxs-lookup"><span data-stu-id="808ec-184">To do this, see [Register your deals](https://docs.microsoft.com/partner-center/register-deals).</span></span>

## <a name="invite-the-customer"></a><span data-ttu-id="808ec-185">De klant uitnodigen</span><span class="sxs-lookup"><span data-stu-id="808ec-185">Invite the customer</span></span>

<span data-ttu-id="808ec-186">Gebruik de volgende procedure om de klant uit te nodigen om deel te nemen aan deze deal.</span><span class="sxs-lookup"><span data-stu-id="808ec-186">Use the following procedure to invite the customer to participate in this deal.</span></span>  

1. <span data-ttu-id="808ec-187">Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="808ec-187">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="808ec-188">Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**</span><span class="sxs-lookup"><span data-stu-id="808ec-188">On the left navigation menu, select **Commercial Marketplace/Overview**.</span></span>
3. <span data-ttu-id="808ec-189">Filter op **Verzonden** deals, selecteer **het tabblad Wordt** uitgevoerd en selecteer vervolgens de deal die u wilt.</span><span class="sxs-lookup"><span data-stu-id="808ec-189">Filter for **Submitted** deals, select the **In Progress** tab, and then select the deal you want.</span></span>
4. <span data-ttu-id="808ec-190">Selecteer Licenties beheren op de **overzichtspagina voor deze deal.**</span><span class="sxs-lookup"><span data-stu-id="808ec-190">On the overview page for this deal, select **Manage licenses**.</span></span>
5. <span data-ttu-id="808ec-191">Selecteer in **het venster Licenties beheren** de klant in de **vervolgkeuzelijst Klantgegevens.**</span><span class="sxs-lookup"><span data-stu-id="808ec-191">In the **Manage licenses** window, select the customer from the **Customer details** dropdown list.</span></span> <span data-ttu-id="808ec-192">Als de klantrelatie nog niet bestaat, selecteert u **+Een nieuwe klant uitnodigen om toestemming te geven.**</span><span class="sxs-lookup"><span data-stu-id="808ec-192">If the customer relationship does not exist yet, select **+Invite a new customer to consent**.</span></span>
6. <span data-ttu-id="808ec-193">Kopieer de koppeling die wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="808ec-193">Copy the link that is displayed.</span></span>
7. <span data-ttu-id="808ec-194">Stuur deze koppeling via e-mail naar de factureringsbeheerder of globale beheerder van uw klant. Laat deze koppeling gebruiken om toegang te krijgen tot admin.microsoft.com en de relatie die u tot stand wilt stellen te accepteren en autoriseerde.</span><span class="sxs-lookup"><span data-stu-id="808ec-194">Email this link to your customer’s billing admin or global admin, and have them use this link to access admin.microsoft.com and accept and authorize the relationship you’re establishing.</span></span>

    >[!NOTE]
    ><span data-ttu-id="808ec-195">De relatie wordt pas tot stand gebracht als de klant deze stap uitvoert.</span><span class="sxs-lookup"><span data-stu-id="808ec-195">The relationship will not be established until the customer performs this step.</span></span>

## <a name="activate-manage-and-remove-your-licenses"></a><span data-ttu-id="808ec-196">Uw licenties activeren, beheren en verwijderen</span><span class="sxs-lookup"><span data-stu-id="808ec-196">Activate, manage, and remove your licenses</span></span>

<span data-ttu-id="808ec-197">Zodra uw klant tot stand is gebracht, kunt u beginnen met het toevoegen van plannen vanuit uw aanbieding en licenties toewijzen aan elk plan.</span><span class="sxs-lookup"><span data-stu-id="808ec-197">Once your customer has been established, you can start adding plans from your offer and assigning licenses to each plan.</span></span>

1. <span data-ttu-id="808ec-198">Selecteer in het venster Licenties beheren voor deze deal de optie **+Een abonnement toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="808ec-198">In the Manage licenses window for this deal, select **+Add a plan**.</span></span>
2. <span data-ttu-id="808ec-199">Vul de **velden Abonnementen voor deze oplossing** en Aantal **licenties** in en selecteer vervolgens **Licenties bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="808ec-199">Complete the **Plans for this solution** and **Number of licenses** fields, and then select **Update licenses**.</span></span> <span data-ttu-id="808ec-200">De licenties zijn beschikbaar op admin.microsoft.com klanten kunnen beheren en toewijzen aan werknemers.</span><span class="sxs-lookup"><span data-stu-id="808ec-200">The licenses will be available at admin.microsoft.com for customers to manage and assign to employees.</span></span>

    - <span data-ttu-id="808ec-201">Als u het aantal licenties voor een bestaand abonnement  wilt wijzigen, voert u het nieuwe nummer in het veld Aantal licenties in en selecteert u **vervolgens Licenties bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="808ec-201">To change the number of licenses for an existing plan, enter the new number in the **Number of licenses** field and then select **Update licenses**.</span></span>

    - <span data-ttu-id="808ec-202">Als u licenties voor een deal wilt deactiveren of verwijderen, selecteert u het prullenbakpictogram in het **veld** Acties en selecteert u **vervolgens Licenties bijwerken.**</span><span class="sxs-lookup"><span data-stu-id="808ec-202">To deactivate or remove licenses for a deal, select the trash can icon in the **Actions** field and then select **Update licenses**.</span></span>