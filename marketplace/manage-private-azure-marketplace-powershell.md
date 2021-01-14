---
title: 'Snelstartgids: een persoonlijke Azure Marketplace beheren met Power shell'
description: In deze Quick start ziet u hoe u aanbiedingen kunt beheren in een persoonlijke Azure Marketplace met behulp van Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182338"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="61595-103">Snelstartgids: een persoonlijke Azure Marketplace beheren met Power shell</span><span class="sxs-lookup"><span data-stu-id="61595-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="61595-104">In dit artikel wordt beschreven hoe u aanbiedingen kunt beheren in een persoonlijke Azure Marketplace met behulp van de [AZ. Marketplace](/powershell/module/az.marketplace) Power shell-module.</span><span class="sxs-lookup"><span data-stu-id="61595-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="61595-105">De persoonlijke Azure Marketplace is momenteel beschikbaar als open bare preview.</span><span class="sxs-lookup"><span data-stu-id="61595-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="61595-106">Deze preview-versie wordt geleverd zonder Service Level Agreement.</span><span class="sxs-lookup"><span data-stu-id="61595-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="61595-107">Dit wordt niet aanbevolen voor productieworkloads.</span><span class="sxs-lookup"><span data-stu-id="61595-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="61595-108">Sommige functies worden mogelijk niet ondersteund of hebben mogelijk beperkte mogelijkheden.</span><span class="sxs-lookup"><span data-stu-id="61595-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="61595-109">Zie [Supplemental Terms of Use for Microsoft Azure Previews (Aanvullende gebruiksvoorwaarden voor Microsoft Azure-previews)](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="61595-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="61595-110">Vereisten</span><span class="sxs-lookup"><span data-stu-id="61595-110">Requirements</span></span>

* <span data-ttu-id="61595-111">Als u nog geen Azure-abonnement hebt, maakt u een [gratis account](https://azure.microsoft.com/free/) voordat u begint.</span><span class="sxs-lookup"><span data-stu-id="61595-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="61595-112">Als u ervoor kiest om Azure PowerShell lokaal te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="61595-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="61595-113">[Installeer de PowerShell-module](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="61595-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="61595-114">Maak verbinding met uw Azure-account met de cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="61595-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="61595-115">Als u ervoor kiest om Azure Cloud Shell te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="61595-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="61595-116">Raadpleeg [Overzicht van Azure Cloud Shell](/azure/cloud-shell/overview) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="61595-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="61595-117">Hoewel de Power shell-module **AZ. Marketplace** in preview is, moet u deze afzonderlijk installeren met behulp van de `Install-Module` cmdlet.</span><span class="sxs-lookup"><span data-stu-id="61595-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="61595-118">Nadat de PowerShell-module algemeen beschikbaar is geworden, wordt deze onderdeel van toekomstige releases van de Az PowerShell-module en is deze standaard beschikbaar vanuit Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="61595-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="61595-119">Als u meerdere Azure-abonnementen hebt, kiest u het juiste abonnement waarin de resource moet worden gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="61595-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="61595-120">Selecteer een specifiek abonnement met de cmdlet [set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="61595-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="61595-121">Persoonlijke winkels weer geven</span><span class="sxs-lookup"><span data-stu-id="61595-121">List private stores</span></span>

<span data-ttu-id="61595-122">Als u een lijst met privé archieven wilt ophalen, gebruikt u de cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="61595-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="61595-123">In het volgende voor beeld ziet u een lijst met privé archieven die zijn gemaakt onder het Tenant bereik.</span><span class="sxs-lookup"><span data-stu-id="61595-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="61595-124">Een aanbieding toevoegen aan een privé Marketplace</span><span class="sxs-lookup"><span data-stu-id="61595-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="61595-125">Als u een aanbieding aan een privé-archief wilt toevoegen, gebruikt u de cmdlet [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="61595-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="61595-126">In het volgende voor beeld wordt het opgegeven aanbod toegevoegd aan een privé-Marketplace voor een privé-archief dat is gemaakt onder het Tenant bereik.</span><span class="sxs-lookup"><span data-stu-id="61595-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="61595-127">Aanbiedingen voor privé winkels ophalen</span><span class="sxs-lookup"><span data-stu-id="61595-127">Get private store offers</span></span>

<span data-ttu-id="61595-128">Als u een of meer aanbiedingen voor privé winkels wilt ophalen, gebruikt u de cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="61595-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="61595-129">In het volgende voor beeld worden aanbiedingen opgehaald die zijn gekoppeld aan het opgegeven privé archief die zijn toegevoegd onder het Tenant bereik.</span><span class="sxs-lookup"><span data-stu-id="61595-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="61595-130">Een aanbieding verwijderen</span><span class="sxs-lookup"><span data-stu-id="61595-130">Remove an offer</span></span>

<span data-ttu-id="61595-131">Als u een aanbieding uit een privé-archief wilt verwijderen, gebruikt u de cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="61595-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="61595-132">In het volgende voor beeld wordt een aanbieding verwijderd uit een privé-archief dat is gemaakt in het Tenant bereik.</span><span class="sxs-lookup"><span data-stu-id="61595-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="61595-133">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="61595-133">Next steps</span></span>

<span data-ttu-id="61595-134">[Persoonlijke Azure Marketplace maken en beheren](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="61595-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>