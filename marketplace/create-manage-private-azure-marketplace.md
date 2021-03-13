---
title: Persoonlijke Azure Marketplace maken en beheren in de Azure Portal
description: Meer informatie over het maken en beheren van privé Azure Marketplace (preview) in de Azure Portal. Met private Azure Marketplace (preview) kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: dbd67ee1d4e9775d37318ec6389888f03a50b6ec
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412706"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Persoonlijke Azure Marketplace maken en beheren in de Azure Portal

Met persoonlijke Azure Marketplace kunnen beheerders bepalen welke oplossingen van derden hun gebruikers kunnen gebruiken. Dit gebeurt door de gebruiker toe te staan alleen aanbiedingen te implementeren die zijn goedgekeurd door de beheerder en te voldoen aan het beleid van uw onderneming. Met persoonlijke Azure Marketplace kunnen gebruikers de online winkel doorzoeken op compatibele aanbiedingen om deze te kopen en te implementeren.

Als Marketplace-beheerder (toegewezen rol) begint u met een uitgeschakeld en leeg privé archief waar u uw goedgekeurde aanbiedingen en abonnementen kunt toevoegen. In dit artikel wordt uitgelegd hoe u de vereiste rol kunt toewijzen, een privé archief kunt maken, items kunt beheren, gebruikers aanvragen kunt goed keuren en persoonlijke Azure Marketplace kunt inschakelen voor uw gebruikers.

