---
title: 雲端解決方案提供者地區授權租用戶彙總 | 合作夥伴中心
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 請依照下列指示合併不同國家/地區的租用戶。 這包括遷移客戶帳戶和客戶訂閱的步驟。
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: jasonwhowell
ms.author: jasonh
keywords: 移轉客戶, 佈建, 租用戶帳戶, 合併租用戶
ms.localizationpriority: medium
robots: noindex,nofollow
ms.openlocfilehash: 04c39d15b9e2c0223ef472bc14de82faae12a449
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390967"
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="ccda1-105">雲端解決方案提供者地區授權租用戶彙總</span><span class="sxs-lookup"><span data-stu-id="ccda1-105">CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="ccda1-106">**適用於**</span><span class="sxs-lookup"><span data-stu-id="ccda1-106">**Applies to**</span></span>

-  <span data-ttu-id="ccda1-107">夥伴中心</span><span class="sxs-lookup"><span data-stu-id="ccda1-107">Partner Center</span></span>
-  <span data-ttu-id="ccda1-108">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="ccda1-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="ccda1-109">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="ccda1-109">**Appropriate roles**</span></span>

- <span data-ttu-id="ccda1-110">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="ccda1-110">Global admin</span></span>
- <span data-ttu-id="ccda1-111">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="ccda1-111">Admin agent</span></span>

