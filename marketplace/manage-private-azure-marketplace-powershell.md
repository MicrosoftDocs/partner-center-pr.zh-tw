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
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="961a5-103">快速入門：使用 PowerShell 管理私用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="961a5-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="961a5-104">本文說明如何使用 [Az](/powershell/module/az.marketplace) PowerShell 模組來管理私用 Azure Marketplace 中的供應專案。</span><span class="sxs-lookup"><span data-stu-id="961a5-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="961a5-105">私用 Azure Marketplace 目前處於公開預覽狀態。</span><span class="sxs-lookup"><span data-stu-id="961a5-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="961a5-106">所提供的這個預覽版本並沒有服務等級協定。</span><span class="sxs-lookup"><span data-stu-id="961a5-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="961a5-107">不建議用於生產工作負載。</span><span class="sxs-lookup"><span data-stu-id="961a5-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="961a5-108">某些功能可能不受支援，或可能具有受限的功能。</span><span class="sxs-lookup"><span data-stu-id="961a5-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="961a5-109">如需詳細資訊，請參閱 [Microsoft Azure 預覽版增補使用條款](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)。</span><span class="sxs-lookup"><span data-stu-id="961a5-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="961a5-110">需求</span><span class="sxs-lookup"><span data-stu-id="961a5-110">Requirements</span></span>

* <span data-ttu-id="961a5-111">如果您沒有 Azure 訂用帳戶，請在開始前建立[免費帳戶](https://azure.microsoft.com/free/)。</span><span class="sxs-lookup"><span data-stu-id="961a5-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="961a5-112">如果您選擇在本機使用 Azure PowerShell：</span><span class="sxs-lookup"><span data-stu-id="961a5-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="961a5-113">[安裝 Az PowerShell 模組](/powershell/azure/install-az-ps)。</span><span class="sxs-lookup"><span data-stu-id="961a5-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="961a5-114">使用 [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) Cmdlet 連線至 Azure 帳戶。</span><span class="sxs-lookup"><span data-stu-id="961a5-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="961a5-115">如果您選擇使用 Azure Cloud Shell：</span><span class="sxs-lookup"><span data-stu-id="961a5-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="961a5-116">請參閱 [Azure Cloud Shell 概觀](https://docs.microsoft.com/azure/cloud-shell/overview) 以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="961a5-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="961a5-117">雖然 **Az** PowerShell 模組目前為預覽狀態，但您必須使用指令程式個別進行安裝 `Install-Module` 。</span><span class="sxs-lookup"><span data-stu-id="961a5-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="961a5-118">此 PowerShell 模組正式推出後，便會成為未來 Az PowerShell 模組版本的一部分，且預設可從 Azure Cloud Shell 內使用。</span><span class="sxs-lookup"><span data-stu-id="961a5-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="961a5-119">如果您有多個 Azure 訂用帳戶，請選擇資源計費的適當訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="961a5-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="961a5-120">使用 [Set-AzContext](/powershell/module/az.accounts/set-azcontext) Cmdlet 來選取特定的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="961a5-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="961a5-121">列出私人存放區</span><span class="sxs-lookup"><span data-stu-id="961a5-121">List private stores</span></span>

<span data-ttu-id="961a5-122">若要取出私人存放區的清單，請使用 [AzMarketplacePrivateStore 指令程式](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) 。</span><span class="sxs-lookup"><span data-stu-id="961a5-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="961a5-123">下列範例會列出在租使用者範圍下建立的私人存放區。</span><span class="sxs-lookup"><span data-stu-id="961a5-123">The following example lists private stores that were created under the tenant scope.</span></span>

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

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="961a5-124">將供應專案新增至私人 marketplace</span><span class="sxs-lookup"><span data-stu-id="961a5-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="961a5-125">若要將供應專案新增至私用存放區，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="961a5-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="961a5-126">下列範例會將指定的供應專案新增至在租使用者範圍下建立之私用存放區的私人 marketplace。</span><span class="sxs-lookup"><span data-stu-id="961a5-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

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

## <a name="get-private-store-offers"></a><span data-ttu-id="961a5-127">取得私人存放區優惠</span><span class="sxs-lookup"><span data-stu-id="961a5-127">Get private store offers</span></span>

<span data-ttu-id="961a5-128">若要取得一或多個私人存放區供應專案，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="961a5-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="961a5-129">下列範例會取得與指定的私用存放區相關聯的供應專案，這些供應專案已新增至租使用者範圍下。</span><span class="sxs-lookup"><span data-stu-id="961a5-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

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

## <a name="remove-an-offer"></a><span data-ttu-id="961a5-130">移除供應專案</span><span class="sxs-lookup"><span data-stu-id="961a5-130">Remove an offer</span></span>

<span data-ttu-id="961a5-131">若要從私人存放區移除供應專案，請使用 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) Cmdlet。</span><span class="sxs-lookup"><span data-stu-id="961a5-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="961a5-132">下列範例會從租使用者範圍中建立的私人存放區移除供應專案。</span><span class="sxs-lookup"><span data-stu-id="961a5-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="961a5-133">後續步驟</span><span class="sxs-lookup"><span data-stu-id="961a5-133">Next steps</span></span>

<span data-ttu-id="961a5-134">[建立及管理私用 Azure Marketplace](create-manage-private-azure-marketplace.md)。</span><span class="sxs-lookup"><span data-stu-id="961a5-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
