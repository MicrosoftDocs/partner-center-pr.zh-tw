---
title: 使用 Webhook 取得資源變更事件
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Webhook Api 來瞭解何時發生參考的資源變更
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 參考，webhook api，資源變更事件
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796204"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="289ef-104">使用 Webhook Api 註冊資源變更事件</span><span class="sxs-lookup"><span data-stu-id="289ef-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="289ef-105">適當的角色</span><span class="sxs-lookup"><span data-stu-id="289ef-105">Appropriate roles</span></span>

- <span data-ttu-id="289ef-106">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="289ef-106">Referrals admin</span></span>
- <span data-ttu-id="289ef-107">Dynamics 365 CRM 或 Salesforce CRM 的系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="289ef-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="289ef-108">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="289ef-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="289ef-109">這些變更事件會當做 HTTP post 傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="289ef-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="289ef-110">本主題說明 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。</span><span class="sxs-lookup"><span data-stu-id="289ef-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="289ef-111">若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。</span><span class="sxs-lookup"><span data-stu-id="289ef-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="289ef-112">新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="289ef-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![觸發程序](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="289ef-114">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="289ef-114">When you make these updates, you will see</span></span>

![Webhook](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="289ef-116">儲存您的變更，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="289ef-117">若要讓合作夥伴中心 webhook 接聽合作夥伴中心和 CRM 系統中 IP 共同銷售/獨立參考物件的事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="289ef-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="289ef-118">選取 [**合作夥伴中心] 至 [Dynamics 365 （Insider preview）** ] 或 **[合作夥伴中心] 至 [Salesforce （insider preview）**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="289ef-119">選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="289ef-120">選取**複製**圖示以複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="289ef-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![複製 URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="289ef-122">現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="289ef-123">確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="289ef-124">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="289ef-124">Enter the following details:</span></span> 

    <span data-ttu-id="289ef-125">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-125">a.</span></span> <span data-ttu-id="289ef-126">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="289ef-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="289ef-127">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-127">b.</span></span> <span data-ttu-id="289ef-128">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="289ef-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="289ef-129">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-129">c.</span></span> <span data-ttu-id="289ef-130">**覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。</span><span class="sxs-lookup"><span data-stu-id="289ef-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="289ef-131">Webhook 現在可以接聽變更（建立和更新事件）。</span><span class="sxs-lookup"><span data-stu-id="289ef-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="289ef-132">選取 [**執行**]，然後選取 [**完成]。**</span><span class="sxs-lookup"><span data-stu-id="289ef-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="289ef-133">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="289ef-133">Customize synchronization steps</span></span>

<span data-ttu-id="289ef-134">在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。</span><span class="sxs-lookup"><span data-stu-id="289ef-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="289ef-135">通常 CRM 系統是高度自訂的。</span><span class="sxs-lookup"><span data-stu-id="289ef-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="289ef-136">您可以自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="289ef-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="289ef-137">遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="289ef-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="289ef-138">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="289ef-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="289ef-139">每個電源自動化流程的多個步驟可以根據您的需求自訂。</span><span class="sxs-lookup"><span data-stu-id="289ef-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="289ef-140">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="289ef-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="289ef-141">若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="289ef-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="289ef-142">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-142">a.</span></span> <span data-ttu-id="289ef-143">選取 [合作夥伴中心] 至 [Dynamics 365 （Insider Preview）] 或 [合作夥伴中心] 至 [Salesforce （Insider Preview）]。</span><span class="sxs-lookup"><span data-stu-id="289ef-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="289ef-144">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-144">b.</span></span> <span data-ttu-id="289ef-145">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="289ef-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="289ef-146">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-146">c.</span></span> <span data-ttu-id="289ef-147">選取 **[（範圍）]，同步處理潛在客戶或商機**。</span><span class="sxs-lookup"><span data-stu-id="289ef-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="289ef-148">若要自訂 [建立事件] 的 CRM 欄位對應（根據欄位對應指南），請選取 [**如果是新的共用機會]，然後**。</span><span class="sxs-lookup"><span data-stu-id="289ef-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="289ef-149">**如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="289ef-150">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="289ef-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="289ef-151">d.</span><span class="sxs-lookup"><span data-stu-id="289ef-151">d.</span></span> <span data-ttu-id="289ef-152">如需自訂 update 事件的 CRM 欄位對應（根據欄位對應指南），請按一下「同步處理潛在客戶或商機」的步驟 [（範圍）]。</span><span class="sxs-lookup"><span data-stu-id="289ef-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="289ef-153">e.</span><span class="sxs-lookup"><span data-stu-id="289ef-153">e.</span></span> <span data-ttu-id="289ef-154">**如果它是商機的更新，請選取此**方式。</span><span class="sxs-lookup"><span data-stu-id="289ef-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="289ef-155">**若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="289ef-156">f.</span><span class="sxs-lookup"><span data-stu-id="289ef-156">f.</span></span> <span data-ttu-id="289ef-157">選取 **[如果是]** ，然後按一下 [**更新現有商機**]</span><span class="sxs-lookup"><span data-stu-id="289ef-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="289ef-158">若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="289ef-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="289ef-159">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-159">a.</span></span> <span data-ttu-id="289ef-160">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="289ef-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="289ef-161">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-161">b.</span></span> <span data-ttu-id="289ef-162">選取 **[（範圍）] 以同步處理商機**。</span><span class="sxs-lookup"><span data-stu-id="289ef-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="289ef-163">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-163">c.</span></span> <span data-ttu-id="289ef-164">針對 [更新事件] 的自訂 CRM 欄位對應（根據欄位對應指南），選取 **[合作夥伴中心和 CRM 中的潛在客戶] 物件之間是否有差異，然後**。</span><span class="sxs-lookup"><span data-stu-id="289ef-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="289ef-165">d.</span><span class="sxs-lookup"><span data-stu-id="289ef-165">d.</span></span> <span data-ttu-id="289ef-166">選取 [子步驟 **] （如果是**），然後展開 [**以商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="289ef-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="289ef-167">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="289ef-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="289ef-168">若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="289ef-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="289ef-169">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-169">a.</span></span> <span data-ttu-id="289ef-170">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="289ef-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="289ef-171">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-171">b.</span></span> <span data-ttu-id="289ef-172">選取 **[同步處理參考] （範圍）。**</span><span class="sxs-lookup"><span data-stu-id="289ef-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="289ef-173">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-173">c.</span></span> <span data-ttu-id="289ef-174">如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="289ef-175">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="289ef-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="289ef-176">端對端雙向共同銷售參考同步處理</span><span class="sxs-lookup"><span data-stu-id="289ef-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="289ef-177">當您安裝、設定並自訂電源自動化解決方案之後，您可以測試 Dynamics 365 或 Salesforce 與合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="289ef-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="289ef-178">必要條件</span><span class="sxs-lookup"><span data-stu-id="289ef-178">Pre-requisites</span></span>

<span data-ttu-id="289ef-179">若要在合作夥伴中心與 Dynamics 365 CRM 之間或跨合作夥伴中心和 Salesforce CRM 之間同步處理這些參考，電源自動化解決方案必須明確地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="289ef-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="289ef-180">這讓您的賣方小組能夠決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="289ef-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="289ef-181">一組自訂欄位可作為 Dynamics 365 解決方案**商機**實體的合作夥伴中心參考同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="289ef-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="289ef-182">CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。</span><span class="sxs-lookup"><span data-stu-id="289ef-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="289ef-183">下列自訂欄位應為 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="289ef-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="289ef-184">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="289ef-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="289ef-185">**參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="289ef-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="289ef-186">**參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="289ef-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="289ef-187">**Microsoft help？**： microsoft 針對此參考所需的協助</span><span class="sxs-lookup"><span data-stu-id="289ef-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="289ef-188">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="289ef-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="289ef-189">**Audit**：與合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="289ef-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="289ef-190">場景</span><span class="sxs-lookup"><span data-stu-id="289ef-190">SCENARIOS:</span></span>

1. <span data-ttu-id="289ef-191">在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="289ef-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="289ef-192">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-192">a.</span></span> <span data-ttu-id="289ef-193">以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 DYNAMICS 365 CRM 環境或 Salesforce CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="289ef-193">Sign into your Dynamics 365 CRM environment or Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="289ef-194">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-194">b.</span></span> <span data-ttu-id="289ef-195">當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="289ef-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![商機](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="289ef-197">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-197">c.</span></span> <span data-ttu-id="289ef-198">若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="289ef-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="289ef-199">「與合作夥伴中心同步」：是</span><span class="sxs-lookup"><span data-stu-id="289ef-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="289ef-200">「Microsoft 如何協助？」：選取下列專案：</span><span class="sxs-lookup"><span data-stu-id="289ef-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![協助選取](images/cosellconnectors/help.png)

    - <span data-ttu-id="289ef-202">產品：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="289ef-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="289ef-203">d.</span><span class="sxs-lookup"><span data-stu-id="289ef-203">d.</span></span> <span data-ttu-id="289ef-204">一旦在 Dynamics 365 中建立商機，並將 [**同步與合作夥伴中心**] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="289ef-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="289ef-205">您的參考會與 Dynamics 365 進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="289ef-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="289ef-206">e.</span><span class="sxs-lookup"><span data-stu-id="289ef-206">e.</span></span> <span data-ttu-id="289ef-207">因此，如果您有機會將「與合作夥伴中心同步」選項設定為「是」，則當您在 Dynamics 365 CRM 中更新商機時，變更將會在您的合作夥伴中心帳戶中同步處理。</span><span class="sxs-lookup"><span data-stu-id="289ef-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="289ef-208">f.</span><span class="sxs-lookup"><span data-stu-id="289ef-208">f.</span></span> <span data-ttu-id="289ef-209">與合作夥伴中心成功同步處理的機會，將會使用 Dynamics 365 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="289ef-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="289ef-210">在 Microsoft 合作夥伴中心建立或更新參照時的參考同步處理，並在 Dynamics 365 環境中進行同步處理：</span><span class="sxs-lookup"><span data-stu-id="289ef-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="289ef-211">a.</span><span class="sxs-lookup"><span data-stu-id="289ef-211">a.</span></span> <span data-ttu-id="289ef-212">登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="289ef-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="289ef-213">b.</span><span class="sxs-lookup"><span data-stu-id="289ef-213">b.</span></span> <span data-ttu-id="289ef-214">從左側功能表中選取 [**參考**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="289ef-215">c.</span><span class="sxs-lookup"><span data-stu-id="289ef-215">c.</span></span> <span data-ttu-id="289ef-216">按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="289ef-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="289ef-217">d.</span><span class="sxs-lookup"><span data-stu-id="289ef-217">d.</span></span> <span data-ttu-id="289ef-218">登入您的 Dynamics 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="289ef-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="289ef-219">e.</span><span class="sxs-lookup"><span data-stu-id="289ef-219">e.</span></span> <span data-ttu-id="289ef-220">流覽至 [**開啟商機**]。</span><span class="sxs-lookup"><span data-stu-id="289ef-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="289ef-221">在 Microsoft 合作夥伴中心建立的參考現在已在 Dynamics 365 CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="289ef-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="289ef-222">f.</span><span class="sxs-lookup"><span data-stu-id="289ef-222">f.</span></span> <span data-ttu-id="289ef-223">當您選取同步處理的參考時，會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="289ef-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="289ef-224">後續步驟</span><span class="sxs-lookup"><span data-stu-id="289ef-224">Next steps</span></span>

- [<span data-ttu-id="289ef-225">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="289ef-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="289ef-226">合作夥伴中心 webhook 事件</span><span class="sxs-lookup"><span data-stu-id="289ef-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="289ef-227">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="289ef-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="289ef-228">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="289ef-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
