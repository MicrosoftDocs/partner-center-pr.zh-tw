---
title: Dynamics 365 CRM 合作夥伴中心的共同銷售連接器
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在合作夥伴中心與您的 Dynamics 365 CRM 同步處理您的參考
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 1b7124ef2db99e4b6e79ed71c2998973ee3ef126
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435447"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="cb419-103">Dynamics 365 CRM 的共同銷售連接器-總覽</span><span class="sxs-lookup"><span data-stu-id="cb419-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="cb419-104">適當的角色</span><span class="sxs-lookup"><span data-stu-id="cb419-104">Appropriate roles</span></span>

- <span data-ttu-id="cb419-105">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="cb419-105">Referrals admin</span></span>
- <span data-ttu-id="cb419-106">CRM 上的系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="cb419-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="cb419-107">合作夥伴中心共同銷售連接器可讓您的銷售人員從您的 CRM 系統內與 Microsoft 共同合作。</span><span class="sxs-lookup"><span data-stu-id="cb419-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="cb419-108">他們不需要經過訓練，就能使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="cb419-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="cb419-109">使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方互動、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。</span><span class="sxs-lookup"><span data-stu-id="cb419-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="cb419-110">您也可以在這些共同銷售交易上，收到 Microsoft 賣方的任何更新。</span><span class="sxs-lookup"><span data-stu-id="cb419-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="cb419-111">您可以在您選擇的 CRM 中，而不是在合作夥伴中心內，執行所有的參考工作。</span><span class="sxs-lookup"><span data-stu-id="cb419-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="cb419-112">解決方案是以 Microsoft 電源自動化解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="cb419-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="cb419-113">安裝之前的必要條件</span><span class="sxs-lookup"><span data-stu-id="cb419-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="cb419-114">**主題**</span><span class="sxs-lookup"><span data-stu-id="cb419-114">**Topics**</span></span>   |<span data-ttu-id="cb419-115">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="cb419-115">**Details**</span></span>   |<span data-ttu-id="cb419-116">**連結**</span><span class="sxs-lookup"><span data-stu-id="cb419-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="cb419-117">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="cb419-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="cb419-118">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="cb419-118">You need a valid MPN ID</span></span>|<span data-ttu-id="cb419-119">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="cb419-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="cb419-120">共同銷售就緒</span><span class="sxs-lookup"><span data-stu-id="cb419-120">Cosell ready</span></span>|<span data-ttu-id="cb419-121">您的 IP/服務解決方案必須共同銷售。</span><span class="sxs-lookup"><span data-stu-id="cb419-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="cb419-122">與 Microsoft 一起銷售</span><span class="sxs-lookup"><span data-stu-id="cb419-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="cb419-123">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="cb419-123">Partner Center account</span></span>|<span data-ttu-id="cb419-124">與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您的共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="cb419-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="cb419-125">在部署連接器之前，請確認您可以在合作夥伴中心入口網站中看到您的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="cb419-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="cb419-126">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="cb419-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="cb419-127">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="cb419-127">Partner Center user roles</span></span>|<span data-ttu-id="cb419-128">將安裝和使用連接器的員工必須是推薦管理員</span><span class="sxs-lookup"><span data-stu-id="cb419-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="cb419-129">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="cb419-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="cb419-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="cb419-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="cb419-131">CRM 使用者角色是系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="cb419-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="cb419-132">指派 Dynamics 365 中的角色</span><span class="sxs-lookup"><span data-stu-id="cb419-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="cb419-133">Power 自動化 Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="cb419-133">Power Automate Flow Account</span></span>|<span data-ttu-id="cb419-134">適用于 CRM 系統管理員或系統自訂者的主動式[電源自動化](https://flow.microsoft.com)帳戶。</span><span class="sxs-lookup"><span data-stu-id="cb419-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="cb419-135">該使用者應該在安裝之前至少登入一次[電源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="cb419-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="cb419-136">安裝 Dynamics 365 的合作夥伴中心推薦同步處理（電源自動化解決方案）</span><span class="sxs-lookup"><span data-stu-id="cb419-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="cb419-137">移至 [[電源自動化](https://flow.microsoft.com)]，並選取右上角的 [**環境**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="cb419-138">此步驟會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="cb419-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="cb419-139">從右上角的下拉式選單中，選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="cb419-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="cb419-140">選取左側導覽列上的 [**方案**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="cb419-141">按一下上方功能表上的 [**開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="cb419-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="cb419-143">在快顯畫面中搜尋**合作夥伴中心的 [推薦] 連接器以進行 Dynamics365** 。</span><span class="sxs-lookup"><span data-stu-id="cb419-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="cb419-144">按一下 [**立即取得**] 按鈕，然後按 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="cb419-145">這會開啟頁面，您可以在其中選取要安裝應用程式的 CRM （Dynamics 365）環境。</span><span class="sxs-lookup"><span data-stu-id="cb419-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="cb419-146">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="cb419-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="cb419-147">接著，您會被導向至 [**管理您的解決方案**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="cb419-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="cb419-148">使用頁面底部的箭號按鈕，流覽至 [合作夥伴中心的參考]。</span><span class="sxs-lookup"><span data-stu-id="cb419-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="cb419-149">已**排程的安裝**應該會出現在合作夥伴中心的 [參考解決方案] 旁。</span><span class="sxs-lookup"><span data-stu-id="cb419-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="cb419-150">安裝需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="cb419-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="cb419-151">安裝完成後，流覽回到 [[電源自動化](https://flow.microsoft.com)]，然後從左側導覽區域選取 [**解決方案**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="cb419-152">請注意，解決方案清單中有提供**Dynamics 365 的合作夥伴中心參照同步**處理。</span><span class="sxs-lookup"><span data-stu-id="cb419-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="cb419-153">選取**Dynamics 365 的合作夥伴中心參照同步**處理。</span><span class="sxs-lookup"><span data-stu-id="cb419-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="cb419-154">下列電源可自動執行流程和實體：</span><span class="sxs-lookup"><span data-stu-id="cb419-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用的 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="cb419-156">最佳做法：在您上線之前進行測試</span><span class="sxs-lookup"><span data-stu-id="cb419-156">Best practice: test before you go live</span></span>

<span data-ttu-id="cb419-157">在您安裝、設定及自訂生產環境的電源自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="cb419-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="cb419-158">在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="cb419-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="cb419-159">建立解決方案的複本，並執行您的設定，並在預備環境中自動執行流程自訂。</span><span class="sxs-lookup"><span data-stu-id="cb419-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="cb419-160">在預備/CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="cb419-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="cb419-161">成功時，將匯入為生產實例的受控解決方案。</span><span class="sxs-lookup"><span data-stu-id="cb419-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="cb419-162">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="cb419-162">Configure the solution</span></span>

1. <span data-ttu-id="cb419-163">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [[電源自動化](https://flow.microsoft.com/)]。</span><span class="sxs-lookup"><span data-stu-id="cb419-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="cb419-164">從右上角的 [**環境**] 下拉式選，選取您已安裝電源自動化解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="cb419-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="cb419-165">您必須建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="cb419-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="cb419-166">具有參考系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="cb419-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="cb419-167">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="cb419-167">Partner Center Events</span></span>

   - <span data-ttu-id="cb419-168">CRM 系統管理員，具備在解決方案中自動化流程的能力。</span><span class="sxs-lookup"><span data-stu-id="cb419-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="cb419-169">從左側導覽列選取 [連線]，**然後從清單**中選取 [合作夥伴中心參照] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="cb419-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="cb419-170">按一下 [**建立連接**] 來建立連線。</span><span class="sxs-lookup"><span data-stu-id="cb419-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="建立連線":::

      3. <span data-ttu-id="cb419-172">在右上角的搜尋列中搜尋**合作夥伴中心參照（預覽）** 。</span><span class="sxs-lookup"><span data-stu-id="cb419-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="cb419-173">使用 [參考管理員] 的認證角色建立合作夥伴中心使用者的連線。</span><span class="sxs-lookup"><span data-stu-id="cb419-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="cb419-174">接下來，使用 [參考管理員] 的認證為合作夥伴中心使用者建立合作夥伴中心的事件連線。</span><span class="sxs-lookup"><span data-stu-id="cb419-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="cb419-175">為 CRM 系統管理員使用者建立 Common Data Service （目前的環境）的連接。</span><span class="sxs-lookup"><span data-stu-id="cb419-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="cb419-176">若要讓電源自動化流程與連線產生關聯，請編輯每個電源自動化流程，以連線至 Common Data Service 和合作夥伴中心的參照。</span><span class="sxs-lookup"><span data-stu-id="cb419-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="cb419-177">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="cb419-177">Save the changes.</span></span>

5. <span data-ttu-id="cb419-178">**開啟**電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="cb419-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="cb419-179">使用 Webhook Api 註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="cb419-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="cb419-180">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="cb419-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="cb419-181">這些變更事件會當做 HTTP post 傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="cb419-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="cb419-182">若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。</span><span class="sxs-lookup"><span data-stu-id="cb419-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="cb419-183">新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="cb419-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. <span data-ttu-id="cb419-185">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="cb419-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="cb419-187">儲存您的變更，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="cb419-188">若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="cb419-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="cb419-189">選取 **[合作夥伴中心] 至 [Dynamics 365 （Insider preview）**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="cb419-190">選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="cb419-191">選取**複製**圖示以複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="cb419-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="複製 URL":::

8. <span data-ttu-id="cb419-193">現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="cb419-194">確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="cb419-195">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="cb419-195">Enter the following details:</span></span>

    1. <span data-ttu-id="cb419-196">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="cb419-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="cb419-197">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="cb419-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="cb419-198">**覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。</span><span class="sxs-lookup"><span data-stu-id="cb419-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="cb419-199">選取 [**執行**]，然後選取 [**完成]。**</span><span class="sxs-lookup"><span data-stu-id="cb419-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="cb419-200">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="cb419-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="cb419-201">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="cb419-201">Customize synchronization steps</span></span>

<span data-ttu-id="cb419-202">在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。</span><span class="sxs-lookup"><span data-stu-id="cb419-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="cb419-203">通常 CRM 系統是高度自訂的。</span><span class="sxs-lookup"><span data-stu-id="cb419-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="cb419-204">您可以自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="cb419-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="cb419-205">遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="cb419-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="cb419-206">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="cb419-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="cb419-207">每個電源自動化流程的多個步驟可以根據您的需求自訂。</span><span class="sxs-lookup"><span data-stu-id="cb419-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="cb419-208">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="cb419-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="cb419-209">若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="cb419-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="cb419-210">a.</span><span class="sxs-lookup"><span data-stu-id="cb419-210">a.</span></span> <span data-ttu-id="cb419-211">選取 [合作夥伴中心] 至 [Dynamics 365 （Insider Preview）] 或 [合作夥伴中心] 至 [Salesforce （Insider Preview）]。</span><span class="sxs-lookup"><span data-stu-id="cb419-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="cb419-212">b.</span><span class="sxs-lookup"><span data-stu-id="cb419-212">b.</span></span> <span data-ttu-id="cb419-213">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="cb419-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="cb419-214">c.</span><span class="sxs-lookup"><span data-stu-id="cb419-214">c.</span></span> <span data-ttu-id="cb419-215">選取 **[（範圍）]，同步處理潛在客戶或商機**。</span><span class="sxs-lookup"><span data-stu-id="cb419-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="cb419-216">若要自訂 [建立事件] 的 CRM 欄位對應（根據欄位對應指南），請選取 [**如果是新的共用機會]，然後**。</span><span class="sxs-lookup"><span data-stu-id="cb419-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="cb419-217">**如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="cb419-218">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="cb419-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="cb419-219">d.</span><span class="sxs-lookup"><span data-stu-id="cb419-219">d.</span></span> <span data-ttu-id="cb419-220">如需自訂 update 事件的 CRM 欄位對應（根據欄位對應指南），請按一下「同步處理潛在客戶或商機」的步驟 [（範圍）]。</span><span class="sxs-lookup"><span data-stu-id="cb419-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="cb419-221">e.</span><span class="sxs-lookup"><span data-stu-id="cb419-221">e.</span></span> <span data-ttu-id="cb419-222">**如果它是商機的更新，請選取此**方式。</span><span class="sxs-lookup"><span data-stu-id="cb419-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="cb419-223">**若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="cb419-224">f.</span><span class="sxs-lookup"><span data-stu-id="cb419-224">f.</span></span> <span data-ttu-id="cb419-225">選取 **[如果是]** ，然後按一下 [**更新現有商機**]</span><span class="sxs-lookup"><span data-stu-id="cb419-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="cb419-226">若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="cb419-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="cb419-227">a.</span><span class="sxs-lookup"><span data-stu-id="cb419-227">a.</span></span> <span data-ttu-id="cb419-228">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="cb419-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="cb419-229">b.</span><span class="sxs-lookup"><span data-stu-id="cb419-229">b.</span></span> <span data-ttu-id="cb419-230">選取 **[（範圍）] 以同步處理商機**。</span><span class="sxs-lookup"><span data-stu-id="cb419-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="cb419-231">c.</span><span class="sxs-lookup"><span data-stu-id="cb419-231">c.</span></span> <span data-ttu-id="cb419-232">若要自訂 update 事件的 CRM 欄位對應，請選取 **[合作夥伴中心與 CRM 中的潛在客戶物件之間是否有差異]，然後**。</span><span class="sxs-lookup"><span data-stu-id="cb419-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="cb419-233">d.</span><span class="sxs-lookup"><span data-stu-id="cb419-233">d.</span></span> <span data-ttu-id="cb419-234">選取子步驟（**如果是**），然後展開 [**以商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="cb419-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="cb419-235">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="cb419-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="cb419-236">若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="cb419-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="cb419-237">a.</span><span class="sxs-lookup"><span data-stu-id="cb419-237">a.</span></span> <span data-ttu-id="cb419-238">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="cb419-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="cb419-239">b.</span><span class="sxs-lookup"><span data-stu-id="cb419-239">b.</span></span> <span data-ttu-id="cb419-240">選取 **[同步處理參考] （範圍）。**</span><span class="sxs-lookup"><span data-stu-id="cb419-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="cb419-241">c.</span><span class="sxs-lookup"><span data-stu-id="cb419-241">c.</span></span> <span data-ttu-id="cb419-242">如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="cb419-243">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="cb419-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="cb419-244">端對端雙向共同銷售參考同步處理</span><span class="sxs-lookup"><span data-stu-id="cb419-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="cb419-245">安裝、設定及自訂電源自動化解決方案之後，您可以測試 Dynamics 365 和合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="cb419-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="cb419-246">必要條件</span><span class="sxs-lookup"><span data-stu-id="cb419-246">Pre-requisites</span></span>

<span data-ttu-id="cb419-247">若要同步處理合作夥伴中心與 Dynamics 365 CRM 之間的參考，Power 自動解決方案會清楚地標示 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="cb419-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="cb419-248">此識別可讓您的賣方小組決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="cb419-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="cb419-249">一組自訂欄位可做為**商機**實體的一部分。</span><span class="sxs-lookup"><span data-stu-id="cb419-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="cb419-250">CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。</span><span class="sxs-lookup"><span data-stu-id="cb419-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="cb419-251">下列自訂欄位應為 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="cb419-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="cb419-252">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="cb419-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="cb419-253">**參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="cb419-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="cb419-254">**參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="cb419-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="cb419-255">**Microsoft help？**： microsoft 針對此參考所需的協助</span><span class="sxs-lookup"><span data-stu-id="cb419-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="cb419-256">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="cb419-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="cb419-257">**Audit**：與合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="cb419-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="cb419-258">場景</span><span class="sxs-lookup"><span data-stu-id="cb419-258">SCENARIOS:</span></span>

1. <span data-ttu-id="cb419-259">在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="cb419-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="cb419-260">以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 DYNAMICS 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="cb419-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="cb419-261">當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="cb419-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="商機":::

   3. <span data-ttu-id="cb419-263">若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="cb419-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="cb419-264">**與合作夥伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="cb419-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="cb419-265">**Microsoft help？**：請從下列專案中選取：</span><span class="sxs-lookup"><span data-stu-id="cb419-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="協助選取":::

      - <span data-ttu-id="cb419-267">**產品**：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="cb419-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="cb419-268">一旦在 Dynamics 365 中建立商機，並將 [與**合作夥伴中心同步**] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="cb419-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="cb419-269">您的參考會與 Dynamics 365 進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="cb419-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="cb419-270">同樣地，如果您更新 Dynamics 365 CRM 中的機會，則會在您的合作夥伴中心帳戶中同步處理變更，並將 [與合作夥伴中心同步] 選項設為 [是]。</span><span class="sxs-lookup"><span data-stu-id="cb419-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="cb419-271">與合作夥伴中心成功同步處理的機會，將會使用 Dynamics 365 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="cb419-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="cb419-272">在 Microsoft 合作夥伴中心建立或更新參照時的參考同步處理，並在 Dynamics 365 環境中進行同步處理：</span><span class="sxs-lookup"><span data-stu-id="cb419-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="cb419-273">登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="cb419-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="cb419-274">從左側功能表中選取 [**參考**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="cb419-275">按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="cb419-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="cb419-276">登入您的 Dynamics 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="cb419-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="cb419-277">流覽至 [**開啟商機**]。</span><span class="sxs-lookup"><span data-stu-id="cb419-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="cb419-278">在 Microsoft 合作夥伴中心建立的參考現在已在 Dynamics 365 CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="cb419-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="cb419-279">當您選取同步處理的參考時，會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="cb419-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cb419-280">後續步驟</span><span class="sxs-lookup"><span data-stu-id="cb419-280">Next steps</span></span>

- [<span data-ttu-id="cb419-281">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="cb419-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="cb419-282">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="cb419-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="cb419-283">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="cb419-283">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="cb419-284">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="cb419-284">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)