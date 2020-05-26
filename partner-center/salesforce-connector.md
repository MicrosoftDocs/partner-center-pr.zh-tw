---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Salesforce CRM 連接器，取得 Microsoft 的參考
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825695"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="4a2ca-103">Salesforce CRM 的共同銷售連接器-總覽</span><span class="sxs-lookup"><span data-stu-id="4a2ca-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="4a2ca-104">適當的角色</span><span class="sxs-lookup"><span data-stu-id="4a2ca-104">Appropriate roles</span></span>

- <span data-ttu-id="4a2ca-105">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="4a2ca-105">Referrals admin</span></span>
- <span data-ttu-id="4a2ca-106">CRM 上的系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="4a2ca-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="4a2ca-107">合作夥伴中心共同銷售連接器可讓您的銷售人員從您的 CRM 系統內與 Microsoft 共同合作。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="4a2ca-108">他們不需要經過訓練，就能使用合作夥伴中心來管理共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="4a2ca-109">使用共同銷售連接器，您將能夠建立新的共同銷售諮詢，以參與 Microsoft 賣方、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值、結束日期等），以及接收來自 Microsoft 賣方的任何更新，以進行這些共同銷售交易。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="4a2ca-110">您可以在您選擇的 CRM 中工作，而不是在合作夥伴中心內執行所有動作。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="4a2ca-111">解決方案是以 Microsoft 電源自動化解決方案為基礎，並使用 Microsoft 合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>


## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="4a2ca-112">安裝之前的必要條件</span><span class="sxs-lookup"><span data-stu-id="4a2ca-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="4a2ca-113">**主題**</span><span class="sxs-lookup"><span data-stu-id="4a2ca-113">**Topics**</span></span>   |<span data-ttu-id="4a2ca-114">**詳細資料**</span><span class="sxs-lookup"><span data-stu-id="4a2ca-114">**Details**</span></span>   |<span data-ttu-id="4a2ca-115">**連結**</span><span class="sxs-lookup"><span data-stu-id="4a2ca-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="4a2ca-116">Microsoft 合作夥伴網路識別碼</span><span class="sxs-lookup"><span data-stu-id="4a2ca-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="4a2ca-117">您需要有效的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="4a2ca-117">You need a valid MPN ID</span></span>|<span data-ttu-id="4a2ca-118">加入[MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="4a2ca-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="4a2ca-119">共同銷售準備就緒</span><span class="sxs-lookup"><span data-stu-id="4a2ca-119">Co-sell ready</span></span>|<span data-ttu-id="4a2ca-120">您的 IP/服務解決方案必須共同銷售。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="4a2ca-121">與 Microsoft 一起銷售</span><span class="sxs-lookup"><span data-stu-id="4a2ca-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="4a2ca-122">合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="4a2ca-122">Partner Center account</span></span>|<span data-ttu-id="4a2ca-123">與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您的共同銷售解決方案相關聯的 MPN 識別碼相同。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="4a2ca-124">在部署連接器之前，請確認您可以在合作夥伴中心入口網站中看到您的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="4a2ca-125">管理您的帳戶</span><span class="sxs-lookup"><span data-stu-id="4a2ca-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="4a2ca-126">合作夥伴中心使用者角色</span><span class="sxs-lookup"><span data-stu-id="4a2ca-126">Partner Center user roles</span></span>|<span data-ttu-id="4a2ca-127">將安裝和使用連接器的員工必須是推薦管理員</span><span class="sxs-lookup"><span data-stu-id="4a2ca-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="4a2ca-128">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="4a2ca-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="4a2ca-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="4a2ca-129">Salesforce CRM</span></span>|<span data-ttu-id="4a2ca-130">CRM 使用者角色是系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="4a2ca-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="4a2ca-131">指派 Dynamics 365 中的角色</span><span class="sxs-lookup"><span data-stu-id="4a2ca-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="4a2ca-132">Power 自動化 Flow 帳戶</span><span class="sxs-lookup"><span data-stu-id="4a2ca-132">Power Automate Flow Account</span></span>|<span data-ttu-id="4a2ca-133">適用于 CRM 系統管理員或系統自訂者的主動式[電源自動化](https://flow.microsoft.com)帳戶。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="4a2ca-134">該使用者應該在安裝之前至少登入一次[電源](https://flow.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="4a2ca-135">安裝 Salesforce CRM 的合作夥伴中心推薦同步處理</span><span class="sxs-lookup"><span data-stu-id="4a2ca-135">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="4a2ca-136">移至 [[電源自動化](https://flow.microsoft.com)]，並選取右上角的 [**環境**]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="4a2ca-137">這會顯示可用的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="4a2ca-138">從右上角的下拉式選單中，選取適當的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="4a2ca-139">選取左側導覽列上的 [**方案**]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="4a2ca-140">按一下上方功能表上的 [**開啟 AppSource** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-140">Click on the **Open AppSource** link on the top menu.</span></span>

