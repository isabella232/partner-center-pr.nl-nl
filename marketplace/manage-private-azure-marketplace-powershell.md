---
title: 'Quickstart: Een privé-Azure Marketplace met PowerShell'
description: In deze quickstart ziet u hoe u aanbiedingen in een privé-Azure Marketplace beheert met Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.service: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d7bd790eab2618822dbc5099ad1ad107794c82d2
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123936879"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>Quickstart: Een privé-Azure Marketplace met PowerShell

In dit artikel wordt beschreven hoe u aanbiedingen in een privé-Azure Marketplace met behulp van de PowerShell-module [Az.Marketplace.](/powershell/module/az.marketplace)

> [!IMPORTANT]
> Privé Azure Marketplace versie is momenteel beschikbaar als openbare preview. Deze preview-versie wordt geleverd zonder Service Level Agreement. Dit wordt niet aanbevolen voor productieworkloads. Sommige functies worden mogelijk niet ondersteund of hebben beperkte mogelijkheden. Zie [Supplemental Terms of Use for Microsoft Azure Previews (Aanvullende gebruiksvoorwaarden voor Microsoft Azure-previews)](https://azure.microsoft.com/support/legal/preview-supplemental-terms/) voor meer informatie.

## <a name="requirements"></a>Vereisten

* Als u nog geen Azure-abonnement hebt, maakt u een [gratis account](https://azure.microsoft.com/free/) voordat u begint.

* Als u ervoor kiest om Azure PowerShell lokaal te gebruiken:
  * [Installeer de PowerShell-module](/powershell/azure/install-az-ps).
  * Maak verbinding met uw Azure-account met de cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).
* Als u ervoor kiest om Azure Cloud Shell te gebruiken:
  * Raadpleeg [Overzicht van Azure Cloud Shell](/azure/cloud-shell/overview) voor meer informatie.

  > [!IMPORTANT]
  > Hoewel de **PowerShell-module Az.Marketplace** in preview is, moet u deze afzonderlijk installeren met behulp van de `Install-Module` cmdlet . Nadat de PowerShell-module algemeen beschikbaar is geworden, wordt deze onderdeel van toekomstige releases van de Az PowerShell-module en is deze standaard beschikbaar vanuit Azure Cloud Shell.

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* Als u meerdere Azure-abonnementen hebt, kiest u het juiste abonnement waarin de resource moet worden gefactureerd. Selecteer een specifiek abonnement met de cmdlet [set-AzContext](/powershell/module/az.accounts/set-azcontext).

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>Een lijst met persoonlijke winkels maken

Als u een lijst met persoonlijke winkels wilt ophalen, gebruikt u de cmdlet [Get-AzMarketplacePrivateStore.](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) In het volgende voorbeeld worden persoonlijke winkels vermeld die zijn gemaakt onder het tenantbereik.

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

## <a name="add-an-offer-to-a-private-marketplace"></a>Een aanbieding toevoegen aan een privé-marketplace

Als u een aanbieding wilt toevoegen aan een privé-winkel, gebruikt u de cmdlet [Set-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) In het volgende voorbeeld wordt de opgegeven aanbieding toegevoegd aan een privé-marketplace voor een privéopslag die wordt gemaakt onder het tenantbereik.

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

## <a name="get-private-store-offers"></a>Aanbiedingen voor privé-winkels downloaden

Als u een of meer aanbiedingen voor een privé-winkel wilt krijgen, gebruikt u de cmdlet [Get-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) In het volgende voorbeeld worden aanbiedingen ontvangen die zijn gekoppeld aan de opgegeven privéopslag die zijn toegevoegd onder het tenantbereik.

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

## <a name="remove-an-offer"></a>Een aanbieding verwijderen

Als u een aanbieding uit een privé-winkel wilt verwijderen, gebruikt u de cmdlet [Remove-AzMarketplacePrivateStoreOffer.](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) In het volgende voorbeeld wordt een aanbieding verwijderd uit een privé-winkel die is gemaakt in het tenantbereik.

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>Volgende stappen

[Privé-Azure Marketplace](create-manage-private-azure-marketplace.md)en beheren.