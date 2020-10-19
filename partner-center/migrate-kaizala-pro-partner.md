---
title: 將 Kaizala Pro 訂閱遷移至 Microsoft 365
description: 瞭解如何將 Kaizala Pro 訂閱遷移至 Microsoft 365 或 Office 365 版本。 如需轉換客戶的詳細資料，請閱讀這篇文章。
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175174"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="4b464-104">將 Kaizala Pro 獨立訂閱遷移至 Microsoft 365 或 Office 365 版本</span><span class="sxs-lookup"><span data-stu-id="4b464-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="4b464-105">從2020年7月1日起，Microsoft 即將結束 Kaizala Pro 獨立服務的銷售。</span><span class="sxs-lookup"><span data-stu-id="4b464-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="4b464-106">客戶將無法再于此日期之後購買新的 Kaizala Pro 訂用帳戶，而且現有的 Kaizala Pro 訂閱將不會在到期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="4b464-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="4b464-107">為確保客戶的持續性，您應該將即將到期的 Kaizala Pro 獨立訂用帳戶轉換為支援的 SKU 選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="4b464-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="4b464-108">建議您將客戶移至訂用帳戶年度結束日期之前的新訂用帳戶，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="4b464-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="4b464-109">如果您使用 API (CREST 或合作夥伴中心) ，您可以評估訂用帳戶的結束日期，並將 [自動更新] 屬性設定為 [false]，以探索即將到期的訂閱： `auto renew = False` 。</span><span class="sxs-lookup"><span data-stu-id="4b464-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="4b464-110">E4 訂閱將于 `auto renew=False` 2020 年7月1日設定為。</span><span class="sxs-lookup"><span data-stu-id="4b464-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="4b464-111">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="4b464-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="4b464-112">Kaizala Pro 獨立取代方案</span><span class="sxs-lookup"><span data-stu-id="4b464-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="4b464-113">透過新的方案，您的客戶可以利用 Microsoft 365 中的較新特性和功能。</span><span class="sxs-lookup"><span data-stu-id="4b464-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="4b464-114">合作夥伴中心的價目表和優惠清單矩陣上可找到定價詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4b464-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="4b464-115">[**商務 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)，包括：</span><span class="sxs-lookup"><span data-stu-id="4b464-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="4b464-116">Microsoft 365 商務基本版</span><span class="sxs-lookup"><span data-stu-id="4b464-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="4b464-117">Microsoft 365 商務標準版</span><span class="sxs-lookup"><span data-stu-id="4b464-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="4b464-118">Microsoft 365 商務進階版</span><span class="sxs-lookup"><span data-stu-id="4b464-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="4b464-119">[**適用于 Frontline 的 Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)，包括：</span><span class="sxs-lookup"><span data-stu-id="4b464-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="4b464-120">Microsoft 365 F3 (先前的 Microsoft 365 F1) 與 Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="4b464-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="4b464-121">[**適用于 Enterprise 的 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)，包括：</span><span class="sxs-lookup"><span data-stu-id="4b464-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="4b464-122">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="4b464-122">Office 365 E1</span></span>
   - <span data-ttu-id="4b464-123">Microsoft 365 E3 與 Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="4b464-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="4b464-124">Microsoft 365 E5 與 Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="4b464-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="4b464-125">[**Microsoft 365 教育**](https://www.microsoft.com/education/buy-license/microsoft365)版，包括：</span><span class="sxs-lookup"><span data-stu-id="4b464-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="4b464-126">Microsoft 365 A1 和 Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="4b464-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="4b464-127">Microsoft 365 A3 和 Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="4b464-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="4b464-128">Microsoft 365 A5 和 Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="4b464-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="4b464-129">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="4b464-129">Transition customers to new product plans</span></span>

<span data-ttu-id="4b464-130">Microsoft 會持續提供新的產品及服務給我們的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="4b464-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="4b464-131">在這些情況下，您可能需要將客戶升級到新服務，或是從最後將會關閉的 SKU 移轉其訂閱。</span><span class="sxs-lookup"><span data-stu-id="4b464-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="4b464-132">將客戶從淘汰的 SKU 移轉到較新的 SKU 時需要依照以下步驟執行：</span><span class="sxs-lookup"><span data-stu-id="4b464-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="4b464-133">A.</span><span class="sxs-lookup"><span data-stu-id="4b464-133">A.</span></span> <span data-ttu-id="4b464-134">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="4b464-134">Purchase the new subscription</span></span>

<span data-ttu-id="4b464-135">B.</span><span class="sxs-lookup"><span data-stu-id="4b464-135">B.</span></span> <span data-ttu-id="4b464-136">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="4b464-136">Reassign current user licenses</span></span>

<span data-ttu-id="4b464-137">C.</span><span class="sxs-lookup"><span data-stu-id="4b464-137">C.</span></span> <span data-ttu-id="4b464-138">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="4b464-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="4b464-139">將您的客戶移轉至新方案</span><span class="sxs-lookup"><span data-stu-id="4b464-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="4b464-140">A.</span><span class="sxs-lookup"><span data-stu-id="4b464-140">A.</span></span> <span data-ttu-id="4b464-141">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="4b464-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="4b464-142">若要購買新的訂用帳戶，請選取 [ **合作夥伴中心** ] 功能表中的 [ **客戶**]，選取您要移動的客戶，然後選取 [ **新增訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="4b464-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="4b464-143">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="4b464-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="4b464-144">您的客戶現在應該會有舊的和新的訂用帳戶，也就是舊的 Kaizala Pro 獨立訂用帳戶和新的「目標」訂用帳戶，例如選項 1-Office 365 Enterprise F1。</span><span class="sxs-lookup"><span data-stu-id="4b464-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="4b464-145">B.</span><span class="sxs-lookup"><span data-stu-id="4b464-145">B.</span></span> <span data-ttu-id="4b464-146">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="4b464-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="4b464-147">若要重新指派客戶的使用者授權，請從 [ **合作夥伴中心** ] 功能表選取 [ **客戶**]，選取您要移動的客戶，然後選取 [ **使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="4b464-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="4b464-148">[客戶的使用者和授權] 頁面隨即開啟。</span><span class="sxs-lookup"><span data-stu-id="4b464-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="4b464-149">若要重新指派使用者授權，請選取要重新指派的使用者，然後選取 [ **管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="4b464-149">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="4b464-150">在 [ **管理授權** ] 頁面上，清除 [Kaizala Pro 獨立授權] 核取方塊，然後為客戶移至的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="4b464-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="4b464-151">選取 [提交]  。</span><span class="sxs-lookup"><span data-stu-id="4b464-151">Select **Submit**.</span></span> <span data-ttu-id="4b464-152">確認頁面會列出新的授權指派。</span><span class="sxs-lookup"><span data-stu-id="4b464-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="4b464-153">為其他需要指派授權的使用者，繼續進行這個相同程序。</span><span class="sxs-lookup"><span data-stu-id="4b464-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="4b464-154">C.</span><span class="sxs-lookup"><span data-stu-id="4b464-154">C.</span></span> <span data-ttu-id="4b464-155">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="4b464-155">Cancel old subscription</span></span>

<span data-ttu-id="4b464-156">將使用者授權移至新服務後，您就可以放心地取消客戶層級的已淘汰訂閱。</span><span class="sxs-lookup"><span data-stu-id="4b464-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="4b464-157">從 [ **合作夥伴中心** ] 功能表選取 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="4b464-157">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="4b464-158">選取您要取消其訂閱的客戶。</span><span class="sxs-lookup"><span data-stu-id="4b464-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="4b464-159">在訂閱詳細資料頁面中，將訂閱設定為 **\[已暫停\]**。</span><span class="sxs-lookup"><span data-stu-id="4b464-159">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="4b464-160">選取 [提交]  。</span><span class="sxs-lookup"><span data-stu-id="4b464-160">Select **Submit**.</span></span>

<span data-ttu-id="4b464-161">舊訂閱已暫停，而新訂閱為使用中。</span><span class="sxs-lookup"><span data-stu-id="4b464-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="4b464-162">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="4b464-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="4b464-163">客戶不會因為舊訂閱而產生額外費用。</span><span class="sxs-lookup"><span data-stu-id="4b464-163">The customer incurs no additional costs for the old subscription.</span></span>
