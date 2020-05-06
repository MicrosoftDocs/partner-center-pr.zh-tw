---
title: 將 Office 365 E4 訂閱移轉至新版 Office 365 | 合作夥伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 企業版 E4 從 2017 年 4 月 7 日起淘汰。 了解如何將您的客戶訂閱移轉至新版 Office 365。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 02d383172595e09a4ab0bf9c6db34862fcc17204
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798874"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="6dbf5-104">將 Office 365 E4 訂閱移轉至新版 Office 365</span><span class="sxs-lookup"><span data-stu-id="6dbf5-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="6dbf5-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="6dbf5-105">**Applies to**</span></span>

-  <span data-ttu-id="6dbf5-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="6dbf5-106">Partner Center</span></span>

<span data-ttu-id="6dbf5-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="6dbf5-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="6dbf5-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="6dbf5-108">Global admin</span></span>
-   <span data-ttu-id="6dbf5-109">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="6dbf5-109">User admin</span></span>
-   <span data-ttu-id="6dbf5-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="6dbf5-110">Admin agent</span></span>
-   <span data-ttu-id="6dbf5-111">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="6dbf5-111">Sales agent</span></span>

<span data-ttu-id="6dbf5-112">Office 365 企業版 E4 方案已淘汰，自 2017 年 4 月 7 日起生效。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="6dbf5-113">您在這個日期之後無法再購買新的 Office 365 E4 訂閱，而且現有的 E4 訂閱到期時不會自動續約。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="6dbf5-114">當 E4 訂閱結束時，會被取消。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="6dbf5-115">為了確保客戶持續的訂閱，您應該將具有即將到期 E4 訂閱的客戶轉換至支援的 SKU 選項，如下所列。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="6dbf5-116">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="6dbf5-117">Office 365 Enterprise E4 商業和政府 Sku 均已淘汰。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="6dbf5-118">在訂閱的詳細資料頁面上，E4 訂閱狀態已從「自動續約於 [日期]」變更為「到期日 [日期]」。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="6dbf5-119">如果您使用 API（CREST 或合作夥伴中心），您可以評估訂閱的結束日期加上自動續約 = False 屬性，探索即將到期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="6dbf5-120">E4 訂閱會設定為自動續約 = False 於 2017 年 4 月 7 日。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="6dbf5-121">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="6dbf5-122">Office 365 企業版 E4 取代方案</span><span class="sxs-lookup"><span data-stu-id="6dbf5-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="6dbf5-123">您可以選擇維持 E4 相同的功能，或讓您的客戶善加利用 Office 365 和商務用 Skype Online 中較新的功能。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="6dbf5-124">合作夥伴中心的價目表和優惠清單矩陣上可找到定價詳細資料。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="6dbf5-125">Secure Product Enterprise E3 或 Secure Productive Enterprise E5 可分別用來取代下列選項中的 Office 365 企業版 E3 或 Office 365 企業版 E5。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="6dbf5-126">選項 1：Office 365 企業版 E5</span><span class="sxs-lookup"><span data-stu-id="6dbf5-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="6dbf5-127">選項 2：Office 365 企業版 E3 + 商務用 Skype 雲端 PBX</span><span class="sxs-lookup"><span data-stu-id="6dbf5-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="6dbf5-128">選項 3：Office 365 企業版 E3 + 商務用 Skype Plus CAL（E4 的價格和功能同位）</span><span class="sxs-lookup"><span data-stu-id="6dbf5-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="6dbf5-129">選項 4：Office 365 企業版 E3</span><span class="sxs-lookup"><span data-stu-id="6dbf5-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="6dbf5-130">功能</span><span class="sxs-lookup"><span data-stu-id="6dbf5-130">Feature</span></span> | <span data-ttu-id="6dbf5-131">選項 1</span><span class="sxs-lookup"><span data-stu-id="6dbf5-131">Option 1</span></span> | <span data-ttu-id="6dbf5-132">選項 2</span><span class="sxs-lookup"><span data-stu-id="6dbf5-132">Option 2</span></span> | <span data-ttu-id="6dbf5-133">選項 3</span><span class="sxs-lookup"><span data-stu-id="6dbf5-133">Option 3</span></span> | <span data-ttu-id="6dbf5-134">選項 4</span><span class="sxs-lookup"><span data-stu-id="6dbf5-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="6dbf5-135">取得 Office 365 企業版 E4 中包含所有的功能？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="6dbf5-136">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-136">Yes</span></span> | <span data-ttu-id="6dbf5-137">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-137">Yes</span></span> | <span data-ttu-id="6dbf5-138">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-138">Yes</span></span> | <span data-ttu-id="6dbf5-139">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-139">No</span></span> |
| <span data-ttu-id="6dbf5-140">在 Office 365 中管理電話號碼？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="6dbf5-141">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-141">Yes</span></span> | <span data-ttu-id="6dbf5-142">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-142">Yes</span></span> | <span data-ttu-id="6dbf5-143">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-143">No</span></span> | <span data-ttu-id="6dbf5-144">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-144">No</span></span> |
| <span data-ttu-id="6dbf5-145">在內部部署和 Office 365（混合部署）中管理電話號碼？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="6dbf5-146">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-146">Yes</span></span> | <span data-ttu-id="6dbf5-147">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-147">Yes</span></span> | <span data-ttu-id="6dbf5-148">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-148">No</span></span> | <span data-ttu-id="6dbf5-149">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-149">No</span></span> |
| <span data-ttu-id="6dbf5-150">選項可新增 PSTN 語音通話方案嗎？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="6dbf5-151">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-151">Yes</span></span> | <span data-ttu-id="6dbf5-152">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-152">Yes</span></span> | <span data-ttu-id="6dbf5-153">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-153">No</span></span> | <span data-ttu-id="6dbf5-154">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-154">No</span></span> |
| <span data-ttu-id="6dbf5-155">PSTN 會議？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-155">PSTN Conferencing?</span></span> | <span data-ttu-id="6dbf5-156">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-156">Yes</span></span> | <span data-ttu-id="6dbf5-157">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-157">No</span></span> | <span data-ttu-id="6dbf5-158">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-158">No</span></span> | <span data-ttu-id="6dbf5-159">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-159">No</span></span> |
| <span data-ttu-id="6dbf5-160">共同作業、分析和安全性的進階工具？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="6dbf5-161">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-161">Yes</span></span> | <span data-ttu-id="6dbf5-162">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-162">No</span></span> | <span data-ttu-id="6dbf5-163">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-163">No</span></span> | <span data-ttu-id="6dbf5-164">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-164">No</span></span> |
| <span data-ttu-id="6dbf5-165">互動式報告、儀表板，以及資料視覺效果？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="6dbf5-166">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-166">Yes</span></span> | <span data-ttu-id="6dbf5-167">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-167">No</span></span> | <span data-ttu-id="6dbf5-168">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-168">No</span></span> | <span data-ttu-id="6dbf5-169">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-169">No</span></span> | 
| <span data-ttu-id="6dbf5-170">使用內建隱私權、透明度及精簡使用者控制項，對資料安全性與合規性的更多控制權？</span><span class="sxs-lookup"><span data-stu-id="6dbf5-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="6dbf5-171">是</span><span class="sxs-lookup"><span data-stu-id="6dbf5-171">Yes</span></span> | <span data-ttu-id="6dbf5-172">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-172">No</span></span> | <span data-ttu-id="6dbf5-173">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-173">No</span></span> | <span data-ttu-id="6dbf5-174">否</span><span class="sxs-lookup"><span data-stu-id="6dbf5-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="6dbf5-175">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="6dbf5-175">Transition customers to new product plans</span></span>

