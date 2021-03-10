---
title: Dynamics 365 CRM 合作夥伴中心的共同銷售連接器
ms.topic: how-to
ms.date: 03/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Dynamics 365 CRM 的共同銷售連接器，同步處理合作夥伴中心內的推薦。 然後，銷售人員可以從您的 CRM 系統內與 Microsoft 共同銷售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 3724b53f527ebe294590c09d7ad77d0dbcfd9c34
ms.sourcegitcommit: 5e9ca304cce4575eed05ca3b17fb77c9711402a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "102532027"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="f9e53-104">Dynamics 365 CRM 的共同銷售連接器–總覽</span><span class="sxs-lookup"><span data-stu-id="f9e53-104">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="f9e53-105">適當的角色</span><span class="sxs-lookup"><span data-stu-id="f9e53-105">Appropriate roles</span></span>

- <span data-ttu-id="f9e53-106">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="f9e53-106">Referrals admin</span></span>
- <span data-ttu-id="f9e53-107">CRM 上的系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="f9e53-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="f9e53-108">合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。</span><span class="sxs-lookup"><span data-stu-id="f9e53-108">Partner Center Co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="f9e53-109">他們不必經過訓練，就能使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="f9e53-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="f9e53-110">使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。</span><span class="sxs-lookup"><span data-stu-id="f9e53-110">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="f9e53-111">您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="f9e53-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="f9e53-112">您可以在您選擇的 CRM 中管理所有的參考工作，而不是在合作夥伴中心內。</span><span class="sxs-lookup"><span data-stu-id="f9e53-112">You can manage all of your referrals work in the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="f9e53-113">解決方案是以 Microsoft Power 自動化解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="f9e53-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="f9e53-114">安裝之前的先決條件</span><span class="sxs-lookup"><span data-stu-id="f9e53-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="f9e53-115">**主題**</span><span class="sxs-lookup"><span data-stu-id="f9e53-115">**Topics**</span></span>   |<span data-ttu-id="f9e53-116">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="f9e53-116">**Details**</span></span>   |<span data-ttu-id="f9e53-117">**連結**</span><span class="sxs-lookup"><span data-stu-id="f9e53-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="f9e53-118">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="f9e53-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="f9e53-119">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="f9e53-119">You need a valid MPN ID</span></span>|<span data-ttu-id="f9e53-120">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f9e53-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="f9e53-121">共同銷售準備就緒</span><span class="sxs-lookup"><span data-stu-id="f9e53-121">Co-sell ready</span></span>|<span data-ttu-id="f9e53-122">您的 IP/服務解決方案必須已準備好共同銷售。</span><span class="sxs-lookup"><span data-stu-id="f9e53-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="f9e53-123">與 Microsoft 銷售</span><span class="sxs-lookup"><span data-stu-id="f9e53-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="f9e53-124">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="f9e53-124">Partner Center account</span></span>|<span data-ttu-id="f9e53-125">與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="f9e53-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="f9e53-126">先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。</span><span class="sxs-lookup"><span data-stu-id="f9e53-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="f9e53-127">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="f9e53-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="f9e53-128">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="f9e53-128">Partner Center user roles</span></span>|<span data-ttu-id="f9e53-129">將安裝並使用連接器的員工必須是推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="f9e53-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="f9e53-130">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="f9e53-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| 
|<span data-ttu-id="f9e53-131">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="f9e53-131">Dynamics 365 CRM</span></span>|<span data-ttu-id="f9e53-132">CRM 使用者角色是系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="f9e53-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="f9e53-133">在 Dynamics 365 中指派角色</span><span class="sxs-lookup"><span data-stu-id="f9e53-133">Assign roles in Dynamics 365</span></span>](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="f9e53-134">Power 自動化流程帳戶</span><span class="sxs-lookup"><span data-stu-id="f9e53-134">Power Automate Flow Account</span></span>|<span data-ttu-id="f9e53-135">使用資料庫為測試/預備和生產環境建立新的生產環境。</span><span class="sxs-lookup"><span data-stu-id="f9e53-135">Create new production environment with database for test/staging and production.</span></span> <span data-ttu-id="f9e53-136">如果您有現有的生產環境與資料庫，就可以重複使用。</span><span class="sxs-lookup"><span data-stu-id="f9e53-136">If you have an existing production environment with database it can be re-used.</span></span> <span data-ttu-id="f9e53-137">即將安裝連接器解決方案的使用者必須具備 Power 自動化授權和此環境的存取權。您可以按一下 [方案] 底下的 [查看歷程記錄]，來監視進度，並在 [電源自動化](https://flow.microsoft.com/) 時取得更多詳細資料。</span><span class="sxs-lookup"><span data-stu-id="f9e53-137">User who is going to install connector solution needs to have Power Automate license and access to this environment.You can monitor the progress and get more details should the installation fail in [Power Automate](https://flow.microsoft.com/) by clicking See history under Solutions.</span></span>|[<span data-ttu-id="f9e53-138">建立或管理環境</span><span class="sxs-lookup"><span data-stu-id="f9e53-138">Create or manage environment</span></span>](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="f9e53-139">安裝 Dynamics 365 (Power 自動化解決方案) 的合作夥伴中心推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="f9e53-139">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="f9e53-140">移至 [ [電源自動化](https://flow.microsoft.com) ]，然後在右上角選取 [ **環境** ]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-140">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="f9e53-141">此步驟會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="f9e53-141">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="f9e53-142">從右上角的下拉式清單中選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="f9e53-142">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="f9e53-143">選取左側導覽列上的 [ **方案** ]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-143">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="f9e53-144">按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="f9e53-144">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="f9e53-146">在快顯視窗中搜尋 **合作夥伴中心的推薦連接器以進行 Dynamics365** 。</span><span class="sxs-lookup"><span data-stu-id="f9e53-146">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="f9e53-147">按一下 [ **立即取得** ] 按鈕，然後 **繼續** 進行。</span><span class="sxs-lookup"><span data-stu-id="f9e53-147">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="f9e53-148">這會開啟頁面，您可以在其中選取 CRM (Dynamics 365) 環境以安裝應用程式。</span><span class="sxs-lookup"><span data-stu-id="f9e53-148">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="f9e53-149">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="f9e53-149">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="f9e53-150">您可以按一下 [**方案**] 底下的 [**查看歷程記錄**]，來監視進度，並在電源自動化時取得更多詳細資料。</span><span class="sxs-lookup"><span data-stu-id="f9e53-150">You can monitor the progress and get more details should the installation fail in Power Automate by clicking **See history** under **Solutions**.</span></span>
 