![開啟 AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="4a2ca-142">在彈出畫面中搜尋**Salesforce 的合作夥伴中心參照連接器**。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-142">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

6. <span data-ttu-id="4a2ca-143">按一下 [**立即取得**] 按鈕，然後按 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="4a2ca-144">這會開啟頁面，您可以在其中選取要安裝應用程式的 CRM （Dynamics 365）環境。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="4a2ca-145">同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="4a2ca-146">接著，您會被導向至 [**管理您的解決方案**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="4a2ca-147">使用頁面底部的箭號按鈕，流覽至 [合作夥伴中心的參考]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="4a2ca-148">已**排程的安裝**應該會出現在合作夥伴中心的 [參考解決方案] 旁。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="4a2ca-149">安裝需要10-15 分鐘的時間。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="4a2ca-150">安裝完成後，流覽回到 [[電源自動化](https://flow.microsoft.com)]，然後從左側導覽區域選取 [**解決方案**]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="4a2ca-151">請注意，解決方案清單中提供**Salesforce 的合作夥伴中心參照同步**處理。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-151">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="4a2ca-152">選取**Dynamics 365 的合作夥伴中心參照同步**處理。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="4a2ca-153">下列電源可自動執行流程和實體：</span><span class="sxs-lookup"><span data-stu-id="4a2ca-153">The following Power Automate flows and entities are available:</span></span>

![可用的 CRM](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="4a2ca-155">最佳做法：在您上線之前進行測試</span><span class="sxs-lookup"><span data-stu-id="4a2ca-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="4a2ca-156">在您安裝、設定及自訂生產環境的電源自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="4a2ca-157">在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="4a2ca-158">建立解決方案的複本並執行設定，並在預備環境上自動化流程自訂。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="4a2ca-159">在預備/CRM 實例上測試解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="4a2ca-160">成功時，將匯入為生產實例的受控解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="4a2ca-161">設定解決方案</span><span class="sxs-lookup"><span data-stu-id="4a2ca-161">Configure the solution</span></span>

1. <span data-ttu-id="4a2ca-162">在您的 CRM 實例中安裝解決方案之後，請流覽回到 [[電源自動化](https://flow.microsoft.com/)]。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="4a2ca-163">從右上角的 [**環境**] 下拉式選，選取您已安裝電源自動化解決方案的 CRM 實例。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="4a2ca-164">您將需要建立與三個使用者帳戶建立關聯的連接：</span><span class="sxs-lookup"><span data-stu-id="4a2ca-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="4a2ca-165">具有參考系統管理員認證的合作夥伴中心使用者</span><span class="sxs-lookup"><span data-stu-id="4a2ca-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="4a2ca-166">合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="4a2ca-166">Partner Center Events</span></span>
- <span data-ttu-id="4a2ca-167">CRM 系統管理員，具備在解決方案中自動化流程的能力。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="4a2ca-168">a.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-168">a.</span></span> <span data-ttu-id="4a2ca-169">從左側導覽列選取 [連線]，**然後從清單**中選取 [合作夥伴中心參照] 解決方案。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="4a2ca-170">b.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-170">b.</span></span> <span data-ttu-id="4a2ca-171">按一下 [**建立連接**] 來建立連線。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![建立連線](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="4a2ca-173">c.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-173">c.</span></span> <span data-ttu-id="4a2ca-174">在右上角的搜尋列中搜尋**合作夥伴中心參照（預覽）** 。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="4a2ca-175">d.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-175">d.</span></span> <span data-ttu-id="4a2ca-176">使用 [參考管理員] 的認證角色建立合作夥伴中心使用者的連線。版.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="4a2ca-177">接下來，使用 [參考管理員] 的認證為合作夥伴中心使用者建立合作夥伴中心的事件連線。f.</span><span class="sxs-lookup"><span data-stu-id="4a2ca-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="4a2ca-178">為 CRM 系統管理員使用者建立 Common Data Service （目前的環境）的連接。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="4a2ca-179">若要讓電源自動化流程與連線產生關聯，請編輯每個電源自動化流程，以連線至 Common Data Service 和合作夥伴中心的參照。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="4a2ca-180">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-180">Save the changes.</span></span>

5. <span data-ttu-id="4a2ca-181">**開啟**電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="4a2ca-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4a2ca-182">後續步驟</span><span class="sxs-lookup"><span data-stu-id="4a2ca-182">Next steps</span></span>

- [<span data-ttu-id="4a2ca-183">使用 Webhook 取得資源變更事件</span><span class="sxs-lookup"><span data-stu-id="4a2ca-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="4a2ca-184">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="4a2ca-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="4a2ca-185">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="4a2ca-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="4a2ca-186">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="4a2ca-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