<span data-ttu-id="6dbf5-176">Microsoft 會持續提供新的產品及服務給我們的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="6dbf5-177">在這些情況下，您可能需要將客戶升級到新服務，或是從最後將會關閉的 SKU 移轉其訂閱。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="6dbf5-178">將客戶從淘汰的 SKU 移轉到較新的 SKU 時需要依照以下步驟執行：</span><span class="sxs-lookup"><span data-stu-id="6dbf5-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="6dbf5-179">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="6dbf5-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="6dbf5-180">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="6dbf5-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="6dbf5-181">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="6dbf5-181">Cancel the old subscription</span></span>

<span data-ttu-id="6dbf5-182">請依照下列步驟，將客戶的 Office 365 企業合作夥伴 E4 訂閱移轉到上述表格中的選項。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="6dbf5-183">步驟 1 - 購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="6dbf5-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="6dbf5-184">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，選取您想要移動的客戶，然後選取 [**新增訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="6dbf5-185">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="6dbf5-186">您的客戶現在應已有舊的和新的訂閱、舊的 Office 365 Enterprise E4 訂閱和新的「目標」訂用帳戶，例如選項 1-Office 365 企業版 E5。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="6dbf5-187">步驟 2 - 重新指派客戶的使用者授權</span><span class="sxs-lookup"><span data-stu-id="6dbf5-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="6dbf5-188">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，選取您想要移動的客戶，然後選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="6dbf5-189">客戶的 [使用者和授權] 頁面隨即開啟。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="6dbf5-190">若要重新指派使用者授權，請選取要重新指派的使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="6dbf5-191">在 **\[管理授權\]** 頁面中，清除 \*\*\[Office 365 企業版 E4\] \*\* 授權核取方塊，然後選取客戶訂閱移動到的新服務方案。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="6dbf5-192">選取 [提交]  。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-192">Select **Submit**.</span></span> <span data-ttu-id="6dbf5-193">確認頁面會列出新的授權指派。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="6dbf5-194">針對需要重新指派授權的任何其他客戶使用者繼續執行相同步驟。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="6dbf5-195">將使用者授權移至新服務後，您就可以放心地取消最上層 \[客戶\] 的已淘汰訂閱。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="6dbf5-196">步驟 3 - 取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="6dbf5-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="6dbf5-197">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="6dbf5-198">選取您想要移動的客戶，然後選取您想要取消的訂閱。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="6dbf5-199">在 [訂閱詳細資料] 頁面中，將訂閱狀態設定為 [已**暫停**]。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="6dbf5-200">選取 [提交]  。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-200">Select **Submit**.</span></span>

<span data-ttu-id="6dbf5-201">舊訂閱已暫停，而新訂閱為使用中。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="6dbf5-202">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="6dbf5-203">客戶不會因為舊訂閱而產生額外費用。</span><span class="sxs-lookup"><span data-stu-id="6dbf5-203">The customer incurs no additional costs for the old subscription.</span></span>



 



