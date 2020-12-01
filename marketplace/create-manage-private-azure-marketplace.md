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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Maak en beheer privé Azure Marketplace (preview) in de Azure Portal

Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken. Dit biedt u de mogelijkheid om alleen aanbiedingen te implementeren die u goed keuren en die voldoen aan het beleid van uw onderneming. Met persoonlijke Azure Marketplace kunnen uw gebruikers de online winkel doorzoeken op compatibele aanbiedingen om deze te kopen en te implementeren. 

Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakeld en leeg privé archief waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen. In dit artikel wordt uitgelegd hoe u persoonlijke Azure Marketplace maakt, beheert en inschakelt voor uw gebruikers.

Opmerkingen:

- De persoonlijke Azure Marketplace bevindt zich op een Tenant niveau, zodat alle gebruikers onder de Tenant dezelfde gehoste lijst zien.
- Alle micro soft-oplossingen worden automatisch toegevoegd aan de persoonlijke Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>De rol Marketplace-beheerder toewijzen

De globale beheerder van de Tenant moet de rol **Marketplace** -beheerder toewijzen aan de persoonlijke Azure Marketplace-beheerder die het privé archief gaat beheren.

>[!IMPORTANT]
> Toegang tot persoonlijk Azure Marketplace-beheer is alleen beschikbaar voor IT-beheerders waaraan de rol Marketplace-beheerder is toegewezen.

### <a name="prerequisites"></a>Vereisten

U moet aan deze vereisten voldoen voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het Tenant bereik:

- U hebt toegang tot een **globale beheerders** gebruiker.
- De Tenant heeft ten minste één abonnement (kan elk wille keurig type zijn).
- De gebruiker van de globale beheerder krijgt de rol **Inzender** of hoger voor het gekozen abonnement.
- De gebruiker van de globale beheerder heeft verhoogde toegang ingesteld op **Ja** (Zie [toegang verhogen om alle Azure-abonnementen en-beheer groepen te beheren](/azure/role-based-access-control/elevate-access-global-admin)).

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>De rol Marketplace-beheerder toewijzen met Power shell

Gebruik het volgende Power shell-script om de rol Marketplace-beheerder toe te wijzen. hiervoor zijn de volgende para meters vereist:

- **TenantId:** De ID van de Tenant in het bereik (de rol Marketplace-beheerder kan worden toegewezen aan het Tenant bereik).
- **SubscriptionId:** Een abonnement waarvan de globale beheerder **een rol of** een hogere toewijzing heeft.
- **GlobalAdminUsername:** De gebruikers naam van de globale beheerder.
- **UsernameToAssignRoleFor:** De gebruikers naam waaraan de rol voor Marketplace-beheerder wordt toegewezen.

> [!NOTE]
> Gast gebruikers die zijn uitgenodigd voor de Tenant, kunnen tot 48 uur duren totdat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder. Zie [Eigenschappen van een Azure Active Directory B2B-samenwerkings gebruiker](/azure/active-directory/b2b/user-properties)voor meer informatie.

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