> [!NOTE]
> - De persoonlijke Azure Marketplace bevindt zich op een Tenant niveau, zodat alle gebruikers onder de Tenant dezelfde gehoste lijst zien.
> - Alle micro soft-oplossingen (inclusief [goedgekeurde Linux-distributies](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) worden automatisch toegevoegd aan de persoonlijke Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>De rol Marketplace-beheerder toewijzen

De globale beheerder van de Tenant moet de rol **Marketplace** -beheerder toewijzen aan de persoonlijke Azure Marketplace-beheerder die het privé archief gaat beheren.

>[!IMPORTANT]
> Toegang tot persoonlijk Azure Marketplace-beheer is alleen beschikbaar voor IT-beheerders waaraan de rol Marketplace-beheerder is toegewezen.

### <a name="prerequisites"></a>Vereisten

Deze vereisten zijn vereist voordat u de rol Marketplace-beheerder kunt toewijzen aan een gebruiker in het Tenant bereik:

- U hebt toegang tot een **globale beheerders** gebruiker.
- De Tenant heeft ten minste één abonnement (kan elk wille keurig type zijn).
- De gebruiker van de globale beheerder krijgt de rol **Inzender** of hoger voor het gekozen abonnement.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>De rol Marketplace-beheerder toewijzen met toegangs beheer (IAM)

1. Meld u aan bij [Azure Portal](https://portal.azure.com/).
1. Selecteer **alle services** en vervolgens **Marketplace**.
1. Selecteer **privé-Marketplace** in het menu aan de linkerkant.

    [![Hiermee wordt de menu optie privé Marketplace weer gegeven aan de linkerkant van Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Selecteer **toegangs beheer (IAM)** om de rol Marketplace-beheerder toe te wijzen.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Hiermee wordt het toegangscontrole scherm van de M weer gegeven.":::

1. Selecteer **+ Toevoegen** > **Roltoewijzing toevoegen**.
1. Kies onder **rol** **Marketplace-beheerder**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Hiermee wordt het menu functie toewijzing weer gegeven.":::

1. Selecteer de gewenste gebruiker in de vervolg keuzelijst en selecteer vervolgens **gereed**.

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

Voor meer informatie over de cmdlets in de Power shell-module AZ. Portal, Zie [Microsoft Azure PowerShell: Portal-dash board-cmdlets](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Een persoonlijke Azure Marketplace maken

1. Meld u aan bij [Azure Portal](https://portal.azure.com/).
2. Selecteer **alle services** en vervolgens **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Hiermee wordt het hoofd venster van Azure Portal weer gegeven.":::

3. Selecteer **privé-Marketplace** in het menu aan de linkerkant.

4. Selecteer aan de **slag** om een persoonlijke Azure Marketplace te maken (u hoeft dit slechts één keer te doen).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Laat zien hoe u het hoofd venster ' aan de slag gaat met het Azure Portal ' selecteert.":::

    Als er al een persoonlijke Azure Marketplace bestaat voor deze Tenant, wordt het **beheren van Marketplace** standaard geselecteerd.

5. Zodra u klaar bent, hebt u een lege en uitgeschakelde persoonlijke Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Toont het lege persoonlijke venster voor Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Items uit de galerie toevoegen

Een item is een combi natie van een aanbieding en een abonnement. U kunt items zoeken en toevoegen op de pagina Marketplace beheren.

1. Selecteer **items toevoegen**.

2. Blader door de **Galerie** of gebruik het zoek veld om het gewenste item te vinden.

    [![Laat zien hoe u door de galerie bladert of het zoek veld gebruikt.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. Bij het toevoegen van een nieuwe aanbieding worden standaard alle huidige plannen toegevoegd aan de lijst met goedgekeurde abonnementen. Als u de plannings selectie wilt wijzigen voordat u de geselecteerde items toevoegt, selecteert u de vervolg keuzelijst op de tegel van de aanbieding en werkt u de vereiste abonnementen bij.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Laat zien hoe u de vereiste abonnementen kunt bijwerken.":::

4. Selecteer in de linkerbenedenhoek nadat u uw **selecties hebt gemaakt** .

>[!Note]
> Het **toevoegen van items** aan Marketplace is alleen beschikbaar voor aanbiedingen die niet van micro soft zijn. Micro soft-oplossingen (inclusief goedgekeurde [Linux-distributies](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) worden gelabeld als ' standaard goedgekeurd ' en kunnen niet worden beheerd in een privé Marketplace.

## <a name="edit-items-plans"></a>Plannen van items bewerken

U kunt de plannen van een item bewerken op de pagina Marketplace beheren.

1. Bekijk in de kolom **plannen** de beschik bare abonnementen in het vervolg keuzemenu voor dat item.
2. Schakel de selectie vakjes in of uit om te kiezen welke abonnementen u beschikbaar wilt maken voor uw gebruikers.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Laat zien hoe u het selectie vakje voor het vereiste item selecteert of uitschakelt.":::

> [!NOTE]
> Voor elke aanbieding moet ten minste één plan worden geselecteerd om de update te laten plaatsvinden. Als u alle abonnementen met betrekking tot een aanbieding wilt verwijderen, verwijdert u de hele aanbieding (Zie de volgende sectie).

## <a name="delete-offers"></a>Aanbiedingen verwijderen

Schakel op de pagina Marketplace beheren het selectie vakje in naast de naam van de aanbieding (Zie het scherm hierboven) en selecteer **items verwijderen**.

## <a name="enabledisable-private-azure-marketplace"></a>Privé Azure Marketplace in-/uitschakelen

Op de pagina Marketplace beheren ziet u een van deze banners, waarin de huidige status van de persoonlijke Azure Marketplace wordt weer gegeven:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Hiermee wordt de banner status uitschakelen weer gegeven.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Toont de banner status inschakelen.":::

U kunt de persoonlijke Azure Marketplace zo nodig in-of uitschakelen.

- Als deze optie is uitgeschakeld, selecteert u **privé Marketplace inschakelen** .
- Als deze optie is ingeschakeld, selecteert u **privé Marketplace uitschakelen** om uit te scha kelen.

## <a name="private-azure-marketplace-notification-center"></a>Persoonlijk Azure Marketplace-meldingen centrum

Het meldingen centrum bestaat uit drie typen meldingen en stelt de Marketplace-beheerder in staat om acties uit te voeren op basis van de melding:

- Goedkeurings aanvragen van gebruikers voor items die zich niet in de goedgekeurde lijst bevinden (Zie [aanvraag voor het toevoegen van aanbiedingen of abonnementen](#request-to-add-offers-or-plans) hieronder).
- Meldingen voor nieuwe abonnementen voor aanbiedingen die al een of meer abonnementen in de goedgekeurde lijst hebben.
- Er zijn plan meldingen verwijderd voor items die in de goedgekeurde lijst staan, maar die zijn verwijderd uit de wereld wijde Azure Marketplace.

Het meldingen centrum openen:

1. Selecteer **meldingen** in het menu aan de linkerkant.

    [![Hiermee wordt het menu meldingen weer gegeven.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Selecteer het menu met weglatings tekens voor meer acties.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Hiermee worden de resultaten van het menu meer opties weer gegeven.":::

1. Voor aanvragen **weer geven worden aanvragen** geopend in het formulier goedkeurings aanvraag, waarin u alle gebruikers aanvragen voor de specifieke aanbieding kunt controleren.
1. Selecteer **goed keuren** of **afwijzen**.

    [![Toont de opties goed keuren en afwijzen.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Selecteer het plan dat u wilt goed keuren in de vervolg keuzelijst.
1. Voeg een opmerking toe en selecteer **verzenden**.

## <a name="browsing-private-azure-marketplace"></a>Surfen op persoonlijke Azure Marketplace

Wanneer persoonlijke Azure Marketplace is ingeschakeld, zien gebruikers welke plannen de Marketplace-beheerder heeft goedgekeurd.

- Een groene **goedgekeurde** kennisgeving duidt op een aanbieding van een partner (niet van micro soft) die is goedgekeurd.
- Een blauw **goedgekeurde** kennisgeving geeft aan dat een micro soft-aanbieding (inclusief goedgekeurde [Linux-distributies](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) wordt goedgekeurd.

Gebruikers kunnen filteren op aanbiedingen die niet zijn goedgekeurd:

[![Hiermee wordt de filter optie weer gegeven.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Kopen of implementeren in een privé Azure Marketplace

Hoewel de pagina met product details vergelijkbaar is met de wereld wijde Azure Marketplace, zijn er drie persoonlijke Azure Marketplace-scenario's.

- Wanneer een gebruiker een goedgekeurd plan selecteert, wordt de knop **maken** ingeschakeld:

    [![Toont de banner van de aanbieding die een plan oplevert kan worden gemaakt.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Als een selectie van een product plan niet wordt weer gegeven op de pagina met product details, maar de beheerder een of meer plannen heeft goedgekeurd, wordt een banner notities gemaakt waarvoor plannen zijn goedgekeurd en wordt de knop **maken** ingeschakeld:

    [![Toont de banner van de aanbieding waarin een plan kan worden gemaakt en de beschik bare abonnementen worden weer gegeven.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Wanneer een gebruiker een niet-goedgekeurd plan selecteert, wordt in een banner het schema als niet-goedgekeurd en de knop **maken** uitgeschakeld. De gebruiker kan nog steeds aanvragen om het abonnement toe te voegen aan de lijst goedgekeurd (zie volgende sectie).

## <a name="request-to-add-offers-or-plans"></a>Aanvraag om aanbiedingen of abonnementen toe te voegen

U kunt aanvragen om een open bare aanbieding of een abonnement toe te voegen dat momenteel niet is goedgekeurd in de persoonlijke Azure Marketplace.

1. Selecteer de **aanvraag die u wilt toevoegen** in de banner om het formulier voor de **toegangs aanvraag** te openen.

    [![Toont de banner met de koppeling aanvragen om toe te voegen.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Hiermee wordt het formulier voor de toegangs aanvraag voor aanbiedingen of abonnementen weer gegeven.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Selecteer welke abonnementen aan de aanvraag moeten worden toegevoegd (**elk plan** geeft aan dat de Marketplace-beheerder u geen voor keur heeft voor een abonnement binnen een aanbieding).

1. Voeg een **reden** toe en selecteer een **aanvraag** om uw aanvraag in te dienen.
  
    [![Toont het formulier voor de toegangs aanvraag voor aanbiedingen of abonnementen met voorbeeld vermeldingen.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Een vermelding voor een aanvraag in behandeling wordt weer gegeven in het formulier voor de toegangs aanvraag met een optie voor het **intrekken** van de aanvraag.

    [![Toont een lijst met goedgekeurde of in behandeling zijnde plannen met de koppeling voor het intrekken van aanvragen.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Zodra de aanvraag is verzonden, wordt het goedkeurings aanvraag formulier verzonden naar het [meldingen centrum](#private-azure-marketplace-notification-center) om de Marketplace-beheerder te controleren en actie te ondernemen.

## <a name="frequently-asked-questions-faqs"></a>Veelgestelde vragen (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ik heb Marketplace van derden al geblokkeerd via Azure Policy. Wat is het verschil?

Er zijn momenteel twee manieren om services van derden te beperken in Marketplace:

1. Via EA portal of de Azure Portal kunt u services van derden uitschakelen of beperken tot ' gratis of BYOL Sku's '.

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Laat zien hoe u services beperkt in de Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Laat zien hoe u services beperkt in de E-Portal.":::

2. Maak een Azure-beleid om alleen specifieke Vm's toe te staan. Zie [beleid Toep assen op Windows-vm's met Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy)voor meer informatie over het afdwingen van beleid voor Windows-vm's.

Met persoonlijke Azure Marketplace kunt u meer flexibiliteit bieden bij het beperken en toestaan van specifieke aanbiedingen en abonnementen. Het informeert eind gebruikers over de beschik baarheid voor implementatie in de Marketplace-galerie, zelfs voordat ze proberen services van derden te implementeren. Als u de implementatie van services van derden wilt toestaan, stelt u Azure Marketplace in op aan/ingeschakeld in EA-Portal en de Azure Portal.

- Persoonlijke Azure Marketplace kan worden toegepast op partner oplossingen die niet beperkt zijn tot virtuele machines.
- De persoonlijke Azure Marketplace kan worden opworpen op plan niveau en kan ook het huidige en toekomstige abonnement instellen.
- Persoonlijke Azure Marketplace kan de eind gebruikers op de hoogte stellen van de voor delen van en kunnen niet worden geïmplementeerd.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>Wat is het verschil tussen een privé-aanbieding en een persoonlijke Azure Marketplace?

Met een **persoonlijke aanbieding** kunnen uitgevers plannen maken die alleen zichtbaar zijn voor doel klanten. Hierdoor kunnen ze persoonlijke oplossingen delen met de overeengekomen prijzen, persoonlijke voor waarden en gespecialiseerde configuraties. Zie voor meer informatie [persoonlijke aanbiedingen in de commerciële Marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).

Met de **persoonlijke Azure Marketplace** in de Azure portal kunnen beheerders vooraf goed keuren welke oplossingen van derden hun gebruikers kunnen implementeren. Met een persoonlijke Azure Marketplace kunnen gebruikers profiteren van de voor delen van Azure Marketplace door compatibele aanbiedingen te zoeken, te kopen en te implementeren. Voor het beheren van privé aanbiedingen op basis van een abonnement in een privé-Marketplace moet de Marketplace-beheerder beschikken over een minimale rol ' lezen ' voor het specifieke abonnement.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>Ik heb een persoonlijke aanbieding aan de persoonlijke Azure Marketplace toegevoegd, waarom wordt deze niet weer gegeven op het tabblad Marketplace beheren?

Privé aanbiedingen op basis van een abonnement zijn alleen zichtbaar voor de vermelde abonnementen in de instellingen van de persoonlijke aanbieding. Als u de persoonlijke aanbieding wilt weer geven, moet u ervoor zorgen dat het wereld wijde abonnements filter alle abonnementen weergeeft.

[![Hiermee wordt het filter voor privé Marketplace weer gegeven.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>Kunnen we aangepaste installatie kopieën in de persoonlijke Azure Marketplace gebruiken?

Nee. Met persoonlijke Azure Marketplace kan elke IT-beheerder oplossingen van derden van wereld wijde Azure Marketplace beheren. Aangezien aangepaste installatie kopieën zich niet op de wereld wijde Azure Marketplace bevinden, kan de IT-beheerder geen aangepaste installatie kopieën kiezen en selecteren. Als u aangepaste installatie kopieën wilt delen, gebruikt u de [Galerie voor gedeelde afbeeldingen](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).

1. Stapsgewijze hand leiding voor het maken van een gemeen schappelijke installatie kopie galerie (SIG) ([cli](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [Power shell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).
2. Een definitie van een installatie kopie maken binnen een SIG-bewerking. De klant moet **gegeneraliseerd** kiezen voor het veld status van het besturings systeem. ([Cli](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [Power shell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Een beheerde installatie kopie in de galerie met gedeelde afbeeldingen plaatsen ([cli](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [Power shell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).
4. De SIG-VM-installatie kopieën bevinden zich in één abonnement. Gebruik een app-registratie ([cli](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [Power shell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) om deze beschikbaar te maken voor andere abonnementen.

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>Waarom zie ik sommige aanbiedingen **standaard goedgekeurd,** ook al is de uitgever niet van micro soft?

Micro soft ondersteunt Linux-en open-source technologie in Azure. [Goedgekeurde Linux-distributies](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) worden ondersteund op Azure en de prijs is geïntegreerd in virtuele machines. Omdat Azure Linux agent al vooraf is geïnstalleerd op Azure Marketplace, wordt deze behandeld als een micro soft-aanbieding. Aangezien micro soft-aanbiedingen standaard zijn goedgekeurd, kunnen goedgekeurde Linux-distributies niet worden beheerd in een privé-Azure Marketplace en standaard worden goedgekeurd.

## <a name="contact-support"></a>Contact opnemen met ondersteuning

- Voor ondersteuning voor Azure Marketplace gaat u naar [micro soft Q&A](/answers/products/).
