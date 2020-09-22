---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 將合作夥伴中心中的參考與 Salesforce CRM 同步處理
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 595cbba8a173eb81b4e3520d1b1b0533c4dee296
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000592"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="379ea-103">Salesforce CRM 的共同銷售連接器 – 概觀</span><span class="sxs-lookup"><span data-stu-id="379ea-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="379ea-104">適當的角色</span><span class="sxs-lookup"><span data-stu-id="379ea-104">Appropriate roles</span></span>

- <span data-ttu-id="379ea-105">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="379ea-105">Referrals admin</span></span>
- <span data-ttu-id="379ea-106">CRM 上的系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="379ea-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="379ea-107">合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。</span><span class="sxs-lookup"><span data-stu-id="379ea-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="379ea-108">他們不需要訓練以使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="379ea-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="379ea-109">您可以使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。</span><span class="sxs-lookup"><span data-stu-id="379ea-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="379ea-110">您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="379ea-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="379ea-111">在您選擇的 CRM 中工作時，您可以執行所有的參考工作，而不是在合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="379ea-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="379ea-112">解決方案是以 Microsoft Power Automate 解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="379ea-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="379ea-113">安裝之前的先決條件</span><span class="sxs-lookup"><span data-stu-id="379ea-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="379ea-114">**主題**</span><span class="sxs-lookup"><span data-stu-id="379ea-114">**Topics**</span></span>   |<span data-ttu-id="379ea-115">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="379ea-115">**Details**</span></span>   |<span data-ttu-id="379ea-116">**連結**</span><span class="sxs-lookup"><span data-stu-id="379ea-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="379ea-117">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="379ea-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="379ea-118">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="379ea-118">You need a valid MPN ID</span></span>|<span data-ttu-id="379ea-119">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="379ea-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="379ea-120">共同銷售準備就緒</span><span class="sxs-lookup"><span data-stu-id="379ea-120">Co-sell ready</span></span>|<span data-ttu-id="379ea-121">您的 IP/服務解決方案必須已準備好共同銷售。</span><span class="sxs-lookup"><span data-stu-id="379ea-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="379ea-122">與 Microsoft 銷售</span><span class="sxs-lookup"><span data-stu-id="379ea-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="379ea-123">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="379ea-123">Partner Center account</span></span>|<span data-ttu-id="379ea-124">與合作夥伴中心租使用者相關聯的 MPN 識別碼必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="379ea-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="379ea-125">先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。</span><span class="sxs-lookup"><span data-stu-id="379ea-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="379ea-126">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="379ea-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="379ea-127">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="379ea-127">Partner Center user roles</span></span>|<span data-ttu-id="379ea-128">將安裝並使用連接器的員工必須是推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="379ea-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="379ea-129">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="379ea-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="379ea-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="379ea-130">Salesforce CRM</span></span>|<span data-ttu-id="379ea-131">CRM 使用者角色是系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="379ea-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="379ea-132">在 Salesforce CRM 中指派角色</span><span class="sxs-lookup"><span data-stu-id="379ea-132">Assign roles in Salesforce CRM</span></span>](/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="379ea-133">Power Automate Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="379ea-133">Power Automate Flow Account</span></span>|<span data-ttu-id="379ea-134">適用于 CRM 系統管理員或系統自訂員的 active [Power Automate](https://flow.microsoft.com) 帳戶。</span><span class="sxs-lookup"><span data-stu-id="379ea-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="379ea-135">在安裝之前，該使用者至少應登入 [Power Automate](https://flow.microsoft.com) 一次。</span><span class="sxs-lookup"><span data-stu-id="379ea-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="379ea-136">安裝 Salesforce CRM 合作夥伴中心推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="379ea-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="379ea-137">移至 [Power Automate](https://flow.microsoft.com) ，然後在右上角選取 [ **環境** ]。</span><span class="sxs-lookup"><span data-stu-id="379ea-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="379ea-138">這會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="379ea-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="379ea-139">從右上角的下拉式清單中選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="379ea-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="379ea-140">選取左側導覽列上的 [ **方案** ]。</span><span class="sxs-lookup"><span data-stu-id="379ea-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="379ea-141">按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="379ea-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="379ea-143">在快顯視窗中搜尋 **Salesforce 的合作夥伴中心推薦連接器** 。</span><span class="sxs-lookup"><span data-stu-id="379ea-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="379ea-145">按一下 [ **立即取得** ] 按鈕，然後 **繼續**進行。</span><span class="sxs-lookup"><span data-stu-id="379ea-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="379ea-146">這會開啟頁面，您可以在其中選取要安裝應用程式的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="379ea-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="379ea-147">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="379ea-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRM":::

8. <span data-ttu-id="379ea-149">然後，系統會將您導向至 [ **管理您的解決方案** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="379ea-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="379ea-150">使用頁面底部的箭號按鈕，流覽至「合作夥伴中心的推薦」。</span><span class="sxs-lookup"><span data-stu-id="379ea-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="379ea-151">已**排程的安裝**應該會出現在合作夥伴中心的推薦解決方案旁邊。</span><span class="sxs-lookup"><span data-stu-id="379ea-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="379ea-152">安裝將需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="379ea-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="379ea-153">安裝完成之後，請流覽回到 [Power Automate](https://flow.microsoft.com) ，然後從左側導覽區域選取 **解決方案** 。</span><span class="sxs-lookup"><span data-stu-id="379ea-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="379ea-154">請注意，[方案] 清單中有提供 **Salesforce 的合作夥伴中心推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="379ea-155">選取 **Salesforce 的合作夥伴中心推薦同步**處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="379ea-156">以下是可用的流程和實體 Power Automate：</span><span class="sxs-lookup"><span data-stu-id="379ea-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce 流程":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="379ea-158">最佳做法：上線之前先進行測試</span><span class="sxs-lookup"><span data-stu-id="379ea-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="379ea-159">在生產環境中安裝、設定和自訂 Power Automate 解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="379ea-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="379ea-160">在預備環境/CRM 實例上安裝 Microsoft Power Automate 的解決方案。</span><span class="sxs-lookup"><span data-stu-id="379ea-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="379ea-161">製作解決方案的複本，並在預備環境中執行設定和 Power Automate 流程自訂。</span><span class="sxs-lookup"><span data-stu-id="379ea-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="379ea-162">測試預備/CRM 實例上的方案。</span><span class="sxs-lookup"><span data-stu-id="379ea-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="379ea-163">成功時，請將受控解決方案匯入至生產環境實例。</span><span class="sxs-lookup"><span data-stu-id="379ea-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="379ea-164">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="379ea-164">Configure the solution</span></span>

1. <span data-ttu-id="379ea-165">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power Automate](https://flow.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="379ea-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="379ea-166">從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power Automate 解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="379ea-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="379ea-167">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="379ea-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="379ea-168">具有推薦系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="379ea-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="379ea-169">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="379ea-169">Partner Center Events</span></span>
   - <span data-ttu-id="379ea-170">CRM 管理員與解決方案中的 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="379ea-171">從左側導覽列選取 [ **連接** ]，然後從清單中選取 [合作夥伴中心的參考] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="379ea-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="379ea-172">按一下 [ **建立連接**] 來建立連接。</span><span class="sxs-lookup"><span data-stu-id="379ea-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="建立連線":::

   3. <span data-ttu-id="379ea-174">在右上角的搜尋列中搜尋 \*\*合作夥伴中心參考 (預覽) \*\* 。</span><span class="sxs-lookup"><span data-stu-id="379ea-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="379ea-175">使用「參考系統管理員」的認證角色建立合作夥伴中心使用者的連接。</span><span class="sxs-lookup"><span data-stu-id="379ea-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="379ea-176">接下來，使用推薦的系統管理員認證來為您的合作夥伴中心使用者建立合作夥伴中心事件連接。</span><span class="sxs-lookup"><span data-stu-id="379ea-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="379ea-177">為 CRM 系統管理員使用者建立 Common Data Service (目前環境) 的連接。</span><span class="sxs-lookup"><span data-stu-id="379ea-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="379ea-178">若要將 Power Automate 流程與連接產生關聯，請編輯每個 Power Automate 流程，以連接到 Common Data Service 和合作夥伴中心的參考。</span><span class="sxs-lookup"><span data-stu-id="379ea-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="379ea-179">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="379ea-179">Save the changes.</span></span>

5. <span data-ttu-id="379ea-180">**開啟** Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="379ea-181">使用 Webhook Api 來註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="379ea-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="379ea-182">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="379ea-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="379ea-183">這些變更事件會以 HTTP 文章的形式傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="379ea-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="379ea-184">若要註冊您的 url，請選取 \*\*合作夥伴中心 Webhook 註冊 (Insider preview) \*\* Power Automate flow。</span><span class="sxs-lookup"><span data-stu-id="379ea-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="379ea-185">新增 (的連接。 ) 合作夥伴中心具有推薦的系統管理員認證的使用者 (b. ) 合作夥伴中心事件，如下所強調</span><span class="sxs-lookup"><span data-stu-id="379ea-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. <span data-ttu-id="379ea-187">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="379ea-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="379ea-189">儲存您的變更，然後選取 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="379ea-190">若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="379ea-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="379ea-191">選取 \*\*合作夥伴中心至 SALESFORCE CRM (Insider preview) \*\*。</span><span class="sxs-lookup"><span data-stu-id="379ea-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="379ea-192">選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="379ea-193">選取 **複製** 圖示來複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="379ea-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="複製 URL":::

8. <span data-ttu-id="379ea-195">現在，選取 [合作夥伴中心 Webhook 註冊 (Insider Preview) ] Power Automate 流程，然後選取 [ **執行**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="379ea-196">確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="379ea-197">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="379ea-197">Enter the following details:</span></span>

    1. <span data-ttu-id="379ea-198">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="379ea-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="379ea-199">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="379ea-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="379ea-200">**覆寫現有的觸發程式端點（如果有的話**）：是 (這會覆寫任何現有的端點。 ) </span><span class="sxs-lookup"><span data-stu-id="379ea-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="379ea-201">選取 [ **執行** ]，然後選取 [ **完成]。**</span><span class="sxs-lookup"><span data-stu-id="379ea-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="379ea-202">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="379ea-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="379ea-203">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="379ea-203">Customize synchronization steps</span></span>

<span data-ttu-id="379ea-204">當共同銷售的參考在合作夥伴中心與您的 CRM 系統之間進行同步處理時，在合作夥伴中心電腦上同步的欄位會列在此處。</span><span class="sxs-lookup"><span data-stu-id="379ea-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="379ea-205">通常會高度自訂 CRM 系統。</span><span class="sxs-lookup"><span data-stu-id="379ea-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="379ea-206">您可以自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="379ea-207">依照欄位對應指南操作，如有必要，請在 Power Automate 流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="379ea-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="379ea-208">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="379ea-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="379ea-209">您可以根據自己的需求自訂每個 Power Automate 流程的多個步驟。</span><span class="sxs-lookup"><span data-stu-id="379ea-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="379ea-210">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="379ea-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="379ea-211">若要自訂合作夥伴中心中的建立或更新事件的欄位以進行 CRM 推薦同步處理：</span><span class="sxs-lookup"><span data-stu-id="379ea-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="379ea-212">選取合作夥伴中心至 Salesforce CRM (Insider preview) 。</span><span class="sxs-lookup"><span data-stu-id="379ea-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="379ea-213">選取 [ **編輯** ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="379ea-214">選取 \*\* (範圍) 同步處理潛在客戶或商機\*\*。</span><span class="sxs-lookup"><span data-stu-id="379ea-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="379ea-215">若要自訂建立事件的 CRM 欄位對應，請選取 **它是否為新的共用商機，然後**。</span><span class="sxs-lookup"><span data-stu-id="379ea-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="379ea-216">若為 [ **是]** ，請選取子步驟，然後 **在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="379ea-217">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="379ea-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="379ea-218">若要自訂更新事件的 CRM 欄位對應，請按一下「 (範圍) 同步處理潛在客戶或商機」步驟。</span><span class="sxs-lookup"><span data-stu-id="379ea-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="379ea-219">**如果這是商機的更新，請選取它**。</span><span class="sxs-lookup"><span data-stu-id="379ea-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="379ea-220">**如果 [是]** ，請選取 [子步驟]，然後展開 [**合作夥伴中心和 CRM 中商機物件之間的差異]，然後再**展開。</span><span class="sxs-lookup"><span data-stu-id="379ea-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="379ea-221">選取 **[是]** ，然後選取 [**更新現有的商機**]</span><span class="sxs-lookup"><span data-stu-id="379ea-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="379ea-222">若要自訂更新事件的 CRM 對電腦推薦同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="379ea-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="379ea-223">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="379ea-224">選取 \*\* (範圍) 同步處理商機\*\*。</span><span class="sxs-lookup"><span data-stu-id="379ea-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="379ea-225">若要根據欄位對應來自訂 CRM 欄位對應 () 針對 update 事件，請選取 **合作夥伴中心和 CRM 中的潛在客戶物件之間是否有差異**。</span><span class="sxs-lookup"><span data-stu-id="379ea-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="379ea-226">**若為 [是]** ，請選取子步驟，然後展開 [**使用商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="379ea-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="379ea-227">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="379ea-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="379ea-228">針對建立事件自訂 CRM 對電腦推薦同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="379ea-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="379ea-229">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="379ea-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="379ea-230">選取 \*\* (範圍) 同步處理參考。\*\*</span><span class="sxs-lookup"><span data-stu-id="379ea-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="379ea-231">若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 [ **建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="379ea-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="379ea-232">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="379ea-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="379ea-233">在 Salesforce CRM 商機配置中建立個別的區段</span><span class="sxs-lookup"><span data-stu-id="379ea-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="379ea-234">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，Power Automate 解決方案必須清楚地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="379ea-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="379ea-235">這可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="379ea-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="379ea-236">有一組自訂欄位可作為 Salesforce CRM **商機** 實體合作夥伴中心推薦同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="379ea-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="379ea-237">CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="379ea-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="379ea-238">Salesforce CRM 系統管理員使用者將需要建立個別的 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="379ea-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="379ea-239">下列自訂欄位應該是 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="379ea-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="379ea-240">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="379ea-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="379ea-241">**參考識別碼**： Microsoft 合作夥伴中心推薦的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="379ea-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="379ea-242">**參考連結**： Microsoft 合作夥伴中心中參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="379ea-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="379ea-243">**Microsoft 如何提供協助？**</span><span class="sxs-lookup"><span data-stu-id="379ea-243">**How can Microsoft help?**</span></span> <span data-ttu-id="379ea-244">參考 Microsoft 所需的協助</span><span class="sxs-lookup"><span data-stu-id="379ea-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="379ea-245">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="379ea-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="379ea-246">**Audit**：與 Microsoft 合作夥伴中心推薦同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="379ea-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="379ea-247">設定欄位和關聯性</span><span class="sxs-lookup"><span data-stu-id="379ea-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="379ea-248">登入您的 Salesforce 帳戶並移至 **商機**。</span><span class="sxs-lookup"><span data-stu-id="379ea-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="379ea-249">按一下 [ **設定** ] 和 [ **編輯物件** ] 選項，以新增必要的欄位。</span><span class="sxs-lookup"><span data-stu-id="379ea-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="379ea-250">從左側導覽中選取 **欄位 & 關聯** 性</span><span class="sxs-lookup"><span data-stu-id="379ea-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="欄位":::

4. <span data-ttu-id="379ea-252">在 [ **欄位] & 關聯** 性資料表中新增下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="379ea-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="379ea-253">**欄位標籤**</span><span class="sxs-lookup"><span data-stu-id="379ea-253">**Field label**</span></span>   |<span data-ttu-id="379ea-254">**欄位名稱**</span><span class="sxs-lookup"><span data-stu-id="379ea-254">**Field name**</span></span>|<span data-ttu-id="379ea-255">**Data type**</span><span class="sxs-lookup"><span data-stu-id="379ea-255">**Data type**</span></span>|<span data-ttu-id="379ea-256">**索引**</span><span class="sxs-lookup"><span data-stu-id="379ea-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="379ea-257">稽核</span><span class="sxs-lookup"><span data-stu-id="379ea-257">Audit</span></span>| <span data-ttu-id="379ea-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="379ea-258">Audit__c</span></span>|<span data-ttu-id="379ea-259">長文字區域 (100000) # B2 可見的第4行) </span><span class="sxs-lookup"><span data-stu-id="379ea-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="379ea-260">Microsoft 如何提供協助？</span><span class="sxs-lookup"><span data-stu-id="379ea-260">How can Microsoft help?</span></span>|<span data-ttu-id="379ea-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="379ea-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="379ea-262">挑選清單</span><span class="sxs-lookup"><span data-stu-id="379ea-262">Picklist\*</span></span>|
   |<span data-ttu-id="379ea-263">產品</span><span class="sxs-lookup"><span data-stu-id="379ea-263">Products</span></span>|<span data-ttu-id="379ea-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="379ea-264">Products_c</span></span>|<span data-ttu-id="379ea-265">文字 (255) </span><span class="sxs-lookup"><span data-stu-id="379ea-265">text (255)</span></span>||
   |<span data-ttu-id="379ea-266">轉介</span><span class="sxs-lookup"><span data-stu-id="379ea-266">Referral</span></span> | <span data-ttu-id="379ea-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="379ea-267">Referral_Identfier_c</span></span>|<span data-ttu-id="379ea-268">文字 (100) # B2 外部識別碼) </span><span class="sxs-lookup"><span data-stu-id="379ea-268">Text(100)(External ID)</span></span>|<span data-ttu-id="379ea-269">是</span><span class="sxs-lookup"><span data-stu-id="379ea-269">yes</span></span>|
   |<span data-ttu-id="379ea-270">參考連結</span><span class="sxs-lookup"><span data-stu-id="379ea-270">Referral Link</span></span>| <span data-ttu-id="379ea-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="379ea-271">Referral_Link_c_</span></span>|<span data-ttu-id="379ea-272">URL (255) </span><span class="sxs-lookup"><span data-stu-id="379ea-272">URL(255)</span></span>||
   |<span data-ttu-id="379ea-273">與合作夥伴中心同步</span><span class="sxs-lookup"><span data-stu-id="379ea-273">Sync with Partner Center</span></span>|<span data-ttu-id="379ea-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="379ea-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="379ea-275">核取方塊 (預設未核取的) </span><span class="sxs-lookup"><span data-stu-id="379ea-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="379ea-276">\* 挑選清單值：</span><span class="sxs-lookup"><span data-stu-id="379ea-276">\*Picklist values:</span></span>

   - <span data-ttu-id="379ea-277">工作負載特定價值主張</span><span class="sxs-lookup"><span data-stu-id="379ea-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="379ea-278">客戶技術架構</span><span class="sxs-lookup"><span data-stu-id="379ea-278">Customer technical architecture</span></span>
   - <span data-ttu-id="379ea-279">概念證明或示範</span><span class="sxs-lookup"><span data-stu-id="379ea-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="379ea-280">報價或授權</span><span class="sxs-lookup"><span data-stu-id="379ea-280">Quotes or licensing</span></span>
   - <span data-ttu-id="379ea-281">銷售後客戶成功</span><span class="sxs-lookup"><span data-stu-id="379ea-281">Post sales customer success</span></span>
   - <span data-ttu-id="379ea-282">一般或其他</span><span class="sxs-lookup"><span data-stu-id="379ea-282">General or other</span></span>

5. <span data-ttu-id="379ea-283">這些欄位會在 [**欄位] & 關聯**性下建立</span><span class="sxs-lookup"><span data-stu-id="379ea-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="已建立欄位":::

6. <span data-ttu-id="379ea-285">在 [商機配置] 中，建立包含上述欄位的個別區段。</span><span class="sxs-lookup"><span data-stu-id="379ea-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="379ea-286">本章節應可供商機配置中的銷售人員使用</span><span class="sxs-lookup"><span data-stu-id="379ea-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="合作夥伴中心欄位版面配置":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="379ea-288">端對端雙向共同銷售推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="379ea-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="379ea-289">安裝、設定和自訂 Power Automate 解決方案之後，您可以測試 Salesforce CRM 和合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="379ea-290">必要條件</span><span class="sxs-lookup"><span data-stu-id="379ea-290">Pre-requisites</span></span>

<span data-ttu-id="379ea-291">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，Power Automate 解決方案必須清楚地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="379ea-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="379ea-292">此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="379ea-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="379ea-293">有一組自訂欄位可作為 Salesforce CRM 解決方案 **商機** 實體合作夥伴中心推薦同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="379ea-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="379ea-294">CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="379ea-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="379ea-295">下列自訂欄位應該是 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="379ea-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="379ea-296">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="379ea-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="379ea-297">**參考識別碼**： Microsoft 合作夥伴中心推薦的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="379ea-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="379ea-298">**參考連結**： Microsoft 合作夥伴中心中參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="379ea-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="379ea-299">**Microsoft 如何協助**：推薦的 microsoft 所需的協助</span><span class="sxs-lookup"><span data-stu-id="379ea-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="379ea-300">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="379ea-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="379ea-301">**Audit**：使用合作夥伴中心參考進行同步處理的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="379ea-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="379ea-302">場景：</span><span class="sxs-lookup"><span data-stu-id="379ea-302">SCENARIOS:</span></span>

1. <span data-ttu-id="379ea-303">參考在 CRM 中建立或更新時的參考同步處理，並在合作夥伴中心中同步處理：</span><span class="sxs-lookup"><span data-stu-id="379ea-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="379ea-304">登入您的 Salesforce CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。</span><span class="sxs-lookup"><span data-stu-id="379ea-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="379ea-305">當您在 Salesforce CRM 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="379ea-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. <span data-ttu-id="379ea-307">若要與 Microsoft 合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="379ea-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="379ea-308">「同步處理合作夥伴中心」：是</span><span class="sxs-lookup"><span data-stu-id="379ea-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="379ea-309">「Microsoft 如何協助？」：從下列選項中選取：</span><span class="sxs-lookup"><span data-stu-id="379ea-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="379ea-310">產品：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="379ea-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="379ea-311">一旦您將 [商機  **同步與合作夥伴中心** ] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="379ea-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="379ea-312">您的參考會與 Salesforce CRM 同步處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="379ea-313">當 [同步處理合作夥伴中心] 選項設定為 [是] 時，如果您更新 Salesforce CRM 中的機會，變更將會與您的合作夥伴中心帳戶進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="379ea-314">與合作夥伴中心成功同步處理的機會，將會使用 Salesforce CRM 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="379ea-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="379ea-315">在 Microsoft 合作夥伴中心中建立或更新參考時的參考同步處理，並在 Salesforce CRM 環境中同步處理：</span><span class="sxs-lookup"><span data-stu-id="379ea-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="379ea-316">登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="379ea-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="379ea-317">從左側功能表中選取 [ **參考** ]。</span><span class="sxs-lookup"><span data-stu-id="379ea-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="379ea-318">按一下 [新增交易] 選項，從合作夥伴中心建立新的共同銷售推薦。</span><span class="sxs-lookup"><span data-stu-id="379ea-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="379ea-319">登入您的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="379ea-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="379ea-320">流覽至 **開啟的商機**。</span><span class="sxs-lookup"><span data-stu-id="379ea-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="379ea-321">在 Microsoft 合作夥伴中心中建立的參照現在已在 Salesforce CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="379ea-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 商機畫面":::

    6. <span data-ttu-id="379ea-323">當您選取同步處理的參考時，就會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="379ea-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="379ea-324">下一步</span><span class="sxs-lookup"><span data-stu-id="379ea-324">Next steps</span></span>

- [<span data-ttu-id="379ea-325">深入瞭解 Microsoft Power Automate platform？</span><span class="sxs-lookup"><span data-stu-id="379ea-325">More about Microsoft Power Automate platform?</span></span>](/-automate/)

- [<span data-ttu-id="379ea-326">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="379ea-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="379ea-327">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="379ea-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="379ea-328">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="379ea-328">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)