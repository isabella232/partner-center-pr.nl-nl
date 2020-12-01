---
title: Privé Azure Marketplace in Azure Portal maken en beheren
description: Meer informatie over het maken en beheren van privé Azure Marketplace (preview) in de Azure Portal. Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439252"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="4433c-104">Maak en beheer privé Azure Marketplace (preview) in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="4433c-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="4433c-105">Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.</span><span class="sxs-lookup"><span data-stu-id="4433c-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="4433c-106">Dit biedt u de mogelijkheid om alleen aanbiedingen te implementeren die u goed keuren en die voldoen aan het beleid van uw onderneming.</span><span class="sxs-lookup"><span data-stu-id="4433c-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="4433c-107">Met persoonlijke Azure Marketplace kunnen uw gebruikers de online winkel doorzoeken op compatibele aanbiedingen om deze te kopen en te implementeren.</span><span class="sxs-lookup"><span data-stu-id="4433c-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="4433c-108">Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakeld en leeg privé archief waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen.</span><span class="sxs-lookup"><span data-stu-id="4433c-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="4433c-109">In dit artikel wordt uitgelegd hoe u persoonlijke Azure Marketplace maakt, beheert en inschakelt voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="4433c-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="4433c-110">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="4433c-110">Notes:</span></span>

- <span data-ttu-id="4433c-111">De persoonlijke Azure Marketplace bevindt zich op een Tenant niveau, zodat alle gebruikers onder de Tenant dezelfde gehoste lijst zien.</span><span class="sxs-lookup"><span data-stu-id="4433c-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="4433c-112">Alle micro soft-oplossingen worden automatisch toegevoegd aan de persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4433c-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="4433c-113">De rol Marketplace-beheerder toewijzen</span><span class="sxs-lookup"><span data-stu-id="4433c-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="4433c-114">De globale beheerder van de Tenant moet de rol **Marketplace** -beheerder toewijzen aan de persoonlijke Azure Marketplace-beheerder die het privé archief gaat beheren.</span><span class="sxs-lookup"><span data-stu-id="4433c-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="4433c-115">Toegang tot persoonlijk Azure Marketplace-beheer is alleen beschikbaar voor IT-beheerders waaraan de rol Marketplace-beheerder is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="4433c-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4433c-116">Vereisten</span><span class="sxs-lookup"><span data-stu-id="4433c-116">Prerequisites</span></span>