9. <span data-ttu-id="f9e53-151">安裝完成之後，請流覽回到 [ [電源自動化](https://flow.microsoft.com) ]，然後從左側導覽區域選取 [ **解決方案** ]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="f9e53-152">請注意，[方案] 清單中有提供 **Dynamics 365 的合作夥伴中心推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="f9e53-153">選取 **Dynamics 365 的合作夥伴中心推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="f9e53-154">以下是可用的 Power 自動化流程和實體：</span><span class="sxs-lookup"><span data-stu-id="f9e53-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用的 CRM":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="f9e53-156">最佳做法：上線之前先進行測試</span><span class="sxs-lookup"><span data-stu-id="f9e53-156">Best practice: test before you go live</span></span>

<span data-ttu-id="f9e53-157">在生產環境中安裝、設定和自訂 Power 自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="f9e53-158">在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="f9e53-159">設定和自訂預備環境中的 Microsoft Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-159">Configure and customize the Microsoft Power Automate solution in staging environment.</span></span>
- <span data-ttu-id="f9e53-160">測試預備/CRM 實例上的方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="f9e53-161">成功時，請將受控解決方案匯入至生產環境實例。</span><span class="sxs-lookup"><span data-stu-id="f9e53-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="f9e53-162">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="f9e53-162">Configure the solution</span></span>

1. <span data-ttu-id="f9e53-163">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power 自動化](https://flow.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="f9e53-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>


2. <span data-ttu-id="f9e53-164">從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power 自動化解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="f9e53-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="f9e53-165">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="f9e53-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="f9e53-166">具有推薦系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="f9e53-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="f9e53-167">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="f9e53-167">Partner Center Events</span></span>

   - <span data-ttu-id="f9e53-168">具有解決方案中電源自動化流程的 CRM 系統管理員。</span><span class="sxs-lookup"><span data-stu-id="f9e53-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="f9e53-169">從左側導覽列中選取 [連線]， **然後從清單** 中選取 [合作夥伴中心推薦] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="f9e53-170">按一下 [ **建立連接**] 來建立連接。</span><span class="sxs-lookup"><span data-stu-id="f9e53-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="建立連線":::

      3. <span data-ttu-id="f9e53-172">在右上角的搜尋列中搜尋 **合作夥伴中心的推薦 (預覽)** 。</span><span class="sxs-lookup"><span data-stu-id="f9e53-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="f9e53-173">為合作夥伴中心使用者建立具有「參考系統管理員」認證角色的連接。</span><span class="sxs-lookup"><span data-stu-id="f9e53-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="f9e53-174">接下來，使用推薦的系統管理員認證來建立合作夥伴中心使用者的合作夥伴中心事件連線。</span><span class="sxs-lookup"><span data-stu-id="f9e53-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="f9e53-175">為 CRM 系統管理員使用者 (目前的環境) 建立 Common Data Service 的連接。</span><span class="sxs-lookup"><span data-stu-id="f9e53-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>
     
      7. <span data-ttu-id="f9e53-176">新增所有連線之後，您應該會在您的環境中看到下列連接：</span><span class="sxs-lookup"><span data-stu-id="f9e53-176">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

         :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="連線":::
   
## <a name="edit-the-connections"></a><span data-ttu-id="f9e53-178">編輯連接</span><span class="sxs-lookup"><span data-stu-id="f9e53-178">Edit the connections</span></span>

1. <span data-ttu-id="f9e53-179">返回 [ **方案** ] 頁面，然後選取 [ **預設方案**]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-179">Return to the **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="f9e53-180">按一下 [**全部**]，以選取 [ **(預覽) 的連接參考**。</span><span class="sxs-lookup"><span data-stu-id="f9e53-180">Select **Connection Reference (preview)** by clicking **All**.</span></span>

:::image type="content" source="images/connection-reference-video.gif" alt-text="編輯連接":::

2. <span data-ttu-id="f9e53-182">選取三個點圖示，逐一編輯每一個連接。</span><span class="sxs-lookup"><span data-stu-id="f9e53-182">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="f9e53-183">新增相關的連接。</span><span class="sxs-lookup"><span data-stu-id="f9e53-183">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="列出的連接"::: 

3.  <span data-ttu-id="f9e53-185">返回 [解決方案] 頁面，選取 [Dynamics 365 的合作夥伴中心推薦同步處理]，然後按一下下列順序中每個流程旁的三個點圖示，即可開啟流程。</span><span class="sxs-lookup"><span data-stu-id="f9e53-185">Return to the Solutions page, select Partner Center Referrals Synchronization for Dynamics 365 and turn on the flow by clicking on three dots icon next to each flow in the following sequence.</span></span> <span data-ttu-id="f9e53-186">如果您在開啟流程時遇到任何問題，請參閱 [自訂步驟](connector-dynamics.md#customize-synchronization-steps) 和 [疑難排解步驟](connectors-troubleshoot.md)。</span><span class="sxs-lookup"><span data-stu-id="f9e53-186">If you encounter any issues while turning on the flow refer to [customization steps](connector-dynamics.md#customize-synchronization-steps) and [troubleshooting steps](connectors-troubleshoot.md).</span></span> 

<span data-ttu-id="f9e53-187">依下列順序開啟流程：</span><span class="sxs-lookup"><span data-stu-id="f9e53-187">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="f9e53-188">合作夥伴中心 Webhook 註冊 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-188">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-189">建立共同銷售參考– Dynamics 365 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-189">Create Co-sell Referral – Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-190">定制從 Dynamics 365 flow 建立或取得詳細資料</span><span class="sxs-lookup"><span data-stu-id="f9e53-190">[Customize] Create or Get Details from Dynamics 365 flow</span></span> 
- <span data-ttu-id="f9e53-191">合作夥伴中心至 Dynamics 365-Helper (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-191">Partner Center to Dynamics 365 - Helper (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-192">合作夥伴中心 Microsoft 共同銷售參考更新至 Dynamics 365 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-192">Partner Center Microsoft Co-sell Referral Updates to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-193">合作夥伴中心至 Dynamics 365 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-193">Partner Center to Dynamics 365 (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-194">Dynamics 365 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-194">Dynamics 365 to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-195">Dynamics 365 商機至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-195">Dynamics 365 Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="f9e53-196">Dynamics 365 Microsoft 解決方案至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="f9e53-196">Dynamics 365 Microsoft Solutions to Partner Center (Insider Preview)</span></span>
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="f9e53-197">使用 Webhook Api 來註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="f9e53-197">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="f9e53-198">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="f9e53-198">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="f9e53-199">這些變更事件會以 HTTP 文章的形式傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="f9e53-199">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="f9e53-200">選取 **合作夥伴中心至 Dynamics 365 (Insider preview)**。</span><span class="sxs-lookup"><span data-stu-id="f9e53-200">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

2. <span data-ttu-id="f9e53-201">選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-201">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

3. <span data-ttu-id="f9e53-202">選取 **複製** 圖示來複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="f9e53-202">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/webhook-video.gif" alt-text="使用 webhook 來註冊資源變更":::

4. <span data-ttu-id="f9e53-204">選取「合作夥伴中心 Webhook 註冊 (Insider Preview) 」電源自動化流程，然後選取 [ **執行**]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-204">Select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and then select **Run**.</span></span>

5. <span data-ttu-id="f9e53-205">確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-205">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

6. <span data-ttu-id="f9e53-206">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="f9e53-206">Enter the following details:</span></span>

   - <span data-ttu-id="f9e53-207">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="f9e53-207">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

   - <span data-ttu-id="f9e53-208">**要註冊的事件**：選取所有可用事件 ( 「參考建立」、「參考-已建立」、「相關-推薦」、「相關-已更新」 ) </span><span class="sxs-lookup"><span data-stu-id="f9e53-208">**Events to Register**: Select all available events (“referral-created”, “referral-updated”, “related-referral-created”, “related-referral-updated”)</span></span>

   <span data-ttu-id="f9e53-209">-**覆寫現有的觸發程式端點（如果有的話**）：是，請務必注意，只有一個 URL 可以針對指定的 webhook 事件註冊。</span><span class="sxs-lookup"><span data-stu-id="f9e53-209">-**Overwrite existing trigger endpoints if present**: Yes It is important to note that only one URL can be registered for a given webhook event.</span></span> <span data-ttu-id="f9e53-210">請務必注意，只有一個 URL 可以針對指定的 webhook 事件註冊。</span><span class="sxs-lookup"><span data-stu-id="f9e53-210">It is important to note that only one URL can be registered for a given webhook event.</span></span> 

7. <span data-ttu-id="f9e53-211">選取 [ **執行** ]，然後選取 [ **完成]。**</span><span class="sxs-lookup"><span data-stu-id="f9e53-211">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="f9e53-212">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="f9e53-212">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="f9e53-213">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="f9e53-213">Customize synchronization steps</span></span>

<span data-ttu-id="f9e53-214">CRM 系統經過高度自訂，而且您可以根據您的 CRM 設定自訂 Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-214">CRM systems are highly customized, and you can customize the Power Automate solution based on your CRM setup.</span></span>  <span data-ttu-id="f9e53-215">當合作夥伴中心與您的 CRM 系統之間的共同銷售參照進行同步處理時，在合作夥伴中心電腦上同步處理的欄位會列在 [自訂欄位對應指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)中。</span><span class="sxs-lookup"><span data-stu-id="f9e53-215">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed in the [Custom field mapping guide](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).</span></span>

<span data-ttu-id="f9e53-216">依照欄位對應指南操作，如有必要，請在 [自訂] 中進行適當的變更，並 **從 Dynamics 365 流程或環境變數取得詳細資料**  。</span><span class="sxs-lookup"><span data-stu-id="f9e53-216">Follow the field mapping guide, and if necessary, make appropriate changes in **[Customize] Create or Get Details from Dynamics 365 flow**  or environment variables.</span></span> <span data-ttu-id="f9e53-217">建議您不要更新 Power 自動化解決方案中的任何其他流程，因為它可能會影響未來的解決方案升級。</span><span class="sxs-lookup"><span data-stu-id="f9e53-217">It is recommended not to update any other flows in Power Automate solution as it can impact future solution upgrades.</span></span> 

<span data-ttu-id="f9e53-218">可用的自訂如下：</span><span class="sxs-lookup"><span data-stu-id="f9e53-218">The following are the available customizations:</span></span>

- <span data-ttu-id="f9e53-219">核取 [商機名稱] 中的 [標記]：根據預設，[商機名稱] 旁邊會顯示核取記號，表示合作夥伴中心與 Dynamics 365 CRM 之間的同步處理已成功發生。</span><span class="sxs-lookup"><span data-stu-id="f9e53-219">Check mark in Opportunity name: By default, a check mark will be displayed next to Opportunity name to indicate that synchronization between Partner Center and Dynamics 365 CRM is happening successfully.</span></span> <span data-ttu-id="f9e53-220">同樣地，如果同步處理失敗，將會顯示交叉標記。</span><span class="sxs-lookup"><span data-stu-id="f9e53-220">Similarly, a cross mark will be displayed if synchronization fails.</span></span> <span data-ttu-id="f9e53-221">若要避免在商機名稱中新增核取或交叉標記，請將 [商機名稱] 環境變數中 [顯示] 核取記號的目前值設定為 [否]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-221">To avoid adding check or cross mark in Opportunity name, set the current value of Display check mark in opportunity name environment variable to No.</span></span>

- <span data-ttu-id="f9e53-222">交易價值：根據預設，合作夥伴中心的交易價值將會在 CRM 中與 **estimatedvalue** 同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-222">Deal value: By default, deal value from Partner Center will be synced to and from **estimatedvalue** in CRM.</span></span> <span data-ttu-id="f9e53-223">如果您在 CRM 中有不同的欄位可供同步處理的價值：</span><span class="sxs-lookup"><span data-stu-id="f9e53-223">If you have a different field in CRM for deal value to sync from:</span></span>

    <span data-ttu-id="f9e53-224">a.</span><span class="sxs-lookup"><span data-stu-id="f9e53-224">a.</span></span>    <span data-ttu-id="f9e53-225">使用 CRM 的功能變數名稱更新 Dynamics 365 環境變數中的交易值功能變數名稱。</span><span class="sxs-lookup"><span data-stu-id="f9e53-225">Update Deal value field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="f9e53-226">請注意，您應該提供欄位的名稱，而不是其顯示名稱。</span><span class="sxs-lookup"><span data-stu-id="f9e53-226">Note that you should provide the field’s name not its display name.</span></span>

    <span data-ttu-id="f9e53-227">b.</span><span class="sxs-lookup"><span data-stu-id="f9e53-227">b.</span></span>    <span data-ttu-id="f9e53-228">編輯 **[自訂] 建立或取得 Dynamics 365 流程的詳細資料**  ，然後流覽至在 Crm 中 **建立或更新** 商機，並更新 **新的** 商機，並 **更新現有的商機** 動作，以將 **DealValue** 值指派給 crm 中的正確欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-228">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update** opportunity in CRM and update **Create a new opportunity** and **Update existing opportunity** actions to assign **DealValue** value to correct field in CRM.</span></span> <span data-ttu-id="f9e53-229">此外，請從 [**估計收益**] 欄位中移除 **DealValue 指派**。</span><span class="sxs-lookup"><span data-stu-id="f9e53-229">Also, remove **DealValue assignment** from **Estimated Revenue** field.</span></span>

- <span data-ttu-id="f9e53-230">客戶帳戶國家/地區代碼：在建立新的參考時，必須提供兩個字母的國家/地區代碼 (ISO 3166) 。</span><span class="sxs-lookup"><span data-stu-id="f9e53-230">Customer Account Country Code: It is mandatory to provide a two-letter country code (ISO 3166) when creating a new referral.</span></span> <span data-ttu-id="f9e53-231">根據預設，國家/地區代碼會與 CRM 中的帳戶 address1_country 欄位進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-231">By default, country code will be synced to and from Account’s address1_country field in CRM.</span></span> <span data-ttu-id="f9e53-232">如果您的 CRM 中有不同的欄位可供同步處理的國家/地區代碼：</span><span class="sxs-lookup"><span data-stu-id="f9e53-232">If you have a different field in CRM for country code to sync from:</span></span>

   <span data-ttu-id="f9e53-233">a.</span><span class="sxs-lookup"><span data-stu-id="f9e53-233">a.</span></span>    <span data-ttu-id="f9e53-234">針對包含雙字母代碼的帳戶中的非查閱國家/地區代碼欄位：</span><span class="sxs-lookup"><span data-stu-id="f9e53-234">For a non-lookup country code field in Account which contains two-letter code:</span></span>

   - <span data-ttu-id="f9e53-235">使用 CRM 的功能變數名稱更新 Dynamics 365 環境變數中的客戶帳戶國家/地區代碼功能變數名稱。</span><span class="sxs-lookup"><span data-stu-id="f9e53-235">Update Customer account country code field name in Dynamics 365 environment variable with the CRM’s field name.</span></span> <span data-ttu-id="f9e53-236">請注意，您應該提供欄位的名稱，而不是其顯示名稱。</span><span class="sxs-lookup"><span data-stu-id="f9e53-236">Note that you should provide the field’s name not its display name.</span></span>

   - <span data-ttu-id="f9e53-237">編輯 **[自訂] 建立或取得 Dynamics 365 流程的詳細資料**  ，然後流覽至 [建立或取得 crm 中的客戶帳戶] 動作，將國家/地區值指派給 crm 中的正確欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-237">Edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to Create or get customer account in CRM action to assign Country value to correct field in CRM.</span></span> <span data-ttu-id="f9e53-238">此外，請移除位址1：國家/地區欄位中的國家/地區值指派。</span><span class="sxs-lookup"><span data-stu-id="f9e53-238">Also, remove Country value assignment from Address 1: Country/Region field.</span></span>

   <span data-ttu-id="f9e53-239">b.</span><span class="sxs-lookup"><span data-stu-id="f9e53-239">b.</span></span>    <span data-ttu-id="f9e53-240">針對帳戶中的 [以查閱為基礎的國家/地區代碼] 欄位：</span><span class="sxs-lookup"><span data-stu-id="f9e53-240">For a lookup-based country code field in Account:</span></span>

   - <span data-ttu-id="f9e53-241">在 [帳戶] 中加入新的自訂欄位，並使用兩個字母的國家/地區代碼自動填入 (ISO 3166) 根據 [查閱] 欄位中選取的值，反之亦然。</span><span class="sxs-lookup"><span data-stu-id="f9e53-241">Add a new custom field in Account and auto-populate it with two-letter country code (ISO 3166) based on the value selected in lookup-based field and vice-versa.</span></span>

   - <span data-ttu-id="f9e53-242">遵循上述的步驟，針對非查閱國家/地區代碼欄位，將新的自訂欄位從 CRM 同步處理到合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="f9e53-242">Follow the steps above for non-lookup country code field to sync new custom field from CRM to and from Partner Center.</span></span>

- <span data-ttu-id="f9e53-243">商機欄位：如果商機中有必要的欄位需要擴展 **[自訂]，請從 Dynamics 365 Flow 建立或取得詳細資料**  ，並在 CRM 中流覽至 **建立或更新商機** ，並更新 **建立新的商機動作** ，根據您的業務需求將值指派給必要欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-243">Opportunity fields: If there are mandatory fields in Opportunity that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update opportunity** in CRM and update **Create a new opportunity action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="f9e53-244">潛在客戶欄位：如果潛在客戶中有需要填入的強制欄位： **[自訂] 建立或從 Dynamics 365 流程取得詳細資料**  ，然後流覽至 [ **建立或更新** CRM 中的潛在客戶] 和 [更新] **建立新的潛在客戶動作** ，根據您的業務需求將值指派給必要欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-244">Lead fields: If there are mandatory fields in Lead that needs to be populated edit **[Customize] Create or Get Details from Dynamics 365 flow**  and navigate to **Create or update lead** in CRM and update **Create a new lead action** to assign values to the mandatory fields based on your business requirements.</span></span>

- <span data-ttu-id="f9e53-245">客戶帳戶：當新的參考從合作夥伴中心同步處理至 CRM 時，Power 自動化解決方案會嘗試使用客戶公司名稱和郵遞區號在 CRM 中搜尋現有的帳戶。</span><span class="sxs-lookup"><span data-stu-id="f9e53-245">Customer Account: When a new referral is synced from Partner Center to CRM, Power Automate solution tries to search for an existing account in CRM using customer company name and postal code.</span></span> <span data-ttu-id="f9e53-246">如果找不到，則會在 CRM 中建立新的客戶帳戶。</span><span class="sxs-lookup"><span data-stu-id="f9e53-246">If it does not find one, a new customer account will be created in CRM.</span></span> <span data-ttu-id="f9e53-247">若要更新搜尋條件和新的帳戶建立詳細資料，請編輯 **[自訂] 建立或從 Dynamics 365 流程取得詳細資料** ，然後流覽至在 CRM 中 **建立或取得客戶帳戶** ，並 **建立客戶帳戶動作**。</span><span class="sxs-lookup"><span data-stu-id="f9e53-247">To update the search criteria and new account creation details, edit **[Customize] Create or Get Details from Dynamics 365 flow** and navigate to **Create or get customer account** in CRM and **Create customer account action**.</span></span>

## <a name="update-environment-variable"></a><span data-ttu-id="f9e53-248">更新環境變數</span><span class="sxs-lookup"><span data-stu-id="f9e53-248">Update environment variable</span></span>

<span data-ttu-id="f9e53-249">若要更新環境變數值：</span><span class="sxs-lookup"><span data-stu-id="f9e53-249">To update an environment variable value:</span></span>

1. <span data-ttu-id="f9e53-250">移至 [ **方案** ] 頁面，然後選取 [ **預設方案**]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-250">Go to **Solutions** page and select **Default Solution**.</span></span> <span data-ttu-id="f9e53-251">按一下 [全部]，以選取 [ **環境變數** ]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-251">Select **Environment Variable** by clicking All.</span></span>

2. <span data-ttu-id="f9e53-252">針對需要更新的值選取環境變數，然後按一下 [使用三個點 **編輯** ] 圖示。</span><span class="sxs-lookup"><span data-stu-id="f9e53-252">Select the environment variable for the value that needs to be updated and click **Edit** using three dots icon.</span></span>

3. <span data-ttu-id="f9e53-253">更新 **目前的值** (請勿使用 [ **新值** ] 選項) 更新預設值，並提供值。</span><span class="sxs-lookup"><span data-stu-id="f9e53-253">Update **Current Value** (do not update Default Value) using **New value** option and provide the value.</span></span> <span data-ttu-id="f9e53-254">值必須符合變數的資料類型，例如 [是]/[否] 資料類型會接受 [是] 或 [否] 值。</span><span class="sxs-lookup"><span data-stu-id="f9e53-254">Value must match the Data type of the variable for e.g. Yes/No data type will accept either Yes or No value.</span></span>

 :::image type="content" source="images/environment-variables-video.gif" alt-text="更新環境變數":::

- <span data-ttu-id="f9e53-256">端對端雙向共同銷售推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="f9e53-256">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="f9e53-257">安裝、設定和自訂 Power 自動化解決方案之後，您可以測試 Dynamics 365 與合作夥伴中心之間的共同銷售推薦同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-257">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f9e53-258">必要條件</span><span class="sxs-lookup"><span data-stu-id="f9e53-258">Pre-requisites</span></span>

<span data-ttu-id="f9e53-259">若要同步處理合作夥伴中心與 Dynamics 365 CRM 之間的參考，Power 自動化解決方案會清楚標示 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-259">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="f9e53-260">此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="f9e53-260">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="f9e53-261">在解決方案安裝過程中，會加入一組自訂欄位和物件。</span><span class="sxs-lookup"><span data-stu-id="f9e53-261">A set of custom fields and objects will get added as part of the solution installation.</span></span> <span data-ttu-id="f9e53-262">CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="f9e53-262">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="f9e53-263">下列自訂欄位應該是 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="f9e53-263">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="f9e53-264">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步商機。</span><span class="sxs-lookup"><span data-stu-id="f9e53-264">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center.</span></span> <span data-ttu-id="f9e53-265">依預設，此欄位的值為 [否]，而且您的賣方必須明確設定為 [是]，才能與 Microsoft 分享商機。</span><span class="sxs-lookup"><span data-stu-id="f9e53-265">By default, the value of this field is No and needs to be explicitly set to Yes by your seller to share an opportunity with Microsoft.</span></span> <span data-ttu-id="f9e53-266">從合作夥伴中心共用的新參考會將此域值設定為 [是]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-266">New referrals shared from Partner Center to CRM will have this field value set to Yes.</span></span>

- <span data-ttu-id="f9e53-267">**參考識別碼**： Microsoft 合作夥伴中心的唯讀識別碼欄位參考</span><span class="sxs-lookup"><span data-stu-id="f9e53-267">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="f9e53-268">**參考連結**： Microsoft 合作夥伴中心內的參考唯讀連結</span><span class="sxs-lookup"><span data-stu-id="f9e53-268">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>
- <span data-ttu-id="f9e53-269">**Microsoft 如何協助？**： microsoft 提供的參考說明。</span><span class="sxs-lookup"><span data-stu-id="f9e53-269">**How can Microsoft help?**: Help required from Microsoft for the referral.</span></span> <span data-ttu-id="f9e53-270">若要建立共同銷售的參考，請選取 Microsoft 所需的適當說明。</span><span class="sxs-lookup"><span data-stu-id="f9e53-270">To create a co-sell referral, select appropriate help required from Microsoft.</span></span> <span data-ttu-id="f9e53-271">客戶連絡人必須與建立共同銷售參考的商機相關聯。</span><span class="sxs-lookup"><span data-stu-id="f9e53-271">A customer contact must be associated to the Opportunity to create a co-sell referral.</span></span> <span data-ttu-id="f9e53-272">若要建立非共同銷售的參考，請不要選取此欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-272">To create a non co-sell referral leave this field un-selected.</span></span> <span data-ttu-id="f9e53-273">您可以藉由選取適當的 [必要的說明] 選項，隨時將非共同銷售的參考轉換成共同銷售的參考。</span><span class="sxs-lookup"><span data-stu-id="f9e53-273">A non co-sell referral can be converted to a co-sell referral anytime by selecting appropriate help required option.</span></span>

- <span data-ttu-id="f9e53-274">**Microsoft 合作夥伴中心的參考可見度**：選取 Microsoft 合作夥伴中心推薦的可見度。</span><span class="sxs-lookup"><span data-stu-id="f9e53-274">**Microsoft Partner Center Referral Visibility**: Select visibility for Microsoft Partner Center Referral.</span></span> <span data-ttu-id="f9e53-275">藉由讓 Microsoft 銷售人員看得到，非共同銷售的參考可能會轉換成共同銷售。</span><span class="sxs-lookup"><span data-stu-id="f9e53-275">By making it visible to Microsoft sellers, a non co-sell referral may get converted to co-sell.</span></span> <span data-ttu-id="f9e53-276">當需要 Microsoft 協助時，預設會對 Microsoft 銷售者顯示推薦。</span><span class="sxs-lookup"><span data-stu-id="f9e53-276">When Microsoft help is required, referral is visible to Microsoft sellers by default.</span></span> <span data-ttu-id="f9e53-277">標記為可見之後，就無法還原此欄位。</span><span class="sxs-lookup"><span data-stu-id="f9e53-277">Once marked as visible this field cannot be reverted.</span></span>

- <span data-ttu-id="f9e53-278">**MICROSOFT CRM 識別碼**：當共同銷售的參考是由 microsoft 所建立並接受時，此欄位將會填入 MICROSOFT 的 CRM 識別碼。</span><span class="sxs-lookup"><span data-stu-id="f9e53-278">**Microsoft CRM Identifier**: When a co-sell referral is created and accepted by Microsoft, this field will get populated with Microsoft’s CRM identifier.</span></span>

- <span data-ttu-id="f9e53-279">**產品：已淘汰** –請勿使用此欄位或將它新增至 CRM 區段，只適用于回溯相容性。</span><span class="sxs-lookup"><span data-stu-id="f9e53-279">**Products: Obsolete** – do not use this field or add it to CRM section, it is available for backward compatibility only.</span></span> <span data-ttu-id="f9e53-280">改為使用 Microsoft 合作夥伴中心方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-280">Use Microsoft Partner Center Solutions instead.</span></span>

- <span data-ttu-id="f9e53-281">**Audit**：與合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="f9e53-281">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

- <span data-ttu-id="f9e53-282">**Microsoft 合作夥伴中心解決方案**：自訂物件，可將共同銷售就緒解決方案或 Microsoft 解決方案與商機產生關聯。</span><span class="sxs-lookup"><span data-stu-id="f9e53-282">**Microsoft Partner Center Solutions**: A custom object to associate Co-sell ready solutions or Microsoft solutions with the opportunity.</span></span> <span data-ttu-id="f9e53-283">您可以新增及/或從商機中移除一或多個解決方案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-283">One or more solutions can be added and/or removed from the Opportunity.</span></span> <span data-ttu-id="f9e53-284">在與 Microsoft 共用之前，您必須先將至少一個共同銷售就緒或 Microsoft 解決方案新增至商機。</span><span class="sxs-lookup"><span data-stu-id="f9e53-284">It is mandatory to add at least one Co-sell ready or Microsoft solution to the Opportunity before sharing it with Microsoft.</span></span> <span data-ttu-id="f9e53-285">若要建立此物件與商機之間的關聯，請更新 CRM 中的商機表單：</span><span class="sxs-lookup"><span data-stu-id="f9e53-285">To associate this object to Opportunity, update the Opportunity form in CRM:</span></span>

  <span data-ttu-id="f9e53-286">在 [商機] 表單中選取適當的索引標籤，然後新增子方格，如下所示：</span><span class="sxs-lookup"><span data-stu-id="f9e53-286">Select the appropriate tab in Opportunity form and add a sub-grid as shown below:</span></span>

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="商機表單":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{替代文字}":::



- <span data-ttu-id="f9e53-289">新增 Microsoft 解決方案之後，您可以預先填入共同銷售就緒解決方案詳細資料，讓您的銷售人員不需要新增它們。</span><span class="sxs-lookup"><span data-stu-id="f9e53-289">After adding Microsoft Solutions, you can pre-populate Co-sell ready solutions details so that your sellers don’t have to add them.</span></span> <span data-ttu-id="f9e53-290">若要加入新的解決方案詳細資料，請移至 CRM 中的 Microsoft 解決方案詳細資料物件，然後按一下 [ **新增記錄** ] 以新增一個專案，或使用 **Excel 上傳** 來新增多個專案。</span><span class="sxs-lookup"><span data-stu-id="f9e53-290">To add a new solution detail, go to Microsoft Solution Details object in CRM and click on **Add Record** to add one entry or use **Excel upload** to add multiple entries.</span></span>

:::image type="content" source="images/dynamic-1a.png" alt-text="解決方案詳細資料":::

### <a name="scenarios"></a><span data-ttu-id="f9e53-292">場景：</span><span class="sxs-lookup"><span data-stu-id="f9e53-292">SCENARIOS:</span></span>

1. <span data-ttu-id="f9e53-293">在 CRM 中建立或更新參考時的參考同步處理，並在合作夥伴中心內同步處理：</span><span class="sxs-lookup"><span data-stu-id="f9e53-293">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="f9e53-294">登入您的 Dynamics 365 CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。</span><span class="sxs-lookup"><span data-stu-id="f9e53-294">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="f9e53-295">當您在 Dynamics 365 環境中建立「新商機」時，請確定 Microsoft 合作夥伴中心區段存在</span><span class="sxs-lookup"><span data-stu-id="f9e53-295">Ensure that the Microsoft Partner Center section  is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   :::image type="content" source="images/dynamic-2a.png" alt-text="新商機"::: 

   3. <span data-ttu-id="f9e53-297">若要與合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="f9e53-297">To synchronize this opportunity with Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="f9e53-298">**Microsoft 如何協助？**：若要建立共同銷售的參考，請選取適當的說明選項。</span><span class="sxs-lookup"><span data-stu-id="f9e53-298">**How can Microsoft help?**: To create a Co-sell referral select an appropriate help option.</span></span>

         :::image type="content" source="images/dynamic-3a.png" alt-text="如何在卡片視圖中取得適當的欄位":::

      - <span data-ttu-id="f9e53-300">**客戶連絡人**：若要建立共同銷售的參考，請將客戶連絡人新增至商機。</span><span class="sxs-lookup"><span data-stu-id="f9e53-300">**Customer Contact**: To create a Co-sell referral, add a customer contact to Opportunity.</span></span>
      - <span data-ttu-id="f9e53-301">**與合作夥伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="f9e53-301">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="f9e53-302">Microsoft 解決方案：若要與 Microsoft 分享參考，請將有效的共同銷售就緒或 Microsoft 解決方案新增至商機。</span><span class="sxs-lookup"><span data-stu-id="f9e53-302">Microsoft Solutions: To share a referral with Microsoft, add a valid Co-sell ready or Microsoft solution to Opportunity.</span></span>
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="解決方案識別碼":::

   4. <span data-ttu-id="f9e53-304">一旦在 Dynamics 365 中建立商機，並將 [同步與合作夥伴中心] 選項設為 [是]，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="f9e53-304">Once the opportunity is created in Dynamics 365 with Sync with Partner Center option set to Yes, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="f9e53-305">您的參考會與 Dynamics 365 和參考識別碼進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-305">Your referrals will be synchronized with Dynamics 365 and Referral Identifier.</span></span> <span data-ttu-id="f9e53-306">將會填入參考連結。</span><span class="sxs-lookup"><span data-stu-id="f9e53-306">Referral Link will get populated.</span></span> <span data-ttu-id="f9e53-307">如果發生失敗，[審核] 欄位將會填入錯誤資訊。</span><span class="sxs-lookup"><span data-stu-id="f9e53-307">In case of a failure, the audit field will be populated with error information.</span></span>
     
    5. <span data-ttu-id="f9e53-308">同樣地，如果有機會將 [與合作夥伴中心同步] 選項設為 [是]，則當您更新 Dynamics 365 CRM 的商機時，變更將會在您的合作夥伴中心帳戶中同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-308">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    6. <span data-ttu-id="f9e53-309">使用合作夥伴中心成功同步處理的商機將會以 Dynamics 365 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="f9e53-309">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="f9e53-310">在 Microsoft 合作夥伴中心內建立或更新參考時的參考同步處理，並在 Dynamics 365 環境中同步處理：</span><span class="sxs-lookup"><span data-stu-id="f9e53-310">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="f9e53-311">登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="f9e53-311">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="f9e53-312">從左側功能表中選取 [ **參考** ]。</span><span class="sxs-lookup"><span data-stu-id="f9e53-312">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="f9e53-313">選取 [  **新增交易** ] 選項，從合作夥伴中心建立新的共同銷售推薦。</span><span class="sxs-lookup"><span data-stu-id="f9e53-313">Create a new Co-sell referral from Partner Center by selecting the  **New deal** option.</span></span>

   4. <span data-ttu-id="f9e53-314">登入您的 Dynamics 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="f9e53-314">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="f9e53-315">流覽至 **開啟的商機**。</span><span class="sxs-lookup"><span data-stu-id="f9e53-315">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="f9e53-316">在 Microsoft 合作夥伴中心內建立的參考現已在 Dynamics 365 CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="f9e53-316">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="f9e53-317">當您選取同步處理的參考時，就會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="f9e53-317">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f9e53-318">下一步</span><span class="sxs-lookup"><span data-stu-id="f9e53-318">Next steps</span></span>

- [<span data-ttu-id="f9e53-319">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="f9e53-319">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="f9e53-320">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="f9e53-320">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="f9e53-321">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="f9e53-321">More about Microsoft Power Automate platform?</span></span>](/power-automate/)

- [<span data-ttu-id="f9e53-322">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="f9e53-322">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
