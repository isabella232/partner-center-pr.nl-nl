---
title: De out-of-Box Experience van een apparaat aanpassen
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Voordat u het nieuwe apparaat van een klant aflevert, kunt u Windows auto pilot-profielen gebruiken om de out-of-Box Experience (OOBE) van het apparaat aan te passen of vooraf te configureren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0ae61db0ca040afe67faa3a0883ea033b8f67562
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528501"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="8f1c5-103">Windows Autopilot-profielen gebruiken op nieuwe apparaten om de kant-en-klaar-ervaring van een klant aan te passen</span><span class="sxs-lookup"><span data-stu-id="8f1c5-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="8f1c5-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="8f1c5-104">**Applies to**</span></span>

- <span data-ttu-id="8f1c5-105">CSP-direct-factuur partners, indirecte providers en indirecte wederverkopers</span><span class="sxs-lookup"><span data-stu-id="8f1c5-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="8f1c5-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="8f1c5-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8f1c5-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="8f1c5-107">Admin agent</span></span>
- <span data-ttu-id="8f1c5-108">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="8f1c5-108">Global admin</span></span>
- <span data-ttu-id="8f1c5-109">Verkoop agent</span><span class="sxs-lookup"><span data-stu-id="8f1c5-109">Sales agent</span></span>
- <span data-ttu-id="8f1c5-110">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="8f1c5-110">User management admin</span></span>

<span data-ttu-id="8f1c5-111">Als u klant apparaten beheert, moet u mogelijk de out-of-Box Experience (OOBE) aanpassen voor de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="8f1c5-112">U kunt vooraf nieuwe apparaten configureren met Windows auto pilot-profielen voordat u de apparaten aan klanten levert en nieuwe profielen toepast op apparaten die klanten al hebben gekocht.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="8f1c5-113">Houd er rekening mee dat Oem's zijn begonnen met het verzenden van een verzend label op de buiten kant van het auto pilot-apparaat waarin de **product code-id (PKID)** van het apparaat wordt weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)** .</span></span>  <span data-ttu-id="8f1c5-114">Deze 1-dimensionale, lees bare streepjes code biedt downstream partners een manier om apparaten te registreren voor auto pilot zonder dat ze de apparaten hoeven te Unbox en de apparaat-ID niet op een andere manier te hoeven verzamelen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="8f1c5-115">In dit artikel wordt uitgelegd hoe u auto pilot-profielen kunt maken en Toep assen op apparaten in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="8f1c5-116">Als u nog niet bekend bent met auto pilot, raadpleegt u de informatie in deze artikelen:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="8f1c5-117">Overzicht van Windows auto pilot</span><span class="sxs-lookup"><span data-stu-id="8f1c5-117">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="8f1c5-118">Naslag Gids voor auto pilot-implementatie</span><span class="sxs-lookup"><span data-stu-id="8f1c5-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="8f1c5-119">Overzicht</span><span class="sxs-lookup"><span data-stu-id="8f1c5-119">Overview</span></span>

