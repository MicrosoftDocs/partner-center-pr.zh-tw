---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 將合作夥伴中心中的參考與 Salesforce CRM 同步處理
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4bc404ca8c0647b1bcece767da75fa07ddc6b51f
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663859"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="68f3c-103">Salesforce CRM 的共同銷售連接器 – 概觀</span><span class="sxs-lookup"><span data-stu-id="68f3c-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="68f3c-104">適當的角色</span><span class="sxs-lookup"><span data-stu-id="68f3c-104">Appropriate roles</span></span>

- <span data-ttu-id="68f3c-105">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="68f3c-105">Referrals admin</span></span>
- <span data-ttu-id="68f3c-106">CRM 上的系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="68f3c-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="68f3c-107">合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。</span><span class="sxs-lookup"><span data-stu-id="68f3c-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="68f3c-108">他們不需要訓練以使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="68f3c-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="68f3c-109">您可以使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。</span><span class="sxs-lookup"><span data-stu-id="68f3c-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="68f3c-110">您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。</span><span class="sxs-lookup"><span data-stu-id="68f3c-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="68f3c-111">在您選擇的 CRM 中工作時，您可以執行所有的參考工作，而不是在合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="68f3c-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="68f3c-112">解決方案是以 Microsoft Power Automate 解決方案為基礎，並使用合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="68f3c-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="68f3c-113">安裝之前的先決條件</span><span class="sxs-lookup"><span data-stu-id="68f3c-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="68f3c-114">**主題**</span><span class="sxs-lookup"><span data-stu-id="68f3c-114">**Topics**</span></span>   |<span data-ttu-id="68f3c-115">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="68f3c-115">**Details**</span></span>   |<span data-ttu-id="68f3c-116">**連結**</span><span class="sxs-lookup"><span data-stu-id="68f3c-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="68f3c-117">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="68f3c-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="68f3c-118">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="68f3c-118">You need a valid MPN ID</span></span>|<span data-ttu-id="68f3c-119">加入 [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="68f3c-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="68f3c-120">共同銷售準備就緒</span><span class="sxs-lookup"><span data-stu-id="68f3c-120">Co-sell ready</span></span>|<span data-ttu-id="68f3c-121">您的 IP/服務解決方案必須已準備好共同銷售。</span><span class="sxs-lookup"><span data-stu-id="68f3c-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="68f3c-122">與 Microsoft 銷售</span><span class="sxs-lookup"><span data-stu-id="68f3c-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="68f3c-123">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="68f3c-123">Partner Center account</span></span>|<span data-ttu-id="68f3c-124">與合作夥伴中心租使用者相關聯的 MPN 識別碼必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="68f3c-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="68f3c-125">先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。</span><span class="sxs-lookup"><span data-stu-id="68f3c-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="68f3c-126">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="68f3c-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="68f3c-127">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="68f3c-127">Partner Center user roles</span></span>|<span data-ttu-id="68f3c-128">將安裝並使用連接器的員工必須是推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="68f3c-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="68f3c-129">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="68f3c-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="68f3c-130">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="68f3c-130">Salesforce CRM</span></span>|<span data-ttu-id="68f3c-131">CRM 使用者角色是系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="68f3c-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="68f3c-132">在 Salesforce CRM 中指派角色</span><span class="sxs-lookup"><span data-stu-id="68f3c-132">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="68f3c-133">Power Automate Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="68f3c-133">Power Automate Flow Account</span></span>|<span data-ttu-id="68f3c-134">適用于 CRM 系統管理員或系統自訂員的 active [Power Automate](https://flow.microsoft.com) 帳戶。</span><span class="sxs-lookup"><span data-stu-id="68f3c-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="68f3c-135">在安裝之前，該使用者至少應登入 [Power Automate](https://flow.microsoft.com) 一次。</span><span class="sxs-lookup"><span data-stu-id="68f3c-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="68f3c-136">安裝適用于 Microsoft 自訂欄位的 Salesforce 套件</span><span class="sxs-lookup"><span data-stu-id="68f3c-136">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="68f3c-137">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，Power Automate 解決方案必須清楚地識別 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="68f3c-137">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="68f3c-138">此分界可讓合作夥伴賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="68f3c-138">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="68f3c-139">在 Salesforce 中，啟用 [ **附注** ]，並將它新增至商機相關清單。</span><span class="sxs-lookup"><span data-stu-id="68f3c-139">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="68f3c-140">參考</span><span class="sxs-lookup"><span data-stu-id="68f3c-140">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="68f3c-141">遵循下列步驟來啟動 **商機小組** ：</span><span class="sxs-lookup"><span data-stu-id="68f3c-141">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="68f3c-142">在安裝程式中，使用 [ **快速尋找** ] 方塊找出商機團隊設定。</span><span class="sxs-lookup"><span data-stu-id="68f3c-142">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="68f3c-143">視需要定義設定。</span><span class="sxs-lookup"><span data-stu-id="68f3c-143">Define the settings as needed.</span></span>
[<span data-ttu-id="68f3c-144">參考</span><span class="sxs-lookup"><span data-stu-id="68f3c-144">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="68f3c-145">在 Salesforce 中，請使用以下的套件安裝程式來安裝自訂欄位和物件。</span><span class="sxs-lookup"><span data-stu-id="68f3c-145">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="68f3c-146">請前往 [這裡](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) 將套件安裝到任何公司：</span><span class="sxs-lookup"><span data-stu-id="68f3c-146">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="68f3c-147">注意：如果您要安裝至沙箱，您必須將 URL 的初始部分取代為 http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="68f3c-147">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="68f3c-148">在 Salesforce 中，將 Microsoft 解決方案新增至 **商機** 相關清單。</span><span class="sxs-lookup"><span data-stu-id="68f3c-148">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="68f3c-149">新增之後，請按一下 [ **扳手** ] 圖示，然後更新屬性</span><span class="sxs-lookup"><span data-stu-id="68f3c-149">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="68f3c-150">最佳做法：上線之前先進行測試</span><span class="sxs-lookup"><span data-stu-id="68f3c-150">Best Practice: Test before you go live</span></span>

<span data-ttu-id="68f3c-151">在生產環境中安裝、設定和自訂 Power Automate 解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="68f3c-151">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="68f3c-152">在預備環境/CRM 實例上安裝 Microsoft Power Automate 的解決方案。</span><span class="sxs-lookup"><span data-stu-id="68f3c-152">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="68f3c-153">製作解決方案的複本，並在預備環境中執行設定和 Power Automate 流程自訂。</span><span class="sxs-lookup"><span data-stu-id="68f3c-153">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="68f3c-154">測試預備/CRM 實例上的方案。</span><span class="sxs-lookup"><span data-stu-id="68f3c-154">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="68f3c-155">成功時，請將匯入為生產實例的受控解決方案。</span><span class="sxs-lookup"><span data-stu-id="68f3c-155">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="68f3c-156">安裝 Salesforce CRM 合作夥伴中心推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="68f3c-156">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="68f3c-157">移至 [Power Automate](https://flow.microsoft.com) ，然後在右上角選取 [ **環境** ]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-157">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="68f3c-158">這會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="68f3c-158">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="68f3c-159">從右上角的下拉式清單中選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="68f3c-159">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="68f3c-160">選取左側導覽列上的 [ **方案** ]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-160">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="68f3c-161">按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="68f3c-161">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. <span data-ttu-id="68f3c-163">在快顯視窗中搜尋 **Salesforce 的合作夥伴中心推薦連接器** 。</span><span class="sxs-lookup"><span data-stu-id="68f3c-163">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="開啟 AppSource":::

6. <span data-ttu-id="68f3c-165">按一下 [ **立即取得** ] 按鈕，然後 **繼續**進行。</span><span class="sxs-lookup"><span data-stu-id="68f3c-165">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="68f3c-166">這會開啟頁面，您可以在其中選取要安裝應用程式的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="68f3c-166">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="68f3c-167">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="68f3c-167">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="開啟 AppSource":::

8. <span data-ttu-id="68f3c-169">然後，系統會將您導向至 [ **管理您的解決方案** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="68f3c-169">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="68f3c-170">使用頁面底部的箭號按鈕，流覽至「合作夥伴中心的推薦」。</span><span class="sxs-lookup"><span data-stu-id="68f3c-170">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="68f3c-171">已**排程的安裝**應該會出現在合作夥伴中心的推薦解決方案旁邊。</span><span class="sxs-lookup"><span data-stu-id="68f3c-171">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="68f3c-172">安裝將需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="68f3c-172">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="68f3c-173">安裝完成之後，請流覽回到 [Power Automate](https://flow.microsoft.com) ，然後從左側導覽區域選取 **解決方案** 。</span><span class="sxs-lookup"><span data-stu-id="68f3c-173">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="68f3c-174">請注意，[方案] 清單中有提供 **Salesforce 的合作夥伴中心推薦同步** 處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-174">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="68f3c-175">選取 **Salesforce 的合作夥伴中心推薦同步**處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-175">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="68f3c-176">以下是可用的流程和實體 Power Automate：</span><span class="sxs-lookup"><span data-stu-id="68f3c-176">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="開啟 AppSource":::



## <a name="configure-the-solution"></a><span data-ttu-id="68f3c-178">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="68f3c-178">Configure the solution</span></span>

1. <span data-ttu-id="68f3c-179">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power Automate](https://flow.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="68f3c-179">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="68f3c-180">從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power Automate 解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="68f3c-180">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="68f3c-181">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="68f3c-181">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="68f3c-182">具有推薦系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="68f3c-182">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="68f3c-183">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="68f3c-183">Partner Center Events</span></span>
    - <span data-ttu-id="68f3c-184">CRM 管理員與解決方案中的 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="68f3c-184">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="68f3c-185">從左側導覽列選取 [ **連接** ]，然後從清單中選取 [合作夥伴中心的參考] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="68f3c-185">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="68f3c-186">按一下 [ **建立連接**] 來建立連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-186">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="開啟 AppSource":::

- <span data-ttu-id="68f3c-188">在右上角的搜尋列中搜尋合作夥伴中心參考 (預覽) 。</span><span class="sxs-lookup"><span data-stu-id="68f3c-188">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="68f3c-189">使用「參考系統管理員」的認證角色建立合作夥伴中心使用者的連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-189">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="68f3c-190">接下來，使用推薦的系統管理員認證來為您的合作夥伴中心使用者建立合作夥伴中心事件連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-190">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="68f3c-191">為 CRM 系統管理員使用者建立 Common Data Service (目前環境) 的連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-191">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

-  <span data-ttu-id="68f3c-192">新增所有連線之後，您應該會在您的環境中看到下列連接：</span><span class="sxs-lookup"><span data-stu-id="68f3c-192">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="開啟 AppSource":::

### <a name="edit-the-connections"></a><span data-ttu-id="68f3c-194">編輯連接</span><span class="sxs-lookup"><span data-stu-id="68f3c-194">Edit the connections</span></span>

1. <span data-ttu-id="68f3c-195">返回 [方案] 頁面，然後選取 [ **預設方案**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-195">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="68f3c-196">按一下 [**全部**]，以選取 [ \*\* (預覽) 的連接參考\*\*。</span><span class="sxs-lookup"><span data-stu-id="68f3c-196">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="開啟 AppSource":::

2. <span data-ttu-id="68f3c-198">選取三個點圖示，逐一編輯每一個連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-198">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="68f3c-199">新增相關的連接。</span><span class="sxs-lookup"><span data-stu-id="68f3c-199">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="開啟 AppSource":::

3. <span data-ttu-id="68f3c-201">依下列順序開啟流程：</span><span class="sxs-lookup"><span data-stu-id="68f3c-201">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="68f3c-202">合作夥伴中心 Webhook 註冊 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="68f3c-202">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-203">建立共同銷售參考-Salesforce 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="68f3c-203">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-204">合作夥伴中心 Microsoft 共同銷售參考更新至 Salesforce (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="68f3c-204">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-205">合作夥伴中心至 Salesforce (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="68f3c-205">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-206">Salesforce 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="68f3c-206">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-207">合作夥伴中心 (Insider Preview) 的 Salesforce 機會</span><span class="sxs-lookup"><span data-stu-id="68f3c-207">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="68f3c-208">合作夥伴中心 (Insider Preview) 的 Salesforce Microsoft 解決方案</span><span class="sxs-lookup"><span data-stu-id="68f3c-208">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="68f3c-209">使用 Webhook Api 來註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="68f3c-209">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="68f3c-210">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="68f3c-210">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="68f3c-211">這些變更事件會以 HTTP 文章的形式傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="68f3c-211">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="68f3c-212">若要註冊您的 url，請選取 \*\*合作夥伴中心 Webhook 註冊 (Insider preview) \*\* Power Automate flow。</span><span class="sxs-lookup"><span data-stu-id="68f3c-212">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="68f3c-213">新增 (的連接。 ) 合作夥伴中心具有推薦的系統管理員認證的使用者 (b. ) 合作夥伴中心事件，如下所強調</span><span class="sxs-lookup"><span data-stu-id="68f3c-213">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="開啟 AppSource":::

3. <span data-ttu-id="68f3c-215">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="68f3c-215">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="開啟 AppSource":::

4. <span data-ttu-id="68f3c-217">儲存您的變更，然後選取 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-217">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="68f3c-218">若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="68f3c-218">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="68f3c-219">選取 \*\*合作夥伴中心至 SALESFORCE CRM (Insider preview) \*\*。</span><span class="sxs-lookup"><span data-stu-id="68f3c-219">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="68f3c-220">選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-220">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="68f3c-221">選取 **複製** 圖示來複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="68f3c-221">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="開啟 AppSource":::

8. <span data-ttu-id="68f3c-223">現在，選取 [合作夥伴中心 Webhook 註冊 (Insider Preview) ] Power Automate 流程，然後選取 [ **執行**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-223">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="68f3c-224">確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-224">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="68f3c-225">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="68f3c-225">Enter the following details:</span></span>

    1. <span data-ttu-id="68f3c-226">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="68f3c-226">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="68f3c-227">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="68f3c-227">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="68f3c-228">**覆寫現有的觸發程式端點（如果有的話**）：是 (這會覆寫任何現有的端點。 ) </span><span class="sxs-lookup"><span data-stu-id="68f3c-228">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="68f3c-229">選取 [ **執行** ]，然後選取 [ **完成]。**</span><span class="sxs-lookup"><span data-stu-id="68f3c-229">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="68f3c-230">Webhook 現在可以接聽建立和更新事件。</span><span class="sxs-lookup"><span data-stu-id="68f3c-230">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="68f3c-231">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="68f3c-231">Customize synchronization steps</span></span>

<span data-ttu-id="68f3c-232">當共同銷售的參考在合作夥伴中心與您的 CRM 系統之間進行同步處理時，在合作夥伴中心電腦上同步的欄位會列在此處。</span><span class="sxs-lookup"><span data-stu-id="68f3c-232">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="68f3c-233">通常會高度自訂 CRM 系統。</span><span class="sxs-lookup"><span data-stu-id="68f3c-233">Often CRM systems are highly customized.</span></span> <span data-ttu-id="68f3c-234">您可以自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="68f3c-234">You can customize the Power Automate flows.</span></span> <span data-ttu-id="68f3c-235">依照欄位對應指南操作，如有必要，請在 Power Automate 流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="68f3c-235">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="68f3c-236">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="68f3c-236">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="68f3c-237">您可以根據自己的需求自訂每個 Power Automate 流程的多個步驟。</span><span class="sxs-lookup"><span data-stu-id="68f3c-237">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="68f3c-238">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="68f3c-238">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="68f3c-239">若要自訂合作夥伴中心中的建立或更新事件的欄位以進行 CRM 推薦同步處理：</span><span class="sxs-lookup"><span data-stu-id="68f3c-239">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="68f3c-240">選取合作夥伴中心至 Salesforce CRM (Insider preview) 。</span><span class="sxs-lookup"><span data-stu-id="68f3c-240">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="68f3c-241">選取 [ **編輯** ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="68f3c-241">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="68f3c-242">選取 \*\* (範圍) 同步處理潛在客戶或商機\*\*。</span><span class="sxs-lookup"><span data-stu-id="68f3c-242">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="68f3c-243">若要自訂建立事件的 CRM 欄位對應，請選取 **它是否為新的共用商機，然後**。</span><span class="sxs-lookup"><span data-stu-id="68f3c-243">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="68f3c-244">若為 [ **是]** ，請選取子步驟，然後 **在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-244">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="68f3c-245">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="68f3c-245">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="68f3c-246">若要自訂更新事件的 CRM 欄位對應，請按一下「 (範圍) 同步處理潛在客戶或商機」步驟。</span><span class="sxs-lookup"><span data-stu-id="68f3c-246">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="68f3c-247">**如果這是商機的更新，請選取它**。</span><span class="sxs-lookup"><span data-stu-id="68f3c-247">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="68f3c-248">**如果 [是]** ，請選取 [子步驟]，然後展開 [**合作夥伴中心和 CRM 中商機物件之間的差異]，然後再**展開。</span><span class="sxs-lookup"><span data-stu-id="68f3c-248">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="68f3c-249">選取 **[是]** ，然後選取 [**更新現有的商機**]</span><span class="sxs-lookup"><span data-stu-id="68f3c-249">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="68f3c-250">若要自訂更新事件的 CRM 對電腦推薦同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="68f3c-250">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="68f3c-251">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="68f3c-251">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="68f3c-252">選取 \*\* (範圍) 同步處理商機\*\*。</span><span class="sxs-lookup"><span data-stu-id="68f3c-252">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="68f3c-253">若要根據欄位對應來自訂 CRM 欄位對應 () 針對 update 事件，請選取 **合作夥伴中心和 CRM 中的潛在客戶物件之間是否有差異**。</span><span class="sxs-lookup"><span data-stu-id="68f3c-253">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="68f3c-254">**若為 [是]** ，請選取子步驟，然後展開 [**使用商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="68f3c-254">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="68f3c-255">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="68f3c-255">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="68f3c-256">針對建立事件自訂 CRM 對電腦推薦同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="68f3c-256">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="68f3c-257">選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。</span><span class="sxs-lookup"><span data-stu-id="68f3c-257">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="68f3c-258">選取 \*\* (範圍) 同步處理參考。\*\*</span><span class="sxs-lookup"><span data-stu-id="68f3c-258">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="68f3c-259">若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 [ **建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-259">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="68f3c-260">您可以根據欄位對應指南編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="68f3c-260">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="68f3c-261">端對端雙向共同銷售推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="68f3c-261">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="68f3c-262">安裝、設定和自訂 Power Automate 解決方案之後，您可以測試 Salesforce CRM 和合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-262">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="68f3c-263">必要條件</span><span class="sxs-lookup"><span data-stu-id="68f3c-263">Pre-requisites</span></span>

<span data-ttu-id="68f3c-264">若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，Power Automate 解決方案必須清楚地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="68f3c-264">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="68f3c-265">此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="68f3c-265">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="68f3c-266">有一組自訂欄位可作為 Salesforce CRM 解決方案 **商機** 實體合作夥伴中心推薦同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="68f3c-266">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="68f3c-267">CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。</span><span class="sxs-lookup"><span data-stu-id="68f3c-267">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="68f3c-268">下列自訂欄位應該是 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="68f3c-268">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="68f3c-269">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="68f3c-269">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="68f3c-270">**參考識別碼**： Microsoft 合作夥伴中心推薦的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="68f3c-270">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="68f3c-271">**參考連結**： Microsoft 合作夥伴中心中參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="68f3c-271">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="68f3c-272">**Microsoft 如何協助**：推薦的 microsoft 所需的協助</span><span class="sxs-lookup"><span data-stu-id="68f3c-272">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="68f3c-273">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="68f3c-273">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="68f3c-274">**Audit**：使用合作夥伴中心參考進行同步處理的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="68f3c-274">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="68f3c-275">場景：</span><span class="sxs-lookup"><span data-stu-id="68f3c-275">SCENARIOS:</span></span>

1. <span data-ttu-id="68f3c-276">參考在 CRM 中建立或更新時的參考同步處理，並在合作夥伴中心中同步處理：</span><span class="sxs-lookup"><span data-stu-id="68f3c-276">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="68f3c-277">登入您的 Salesforce CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。</span><span class="sxs-lookup"><span data-stu-id="68f3c-277">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="68f3c-278">當您在 Salesforce CRM 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="68f3c-278">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="開啟 AppSource":::

   3. <span data-ttu-id="68f3c-280">若要與 Microsoft 合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="68f3c-280">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="68f3c-281">「同步處理合作夥伴中心」：是</span><span class="sxs-lookup"><span data-stu-id="68f3c-281">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="68f3c-282">「Microsoft 如何協助？」：從下列選項中選取：</span><span class="sxs-lookup"><span data-stu-id="68f3c-282">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="68f3c-283">產品：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="68f3c-283">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="68f3c-284">一旦您將 [商機  **同步與合作夥伴中心** ] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="68f3c-284">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="68f3c-285">您的參考會與 Salesforce CRM 同步處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-285">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="68f3c-286">當 [同步處理合作夥伴中心] 選項設定為 [是] 時，如果您更新 Salesforce CRM 中的機會，變更將會與您的合作夥伴中心帳戶進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-286">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="68f3c-287">與合作夥伴中心成功同步處理的機會，將會使用 Salesforce CRM 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="68f3c-287">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="68f3c-288">在 Microsoft 合作夥伴中心中建立或更新參考時的參考同步處理，並在 Salesforce CRM 環境中同步處理：</span><span class="sxs-lookup"><span data-stu-id="68f3c-288">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="68f3c-289">登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="68f3c-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="68f3c-290">從左側功能表中選取 [ **參考** ]。</span><span class="sxs-lookup"><span data-stu-id="68f3c-290">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="68f3c-291">按一下 [新增交易] 選項，從合作夥伴中心建立新的共同銷售推薦。</span><span class="sxs-lookup"><span data-stu-id="68f3c-291">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="68f3c-292">登入您的 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="68f3c-292">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="68f3c-293">流覽至 **開啟的商機**。</span><span class="sxs-lookup"><span data-stu-id="68f3c-293">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="68f3c-294">在 Microsoft 合作夥伴中心中建立的參照現在已在 Salesforce CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="68f3c-294">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="開啟 AppSource":::

    6. <span data-ttu-id="68f3c-296">當您選取同步處理的參考時，就會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="68f3c-296">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="68f3c-297">後續步驟</span><span class="sxs-lookup"><span data-stu-id="68f3c-297">Next steps</span></span>

- [<span data-ttu-id="68f3c-298">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="68f3c-298">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="68f3c-299">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="68f3c-299">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="68f3c-300">合作夥伴中心 Webhook</span><span class="sxs-lookup"><span data-stu-id="68f3c-300">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)