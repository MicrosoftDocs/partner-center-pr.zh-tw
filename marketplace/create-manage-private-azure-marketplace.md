---
title: 在 Azure 入口網站中建立和管理私用 Azure Marketplace
description: 瞭解如何在 Azure 入口網站中建立及管理私人 Azure Marketplace (預覽版) 。 私人 Azure Marketplace (預覽版) 可讓系統管理員管理使用者可以使用的協力廠商解決方案。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "101757080"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>在 Azure 入口網站中建立和管理私用 Azure Marketplace

私用 Azure Marketplace 可讓系統管理員管理使用者可以使用的協力廠商解決方案。 這樣做的方法是讓使用者只部署由系統管理員核准並符合您企業原則的供應專案。 使用私用 Azure Marketplace 時，使用者可以在線上商店搜尋符合規範的供應專案以進行購買及部署。

作為 Marketplace 管理員 (指派的角色) ，您將從已停用和空白的私用存放區開始，您可以在其中新增已核准的供應專案和方案。 本文說明如何指派所需的角色、建立私人存放區、管理專案、核准使用者要求，以及為您的使用者啟用私用 Azure Marketplace。

> [!NOTE]
> - 私用 Azure Marketplace 是租使用者層級，因此租使用者下的所有使用者都會看到相同的策劃清單。
> - 所有 Microsoft 解決方案 (包括 [背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 散發套件) 都會自動新增至私用 Azure Marketplace。

## <a name="assign-the-marketplace-admin-role"></a>指派 Marketplace 管理員角色

租使用者全域管理員必須將 **Marketplace 管理員** 角色指派給將管理私用存放區的私人 Azure Marketplace 系統管理員。

>[!IMPORTANT]
> 私人 Azure Marketplace 管理的存取權僅適用于已指派 Marketplace 管理員角色的 IT 系統管理員。

### <a name="prerequisites"></a>必要條件

您必須要有這些必要條件，才能將 Marketplace 系統管理員角色指派給租使用者範圍中的使用者：

- 您可以存取 **全域管理員** 使用者。
- 租使用者至少有一個訂用帳戶 (可以是任何類型) 。
- 系統會將所選訂用帳戶的「 **參與者** 」角色或更高許可權指派給全域管理員使用者。

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>指派具有存取控制 (IAM) 的 Marketplace 管理員角色

1. 登入 [Azure 入口網站](https://portal.azure.com/)。
1. 選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。
1. 從左側功能表中選取 [ **私人 Marketplace** ]。

    [![顯示 Marketplace 左側的 [私用 marketplace] 功能表選項。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. 選取 [ **存取控制] (IAM)** 以指派 Marketplace 管理員角色。

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="顯示 I A M 存取控制畫面。":::

1. 選取 [+新增] > [新增角色指派]。
1. 在 [ **角色**] 下，選擇 [ **Marketplace 管理員**]。

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="顯示 [角色指派] 功能表。":::

1. 從下拉式清單中選取所需的使用者，然後選取 [ **完成**]。

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>使用 PowerShell 指派 Marketplace 管理員角色

使用下列 PowerShell 腳本來指派 Marketplace 管理員角色;它需要下列參數：

- **TenantId：** (Marketplace 管理員角色範圍內的租使用者識別碼可指派于租使用者範圍) 。
- **SubscriptionId：** 全域管理員已獲指派 **參與者** 角色或更高許可權的訂用帳戶。
- **GlobalAdminUsername：** 全域管理員的使用者名稱。
- **UsernameToAssignRoleFor：** 將指派 Marketplace 管理員角色的使用者名稱。

> [!NOTE]
> 對於受邀加入租使用者的來賓使用者，最多可能需要48小時，直到他們的帳戶可以指派 Marketplace 管理員角色為止。 如需詳細資訊，請參閱 [Azure Active DIRECTORY B2B 共同作業使用者的屬性](/azure/active-directory/b2b/user-properties)。

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

## <a name="create-private-azure-marketplace"></a>建立私人 Azure Marketplace

1. 登入 [Azure 入口網站](https://portal.azure.com/)。
2. 選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="顯示 Azure 入口網站主視窗。":::

3. 從左側功能表中選取 [ **私人 Marketplace** ]。

4. 選取 [ **開始** 使用] 建立私人 Azure Marketplace (您只需要) 。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="顯示如何選取 [開始使用 Azure 入口網站] 主視窗。":::

    如果此租使用者已有私人 Azure Marketplace 存在，預設會選取 [ **管理 Marketplace** ]。

5. 完成之後，您將會有空白且已停用的私人 Azure Marketplace。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="顯示空白的私用 Azure Marketplace 畫面。":::

## <a name="add-items-from-gallery"></a>從資源庫新增專案

專案是供應專案和方案的組合。 您可以在 [管理 Marketplace] 頁面上搜尋和新增專案。

1. 選取 [ **加入專案**]。

2. 流覽資源 **庫** ，或使用搜尋欄位來尋找您想要的專案。

    [![顯示如何流覽資源庫或使用搜尋欄位。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. 依預設，加入新的供應專案時，會將所有目前的方案新增至核准的清單。 若要在加入選取的專案之前修改方案選取專案，請選取供應專案磚中的下拉式功能表，並更新所需的方案。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="顯示如何更新所需的計畫。":::

4. 選取之後，請選取左下方的 [ **完成** ]。

>[!Note]
> 將 **專案新增** 至 Marketplace 的功能只適用于非 Microsoft 供應專案。 Microsoft 解決方案 (包括 [背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 散發套件) 將會標記為「預設為已核准」，且無法在私人 Marketplace 中進行管理。

## <a name="edit-items-plans"></a>編輯專案的計畫

您可以在 [管理 Marketplace] 頁面上編輯專案的方案。

1. 在 [ **方案** ] 資料行中，從該專案的下拉式功能表中，檢查可用的方案。
2. 選取或清除核取方塊，以選擇要讓使用者使用的方案。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="顯示如何選取或清除必要專案的核取方塊。":::

> [!NOTE]
> 每個供應專案都需要至少選取一個方案，才能進行更新。 若要移除與供應專案相關的所有方案，請刪除整個供應專案 (參閱下一節) 。

## <a name="delete-offers"></a>刪除供應項目

在 [管理 Marketplace] 頁面中，選取供應專案名稱旁邊的核取方塊 (查看上面的畫面) 然後選取 [ **刪除專案**]。

## <a name="enabledisable-private-azure-marketplace"></a>啟用/停用私人 Azure Marketplace

在 [管理 Marketplace] 頁面中，您會看到其中一個橫幅，其中顯示私人 Azure Marketplace 的目前狀態：

:::image type="content" source="media/private-azure/state-disable.png" alt-text="顯示「停用狀態」橫幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="顯示 [啟用狀態] 橫幅。":::

您可以視需要啟用或停用私人 Azure Marketplace。

- 如果已停用，請選取 [ **啟用私人 Marketplace** ] 以啟用。
- 若已啟用，請選取 [ **停用私人 Marketplace** ] 以停用。

## <a name="private-azure-marketplace-notification-center"></a>私人 Azure Marketplace 通知中心

通知中心包含三種類型的通知，可讓 Marketplace 系統管理員根據通知採取動作：

- 針對不在核准清單中之專案的使用者核准要求 (查看在) [新增優惠或方案的要求](#request-to-add-offers-or-plans) 。
- 針對已在核准清單中有一或多個方案的供應專案，提供新的方案通知。
- 已針對核准清單中的專案移除方案通知，但已從全域 Azure Marketplace 中移除。

若要存取通知中心：

1. 從左側功能表中選取 [ **通知** ]。

    [![顯示 [通知] 功能表。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. 選取省略號功能表以尋找更多動作。

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="顯示更多選項功能表結果。":::

1. 針對方案要求， **顯示要求** 會開啟核准要求表單，您可以在其中查看特定供應專案的所有使用者要求。
1. 選取 [ **核准** ] 或 [ **拒絕**]。

    [![顯示 [核准] 和 [拒絕] 選項。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. 從下拉式功能表中選取要核准的方案。
1. 新增批註，然後選取 [ **提交**]。

## <a name="browsing-private-azure-marketplace"></a>流覽私人 Azure Marketplace

啟用私人 Azure Marketplace 時，使用者會看到 Marketplace 系統管理員已核准的方案。

- 綠色的 **核准** 通知表示合作夥伴 (非 Microsoft) 供應專案已核准。
- 藍色 **核准** 的通知表示 Microsoft 供應專案 (包括已核准的 [背書 Linux 發行](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 版) 。

使用者可以篩選未核准的供應專案（& a）：

[![顯示篩選選項。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>在私人 Azure Marketplace 中購買或部署

雖然產品詳細資料頁面體驗類似于全球 Azure Marketplace，但有三個私人 Azure Marketplace 特定案例。

- 當使用者選取核准的方案時，會啟用 [ **建立** ] 按鈕：

    [![顯示供應專案橫幅，指出可以建立方案。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- 如果產品方案選項未出現在 [產品詳細資料] 頁面中，但系統管理員已核准一或多個方案，則橫幅會注明哪些方案已通過核准，並已啟用 [ **建立** ] 按鈕：

    [![顯示供應專案橫幅，指出可以建立方案並顯示可用的方案。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- 當使用者選取未核准的方案時，橫幅會將方案注明為 [未核准]，並停用 [ **建立** ] 按鈕。 使用者仍然可以要求將方案新增至核准清單 (請參閱下一節) 。

## <a name="request-to-add-offers-or-plans"></a>新增優惠或方案的要求

您可以要求新增私人 Azure Marketplace 中目前未核准的公用供應專案或方案。

1. 選取 **要** 在橫幅中新增的要求，以開啟 **存取要求表單**。

    [![顯示具有 [要新增的要求] 連結的橫幅。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![顯示供應專案或方案的存取要求表單。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. 選取要新增至要求的計畫 (**任何方案** 都會告知 Marketplace 系統管理員，您在供應專案) 內沒有方案的喜好設定。

1. 新增 **理由** 並選取提交要求的 **要求** 。
  
    [![以範例專案顯示供應專案或方案的存取要求表單。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. 「存取要求」表單中會出現暫止要求的指示，並提供撤銷 **要求** 的選項。

    [![使用撤銷要求連結來顯示已核准或擱置中的計畫清單。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> 提交之後，會將核准要求表單傳送到 [通知中心](#private-azure-marketplace-notification-center) ，讓 Marketplace 系統管理員可以審核要求並採取動作。

## <a name="frequently-asked-questions-faqs"></a>常見問題集 (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>我已經透過 Azure 原則封鎖 Marketplace 協力廠商應用程式。 這有何不同？

目前有兩種方式可以限制 Marketplace 中的協力廠商服務：

1. 透過 EA 入口網站或 Azure 入口網站，停用協力廠商服務，或限制為「僅限可用或 BYOL Sku」。

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="顯示如何在 Azure 入口網站中限制服務。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="顯示如何在 E A 入口網站中限制服務。":::

2. 建立 Azure 原則，以僅允許特定的 Vm。 如需如何將原則強制套用至 Windows Vm 的詳細資訊，請參閱 [使用 Azure Resource Manager 將原則套用至 Windows vm](https://docs.microsoft.com/azure/virtual-machines/windows/policy)。

私用 Azure Marketplace 可讓您更靈活地限制和允許特定的供應專案和方案。 它會通知終端使用者，即使在嘗試部署協力廠商服務之前，仍可在 marketplace 資源庫中進行部署。 若要允許部署協力廠商服務，請在 EA 入口網站和 Azure 入口網站中，將 Azure Marketplace 設定為 On/Enabled。

- 私用 Azure Marketplace 可策展不限於虛擬機器的合作夥伴解決方案。
- 私用 Azure Marketplace 可在方案層級策展，也可以設定「目前與未來的計畫」。
- 私用 Azure Marketplace 可以事先通知終端使用者可和無法部署的內容。

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>私人供應專案和私人 Azure Marketplace 之間有何差異？

**私人供應** 專案可讓發行者建立只有目標客戶可以看見的方案。 這可讓他們私用已協商定價、私用條款及條件，以及特殊設定的自訂解決方案。 如需詳細資訊，請參閱 [商業 marketplace 中的私用](https://docs.microsoft.com/azure/marketplace/private-offers)供應專案。

Azure 入口網站中的 **私用 Azure Marketplace** 可讓系統管理員預先核准使用者可以部署的協力廠商解決方案。 使用私用 Azure Marketplace，使用者可以藉由尋找、購買及部署符合規範的供應專案，享受 Azure Marketplace 的優點。 若要在私人 Marketplace 中管理以訂用帳戶為基礎的私人供應專案，Marketplace 系統管理員在特定訂用帳戶上至少必須有「讀取」角色。

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>我已將私人供應專案新增至私用 Azure Marketplace，為什麼它不會顯示在 [管理 Marketplace] 索引標籤中？

以訂用帳戶為基礎的私人供應專案，只會顯示在私用供應專案設定中列出的訂用帳戶。 若要查看私人供應專案，請確定全域訂用帳戶篩選器會顯示所有訂用帳戶。

[![顯示私人 marketplace 篩選。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>我們可以在私人 Azure Marketplace 中包含自訂映射嗎？

不會。 私用 Azure Marketplace 可讓任何 IT 系統管理員從全球 Azure Marketplace 管理和策展協力廠商解決方案。 由於自訂映射不在全域 Azure Marketplace 上，因此 IT 系統管理員無法挑選並選擇您的自訂映射。 如果您想要共用自訂映射，請使用 [共用映射庫](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries)。

1. 建立共用映射庫 (SIG)  ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)) 的逐步指南。
2. 在 SIG 內建立映射定義。 客戶應該針對 [OS 狀態] 欄位選擇 [ **一般化** ]。  ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。
3.  ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)) 將受控映射帶入共用映射庫。
4. SIG VM 映射會位於一個訂用帳戶中。 若要將它提供給其他訂用帳戶使用，請使用應用程式註冊 ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) 。

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>為什麼我會看到某些供應專案 **預設為核准** ，即使發行者不是 Microsoft 也是一樣？

Microsoft 支援 Azure 中的 Linux 和開放原始碼技術。 Azure 支援[背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)散發套件，且價格已在虛擬機器中整合。 因為 azure Linux 代理程式已預先安裝在 Azure Marketplace 上，所以會被視為 Microsoft 供應專案。 由於 Microsoft 供應專案預設為已核准，因此無法在私人 Azure Marketplace 中管理背書的 Linux 散發套件，並依預設核准。

## <a name="contact-support"></a>請連絡支援人員

- 如需 Azure Marketplace 支援，請造訪 [Microsoft Q&A](/answers/products/)。
