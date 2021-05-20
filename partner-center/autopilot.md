---
title: De out-of-box-ervaring van een apparaat aanpassen
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Voordat u het nieuwe apparaat van een klant levert, kunt u Windows Autopilot-profielen gebruiken om de out-of-box experience (OOBE) van het apparaat aan te passen of vooraf te configureren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149822"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="15995-103">Windows Autopilot-profielen gebruiken op nieuwe apparaten om de kant-en-klaar-ervaring van een klant aan te passen</span><span class="sxs-lookup"><span data-stu-id="15995-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="15995-104">**Juiste rollen:** beheeragent | Globale beheerder | Verkoopagent | Beheerder van gebruikersbeheer</span><span class="sxs-lookup"><span data-stu-id="15995-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="15995-105">Als u klantapparaten beheert, moet u mogelijk de out-of-box experience (OOBE) aanpassen voor de gebruikers van de klant.</span><span class="sxs-lookup"><span data-stu-id="15995-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="15995-106">U kunt nieuwe apparaten vooraf configureren met Windows Autopilot-profielen voordat u de apparaten aan klanten levert en nieuwe profielen toepassen op apparaten die klanten al hebben aangeschaft.</span><span class="sxs-lookup"><span data-stu-id="15995-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="15995-107">Houd er rekening mee dat OEM's zijn begonnen met het gebruik van een verzendlabel aan de buitenzijde van het Autopilot-apparaatvak, met daarin de **PKID (Product Key ID)** van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="15995-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="15995-108">Deze 1-dimensionale, leesbare streepjescode biedt downstreampartners een manier om apparaten te registreren voor Autopilot zonder dat de apparaten uit het postvak moeten worden geplaatst en de apparaat-id op een alternatieve manier moeten worden gesereerd.</span><span class="sxs-lookup"><span data-stu-id="15995-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="15995-109">In dit artikel wordt uitgelegd hoe u Autopilot-profielen kunt maken en toepassen op apparaten in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15995-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="15995-110">Als u nog niet bekend bent met Autopilot, bekijkt u de informatie in deze artikelen:</span><span class="sxs-lookup"><span data-stu-id="15995-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="15995-111">Overzicht van Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="15995-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="15995-112">Naslaghandleiding voor Autopilot-implementatie</span><span class="sxs-lookup"><span data-stu-id="15995-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="15995-113">Overzicht</span><span class="sxs-lookup"><span data-stu-id="15995-113">Overview</span></span>

