---
title: 使用 Webhook 取得資源變更事件
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作夥伴中心 Webhook Api 來瞭解 Dynamics 365 CRM 或 Salesforce CRM 何時會發生參考的資源變更。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: 參考，webhook api，資源變更事件
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89628fd6ccab6a943d8bd816afa7b5d3b0f241f7
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749175"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a><span data-ttu-id="3b6aa-104">使用 Webhook Api 來註冊 Dynamics 365 CRM 和 Salesforce CRM 的資源變更事件</span><span class="sxs-lookup"><span data-stu-id="3b6aa-104">Use Webhook APIs to register for resource change events for Dynamics 365 CRM and Salesforce CRM</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="3b6aa-105">適當的角色</span><span class="sxs-lookup"><span data-stu-id="3b6aa-105">Appropriate roles</span></span>

- <span data-ttu-id="3b6aa-106">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="3b6aa-106">Referrals admin</span></span>
- <span data-ttu-id="3b6aa-107">Dynamics 365 CRM 或 Salesforce CRM 的系統管理員或系統自訂者</span><span class="sxs-lookup"><span data-stu-id="3b6aa-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>

<span data-ttu-id="3b6aa-108">合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="3b6aa-109">這些變更事件會當做 HTTP post 傳送至您的 url。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="3b6aa-110">本主題說明 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

## <a name="configure-the-webhook"></a><span data-ttu-id="3b6aa-111">設定 Webhook</span><span class="sxs-lookup"><span data-stu-id="3b6aa-111">Configure the webhook</span></span>

1. <span data-ttu-id="3b6aa-112">若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-112">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="3b6aa-113">新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件</span><span class="sxs-lookup"><span data-stu-id="3b6aa-113">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. <span data-ttu-id="3b6aa-115">當您進行這些更新時，您會看到</span><span class="sxs-lookup"><span data-stu-id="3b6aa-115">When you make these updates, you will see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. <span data-ttu-id="3b6aa-117">儲存您的變更，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-117">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="3b6aa-118">若要讓合作夥伴中心 webhook 接聽合作夥伴中心和 CRM 系統中 IP 共同銷售/獨立參考物件的事件變更，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-118">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="3b6aa-119">選取 [**合作夥伴中心] 至 [Dynamics 365 （Insider preview）** ] 或 **[合作夥伴中心] 至 [Salesforce （insider preview）**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-119">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="3b6aa-120">選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-120">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="3b6aa-121">選取**複製**圖示以複製提供的 HTTP POST URL。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-121">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="複製 URL":::

8. <span data-ttu-id="3b6aa-123">現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-123">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="3b6aa-124">確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-124">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="3b6aa-125">輸入下列詳細資料：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-125">Enter the following details:</span></span>

    1. <span data-ttu-id="3b6aa-126">**Http 觸發程式端點**：從先前步驟複製的 URL</span><span class="sxs-lookup"><span data-stu-id="3b6aa-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="3b6aa-127">**要註冊的事件**：「參考建立」和「參考更新」</span><span class="sxs-lookup"><span data-stu-id="3b6aa-127">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="3b6aa-128">**覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-128">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

    <span data-ttu-id="3b6aa-129">Webhook 現在可以接聽變更（建立和更新事件）。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-129">The webhook can now listen to changes (create and update events).</span></span>

11. <span data-ttu-id="3b6aa-130">選取 [**執行**]，然後選取 [**完成]。**</span><span class="sxs-lookup"><span data-stu-id="3b6aa-130">Select **Run** and then select **Done.**</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="3b6aa-131">自訂同步處理步驟</span><span class="sxs-lookup"><span data-stu-id="3b6aa-131">Customize synchronization steps</span></span>

<span data-ttu-id="3b6aa-132">在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-132">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="3b6aa-133">通常 CRM 系統是高度自訂的。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-133">Often CRM systems are highly customized.</span></span> <span data-ttu-id="3b6aa-134">您可以自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-134">You can customize the Power Automate flows.</span></span> <span data-ttu-id="3b6aa-135">遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-135">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="3b6aa-136">系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-136">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="3b6aa-137">每個電源自動化流程的多個步驟可以根據您的需求自訂。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-137">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="3b6aa-138">以下是可用自訂的範例：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-138">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="3b6aa-139">若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-139">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="3b6aa-140">選取 [合作夥伴中心] 至 [Dynamics 365 （Insider Preview）] 或 [合作夥伴中心] 至 [Salesforce （Insider Preview）]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-140">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

   2. <span data-ttu-id="3b6aa-141">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-141">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="3b6aa-142">選取 **[（範圍）]，同步處理潛在客戶或商機**。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-142">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="3b6aa-143">若要自訂 [建立事件] 的 CRM 欄位對應（根據欄位對應指南），請選取 [**如果是新的共用機會]，然後**。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-143">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="3b6aa-144">**如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-144">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="3b6aa-145">您可以使用欄位對應指南來編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-145">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="3b6aa-146">如需自訂 update 事件的 CRM 欄位對應（根據欄位對應指南），請按一下「同步處理潛在客戶或商機」的步驟 [（範圍）]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-146">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

   2. <span data-ttu-id="3b6aa-147">**如果它是商機的更新，請選取此**方式。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-147">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="3b6aa-148">**若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-148">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="3b6aa-149">選取 **[如果是]** ，然後按一下 [**更新現有商機**]</span><span class="sxs-lookup"><span data-stu-id="3b6aa-149">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="3b6aa-150">若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-150">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="3b6aa-151">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-151">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="3b6aa-152">選取 **[（範圍）] 以同步處理商機**。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-152">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="3b6aa-153">針對 [更新事件] 的自訂 CRM 欄位對應（根據欄位對應指南），選取 **[合作夥伴中心和 CRM 中的潛在客戶] 物件之間是否有差異，然後**。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-153">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="3b6aa-154">選取 [子步驟 **] （如果是**），然後展開 [**以商機資料更新參考**] 步驟。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-154">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="3b6aa-155">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-155">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="3b6aa-156">若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？</span><span class="sxs-lookup"><span data-stu-id="3b6aa-156">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="3b6aa-157">選取 [**編輯**] 以編輯/自訂電源自動化流程。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-157">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="3b6aa-158">選取 **[同步處理參考] （範圍）。**</span><span class="sxs-lookup"><span data-stu-id="3b6aa-158">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="3b6aa-159">如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-159">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="3b6aa-160">您可以根據欄位對應指南，編輯本節中的對應。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-160">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="3b6aa-161">端對端雙向共同銷售參考同步處理</span><span class="sxs-lookup"><span data-stu-id="3b6aa-161">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="3b6aa-162">當您安裝、設定並自訂電源自動化解決方案之後，您可以測試 Dynamics 365 或 Salesforce 與合作夥伴中心之間的共同銷售參照同步處理。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-162">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="3b6aa-163">必要條件</span><span class="sxs-lookup"><span data-stu-id="3b6aa-163">Pre-requisites</span></span>

