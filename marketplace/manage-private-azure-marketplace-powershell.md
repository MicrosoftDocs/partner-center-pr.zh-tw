---
title: 快速入門：使用 PowerShell 管理私用 Azure Marketplace
description: 本快速入門說明如何使用 Azure PowerShell 管理私用 Azure Marketplace 中的供應專案。
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536075"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a>快速入門：使用 PowerShell 管理私用 Azure Marketplace

本文說明如何使用 [Az](/powershell/module/az.marketplace) PowerShell 模組來管理私用 Azure Marketplace 中的供應專案。

> [!IMPORTANT]
> 私用 Azure Marketplace 目前處於公開預覽狀態。 所提供的這個預覽版本並沒有服務等級協定。 不建議用於生產工作負載。 某些功能可能不受支援，或可能具有受限的功能。 如需詳細資訊，請參閱 [Microsoft Azure 預覽版增補使用條款](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)。

## <a name="requirements"></a>需求

* 如果您沒有 Azure 訂用帳戶，請在開始前建立[免費帳戶](https://azure.microsoft.com/free/)。

* 如果您選擇在本機使用 Azure PowerShell：
  * [安裝 Az PowerShell 模組](/powershell/azure/install-az-ps)。
  * 使用 [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) Cmdlet 連線至 Azure 帳戶。
* 如果您選擇使用 Azure Cloud Shell：
  * 請參閱 [Azure Cloud Shell 概觀](https://docs.microsoft.com/azure/cloud-shell/overview) 以取得詳細資訊。

  > [!IMPORTANT]
  > 雖然 **Az** PowerShell 模組目前為預覽狀態，但您必須使用指令程式個別進行安裝 `Install-Module` 。 此 PowerShell 模組正式推出後，便會成為未來 Az PowerShell 模組版本的一部分，且預設可從 Azure Cloud Shell 內使用。

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* 如果您有多個 Azure 訂用帳戶，請選擇資源計費的適當訂用帳戶。 使用 [Set-AzContext](/powershell/module/az.accounts/set-azcontext) Cmdlet 來選取特定的訂用帳戶。

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a>列出私人存放區

若要取出私人存放區的清單，請使用 [AzMarketplacePrivateStore 指令程式](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) 。 下列範例會列出在租使用者範圍下建立的私人存放區。

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

## <a name="add-an-offer-to-a-private-marketplace"></a>將供應專案新增至私人 marketplace

若要將供應專案新增至私用存放區，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) Cmdlet。 下列範例會將指定的供應專案新增至在租使用者範圍下建立之私用存放區的私人 marketplace。

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

## <a name="get-private-store-offers"></a>取得私人存放區優惠

若要取得一或多個私人存放區供應專案，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) Cmdlet。 下列範例會取得與指定的私用存放區相關聯的供應專案，這些供應專案已新增至租使用者範圍下。

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

## <a name="remove-an-offer"></a>移除供應專案

若要從私人存放區移除供應專案，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) Cmdlet。 下列範例會從租使用者範圍中建立的私人存放區移除供應專案。

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a>後續步驟

[建立及管理私用 Azure Marketplace](create-manage-private-azure-marketplace.md)。
