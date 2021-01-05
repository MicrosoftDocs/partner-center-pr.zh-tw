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
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="58fa9-104">在 Azure 入口網站中建立及管理私人 Azure Marketplace (預覽) </span><span class="sxs-lookup"><span data-stu-id="58fa9-104">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="58fa9-105">私人 Azure Marketplace (預覽) 可讓系統管理員管理使用者可以使用的協力廠商解決方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-105">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="58fa9-106">這樣做的方法是讓您只部署您核准且符合企業原則的供應專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-106">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="58fa9-107">使用私用 Azure Marketplace 時，您的使用者可以在線上商店搜尋符合規範的供應專案以進行購買及部署。</span><span class="sxs-lookup"><span data-stu-id="58fa9-107">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="58fa9-108">作為 Marketplace 管理員 (指派的角色) ，您將從已停用和空白的私用存放區開始，您可以在其中新增已核准的供應專案和方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="58fa9-109">本文說明如何為您的使用者建立、管理及啟用私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="58fa9-109">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="58fa9-110">注意：</span><span class="sxs-lookup"><span data-stu-id="58fa9-110">Notes:</span></span>

- <span data-ttu-id="58fa9-111">私人 Azure Marketplace 是在租使用者層級，因此租使用者下的所有使用者都會看到相同的策劃清單。</span><span class="sxs-lookup"><span data-stu-id="58fa9-111">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="58fa9-112">所有 Microsoft 解決方案都會自動新增至私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="58fa9-112">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="58fa9-113">指派 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="58fa9-113">Assign the Marketplace admin role</span></span>

<span data-ttu-id="58fa9-114">租使用者全域管理員必須將 **Marketplace 管理員** 角色指派給將管理私用存放區的私用 Azure Marketplace 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="58fa9-114">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="58fa9-115">私人 Azure Marketplace 管理的存取權僅適用于已指派 Marketplace 管理員角色的 IT 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="58fa9-115">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="58fa9-116">必要條件</span><span class="sxs-lookup"><span data-stu-id="58fa9-116">Prerequisites</span></span>

<span data-ttu-id="58fa9-117">您必須符合這些必要條件，才能將 Marketplace 系統管理員角色指派給租使用者範圍的使用者：</span><span class="sxs-lookup"><span data-stu-id="58fa9-117">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="58fa9-118">您可以存取 **全域管理員** 使用者。</span><span class="sxs-lookup"><span data-stu-id="58fa9-118">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="58fa9-119">租使用者至少有一個訂用帳戶 (可以是任何類型) 。</span><span class="sxs-lookup"><span data-stu-id="58fa9-119">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="58fa9-120">系統會將所選訂用帳戶的「 **參與者** 」角色或更高許可權指派給全域管理員使用者。</span><span class="sxs-lookup"><span data-stu-id="58fa9-120">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-iam"></a><span data-ttu-id="58fa9-121">使用 IAM 指派 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="58fa9-121">Assign the Marketplace admin role with IAM</span></span>

1. <span data-ttu-id="58fa9-122">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="58fa9-122">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="58fa9-123">選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-123">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 入口網站主視窗。":::