Voor meer informatie over de cmdlets in de Power shell-module AZ. Portal, Zie [Microsoft Azure PowerShell: Portal-dash board-cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Een persoonlijke Azure Marketplace maken

1. Meld u aan bij [Azure Portal](https://portal.azure.com/).
2. Selecteer **alle services** en vervolgens **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal hoofd venster.":::

3. Selecteer **privé Marketplace** in de opties aan de linkerkant.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Selecteer privé Marketplace in het hoofd venster van Azure Portal.":::

4. Selecteer aan de **slag** om een persoonlijke Azure Marketplace te maken (u hoeft dit slechts één keer te doen).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Selecteer aan de slag in het hoofd venster van de Azure Portal.":::

    Als er al een persoonlijke Azure Marketplace bestaat voor deze Tenant, wordt het **beheren van Marketplace** standaard geselecteerd.

5. Zodra u klaar bent, hebt u een lege en uitgeschakelde persoonlijke Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Het lege persoonlijke venster voor Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Items uit de galerie toevoegen

Een item is een combi natie van een aanbieding en een abonnement. U kunt items zoeken en toevoegen op de pagina Marketplace beheren.

1. Selecteer **items toevoegen**.

2. Blader door de **Galerie** of gebruik het zoek veld om het gewenste item te vinden.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Door de galerie bladeren of het zoek veld gebruiken.":::

3. Bij het toevoegen van een nieuwe aanbieding worden standaard alle huidige plannen toegevoegd aan de lijst met toegestane abonnementen. Als u de plannings selectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolg keuzelijst op de tegel van de aanbieding en werkt u de vereiste abonnementen bij.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Vereiste abonnementen bijwerken.":::

4. Selecteer in de linkerbenedenhoek nadat u uw **selecties hebt gemaakt** .

>[!Note]
> Het **toevoegen van items** aan Marketplace is alleen beschikbaar voor aanbiedingen die niet van micro soft zijn. Aanbiedingen van micro soft zijn standaard toegestaan.

## <a name="edit-item-plans"></a>Item plannen bewerken

U kunt de plannen van een item bewerken op de pagina Marketplace beheren.

1. Bekijk in de kolom **plannen** de beschik bare abonnementen in het vervolg keuzemenu voor dat item.
2. Schakel de selectie vakjes in of uit om te kiezen welke abonnementen u beschikbaar wilt maken voor uw gebruikers.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Het selectie vakje voor het vereiste item in-of uitschakelen.":::

> [!NOTE]
> Voor elke aanbieding moet ten minste één abonnement zijn geselecteerd om de update te laten plaatsvinden. Als u alle abonnementen met betrekking tot een aanbieding wilt verwijderen, verwijdert u de hele aanbieding (Zie de volgende sectie).

## <a name="delete-offers"></a>Aanbiedingen verwijderen

Schakel op de pagina Marketplace beheren het selectie vakje in naast de naam van de aanbieding (Zie het scherm hierboven) en selecteer **items verwijderen**.

## <a name="enabledisable-private-azure-marketplace"></a>Privé Azure Marketplace in-/uitschakelen

Op de pagina Marketplace beheren ziet u een van deze banners, waarin de huidige status van de persoonlijke Azure Marketplace wordt weer gegeven:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Status banner uitschakelen":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Status banner inschakelen":::

U kunt de persoonlijke Azure Marketplace zo nodig in-of uitschakelen.

1. Als deze optie is uitgeschakeld, selecteert u **privé Marketplace inschakelen** .
2. Als deze optie is ingeschakeld, selecteert u **privé Marketplace uitschakelen** om uit te scha kelen.

## <a name="browsing-private-azure-marketplace"></a>Surfen op persoonlijke Azure Marketplace

Wanneer persoonlijke Azure Marketplace is ingeschakeld, zien gebruikers welke abonnementen de Marketplace-beheerder heeft toegestaan.

- Een groene, **toegestane** kennisgeving duidt op een aanbieding van een partner (niet van micro soft) die is toegestaan.
- Een blauwe, **toegestane** kennisgeving geeft aan dat een micro soft-aanbieding is toegestaan.

Gebruikers kunnen filteren op aanbiedingen die niet zijn toegestaan:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Filter optie.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kopen of implementeren in een privé Azure Marketplace

Hoewel de pagina met product details vergelijkbaar is met de open bare Azure Marketplace, zijn er drie persoonlijke Azure Marketplace-specifieke scenario's.

- Wanneer een gebruiker een toegestaan plan selecteert, wordt de knop **maken** ingeschakeld:

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="Span doek voor aanbiedingen er kan een plan worden gemaakt.":::

- Wanneer een gebruiker een niet-toegestaan plan selecteert, wordt er een banner notitie gemaakt dat het plan niet is toegestaan en wordt de knop **maken** uitgeschakeld.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="Banner van aanbieding voor een abonnement kan niet worden gemaakt.":::

- Als een selectie van een product plan niet wordt weer gegeven op de pagina product details, maar de beheerder een of meer plannen heeft goedgekeurd, wordt een banner notities **gemaakt** waarvoor plannen zijn toegestaan en wordt de knop maken ingeschakeld:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="Banner van aanbieding voor een abonnement kan worden gemaakt en de beschik bare abonnementen worden weer gegeven.":::

## <a name="contact-support"></a>Contact opnemen met ondersteuning

Voor ondersteuning voor Azure Marketplace gaat u naar [micro soft Q&A](/answers/products/). 
