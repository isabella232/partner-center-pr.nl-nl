---
title: Privé-Azure Marketplace maken en beheren in Azure Portal
description: Meer informatie over het maken en beheren van Azure Marketplace privé-Azure Portal. Met Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431674"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="fa103-104">Privé-Azure Marketplace maken en beheren in Azure Portal</span><span class="sxs-lookup"><span data-stu-id="fa103-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="fa103-105">Met Azure Marketplace kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="fa103-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="fa103-106">Dit gebeurt door de gebruiker alleen aanbiedingen te laten implementeren die zijn goedgekeurd door de beheerder en voldoen aan het beleid van uw onderneming.</span><span class="sxs-lookup"><span data-stu-id="fa103-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="fa103-107">Met Private Azure Marketplace kunnen gebruikers in de online winkel zoeken naar compatibele aanbiedingen om aan te schaffen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="fa103-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="fa103-108">Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakelde en lege privéopslag waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="fa103-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="fa103-109">In dit artikel wordt uitgelegd hoe u de benodigde rol toewijst, een privé-winkel maakt, items beheert, gebruikersaanvragen goedkeurt en privé-Azure Marketplace inschakelen voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="fa103-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="fa103-110">Privé Azure Marketplace zich op tenantniveau, zodat alle gebruikers onder de tenant dezelfde gecureerde lijst zien.</span><span class="sxs-lookup"><span data-stu-id="fa103-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="fa103-111">Alle Microsoft-oplossingen (inclusief [goedgekeurde Linux-distributies)](/azure/virtual-machines/linux/endorsed-distros)worden automatisch toegevoegd aan privé-Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="fa103-112">De Marketplace-beheerdersrol toewijzen</span><span class="sxs-lookup"><span data-stu-id="fa103-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="fa103-113">De tenantbeheerder Globale beheerder de **Marketplace-beheerdersrol** toewijzen aan de Azure Marketplace private Azure Marketplace die de privéopslag gaat beheren.</span><span class="sxs-lookup"><span data-stu-id="fa103-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="fa103-114">Toegang tot Azure Marketplace is alleen beschikbaar voor IT-beheerders met de toegewezen Marketplace-beheerdersrol.</span><span class="sxs-lookup"><span data-stu-id="fa103-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="fa103-115">Vereisten</span><span class="sxs-lookup"><span data-stu-id="fa103-115">Prerequisites</span></span>