<span data-ttu-id="4433c-117">U moet aan deze vereisten voldoen voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het Tenant bereik:</span><span class="sxs-lookup"><span data-stu-id="4433c-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="4433c-118">U hebt toegang tot een **globale beheerders** gebruiker.</span><span class="sxs-lookup"><span data-stu-id="4433c-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="4433c-119">De Tenant heeft ten minste één abonnement (kan elk wille keurig type zijn).</span><span class="sxs-lookup"><span data-stu-id="4433c-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="4433c-120">De gebruiker van de globale beheerder krijgt de rol **Inzender** of hoger voor het gekozen abonnement.</span><span class="sxs-lookup"><span data-stu-id="4433c-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>
- <span data-ttu-id="4433c-121">De gebruiker van de globale beheerder heeft verhoogde toegang ingesteld op **Ja** (Zie [toegang verhogen om alle Azure-abonnementen en-beheer groepen te beheren](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="4433c-121">The Global administrator user has elevated access set to **Yes** (see [Elevate access to manage all Azure subscriptions and management groups](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="4433c-122">De rol Marketplace-beheerder toewijzen met Power shell</span><span class="sxs-lookup"><span data-stu-id="4433c-122">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="4433c-123">Gebruik het volgende Power shell-script om de rol Marketplace-beheerder toe te wijzen. hiervoor zijn de volgende para meters vereist:</span><span class="sxs-lookup"><span data-stu-id="4433c-123">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="4433c-124">**TenantId:** De ID van de Tenant in het bereik (de rol Marketplace-beheerder kan worden toegewezen aan het Tenant bereik).</span><span class="sxs-lookup"><span data-stu-id="4433c-124">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="4433c-125">**SubscriptionId:** Een abonnement waarvan de globale beheerder **een rol of** een hogere toewijzing heeft.</span><span class="sxs-lookup"><span data-stu-id="4433c-125">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="4433c-126">**GlobalAdminUsername:** De gebruikers naam van de globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="4433c-126">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="4433c-127">**UsernameToAssignRoleFor:** De gebruikers naam waaraan de rol voor Marketplace-beheerder wordt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="4433c-127">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="4433c-128">Gast gebruikers die zijn uitgenodigd voor de Tenant, kunnen tot 48 uur duren totdat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder.</span><span class="sxs-lookup"><span data-stu-id="4433c-128">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="4433c-129">Zie [Eigenschappen van een Azure Active Directory B2B-samenwerkings gebruiker](/azure/active-directory/b2b/user-properties)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4433c-129">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="4433c-130">Voor meer informatie over de cmdlets in de Power shell-module AZ. Portal, Zie [Microsoft Azure PowerShell: Portal-dash board-cmdlets](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="4433c-130">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="4433c-131">Een persoonlijke Azure Marketplace maken</span><span class="sxs-lookup"><span data-stu-id="4433c-131">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="4433c-132">Meld u aan bij [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="4433c-132">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="4433c-133">Selecteer **alle services** en vervolgens **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="4433c-133">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hoofd venster.":::

3. <span data-ttu-id="4433c-135">Selecteer **privé Marketplace** in de opties aan de linkerkant.</span><span class="sxs-lookup"><span data-stu-id="4433c-135">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecteer privé Marketplace in het hoofd venster van Azure Portal.":::

4. <span data-ttu-id="4433c-137">Selecteer aan de **slag** om een persoonlijke Azure Marketplace te maken (u hoeft dit slechts één keer te doen).</span><span class="sxs-lookup"><span data-stu-id="4433c-137">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecteer aan de slag in het hoofd venster van de Azure Portal.":::

    <span data-ttu-id="4433c-139">Als er al een persoonlijke Azure Marketplace bestaat voor deze Tenant, wordt het **beheren van Marketplace** standaard geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="4433c-139">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="4433c-140">Zodra u klaar bent, hebt u een lege en uitgeschakelde persoonlijke Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="4433c-140">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Het lege persoonlijke venster voor Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="4433c-142">Items uit de galerie toevoegen</span><span class="sxs-lookup"><span data-stu-id="4433c-142">Add items from gallery</span></span>

<span data-ttu-id="4433c-143">Een item is een combi natie van een aanbieding en een abonnement.</span><span class="sxs-lookup"><span data-stu-id="4433c-143">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="4433c-144">U kunt items zoeken en toevoegen op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="4433c-144">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4433c-145">Selecteer **items toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="4433c-145">Select **Add items**.</span></span>

2. <span data-ttu-id="4433c-146">Blader door de **Galerie** of gebruik het zoek veld om het gewenste item te vinden.</span><span class="sxs-lookup"><span data-stu-id="4433c-146">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Door de galerie bladeren of het zoek veld gebruiken.":::

3. <span data-ttu-id="4433c-148">Bij het toevoegen van een nieuwe aanbieding worden standaard alle huidige plannen toegevoegd aan de lijst met toegestane abonnementen.</span><span class="sxs-lookup"><span data-stu-id="4433c-148">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="4433c-149">Als u de plannings selectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolg keuzelijst op de tegel van de aanbieding en werkt u de vereiste abonnementen bij.</span><span class="sxs-lookup"><span data-stu-id="4433c-149">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Vereiste abonnementen bijwerken.":::

4. <span data-ttu-id="4433c-151">Selecteer in de linkerbenedenhoek nadat u uw **selecties hebt gemaakt** .</span><span class="sxs-lookup"><span data-stu-id="4433c-151">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="4433c-152">Het **toevoegen van items** aan Marketplace is alleen beschikbaar voor aanbiedingen die niet van micro soft zijn.</span><span class="sxs-lookup"><span data-stu-id="4433c-152">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="4433c-153">Aanbiedingen van micro soft zijn standaard toegestaan.</span><span class="sxs-lookup"><span data-stu-id="4433c-153">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="4433c-154">Item plannen bewerken</span><span class="sxs-lookup"><span data-stu-id="4433c-154">Edit item plans</span></span>

<span data-ttu-id="4433c-155">U kunt de plannen van een item bewerken op de pagina Marketplace beheren.</span><span class="sxs-lookup"><span data-stu-id="4433c-155">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4433c-156">Bekijk in de kolom **plannen** de beschik bare abonnementen in het vervolg keuzemenu voor dat item.</span><span class="sxs-lookup"><span data-stu-id="4433c-156">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="4433c-157">Schakel de selectie vakjes in of uit om te kiezen welke abonnementen u beschikbaar wilt maken voor uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="4433c-157">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Het selectie vakje voor het vereiste item in-of uitschakelen.":::

> [!NOTE]
> <span data-ttu-id="4433c-159">Voor elke aanbieding moet ten minste één abonnement zijn geselecteerd om de update te laten plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="4433c-159">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="4433c-160">Als u alle abonnementen met betrekking tot een aanbieding wilt verwijderen, verwijdert u de hele aanbieding (Zie de volgende sectie).</span><span class="sxs-lookup"><span data-stu-id="4433c-160">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="4433c-161">Aanbiedingen verwijderen</span><span class="sxs-lookup"><span data-stu-id="4433c-161">Delete offers</span></span>

<span data-ttu-id="4433c-162">Schakel op de pagina Marketplace beheren het selectie vakje in naast de naam van de aanbieding (Zie het scherm hierboven) en selecteer **items verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="4433c-162">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="4433c-163">Privé Azure Marketplace in-/uitschakelen</span><span class="sxs-lookup"><span data-stu-id="4433c-163">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="4433c-164">Op de pagina Marketplace beheren ziet u een van deze banners, waarin de huidige status van de persoonlijke Azure Marketplace wordt weer gegeven:</span><span class="sxs-lookup"><span data-stu-id="4433c-164">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Status banner uitschakelen":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Status banner inschakelen":::

<span data-ttu-id="4433c-167">U kunt de persoonlijke Azure Marketplace zo nodig in-of uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="4433c-167">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="4433c-168">Als deze optie is uitgeschakeld, selecteert u **privé Marketplace inschakelen** .</span><span class="sxs-lookup"><span data-stu-id="4433c-168">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="4433c-169">Als deze optie is ingeschakeld, selecteert u **privé Marketplace uitschakelen** om uit te scha kelen.</span><span class="sxs-lookup"><span data-stu-id="4433c-169">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="4433c-170">Surfen op persoonlijke Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4433c-170">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="4433c-171">Wanneer persoonlijke Azure Marketplace is ingeschakeld, zien gebruikers welke abonnementen de Marketplace-beheerder heeft toegestaan.</span><span class="sxs-lookup"><span data-stu-id="4433c-171">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="4433c-172">Een groene, **toegestane** kennisgeving duidt op een aanbieding van een partner (niet van micro soft) die is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="4433c-172">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="4433c-173">Een blauwe, **toegestane** kennisgeving geeft aan dat een micro soft-aanbieding is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="4433c-173">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="4433c-174">Gebruikers kunnen filteren op aanbiedingen die niet zijn toegestaan:</span><span class="sxs-lookup"><span data-stu-id="4433c-174">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filter optie.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="4433c-176">Kopen of implementeren in een privé Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4433c-176">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="4433c-177">Hoewel de pagina met product details vergelijkbaar is met de open bare Azure Marketplace, zijn er drie persoonlijke Azure Marketplace-specifieke scenario's.</span><span class="sxs-lookup"><span data-stu-id="4433c-177">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="4433c-178">Wanneer een gebruiker een toegestaan plan selecteert, wordt de knop **maken** ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="4433c-178">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Span doek voor aanbiedingen er kan een plan worden gemaakt.":::

- <span data-ttu-id="4433c-180">Wanneer een gebruiker een niet-toegestaan plan selecteert, wordt er een banner notitie gemaakt dat het plan niet is toegestaan en wordt de knop **maken** uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="4433c-180">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner van aanbieding voor een abonnement kan niet worden gemaakt.":::

- <span data-ttu-id="4433c-182">Als een selectie van een product plan niet wordt weer gegeven op de pagina product details, maar de beheerder een of meer plannen heeft goedgekeurd, wordt een banner notities **gemaakt** waarvoor plannen zijn toegestaan en wordt de knop maken ingeschakeld:</span><span class="sxs-lookup"><span data-stu-id="4433c-182">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner van aanbieding voor een abonnement kan worden gemaakt en de beschik bare abonnementen worden weer gegeven.":::

## <a name="contact-support"></a><span data-ttu-id="4433c-184">Contact opnemen met ondersteuning</span><span class="sxs-lookup"><span data-stu-id="4433c-184">Contact support</span></span>

<span data-ttu-id="4433c-185">Voor ondersteuning voor Azure Marketplace gaat u naar [micro soft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="4433c-185">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