<span data-ttu-id="ccda1-112">\[一些與預先發行產品相關的資訊，在正式發行之前，可能會大幅修改。</span><span class="sxs-lookup"><span data-stu-id="ccda1-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="ccda1-113">Microsoft 對於此處提供的資訊不做任何明示或默示的擔保。\]</span><span class="sxs-lookup"><span data-stu-id="ccda1-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="ccda1-114">請依照下列指示合併不同國家/地區的租用戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="ccda1-115">**注意**：您必須知道您從轉換帳戶佈建之客戶的所有訂閱和基座數目。</span><span class="sxs-lookup"><span data-stu-id="ccda1-115">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="ccda1-116">您將在移轉程序中，於新的中央雲端解決方案提供者帳戶底下被精確地重新佈建那些相同的訂閱與相同的基座數目。</span><span class="sxs-lookup"><span data-stu-id="ccda1-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="ccda1-117">請使用匯出清單功能來協助建立要移到集中式租用戶之客戶的清單。</span><span class="sxs-lookup"><span data-stu-id="ccda1-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="ccda1-118">合作夥伴選擇合併他們的租用戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="ccda1-119">合併完成之後，合作夥伴就無法回復到先前的狀態。</span><span class="sxs-lookup"><span data-stu-id="ccda1-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="ccda1-120">請注意，也需要執行客戶動作。</span><span class="sxs-lookup"><span data-stu-id="ccda1-120">Note that customer action may also be required.</span></span>



## <a name="prepare-for-migration"></a><span data-ttu-id="ccda1-121">準備移轉</span><span class="sxs-lookup"><span data-stu-id="ccda1-121">Prepare for migration</span></span>


-   <span data-ttu-id="ccda1-122">使用**轉換**（現有）帳戶（您將轉換的帳戶）登入**合作夥伴中心**，並記下所有客戶和為這些客戶布建的所有服務。</span><span class="sxs-lookup"><span data-stu-id="ccda1-122">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

![地區客戶清單](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="ccda1-124">移轉客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="ccda1-124">Migrate customer accounts</span></span>


1.  <span data-ttu-id="ccda1-125">使用**轉換**（新）帳戶（您要轉換的使用者）登入您的**合作夥伴中心**，然後流覽至**客戶**的客戶清單。</span><span class="sxs-lookup"><span data-stu-id="ccda1-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2.  <span data-ttu-id="ccda1-126">選取客戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-126">Select Customers.</span></span>

3.  <span data-ttu-id="ccda1-127">按一下 \[要求建立經銷商關係\]。</span><span class="sxs-lookup"><span data-stu-id="ccda1-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="ccda1-128">系統就會提供您一則預設的電子郵件訊息以供您提供給您的客戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="ccda1-129">此訊息包含一個 URL，其中包含您新的合作夥伴中心帳戶唯一的組織識別碼。</span><span class="sxs-lookup"><span data-stu-id="ccda1-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="ccda1-130">**客戶動作：** 確保您要移轉的每個作用中客戶都會造訪此 URL。</span><span class="sxs-lookup"><span data-stu-id="ccda1-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="ccda1-131">開啟 URL 時，會提示客戶登入 Office 365 入口網站。</span><span class="sxs-lookup"><span data-stu-id="ccda1-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="ccda1-132">客戶使用和用來存取 Azure 及 Office 365 管理入口網站時相同的組織識別碼登入。</span><span class="sxs-lookup"><span data-stu-id="ccda1-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="ccda1-133">登入之後，就會提示客戶帳戶的全域系統管理員送出合約，以提供委派的系統管理員權限給新的雲端解決方案提供者帳戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="ccda1-134">如果他們同意，客戶就能選取核取方塊並同意授權關係。</span><span class="sxs-lookup"><span data-stu-id="ccda1-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="ccda1-135">當客戶提交合約之後，就會出現在合作夥伴的客戶清單中。</span><span class="sxs-lookup"><span data-stu-id="ccda1-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="ccda1-136">移轉 Office 365 和非 Azure 用量型訂閱</span><span class="sxs-lookup"><span data-stu-id="ccda1-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="ccda1-137">在您的客戶簽署合約之後，您就可以在您的集中式合作夥伴租用戶底下重新建立他們的訂閱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="ccda1-138">從**合作夥伴中心**選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="ccda1-138">From the **Partner Center** select **Customers**.</span></span>

3.  <span data-ttu-id="ccda1-139">開啟您要移轉之客戶的公司名稱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-139">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="ccda1-140">按一下 **\[新增訂閱\]** 。</span><span class="sxs-lookup"><span data-stu-id="ccda1-140">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="ccda1-141">從目錄新增正確的訂閱與基座數目。</span><span class="sxs-lookup"><span data-stu-id="ccda1-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="ccda1-142">檢視 **\[轉換來源\]** 合作夥伴帳戶中提供的資訊。</span><span class="sxs-lookup"><span data-stu-id="ccda1-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

![客戶清單](images/regionalcustomer2.png)

6.  <span data-ttu-id="ccda1-144">按一下 **\[送出\]** 。</span><span class="sxs-lookup"><span data-stu-id="ccda1-144">Click **Submit.**</span></span>

<span data-ttu-id="ccda1-145">服務現在就會提供給來自 **\[轉換至\]** 合作夥伴帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ccda1-146">請重複這些步驟來移轉所有其他客戶的訂閱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="ccda1-147">在繼續到下一節之前，請確定存在於 \[轉換來源\] 合作夥伴帳戶底下的所有客戶訂閱，都已經在 \[轉換至\] 合作夥伴帳戶底下重新佈建。</span><span class="sxs-lookup"><span data-stu-id="ccda1-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="ccda1-148">**注意**：合作夥伴必須在轉換那些訂閱的同一天，於合作夥伴中心中的 \[轉換來源\] 合作夥伴租用戶帳戶上暫停訂閱，然後在合作夥伴中心中的 \[轉換至\] 合作夥伴租用戶帳戶底下設定，以確保不會發生重複收費。</span><span class="sxs-lookup"><span data-stu-id="ccda1-148">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ccda1-149">如果因為未正確設定要停用的 \[轉換來源\] 訂閱而發生任何重疊帳單，點數的支援要求將會被拒絕。</span><span class="sxs-lookup"><span data-stu-id="ccda1-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>



## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="ccda1-150">停用 \[轉換來源\] 合作夥伴帳戶底下的 Office 365 訂閱</span><span class="sxs-lookup"><span data-stu-id="ccda1-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="ccda1-151">停用 **\[轉換來源\]** 合作夥伴帳戶底下的雲端解決方案提供者訂閱會停止產生任何未來的帳單。</span><span class="sxs-lookup"><span data-stu-id="ccda1-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="ccda1-152">您不需要手動停用 Azrue 訂閱，因為 Azure 訂閱會在移轉過程中自動停用。</span><span class="sxs-lookup"><span data-stu-id="ccda1-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="ccda1-153">使用 [**從 CSP 轉換**] 帳戶登入**合作夥伴中心**，並流覽至 [客戶] 清單。</span><span class="sxs-lookup"><span data-stu-id="ccda1-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="ccda1-154">開啟含有要停用之訂閱的客戶，然後選取第一項要停用的服務。</span><span class="sxs-lookup"><span data-stu-id="ccda1-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="ccda1-155">將訂閱設定為 **\[暫停\]** ，然後按一下 **\[送出\]** 。</span><span class="sxs-lookup"><span data-stu-id="ccda1-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

 >[!**注意**]<span data-ttu-id="ccda1-156">暫停訂閱可確保不會進行雙重計費。</span><span class="sxs-lookup"><span data-stu-id="ccda1-156"> Suspending the subscription ensures double billing does not occur.</span></span>



~~~
The Subscription shows **suspended** on the subscriptions list.
~~~

4.  <span data-ttu-id="ccda1-157">請針對客戶底下的所有訂閱重複這些步驟。</span><span class="sxs-lookup"><span data-stu-id="ccda1-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="ccda1-158">確認全部顯示 \[暫停\]。</span><span class="sxs-lookup"><span data-stu-id="ccda1-158">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="ccda1-159">選取清單中的下一個客戶，並重複停用所有訂閱的程序。</span><span class="sxs-lookup"><span data-stu-id="ccda1-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="ccda1-160">移轉 Azure 用量型訂閱</span><span class="sxs-lookup"><span data-stu-id="ccda1-160">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="ccda1-161">請注意，Azure 用量型雲端解決方案提供者訂閱不需要像 Office 365 雲端解決方案提供者訂閱一樣手動移轉。</span><span class="sxs-lookup"><span data-stu-id="ccda1-161">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="ccda1-162">Microsoft Azure 支援可以將 Azure 訂閱和所有部署的服務或資源從 \[轉換來源\] 雲端解決方案提供者經銷商帳戶移轉至 \[轉換至\] 雲端解決方案提供者經銷商帳戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-162">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="ccda1-163">轉換期間對客戶的服務不會中斷。</span><span class="sxs-lookup"><span data-stu-id="ccda1-163">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="ccda1-164">請確定需要移轉 Azure 訂閱的客戶帳戶已經接受要與新的 \[轉換至\] 雲端解決方案提供者帳戶關聯的合約。</span><span class="sxs-lookup"><span data-stu-id="ccda1-164">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="ccda1-165">合作夥伴會通知 Microsoft 具有 Azure 訂用帳戶的客戶帳戶已準備好進行遷移，並提供這些客戶的公司名稱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-165">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>
3.  <span data-ttu-id="ccda1-166">Microsoft 移轉 Azure 用量型訂閱並在移轉完成時通知合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="ccda1-166">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="ccda1-167">合作夥伴確認 **\[轉換來源\]** 雲端解決方案提供者經銷商帳戶底下的 Azure 訂閱，現在在合作夥伴中心的客戶訂閱區段底下顯示為 \[暫停\]。</span><span class="sxs-lookup"><span data-stu-id="ccda1-167">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="ccda1-168">合作夥伴確認 **\[轉換至\]** 雲端解決方案提供者經銷商帳戶底下的 Azure 訂閱，在合作夥伴中心的客戶訂閱區段底下顯示 **\[作用中\]** 狀態。</span><span class="sxs-lookup"><span data-stu-id="ccda1-168">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

>[!**注意**]<span data-ttu-id="ccda1-169">停用客戶下的訂用帳戶並不會變更客戶在 Customers 清單中的外觀。</span><span class="sxs-lookup"><span data-stu-id="ccda1-169"> Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="ccda1-170">目前沒有將客戶從清單移除的選項。</span><span class="sxs-lookup"><span data-stu-id="ccda1-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="ccda1-171">合作夥伴未來應避免從客戶的 **\[轉換來源\]** 帳戶將訂閱加回給這些客戶。</span><span class="sxs-lookup"><span data-stu-id="ccda1-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>



6.  <span data-ttu-id="ccda1-172">請針對您所有客戶底下的所有訂閱重複這些步驟，以停止未來在 **\[轉換來源\]** 帳戶上收費。</span><span class="sxs-lookup"><span data-stu-id="ccda1-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="ccda1-173">合作夥伴將會收到一份最終發票，其中包含取消日期到計費期間最後一天之間未使用天數的點數。</span><span class="sxs-lookup"><span data-stu-id="ccda1-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="ccda1-174">未來在該最終計費期間之後將不會再產生發票。</span><span class="sxs-lookup"><span data-stu-id="ccda1-174">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="ccda1-175">注意事項</span><span class="sxs-lookup"><span data-stu-id="ccda1-175">Notes</span></span>

-   <span data-ttu-id="ccda1-176">從 [**從 CSP 轉換**] 帳戶停用訂閱並不會影響終端客戶的服務，前提是在停用之前，已從**轉換到**CSP 帳戶布建服務。</span><span class="sxs-lookup"><span data-stu-id="ccda1-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="ccda1-177">暫停或取消訂閱之後，客戶就無法使用訂閱，並且不會產生費用。</span><span class="sxs-lookup"><span data-stu-id="ccda1-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="ccda1-178">目前沒有任何方式可以將客戶完全從客戶清單中移除。</span><span class="sxs-lookup"><span data-stu-id="ccda1-178">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="ccda1-179">**注意**：合作夥伴必須在轉換那些訂閱的同一天，於合作夥伴中心中的 \[轉換來源\] 合作夥伴租用戶帳戶上暫停訂閱，然後在合作夥伴中心中的 \[轉換至\] 合作夥伴租用戶帳戶底下設定，以確保不會發生重複收費。</span><span class="sxs-lookup"><span data-stu-id="ccda1-179">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="ccda1-180">如果因為未正確設定要暫停的 \[轉換來源\] 訂閱而發生任何重疊帳單，Microsoft 將不會支援對點數的要求。</span><span class="sxs-lookup"><span data-stu-id="ccda1-180">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>



### <a name="simplify-migration-using-export"></a><span data-ttu-id="ccda1-181">使用匯出功能簡化移轉</span><span class="sxs-lookup"><span data-stu-id="ccda1-181">Simplify migration using Export</span></span>

<span data-ttu-id="ccda1-182">使用 \[匯出功能\]，您就可以擷取您需要在新的合併結構中使用的訂閱：</span><span class="sxs-lookup"><span data-stu-id="ccda1-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="ccda1-183">按一下 [合作夥伴中心] 上的 [**客戶**]，以查看現有結構中的客戶清單。</span><span class="sxs-lookup"><span data-stu-id="ccda1-183">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="ccda1-184">開啟想查看之客戶的名稱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-184">Open the desired customer name.</span></span>

3.  <span data-ttu-id="ccda1-185">在 **\[訂閱\]** 頁面上，按一下 **\[匯出訂閱\]** 來將訂閱的詳細資料匯出到 Excel 檔案。</span><span class="sxs-lookup"><span data-stu-id="ccda1-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="ccda1-186">請使用此清單在您新的合併租用戶中重新建立訂閱。</span><span class="sxs-lookup"><span data-stu-id="ccda1-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="ccda1-187">API 註冊</span><span class="sxs-lookup"><span data-stu-id="ccda1-187">API registration</span></span>

<span data-ttu-id="ccda1-188">如需 API 註冊的詳細資訊，請[參閱此頁面](https://go.microsoft.com/fwlink/?linkid=847990)。</span><span class="sxs-lookup"><span data-stu-id="ccda1-188">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>








