---
title: Privé-Azure Marketplace maken en beheren in de Azure Portal
description: Meer informatie over het maken en beheren van Azure Marketplace privé-Azure Portal in de verouderde weergave. Met Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 08/10/2021
ms.openlocfilehash: da44807519f18d6aa17e41d8e81b9ad774e40d2d
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244852"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Privé-Azure Marketplace maken en beheren in de Azure Portal

> [!NOTE]
> In dit artikel worden verouderde privé-Azure Marketplace. Zie in plaats daarvan dit nieuwe artikel voor de [nieuwe weergave](create-manage-private-azure-marketplace-new.md) Verzamelingen.

Met Azure Marketplace kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken. Dit gebeurt door de gebruiker alleen aanbiedingen te laten implementeren die zijn goedgekeurd door de beheerder en die voldoen aan het beleid van uw onderneming. Met Privé Azure Marketplace kunnen gebruikers in de online winkel zoeken naar compatibele aanbiedingen om te kopen en te implementeren.

Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakelde en lege persoonlijke winkel waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen. In dit artikel wordt uitgelegd hoe u de benodigde rol toewijst, een privé-winkel maakt, items beheert, gebruikersaanvragen goedkeurt en privé-Azure Marketplace inschakelen voor uw gebruikers.

> [!NOTE]
> - Privé Azure Marketplace zich op tenantniveau, zodat alle gebruikers onder de tenant dezelfde gecureerde lijst zien.
> - Alle Microsoft-oplossingen (inclusief [goedgekeurde Linux-distributies)](/azure/virtual-machines/linux/endorsed-distros)worden automatisch toegevoegd aan Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>De Marketplace-beheerdersrol toewijzen

De tenant-Globale beheerder moet de **Marketplace-beheerdersrol** toewijzen aan de Azure Marketplace-beheerder die de privéopslag gaat beheren.

>[!IMPORTANT]
> Toegang tot Azure Marketplace is alleen beschikbaar voor IT-beheerders met de toegewezen Marketplace-beheerdersrol.

### <a name="prerequisites"></a>Vereisten

Deze vereisten zijn vereist voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het tenantbereik:

- U hebt toegang tot een **Globale beheerder** gebruiker.
- De tenant heeft ten minste één abonnement (elk type kan zijn).
- Aan Globale beheerder gebruiker is de rol **Inzender** of hoger toegewezen voor het gekozen abonnement.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>De Marketplace-beheerdersrol toewijzen met toegangsbeheer (IAM)