<span data-ttu-id="3b6aa-164">若要在合作夥伴中心與 Dynamics 365 CRM 之間或跨合作夥伴中心和 Salesforce CRM 之間同步處理這些參考，電源自動化解決方案必須明確地區分 Microsoft 特定的參考欄位。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-164">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="3b6aa-165">這讓您的賣方小組能夠決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-165">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="3b6aa-166">一組自訂欄位可作為 Dynamics 365 解決方案**商機**實體的合作夥伴中心參考同步處理的一部分。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-166">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="3b6aa-167">CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-167">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="3b6aa-168">下列自訂欄位應為 CRM 區段的一部分：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-168">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="3b6aa-169">**與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機</span><span class="sxs-lookup"><span data-stu-id="3b6aa-169">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="3b6aa-170">**參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位</span><span class="sxs-lookup"><span data-stu-id="3b6aa-170">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="3b6aa-171">**參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結</span><span class="sxs-lookup"><span data-stu-id="3b6aa-171">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="3b6aa-172">**Microsoft help？**： microsoft 針對此參考所需的協助</span><span class="sxs-lookup"><span data-stu-id="3b6aa-172">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="3b6aa-173">**產品**：與此商機相關聯的產品清單</span><span class="sxs-lookup"><span data-stu-id="3b6aa-173">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="3b6aa-174">**Audit**：與合作夥伴中心參考同步的唯讀審核記錄</span><span class="sxs-lookup"><span data-stu-id="3b6aa-174">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="3b6aa-175">場景</span><span class="sxs-lookup"><span data-stu-id="3b6aa-175">SCENARIOS:</span></span>

1. <span data-ttu-id="3b6aa-176">在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-176">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="3b6aa-177">以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 DYNAMICS 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-177">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="3b6aa-178">當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在</span><span class="sxs-lookup"><span data-stu-id="3b6aa-178">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="商機":::

   3. <span data-ttu-id="3b6aa-180">若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-180">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="3b6aa-181">**與合作夥伴中心同步**：是</span><span class="sxs-lookup"><span data-stu-id="3b6aa-181">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="3b6aa-182">**Microsoft help？**：請從下列專案中選取：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-182">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="協助選取":::

      - <span data-ttu-id="3b6aa-184">**產品**：產品的解決方案識別碼</span><span class="sxs-lookup"><span data-stu-id="3b6aa-184">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="3b6aa-185">一旦在 Dynamics 365 中建立商機，並將 [**同步與合作夥伴中心**] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-185">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="3b6aa-186">您的參考會與 Dynamics 365 進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-186">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="3b6aa-187">因此，如果您有機會將「與合作夥伴中心同步」選項設定為「是」，則當您在 Dynamics 365 CRM 中更新商機時，變更將會在您的合作夥伴中心帳戶中同步處理。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-187">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="3b6aa-188">與合作夥伴中心成功同步處理的機會，將會使用 Dynamics 365 中的✔圖示來識別。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-188">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="3b6aa-189">在 Microsoft 合作夥伴中心建立或更新參照時的參考同步處理，並在 Dynamics 365 環境中進行同步處理：</span><span class="sxs-lookup"><span data-stu-id="3b6aa-189">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="3b6aa-190">登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-190">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="3b6aa-191">從左側功能表中選取 [**參考**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-191">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="3b6aa-192">按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-192">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="3b6aa-193">登入您的 Dynamics 365 CRM 環境。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-193">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="3b6aa-194">流覽至 [**開啟商機**]。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-194">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="3b6aa-195">在 Microsoft 合作夥伴中心建立的參考現在已在 Dynamics 365 CRM 中同步處理。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-195">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="3b6aa-196">當您選取同步處理的參考時，會填入卡片視圖詳細資料。</span><span class="sxs-lookup"><span data-stu-id="3b6aa-196">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3b6aa-197">後續步驟</span><span class="sxs-lookup"><span data-stu-id="3b6aa-197">Next steps</span></span>

- [<span data-ttu-id="3b6aa-198">深入瞭解 Microsoft Power 自動化平臺？</span><span class="sxs-lookup"><span data-stu-id="3b6aa-198">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="3b6aa-199">合作夥伴中心 webhook 事件</span><span class="sxs-lookup"><span data-stu-id="3b6aa-199">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="3b6aa-200">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="3b6aa-200">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="3b6aa-201">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="3b6aa-201">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
