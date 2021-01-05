---
title: 在 Azure 入口網站中建立和管理私用 Azure Marketplace
description: 瞭解如何在 Azure 入口網站中建立和管理私人 Azure Marketplace (preview) 。 私人 Azure Marketplace (預覽) 可讓系統管理員管理使用者可以使用的協力廠商解決方案。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 12/22/2020
ms.openlocfilehash: 09f7bcb29dc619e4e31c0aa3d5c73fade5218819
ms.sourcegitcommit: 30d154cdf40aa75400be7805cd9b2685b66a1382
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/24/2020
ms.locfileid: "97760797"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>在 Azure 入口網站中建立及管理私人 Azure Marketplace (預覽) 

私人 Azure Marketplace (預覽) 可讓系統管理員管理使用者可以使用的協力廠商解決方案。 這樣做的方法是讓您只部署您核准且符合企業原則的供應專案。 使用私用 Azure Marketplace 時，您的使用者可以在線上商店搜尋符合規範的供應專案以進行購買及部署。 

作為 Marketplace 管理員 (指派的角色) ，您將從已停用和空白的私用存放區開始，您可以在其中新增已核准的供應專案和方案。 本文說明如何為您的使用者建立、管理及啟用私用 Azure Marketplace。

注意：

- 私人 Azure Marketplace 是在租使用者層級，因此租使用者下的所有使用者都會看到相同的策劃清單。
- 所有 Microsoft 解決方案都會自動新增至私用 Azure Marketplace。

## <a name="assign-the-marketplace-admin-role"></a>指派 Marketplace 管理員角色

租使用者全域管理員必須將 **Marketplace 管理員** 角色指派給將管理私用存放區的私用 Azure Marketplace 系統管理員。

>[!IMPORTANT]
> 私人 Azure Marketplace 管理的存取權僅適用于已指派 Marketplace 管理員角色的 IT 系統管理員。

### <a name="prerequisites"></a>必要條件

您必須符合這些必要條件，才能將 Marketplace 系統管理員角色指派給租使用者範圍的使用者：

- 您可以存取 **全域管理員** 使用者。
- 租使用者至少有一個訂用帳戶 (可以是任何類型) 。
- 系統會將所選訂用帳戶的「 **參與者** 」角色或更高許可權指派給全域管理員使用者。

### <a name="assign-the-marketplace-admin-role-with-iam"></a>使用 IAM 指派 Marketplace 管理員角色