1. Meld u aan bij de [Azure-portal](https://portal.azure.com/).

1. Selecteer **Alle services** en vervolgens **Marketplace.**

1. Selecteer **Private Marketplace** in het menu aan de linkerkant.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Toont de menuoptie Private Marketplace aan de linkerkant van Marketplace.":::

1. Selecteer **Toegangsbeheer (IAM) om** de Marketplace-beheerdersrol toe te wijzen.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Geeft het scherm I A M-toegangsbeheer weer.":::

1. Selecteer **+ Toevoegen** > **Roltoewijzing toevoegen**.

1. Kies **onder Rol** de optie **Marketplace-beheerder.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Geeft het menu Roltoewijzing weer.":::

1. Selecteer de gewenste gebruiker in de vervolgkeuzelijst en selecteer vervolgens **Done.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>De Marketplace-beheerdersrol toewijzen met PowerShell

Gebruik het volgende PowerShell-script om de marketplace-beheerdersrol toe te wijzen; Hiervoor zijn de volgende parameters vereist:

- **TenantId:** De id van de tenant binnen het bereik (de Marketplace-beheerdersrol kan worden toegewezen in het tenantbereik).
- **SubscriptionId:** Een abonnement waaraan de globale beheerder de rol **Inzender** of hoger heeft toegewezen.
- **GlobalAdminUsername:** De gebruikersnaam van de globale beheerder.
- **UsernameToAssignRoleFor:** De gebruikersnaam waaraan de Marketplace-beheerdersrol wordt toegewezen.

> [!NOTE]
> Voor gastgebruikers die zijn uitgenodigd voor de tenant, kan het tot 48 uur duren voordat hun account beschikbaar is voor het toewijzen van de rol Marketplace-beheerder. Zie Eigenschappen van een Azure Active Directory [B2B-samenwerkingsgebruiker voor meer informatie.](/azure/active-directory/b2b/user-properties)

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

Zie voor meer informatie over de cmdlets in de PowerShell-module Az.Portal [Microsoft Azure PowerShell: Portal Dashboard-cmdlets.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Privé-Azure Marketplace

1. Meld u aan bij de [Azure-portal](https://portal.azure.com/).
2. Selecteer **Alle services** en vervolgens **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Toont het Azure Portal hoofdvenster.":::

3. Selecteer **Private Marketplace** in het menu aan de linkerkant.

4. Selecteer **Aan de slag** privé-Azure Marketplace maken (u hoeft dit maar één keer te doen).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Laat zien hoe u het hoofdvenster Aan de slag 'Azure Portal' selecteert.":::

    Als er Azure Marketplace voor deze tenant **bestaat,** wordt Marketplace beheren standaard geselecteerd.

5. Als dit is voltooid, hebt u een lege en uitgeschakelde privé Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Geeft het lege scherm Azure Marketplace weer.":::

## <a name="add-items-from-gallery"></a>Items uit galerie toevoegen

Een item is een combinatie van een aanbieding en een plan. U kunt items zoeken en toevoegen op de pagina Marketplace beheren.

1. Selecteer **Items toevoegen.**

2. Blader door **de galerie** of gebruik het zoekveld om het gezochte item te vinden.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Laat zien hoe u door de galerie bladert of het zoekveld gebruikt.":::

3. Wanneer u een nieuwe aanbieding toevoegt, worden alle huidige abonnementen standaard toegevoegd aan de lijst met goedgekeurde abonnementen. Als u de abonnementsselectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolgkeuzelijst op de tegel van de aanbieding en werk u de vereiste plannen bij.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Laat zien hoe u de vereiste plannen bij kunt werken.":::

4. Selecteer **Linksonder,** nadat u uw selecties hebt gemaakt, de optie Done.

>[!Note]
> **Items toevoegen** aan de Marketplace is alleen beschikbaar voor aanbiedingen die niet van Microsoft zijn. Microsoft-oplossingen (inclusief [goedgekeurde Linux-distributies](/azure/virtual-machines/linux/endorsed-distros)) worden gelabeld als 'Standaard goedgekeurd' en kunnen niet worden beheerd in Private Marketplace.

## <a name="edit-items-plans"></a>De abonnementen van het item bewerken

U kunt de abonnementen van een item bewerken op de pagina Marketplace beheren.

1. Bekijk in **de** kolom Plannen de beschikbare plannen in de vervolgkeuzelijst voor dat item.

2. Schakel de selectievakjes in of uit om te kiezen welke abonnementen beschikbaar moeten worden gesteld aan uw gebruikers.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Laat zien hoe u het selectievakje voor het vereiste item in- of uitkist.":::

   > [!NOTE]
   > Voor elke aanbieding moet ten minste één abonnement zijn geselecteerd om de update uit te voeren. Als u alle abonnementen wilt verwijderen die betrekking hebben op een aanbieding, verwijdert u de hele aanbieding (zie de volgende sectie).

## <a name="delete-offers"></a>Aanbiedingen verwijderen

Schakel op de pagina Marketplace beheren het selectievakje in naast de naam van de aanbieding (zie het bovenstaande scherm) en **selecteer Items verwijderen.**

## <a name="enabledisable-private-azure-marketplace"></a>Privé-Azure Marketplace/uitschakelen

Op de pagina Marketplace beheren ziet u een van deze banners die de huidige status van privé-Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Geeft de banner Status uitschakelen weer.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Toont de banner Status inschakelen.":::

U kunt privé-Azure Marketplace in- of uitschakelen.

- Als deze optie is uitgeschakeld, **selecteert u Private Marketplace inschakelen** om in teschakelen.
- Als deze optie is ingeschakeld, **selecteert u Private Marketplace uitschakelen** om dit uit te schakelen.

## <a name="private-azure-marketplace-notification-center"></a>Meldingencentrum Azure Marketplace privé-Azure Marketplace

Meldingencentrum bestaat uit drie typen meldingen en stelt de Marketplace-beheerder in staat om acties uit te voeren op basis van de melding:

- Goedkeuringsaanvragen van gebruikers voor items die niet in de goedgekeurde lijst staan (zie [Aanvraag om aanbiedingen of plannen](#request-to-add-offers-or-plans) toe te voegen hieronder).
- Nieuwe abonnementsmeldingen voor aanbiedingen die al een of meer plannen in de goedgekeurde lijst hebben.
- Planmeldingen verwijderd voor items die in de goedgekeurde lijst staan, maar zijn verwijderd uit de algemene Azure Marketplace.

Voor toegang tot het meldingencentrum:

1. Selecteer **Meldingen in** het menu aan de linkerkant.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Geeft het menu Meldingen weer.":::

1. Selecteer het beletseltekenmenu voor meer acties.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Geeft de meer opties menuresultaten.":::

1. Voor planaanvragen wordt **met Aanvragen tonen** het formulier voor goedkeuringsaanvragen geopend, waar u alle aanvragen van gebruikers voor de specifieke aanbieding kunt controleren.
1. Selecteer **Goedkeuren** of **Afwijzen.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Toont de goedkeurings- en afwijzingsopties.":::

1. Selecteer het plan dat u wilt goedkeuren in de vervolgkeuzelijst.
1. Voeg een opmerking toe en selecteer **Verzenden.**

## <a name="browsing-private-azure-marketplace"></a>Bladeren door privé-Azure Marketplace

Wanneer Privé Azure Marketplace is ingeschakeld, zien gebruikers welke abonnementen de Marketplace-beheerder heeft goedgekeurd.

- Een groene **goedkeuringsverklaring** geeft aan dat een partneraanbieding (niet-Microsoft) is goedgekeurd.
- Een blauwe **goedkeuringsverklaring** geeft aan dat een Microsoft-aanbieding (inclusief [goedgekeurde Linux-distributies)](/azure/virtual-machines/linux/endorsed-distros)is goedgekeurd.

Gebruikers kunnen filteren tussen aanbiedingen die wel en niet zijn goedgekeurd:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Toont de filteroptie.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kopen of implementeren in privé-Azure Marketplace

Hoewel de pagina met productdetails vergelijkbaar is met de algemene Azure Marketplace, zijn er drie Azure Marketplace specifieke scenario's.

- Wanneer een gebruiker een goedgekeurd abonnement selecteert, wordt **de knop Maken** ingeschakeld:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Toont de banner van de aanbieding met de notering dat een plan kan worden gemaakt.":::

- Als de selectie van een productplan niet wordt weergegeven op de pagina met productdetails, maar de beheerder een of meer abonnementen heeft goedgekeurd, wordt in een banner weergegeven welke plannen zijn goedgekeurd en de knop Maken is ingeschakeld: 

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Toont de aanbiedingsbanner waarin wordt weergegeven dat er een plan kan worden gemaakt en dat er beschikbare abonnementen kunnen worden weergegeven.":::

- Wanneer een gebruiker een niet-goedgekeurd plan selecteert, wordt in een banner het plan als niet goedgekeurd gezien en wordt **de** knop Maken uitgeschakeld. De gebruiker kan nog steeds een aanvraag indienen om het plan toe te voegen aan de goedgekeurde lijst (zie de volgende sectie).

## <a name="request-to-add-offers-or-plans"></a>Aanvraag om aanbiedingen of plannen toe te voegen

U kunt een aanvraag indienen om een openbare aanbieding of een plan toe te voegen dat momenteel niet is goedgekeurd in de Azure Marketplace.

1. Selecteer **Aanvraag om toe te voegen** in de banner om het formulier **Toegangsaanvraag te openen.**

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Toont de banner met de koppeling 'Aanvraag om toe te voegen'.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Toont het formulier voor toegangsaanvraag voor aanbiedingen of abonnementen.":::

1. Selecteer welke abonnementen u wilt toevoegen aan de aanvraag ( Elk **plan** vertelt de Marketplace-beheerder dat u geen voorkeur hebt voor een plan binnen een aanbieding).

1. Voeg een Reden **toe** en selecteer **Aanvraag om** uw aanvraag in te dienen.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Toont het formulier voor toegangsaanvraag voor aanbiedingen of plannen met voorbeeldgegevens.":::

1. Er wordt een indicatie voor een aanvraag in behandeling weergegeven in het formulier Toegangsaanvraag met de optie **Aanvraag intrekken.**

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Toont een lijst met goedgekeurde of in behandeling zijnde plannen met de koppeling Aanvraag intrekken.":::

> [!NOTE]
> Na het indienen wordt het goedkeuringsaanvraagformulier verzonden naar het meldingencentrum, waar de Marketplace-beheerder de aanvraag kan controleren en actie kan ondernemen. [](#private-azure-marketplace-notification-center)

> [!CAUTION]
> Goedkeuring in Private Marketplace duidt niet op de aanschaf van een oplossing.

## <a name="frequently-asked-questions-faqs"></a>Veelgestelde vragen

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ik blokkeer de Marketplace-toepassing van derden al via Azure Policy. Wat is het verschil?

Er zijn momenteel twee manieren om services van derden te beperken in Marketplace:

1. Schakel via de EA-portal of Azure Portal services van derden uit of beperk deze tot 'Alleen gratis SKU's of BYOL-SKU's'.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Laat zien hoe u services in de Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Laat zien hoe u services kunt beperken in de E A-portal.":::

2. Maak een Azure-beleid om alleen specifieke VM's toe te staan. Zie Apply [policies to Windows VMs with](/azure/virtual-machines/windows/policy)Windows Azure Resource Manager (Beleid toepassen op virtuele Windows met VM's met Azure Resource Manager) voor meer informatie over het afdwingen van Azure Resource Manager.

Privé Azure Marketplace bieden meer flexibiliteit bij het beperken en toestaan van specifieke aanbiedingen en plannen. Het informeert eindgebruikers over de beschikbaarheid voor implementatie in de Marketplace-galerie, zelfs voordat ze services van derden proberen te implementeren. Als u de implementatie van services van derden wilt toestaan, stelt Azure Marketplace in op Aan/ingeschakeld in EA Portal de Azure Portal.

- Privé Azure Marketplace kunnen partneroplossingen cureren die niet beperkt zijn tot virtuele machines.
- Privé Azure Marketplace kunnen cureren op planniveau en kunnen ook 'Huidig en toekomstig plan' instellen.
- Privé Azure Marketplace kunnen de eindgebruikers van te voren informeren over wat wel en niet kan worden geïmplementeerd.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Wat is het verschil tussen een privéaanbieding en een Azure Marketplace?

Met **een privéaanbieding** kunnen uitgevers plannen maken die alleen zichtbaar zijn voor de beoogde klanten. Hierdoor kunnen ze aangepaste oplossingen privé delen met overeengekomen prijzen, privévoorwaarden en gespecialiseerde configuraties. Zie Privéaanbiedingen [in de commerciële marketplace voor meer informatie.](/azure/marketplace/private-offers)

**Met Azure Marketplace** in de Azure Portal kunnen beheerders vooraf goedkeuren welke oplossingen van derden hun gebruikers kunnen implementeren. Met een privé Azure Marketplace kunnen gebruikers profiteren van de voordelen van Azure Marketplace door compatibele aanbiedingen te zoeken, te kopen en te implementeren. Als u persoonlijke aanbiedingen op basis van abonnementen wilt beheren in Private Marketplace, moet de Marketplace-beheerder minimaal de rol Lezen hebben voor het specifieke abonnement.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Ik heb een persoonlijke aanbieding toegevoegd aan Azure Marketplace privé-Azure Marketplace waarom wordt deze niet weergegeven op het tabblad Marketplace beheren?

Persoonlijke aanbiedingen op basis van abonnementen zijn alleen zichtbaar voor de vermelde abonnementen in de instellingen van de persoonlijke aanbieding. Als u de persoonlijke aanbieding wilt weergeven, controleert u of het globale abonnementsfilter alle abonnementen we weergeven.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Geeft het filter Private Marketplace weer.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Kunnen we aangepaste afbeeldingen in privé-Azure Marketplace?

Nee. Met Azure Marketplace IT-beheerder kunnen oplossingen van derden van wereldwijde Azure Marketplace. Omdat aangepaste afbeeldingen niet wereldwijd worden Azure Marketplace, kan de IT-beheerder uw aangepaste afbeeldingen niet kiezen en kiezen. Als u aangepaste afbeeldingen wilt delen, gebruikt [u Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Stapsgewijs handleiding Een Shared Image Gallery (SIG) ([CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell) maken.](/azure/virtual-machines/shared-images-powershell)
2. Maak een definitie van een afbeelding binnen een SIG. De klant moet Ge **generaliseerd kiezen** voor het veld Os-state. ([CLI,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Beheerde afbeelding in de Shared Image Gallery ([CLI,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).
4. De SIG VM-afbeeldingen bevinden zich in één abonnement. Als u de app beschikbaar wilt maken voor andere abonnementen, gebruikt u een app-registratie[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Waarom zie ik dat sommige aanbiedingen **standaard zijn goedgekeurd,** zelfs als de uitgever niet Microsoft is?

Microsoft ondersteunt Linux en opensource-technologie in Azure. [Goedgekeurde Linux-distributies](/azure/virtual-machines/linux/endorsed-distros) worden ondersteund in Azure en de prijs is geïntegreerd in virtuele machines. Omdat Azure Linux Agent al vooraf is geïnstalleerd op Azure Marketplace, wordt deze behandeld als een Microsoft-aanbieding. Omdat Microsoft-aanbiedingen standaard zijn goedgekeurd, kunnen goedgekeurde Linux-distributies niet worden beheerd in privé-Azure Marketplace en worden ze standaard goedgekeurd.

## <a name="contact-support"></a>Contact opnemen met ondersteuning

- Ga Azure Marketplace Microsoft Q&A voor [meer informatie.](/answers/products/)