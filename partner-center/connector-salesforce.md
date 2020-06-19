---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在合作夥伴中心與您的 Salesforce CRM 同步處理您的參考
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e51ddc8ec3ea568a20404801802548f79cae43d0
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991617"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="98897-103">Salesforce CRM 的共同銷售連接器 – 概觀</span><span class="sxs-lookup"><span data-stu-id="98897-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="98897-104">適當的角色</span><span class="sxs-lookup"><span data-stu-id="98897-104">Appropriate roles</span></span>

- <span data-ttu-id="98897-105">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="98897-105">Referrals admin</span></span>
- <span data-ttu-id="98897-106">CRM 上的系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="98897-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="98897-107">合作夥伴中心共同銷售連接器可讓您的銷售人員從您的 CRM 系統內與 Microsoft 共同合作。</span><span class="sxs-lookup"><span data-stu-id="98897-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="98897-108">他們不需要經過訓練，就能使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="98897-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="98897-109">使用共同銷售連接器，您可以建立新的共同銷售參照來與 Microsoft 賣方互動、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料，例如交易價值和結束日期。</span><span class="sxs-lookup"><span data-stu-id="98897-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="98897-110">您也可以在這些共同銷售交易上，收到 Microsoft 賣方的任何更新。</span><span class="sxs-lookup"><span data-stu-id="98897-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="98897-111">在您選擇的 CRM 中工作時（而不是在合作夥伴中心），您可以執行所有的參考工作。</span><span class="sxs-lookup"><span data-stu-id="98897-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="98897-112">解決方案是以 Microsoft 電源自動化解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="98897-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="98897-113">安裝之前的必要條件</span><span class="sxs-lookup"><span data-stu-id="98897-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="98897-114">**主題**</span><span class="sxs-lookup"><span data-stu-id="98897-114">**Topics**</span></span>   |<span data-ttu-id="98897-115">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="98897-115">**Details**</span></span>   |<span data-ttu-id="98897-116">**連結**</span><span class="sxs-lookup"><span data-stu-id="98897-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="98897-117">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="98897-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="98897-118">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="98897-118">You need a valid MPN ID</span></span>|<span data-ttu-id="98897-119">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="98897-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="98897-120">共同銷售準備就緒</span><span class="sxs-lookup"><span data-stu-id="98897-120">Co-sell ready</span></span>|<span data-ttu-id="98897-121">您的 IP/服務解決方案必須共同銷售。</span><span class="sxs-lookup"><span data-stu-id="98897-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="98897-122">與 Microsoft 一起銷售</span><span class="sxs-lookup"><span data-stu-id="98897-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="98897-123">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="98897-123">Partner Center account</span></span>|<span data-ttu-id="98897-124">與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您的共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="98897-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="98897-125">在部署連接器之前，請確認您可以在合作夥伴中心入口網站中看到您的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="98897-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="98897-126">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="98897-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="98897-127">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="98897-127">Partner Center user roles</span></span>|<span data-ttu-id="98897-128">將安裝和使用連接器的員工必須是推薦管理員</span><span class="sxs-lookup"><span data-stu-id="98897-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="98897-129">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="98897-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="98897-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="98897-130">Salesforce CRM</span></span>|<span data-ttu-id="98897-131">CRM 使用者角色是系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="98897-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="98897-132">在 Salesforce CRM 中指派角色</span><span class="sxs-lookup"><span data-stu-id="98897-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="98897-133">Power 自動化 Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="98897-133">Power Automate Flow Account</span></span>|<span data-ttu-id="98897-134">適用于 CRM 系統管理員或系統自訂者的主動式[電源自動化](https://flow.microsoft.com)帳戶。</span><span class="sxs-lookup"><span data-stu-id="98897-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="98897-135">該使用者應該在安裝之前至少登入一次[電源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="98897-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="98897-136">安裝 Salesforce CRM 的合作夥伴中心推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="98897-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="98897-137">移至 [[電源自動化](https://flow.microsoft.com)]，並選取右上角的 [**環境**]。</span><span class="sxs-lookup"><span data-stu-id="98897-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="98897-138">這會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="98897-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="98897-139">從右上角的下拉式選單中，選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="98897-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="98897-140">選取左側導覽列上的 [**方案**]。</span><span class="sxs-lookup"><span data-stu-id="98897-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="98897-141">按一下上方功能表上的 [**開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="98897-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="98897-143">在彈出畫面中搜尋**Salesforce 的合作夥伴中心參照連接器**。</span><span class="sxs-lookup"><span data-stu-id="98897-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="98897-145">按一下 [**立即取得**] 按鈕，然後按 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="98897-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="98897-146">這會開啟頁面，您可以在其中選取要安裝應用程式的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="98897-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="98897-147">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="98897-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRM":::

8. <span data-ttu-id="98897-149">接著，您會被導向至 [**管理您的解決方案**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="98897-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="98897-150">使用頁面底部的箭號按鈕，流覽至 [合作夥伴中心的參考]。</span><span class="sxs-lookup"><span data-stu-id="98897-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="98897-151">已**排程的安裝**應該會出現在合作夥伴中心的 [參考解決方案] 旁。</span><span class="sxs-lookup"><span data-stu-id="98897-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="98897-152">安裝需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="98897-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="98897-153">安裝完成後，流覽回到 [[電源自動化](https://flow.microsoft.com)]，然後從左側導覽區域選取 [**解決方案**]。</span><span class="sxs-lookup"><span data-stu-id="98897-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="98897-154">請注意，解決方案清單中提供**Salesforce 的合作夥伴中心參照同步**處理。</span><span class="sxs-lookup"><span data-stu-id="98897-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="98897-155">選取**Salesforce 的 [合作夥伴中心參考同步**處理]。</span><span class="sxs-lookup"><span data-stu-id="98897-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="98897-156">下列電源可自動執行流程和實體：</span><span class="sxs-lookup"><span data-stu-id="98897-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce 流程":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="98897-158">最佳做法：在您上線之前進行測試</span><span class="sxs-lookup"><span data-stu-id="98897-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="98897-159">在您安裝、設定及自訂生產環境的電源自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="98897-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="98897-160">在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="98897-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="98897-161">建立解決方案的複本，並執行您的設定，並在預備環境中自動執行流程自訂。</span><span class="sxs-lookup"><span data-stu-id="98897-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="98897-162">在預備/CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="98897-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="98897-163">成功時，將匯入為生產實例的受控解決方案。</span><span class="sxs-lookup"><span data-stu-id="98897-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="98897-164">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="98897-164">Configure the solution</span></span>

1. <span data-ttu-id="98897-165">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [[電源自動化](https://flow.microsoft.com/)]。</span><span class="sxs-lookup"><span data-stu-id="98897-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="98897-166">從右上角的 [**環境**] 下拉式選，選取您已安裝電源自動化解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="98897-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="98897-167">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="98897-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="98897-168">具有參考系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="98897-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="98897-169">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="98897-169">Partner Center Events</span></span>
   - <span data-ttu-id="98897-170">CRM 系統管理員，具備在解決方案中自動化流程的能力。</span><span class="sxs-lookup"><span data-stu-id="98897-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="98897-171">從左側導覽列選取 [連線]，**然後從清單**中選取 [合作夥伴中心參照] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="98897-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="98897-172">按一下 [**建立連接**] 來建立連線。</span><span class="sxs-lookup"><span data-stu-id="98897-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="建立連線":::

   3. <span data-ttu-id="98897-174">在右上角的搜尋列中搜尋**合作夥伴中心參照（預覽）** 。</span><span class="sxs-lookup"><span data-stu-id="98897-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="98897-175">使用 [參考管理員] 的認證角色建立合作夥伴中心使用者的連線。</span><span class="sxs-lookup"><span data-stu-id="98897-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="98897-176">接下來，使用 [參考管理員] 的認證為合作夥伴中心使用者建立合作夥伴中心的事件連線。</span><span class="sxs-lookup"><span data-stu-id="98897-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="98897-177">為 CRM 系統管理員使用者建立 Common Data Service （目前的環境）的連接。</span><span class="sxs-lookup"><span data-stu-id="98897-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="98897-178">若要讓電源自動化流程與連線產生關聯，請編輯每個電源自動化流程，以連線至 Common Data Service 和合作夥伴中心的參照。</span><span class="sxs-lookup"><span data-stu-id="98897-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="98897-179">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="98897-179">Save the changes.</span></span>

5. <span data-ttu-id="98897-180">**開啟**電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="98897-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="98897-181">使用 Webhook Api 註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="98897-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="98897-182">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="98897-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="98897-183">這些變更事件會當做 HTTP post 傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="98897-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="98897-184">若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。</span><span class="sxs-lookup"><span data-stu-id="98897-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="98897-185">新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="98897-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. <span data-ttu-id="98897-187">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="98897-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="98897-189">儲存您的變更，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="98897-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="98897-190">若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="98897-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="98897-191">選取 **[合作夥伴中心至 SALESFORCE CRM （Insider preview）**]。</span><span class="sxs-lookup"><span data-stu-id="98897-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="98897-192">選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="98897-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="98897-193">選取**複製**圖示以複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="98897-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="複製 URL":::

8. <span data-ttu-id="98897-195">現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。</span><span class="sxs-lookup"><span data-stu-id="98897-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="98897-196">確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="98897-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="98897-197">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="98897-197">Enter the following details:</span></span>

    1. <span data-ttu-id="98897-198">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="98897-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="98897-199">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="98897-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="98897-200">**覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。</span><span class="sxs-lookup"><span data-stu-id="98897-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="98897-201">選取 [**執行**]，然後選取 [**完成]。**</span><span class="sxs-lookup"><span data-stu-id="98897-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="98897-202">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="98897-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="98897-203">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="98897-203">Customize synchronization steps</span></span>

<span data-ttu-id="98897-204">在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。</span><span class="sxs-lookup"><span data-stu-id="98897-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="98897-205">通常 CRM 系統是高度自訂的。</span><span class="sxs-lookup"><span data-stu-id="98897-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="98897-206">您可以自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="98897-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="98897-207">遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="98897-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="98897-208">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="98897-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="98897-209">每個電源自動化流程的多個步驟可以根據您的需求自訂。</span><span class="sxs-lookup"><span data-stu-id="98897-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="98897-210">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="98897-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="98897-211">若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="98897-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="98897-212">選取 [合作夥伴中心至 Salesforce CRM （Insider Preview）]。</span><span class="sxs-lookup"><span data-stu-id="98897-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="98897-213">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="98897-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="98897-214">選取 **[（範圍）]，同步處理潛在客戶或商機**。</span><span class="sxs-lookup"><span data-stu-id="98897-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="98897-215">若要自訂建立事件的 CRM 欄位對應，請選取 [**如果是新的共用機會]，然後**。</span><span class="sxs-lookup"><span data-stu-id="98897-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="98897-216">**如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="98897-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="98897-217">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="98897-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="98897-218">若要自訂更新事件的 CRM 欄位對應，請按一下步驟「（範圍）同步處理潛在客戶或商機」。</span><span class="sxs-lookup"><span data-stu-id="98897-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="98897-219">**如果它是商機的更新，請選取此**方式。</span><span class="sxs-lookup"><span data-stu-id="98897-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="98897-220">**若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。</span><span class="sxs-lookup"><span data-stu-id="98897-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="98897-221">選取 **[如果是]** ，然後按一下 [**更新現有商機**]</span><span class="sxs-lookup"><span data-stu-id="98897-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="98897-222">若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="98897-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="98897-223">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="98897-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="98897-224">選取 **[（範圍）] 以同步處理商機**。</span><span class="sxs-lookup"><span data-stu-id="98897-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="98897-225">針對 [更新事件] 的自訂 CRM 欄位對應（根據欄位對應指南），選取 **[合作夥伴中心和 CRM 中的潛在客戶] 物件之間是否有差異，然後**。</span><span class="sxs-lookup"><span data-stu-id="98897-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="98897-226">選取子步驟（**如果是**），然後展開 [**以商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="98897-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="98897-227">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="98897-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="98897-228">若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="98897-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="98897-229">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="98897-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="98897-230">選取 **[同步處理參考] （範圍）。**</span><span class="sxs-lookup"><span data-stu-id="98897-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="98897-231">如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="98897-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="98897-232">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="98897-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="98897-233">在 Salesforce CRM 商機版面配置中建立個別的區段</span><span class="sxs-lookup"><span data-stu-id="98897-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="98897-234">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，電源自動化解決方案必須清楚地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="98897-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="98897-235">這讓您的賣方小組能夠決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="98897-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="98897-236">一組自訂欄位可作為 Salesforce CRM**商機**實體的合作夥伴中心參考同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="98897-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="98897-237">CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。</span><span class="sxs-lookup"><span data-stu-id="98897-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="98897-238">Salesforce CRM 系統管理員使用者將需要建立個別的 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="98897-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="98897-239">下列自訂欄位應為 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="98897-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="98897-240">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="98897-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="98897-241">**參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="98897-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="98897-242">**參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="98897-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="98897-243">**Microsoft 如何提供協助？**</span><span class="sxs-lookup"><span data-stu-id="98897-243">**How can Microsoft help?**</span></span> <span data-ttu-id="98897-244">Microsoft 針對此參考所需的協助</span><span class="sxs-lookup"><span data-stu-id="98897-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="98897-245">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="98897-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="98897-246">**Audit**：與 Microsoft 合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="98897-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="98897-247">設定欄位和關聯性</span><span class="sxs-lookup"><span data-stu-id="98897-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="98897-248">登入您的 Salesforce 帳戶，並移至 [**商機**]。</span><span class="sxs-lookup"><span data-stu-id="98897-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="98897-249">按一下 [**設定**] 和 [**編輯物件**] 選項，以加入必要的欄位。</span><span class="sxs-lookup"><span data-stu-id="98897-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="98897-250">從左側導覽中選取**欄位 & 關聯**性</span><span class="sxs-lookup"><span data-stu-id="98897-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="欄位":::

4. <span data-ttu-id="98897-252">在 [**欄位 & 關聯**性] 資料表中新增下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="98897-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="98897-253">**欄位標籤**</span><span class="sxs-lookup"><span data-stu-id="98897-253">**Field label**</span></span>   |<span data-ttu-id="98897-254">**欄位名稱**</span><span class="sxs-lookup"><span data-stu-id="98897-254">**Field name**</span></span>|<span data-ttu-id="98897-255">**Data type**</span><span class="sxs-lookup"><span data-stu-id="98897-255">**Data type**</span></span>|<span data-ttu-id="98897-256">**編制**</span><span class="sxs-lookup"><span data-stu-id="98897-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="98897-257">稽核</span><span class="sxs-lookup"><span data-stu-id="98897-257">Audit</span></span>| <span data-ttu-id="98897-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="98897-258">Audit__c</span></span>|<span data-ttu-id="98897-259">長文字區域（100000）（顯示行4）</span><span class="sxs-lookup"><span data-stu-id="98897-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="98897-260">Microsoft 如何提供協助？</span><span class="sxs-lookup"><span data-stu-id="98897-260">How can Microsoft help?</span></span>|<span data-ttu-id="98897-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="98897-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="98897-262">清單</span><span class="sxs-lookup"><span data-stu-id="98897-262">Picklist\*</span></span>|
   |<span data-ttu-id="98897-263">Products</span><span class="sxs-lookup"><span data-stu-id="98897-263">Products</span></span>|<span data-ttu-id="98897-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="98897-264">Products_c</span></span>|<span data-ttu-id="98897-265">文字（255）</span><span class="sxs-lookup"><span data-stu-id="98897-265">text (255)</span></span>||
   |<span data-ttu-id="98897-266">轉介</span><span class="sxs-lookup"><span data-stu-id="98897-266">Referral</span></span> | <span data-ttu-id="98897-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="98897-267">Referral_Identfier_c</span></span>|<span data-ttu-id="98897-268">文字（100）（外部識別碼）</span><span class="sxs-lookup"><span data-stu-id="98897-268">Text(100)(External ID)</span></span>|<span data-ttu-id="98897-269">是</span><span class="sxs-lookup"><span data-stu-id="98897-269">yes</span></span>|
   |<span data-ttu-id="98897-270">參考連結</span><span class="sxs-lookup"><span data-stu-id="98897-270">Referral Link</span></span>| <span data-ttu-id="98897-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="98897-271">Referral_Link_c_</span></span>|<span data-ttu-id="98897-272">URL （255）</span><span class="sxs-lookup"><span data-stu-id="98897-272">URL(255)</span></span>||
   |<span data-ttu-id="98897-273">與合作夥伴中心同步</span><span class="sxs-lookup"><span data-stu-id="98897-273">Sync with Partner Center</span></span>|<span data-ttu-id="98897-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="98897-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="98897-275">核取方塊（預設為未核取）</span><span class="sxs-lookup"><span data-stu-id="98897-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="98897-276">\* 挑選清單值：</span><span class="sxs-lookup"><span data-stu-id="98897-276">\*Picklist values:</span></span>

   - <span data-ttu-id="98897-277">工作負載特定價值主張</span><span class="sxs-lookup"><span data-stu-id="98897-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="98897-278">客戶技術架構</span><span class="sxs-lookup"><span data-stu-id="98897-278">Customer technical architecture</span></span>
   - <span data-ttu-id="98897-279">概念證明或示範</span><span class="sxs-lookup"><span data-stu-id="98897-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="98897-280">報價或授權</span><span class="sxs-lookup"><span data-stu-id="98897-280">Quotes or licensing</span></span>
   - <span data-ttu-id="98897-281">將銷售客戶成功後置</span><span class="sxs-lookup"><span data-stu-id="98897-281">Post sales customer success</span></span>
   - <span data-ttu-id="98897-282">一般或其他</span><span class="sxs-lookup"><span data-stu-id="98897-282">General or other</span></span>

5. <span data-ttu-id="98897-283">欄位會在 [欄位] **& [關聯**性] 底下建立</span><span class="sxs-lookup"><span data-stu-id="98897-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="建立的欄位":::

6. <span data-ttu-id="98897-285">在 [商機配置] 中，以上欄欄位建立個別的區段。</span><span class="sxs-lookup"><span data-stu-id="98897-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="98897-286">此章節應適用于商機配置中的銷售人員</span><span class="sxs-lookup"><span data-stu-id="98897-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="合作夥伴中心欄位版面配置":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="98897-288">端對端雙向共同銷售參考同步處理</span><span class="sxs-lookup"><span data-stu-id="98897-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="98897-289">當您安裝、設定並自訂電源自動化解決方案之後，您可以測試 Salesforce CRM 和合作夥伴中心之間的共同銷售參考同步處理。</span><span class="sxs-lookup"><span data-stu-id="98897-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="98897-290">必要條件</span><span class="sxs-lookup"><span data-stu-id="98897-290">Pre-requisites</span></span>

<span data-ttu-id="98897-291">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，電源自動化解決方案必須清楚地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="98897-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="98897-292">此識別可讓您的賣方小組決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="98897-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="98897-293">一組自訂欄位可作為 Salesforce CRM 解決方案**商機**實體的合作夥伴中心參考同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="98897-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="98897-294">CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。</span><span class="sxs-lookup"><span data-stu-id="98897-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="98897-295">下列自訂欄位應為 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="98897-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="98897-296">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="98897-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="98897-297">**參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="98897-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="98897-298">**參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="98897-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="98897-299">**Microsoft 說明如何**： microsoft 針對此參考所需的協助</span><span class="sxs-lookup"><span data-stu-id="98897-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="98897-300">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="98897-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="98897-301">**Audit**：與合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="98897-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="98897-302">場景</span><span class="sxs-lookup"><span data-stu-id="98897-302">SCENARIOS:</span></span>

1. <span data-ttu-id="98897-303">在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="98897-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="98897-304">以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="98897-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="98897-305">當您在 Salesforce CRM 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="98897-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. <span data-ttu-id="98897-307">若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="98897-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="98897-308">「與合作夥伴中心同步」：是</span><span class="sxs-lookup"><span data-stu-id="98897-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="98897-309">「Microsoft 如何協助？」：從下列選項中選取：</span><span class="sxs-lookup"><span data-stu-id="98897-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="98897-310">產品：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="98897-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="98897-311">將 [商機**與合作夥伴中心同步**] 選項設定為 **[是]** 之後，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="98897-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="98897-312">您的參考將與 Salesforce CRM 同步處理。</span><span class="sxs-lookup"><span data-stu-id="98897-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="98897-313">當 [與合作夥伴中心同步] 選項設定為 [是] 時，如果您更新 Salesforce CRM 中的機會，這些變更將會與您的合作夥伴中心帳戶同步處理。</span><span class="sxs-lookup"><span data-stu-id="98897-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="98897-314">與合作夥伴中心成功同步處理的機會，將會使用 Salesforce CRM 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="98897-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="98897-315">在 Microsoft 合作夥伴中心內建立或更新參照時的參考同步處理，並在 Salesforce CRM 環境中同步處理：</span><span class="sxs-lookup"><span data-stu-id="98897-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="98897-316">登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="98897-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="98897-317">從左側功能表中選取 [**參考**]。</span><span class="sxs-lookup"><span data-stu-id="98897-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="98897-318">按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="98897-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="98897-319">登入您的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="98897-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="98897-320">流覽至 [**開啟商機**]。</span><span class="sxs-lookup"><span data-stu-id="98897-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="98897-321">在 Microsoft 合作夥伴中心建立的參考現在已在 Salesforce CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="98897-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 商機畫面":::

    6. <span data-ttu-id="98897-323">當您選取同步處理的參考時，會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="98897-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="98897-324">後續步驟</span><span class="sxs-lookup"><span data-stu-id="98897-324">Next steps</span></span>

- [<span data-ttu-id="98897-325">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="98897-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="98897-326">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="98897-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="98897-327">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="98897-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="98897-328">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="98897-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)