1. 登入 [Azure 入口網站](https://portal.azure.com/)。
1. 選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 入口網站主視窗。":::

3. 從左側的選項中選取 [ **私人 Marketplace** ]。
1. 選取 [ **存取控制] (IAM)** 以指派 Marketplace 管理員角色。

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="IAM 存取控制畫面。":::

1. 選取 [+新增] > [新增角色指派]。
1. 在 [ **角色**] 下，選擇 [ **Marketplace 管理員**]。

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="角色指派功能表。":::

1. 從下拉式清單中選取所需的使用者，然後選取 [ **完成**]。

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>使用 PowerShell 指派 Marketplace 管理員角色

使用下列 PowerShell 腳本來指派 Marketplace 管理員角色;它需要下列參數：

- **TenantId：** (Marketplace 管理員角色範圍內的租使用者識別碼可指派于租使用者範圍) 。
- **SubscriptionId：** 全域管理員已獲指派 **參與者** 角色或更高許可權的訂用帳戶。
- **GlobalAdminUsername：** 全域管理員的使用者名稱。
- **UsernameToAssignRoleFor：** 將指派 Marketplace 管理員角色的使用者名稱。

> [!NOTE]
> 對於受邀加入租使用者的來賓使用者，最多可能需要48小時，直到他們的帳戶可以指派 Marketplace 管理員角色為止。 如需詳細資訊，請參閱 [AZURE ACTIVE DIRECTORY B2B 共同作業使用者的屬性](/azure/active-directory/b2b/user-properties)。

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

如需 Az. Portal PowerShell 模組中所含 Cmdlet 的詳細資訊，請參閱 [Microsoft Azure PowerShell：入口網站儀表板 Cmdlet](/powershell/module/az.portal/)。

## <a name="create-private-azure-marketplace"></a>建立私用 Azure Marketplace

1. 登入 [Azure 入口網站](https://portal.azure.com/)。
2. 選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 入口網站主視窗。":::

3. 從左側的選項中選取 [ **私人 Marketplace** ]。

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="在 Azure 入口網站主視窗中選取 [私人 Marketplace]。":::

4. 選取 **開始** 建立私用 Azure Marketplace (您只需要) 進行一次。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="選取 Azure 入口網站主視窗上的開始。":::

    如果此租使用者已有私人 Azure Marketplace，預設會選取 [ **管理 Marketplace** ]。

5. 完成之後，您將會有空白且已停用的私用 Azure Marketplace。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空白的私用 Azure Marketplace 畫面。":::

## <a name="add-items-from-gallery"></a>從資源庫新增專案

專案是供應專案和方案的組合。 您可以在 [管理 Marketplace] 頁面中搜尋和新增專案。

1. 選取 [ **加入專案**]。

2. 流覽資源 **庫** ，或使用搜尋欄位來尋找您想要的專案。

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="流覽資源庫或使用 [搜尋] 欄位。":::

3. 依預設，加入新的供應專案時，會將所有目前的方案新增至允許清單。 若要在加入選取的專案之前修改方案選取專案，請選取供應專案磚中的下拉式功能表，並更新所需的方案。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="更新所需的方案。":::

4. 選取之後，請選取左下方的 [ **完成** ]。

>[!Note]
> 將 **專案新增** 至 Marketplace 的功能只適用于非 Microsoft 供應專案。 預設允許 Microsoft 優惠。

## <a name="edit-item-plans"></a>編輯專案計劃

您可以在 [管理 Marketplace] 頁面中編輯專案的方案。

1. 在 [ **方案** ] 資料行中，從該專案的下拉式功能表中，檢查可用的方案。
2. 選取或清除核取方塊，以選擇要讓使用者使用的方案。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="選取或清除必要專案的核取方塊。":::

> [!NOTE]
> 每個供應專案都需要至少選取一個方案，才能進行更新。 若要移除與供應專案相關的所有方案，請刪除整個供應專案 (參閱下一節) 。

## <a name="delete-offers"></a>刪除供應項目

在 [管理 Marketplace] 頁面中，選取供應專案名稱旁邊的核取方塊 (查看上面的畫面) 然後選取 [ **刪除專案**]。

## <a name="enabledisable-private-azure-marketplace"></a>啟用/停用私人 Azure Marketplace

在 [管理 Marketplace] 頁面中，您會看到其中一個橫幅，其中顯示私人 Azure Marketplace 的目前狀態：

:::image type="content" source="media/private-azure/state-disable.png" alt-text="停用狀態橫幅":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="啟用狀態橫幅":::

您可以視需要啟用或停用私用 Azure Marketplace。

- 如果已停用，請選取 [ **啟用私人 Marketplace** ] 以啟用。
- 若已啟用，請選取 [ **停用私人 Marketplace** ] 以停用。

## <a name="browsing-private-azure-marketplace"></a>流覽私用 Azure Marketplace

啟用私人 Azure Marketplace 時，使用者會看到 Marketplace 系統管理員允許的方案。

- 綠色的 **許可** 通知表示合作夥伴 (不允許的非 Microsoft) 供應專案。
- 藍色 **許可** 聲明表示允許的 Microsoft 供應專案。

使用者可以篩選不允許且不允許的供應專案：

:::image type="content" source="media/private-azure/filter-option.png" alt-text="篩選選項。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>在私用 Azure Marketplace 中購買或部署

雖然產品詳細資料網頁體驗類似于公用 Azure Marketplace，但有三個私用 Azure Marketplace 特定案例。

- 當使用者選取允許的方案時，會啟用 [ **建立** ] 按鈕：

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="提供可建立方案的供應專案橫幅。":::

- 當使用者選取非允許的方案時，橫幅會指出不允許該計畫，而 [ **建立** ] 按鈕已停用。

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="供應專案橫幅指出無法建立方案。":::

- 如果產品方案選項未出現在 [產品詳細資料] 頁面中，但系統管理員已核准一或多個方案，則橫幅會注明允許的方案，並啟用 [ **建立** ] 按鈕：

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="供應專案橫幅指出可以建立方案並顯示可用的方案。":::

## <a name="contact-support"></a>請連絡支援人員

如 Azure Marketplace 支援，請造訪 [Microsoft Q&A](/answers/products/)。 
