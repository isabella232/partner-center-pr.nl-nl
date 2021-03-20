---
title: Persoonlijke Azure Marketplace maken en beheren in de Azure Portal
description: Meer informatie over het maken en beheren van privé Azure Marketplace (preview) in de Azure Portal. Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8cfe0e95d1655530c9bc9d24b1efe85e6432236b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712763"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="7ed01-104">Persoonlijke Azure Marketplace maken en beheren in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="7ed01-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="7ed01-105">Met persoonlijke Azure Marketplace kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="7ed01-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="7ed01-106">Dit gebeurt door de gebruiker toe te staan alleen aanbiedingen te implementeren die zijn goedgekeurd door de beheerder en te voldoen aan het beleid van uw onderneming.</span><span class="sxs-lookup"><span data-stu-id="7ed01-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="7ed01-107">Met persoonlijke Azure Marketplace kunnen gebruikers de online winkel doorzoeken op compatibele aanbiedingen om deze te kopen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="7ed01-108">Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakeld en leeg privé archief waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="7ed01-109">In dit artikel wordt uitgelegd hoe u de vereiste rol kunt toewijzen, een privé archief kunt maken, items kunt beheren, gebruikers aanvragen kunt goed keuren en persoonlijke Azure Marketplace kunt inschakelen voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="7ed01-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="7ed01-110">De persoonlijke Azure Marketplace bevindt zich op een Tenant niveau, zodat alle gebruikers onder de Tenant dezelfde gehoste lijst zien.</span><span class="sxs-lookup"><span data-stu-id="7ed01-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="7ed01-111">Alle micro soft-oplossingen (inclusief [goedgekeurde Linux-distributies](/azure/virtual-machines/linux/endorsed-distros)) worden automatisch toegevoegd aan de persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7ed01-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="7ed01-112">De rol Marketplace-beheerder toewijzen</span><span class="sxs-lookup"><span data-stu-id="7ed01-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="7ed01-113">De globale beheerder van de Tenant moet de rol **Marketplace** -beheerder toewijzen aan de persoonlijke Azure Marketplace-beheerder die het privé archief gaat beheren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="7ed01-114">Toegang tot persoonlijk Azure Marketplace-beheer is alleen beschikbaar voor IT-beheerders waaraan de rol Marketplace-beheerder is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="7ed01-115">Vereisten</span><span class="sxs-lookup"><span data-stu-id="7ed01-115">Prerequisites</span></span>