3. <span data-ttu-id="58fa9-125">從左側的選項中選取 [ **私人 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-125">Select **Private Marketplace** from the options on the left.</span></span>
1. <span data-ttu-id="58fa9-126">選取 [ **存取控制] (IAM)** 以指派 Marketplace 管理員角色。</span><span class="sxs-lookup"><span data-stu-id="58fa9-126">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="IAM 存取控制畫面。":::

1. <span data-ttu-id="58fa9-128">選取 [+新增] > [新增角色指派]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-128">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="58fa9-129">在 [ **角色**] 下，選擇 [ **Marketplace 管理員**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-129">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="角色指派功能表。":::

1. <span data-ttu-id="58fa9-131">從下拉式清單中選取所需的使用者，然後選取 [ **完成**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-131">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="58fa9-132">使用 PowerShell 指派 Marketplace 管理員角色</span><span class="sxs-lookup"><span data-stu-id="58fa9-132">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="58fa9-133">使用下列 PowerShell 腳本來指派 Marketplace 管理員角色;它需要下列參數：</span><span class="sxs-lookup"><span data-stu-id="58fa9-133">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="58fa9-134">**TenantId：** (Marketplace 管理員角色範圍內的租使用者識別碼可指派于租使用者範圍) 。</span><span class="sxs-lookup"><span data-stu-id="58fa9-134">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="58fa9-135">**SubscriptionId：** 全域管理員已獲指派 **參與者** 角色或更高許可權的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="58fa9-135">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="58fa9-136">**GlobalAdminUsername：** 全域管理員的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="58fa9-136">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="58fa9-137">**UsernameToAssignRoleFor：** 將指派 Marketplace 管理員角色的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="58fa9-137">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="58fa9-138">對於受邀加入租使用者的來賓使用者，最多可能需要48小時，直到他們的帳戶可以指派 Marketplace 管理員角色為止。</span><span class="sxs-lookup"><span data-stu-id="58fa9-138">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="58fa9-139">如需詳細資訊，請參閱 [AZURE ACTIVE DIRECTORY B2B 共同作業使用者的屬性](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="58fa9-139">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="58fa9-140">如需 Az. Portal PowerShell 模組中所含 Cmdlet 的詳細資訊，請參閱 [Microsoft Azure PowerShell：入口網站儀表板 Cmdlet](/powershell/module/az.portal/)。</span><span class="sxs-lookup"><span data-stu-id="58fa9-140">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="58fa9-141">建立私用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="58fa9-141">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="58fa9-142">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="58fa9-142">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="58fa9-143">選取 [ **所有服務** ]，然後選取 [ **Marketplace**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-143">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure 入口網站主視窗。":::

3. <span data-ttu-id="58fa9-145">從左側的選項中選取 [ **私人 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-145">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="在 Azure 入口網站主視窗中選取 [私人 Marketplace]。":::

4. <span data-ttu-id="58fa9-147">選取 **開始** 建立私用 Azure Marketplace (您只需要) 進行一次。</span><span class="sxs-lookup"><span data-stu-id="58fa9-147">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="選取 Azure 入口網站主視窗上的開始。":::

    <span data-ttu-id="58fa9-149">如果此租使用者已有私人 Azure Marketplace，預設會選取 [ **管理 Marketplace** ]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-149">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="58fa9-150">完成之後，您將會有空白且已停用的私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="58fa9-150">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空白的私用 Azure Marketplace 畫面。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="58fa9-152">從資源庫新增專案</span><span class="sxs-lookup"><span data-stu-id="58fa9-152">Add items from gallery</span></span>

<span data-ttu-id="58fa9-153">專案是供應專案和方案的組合。</span><span class="sxs-lookup"><span data-stu-id="58fa9-153">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="58fa9-154">您可以在 [管理 Marketplace] 頁面中搜尋和新增專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-154">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="58fa9-155">選取 [ **加入專案**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-155">Select **Add items**.</span></span>

2. <span data-ttu-id="58fa9-156">流覽資源 **庫** ，或使用搜尋欄位來尋找您想要的專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-156">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="流覽資源庫或使用 [搜尋] 欄位。":::

3. <span data-ttu-id="58fa9-158">依預設，加入新的供應專案時，會將所有目前的方案新增至允許清單。</span><span class="sxs-lookup"><span data-stu-id="58fa9-158">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="58fa9-159">若要在加入選取的專案之前修改方案選取專案，請選取供應專案磚中的下拉式功能表，並更新所需的方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-159">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="更新所需的方案。":::

4. <span data-ttu-id="58fa9-161">選取之後，請選取左下方的 [ **完成** ]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-161">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="58fa9-162">將 **專案新增** 至 Marketplace 的功能只適用于非 Microsoft 供應專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-162">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="58fa9-163">預設允許 Microsoft 優惠。</span><span class="sxs-lookup"><span data-stu-id="58fa9-163">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="58fa9-164">編輯專案計劃</span><span class="sxs-lookup"><span data-stu-id="58fa9-164">Edit item plans</span></span>

<span data-ttu-id="58fa9-165">您可以在 [管理 Marketplace] 頁面中編輯專案的方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-165">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="58fa9-166">在 [ **方案** ] 資料行中，從該專案的下拉式功能表中，檢查可用的方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-166">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="58fa9-167">選取或清除核取方塊，以選擇要讓使用者使用的方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-167">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="選取或清除必要專案的核取方塊。":::

> [!NOTE]
> <span data-ttu-id="58fa9-169">每個供應專案都需要至少選取一個方案，才能進行更新。</span><span class="sxs-lookup"><span data-stu-id="58fa9-169">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="58fa9-170">若要移除與供應專案相關的所有方案，請刪除整個供應專案 (參閱下一節) 。</span><span class="sxs-lookup"><span data-stu-id="58fa9-170">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="58fa9-171">刪除供應項目</span><span class="sxs-lookup"><span data-stu-id="58fa9-171">Delete offers</span></span>

<span data-ttu-id="58fa9-172">在 [管理 Marketplace] 頁面中，選取供應專案名稱旁邊的核取方塊 (查看上面的畫面) 然後選取 [ **刪除專案**]。</span><span class="sxs-lookup"><span data-stu-id="58fa9-172">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="58fa9-173">啟用/停用私人 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="58fa9-173">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="58fa9-174">在 [管理 Marketplace] 頁面中，您會看到其中一個橫幅，其中顯示私人 Azure Marketplace 的目前狀態：</span><span class="sxs-lookup"><span data-stu-id="58fa9-174">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="停用狀態橫幅":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="啟用狀態橫幅":::

<span data-ttu-id="58fa9-177">您可以視需要啟用或停用私用 Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="58fa9-177">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="58fa9-178">如果已停用，請選取 [ **啟用私人 Marketplace** ] 以啟用。</span><span class="sxs-lookup"><span data-stu-id="58fa9-178">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="58fa9-179">若已啟用，請選取 [ **停用私人 Marketplace** ] 以停用。</span><span class="sxs-lookup"><span data-stu-id="58fa9-179">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="58fa9-180">流覽私用 Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="58fa9-180">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="58fa9-181">啟用私人 Azure Marketplace 時，使用者會看到 Marketplace 系統管理員允許的方案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-181">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="58fa9-182">綠色的 **許可** 通知表示合作夥伴 (不允許的非 Microsoft) 供應專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-182">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="58fa9-183">藍色 **許可** 聲明表示允許的 Microsoft 供應專案。</span><span class="sxs-lookup"><span data-stu-id="58fa9-183">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="58fa9-184">使用者可以篩選不允許且不允許的供應專案：</span><span class="sxs-lookup"><span data-stu-id="58fa9-184">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="篩選選項。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="58fa9-186">在私用 Azure Marketplace 中購買或部署</span><span class="sxs-lookup"><span data-stu-id="58fa9-186">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="58fa9-187">雖然產品詳細資料網頁體驗類似于公用 Azure Marketplace，但有三個私用 Azure Marketplace 特定案例。</span><span class="sxs-lookup"><span data-stu-id="58fa9-187">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="58fa9-188">當使用者選取允許的方案時，會啟用 [ **建立** ] 按鈕：</span><span class="sxs-lookup"><span data-stu-id="58fa9-188">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="提供可建立方案的供應專案橫幅。":::

- <span data-ttu-id="58fa9-190">當使用者選取非允許的方案時，橫幅會指出不允許該計畫，而 [ **建立** ] 按鈕已停用。</span><span class="sxs-lookup"><span data-stu-id="58fa9-190">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="供應專案橫幅指出無法建立方案。":::

- <span data-ttu-id="58fa9-192">如果產品方案選項未出現在 [產品詳細資料] 頁面中，但系統管理員已核准一或多個方案，則橫幅會注明允許的方案，並啟用 [ **建立** ] 按鈕：</span><span class="sxs-lookup"><span data-stu-id="58fa9-192">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="供應專案橫幅指出可以建立方案並顯示可用的方案。":::

## <a name="contact-support"></a><span data-ttu-id="58fa9-194">請連絡支援人員</span><span class="sxs-lookup"><span data-stu-id="58fa9-194">Contact support</span></span>

<span data-ttu-id="58fa9-195">如 Azure Marketplace 支援，請造訪 [Microsoft Q&A](/answers/products/)。</span><span class="sxs-lookup"><span data-stu-id="58fa9-195">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