<span data-ttu-id="15995-114">Met de Windows Autopilot-functie in Partner Center kunt u aangepaste profielen maken om toe te passen op apparaten van klanten.</span><span class="sxs-lookup"><span data-stu-id="15995-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="15995-115">De volgende profielinstellingen waren beschikbaar op het moment dat dit artikel werd gepubliceerd:</span><span class="sxs-lookup"><span data-stu-id="15995-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="15995-116">Privacy-instellingen overslaan.</span><span class="sxs-lookup"><span data-stu-id="15995-116">Skip privacy settings.</span></span> <span data-ttu-id="15995-117">Met deze optionele Autopilot-profielinstelling kunnen organisaties geen vragen stellen over privacy-instellingen tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="15995-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="15995-118">Het maken van lokale beheerdersaccounts op het apparaat uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="15995-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="15995-119">Organisaties kunnen bepalen of de gebruiker die het apparaat instel, beheerderstoegang moet hebben zodra het proces is voltooid.</span><span class="sxs-lookup"><span data-stu-id="15995-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="15995-120">Apparaat automatisch instellen voor werk of school.</span><span class="sxs-lookup"><span data-stu-id="15995-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="15995-121">Alle apparaten die zijn geregistreerd bij Autopilot, worden automatisch beschouwd als werk- of schoolapparaten. Deze vraag wordt dus niet gesteld tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="15995-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="15995-122">Sla de installatiepagina's voor Cortana, OneDrive en OEM-registratie over.</span><span class="sxs-lookup"><span data-stu-id="15995-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="15995-123">Alle apparaten die zijn geregistreerd bij Autopilot slaan deze pagina's automatisch over tijdens het OOBE-proces (Out-Of-Box Experience).</span><span class="sxs-lookup"><span data-stu-id="15995-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="15995-124">Sla de gebruikersinterface (EULA) over.</span><span class="sxs-lookup"><span data-stu-id="15995-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="15995-125">Vanaf Windows 10 versie 1709 kunnen organisaties besluiten om de eula-pagina over te slaan die tijdens het OOBE-proces wordt gepresenteerd.</span><span class="sxs-lookup"><span data-stu-id="15995-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="15995-126">Zie [Windows Autopilot eula hieronder voor](#windows-autopilot-eula-dismissal) belangrijke informatie over het overslaan van de eula-pagina tijdens de installatie van Windows.</span><span class="sxs-lookup"><span data-stu-id="15995-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="15995-127">De volgende profiel- en apparaatbeheermachtigingen en -beperkingen zijn van toepassing:</span><span class="sxs-lookup"><span data-stu-id="15995-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="15995-128">CSP-partners kunnen Autopilot-profielen blijven beheren voor bestaande klanten waarmee ze een reseller-relatie hebben, zelfs als de klanten de gedelegeerde beheermachtigingen van de partner hebben verwijderd.</span><span class="sxs-lookup"><span data-stu-id="15995-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="15995-129">U kunt bestaande apparaten beheren voor de klanten die u hebt toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="15995-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="15995-130">U kunt geen apparaten beheren die uw klant heeft geüpload naar Microsoft Store voor Bedrijven of de Microsoft Intune-portal.</span><span class="sxs-lookup"><span data-stu-id="15995-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="15995-131">Autopilot-profielen maken en beheren in Partner Center</span><span class="sxs-lookup"><span data-stu-id="15995-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="15995-132">In Partner Center kunt u een Windows Autopilot maken en toepassen op apparaten.</span><span class="sxs-lookup"><span data-stu-id="15995-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="15995-133">Alleen beheerders kunnen profielen maken en toepassen.</span><span class="sxs-lookup"><span data-stu-id="15995-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="15995-134">Een nieuw Autopilot-profiel maken</span><span class="sxs-lookup"><span data-stu-id="15995-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="15995-135">Selecteer **Klanten** in Partner Center menu en selecteer vervolgens de klant voor wie u het Autopilot-profiel maakt.</span><span class="sxs-lookup"><span data-stu-id="15995-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="15995-136">Selecteer apparaten op de detailpagina van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="15995-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="15995-137">Selecteer **onder Windows Autopilot de** optie Nieuw profiel **toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="15995-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="15995-138">Voer de naam en beschrijving van het profiel in en configureer vervolgens de OOBE-instellingen.</span><span class="sxs-lookup"><span data-stu-id="15995-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="15995-139">U kunt kiezen uit:</span><span class="sxs-lookup"><span data-stu-id="15995-139">Choose from:</span></span>  

   - <span data-ttu-id="15995-140">Privacy-instellingen overslaan tijdens de installatie</span><span class="sxs-lookup"><span data-stu-id="15995-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="15995-141">Lokaal beheerdersaccount uitschakelen tijdens de installatie</span><span class="sxs-lookup"><span data-stu-id="15995-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="15995-142">Pagina's automatisch overslaan tijdens de installatie</span><span class="sxs-lookup"><span data-stu-id="15995-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="15995-143">*(Inclusief: automatisch instellen selecteren voor werk of school* en pagina's voor het instellen van *Cortana, OneDrive en OEM-registratie overslaan)*</span><span class="sxs-lookup"><span data-stu-id="15995-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="15995-144">Gebruikersinterfaceovereenkomst (EULA) overslaan</span><span class="sxs-lookup"><span data-stu-id="15995-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="15995-145">Zie [Windows Autopilot eula hieronder voor](#windows-autopilot-eula-dismissal) belangrijke informatie over het overslaan van de eula-pagina tijdens de installatie van Windows.</span><span class="sxs-lookup"><span data-stu-id="15995-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="15995-146">Selecteer **Verzenden wanneer** u klaar bent.</span><span class="sxs-lookup"><span data-stu-id="15995-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="15995-147">Een Autopilot-profiel toepassen op apparaten van klanten</span><span class="sxs-lookup"><span data-stu-id="15995-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="15995-148">In de onderstaande instructies wordt ervan uitgenomen dat u de apparaten van de klant al hebt toegevoegd aan Partner Center en dat u toegang hebt tot de apparatenlijst.</span><span class="sxs-lookup"><span data-stu-id="15995-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="15995-149">Als u de apparaten van de klant nog niet hebt toegevoegd, volgt u de instructies in Apparaten toevoegen aan het account van een [klant](#add-devices-to-a-customers-account) en volgt u de onderstaande stappen.</span><span class="sxs-lookup"><span data-stu-id="15995-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="15995-150">Nadat u een Autopilot-profiel voor een klant hebt gemaakt, kunt u dit toepassen op de apparaten van de klant.</span><span class="sxs-lookup"><span data-stu-id="15995-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="15995-151">Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant voor wie u het Autopilot-profiel hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="15995-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="15995-152">Selecteer apparaten op de detailpagina van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="15995-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="15995-153">Selecteer **onder Profielen toepassen op apparaten** de apparaten of apparaatgroepen aan wie u profielen wilt toevoegen en selecteer vervolgens Profiel **toepassen.**</span><span class="sxs-lookup"><span data-stu-id="15995-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="15995-154">Het profiel dat u zojuist hebt toegepast, wordt weergegeven in de **kolom** Profiel.</span><span class="sxs-lookup"><span data-stu-id="15995-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="15995-155">Volg de onderstaande stappen om te controleren of het profiel wordt toegepast op het apparaat.</span><span class="sxs-lookup"><span data-stu-id="15995-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="15995-156">a.</span><span class="sxs-lookup"><span data-stu-id="15995-156">a.</span></span>  <span data-ttu-id="15995-157">Verbind een apparaat met het netwerk en schakel het in.</span><span class="sxs-lookup"><span data-stu-id="15995-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="15995-158">b.</span><span class="sxs-lookup"><span data-stu-id="15995-158">b.</span></span>  <span data-ttu-id="15995-159">Controleer of de juiste OOBE-schermen (indien van toepassing) worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="15995-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="15995-160">c.</span><span class="sxs-lookup"><span data-stu-id="15995-160">c.</span></span>  <span data-ttu-id="15995-161">Wanneer het OOBE-proces stopt, stelt u de fabrieksinstellingen van het apparaat opnieuw in om het voor te bereiden voor een nieuwe gebruiker.</span><span class="sxs-lookup"><span data-stu-id="15995-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="15995-162">Een Autopilot-profiel verwijderen van het apparaat van een klant</span><span class="sxs-lookup"><span data-stu-id="15995-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="15995-163">Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant voor wie u het Autopilot-profiel hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="15995-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="15995-164">Selecteer apparaten op de detailpagina van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="15995-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="15995-165">Selecteer **onder Profielen toepassen op** apparaten de apparaten waar u het profiel uit wilt verwijderen en selecteer vervolgens Profiel **verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="15995-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="15995-166">Als u een profiel van een apparaat verwijdert, wordt het profiel niet uit de lijst verwijderd.</span><span class="sxs-lookup"><span data-stu-id="15995-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="15995-167">Als u een profiel wilt verwijderen, volgt u de instructies in [Een Autopilot-profiel](#update-or-delete-an-autopilot-profile)bijwerken of verwijderen.</span><span class="sxs-lookup"><span data-stu-id="15995-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="15995-168">Een Autopilot-profiel bijwerken of verwijderen</span><span class="sxs-lookup"><span data-stu-id="15995-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="15995-169">Als een klant de out-of-box-ervaring wil wijzigen nadat u de apparaten naar hen hebt verzonden, kunt u het profiel wijzigen in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15995-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="15995-170">Wanneer het apparaat van de klant verbinding maakt met internet, wordt de meest recente profielversie gedownload tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="15995-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="15995-171">Steeds als een klant de fabrieksinstellingen van een apparaat herstelt, downloadt het apparaat opnieuw de meest recente profielversie tijdens het OOBE-proces.</span><span class="sxs-lookup"><span data-stu-id="15995-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="15995-172">Selecteer **Klanten** in Partner Center menu en selecteer vervolgens de klant die u een Autopilot-profiel wilt laten wijzigen.</span><span class="sxs-lookup"><span data-stu-id="15995-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="15995-173">Selecteer apparaten op de detailpagina van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="15995-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="15995-174">Selecteer **Windows Autopilot profielen** het profiel dat u wilt bijwerken.</span><span class="sxs-lookup"><span data-stu-id="15995-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="15995-175">Maak de vereiste wijzigingen en selecteer vervolgens **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="15995-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="15995-176">Als u dit profiel wilt verwijderen, **selecteert u** Profiel verwijderen in de rechterbovenhoek van de pagina.</span><span class="sxs-lookup"><span data-stu-id="15995-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="15995-177">Apparaten aan de account van een klant toevoegen</span><span class="sxs-lookup"><span data-stu-id="15995-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="15995-178">Verkoopmedewerkers en beheerdersagenten kunnen apparaten toevoegen aan het account van een klant.</span><span class="sxs-lookup"><span data-stu-id="15995-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="15995-179">Voordat u aangepaste Autopilot-profielen kunt toepassen op apparaten van klanten, moet u toegang hebben tot de apparatenlijst van de klant.</span><span class="sxs-lookup"><span data-stu-id="15995-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="15995-180">Als u van plan bent om de combinatie van OEM-naam, serienummer en model te gebruiken, moet u rekening houden met de volgende beperkingen:</span><span class="sxs-lookup"><span data-stu-id="15995-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="15995-181">Deze tuple werkt alleen voor nieuwere apparaten (bijvoorbeeld 4.000 hashes) en wordt niet ondersteund voor 128b-hashes (RS2 en eerdere apparaten).</span><span class="sxs-lookup"><span data-stu-id="15995-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="15995-182">De tuple-registratie is casegevoelig, dus de gegevens in  het bestand moeten exact overeenkomen met de namen van het model en de fabrikant, zoals opgegeven door de OEM-provider (hardwareprovider).</span><span class="sxs-lookup"><span data-stu-id="15995-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="15995-183">Volg de onderstaande instructies om apparaten toe te voegen aan het account van een klant in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15995-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="15995-184">Selecteer **Klanten** in Partner Center menu en selecteer vervolgens de klant van wie u de apparaten wilt beheren.</span><span class="sxs-lookup"><span data-stu-id="15995-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="15995-185">Selecteer apparaten op de detailpagina van **de klant.**</span><span class="sxs-lookup"><span data-stu-id="15995-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="15995-186">Selecteer **onder Profielen toepassen op apparaten** de optie Apparaten **toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="15995-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="15995-187">Voer een naam in voor de apparatenlijst en selecteer vervolgens **Bladeren** om de lijst van de klant (in CSV-bestandsindeling) te uploaden naar Partner Center.</span><span class="sxs-lookup"><span data-stu-id="15995-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="15995-188">U zou dit CSV-bestand moeten hebben ontvangen bij de aankoop van uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="15995-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="15995-189">Als u geen CSV-bestand hebt ontvangen, kunt u er zelf een maken door de stappen te volgen in Apparaten [toevoegen aan Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="15995-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="15995-190">Upload het CSV-bestand en selecteer **opslaan.**</span><span class="sxs-lookup"><span data-stu-id="15995-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="15995-191">Als u een foutbericht krijgt terwijl u probeert het .csv-bestand te uploaden, moet u de bestandsindeling controleren.</span><span class="sxs-lookup"><span data-stu-id="15995-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="15995-192">U kunt alleen de hardwarehash gebruiken, of de OEM-naam, het serienummer en het model (in die kolomvolgorde) of de Windows-product-id.</span><span class="sxs-lookup"><span data-stu-id="15995-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="15995-193">U kunt ook het CSV-voorbeeldbestand van de koppeling naast **Apparaten toevoegen** gebruiken om een apparatenlijst te maken.</span><span class="sxs-lookup"><span data-stu-id="15995-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="15995-194">Uw CSV-bestand moet er als het volgende uitzien:</span><span class="sxs-lookup"><span data-stu-id="15995-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="15995-195">**Serienummer van apparaat,Windows-product-id,hardware-hash,fabrikantnaam,apparaatmodel**</span><span class="sxs-lookup"><span data-stu-id="15995-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="15995-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="15995-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="15995-197">'Fabrikantnaam' en 'Apparaatmodel' zijn casegevoelig.</span><span class="sxs-lookup"><span data-stu-id="15995-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="15995-198">Als u niet weet welke waarde u moet gebruiken voor Fabrikantnaam en Apparaatmodel, kunt u dit op het apparaat uitvoeren om de juiste waarden te verzamelen:</span><span class="sxs-lookup"><span data-stu-id="15995-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="15995-199">Windows Autopilot EULA-afwijzing</span><span class="sxs-lookup"><span data-stu-id="15995-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="15995-200">BELANGRIJKE INFORMATIE</span><span class="sxs-lookup"><span data-stu-id="15995-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="15995-201">Windows Autopilot kunt u aangepaste installaties van Windows configureren op apparaten die u voor uw klanten beheert.</span><span class="sxs-lookup"><span data-stu-id="15995-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="15995-202">Als de klant gemachtigd is om dit te doen, kunt u bepaalde instelschermen onderdrukken of verbergen die normaal gesproken aan gebruikers worden gepresenteerd bij het instellen van Windows, met inbegrip van het acceptatiescherm voor de gebruikersinterface (gebruikslicentieovereenkomst).</span><span class="sxs-lookup"><span data-stu-id="15995-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="15995-203">Met deze functie gaat u ermee akkoord dat het onderdrukken of verbergen van schermen die zijn ontworpen om gebruikers kennisgeving te geven of de voorwaarden te accepteren, betekent dat u voldoende toestemming en autorisatie van uw klant hebt verkregen om voorwaarden te verbergen, en dat u namens uw klant (of het nu een organisatie of een afzonderlijke gebruiker is, zoals het geval is), toestemming hebt verkregen voor kennisgevingen en alle voorwaarden accepteert die van toepassing zijn op uw klant.</span><span class="sxs-lookup"><span data-stu-id="15995-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="15995-204">Dit omvat overeenkomst met de voorwaarden van de licentie of kennisgeving die aan de gebruiker zou worden gepresenteerd als u deze niet onderdrukt of verbergt met behulp van dit hulpprogramma.</span><span class="sxs-lookup"><span data-stu-id="15995-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="15995-205">Uw klant mag de Windows-software op deze apparaten niet gebruiken als de klant geen geldige licentie voor de software heeft verkregen van Microsoft of zijn gelicentieerde distributeurs.</span><span class="sxs-lookup"><span data-stu-id="15995-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>