<span data-ttu-id="7ed01-116">Deze vereisten zijn vereist voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het Tenant bereik:</span><span class="sxs-lookup"><span data-stu-id="7ed01-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="7ed01-117">U hebt toegang tot een **globale beheerders** gebruiker.</span><span class="sxs-lookup"><span data-stu-id="7ed01-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="7ed01-118">De Tenant heeft ten minste één abonnement (kan elk wille keurig type zijn).</span><span class="sxs-lookup"><span data-stu-id="7ed01-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="7ed01-119">De gebruiker van de globale beheerder krijgt de rol **Inzender** of hoger voor het gekozen abonnement.</span><span class="sxs-lookup"><span data-stu-id="7ed01-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="7ed01-120">De rol Marketplace-beheerder toewijzen met toegangs beheer (IAM)</span><span class="sxs-lookup"><span data-stu-id="7ed01-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="7ed01-121">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7ed01-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="7ed01-122">Selecteer **alle services** en vervolgens **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="7ed01-123">Selecteer **privé-Marketplace** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="7ed01-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="7ed01-124">[![Hiermee wordt de menu optie privé Marketplace weer gegeven aan de linkerkant van Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="7ed01-125">Selecteer **toegangs beheer (IAM)** om de rol Marketplace-beheerder toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Hiermee wordt het toegangscontrole scherm van de M weer gegeven.":::

1. <span data-ttu-id="7ed01-127">Selecteer **+ Toevoegen** > **Roltoewijzing toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="7ed01-128">Kies onder **rol** **Marketplace-beheerder**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Hiermee wordt het menu functie toewijzing weer gegeven.":::

1. <span data-ttu-id="7ed01-130">Selecteer de gewenste gebruiker in de vervolg keuzelijst en selecteer vervolgens **gereed**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="7ed01-131">De rol Marketplace-beheerder toewijzen met Power shell</span><span class="sxs-lookup"><span data-stu-id="7ed01-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="7ed01-132">Gebruik het volgende Power shell-script om de rol Marketplace-beheerder toe te wijzen. hiervoor zijn de volgende para meters vereist:</span><span class="sxs-lookup"><span data-stu-id="7ed01-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="7ed01-133">**TenantId:** De ID van de Tenant in het bereik (de rol Marketplace-beheerder kan worden toegewezen aan het Tenant bereik).</span><span class="sxs-lookup"><span data-stu-id="7ed01-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="7ed01-134">**SubscriptionId:** Een abonnement waarvan de globale beheerder **een rol of** een hogere toewijzing heeft.</span><span class="sxs-lookup"><span data-stu-id="7ed01-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="7ed01-135">**GlobalAdminUsername:** De gebruikers naam van de globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="7ed01-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="7ed01-136">**UsernameToAssignRoleFor:** De gebruikers naam waaraan de rol voor Marketplace-beheerder wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="7ed01-137">Gast gebruikers die zijn uitgenodigd voor de Tenant, kunnen tot 48 uur duren totdat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder.</span><span class="sxs-lookup"><span data-stu-id="7ed01-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="7ed01-138">Zie [Eigenschappen van een Azure Active Directory B2B-samenwerkings gebruiker](/azure/active-directory/b2b/user-properties)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7ed01-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="7ed01-139">Voor meer informatie over de cmdlets in de Power shell-module AZ. Portal, Zie [Microsoft Azure PowerShell: Portal-dash board-cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="7ed01-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="7ed01-140">Een persoonlijke Azure Marketplace maken</span><span class="sxs-lookup"><span data-stu-id="7ed01-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="7ed01-141">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7ed01-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="7ed01-142">Selecteer **alle services** en vervolgens **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Hiermee wordt het hoofd venster van Azure Portal weer gegeven.":::

3. <span data-ttu-id="7ed01-144">Selecteer **privé-Marketplace** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="7ed01-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="7ed01-145">Selecteer aan de **slag** om een persoonlijke Azure Marketplace te maken (u hoeft dit slechts één keer te doen).</span><span class="sxs-lookup"><span data-stu-id="7ed01-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Laat zien hoe u het hoofd venster ' aan de slag gaat met het Azure Portal ' selecteert.":::

    <span data-ttu-id="7ed01-147">Als er al een persoonlijke Azure Marketplace bestaat voor deze Tenant, wordt het **beheren van Marketplace** standaard geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="7ed01-148">Zodra u klaar bent, hebt u een lege en uitgeschakelde persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7ed01-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Toont het lege persoonlijke venster voor Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="7ed01-150">Items uit de galerie toevoegen</span><span class="sxs-lookup"><span data-stu-id="7ed01-150">Add items from gallery</span></span>

<span data-ttu-id="7ed01-151">Een item is een combi natie van een aanbieding en een abonnement.</span><span class="sxs-lookup"><span data-stu-id="7ed01-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="7ed01-152">U kunt items zoeken en toevoegen op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7ed01-153">Selecteer **items toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-153">Select **Add items**.</span></span>

2. <span data-ttu-id="7ed01-154">Blader door de **Galerie** of gebruik het zoek veld om het gewenste item te vinden.</span><span class="sxs-lookup"><span data-stu-id="7ed01-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="7ed01-155">[![Laat zien hoe u door de galerie bladert of het zoek veld gebruikt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="7ed01-156">Bij het toevoegen van een nieuwe aanbieding worden standaard alle huidige plannen toegevoegd aan de lijst met goedgekeurde abonnementen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="7ed01-157">Als u de plannings selectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolg keuzelijst op de tegel van de aanbieding en werkt u de vereiste abonnementen bij.</span><span class="sxs-lookup"><span data-stu-id="7ed01-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Laat zien hoe u de vereiste abonnementen kunt bijwerken.":::

4. <span data-ttu-id="7ed01-159">Selecteer in de linkerbenedenhoek nadat u uw **selecties hebt gemaakt** .</span><span class="sxs-lookup"><span data-stu-id="7ed01-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="7ed01-160">Het **toevoegen van items** aan Marketplace is alleen beschikbaar voor aanbiedingen die niet van micro soft zijn.</span><span class="sxs-lookup"><span data-stu-id="7ed01-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="7ed01-161">Micro soft-oplossingen (inclusief goedgekeurde [Linux-distributies](/azure/virtual-machines/linux/endorsed-distros)) worden gelabeld als ' standaard goedgekeurd ' en kunnen niet worden beheerd in een privé Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7ed01-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="7ed01-162">Plannen van items bewerken</span><span class="sxs-lookup"><span data-stu-id="7ed01-162">Edit item's plans</span></span>

<span data-ttu-id="7ed01-163">U kunt de plannen van een item bewerken op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="7ed01-164">Bekijk in de kolom **plannen** de beschik bare abonnementen in het vervolg keuzemenu voor dat item.</span><span class="sxs-lookup"><span data-stu-id="7ed01-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="7ed01-165">Schakel de selectie vakjes in of uit om te kiezen welke abonnementen u beschikbaar wilt maken voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="7ed01-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Laat zien hoe u het selectie vakje voor het vereiste item selecteert of uitschakelt.":::

> [!NOTE]
> <span data-ttu-id="7ed01-167">Voor elke aanbieding moet ten minste één plan worden geselecteerd om de update te laten plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="7ed01-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="7ed01-168">Als u alle abonnementen met betrekking tot een aanbieding wilt verwijderen, verwijdert u de hele aanbieding (Zie de volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="7ed01-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="7ed01-169">Aanbiedingen verwijderen</span><span class="sxs-lookup"><span data-stu-id="7ed01-169">Delete offers</span></span>

<span data-ttu-id="7ed01-170">Schakel op de pagina Marketplace beheren het selectie vakje in naast de naam van de aanbieding (Zie het scherm hierboven) en selecteer **items verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="7ed01-171">Privé Azure Marketplace in-/uitschakelen</span><span class="sxs-lookup"><span data-stu-id="7ed01-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="7ed01-172">Op de pagina Marketplace beheren ziet u een van deze banners, waarin de huidige status van de persoonlijke Azure Marketplace wordt weer gegeven:</span><span class="sxs-lookup"><span data-stu-id="7ed01-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Hiermee wordt de banner status uitschakelen weer gegeven.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Toont de banner status inschakelen.":::

<span data-ttu-id="7ed01-175">U kunt de persoonlijke Azure Marketplace zo nodig in-of uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="7ed01-176">Als deze optie is uitgeschakeld, selecteert u **privé Marketplace inschakelen** .</span><span class="sxs-lookup"><span data-stu-id="7ed01-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="7ed01-177">Als deze optie is ingeschakeld, selecteert u **privé Marketplace uitschakelen** om uit te scha kelen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="7ed01-178">Persoonlijk Azure Marketplace-meldingen centrum</span><span class="sxs-lookup"><span data-stu-id="7ed01-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="7ed01-179">Het meldingen centrum bestaat uit drie typen meldingen en stelt de Marketplace-beheerder in staat om acties uit te voeren op basis van de melding:</span><span class="sxs-lookup"><span data-stu-id="7ed01-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="7ed01-180">Goedkeurings aanvragen van gebruikers voor items die zich niet in de goedgekeurde lijst bevinden (Zie [aanvraag voor het toevoegen van aanbiedingen of abonnementen](#request-to-add-offers-or-plans) hieronder).</span><span class="sxs-lookup"><span data-stu-id="7ed01-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="7ed01-181">Meldingen voor nieuwe abonnementen voor aanbiedingen die al een of meer abonnementen in de goedgekeurde lijst hebben.</span><span class="sxs-lookup"><span data-stu-id="7ed01-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="7ed01-182">Er zijn plan meldingen verwijderd voor items die in de goedgekeurde lijst staan, maar die zijn verwijderd uit de wereld wijde Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7ed01-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="7ed01-183">Het meldingen centrum openen:</span><span class="sxs-lookup"><span data-stu-id="7ed01-183">To access the notification center:</span></span>

1. <span data-ttu-id="7ed01-184">Selecteer **meldingen** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="7ed01-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="7ed01-185">[![Hiermee wordt het menu meldingen weer gegeven.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="7ed01-186">Selecteer het menu met weglatings tekens voor meer acties.</span><span class="sxs-lookup"><span data-stu-id="7ed01-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Hiermee worden de resultaten van het menu meer opties weer gegeven.":::

1. <span data-ttu-id="7ed01-188">Voor aanvragen **weer geven worden aanvragen** geopend in het formulier goedkeurings aanvraag, waarin u alle gebruikers aanvragen voor de specifieke aanbieding kunt controleren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="7ed01-189">Selecteer **goed keuren** of **afwijzen**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="7ed01-190">[![Toont de opties goed keuren en afwijzen.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="7ed01-191">Selecteer het plan dat u wilt goed keuren in de vervolg keuzelijst.</span><span class="sxs-lookup"><span data-stu-id="7ed01-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="7ed01-192">Voeg een opmerking toe en selecteer **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="7ed01-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="7ed01-193">Surfen op persoonlijke Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7ed01-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="7ed01-194">Wanneer persoonlijke Azure Marketplace is ingeschakeld, zien gebruikers welke plannen de Marketplace-beheerder heeft goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="7ed01-195">Een groene **goedgekeurde** kennisgeving duidt op een aanbieding van een partner (niet van micro soft) die is goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="7ed01-196">Een blauw **goedgekeurde** kennisgeving geeft aan dat een micro soft-aanbieding (inclusief goedgekeurde [Linux-distributies](/azure/virtual-machines/linux/endorsed-distros)) wordt goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="7ed01-197">Gebruikers kunnen filteren op aanbiedingen die niet zijn goedgekeurd:</span><span class="sxs-lookup"><span data-stu-id="7ed01-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="7ed01-198">[![Hiermee wordt de filter optie weer gegeven.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="7ed01-199">Kopen of implementeren in een privé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="7ed01-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="7ed01-200">Hoewel de pagina met product details vergelijkbaar is met de wereld wijde Azure Marketplace, zijn er drie persoonlijke Azure Marketplace-scenario's.</span><span class="sxs-lookup"><span data-stu-id="7ed01-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="7ed01-201">Wanneer een gebruiker een goedgekeurd plan selecteert, wordt de knop **maken** ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="7ed01-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="7ed01-202">[![Toont de banner van de aanbieding die een plan oplevert kan worden gemaakt.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="7ed01-203">Als een selectie van een product plan niet wordt weer gegeven op de pagina met product details, maar de beheerder een of meer plannen heeft goedgekeurd, wordt een banner notities gemaakt waarvoor plannen zijn goedgekeurd en wordt de knop **maken** ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="7ed01-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="7ed01-204">[![Toont de banner van de aanbieding waarin een plan kan worden gemaakt en de beschik bare abonnementen worden weer gegeven.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="7ed01-205">Wanneer een gebruiker een niet-goedgekeurd plan selecteert, wordt in een banner het schema als niet-goedgekeurd en de knop **maken** uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="7ed01-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="7ed01-206">De gebruiker kan nog steeds aanvragen om het abonnement toe te voegen aan de lijst goedgekeurd (zie volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="7ed01-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="7ed01-207">Aanvraag om aanbiedingen of abonnementen toe te voegen</span><span class="sxs-lookup"><span data-stu-id="7ed01-207">Request to add offers or plans</span></span>

<span data-ttu-id="7ed01-208">U kunt aanvragen om een open bare aanbieding of een abonnement toe te voegen dat momenteel niet is goedgekeurd in de persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="7ed01-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="7ed01-209">Selecteer de **aanvraag die u wilt toevoegen** in de banner om het formulier voor de **toegangs aanvraag** te openen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="7ed01-210">[![Toont de banner met de koppeling aanvragen om toe te voegen.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="7ed01-211">[![Hiermee wordt het formulier voor de toegangs aanvraag voor aanbiedingen of abonnementen weer gegeven.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="7ed01-212">Selecteer welke abonnementen aan de aanvraag moeten worden toegevoegd (**elk plan** geeft aan dat de Marketplace-beheerder u geen voor keur heeft voor een abonnement binnen een aanbieding).</span><span class="sxs-lookup"><span data-stu-id="7ed01-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="7ed01-213">Voeg een **reden** toe en selecteer een **aanvraag** om uw aanvraag in te dienen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="7ed01-214">[![Toont het formulier voor de toegangs aanvraag voor aanbiedingen of abonnementen met voorbeeld vermeldingen.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="7ed01-215">Een vermelding voor een aanvraag in behandeling wordt weer gegeven in het formulier voor de toegangs aanvraag met een optie voor het **intrekken** van de aanvraag.</span><span class="sxs-lookup"><span data-stu-id="7ed01-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="7ed01-216">[![Toont een lijst met goedgekeurde of in behandeling zijnde plannen met de koppeling voor het intrekken van aanvragen.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="7ed01-217">Zodra de aanvraag is verzonden, wordt het goedkeurings aanvraag formulier verzonden naar het [meldingen centrum](#private-azure-marketplace-notification-center) om de Marketplace-beheerder te controleren en actie te ondernemen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="7ed01-218">Veelgestelde vragen (FAQ)</span><span class="sxs-lookup"><span data-stu-id="7ed01-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="7ed01-219">Ik heb Marketplace van derden al geblokkeerd via Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="7ed01-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="7ed01-220">Wat is het verschil?</span><span class="sxs-lookup"><span data-stu-id="7ed01-220">How is this different?</span></span>

<span data-ttu-id="7ed01-221">Er zijn momenteel twee manieren om services van derden te beperken in Marketplace:</span><span class="sxs-lookup"><span data-stu-id="7ed01-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="7ed01-222">Via EA portal of de Azure Portal kunt u services van derden uitschakelen of beperken tot ' gratis of BYOL Sku's '.</span><span class="sxs-lookup"><span data-stu-id="7ed01-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Laat zien hoe u services beperkt in de Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Laat zien hoe u services beperkt in de E-Portal.":::

2. <span data-ttu-id="7ed01-225">Maak een Azure-beleid om alleen specifieke Vm's toe te staan.</span><span class="sxs-lookup"><span data-stu-id="7ed01-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="7ed01-226">Zie [beleid Toep assen op Windows-vm's met Azure Resource Manager](/azure/virtual-machines/windows/policy)voor meer informatie over het afdwingen van beleid voor Windows-vm's.</span><span class="sxs-lookup"><span data-stu-id="7ed01-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="7ed01-227">Met persoonlijke Azure Marketplace kunt u meer flexibiliteit bieden bij het beperken en toestaan van specifieke aanbiedingen en abonnementen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="7ed01-228">Het informeert eind gebruikers over de beschik baarheid voor implementatie in de Marketplace-galerie, zelfs voordat ze proberen services van derden te implementeren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="7ed01-229">Als u de implementatie van services van derden wilt toestaan, stelt u Azure Marketplace in op aan/ingeschakeld in EA-Portal en de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7ed01-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="7ed01-230">Persoonlijke Azure Marketplace kan worden toegepast op partner oplossingen die niet beperkt zijn tot virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="7ed01-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="7ed01-231">De persoonlijke Azure Marketplace kan worden opworpen op plan niveau en kan ook het huidige en toekomstige abonnement instellen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="7ed01-232">Persoonlijke Azure Marketplace kan de eind gebruikers op de hoogte stellen van de voor delen van en kunnen niet worden geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="7ed01-233">Wat is het verschil tussen een privé-aanbieding en een persoonlijke Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="7ed01-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="7ed01-234">Met een **persoonlijke aanbieding** kunnen uitgevers plannen maken die alleen zichtbaar zijn voor doel klanten.</span><span class="sxs-lookup"><span data-stu-id="7ed01-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="7ed01-235">Hierdoor kunnen ze persoonlijke oplossingen delen met de overeengekomen prijzen, persoonlijke voor waarden en gespecialiseerde configuraties.</span><span class="sxs-lookup"><span data-stu-id="7ed01-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="7ed01-236">Zie voor meer informatie [persoonlijke aanbiedingen in de commerciële Marketplace](/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="7ed01-236">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="7ed01-237">Met de **persoonlijke Azure Marketplace** in de Azure portal kunnen beheerders vooraf goed keuren welke oplossingen van derden hun gebruikers kunnen implementeren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="7ed01-238">Met een persoonlijke Azure Marketplace kunnen gebruikers profiteren van de voor delen van Azure Marketplace door compatibele aanbiedingen te zoeken, te kopen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="7ed01-239">Voor het beheren van privé aanbiedingen op basis van een abonnement in een privé-Marketplace moet de Marketplace-beheerder beschikken over een minimale rol ' lezen ' voor het specifieke abonnement.</span><span class="sxs-lookup"><span data-stu-id="7ed01-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="7ed01-240">Ik heb een persoonlijke aanbieding aan de persoonlijke Azure Marketplace toegevoegd, waarom wordt deze niet weer gegeven op het tabblad Marketplace beheren?</span><span class="sxs-lookup"><span data-stu-id="7ed01-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="7ed01-241">Privé aanbiedingen op basis van een abonnement zijn alleen zichtbaar voor de vermelde abonnementen in de instellingen van de persoonlijke aanbieding.</span><span class="sxs-lookup"><span data-stu-id="7ed01-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="7ed01-242">Als u de persoonlijke aanbieding wilt weer geven, moet u ervoor zorgen dat het wereld wijde abonnements filter alle abonnementen weergeeft.</span><span class="sxs-lookup"><span data-stu-id="7ed01-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="7ed01-243">[![Hiermee wordt het filter voor privé Marketplace weer gegeven.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="7ed01-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="7ed01-244">Kunnen we aangepaste installatie kopieën in de persoonlijke Azure Marketplace gebruiken?</span><span class="sxs-lookup"><span data-stu-id="7ed01-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="7ed01-245">Nee.</span><span class="sxs-lookup"><span data-stu-id="7ed01-245">No.</span></span> <span data-ttu-id="7ed01-246">Met persoonlijke Azure Marketplace kan elke IT-beheerder oplossingen van derden van wereld wijde Azure Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="7ed01-247">Aangezien aangepaste installatie kopieën zich niet op de wereld wijde Azure Marketplace bevinden, kan de IT-beheerder geen aangepaste installatie kopieën kiezen en selecteren.</span><span class="sxs-lookup"><span data-stu-id="7ed01-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="7ed01-248">Als u aangepaste installatie kopieën wilt delen, gebruikt u de [Galerie voor gedeelde afbeeldingen](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="7ed01-248">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="7ed01-249">Stapsgewijze hand leiding voor het maken van een gemeen schappelijke installatie kopie galerie (SIG) ([cli](/azure/virtual-machines/shared-images-cli), [Power shell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="7ed01-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="7ed01-250">Een definitie van een installatie kopie maken binnen een SIG-bewerking.</span><span class="sxs-lookup"><span data-stu-id="7ed01-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="7ed01-251">De klant moet **gegeneraliseerd** kiezen voor het veld status van het besturings systeem.</span><span class="sxs-lookup"><span data-stu-id="7ed01-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="7ed01-252">([Cli](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [Power shell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="7ed01-252">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="7ed01-253">Een beheerde installatie kopie in de galerie met gedeelde afbeeldingen plaatsen ([cli](/azure/virtual-machines/image-version-managed-image-cli), [Power shell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="7ed01-253">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="7ed01-254">De SIG-VM-installatie kopieën bevinden zich in één abonnement.</span><span class="sxs-lookup"><span data-stu-id="7ed01-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="7ed01-255">Gebruik een app-registratie ([cli](/azure/virtual-machines/linux/share-images-across-tenants), [Power shell](/azure/virtual-machines/windows/share-images-across-tenants)) om deze beschikbaar te maken voor andere abonnementen.</span><span class="sxs-lookup"><span data-stu-id="7ed01-255">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="7ed01-256">Waarom zie ik sommige aanbiedingen **standaard goedgekeurd,** ook al is de uitgever niet van micro soft?</span><span class="sxs-lookup"><span data-stu-id="7ed01-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="7ed01-257">Micro soft ondersteunt Linux-en open-source technologie in Azure.</span><span class="sxs-lookup"><span data-stu-id="7ed01-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="7ed01-258">[Goedgekeurde Linux-distributies](/azure/virtual-machines/linux/endorsed-distros) worden ondersteund op Azure en de prijs is geïntegreerd in virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="7ed01-258">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="7ed01-259">Omdat Azure Linux agent al vooraf is geïnstalleerd op Azure Marketplace, wordt deze behandeld als een micro soft-aanbieding.</span><span class="sxs-lookup"><span data-stu-id="7ed01-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="7ed01-260">Aangezien micro soft-aanbiedingen standaard zijn goedgekeurd, kunnen goedgekeurde Linux-distributies niet worden beheerd in een privé-Azure Marketplace en standaard worden goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="7ed01-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="7ed01-261">Contact opnemen met ondersteuning</span><span class="sxs-lookup"><span data-stu-id="7ed01-261">Contact support</span></span>

- <span data-ttu-id="7ed01-262">Voor ondersteuning voor Azure Marketplace gaat u naar [micro soft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="7ed01-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>