<span data-ttu-id="8f1c5-120">Met de functie Windows auto pilot in Partner Center kunt u aangepaste profielen maken om op klant apparaten toe te passen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="8f1c5-121">De volgende profiel instellingen zijn beschikbaar op het moment dat dit artikel werd gepubliceerd:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="8f1c5-122">Privacy-instellingen overs Laan.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-122">Skip privacy settings.</span></span> <span data-ttu-id="8f1c5-123">Met deze optionele auto pilot-profiel instelling kunnen organisaties geen privacy-instellingen meer vragen tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="8f1c5-124">Het maken van een lokaal beheerders account op het apparaat uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="8f1c5-125">Organisaties kunnen bepalen of de gebruiker die het apparaat instelt, beheerders toegang moet hebben nadat het proces is voltooid.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="8f1c5-126">Apparaat automatisch instellen voor werk of school.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="8f1c5-127">Alle apparaten die zijn geregistreerd met auto pilot worden automatisch beschouwd als werk-of school apparaten, zodat deze vraag niet wordt gesteld tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="8f1c5-128">Sla Setup-pagina's voor Cortana, OneDrive en OEM-registratie over.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="8f1c5-129">Alle apparaten die zijn geregistreerd met auto pilot, slaan deze pagina's automatisch over tijdens het OOBE-proces (out-of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="8f1c5-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="8f1c5-130">De gebruiksrecht overeenkomst (EULA) overs Laan.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="8f1c5-131">Met ingang van Windows 10 versie 1709 kunnen organisaties besluiten de EULA-pagina die wordt gepresenteerd tijdens het OOBE-proces over te slaan.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="8f1c5-132">Zie de [gebruiksrecht overeenkomst voor Windows auto pilot](#windows-autopilot-eula-dismissal) hieronder voor belang rijke informatie over het overs laan van de EULA-pagina tijdens Windows Setup.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="8f1c5-133">De volgende profiel- en apparaatbeheermachtigingen en -beperkingen zijn van toepassing:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="8f1c5-134">CSP-partners kunnen Autopilot-profielen blijven beheren voor bestaande klanten waarmee ze een reseller-relatie hebben, zelfs als de klanten de gedelegeerde beheermachtigingen van de partner hebben verwijderd.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="8f1c5-135">U kunt bestaande apparaten beheren voor de klanten die u hebt toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="8f1c5-136">U kunt geen apparaten beheren die uw klant heeft geüpload naar Microsoft Store voor Bedrijven of de Microsoft Intune-portal.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="8f1c5-137">Auto Pilot-profielen maken en beheren in het partner centrum</span><span class="sxs-lookup"><span data-stu-id="8f1c5-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="8f1c5-138">In Partner Center kunt u Windows auto pilot-implementatie profielen maken en deze Toep assen op apparaten.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="8f1c5-139">Alleen beheerder-agents kunnen profielen maken en Toep assen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="8f1c5-140">Een nieuw auto pilot-profiel maken</span><span class="sxs-lookup"><span data-stu-id="8f1c5-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="8f1c5-141">Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel wilt maken.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="8f1c5-142">Selecteer op de detail pagina van de klant de optie **apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-142">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="8f1c5-143">Onder **Windows auto pilot-profielen** selecteert u **Nieuw profiel toevoegen** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-143">Under **Windows Autopilot profiles** select **Add new profile** .</span></span>

4. <span data-ttu-id="8f1c5-144">Voer de naam en beschrijving van het profiel in en configureer de OOBE-instellingen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="8f1c5-145">U kunt kiezen uit:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-145">Choose from:</span></span>  

   - <span data-ttu-id="8f1c5-146">Privacy-instellingen in Setup overs Laan</span><span class="sxs-lookup"><span data-stu-id="8f1c5-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="8f1c5-147">Lokale beheerders account uitschakelen in installatie</span><span class="sxs-lookup"><span data-stu-id="8f1c5-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="8f1c5-148">Pagina's in Setup automatisch overs Laan</span><span class="sxs-lookup"><span data-stu-id="8f1c5-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="8f1c5-149">(Hiertoe *selecteert u automatisch instellingen voor werk of school en gaat u naar* de *pagina instellingen voor het instellen van Cortana, OneDrive en OEM-registratie.*</span><span class="sxs-lookup"><span data-stu-id="8f1c5-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages* )</span></span>
  
   - <span data-ttu-id="8f1c5-150">Gebruiksrecht overeenkomst overs Laan (EULA)</span><span class="sxs-lookup"><span data-stu-id="8f1c5-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="8f1c5-151">Zie de [gebruiksrecht overeenkomst voor Windows auto pilot](#windows-autopilot-eula-dismissal) hieronder voor belang rijke informatie over het overs laan van de EULA-pagina tijdens Windows Setup.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="8f1c5-152">Selecteer **verzenden** wanneer u klaar bent.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="8f1c5-153">Een auto pilot-profiel Toep assen op klant apparaten</span><span class="sxs-lookup"><span data-stu-id="8f1c5-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="8f1c5-154">In de onderstaande instructies wordt ervan uitgegaan dat u de apparaten van de klant al aan het partner centrum hebt toegevoegd en dat u toegang hebt tot hun apparaten lijst.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="8f1c5-155">Als u de apparaten van de klant nog niet hebt toegevoegd, volgt u de instructies in [apparaten toevoegen aan het account van een klant](#add-devices-to-a-customers-account) en volgt u de onderstaande stappen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="8f1c5-156">Nadat u een auto pilot-profiel voor een klant hebt gemaakt, kunt u dit Toep assen op de apparaten van de klant.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="8f1c5-157">Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8f1c5-158">Selecteer op de detail pagina van de klant de optie **apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-158">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="8f1c5-159">Selecteer onder **profielen Toep assen op apparaten** de apparaten of apparaatgroepen waaraan u profielen wilt toevoegen en selecteer vervolgens **profiel Toep assen** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile** .</span></span> <span data-ttu-id="8f1c5-160">Het profiel dat u zojuist hebt toegepast, wordt weer gegeven in de kolom **profiel** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="8f1c5-161">Volg de onderstaande stappen om te controleren of het profiel correct wordt toegepast op het apparaat.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="8f1c5-162">a.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-162">a.</span></span>  <span data-ttu-id="8f1c5-163">Sluit een apparaat aan op het netwerk en schakel het in.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="8f1c5-164">b.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-164">b.</span></span>  <span data-ttu-id="8f1c5-165">Controleer of de juiste OOBE-schermen (indien aanwezig) worden weer gegeven.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="8f1c5-166">c.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-166">c.</span></span>  <span data-ttu-id="8f1c5-167">Wanneer het OOBE-proces wordt gestopt, herstelt u de fabrieks instellingen van het apparaat om het voor te bereiden voor een nieuwe gebruiker.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="8f1c5-168">Een auto pilot-profiel verwijderen van het apparaat van een klant</span><span class="sxs-lookup"><span data-stu-id="8f1c5-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="8f1c5-169">Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="8f1c5-170">Selecteer op de detail pagina van de klant de optie **apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-170">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="8f1c5-171">Selecteer onder **profielen Toep assen op apparaten** de apparaten waarvan u het profiel wilt verwijderen en selecteer vervolgens **profiel verwijderen** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile** .</span></span>

   >[!NOTE]
   ><span data-ttu-id="8f1c5-172">Als u een profiel van een apparaat verwijdert, wordt het profiel niet uit de lijst verwijderd.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="8f1c5-173">Als u een profiel wilt verwijderen, volgt u de instructies in [Update of verwijdert u een auto pilot-profiel](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="8f1c5-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="8f1c5-174">Een auto pilot-profiel bijwerken of verwijderen</span><span class="sxs-lookup"><span data-stu-id="8f1c5-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="8f1c5-175">Als een klant de out-of-Box-ervaring wil wijzigen nadat u de apparaten naar hen hebt verzonden, kunt u het profiel wijzigen in partner centrum.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="8f1c5-176">Wanneer het apparaat van de klant verbinding maakt met internet, wordt de nieuwste profiel versie gedownload tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="8f1c5-177">Elke keer dat een klant een apparaat herstelt naar de standaard instellingen van de fabriek, zal het apparaat de meest recente profiel versie opnieuw downloaden tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="8f1c5-178">Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u een auto pilot-profiel wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="8f1c5-179">Selecteer op de detail pagina van de klant de optie **apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-179">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="8f1c5-180">Selecteer onder **Windows auto pilot-profielen** het profiel dat u wilt bijwerken.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="8f1c5-181">Breng de gewenste wijzigingen aan en selecteer vervolgens **verzenden** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-181">Make the required changes and then select **Submit** .</span></span>

<span data-ttu-id="8f1c5-182">Als u dit profiel wilt verwijderen, selecteert u **profiel verwijderen** in de rechter bovenhoek van de pagina.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="8f1c5-183">Apparaten aan de account van een klant toevoegen</span><span class="sxs-lookup"><span data-stu-id="8f1c5-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="8f1c5-184">Verkoop medewerkers en beheerders kunnen apparaten toevoegen aan het account van een klant.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="8f1c5-185">Voordat u aangepaste auto pilot-profielen op klant apparaten kunt Toep assen, moet u toegang hebben tot de apparaten lijst van de klant.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="8f1c5-186">Als u van plan bent om de combi natie van OEM-naam, serie nummer en model te gebruiken, moet u rekening houden met de volgende beperkingen:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="8f1c5-187">Deze tuple werkt alleen voor nieuwere apparaten (bijvoorbeeld 4.000 hashes) en wordt niet ondersteund voor 128b-hashes (RS2 en eerdere apparaten).</span><span class="sxs-lookup"><span data-stu-id="8f1c5-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="8f1c5-188">De tuple-registratie is hoofdletter gevoelig, dus de gegevens in het bestand moeten overeenkomen met de namen van het model en de fabrikant ***precies*** zoals opgegeven door de OEM-provider (hardwareprovider).</span><span class="sxs-lookup"><span data-stu-id="8f1c5-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="8f1c5-189">Volg de onderstaande instructies om apparaten toe te voegen aan het account van een klant in het partner centrum.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="8f1c5-190">Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant van wie u de apparaten wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="8f1c5-191">Selecteer op de detail pagina van de klant de optie **apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-191">On the customer's detail page, select **Devices** .</span></span>

3. <span data-ttu-id="8f1c5-192">Selecteer **apparaten toevoegen** onder **profielen Toep assen op apparaten** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-192">Under **Apply profiles to devices** select **Add devices** .</span></span>

4. <span data-ttu-id="8f1c5-193">Voer een naam in voor de apparaten lijst en selecteer vervolgens **Bladeren** om de lijst van de klant (in CSV-bestands indeling) naar het partner centrum te uploaden.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="8f1c5-194">U zou dit CSV-bestand moeten hebben ontvangen bij de aankoop van uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="8f1c5-195">Als u geen CSV-bestand hebt ontvangen, kunt u er zelf een maken door de stappen in [apparaten toevoegen aan Windows auto pilot te](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)volgen.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="8f1c5-196">Upload het CSV-bestand en selecteer vervolgens **Opslaan** .</span><span class="sxs-lookup"><span data-stu-id="8f1c5-196">Upload the .csv file and then select **Save** .</span></span>

<span data-ttu-id="8f1c5-197">Als u een foutbericht krijgt terwijl u probeert het .csv-bestand te uploaden, moet u de bestandsindeling controleren.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="8f1c5-198">U kunt alleen de hardwarehash gebruiken, of de OEM-naam, het serienummer en het model (in die kolomvolgorde) of de Windows-product-id.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="8f1c5-199">U kunt ook het bestand Sample. csv gebruiken dat is opgenomen in de koppeling naast **apparaten toevoegen** om een apparaten lijst te maken.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="8f1c5-200">Het CSV-bestand ziet er ongeveer als volgt uit:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="8f1c5-201">**Serie nummer van apparaat, Windows-product-ID, hardware-hash, naam van fabrikant, model van apparaat**</span><span class="sxs-lookup"><span data-stu-id="8f1c5-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="8f1c5-202">**{serialNumber},,, micro soft Corporation, Surface-laptop**</span><span class="sxs-lookup"><span data-stu-id="8f1c5-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="8f1c5-203">' Fabrikant naam ' en ' apparaat model ' zijn hoofdletter gevoelig.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="8f1c5-204">Als u niet weet welke waarde moet worden geplaatst voor de naam van de fabrikant en het model van het apparaat, kunt u dit op het apparaat uitvoeren om de juiste waarden te verzamelen:</span><span class="sxs-lookup"><span data-stu-id="8f1c5-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="8f1c5-205">Windows auto pilot-gebruiksrecht overeenkomst wordt genegeerd</span><span class="sxs-lookup"><span data-stu-id="8f1c5-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="8f1c5-206">BELANG RIJKE INFORMATIE</span><span class="sxs-lookup"><span data-stu-id="8f1c5-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="8f1c5-207">Met Windows auto pilot kunt u aangepaste installaties van Windows configureren op apparaten die u beheert voor uw klanten.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="8f1c5-208">Als de klant hiertoe hiertoe toestemming heeft gegeven, kunt u bepaalde ingestelde schermen onderdrukken of verbergen die normaal gesp roken worden gepresenteerd aan gebruikers bij het instellen van Windows, met inbegrip van de gebruiksrecht overeenkomst (EULA) op het acceptatie scherm.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="8f1c5-209">Als u deze functie gebruikt, u stemt ermee in dat alle schermen die zijn ontworpen om gebruikers te voorzien van een kennisgeving of instemming van de voor waarden, te onderdrukken of te verbergen. Dit betekent dat u voldoende toestemming hebt verkregen voor het verbergen van de voor waarden en dat u namens uw klant (of een organisatie of een individuele gebruiker als het geval) de voor waarden die van toepassing zijn op uw klant.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="8f1c5-210">Dit omvat overeenkomst met de voor waarden van de licentie of de kennisgeving die aan de gebruiker zou worden gepresenteerd als u deze niet hebt onderdrukt of verborgen met dit hulp programma.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="8f1c5-211">Uw klant gebruikt de Windows-software mogelijk niet op deze apparaten als de klant geen licentie heeft aangeschaft voor de software van micro soft of haar gelicentieerde distributeurs.</span><span class="sxs-lookup"><span data-stu-id="8f1c5-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>