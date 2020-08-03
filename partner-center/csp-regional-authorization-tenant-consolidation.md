---
title: 雲端解決方案提供者地區授權租用戶彙總
ms.topic: article
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 請依照下列指示合併不同國家/地區的租用戶。 這包括遷移客戶帳戶和客戶訂閱的步驟。
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 4389ed675bfc7186aa19e595b14ac9200334c61c
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444928"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="a0e41-104">雲端解決方案提供者地區授權租用戶彙總簡介</span><span class="sxs-lookup"><span data-stu-id="a0e41-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="a0e41-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="a0e41-105">**Applies to**</span></span>

-  <span data-ttu-id="a0e41-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a0e41-106">Partner Center</span></span>
-  <span data-ttu-id="a0e41-107">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a0e41-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a0e41-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="a0e41-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a0e41-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a0e41-109">Global admin</span></span>
- <span data-ttu-id="a0e41-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="a0e41-110">Admin agent</span></span>

<span data-ttu-id="a0e41-111">\[某些資訊與預先發行的產品有關，在正式發行之前，可能會大幅修改。</span><span class="sxs-lookup"><span data-stu-id="a0e41-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="a0e41-112">針對此處提供的資訊，Microsoft 不做任何明示或默許的擔保。\]</span><span class="sxs-lookup"><span data-stu-id="a0e41-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="a0e41-113">您可以為您的企業合併租使用者。</span><span class="sxs-lookup"><span data-stu-id="a0e41-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="a0e41-114">請依照下列指示合併不同國家/地區的租用戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="a0e41-115">您必須知道您要轉換的帳戶中，每個客戶的所有布建訂閱和授權計數。</span><span class="sxs-lookup"><span data-stu-id="a0e41-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="a0e41-116">在遷移過程中，您將會在新的中央 CSP 帳戶底下，以相同的授權計數重新布建那些相同的正確訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="a0e41-117">請使用匯出清單功能來協助建立要移到集中式租用戶之客戶的清單。</span><span class="sxs-lookup"><span data-stu-id="a0e41-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="a0e41-118">合併完成後，您就無法還原為先前的租使用者狀態。</span><span class="sxs-lookup"><span data-stu-id="a0e41-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="a0e41-119">可能也需要客戶動作。</span><span class="sxs-lookup"><span data-stu-id="a0e41-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="a0e41-120">為移轉做準備</span><span class="sxs-lookup"><span data-stu-id="a0e41-120">Prepare for migration</span></span>

- <span data-ttu-id="a0e41-121">使用**轉換**的帳戶（您將轉換至新帳戶的帳戶）登入**合作夥伴中心**，並查看所有客戶和為這些客戶布建的所有服務。</span><span class="sxs-lookup"><span data-stu-id="a0e41-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="a0e41-122">登出此帳戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="a0e41-123">移轉客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="a0e41-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="a0e41-124">使用**轉換**（新）帳戶（您要將客戶轉換成其中一項）來登入**合作夥伴中心**。</span><span class="sxs-lookup"><span data-stu-id="a0e41-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="a0e41-125">選取 [客戶]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-125">Select **Customers**.</span></span>

3. <span data-ttu-id="a0e41-126">按一下 [**要求轉銷商關聯**性]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="a0e41-127">系統會顯示您要傳送給客戶的預設電子郵件訊息。</span><span class="sxs-lookup"><span data-stu-id="a0e41-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="a0e41-128">此訊息包含一個 URL，其中包含您新的合作夥伴中心帳戶唯一的組織識別碼。</span><span class="sxs-lookup"><span data-stu-id="a0e41-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="a0e41-129">**客戶動作：** 確保您要移轉的每個作用中客戶都會造訪此 URL。</span><span class="sxs-lookup"><span data-stu-id="a0e41-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="a0e41-130">開啟 URL 時，會提示客戶登入 Office 365 入口網站。</span><span class="sxs-lookup"><span data-stu-id="a0e41-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="a0e41-131">客戶使用和用來存取 Azure 及 Office 365 管理入口網站時相同的組織識別碼登入。</span><span class="sxs-lookup"><span data-stu-id="a0e41-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="a0e41-132">登入之後，系統會提示**客戶帳戶**的全域管理員提交合約，以提供委派系統管理員許可權給新的 CSP 帳戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="a0e41-133">如果他們同意，客戶就能選取核取方塊並同意授權關係。</span><span class="sxs-lookup"><span data-stu-id="a0e41-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="a0e41-134">當客戶提交合約之後，就會出現在合作夥伴的客戶清單中。</span><span class="sxs-lookup"><span data-stu-id="a0e41-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="a0e41-135">移轉 Office 365 和非 Azure 用量型訂閱</span><span class="sxs-lookup"><span data-stu-id="a0e41-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="a0e41-136">在您的客戶簽署合約之後，您就可以在您的集中式合作夥伴租用戶底下重新建立他們的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="a0e41-137">從**合作夥伴中心**選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="a0e41-138">開啟您要移轉之客戶的公司名稱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="a0e41-139">選取 [訂用帳戶]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="a0e41-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="a0e41-140">從目錄新增正確的訂用帳戶和授權計數。</span><span class="sxs-lookup"><span data-stu-id="a0e41-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="a0e41-141">請使用從合作夥伴帳戶**轉換**中提供的資訊進行驗證。</span><span class="sxs-lookup"><span data-stu-id="a0e41-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="客戶清單":::

6. <span data-ttu-id="a0e41-143">按一下 [**提交]。**</span><span class="sxs-lookup"><span data-stu-id="a0e41-143">Click **Submit.**</span></span>

   <span data-ttu-id="a0e41-144">服務現在會從**轉換到**合作夥伴帳戶提供給客戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="a0e41-145">請重複這些步驟來移轉所有其他客戶的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="a0e41-146">在繼續到下一節之前，請確定存在於 **\[轉換來源\]** 合作夥伴帳戶底下的所有客戶訂閱，都已經在 **\[轉換至\]** 合作夥伴帳戶底下重新佈建。</span><span class="sxs-lookup"><span data-stu-id="a0e41-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="a0e41-147">合作夥伴必須在合作夥伴中心的 [從合作夥伴] 租使用者帳戶**轉換**時暫停訂閱，並在合作夥伴中心的 [**轉換至**合作夥伴租使用者帳戶] 下設定這些訂用帳戶，以確保不會發生雙重計費。</span><span class="sxs-lookup"><span data-stu-id="a0e41-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="a0e41-148">由於未正確停用訂用帳戶的**轉換**，因此會拒絕信用額度的支援要求。</span><span class="sxs-lookup"><span data-stu-id="a0e41-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="a0e41-149">停用 \[轉換來源\] 合作夥伴帳戶底下的 Office 365 訂閱</span><span class="sxs-lookup"><span data-stu-id="a0e41-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="a0e41-150">在從合作夥伴帳戶**轉換**下停用 CSP 訂用帳戶，會停止任何未來的帳單。</span><span class="sxs-lookup"><span data-stu-id="a0e41-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="a0e41-151">您不需要手動停用 Azure 訂用帳戶，因為在遷移過程中會自動停用 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="a0e41-152">使用 [**從 CSP 轉換**] 帳戶登入**合作夥伴中心**，並流覽至 [客戶] 清單。</span><span class="sxs-lookup"><span data-stu-id="a0e41-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="a0e41-153">開啟含有要停用之訂閱的客戶，然後選取第一項要停用的服務。</span><span class="sxs-lookup"><span data-stu-id="a0e41-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="a0e41-154">將 [訂用帳戶] 設定為 [已**暫停**]，然後按一下 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="a0e41-155">暫停訂閱可確保不會進行雙重計費。</span><span class="sxs-lookup"><span data-stu-id="a0e41-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="a0e41-156">訂閱會在訂用帳戶清單上顯示 [已**暫停**]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="a0e41-157">請針對客戶底下的所有訂閱重複這些步驟。</span><span class="sxs-lookup"><span data-stu-id="a0e41-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="a0e41-158">確認全部顯示 **\[暫停\]**。</span><span class="sxs-lookup"><span data-stu-id="a0e41-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="a0e41-159">選取清單中的下一個客戶，並重複停用所有訂閱的程序。</span><span class="sxs-lookup"><span data-stu-id="a0e41-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="a0e41-160">移轉 Azure 用量型訂閱</span><span class="sxs-lookup"><span data-stu-id="a0e41-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="a0e41-161">不同于 Office 365 CSP 訂用帳戶，Azure，以使用方式為基礎的 CSP 訂用帳戶不需要手動遷移。</span><span class="sxs-lookup"><span data-stu-id="a0e41-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="a0e41-162">Microsoft Azure 支援會將 Azure 訂用帳戶以及所有已部署的服務或資源，從從 CSP 轉銷商帳戶**轉換**到**轉換為**csp 轉銷商帳戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="a0e41-163">轉換期間對客戶的服務不會中斷。</span><span class="sxs-lookup"><span data-stu-id="a0e41-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="a0e41-164">請確定將會遷移 Azure 訂用帳戶的客戶帳戶已接受合約，使其與新**轉換至**CSP 帳戶相關聯。</span><span class="sxs-lookup"><span data-stu-id="a0e41-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="a0e41-165">您會通知 Microsoft 哪些客戶帳戶已準備好進行遷移，並提供這些客戶的公司名稱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="a0e41-166">Microsoft 會遷移以 Azure 使用量為基礎的訂用帳戶，並在遷移完成時通知您。</span><span class="sxs-lookup"><span data-stu-id="a0e41-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="a0e41-167">您必須確認在合作夥伴中心的 [客戶訂**用**帳戶] 區段下，已將 Azure 訂用帳戶從 CSP 轉銷商帳戶轉換為 [已**暫停**]。</span><span class="sxs-lookup"><span data-stu-id="a0e41-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="a0e41-168">確認在 [正在**轉換至**CSP 轉銷商帳戶] 下的 Azure 訂用帳戶現在在 [合作夥伴中心] 的 [客戶訂閱] 區段底下顯示 [**作用中]** 狀態。</span><span class="sxs-lookup"><span data-stu-id="a0e41-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="a0e41-169">停用客戶下的訂用帳戶並不會變更客戶在 Customers 清單中的外觀。</span><span class="sxs-lookup"><span data-stu-id="a0e41-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="a0e41-170">目前沒有將客戶從清單移除的選項。</span><span class="sxs-lookup"><span data-stu-id="a0e41-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="a0e41-171">合作夥伴應避免將訂用帳戶從他們在未來的**轉換中**，新增回給這些客戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="a0e41-172">針對所有客戶下的所有訂用帳戶，重複這些步驟，以停止未來**從帳戶轉換**的費用。</span><span class="sxs-lookup"><span data-stu-id="a0e41-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="a0e41-173">合作夥伴將會收到一份最終發票，其中包含取消日期到計費期間最後一天之間未使用天數的點數。</span><span class="sxs-lookup"><span data-stu-id="a0e41-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="a0e41-174">未來在該最終計費期間之後將不會再產生發票。</span><span class="sxs-lookup"><span data-stu-id="a0e41-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="a0e41-175">其他資訊</span><span class="sxs-lookup"><span data-stu-id="a0e41-175">Additional information</span></span>

- <span data-ttu-id="a0e41-176">只要服務是在停用訂用帳戶之前，從**轉換為**csp 帳戶布建，則從 csp 帳戶的**轉換**中停用訂閱並不會影響終端客戶的服務。</span><span class="sxs-lookup"><span data-stu-id="a0e41-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="a0e41-177">訂用帳戶無法供客戶使用，且在暫停或取消時不會產生費用。</span><span class="sxs-lookup"><span data-stu-id="a0e41-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="a0e41-178">目前沒有任何方法可以完全從**客戶**清單移除客戶。</span><span class="sxs-lookup"><span data-stu-id="a0e41-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="a0e41-179">合作夥伴必須在合作夥伴中心的 [從合作夥伴] 租使用者帳戶**轉換**時暫停訂閱，而這些訂用帳戶會轉換成，並在 [**轉換成**] 帳戶下設定，以確保不會發生雙重計費。</span><span class="sxs-lookup"><span data-stu-id="a0e41-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="a0e41-180">由於未正確設定從訂用帳戶**轉換**為暫停的計費，Microsoft 不會支援信用額度的要求。</span><span class="sxs-lookup"><span data-stu-id="a0e41-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="a0e41-181">使用匯出功能簡化移轉</span><span class="sxs-lookup"><span data-stu-id="a0e41-181">Simplify migration using Export</span></span>

<span data-ttu-id="a0e41-182">使用 **\[匯出功能\]**，您就可以擷取您需要在新的合併結構中使用的訂閱：</span><span class="sxs-lookup"><span data-stu-id="a0e41-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="a0e41-183">按一下 [合作夥伴中心] 上的 [**客戶**]，以查看客戶的清單。</span><span class="sxs-lookup"><span data-stu-id="a0e41-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="a0e41-184">開啟想查看之客戶的名稱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="a0e41-185">在 [**訂閱**] 頁面上，按一下 [**匯出訂閱**]，將訂閱的詳細資料匯出至 Excel 檔案。</span><span class="sxs-lookup"><span data-stu-id="a0e41-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="a0e41-186">請使用此清單在您新的合併租用戶中重新建立訂閱。</span><span class="sxs-lookup"><span data-stu-id="a0e41-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="a0e41-187">API 註冊</span><span class="sxs-lookup"><span data-stu-id="a0e41-187">API registration</span></span>

<span data-ttu-id="a0e41-188">如需 API 註冊的詳細資訊，請參閱[在合作夥伴中心設定 api 存取](https://go.microsoft.com/fwlink/?linkid=847990)。</span><span class="sxs-lookup"><span data-stu-id="a0e41-188">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a0e41-189">後續步驟</span><span class="sxs-lookup"><span data-stu-id="a0e41-189">Next steps</span></span>

- [<span data-ttu-id="a0e41-190">合作夥伴中心內轉售商合作夥伴的客戶帳戶設定和管理</span><span class="sxs-lookup"><span data-stu-id="a0e41-190">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)
