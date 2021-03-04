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
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="89cf8-104">在 Azure 入口網站中建立和管理私用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="89cf8-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="89cf8-105">私用 Azure Marketplace 可讓系統管理員管理使用者可以使用的協力廠商解決方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="89cf8-106">這樣做的方法是讓使用者只部署由系統管理員核准並符合您企業原則的供應專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="89cf8-107">使用私用 Azure Marketplace 時，使用者可以在線上商店搜尋符合規範的供應專案以進行購買及部署。</span><span class="sxs-lookup"><span data-stu-id="89cf8-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="89cf8-108">作為 Marketplace 管理員 (指派的角色) ，您將從已停用和空白的私用存放區開始，您可以在其中新增已核准的供應專案和方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="89cf8-109">本文說明如何指派所需的角色、建立私人存放區、管理專案、核准使用者要求，以及為您的使用者啟用私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="89cf8-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="89cf8-110">私用 Azure Marketplace 是租使用者層級，因此租使用者下的所有使用者都會看到相同的策劃清單。</span><span class="sxs-lookup"><span data-stu-id="89cf8-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="89cf8-111">所有 Microsoft 解決方案 (包括 [背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 散發套件) 都會自動新增至私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="89cf8-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="89cf8-112">指派 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="89cf8-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="89cf8-113">租使用者全域管理員必須將 **Marketplace 管理員** 角色指派給將管理私用存放區的私人 Azure Marketplace 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="89cf8-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="89cf8-114">私人 Azure Marketplace 管理的存取權僅適用于已指派 Marketplace 管理員角色的 IT 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="89cf8-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="89cf8-115">必要條件</span><span class="sxs-lookup"><span data-stu-id="89cf8-115">Prerequisites</span></span>

<span data-ttu-id="89cf8-116">您必須要有這些必要條件，才能將 Marketplace 系統管理員角色指派給租使用者範圍中的使用者：</span><span class="sxs-lookup"><span data-stu-id="89cf8-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="89cf8-117">您可以存取 **全域管理員** 使用者。</span><span class="sxs-lookup"><span data-stu-id="89cf8-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="89cf8-118">租使用者至少有一個訂用帳戶 (可以是任何類型) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="89cf8-119">系統會將所選訂用帳戶的「 **參與者** 」角色或更高許可權指派給全域管理員使用者。</span><span class="sxs-lookup"><span data-stu-id="89cf8-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="89cf8-120">指派具有存取控制 (IAM) 的 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="89cf8-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="89cf8-121">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="89cf8-122">選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="89cf8-123">從左側功能表中選取 [ **私人 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="89cf8-124">[![顯示 Marketplace 左側的 [私用 marketplace] 功能表選項。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="89cf8-125">選取 [ **存取控制] (IAM)** 以指派 Marketplace 管理員角色。</span><span class="sxs-lookup"><span data-stu-id="89cf8-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="顯示 I A M 存取控制畫面。":::

1. <span data-ttu-id="89cf8-127">選取 [+新增] > [新增角色指派]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="89cf8-128">在 [ **角色**] 下，選擇 [ **Marketplace 管理員**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="顯示 [角色指派] 功能表。":::

1. <span data-ttu-id="89cf8-130">從下拉式清單中選取所需的使用者，然後選取 [ **完成**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="89cf8-131">使用 PowerShell 指派 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="89cf8-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="89cf8-132">使用下列 PowerShell 腳本來指派 Marketplace 管理員角色;它需要下列參數：</span><span class="sxs-lookup"><span data-stu-id="89cf8-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="89cf8-133">**TenantId：** (Marketplace 管理員角色範圍內的租使用者識別碼可指派于租使用者範圍) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="89cf8-134">**SubscriptionId：** 全域管理員已獲指派 **參與者** 角色或更高許可權的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="89cf8-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="89cf8-135">**GlobalAdminUsername：** 全域管理員的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="89cf8-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="89cf8-136">**UsernameToAssignRoleFor：** 將指派 Marketplace 管理員角色的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="89cf8-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="89cf8-137">對於受邀加入租使用者的來賓使用者，最多可能需要48小時，直到他們的帳戶可以指派 Marketplace 管理員角色為止。</span><span class="sxs-lookup"><span data-stu-id="89cf8-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="89cf8-138">如需詳細資訊，請參閱 [Azure Active DIRECTORY B2B 共同作業使用者的屬性](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="89cf8-139">如需 Az. Portal PowerShell 模組中所含 Cmdlet 的詳細資訊，請參閱 [Microsoft Azure PowerShell：入口網站儀表板 Cmdlet](/powershell/module/az.portal/)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="89cf8-140">建立私人 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="89cf8-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="89cf8-141">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="89cf8-142">選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="顯示 Azure 入口網站主視窗。":::

3. <span data-ttu-id="89cf8-144">從左側功能表中選取 [ **私人 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="89cf8-145">選取 [ **開始** 使用] 建立私人 Azure Marketplace (您只需要) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="顯示如何選取 [開始使用 Azure 入口網站] 主視窗。":::

    <span data-ttu-id="89cf8-147">如果此租使用者已有私人 Azure Marketplace 存在，預設會選取 [ **管理 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="89cf8-148">完成之後，您將會有空白且已停用的私人 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="89cf8-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="顯示空白的私用 Azure Marketplace 畫面。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="89cf8-150">從資源庫新增專案</span><span class="sxs-lookup"><span data-stu-id="89cf8-150">Add items from gallery</span></span>

<span data-ttu-id="89cf8-151">專案是供應專案和方案的組合。</span><span class="sxs-lookup"><span data-stu-id="89cf8-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="89cf8-152">您可以在 [管理 Marketplace] 頁面上搜尋和新增專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="89cf8-153">選取 [ **加入專案**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-153">Select **Add items**.</span></span>

2. <span data-ttu-id="89cf8-154">流覽資源 **庫** ，或使用搜尋欄位來尋找您想要的專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="89cf8-155">[![顯示如何流覽資源庫或使用搜尋欄位。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="89cf8-156">依預設，加入新的供應專案時，會將所有目前的方案新增至核准的清單。</span><span class="sxs-lookup"><span data-stu-id="89cf8-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="89cf8-157">若要在加入選取的專案之前修改方案選取專案，請選取供應專案磚中的下拉式功能表，並更新所需的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="顯示如何更新所需的計畫。":::

4. <span data-ttu-id="89cf8-159">選取之後，請選取左下方的 [ **完成** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="89cf8-160">將 **專案新增** 至 Marketplace 的功能只適用于非 Microsoft 供應專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="89cf8-161">Microsoft 解決方案 (包括 [背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 散發套件) 將會標記為「預設為已核准」，且無法在私人 Marketplace 中進行管理。</span><span class="sxs-lookup"><span data-stu-id="89cf8-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="89cf8-162">編輯專案的計畫</span><span class="sxs-lookup"><span data-stu-id="89cf8-162">Edit item's plans</span></span>

<span data-ttu-id="89cf8-163">您可以在 [管理 Marketplace] 頁面上編輯專案的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="89cf8-164">在 [ **方案** ] 資料行中，從該專案的下拉式功能表中，檢查可用的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="89cf8-165">選取或清除核取方塊，以選擇要讓使用者使用的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="顯示如何選取或清除必要專案的核取方塊。":::

> [!NOTE]
> <span data-ttu-id="89cf8-167">每個供應專案都需要至少選取一個方案，才能進行更新。</span><span class="sxs-lookup"><span data-stu-id="89cf8-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="89cf8-168">若要移除與供應專案相關的所有方案，請刪除整個供應專案 (參閱下一節) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="89cf8-169">刪除供應項目</span><span class="sxs-lookup"><span data-stu-id="89cf8-169">Delete offers</span></span>

<span data-ttu-id="89cf8-170">在 [管理 Marketplace] 頁面中，選取供應專案名稱旁邊的核取方塊 (查看上面的畫面) 然後選取 [ **刪除專案**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="89cf8-171">啟用/停用私人 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="89cf8-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="89cf8-172">在 [管理 Marketplace] 頁面中，您會看到其中一個橫幅，其中顯示私人 Azure Marketplace 的目前狀態：</span><span class="sxs-lookup"><span data-stu-id="89cf8-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="顯示「停用狀態」橫幅。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="顯示 [啟用狀態] 橫幅。":::

<span data-ttu-id="89cf8-175">您可以視需要啟用或停用私人 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="89cf8-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="89cf8-176">如果已停用，請選取 [ **啟用私人 Marketplace** ] 以啟用。</span><span class="sxs-lookup"><span data-stu-id="89cf8-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="89cf8-177">若已啟用，請選取 [ **停用私人 Marketplace** ] 以停用。</span><span class="sxs-lookup"><span data-stu-id="89cf8-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="89cf8-178">私人 Azure Marketplace 通知中心</span><span class="sxs-lookup"><span data-stu-id="89cf8-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="89cf8-179">通知中心包含三種類型的通知，可讓 Marketplace 系統管理員根據通知採取動作：</span><span class="sxs-lookup"><span data-stu-id="89cf8-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="89cf8-180">針對不在核准清單中之專案的使用者核准要求 (查看在) [新增優惠或方案的要求](#request-to-add-offers-or-plans) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="89cf8-181">針對已在核准清單中有一或多個方案的供應專案，提供新的方案通知。</span><span class="sxs-lookup"><span data-stu-id="89cf8-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="89cf8-182">已針對核准清單中的專案移除方案通知，但已從全域 Azure Marketplace 中移除。</span><span class="sxs-lookup"><span data-stu-id="89cf8-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="89cf8-183">若要存取通知中心：</span><span class="sxs-lookup"><span data-stu-id="89cf8-183">To access the notification center:</span></span>

1. <span data-ttu-id="89cf8-184">從左側功能表中選取 [ **通知** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="89cf8-185">[![顯示 [通知] 功能表。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="89cf8-186">選取省略號功能表以尋找更多動作。</span><span class="sxs-lookup"><span data-stu-id="89cf8-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="顯示更多選項功能表結果。":::

1. <span data-ttu-id="89cf8-188">針對方案要求， **顯示要求** 會開啟核准要求表單，您可以在其中查看特定供應專案的所有使用者要求。</span><span class="sxs-lookup"><span data-stu-id="89cf8-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="89cf8-189">選取 [ **核准** ] 或 [ **拒絕**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="89cf8-190">[![顯示 [核准] 和 [拒絕] 選項。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="89cf8-191">從下拉式功能表中選取要核准的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="89cf8-192">新增批註，然後選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="89cf8-193">流覽私人 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="89cf8-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="89cf8-194">啟用私人 Azure Marketplace 時，使用者會看到 Marketplace 系統管理員已核准的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="89cf8-195">綠色的 **核准** 通知表示合作夥伴 (非 Microsoft) 供應專案已核准。</span><span class="sxs-lookup"><span data-stu-id="89cf8-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="89cf8-196">藍色 **核准** 的通知表示 Microsoft 供應專案 (包括已核准的 [背書 Linux 發行](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) 版) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="89cf8-197">使用者可以篩選未核准的供應專案（& a）：</span><span class="sxs-lookup"><span data-stu-id="89cf8-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="89cf8-198">[![顯示篩選選項。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="89cf8-199">在私人 Azure Marketplace 中購買或部署</span><span class="sxs-lookup"><span data-stu-id="89cf8-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="89cf8-200">雖然產品詳細資料頁面體驗類似于全球 Azure Marketplace，但有三個私人 Azure Marketplace 特定案例。</span><span class="sxs-lookup"><span data-stu-id="89cf8-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="89cf8-201">當使用者選取核准的方案時，會啟用 [ **建立** ] 按鈕：</span><span class="sxs-lookup"><span data-stu-id="89cf8-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="89cf8-202">[![顯示供應專案橫幅，指出可以建立方案。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="89cf8-203">如果產品方案選項未出現在 [產品詳細資料] 頁面中，但系統管理員已核准一或多個方案，則橫幅會注明哪些方案已通過核准，並已啟用 [ **建立** ] 按鈕：</span><span class="sxs-lookup"><span data-stu-id="89cf8-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="89cf8-204">[![顯示供應專案橫幅，指出可以建立方案並顯示可用的方案。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="89cf8-205">當使用者選取未核准的方案時，橫幅會將方案注明為 [未核准]，並停用 [ **建立** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="89cf8-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="89cf8-206">使用者仍然可以要求將方案新增至核准清單 (請參閱下一節) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="89cf8-207">新增優惠或方案的要求</span><span class="sxs-lookup"><span data-stu-id="89cf8-207">Request to add offers or plans</span></span>

<span data-ttu-id="89cf8-208">您可以要求新增私人 Azure Marketplace 中目前未核准的公用供應專案或方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="89cf8-209">選取 **要** 在橫幅中新增的要求，以開啟 **存取要求表單**。</span><span class="sxs-lookup"><span data-stu-id="89cf8-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="89cf8-210">[![顯示具有 [要新增的要求] 連結的橫幅。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="89cf8-211">[![顯示供應專案或方案的存取要求表單。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="89cf8-212">選取要新增至要求的計畫 (**任何方案** 都會告知 Marketplace 系統管理員，您在供應專案) 內沒有方案的喜好設定。</span><span class="sxs-lookup"><span data-stu-id="89cf8-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="89cf8-213">新增 **理由** 並選取提交要求的 **要求** 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="89cf8-214">[![以範例專案顯示供應專案或方案的存取要求表單。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="89cf8-215">「存取要求」表單中會出現暫止要求的指示，並提供撤銷 **要求** 的選項。</span><span class="sxs-lookup"><span data-stu-id="89cf8-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="89cf8-216">[![使用撤銷要求連結來顯示已核准或擱置中的計畫清單。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="89cf8-217">提交之後，會將核准要求表單傳送到 [通知中心](#private-azure-marketplace-notification-center) ，讓 Marketplace 系統管理員可以審核要求並採取動作。</span><span class="sxs-lookup"><span data-stu-id="89cf8-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="89cf8-218">常見問題集 (FAQ)</span><span class="sxs-lookup"><span data-stu-id="89cf8-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="89cf8-219">我已經透過 Azure 原則封鎖 Marketplace 協力廠商應用程式。</span><span class="sxs-lookup"><span data-stu-id="89cf8-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="89cf8-220">這有何不同？</span><span class="sxs-lookup"><span data-stu-id="89cf8-220">How is this different?</span></span>

<span data-ttu-id="89cf8-221">目前有兩種方式可以限制 Marketplace 中的協力廠商服務：</span><span class="sxs-lookup"><span data-stu-id="89cf8-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="89cf8-222">透過 EA 入口網站或 Azure 入口網站，停用協力廠商服務，或限制為「僅限可用或 BYOL Sku」。</span><span class="sxs-lookup"><span data-stu-id="89cf8-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="顯示如何在 Azure 入口網站中限制服務。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="顯示如何在 E A 入口網站中限制服務。":::

2. <span data-ttu-id="89cf8-225">建立 Azure 原則，以僅允許特定的 Vm。</span><span class="sxs-lookup"><span data-stu-id="89cf8-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="89cf8-226">如需如何將原則強制套用至 Windows Vm 的詳細資訊，請參閱 [使用 Azure Resource Manager 將原則套用至 Windows vm](https://docs.microsoft.com/azure/virtual-machines/windows/policy)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="89cf8-227">私用 Azure Marketplace 可讓您更靈活地限制和允許特定的供應專案和方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="89cf8-228">它會通知終端使用者，即使在嘗試部署協力廠商服務之前，仍可在 marketplace 資源庫中進行部署。</span><span class="sxs-lookup"><span data-stu-id="89cf8-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="89cf8-229">若要允許部署協力廠商服務，請在 EA 入口網站和 Azure 入口網站中，將 Azure Marketplace 設定為 On/Enabled。</span><span class="sxs-lookup"><span data-stu-id="89cf8-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="89cf8-230">私用 Azure Marketplace 可策展不限於虛擬機器的合作夥伴解決方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="89cf8-231">私用 Azure Marketplace 可在方案層級策展，也可以設定「目前與未來的計畫」。</span><span class="sxs-lookup"><span data-stu-id="89cf8-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="89cf8-232">私用 Azure Marketplace 可以事先通知終端使用者可和無法部署的內容。</span><span class="sxs-lookup"><span data-stu-id="89cf8-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="89cf8-233">私人供應專案和私人 Azure Marketplace 之間有何差異？</span><span class="sxs-lookup"><span data-stu-id="89cf8-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="89cf8-234">**私人供應** 專案可讓發行者建立只有目標客戶可以看見的方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="89cf8-235">這可讓他們私用已協商定價、私用條款及條件，以及特殊設定的自訂解決方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="89cf8-236">如需詳細資訊，請參閱 [商業 marketplace 中的私用](https://docs.microsoft.com/azure/marketplace/private-offers)供應專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="89cf8-237">Azure 入口網站中的 **私用 Azure Marketplace** 可讓系統管理員預先核准使用者可以部署的協力廠商解決方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="89cf8-238">使用私用 Azure Marketplace，使用者可以藉由尋找、購買及部署符合規範的供應專案，享受 Azure Marketplace 的優點。</span><span class="sxs-lookup"><span data-stu-id="89cf8-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="89cf8-239">若要在私人 Marketplace 中管理以訂用帳戶為基礎的私人供應專案，Marketplace 系統管理員在特定訂用帳戶上至少必須有「讀取」角色。</span><span class="sxs-lookup"><span data-stu-id="89cf8-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="89cf8-240">我已將私人供應專案新增至私用 Azure Marketplace，為什麼它不會顯示在 [管理 Marketplace] 索引標籤中？</span><span class="sxs-lookup"><span data-stu-id="89cf8-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="89cf8-241">以訂用帳戶為基礎的私人供應專案，只會顯示在私用供應專案設定中列出的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="89cf8-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="89cf8-242">若要查看私人供應專案，請確定全域訂用帳戶篩選器會顯示所有訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="89cf8-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="89cf8-243">[![顯示私人 marketplace 篩選。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="89cf8-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="89cf8-244">我們可以在私人 Azure Marketplace 中包含自訂映射嗎？</span><span class="sxs-lookup"><span data-stu-id="89cf8-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="89cf8-245">不會。</span><span class="sxs-lookup"><span data-stu-id="89cf8-245">No.</span></span> <span data-ttu-id="89cf8-246">私用 Azure Marketplace 可讓任何 IT 系統管理員從全球 Azure Marketplace 管理和策展協力廠商解決方案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="89cf8-247">由於自訂映射不在全域 Azure Marketplace 上，因此 IT 系統管理員無法挑選並選擇您的自訂映射。</span><span class="sxs-lookup"><span data-stu-id="89cf8-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="89cf8-248">如果您想要共用自訂映射，請使用 [共用映射庫](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="89cf8-249">建立共用映射庫 (SIG)  ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)) 的逐步指南。</span><span class="sxs-lookup"><span data-stu-id="89cf8-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="89cf8-250">在 SIG 內建立映射定義。</span><span class="sxs-lookup"><span data-stu-id="89cf8-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="89cf8-251">客戶應該針對 [OS 狀態] 欄位選擇 [ **一般化** ]。</span><span class="sxs-lookup"><span data-stu-id="89cf8-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="89cf8-252"> ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="89cf8-253"> ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)) 將受控映射帶入共用映射庫。</span><span class="sxs-lookup"><span data-stu-id="89cf8-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="89cf8-254">SIG VM 映射會位於一個訂用帳戶中。</span><span class="sxs-lookup"><span data-stu-id="89cf8-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="89cf8-255">若要將它提供給其他訂用帳戶使用，請使用應用程式註冊 ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) 。</span><span class="sxs-lookup"><span data-stu-id="89cf8-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="89cf8-256">為什麼我會看到某些供應專案 **預設為核准** ，即使發行者不是 Microsoft 也是一樣？</span><span class="sxs-lookup"><span data-stu-id="89cf8-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="89cf8-257">Microsoft 支援 Azure 中的 Linux 和開放原始碼技術。</span><span class="sxs-lookup"><span data-stu-id="89cf8-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="89cf8-258">Azure 支援[背書的 Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)散發套件，且價格已在虛擬機器中整合。</span><span class="sxs-lookup"><span data-stu-id="89cf8-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="89cf8-259">因為 azure Linux 代理程式已預先安裝在 Azure Marketplace 上，所以會被視為 Microsoft 供應專案。</span><span class="sxs-lookup"><span data-stu-id="89cf8-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="89cf8-260">由於 Microsoft 供應專案預設為已核准，因此無法在私人 Azure Marketplace 中管理背書的 Linux 散發套件，並依預設核准。</span><span class="sxs-lookup"><span data-stu-id="89cf8-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="89cf8-261">請連絡支援人員</span><span class="sxs-lookup"><span data-stu-id="89cf8-261">Contact support</span></span>

- <span data-ttu-id="89cf8-262">如需 Azure Marketplace 支援，請造訪 [Microsoft Q&A](/answers/products/)。</span><span class="sxs-lookup"><span data-stu-id="89cf8-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
