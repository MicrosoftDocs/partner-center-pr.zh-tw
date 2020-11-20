---
title: Dynamics 365 CRM 的共同銷售連接器合作夥伴中心
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 將合作夥伴中心中的推薦與 Dynamics 365 CRM 的共同銷售連接器同步處理。 然後，銷售人員可以從您的 CRM 系統內與 Microsoft 共同銷售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947738"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="59b55-104">Dynamics 365 CRM 的共同銷售連接器–總覽</span><span class="sxs-lookup"><span data-stu-id="59b55-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="59b55-105">適當的角色</span><span class="sxs-lookup"><span data-stu-id="59b55-105">Appropriate roles</span></span>

- <span data-ttu-id="59b55-106">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="59b55-106">Referrals admin</span></span>
- <span data-ttu-id="59b55-107">CRM 上的系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="59b55-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="59b55-108">合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。</span><span class="sxs-lookup"><span data-stu-id="59b55-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="59b55-109">他們不需要訓練以使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="59b55-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="59b55-110">使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。</span><span class="sxs-lookup"><span data-stu-id="59b55-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="59b55-111">您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="59b55-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="59b55-112">您可以在您選擇的 CRM 中，而不是在合作夥伴中心中，執行所有的參考工作。</span><span class="sxs-lookup"><span data-stu-id="59b55-112">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="59b55-113">解決方案是以 Microsoft Power Automate 解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="59b55-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="59b55-114">安裝之前的先決條件</span><span class="sxs-lookup"><span data-stu-id="59b55-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="59b55-115">**主題**</span><span class="sxs-lookup"><span data-stu-id="59b55-115">**Topics**</span></span>   |<span data-ttu-id="59b55-116">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="59b55-116">**Details**</span></span>   |<span data-ttu-id="59b55-117">**連結**</span><span class="sxs-lookup"><span data-stu-id="59b55-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="59b55-118">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="59b55-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="59b55-119">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="59b55-119">You need a valid MPN ID</span></span>|<span data-ttu-id="59b55-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="59b55-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="59b55-121">共同銷售解決方案就緒</span><span class="sxs-lookup"><span data-stu-id="59b55-121">Cosell ready</span></span>|<span data-ttu-id="59b55-122">您的 IP/服務解決方案必須已準備好共同銷售。</span><span class="sxs-lookup"><span data-stu-id="59b55-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="59b55-123">與 Microsoft 銷售</span><span class="sxs-lookup"><span data-stu-id="59b55-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="59b55-124">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="59b55-124">Partner Center account</span></span>|<span data-ttu-id="59b55-125">與合作夥伴中心租使用者相關聯的 MPN 識別碼必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="59b55-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="59b55-126">先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。</span><span class="sxs-lookup"><span data-stu-id="59b55-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="59b55-127">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="59b55-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="59b55-128">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="59b55-128">Partner Center user roles</span></span>|<span data-ttu-id="59b55-129">將安裝並使用連接器的員工必須是推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="59b55-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="59b55-130">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="59b55-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="59b55-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="59b55-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="59b55-132">CRM 使用者角色是系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="59b55-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="59b55-133">在 Dynamics 365 中指派角色</span><span class="sxs-lookup"><span data-stu-id="59b55-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="59b55-134">Power Automate Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="59b55-134">Power Automate Flow Account</span></span>|<span data-ttu-id="59b55-135">適用于 CRM 系統管理員或系統自訂員的 active [Power Automate](https://flow.microsoft.com) 帳戶。</span><span class="sxs-lookup"><span data-stu-id="59b55-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="59b55-136">在安裝之前，該使用者至少應登入 [Power Automate](https://flow.microsoft.com) 一次。</span><span class="sxs-lookup"><span data-stu-id="59b55-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="59b55-137">為 Dynamics 365 (Power Automate 解決方案) 安裝合作夥伴中心的推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="59b55-137">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="59b55-138">移至 [Power Automate](https://flow.microsoft.com) ，然後在右上角選取 [ **環境** ]。</span><span class="sxs-lookup"><span data-stu-id="59b55-138">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="59b55-139">此步驟會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="59b55-139">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="59b55-140">從右上角的下拉式清單中選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="59b55-140">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="59b55-141">選取左側導覽列上的 [ **方案** ]。</span><span class="sxs-lookup"><span data-stu-id="59b55-141">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="59b55-142">按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="59b55-142">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="59b55-144">在快顯視窗中搜尋 **合作夥伴中心的 Dynamics365 參考連接器以進行** 。</span><span class="sxs-lookup"><span data-stu-id="59b55-144">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="59b55-145">按一下 [ **立即取得** ] 按鈕，然後 **繼續** 進行。</span><span class="sxs-lookup"><span data-stu-id="59b55-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="59b55-146">這會開啟頁面，您可以在其中選取 CRM (Dynamics 365) 環境以安裝應用程式。</span><span class="sxs-lookup"><span data-stu-id="59b55-146">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="59b55-147">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="59b55-147">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="59b55-148">然後，系統會將您導向至 [ **管理您的解決方案** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="59b55-148">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="59b55-149">使用頁面底部的箭號按鈕，流覽至「合作夥伴中心的推薦」。</span><span class="sxs-lookup"><span data-stu-id="59b55-149">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="59b55-150">已 **排程的安裝** 應該會出現在合作夥伴中心的推薦解決方案旁邊。</span><span class="sxs-lookup"><span data-stu-id="59b55-150">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="59b55-151">安裝將需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="59b55-151">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="59b55-152">安裝完成之後，請流覽回到 [Power Automate](https://flow.microsoft.com) ，然後從左側導覽區域選取 **解決方案** 。</span><span class="sxs-lookup"><span data-stu-id="59b55-152">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="59b55-153">請注意，您可以在 [方案] 清單中找到 **Dynamics 365 的合作夥伴中心推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-153">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="59b55-154">選取 **合作夥伴中心 Dynamics 365 的推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-154">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="59b55-155">以下是可用的流程和實體 Power Automate：</span><span class="sxs-lookup"><span data-stu-id="59b55-155">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用的 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="59b55-157">最佳做法：上線之前先進行測試</span><span class="sxs-lookup"><span data-stu-id="59b55-157">Best practice: test before you go live</span></span>

<span data-ttu-id="59b55-158">在生產環境中安裝、設定和自訂 Power Automate 解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="59b55-158">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="59b55-159">在預備環境/CRM 實例上安裝 Microsoft Power Automate 的解決方案。</span><span class="sxs-lookup"><span data-stu-id="59b55-159">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="59b55-160">製作解決方案的複本，並在預備環境中執行設定和 Power Automate 流程自訂。</span><span class="sxs-lookup"><span data-stu-id="59b55-160">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="59b55-161">測試預備/CRM 實例上的方案。</span><span class="sxs-lookup"><span data-stu-id="59b55-161">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="59b55-162">成功時，請將受控解決方案匯入至生產環境實例。</span><span class="sxs-lookup"><span data-stu-id="59b55-162">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="59b55-163">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="59b55-163">Configure the solution</span></span>

1. <span data-ttu-id="59b55-164">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power Automate](https://flow.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="59b55-164">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="59b55-165">從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power Automate 解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="59b55-165">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="59b55-166">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="59b55-166">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="59b55-167">具有推薦系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="59b55-167">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="59b55-168">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="59b55-168">Partner Center Events</span></span>

   - <span data-ttu-id="59b55-169">CRM 管理員與解決方案中的 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="59b55-169">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="59b55-170">從左側導覽列選取 [ **連接** ]，然後從清單中選取 [合作夥伴中心的參考] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="59b55-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="59b55-171">按一下 [ **建立連接**] 來建立連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-171">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="建立連線":::

      3. <span data-ttu-id="59b55-173">在右上角的搜尋列中搜尋 **合作夥伴中心參考 (預覽)** 。</span><span class="sxs-lookup"><span data-stu-id="59b55-173">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="59b55-174">使用「參考系統管理員」的認證角色建立合作夥伴中心使用者的連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-174">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="59b55-175">接下來，使用推薦的系統管理員認證來為您的合作夥伴中心使用者建立合作夥伴中心事件連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-175">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="59b55-176">為 CRM 系統管理員使用者建立 Common Data Service (目前環境) 的連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-176">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
       
     
      7. <span data-ttu-id="59b55-177">新增所有連線之後，您應該會在您的環境中看到下列連接：</span><span class="sxs-lookup"><span data-stu-id="59b55-177">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="連線":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="59b55-179">編輯連接</span><span class="sxs-lookup"><span data-stu-id="59b55-179">Edit the connections</span></span>

1. <span data-ttu-id="59b55-180">返回 [ **方案** ] 頁面，然後選取 [ **預設方案**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-180">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="59b55-181">按一下 [**全部**]，以選取 [ **(預覽) 的連接參考**。</span><span class="sxs-lookup"><span data-stu-id="59b55-181">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="[連接]":::

2. <span data-ttu-id="59b55-183">選取三個點圖示，逐一編輯每一個連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-183">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="59b55-184">新增相關的連接。</span><span class="sxs-lookup"><span data-stu-id="59b55-184">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="列出的連接"::: 

3.  <span data-ttu-id="59b55-186">依下列順序開啟流程：</span><span class="sxs-lookup"><span data-stu-id="59b55-186">Turn on the flows in the following sequence:</span></span>
- <span data-ttu-id="59b55-187">合作夥伴中心 Webhook 註冊 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="59b55-187">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="59b55-188">建立共同銷售參考– Dynamics 365 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="59b55-188">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59b55-189">合作夥伴中心 Microsoft 共同銷售參考更新至 Dynamics 365 (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="59b55-189">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="59b55-190">合作夥伴中心至 Dynamics 365 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="59b55-190">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="59b55-191">Dynamics 365 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="59b55-191">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59b55-192">Dynamics 365 (Insider preview 的合作夥伴中心機會) </span><span class="sxs-lookup"><span data-stu-id="59b55-192">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="59b55-193">可合作夥伴中心 (Insider Preview) 的 Dynamics 365 Microsoft 解決方案</span><span class="sxs-lookup"><span data-stu-id="59b55-193">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="59b55-194">使用 Webhook Api 來註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="59b55-194">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="59b55-195">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="59b55-195">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="59b55-196">這些變更事件會以 HTTP 文章的形式傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="59b55-196">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="59b55-197">若要註冊您的 url，請選取 **合作夥伴中心 Webhook 註冊 (Insider preview)** Power Automate flow。</span><span class="sxs-lookup"><span data-stu-id="59b55-197">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="59b55-198">新增 (的連接。 ) 合作夥伴中心具有推薦的系統管理員認證的使用者 (b. ) 合作夥伴中心事件，如下所強調</span><span class="sxs-lookup"><span data-stu-id="59b55-198">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. <span data-ttu-id="59b55-200">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="59b55-200">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="59b55-202">儲存您的變更，然後選取 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-202">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="59b55-203">若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="59b55-203">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="59b55-204">選取 **合作夥伴中心至 Dynamics 365 (Insider preview)**。</span><span class="sxs-lookup"><span data-stu-id="59b55-204">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="59b55-205">選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-205">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="59b55-206">選取 **複製** 圖示來複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="59b55-206">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="複製 URL":::

8. <span data-ttu-id="59b55-208">現在，選取 [合作夥伴中心 Webhook 註冊 (Insider Preview) ] Power Automate 流程，然後選取 [ **執行**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-208">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="59b55-209">確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-209">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="59b55-210">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="59b55-210">Enter the following details:</span></span>

    1. <span data-ttu-id="59b55-211">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="59b55-211">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="59b55-212">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="59b55-212">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="59b55-213">**覆寫現有的觸發程式端點（如果有的話**）：是 (這會覆寫任何現有的端點。 ) </span><span class="sxs-lookup"><span data-stu-id="59b55-213">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="59b55-214">選取 [ **執行** ]，然後選取 [ **完成]。**</span><span class="sxs-lookup"><span data-stu-id="59b55-214">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="59b55-215">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="59b55-215">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="59b55-216">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="59b55-216">Customize synchronization steps</span></span>

<span data-ttu-id="59b55-217">當共同銷售的參考在合作夥伴中心與您的 CRM 系統之間進行同步處理時，在合作夥伴中心電腦上同步的欄位會列在此處。</span><span class="sxs-lookup"><span data-stu-id="59b55-217">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="59b55-218">通常會高度自訂 CRM 系統。</span><span class="sxs-lookup"><span data-stu-id="59b55-218">Often CRM systems are highly customized.</span></span> <span data-ttu-id="59b55-219">您可以自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="59b55-219">You can customize the Power Automate flows.</span></span> <span data-ttu-id="59b55-220">依照欄位對應指南操作，如有必要，請在 Power Automate 流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="59b55-220">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="59b55-221">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="59b55-221">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="59b55-222">您可以根據自己的需求自訂每個 Power Automate 流程的多個步驟。</span><span class="sxs-lookup"><span data-stu-id="59b55-222">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="59b55-223">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="59b55-223">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="59b55-224">若要自訂合作夥伴中心中的建立或更新事件的欄位以進行 CRM 推薦同步處理：</span><span class="sxs-lookup"><span data-stu-id="59b55-224">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="59b55-225">a.</span><span class="sxs-lookup"><span data-stu-id="59b55-225">a.</span></span> <span data-ttu-id="59b55-226">選取合作夥伴中心至 Dynamics 365 (Insider preview) 或合作夥伴中心至 Salesforce (Insider preview) 。</span><span class="sxs-lookup"><span data-stu-id="59b55-226">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="59b55-227">b.</span><span class="sxs-lookup"><span data-stu-id="59b55-227">b.</span></span> <span data-ttu-id="59b55-228">選取 [ **編輯** ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="59b55-228">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="59b55-229">c.</span><span class="sxs-lookup"><span data-stu-id="59b55-229">c.</span></span> <span data-ttu-id="59b55-230">選取 **(範圍) 同步處理潛在客戶或商機**。</span><span class="sxs-lookup"><span data-stu-id="59b55-230">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="59b55-231">若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 **它是否為新的共用商機，然後**。</span><span class="sxs-lookup"><span data-stu-id="59b55-231">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="59b55-232">若為 [ **是]** ，請選取子步驟，然後 **在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-232">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="59b55-233">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="59b55-233">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="59b55-234">d.</span><span class="sxs-lookup"><span data-stu-id="59b55-234">d.</span></span> <span data-ttu-id="59b55-235">若要根據 [更新事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請按一下 [ (範圍) 同步處理潛在客戶或商機] 步驟。</span><span class="sxs-lookup"><span data-stu-id="59b55-235">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="59b55-236">e.</span><span class="sxs-lookup"><span data-stu-id="59b55-236">e.</span></span> <span data-ttu-id="59b55-237">**如果這是商機的更新，請選取它**。</span><span class="sxs-lookup"><span data-stu-id="59b55-237">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="59b55-238">**如果 [是]** ，請選取 [子步驟]，然後展開 [**合作夥伴中心和 CRM 中商機物件之間的差異]，然後再** 展開。</span><span class="sxs-lookup"><span data-stu-id="59b55-238">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="59b55-239">f.</span><span class="sxs-lookup"><span data-stu-id="59b55-239">f.</span></span> <span data-ttu-id="59b55-240">選取 **[是]** ，然後選取 [**更新現有的商機**]</span><span class="sxs-lookup"><span data-stu-id="59b55-240">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="59b55-241">若要自訂更新事件的 CRM 對電腦推薦同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="59b55-241">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="59b55-242">a.</span><span class="sxs-lookup"><span data-stu-id="59b55-242">a.</span></span> <span data-ttu-id="59b55-243">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="59b55-243">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="59b55-244">b.</span><span class="sxs-lookup"><span data-stu-id="59b55-244">b.</span></span> <span data-ttu-id="59b55-245">選取 **(範圍) 同步處理商機**。</span><span class="sxs-lookup"><span data-stu-id="59b55-245">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="59b55-246">c.</span><span class="sxs-lookup"><span data-stu-id="59b55-246">c.</span></span> <span data-ttu-id="59b55-247">若要自訂 update 事件的 CRM 欄位對應，請選取 **合作夥伴中心和 CRM 中的潛在客戶物件之間是否有差異**。</span><span class="sxs-lookup"><span data-stu-id="59b55-247">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="59b55-248">d.</span><span class="sxs-lookup"><span data-stu-id="59b55-248">d.</span></span> <span data-ttu-id="59b55-249">**若為 [是]** ，請選取子步驟，然後展開 [**使用商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="59b55-249">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="59b55-250">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="59b55-250">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="59b55-251">針對建立事件自訂 CRM 對電腦推薦同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="59b55-251">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="59b55-252">a.</span><span class="sxs-lookup"><span data-stu-id="59b55-252">a.</span></span> <span data-ttu-id="59b55-253">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="59b55-253">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="59b55-254">b.</span><span class="sxs-lookup"><span data-stu-id="59b55-254">b.</span></span> <span data-ttu-id="59b55-255">選取 **(範圍) 同步處理參考。**</span><span class="sxs-lookup"><span data-stu-id="59b55-255">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="59b55-256">c.</span><span class="sxs-lookup"><span data-stu-id="59b55-256">c.</span></span> <span data-ttu-id="59b55-257">若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 [ **建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="59b55-257">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="59b55-258">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="59b55-258">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

<span data-ttu-id="59b55-259">已建立兩個環境變數：</span><span class="sxs-lookup"><span data-stu-id="59b55-259">There are two environment variables created:</span></span>

- <span data-ttu-id="59b55-260">核取記號：表示除了在合作夥伴中心與 Dynamics 365 CRM 之間雙向同步處理的商機之外，是否還需要核取記號圖示。</span><span class="sxs-lookup"><span data-stu-id="59b55-260">Checkmark: Signifies whether you would need a checkmark icon besides opportunities that are synchronized bi-directionally between Partner Center and Dynamics 365 CRM.</span></span>

- <span data-ttu-id="59b55-261">僅同步共同銷售商機：表示您是否只要同步處理共同銷售商機。</span><span class="sxs-lookup"><span data-stu-id="59b55-261">Sync co-sell opportunities only: Signifies whether you want to synchronize only Co-sell opportunities.</span></span>

<span data-ttu-id="59b55-262">您可以選擇編輯環境變數的預設值。</span><span class="sxs-lookup"><span data-stu-id="59b55-262">You can choose to edit the default value for the environment variables.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="預設值的編輯方塊":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="59b55-264">端對端雙向共同銷售推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="59b55-264">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="59b55-265">安裝、設定和自訂 Power Automate 解決方案之後，您可以測試 Dynamics 365 和合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-265">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="59b55-266">必要條件</span><span class="sxs-lookup"><span data-stu-id="59b55-266">Pre-requisites</span></span>

<span data-ttu-id="59b55-267">為了同步處理合作夥伴中心與 Dynamics 365 CRM 之間的參考，Power Automate 解決方案清楚標示 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="59b55-267">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="59b55-268">此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="59b55-268">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="59b55-269">一組自訂欄位可作為 **商機** 實體的一部分。</span><span class="sxs-lookup"><span data-stu-id="59b55-269">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="59b55-270">CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="59b55-270">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="59b55-271">下列自訂欄位應該是 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="59b55-271">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="59b55-272">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="59b55-272">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="59b55-273">**參考識別碼**： Microsoft 合作夥伴中心推薦的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="59b55-273">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="59b55-274">**參考連結**： Microsoft 合作夥伴中心中參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="59b55-274">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="59b55-275">**Microsoft 如何協助？**： microsoft 針對此推薦提供的協助</span><span class="sxs-lookup"><span data-stu-id="59b55-275">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="59b55-276">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="59b55-276">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="59b55-277">**Audit**：使用合作夥伴中心參考進行同步處理的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="59b55-277">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

<span data-ttu-id="59b55-278">更新 Dynamics 365 CRM 中的商機表單，以包含 Products 欄位的解決方案。</span><span class="sxs-lookup"><span data-stu-id="59b55-278">Update the opportunity form in Dynamics 365 CRM to include Solutions for Products field.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="商機表單":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{替代文字}":::

### <a name="scenarios"></a><span data-ttu-id="59b55-281">場景：</span><span class="sxs-lookup"><span data-stu-id="59b55-281">SCENARIOS:</span></span>

1. <span data-ttu-id="59b55-282">參考在 CRM 中建立或更新時的參考同步處理，並在合作夥伴中心中同步處理：</span><span class="sxs-lookup"><span data-stu-id="59b55-282">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="59b55-283">登入您的 Dynamics 365 CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。</span><span class="sxs-lookup"><span data-stu-id="59b55-283">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="59b55-284">當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="59b55-284">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="顯示 Dynamics 365 中 Microsoft 合作夥伴中心資訊的 [範例商機] 區段。":::

   3. <span data-ttu-id="59b55-286">若要與 Microsoft 合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="59b55-286">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="59b55-287">**與合作夥伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="59b55-287">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="59b55-288">**Microsoft 如何協助？**：請從下列專案進行選取：</span><span class="sxs-lookup"><span data-stu-id="59b55-288">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 中的 [範例商機] 區段，會顯示名為「Microsoft 如何協助」之欄位旁的 Microsoft 合作夥伴中心說明選項？":::

      - <span data-ttu-id="59b55-290">**產品**：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="59b55-290">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="59b55-291">一旦在 Dynamics 365 中建立商機，並將 [ **同步處理合作夥伴中心** ] 選項設為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="59b55-291">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="59b55-292">您的參考會與 Dynamics 365 進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-292">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="59b55-293">同樣地，如果有 [同步處理合作夥伴中心] 選項設定為 [是] 的商機，如果您更新 Dynamics 365 CRM 的商機，這些變更將會在您的合作夥伴中心帳戶中同步處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-293">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="59b55-294">使用合作夥伴中心成功同步處理的商機將會以 Dynamics 365 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="59b55-294">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="59b55-295">在 Microsoft 合作夥伴中心中建立或更新參考時的參考同步處理，並在 Dynamics 365 環境中同步處理：</span><span class="sxs-lookup"><span data-stu-id="59b55-295">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="59b55-296">登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="59b55-296">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="59b55-297">從左側功能表中選取 [ **參考** ]。</span><span class="sxs-lookup"><span data-stu-id="59b55-297">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="59b55-298">按一下 [新增交易] 選項，從合作夥伴中心建立新的共同銷售推薦。</span><span class="sxs-lookup"><span data-stu-id="59b55-298">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="59b55-299">登入您的 Dynamics 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="59b55-299">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="59b55-300">流覽至 **開啟的商機**。</span><span class="sxs-lookup"><span data-stu-id="59b55-300">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="59b55-301">在 Microsoft 合作夥伴中心中建立的參照現在已在 Dynamics 365 CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="59b55-301">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="59b55-302">當您選取同步處理的參考時，就會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="59b55-302">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="59b55-303">後續步驟</span><span class="sxs-lookup"><span data-stu-id="59b55-303">Next steps</span></span>

- [<span data-ttu-id="59b55-304">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="59b55-304">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="59b55-305">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="59b55-305">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="59b55-306">深入瞭解 Microsoft Power Automate platform？</span><span class="sxs-lookup"><span data-stu-id="59b55-306">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="59b55-307">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="59b55-307">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)