<span data-ttu-id="fa103-116">Deze vereisten zijn vereist voordat u de marketplace-beheerdersrol kunt toewijzen aan een gebruiker in het tenantbereik:</span><span class="sxs-lookup"><span data-stu-id="fa103-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="fa103-117">U hebt toegang tot een **Globale beheerder** gebruiker.</span><span class="sxs-lookup"><span data-stu-id="fa103-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="fa103-118">De tenant heeft ten minste één abonnement (elk type kan zijn).</span><span class="sxs-lookup"><span data-stu-id="fa103-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="fa103-119">Aan Globale beheerder gebruiker is de rol **Inzender** of hoger toegewezen voor het gekozen abonnement.</span><span class="sxs-lookup"><span data-stu-id="fa103-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="fa103-120">De Marketplace-beheerdersrol toewijzen met toegangsbeheer (IAM)</span><span class="sxs-lookup"><span data-stu-id="fa103-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="fa103-121">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="fa103-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="fa103-122">Selecteer **Alle services** en vervolgens **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="fa103-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="fa103-123">Selecteer **Private Marketplace** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="fa103-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="fa103-124">[![Toont de menuoptie Private Marketplace aan de linkerkant van de Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="fa103-125">Selecteer **Toegangsbeheer (IAM) om** de marketplace-beheerdersrol toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="fa103-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Geeft het scherm I A M-toegangsbeheer weer.":::

1. <span data-ttu-id="fa103-127">Selecteer **+ Toevoegen** > **Roltoewijzing toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="fa103-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="fa103-128">Kies **onder Rol** de optie **Marketplace-beheerder.**</span><span class="sxs-lookup"><span data-stu-id="fa103-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Toont het menu Roltoewijzing.":::

1. <span data-ttu-id="fa103-130">Selecteer de gewenste gebruiker in de vervolgkeuzelijst en selecteer vervolgens **Done.**</span><span class="sxs-lookup"><span data-stu-id="fa103-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="fa103-131">De Marketplace-beheerdersrol toewijzen met PowerShell</span><span class="sxs-lookup"><span data-stu-id="fa103-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="fa103-132">Gebruik het volgende PowerShell-script om de marketplace-beheerdersrol toe te wijzen; Hiervoor zijn de volgende parameters vereist:</span><span class="sxs-lookup"><span data-stu-id="fa103-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="fa103-133">**TenantId:** De id van de tenant in het bereik (de Marketplace-beheerdersrol kan worden toegewezen in het tenantbereik).</span><span class="sxs-lookup"><span data-stu-id="fa103-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="fa103-134">**SubscriptionId:** Een abonnement waaraan de globale beheerder de rol **Inzender** of hoger heeft toegewezen.</span><span class="sxs-lookup"><span data-stu-id="fa103-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="fa103-135">**GlobalAdminUsername:** De gebruikersnaam van de globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="fa103-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="fa103-136">**UsernameToAssignRoleFor:** De gebruikersnaam waaraan de Marketplace-beheerdersrol wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="fa103-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="fa103-137">Voor gastgebruikers die zijn uitgenodigd voor de tenant, kan het tot 48 uur duren voordat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder.</span><span class="sxs-lookup"><span data-stu-id="fa103-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="fa103-138">Zie Eigenschappen van een Azure Active Directory [B2B-samenwerkingsgebruiker voor meer informatie.](/azure/active-directory/b2b/user-properties)</span><span class="sxs-lookup"><span data-stu-id="fa103-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="fa103-139">Zie voor meer informatie over de cmdlets in de Az.Portal PowerShell-module [Microsoft Azure PowerShell: Portal Dashboard-cmdlets.](/powershell/module/az.portal/)</span><span class="sxs-lookup"><span data-stu-id="fa103-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="fa103-140">Privé-Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa103-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="fa103-141">Meld u aan bij de [Azure-portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="fa103-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="fa103-142">Selecteer **Alle services** en vervolgens **Marketplace.**</span><span class="sxs-lookup"><span data-stu-id="fa103-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Toont het Azure Portal hoofdvenster.":::

3. <span data-ttu-id="fa103-144">Selecteer **Private Marketplace** in het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="fa103-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="fa103-145">Selecteer **Aan de slag** om persoonlijke Azure Marketplace maken (u hoeft dit maar één keer te doen).</span><span class="sxs-lookup"><span data-stu-id="fa103-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Laat zien hoe u het hoofdvenster 'Get Started on the Azure Portal' selecteert.":::

    <span data-ttu-id="fa103-147">Als er Azure Marketplace voor deze tenant bestaat, wordt **Marketplace** beheren standaard geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="fa103-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="fa103-148">Zodra dit is voltooid, hebt u een lege en uitgeschakelde Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Hier wordt het lege scherm Azure Marketplace weergegeven.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="fa103-150">Items uit de galerie toevoegen</span><span class="sxs-lookup"><span data-stu-id="fa103-150">Add items from gallery</span></span>

<span data-ttu-id="fa103-151">Een item is een combinatie van een aanbieding en een plan.</span><span class="sxs-lookup"><span data-stu-id="fa103-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="fa103-152">U kunt items zoeken en toevoegen op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="fa103-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="fa103-153">Selecteer **Items toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="fa103-153">Select **Add items**.</span></span>

2. <span data-ttu-id="fa103-154">Blader door **de galerie** of gebruik het zoekveld om het gezochte item te vinden.</span><span class="sxs-lookup"><span data-stu-id="fa103-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="fa103-155">[![Laat zien hoe u door de galerie bladert of het zoekveld gebruikt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="fa103-156">Wanneer u een nieuwe aanbieding toevoegt, worden alle huidige abonnementen standaard toegevoegd aan de goedgekeurde lijst.</span><span class="sxs-lookup"><span data-stu-id="fa103-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="fa103-157">Als u de abonnementsselectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolgkeuzelijst in de tegel van de aanbieding en werk u de vereiste plannen bij.</span><span class="sxs-lookup"><span data-stu-id="fa103-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Laat zien hoe u de vereiste plannen bij kunt werken.":::

4. <span data-ttu-id="fa103-159">Selecteer **Klaar** linksonder nadat u uw selecties hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="fa103-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="fa103-160">**Items toevoegen** aan de Marketplace is alleen beschikbaar voor aanbiedingen die niet van Microsoft zijn.</span><span class="sxs-lookup"><span data-stu-id="fa103-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="fa103-161">Microsoft-oplossingen (inclusief [goedgekeurde Linux-distributies)](/azure/virtual-machines/linux/endorsed-distros)worden gelabeld als 'Standaard goedgekeurd' en kunnen niet worden beheerd in Private Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="fa103-162">De plannen van het item bewerken</span><span class="sxs-lookup"><span data-stu-id="fa103-162">Edit item's plans</span></span>

<span data-ttu-id="fa103-163">U kunt de abonnementen van een item bewerken op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="fa103-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="fa103-164">Bekijk in **de** kolom Plannen de beschikbare plannen in de vervolgkeuzelijst voor dat item.</span><span class="sxs-lookup"><span data-stu-id="fa103-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="fa103-165">Schakel de selectievakjes in of uit om te kiezen welke plannen beschikbaar moeten worden gesteld aan uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="fa103-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Laat zien hoe u het selectievakje voor het vereiste item in- of uitcheckt.":::

> [!NOTE]
> <span data-ttu-id="fa103-167">Voor elke aanbieding moet ten minste één abonnement zijn geselecteerd om de update uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="fa103-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="fa103-168">Als u alle abonnementen wilt verwijderen die betrekking hebben op een aanbieding, verwijdert u de hele aanbieding (zie de volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="fa103-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="fa103-169">Aanbiedingen verwijderen</span><span class="sxs-lookup"><span data-stu-id="fa103-169">Delete offers</span></span>

<span data-ttu-id="fa103-170">Schakel op de pagina Marketplace beheren het selectievakje in naast de naam van de aanbieding (zie het bovenstaande scherm) en **selecteer Items verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="fa103-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="fa103-171">Privé-Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa103-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="fa103-172">Op de pagina Marketplace beheren ziet u een van deze banners, waarop de huidige status van privé-Azure Marketplace:</span><span class="sxs-lookup"><span data-stu-id="fa103-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Geeft de banner Status uitschakelen weer.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Toont de banner Status inschakelen.":::

<span data-ttu-id="fa103-175">U kunt privé-Azure Marketplace in- of uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="fa103-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="fa103-176">Als deze optie is uitgeschakeld, **selecteert u Private Marketplace inschakelen** om in teschakelen.</span><span class="sxs-lookup"><span data-stu-id="fa103-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="fa103-177">Als deze optie is ingeschakeld, **selecteert u Private Marketplace uitschakelen om** dit uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="fa103-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="fa103-178">Meldingencentrum Azure Marketplace privé-Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa103-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="fa103-179">Meldingencentrum bestaat uit drie typen meldingen en stelt de Marketplace-beheerder in staat om acties uit te voeren op basis van de melding:</span><span class="sxs-lookup"><span data-stu-id="fa103-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="fa103-180">Goedkeuringsaanvragen van gebruikers voor items die niet in de goedgekeurde lijst staan (zie [Aanvraag om](#request-to-add-offers-or-plans) aanbiedingen of plannen toe te voegen hieronder).</span><span class="sxs-lookup"><span data-stu-id="fa103-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="fa103-181">Nieuwe abonnementsmeldingen voor aanbiedingen die al een of meer abonnementen in de goedgekeurde lijst hebben.</span><span class="sxs-lookup"><span data-stu-id="fa103-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="fa103-182">Planmeldingen verwijderd voor items die in de goedgekeurde lijst staan, maar zijn verwijderd uit de algemene Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="fa103-183">Voor toegang tot het meldingencentrum:</span><span class="sxs-lookup"><span data-stu-id="fa103-183">To access the notification center:</span></span>

1. <span data-ttu-id="fa103-184">Selecteer **Meldingen in** het menu aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="fa103-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="fa103-185">[![Geeft het menu Meldingen weer.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="fa103-186">Selecteer het beletseltekenmenu voor meer acties.</span><span class="sxs-lookup"><span data-stu-id="fa103-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Toont de meer opties menuresultaten.":::

1. <span data-ttu-id="fa103-188">Voor planaanvragen wordt **met Aanvragen tonen** het formulier voor goedkeuringsaanvragen geopend, waar u alle gebruikersaanvragen voor de specifieke aanbieding kunt controleren.</span><span class="sxs-lookup"><span data-stu-id="fa103-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="fa103-189">Selecteer **Goedkeuren** of **Afwijzen.**</span><span class="sxs-lookup"><span data-stu-id="fa103-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="fa103-190">[![Geeft de opties voor goedkeuren en afwijzen weer.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="fa103-191">Selecteer het plan dat u wilt goedkeuren in de vervolgkeuzelijst.</span><span class="sxs-lookup"><span data-stu-id="fa103-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="fa103-192">Voeg een opmerking toe en selecteer **Verzenden.**</span><span class="sxs-lookup"><span data-stu-id="fa103-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="fa103-193">Bladeren door privé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa103-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="fa103-194">Wanneer Privé Azure Marketplace is ingeschakeld, zien gebruikers welke abonnementen de Marketplace-beheerder heeft goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="fa103-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="fa103-195">Een groene **goedkeuringsbericht** geeft aan dat een partneraanbieding (niet-Microsoft) is goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="fa103-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="fa103-196">Een blauwe **goedkeuringsbericht** geeft aan dat een Microsoft-aanbieding (inclusief [goedgekeurde Linux-distributies)](/azure/virtual-machines/linux/endorsed-distros)is goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="fa103-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="fa103-197">Gebruikers kunnen filteren tussen aanbiedingen die wel en niet zijn goedgekeurd:</span><span class="sxs-lookup"><span data-stu-id="fa103-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="fa103-198">[![Toont de filteroptie.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="fa103-199">Kopen of implementeren in privé-Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="fa103-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="fa103-200">Hoewel de pagina met productdetails vergelijkbaar is met de algemene Azure Marketplace, zijn er drie privé-Azure Marketplace specifieke scenario's.</span><span class="sxs-lookup"><span data-stu-id="fa103-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="fa103-201">Wanneer een gebruiker een goedgekeurd abonnement selecteert, wordt **de knop** Maken ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="fa103-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="fa103-202">[![Toont de aanbiedingsbanner die laat zien dat er een plan kan worden gemaakt.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="fa103-203">Als de selectie van een productplan niet wordt weergegeven op de pagina met productdetails, maar de beheerder een of meer abonnementen heeft goedgekeurd, wordt in een banner weergegeven welke plannen zijn goedgekeurd en de knop Maken is ingeschakeld: </span><span class="sxs-lookup"><span data-stu-id="fa103-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="fa103-204">[![Toont de aanbiedingsbanner waarin u ziet dat er een plan kan worden gemaakt en dat er beschikbare abonnementen kunnen worden weergegeven.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="fa103-205">Wanneer een gebruiker een niet-goedgekeurd abonnement selecteert, wordt in een banner het plan als niet goedgekeurd gezien en wordt **de** knop Maken uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="fa103-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="fa103-206">De gebruiker kan nog steeds een aanvraag indienen om het plan toe te voegen aan de goedgekeurde lijst (zie de volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="fa103-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="fa103-207">Aanvraag om aanbiedingen of plannen toe te voegen</span><span class="sxs-lookup"><span data-stu-id="fa103-207">Request to add offers or plans</span></span>

<span data-ttu-id="fa103-208">U kunt een verzoek indienen om een openbare aanbieding of een openbaar abonnement toe te voegen dat momenteel niet is goedgekeurd in de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="fa103-209">Selecteer **Aanvraag om toe te voegen** in de banner om het formulier **Toegangsaanvraag te openen.**</span><span class="sxs-lookup"><span data-stu-id="fa103-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="fa103-210">[![Toont de banner met de koppeling 'Aanvraag om toe te voegen'.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="fa103-211">[![Toont het formulier voor toegangsaanvraag voor aanbiedingen of abonnementen.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="fa103-212">Selecteer welke abonnementen u wilt toevoegen aan de aanvraag ( Elk **plan** vertelt de Marketplace-beheerder dat u geen voorkeur hebt voor een plan binnen een aanbieding).</span><span class="sxs-lookup"><span data-stu-id="fa103-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="fa103-213">Voeg een Reden **toe** en selecteer **Aanvraag om** uw aanvraag in te dienen.</span><span class="sxs-lookup"><span data-stu-id="fa103-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="fa103-214">[![Toont het formulier voor toegangsaanvraag voor aanbiedingen of plannen met voorbeeldgegevens.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="fa103-215">Er wordt een indicatie voor een aanvraag in behandeling weergegeven in het formulier Toegangsaanvraag met de optie **Aanvraag intrekken.**</span><span class="sxs-lookup"><span data-stu-id="fa103-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="fa103-216">[![Toont een lijst met goedgekeurde of in behandeling zijnde plannen met de koppeling Aanvraag intrekken.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="fa103-217">Na het indienen wordt het goedkeuringsaanvraagformulier verzonden naar het meldingencentrum, waar de Marketplace-beheerder de aanvraag kan controleren en actie kan ondernemen. [](#private-azure-marketplace-notification-center)</span><span class="sxs-lookup"><span data-stu-id="fa103-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="fa103-218">Goedkeuring in Private Marketplace duidt niet op de aanschaf van een oplossing.</span><span class="sxs-lookup"><span data-stu-id="fa103-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="fa103-219">Veelgestelde vragen</span><span class="sxs-lookup"><span data-stu-id="fa103-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="fa103-220">Ik blokkeer de Marketplace-toepassing van derden al via Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="fa103-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="fa103-221">Wat is het verschil?</span><span class="sxs-lookup"><span data-stu-id="fa103-221">How is this different?</span></span>

<span data-ttu-id="fa103-222">Er zijn momenteel twee manieren om services van derden in Marketplace te beperken:</span><span class="sxs-lookup"><span data-stu-id="fa103-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="fa103-223">Schakel via de EA-portal of Azure Portal services van derden uit of beperk tot 'Alleen gratis SKU's of BYOL-SKU's'.</span><span class="sxs-lookup"><span data-stu-id="fa103-223">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Laat zien hoe u services in de Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Laat zien hoe u services kunt beperken in de E A-portal.":::

2. <span data-ttu-id="fa103-226">Maak een Azure-beleid om alleen specifieke VM's toe te staan.</span><span class="sxs-lookup"><span data-stu-id="fa103-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="fa103-227">Zie Apply policies to Windows VMs with Azure Resource Manager (Beleid toepassen op Windows-VM's met [VM'Azure Resource Manager)](/azure/virtual-machines/windows/policy)voor meer informatie over het afdwingen van beleid Azure Resource Manager.</span><span class="sxs-lookup"><span data-stu-id="fa103-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="fa103-228">Privé Azure Marketplace bieden meer flexibiliteit bij het beperken en toestaan van specifieke aanbiedingen en plannen.</span><span class="sxs-lookup"><span data-stu-id="fa103-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="fa103-229">Het informeert eindgebruikers over de beschikbaarheid voor implementatie in de Marketplace-galerie, zelfs voordat ze services van derden proberen te implementeren.</span><span class="sxs-lookup"><span data-stu-id="fa103-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="fa103-230">Als u de implementatie van services van derden wilt toestaan, stelt u Azure Marketplace in op Aan/ingeschakeld in EA Portal de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="fa103-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="fa103-231">Privé Azure Marketplace kunnen partneroplossingen cureren die niet beperkt zijn tot virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="fa103-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="fa103-232">Privé Azure Marketplace kunnen cureren op planniveau en kunnen ook 'Huidig en toekomstig plan' instellen.</span><span class="sxs-lookup"><span data-stu-id="fa103-232">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="fa103-233">Privé Azure Marketplace kunnen eindgebruikers van te voren informeren over wat wel en niet kan worden geïmplementeerd.</span><span class="sxs-lookup"><span data-stu-id="fa103-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="fa103-234">Wat is het verschil tussen een privéaanbieding en een privé-Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="fa103-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="fa103-235">Met **een privéaanbieding** kunnen uitgevers plannen maken die alleen zichtbaar zijn voor de beoogde klanten.</span><span class="sxs-lookup"><span data-stu-id="fa103-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="fa103-236">Hierdoor kunnen ze aangepaste oplossingen privé delen met overeengekomen prijzen, privévoorwaarden en gespecialiseerde configuraties.</span><span class="sxs-lookup"><span data-stu-id="fa103-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="fa103-237">Zie Privéaanbiedingen [in de commerciële marketplace voor meer informatie.](/azure/marketplace/private-offers)</span><span class="sxs-lookup"><span data-stu-id="fa103-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="fa103-238">**Met Azure Marketplace** in de Azure Portal kunnen beheerders vooraf goedkeuren welke oplossingen van derden hun gebruikers kunnen implementeren.</span><span class="sxs-lookup"><span data-stu-id="fa103-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="fa103-239">Met een privé Azure Marketplace kunnen gebruikers profiteren van de voordelen van Azure Marketplace door compatibele aanbiedingen te zoeken, te kopen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="fa103-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="fa103-240">Als u persoonlijke aanbiedingen op basis van een abonnement wilt beheren in Private Marketplace, moet de Marketplace-beheerder minimaal de rol Lezen hebben voor het specifieke abonnement.</span><span class="sxs-lookup"><span data-stu-id="fa103-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="fa103-241">Ik heb een persoonlijke aanbieding toegevoegd aan Azure Marketplace privé-Azure Marketplace waarom wordt deze niet weergegeven op het tabblad Marketplace beheren?</span><span class="sxs-lookup"><span data-stu-id="fa103-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="fa103-242">Persoonlijke aanbiedingen op basis van abonnementen zijn alleen zichtbaar voor de vermelde abonnementen in de instellingen van de persoonlijke aanbieding.</span><span class="sxs-lookup"><span data-stu-id="fa103-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="fa103-243">Als u de persoonlijke aanbieding wilt weergeven, moet u ervoor zorgen dat het globale abonnementsfilter alle abonnementen we weergeven.</span><span class="sxs-lookup"><span data-stu-id="fa103-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="fa103-244">[![Geeft het filter private marketplace weer.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="fa103-244">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="fa103-245">Kunnen we aangepaste afbeeldingen in privé-Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="fa103-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="fa103-246">Nee.</span><span class="sxs-lookup"><span data-stu-id="fa103-246">No.</span></span> <span data-ttu-id="fa103-247">Met Azure Marketplace it-beheerder kunnen oplossingen van derden beheren en cureren vanuit wereldwijde Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fa103-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="fa103-248">Omdat aangepaste afbeeldingen zich niet op globale Azure Marketplace, kan de IT-beheerder uw aangepaste afbeeldingen niet kiezen en kiezen.</span><span class="sxs-lookup"><span data-stu-id="fa103-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="fa103-249">Als u aangepaste afbeeldingen wilt delen, gebruikt u [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="fa103-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="fa103-250">Stapsgewijs handleiding Maak een Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="fa103-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="fa103-251">Maak een definitie van een afbeelding in een SIG.</span><span class="sxs-lookup"><span data-stu-id="fa103-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="fa103-252">De klant moet **Generalized kiezen** voor het veld Os-state.</span><span class="sxs-lookup"><span data-stu-id="fa103-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="fa103-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="fa103-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="fa103-254">Breng de beheerde afbeelding naar de Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="fa103-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="fa103-255">De SIG VM-afbeeldingen bevinden zich in één abonnement.</span><span class="sxs-lookup"><span data-stu-id="fa103-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="fa103-256">Als u de app beschikbaar wilt maken voor andere abonnementen, gebruikt u een app-registratie ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="fa103-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="fa103-257">Waarom zie ik dat sommige aanbiedingen **standaard zijn goedgekeurd,** zelfs als de uitgever niet Microsoft is?</span><span class="sxs-lookup"><span data-stu-id="fa103-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="fa103-258">Microsoft ondersteunt Linux en opensource-technologie in Azure.</span><span class="sxs-lookup"><span data-stu-id="fa103-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="fa103-259">[Goedgekeurde Linux-distributies](/azure/virtual-machines/linux/endorsed-distros) worden ondersteund in Azure en de prijs is geïntegreerd in virtuele machines.</span><span class="sxs-lookup"><span data-stu-id="fa103-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="fa103-260">Omdat Azure Linux Agent al vooraf is geïnstalleerd op Azure Marketplace, wordt deze behandeld als een Microsoft-aanbieding.</span><span class="sxs-lookup"><span data-stu-id="fa103-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="fa103-261">Omdat Microsoft-aanbiedingen standaard zijn goedgekeurd, kunnen goedgekeurde Linux-distributies niet worden beheerd in privé-Azure Marketplace en worden ze standaard goedgekeurd.</span><span class="sxs-lookup"><span data-stu-id="fa103-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="fa103-262">Contact opnemen met ondersteuning</span><span class="sxs-lookup"><span data-stu-id="fa103-262">Contact support</span></span>

- <span data-ttu-id="fa103-263">Ga Azure Marketplace Microsoft Q&A voor [meer informatie.](/answers/products/)</span><span class="sxs-lookup"><span data-stu-id="fa103-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>