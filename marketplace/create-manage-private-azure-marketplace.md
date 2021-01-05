---
title: Privé Azure Marketplace in Azure Portal maken en beheren
description: Meer informatie over het maken en beheren van privé Azure Marketplace (preview) in de Azure Portal. Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760807"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="f267d-104">Maak en beheer privé Azure Marketplace (preview) in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="f267d-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="f267d-105">Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="f267d-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="f267d-106">Dit biedt u de mogelijkheid om alleen aanbiedingen te implementeren die u goed keuren en die voldoen aan het beleid van uw onderneming.</span><span class="sxs-lookup"><span data-stu-id="f267d-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="f267d-107">Met persoonlijke Azure Marketplace kunnen uw gebruikers de online winkel doorzoeken op compatibele aanbiedingen om deze te kopen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="f267d-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="f267d-108">Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakeld en leeg privé archief waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="f267d-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="f267d-109">In dit artikel wordt uitgelegd hoe u persoonlijke Azure Marketplace maakt, beheert en inschakelt voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="f267d-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="f267d-110">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="f267d-110">Notes:</span></span>

- <span data-ttu-id="f267d-111">De persoonlijke Azure Marketplace bevindt zich op een Tenant niveau, zodat alle gebruikers onder de Tenant dezelfde gehoste lijst zien.</span><span class="sxs-lookup"><span data-stu-id="f267d-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="f267d-112">Alle micro soft-oplossingen worden automatisch toegevoegd aan de persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f267d-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="f267d-113">De rol Marketplace-beheerder toewijzen</span><span class="sxs-lookup"><span data-stu-id="f267d-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="f267d-114">De globale beheerder van de Tenant moet de rol **Marketplace** -beheerder toewijzen aan de persoonlijke Azure Marketplace-beheerder die het privé archief gaat beheren.</span><span class="sxs-lookup"><span data-stu-id="f267d-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="f267d-115">Toegang tot persoonlijk Azure Marketplace-beheer is alleen beschikbaar voor IT-beheerders waaraan de rol Marketplace-beheerder is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="f267d-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="f267d-116">Vereisten</span><span class="sxs-lookup"><span data-stu-id="f267d-116">Prerequisites</span></span>

<span data-ttu-id="f267d-117">U moet aan deze vereisten voldoen voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het Tenant bereik:</span><span class="sxs-lookup"><span data-stu-id="f267d-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="f267d-118">U hebt toegang tot een **globale beheerders** gebruiker.</span><span class="sxs-lookup"><span data-stu-id="f267d-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="f267d-119">De Tenant heeft ten minste één abonnement (kan elk wille keurig type zijn).</span><span class="sxs-lookup"><span data-stu-id="f267d-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="f267d-120">De gebruiker van de globale beheerder krijgt de rol **Inzender** of hoger voor het gekozen abonnement.</span><span class="sxs-lookup"><span data-stu-id="f267d-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="f267d-121">De rol Marketplace-beheerder toewijzen met IAM</span><span class="sxs-lookup"><span data-stu-id="f267d-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="f267d-122">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f267d-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="f267d-123">Selecteer **alle services** en vervolgens **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="f267d-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hoofd venster.":::

3. <span data-ttu-id="f267d-125">Selecteer **privé Marketplace** in de opties aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="f267d-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="f267d-126">Selecteer **toegangs beheer (IAM)** om de rol Marketplace-beheerder toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="f267d-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Toegangs beheer scherm van IAM.":::

1. <span data-ttu-id="f267d-128">Selecteer **+ Toevoegen** > **Roltoewijzing toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="f267d-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="f267d-129">Kies onder **rol** **Marketplace-beheerder**.</span><span class="sxs-lookup"><span data-stu-id="f267d-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Menu functie toewijzing.":::

1. <span data-ttu-id="f267d-131">Selecteer de gewenste gebruiker in de vervolg keuzelijst en selecteer vervolgens **gereed**.</span><span class="sxs-lookup"><span data-stu-id="f267d-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="f267d-132">De rol Marketplace-beheerder toewijzen met Power shell</span><span class="sxs-lookup"><span data-stu-id="f267d-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="f267d-133">Gebruik het volgende Power shell-script om de rol Marketplace-beheerder toe te wijzen. hiervoor zijn de volgende para meters vereist:</span><span class="sxs-lookup"><span data-stu-id="f267d-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="f267d-134">**TenantId:** De ID van de Tenant in het bereik (de rol Marketplace-beheerder kan worden toegewezen aan het Tenant bereik).</span><span class="sxs-lookup"><span data-stu-id="f267d-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="f267d-135">**SubscriptionId:** Een abonnement waarvan de globale beheerder **een rol of** een hogere toewijzing heeft.</span><span class="sxs-lookup"><span data-stu-id="f267d-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="f267d-136">**GlobalAdminUsername:** De gebruikers naam van de globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="f267d-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="f267d-137">**UsernameToAssignRoleFor:** De gebruikers naam waaraan de rol voor Marketplace-beheerder wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="f267d-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="f267d-138">Gast gebruikers die zijn uitgenodigd voor de Tenant, kunnen tot 48 uur duren totdat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder.</span><span class="sxs-lookup"><span data-stu-id="f267d-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="f267d-139">Zie [Eigenschappen van een Azure Active Directory B2B-samenwerkings gebruiker](/azure/active-directory/b2b/user-properties)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f267d-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="f267d-140">Voor meer informatie over de cmdlets in de Power shell-module AZ. Portal, Zie [Microsoft Azure PowerShell: Portal-dash board-cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="f267d-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="f267d-141">Een persoonlijke Azure Marketplace maken</span><span class="sxs-lookup"><span data-stu-id="f267d-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="f267d-142">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="f267d-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f267d-143">Selecteer **alle services** en vervolgens **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="f267d-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hoofd venster.":::

3. <span data-ttu-id="f267d-145">Selecteer **privé Marketplace** in de opties aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="f267d-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecteer privé Marketplace in het hoofd venster van Azure Portal.":::

4. <span data-ttu-id="f267d-147">Selecteer aan de **slag** om een persoonlijke Azure Marketplace te maken (u hoeft dit slechts één keer te doen).</span><span class="sxs-lookup"><span data-stu-id="f267d-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecteer aan de slag in het hoofd venster van de Azure Portal.":::

    <span data-ttu-id="f267d-149">Als er al een persoonlijke Azure Marketplace bestaat voor deze Tenant, wordt het **beheren van Marketplace** standaard geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="f267d-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="f267d-150">Zodra u klaar bent, hebt u een lege en uitgeschakelde persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f267d-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Het lege persoonlijke venster voor Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="f267d-152">Items uit de galerie toevoegen</span><span class="sxs-lookup"><span data-stu-id="f267d-152">Add items from gallery</span></span>

<span data-ttu-id="f267d-153">Een item is een combi natie van een aanbieding en een abonnement.</span><span class="sxs-lookup"><span data-stu-id="f267d-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="f267d-154">U kunt items zoeken en toevoegen op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="f267d-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f267d-155">Selecteer **items toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="f267d-155">Select **Add items**.</span></span>

2. <span data-ttu-id="f267d-156">Blader door de **Galerie** of gebruik het zoek veld om het gewenste item te vinden.</span><span class="sxs-lookup"><span data-stu-id="f267d-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Door de galerie bladeren of het zoek veld gebruiken.":::

3. <span data-ttu-id="f267d-158">Bij het toevoegen van een nieuwe aanbieding worden standaard alle huidige plannen toegevoegd aan de lijst met toegestane abonnementen.</span><span class="sxs-lookup"><span data-stu-id="f267d-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="f267d-159">Als u de plannings selectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolg keuzelijst op de tegel van de aanbieding en werkt u de vereiste abonnementen bij.</span><span class="sxs-lookup"><span data-stu-id="f267d-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Vereiste abonnementen bijwerken.":::

4. <span data-ttu-id="f267d-161">Selecteer in de linkerbenedenhoek nadat u uw **selecties hebt gemaakt** .</span><span class="sxs-lookup"><span data-stu-id="f267d-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="f267d-162">Het **toevoegen van items** aan Marketplace is alleen beschikbaar voor aanbiedingen die niet van micro soft zijn.</span><span class="sxs-lookup"><span data-stu-id="f267d-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="f267d-163">Aanbiedingen van micro soft zijn standaard toegestaan.</span><span class="sxs-lookup"><span data-stu-id="f267d-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="f267d-164">Item plannen bewerken</span><span class="sxs-lookup"><span data-stu-id="f267d-164">Edit item plans</span></span>

<span data-ttu-id="f267d-165">U kunt de plannen van een item bewerken op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="f267d-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="f267d-166">Bekijk in de kolom **plannen** de beschik bare abonnementen in het vervolg keuzemenu voor dat item.</span><span class="sxs-lookup"><span data-stu-id="f267d-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="f267d-167">Schakel de selectie vakjes in of uit om te kiezen welke abonnementen u beschikbaar wilt maken voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="f267d-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Het selectie vakje voor het vereiste item in-of uitschakelen.":::

> [!NOTE]
> <span data-ttu-id="f267d-169">Voor elke aanbieding moet ten minste één abonnement zijn geselecteerd om de update te laten plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="f267d-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="f267d-170">Als u alle abonnementen met betrekking tot een aanbieding wilt verwijderen, verwijdert u de hele aanbieding (Zie de volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="f267d-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="f267d-171">Aanbiedingen verwijderen</span><span class="sxs-lookup"><span data-stu-id="f267d-171">Delete offers</span></span>

<span data-ttu-id="f267d-172">Schakel op de pagina Marketplace beheren het selectie vakje in naast de naam van de aanbieding (Zie het scherm hierboven) en selecteer **items verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="f267d-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="f267d-173">Privé Azure Marketplace in-/uitschakelen</span><span class="sxs-lookup"><span data-stu-id="f267d-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="f267d-174">Op de pagina Marketplace beheren ziet u een van deze banners, waarin de huidige status van de persoonlijke Azure Marketplace wordt weer gegeven:</span><span class="sxs-lookup"><span data-stu-id="f267d-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Status banner uitschakelen":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Status banner inschakelen":::

<span data-ttu-id="f267d-177">U kunt de persoonlijke Azure Marketplace zo nodig in-of uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="f267d-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="f267d-178">Als deze optie is uitgeschakeld, selecteert u **privé Marketplace inschakelen** .</span><span class="sxs-lookup"><span data-stu-id="f267d-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="f267d-179">Als deze optie is ingeschakeld, selecteert u **privé Marketplace uitschakelen** om uit te scha kelen.</span><span class="sxs-lookup"><span data-stu-id="f267d-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="f267d-180">Surfen op persoonlijke Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f267d-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="f267d-181">Wanneer persoonlijke Azure Marketplace is ingeschakeld, zien gebruikers welke abonnementen de Marketplace-beheerder heeft toegestaan.</span><span class="sxs-lookup"><span data-stu-id="f267d-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="f267d-182">Een groene, **toegestane** kennisgeving duidt op een aanbieding van een partner (niet van micro soft) die is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="f267d-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="f267d-183">Een blauwe, **toegestane** kennisgeving geeft aan dat een micro soft-aanbieding is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="f267d-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="f267d-184">Gebruikers kunnen filteren op aanbiedingen die niet zijn toegestaan:</span><span class="sxs-lookup"><span data-stu-id="f267d-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filter optie.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="f267d-186">Kopen of implementeren in een privé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="f267d-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="f267d-187">Hoewel de pagina met product details vergelijkbaar is met de open bare Azure Marketplace, zijn er drie persoonlijke Azure Marketplace-specifieke scenario's.</span><span class="sxs-lookup"><span data-stu-id="f267d-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="f267d-188">Wanneer een gebruiker een toegestaan plan selecteert, wordt de knop **maken** ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="f267d-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Span doek voor aanbiedingen er kan een plan worden gemaakt.":::

- <span data-ttu-id="f267d-190">Wanneer een gebruiker een niet-toegestaan plan selecteert, wordt er een banner notitie gemaakt dat het plan niet is toegestaan en wordt de knop **maken** uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="f267d-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner van aanbieding voor een abonnement kan niet worden gemaakt.":::

- <span data-ttu-id="f267d-192">Als een selectie van een product plan niet wordt weer gegeven op de pagina product details, maar de beheerder een of meer plannen heeft goedgekeurd, wordt een banner notities **gemaakt** waarvoor plannen zijn toegestaan en wordt de knop maken ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="f267d-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner van aanbieding waarin een plan kan worden gemaakt en de beschik bare abonnementen worden weer gegeven.":::

## <a name="contact-support"></a><span data-ttu-id="f267d-194">Contact opnemen met ondersteuning</span><span class="sxs-lookup"><span data-stu-id="f267d-194">Contact support</span></span>

<span data-ttu-id="f267d-195">Voor ondersteuning voor Azure Marketplace gaat u naar [micro soft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="f267d-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
