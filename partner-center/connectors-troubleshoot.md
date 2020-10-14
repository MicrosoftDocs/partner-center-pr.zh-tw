---
title: 對共同銷售推薦連接器進行疑難排解
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解使用共同銷售連接器的常見問題解答。 閱讀此常見問題以瞭解如何針對共同銷售連接器進行疑難排解。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031261"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="56cdb-104">對共同銷售推薦連接器進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="56cdb-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="56cdb-105">**適用於：**</span><span class="sxs-lookup"><span data-stu-id="56cdb-105">**Applies to:**</span></span>

- <span data-ttu-id="56cdb-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="56cdb-106">Partner Center</span></span>
- <span data-ttu-id="56cdb-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="56cdb-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="56cdb-108">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="56cdb-108">Salesforce CRM</span></span>

<span data-ttu-id="56cdb-109">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="56cdb-109">**Appropriate roles**</span></span>

- <span data-ttu-id="56cdb-110">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="56cdb-110">Referrals admin</span></span>
- <span data-ttu-id="56cdb-111">CRM 上的系統管理員或系統自訂員</span><span class="sxs-lookup"><span data-stu-id="56cdb-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="56cdb-112">先決條件的相關問題和解答</span><span class="sxs-lookup"><span data-stu-id="56cdb-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="56cdb-113">您可以針對您的環境使用試用共同銷售推薦連接器解決方案嗎？</span><span class="sxs-lookup"><span data-stu-id="56cdb-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="56cdb-114">如果您是在測試/預備環境中，您可以選擇試用版解決方案。</span><span class="sxs-lookup"><span data-stu-id="56cdb-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="56cdb-115">付費版本的連接器可在 AppSource 中使用，每月 $ 15/月。</span><span class="sxs-lookup"><span data-stu-id="56cdb-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="56cdb-116">使用付費連線時，您每天會收到10K 的 API 呼叫。</span><span class="sxs-lookup"><span data-stu-id="56cdb-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="56cdb-117">連接器是合作夥伴中心參考 Api 之上的包裝函式。</span><span class="sxs-lookup"><span data-stu-id="56cdb-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="56cdb-118">每當連接器解決方案針對合作夥伴中心或 CRM 端的商機執行 **建立** 或 **更新** 事件時，就會進行 API 呼叫。</span><span class="sxs-lookup"><span data-stu-id="56cdb-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="56cdb-119">您需要在 CRM 環境中建立區段的角色為何？</span><span class="sxs-lookup"><span data-stu-id="56cdb-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="56cdb-120">身為系統管理員或系統自訂員的使用者，可以為所有人套用變更。</span><span class="sxs-lookup"><span data-stu-id="56cdb-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="56cdb-121">不過，所有的應用程式使用者都可以個人化系統，甚至與其他人共用部分自訂。</span><span class="sxs-lookup"><span data-stu-id="56cdb-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="56cdb-122">合作夥伴銷售人員是否需要特殊角色才能處理合作夥伴中心？</span><span class="sxs-lookup"><span data-stu-id="56cdb-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="56cdb-123">合作夥伴賣方必須獲派「推薦系統管理員」角色。</span><span class="sxs-lookup"><span data-stu-id="56cdb-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="56cdb-124">如需詳細資訊，請參閱下列 [許可權總覽) # B1 建立-使用者-帳戶-和設定許可權) 。</span><span class="sxs-lookup"><span data-stu-id="56cdb-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="56cdb-125">您需要在 CRM 環境中先設定哪些欄位？</span><span class="sxs-lookup"><span data-stu-id="56cdb-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="56cdb-126">•確定您的貨幣適用于您的位置，並且正確地放在您的 CRM 環境中。</span><span class="sxs-lookup"><span data-stu-id="56cdb-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="56cdb-127">•您的銷售小組應以 crm 使用者的形式列在您的 CRM 環境中。</span><span class="sxs-lookup"><span data-stu-id="56cdb-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="56cdb-128">Power Automate 環境建立需要哪些必要條件？</span><span class="sxs-lookup"><span data-stu-id="56cdb-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="56cdb-129">若要使用 Power Automate 環境，您需要：</span><span class="sxs-lookup"><span data-stu-id="56cdb-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="56cdb-130">需要 Power Automate 授權。</span><span class="sxs-lookup"><span data-stu-id="56cdb-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="56cdb-131">至少需要 1 GB 的儲存體。</span><span class="sxs-lookup"><span data-stu-id="56cdb-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="56cdb-132">您需要 Dynamics 365 訂用帳戶才能使用 Salesforce 連接器解決方案嗎？</span><span class="sxs-lookup"><span data-stu-id="56cdb-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="56cdb-133">Salesforce 連接器解決方案的類型為「Dynamics Flow」，可支援與其他 CRM 系統進行同步處理。</span><span class="sxs-lookup"><span data-stu-id="56cdb-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="56cdb-134">解決方案不需要您擁有 Dynamics 365 實例或訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="56cdb-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="56cdb-135">安裝 Salesforce 解決方案時，可能會出現您公司中現有 CD 環境的下拉式清單。</span><span class="sxs-lookup"><span data-stu-id="56cdb-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="56cdb-136">您必須選取該環境。</span><span class="sxs-lookup"><span data-stu-id="56cdb-136">You need to select that environment.</span></span> <span data-ttu-id="56cdb-137">此外，如果您收到錯誤「找不到連線至登入使用者的 Dynamics 365 組織」，則您將需要為連接器建立新的環境。</span><span class="sxs-lookup"><span data-stu-id="56cdb-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="56cdb-138">關於設定的問題和解答</span><span class="sxs-lookup"><span data-stu-id="56cdb-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="56cdb-139">如果您在 Power Automate 平臺中啟動流程時遇到下列錯誤，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="56cdb-140">錯誤： Azure Resource Manager 的要求失敗，錯誤為： ' {"error"： {"code"： "WorkflowTriggerNotFound"，"message"： "找不到工作流程 ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' 觸發程式 ' manual '。"}} '。</span><span class="sxs-lookup"><span data-stu-id="56cdb-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="56cdb-141">遵循下列疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="56cdb-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="56cdb-142">刪除 CD 連線，然後重新建立 CD 連線。</span><span class="sxs-lookup"><span data-stu-id="56cdb-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="56cdb-143">關閉和開啟子流程</span><span class="sxs-lookup"><span data-stu-id="56cdb-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="56cdb-144">刪除解決方案，然後重新安裝解決方案。</span><span class="sxs-lookup"><span data-stu-id="56cdb-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="56cdb-145">如果您在 Power Automate 平臺中新增合作夥伴中心連接器時遇到「登入」錯誤，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="要求登入的錯誤訊息":::

<span data-ttu-id="56cdb-147">遵循下列疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="56cdb-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="56cdb-148">使用合作夥伴中心認證登入流程環境， (flow.microsoft.com) 。</span><span class="sxs-lookup"><span data-stu-id="56cdb-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="56cdb-149">如果您在 Power Automate 平臺中啟用 CRM 流程的合作夥伴中心時收到下列錯誤，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="要求登入的錯誤訊息":::

<span data-ttu-id="56cdb-151">遵循下列疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="56cdb-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="56cdb-152">先啟用下列兩個子流程，再啟用合作夥伴中心至 CRM flow。</span><span class="sxs-lookup"><span data-stu-id="56cdb-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="56cdb-153">合作夥伴中心至 CRM-Helper (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="56cdb-154">合作夥伴中心 Microsoft 共同銷售參考更新至 CRM (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="56cdb-155">當您嘗試編輯流程時，當您無法將連接新增至流程時，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="56cdb-156">當流程正在執行時，您會新增流程的連接，而且您會個別新增至每個流程。</span><span class="sxs-lookup"><span data-stu-id="56cdb-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="56cdb-157">如果在編輯流程時，加入連接的對話方塊未自動開啟，則您可以個別編輯流程的每個步驟和子步驟。</span><span class="sxs-lookup"><span data-stu-id="56cdb-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="56cdb-158">選取每個流程，並個別加以編輯。</span><span class="sxs-lookup"><span data-stu-id="56cdb-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="56cdb-159">展開流程中的所有步驟</span><span class="sxs-lookup"><span data-stu-id="56cdb-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="要求登入的錯誤訊息":::

- <span data-ttu-id="56cdb-161">選取您會在其中看到警告圖示的步驟，要求關聯連接，以及新增連接。</span><span class="sxs-lookup"><span data-stu-id="56cdb-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="要求登入的錯誤訊息":::


5. <span data-ttu-id="56cdb-163">如果共同銷售推薦連接器解決方案的流程未開啟，您該怎麼做？</span><span class="sxs-lookup"><span data-stu-id="56cdb-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="56cdb-164">A.</span><span class="sxs-lookup"><span data-stu-id="56cdb-164">A.</span></span> <span data-ttu-id="56cdb-165">在 Power Automate 中，您必須以下列順序編輯流程，並將其更新為使用正確的連接：</span><span class="sxs-lookup"><span data-stu-id="56cdb-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="56cdb-166">合作夥伴中心 Webhook 註冊 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-167">建立共同銷售參考-Salesforce 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-168">合作夥伴中心 Microsoft 共同銷售參考更新至 Salesforce (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-169">合作夥伴中心至 Salesforce (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-170">Salesforce 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-171">合作夥伴中心 (Insider Preview) 的 Salesforce 機會</span><span class="sxs-lookup"><span data-stu-id="56cdb-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="56cdb-172">合作夥伴中心 (Insider Preview) 的 Salesforce Microsoft 解決方案</span><span class="sxs-lookup"><span data-stu-id="56cdb-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="56cdb-173">B.</span><span class="sxs-lookup"><span data-stu-id="56cdb-173">B.</span></span> <span data-ttu-id="56cdb-174">針對每個流程，選取 [ **僅執行使用者** ] 選項。</span><span class="sxs-lookup"><span data-stu-id="56cdb-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="56cdb-175">選取 [ **使用連接** ，而不是 **由僅限執行的使用者提供**]。</span><span class="sxs-lookup"><span data-stu-id="56cdb-175">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="要求登入的錯誤訊息":::


<span data-ttu-id="56cdb-177">C.</span><span class="sxs-lookup"><span data-stu-id="56cdb-177">C.</span></span> <span data-ttu-id="56cdb-178">在下列提及的流程中啟用下列各項：</span><span class="sxs-lookup"><span data-stu-id="56cdb-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="56cdb-179">合作夥伴中心 Microsoft 共同銷售參考更新至 Salesforce (Insider preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="56cdb-180">Salesforce 至合作夥伴中心 (Insider Preview) </span><span class="sxs-lookup"><span data-stu-id="56cdb-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="56cdb-181">D.</span><span class="sxs-lookup"><span data-stu-id="56cdb-181">D.</span></span> <span data-ttu-id="56cdb-182">啟用所有剩餘的流程。</span><span class="sxs-lookup"><span data-stu-id="56cdb-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="56cdb-183">E.</span><span class="sxs-lookup"><span data-stu-id="56cdb-183">E.</span></span> <span data-ttu-id="56cdb-184">在 [flow] 合作夥伴中心 Webhook 註冊中，選取 [ **執行**]。</span><span class="sxs-lookup"><span data-stu-id="56cdb-184">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="56cdb-185">從合作夥伴中心中的第一個動作提供 **HTTP url** **至 Salesforce** flow。</span><span class="sxs-lookup"><span data-stu-id="56cdb-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="56cdb-186">選取 [ **要註冊的事件** ] 底下的四個選項，然後選取 **[是]** 進行覆寫。</span><span class="sxs-lookup"><span data-stu-id="56cdb-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="56cdb-187">有關執行/維護的問題和解答</span><span class="sxs-lookup"><span data-stu-id="56cdb-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="56cdb-188">當 Power Automate 流程執行期間發生失敗時，您要如何進行疑難排解？</span><span class="sxs-lookup"><span data-stu-id="56cdb-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="56cdb-189">為了確保您的 Power Automate 流程會如預期般執行，並在執行期間針對失敗進行疑難排解，請參閱 [修正流程失敗](/power-automate/fix-flow-failures)。</span><span class="sxs-lookup"><span data-stu-id="56cdb-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="56cdb-190">如果您在合作夥伴中心或 CRM 環境中看到未正確同步處理的參考，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="56cdb-191">若要判斷參照同步處理的狀態，請選取 [ **Audit**]。</span><span class="sxs-lookup"><span data-stu-id="56cdb-191">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="要求登入的錯誤訊息":::

<span data-ttu-id="56cdb-193">請確定符合下列條件：</span><span class="sxs-lookup"><span data-stu-id="56cdb-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="56cdb-194">解決方案識別碼會作為商機的一部分來提供。</span><span class="sxs-lookup"><span data-stu-id="56cdb-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="56cdb-195">需要兩個字母的國家/地區代碼。</span><span class="sxs-lookup"><span data-stu-id="56cdb-195">Two letter country code is required.</span></span>

- <span data-ttu-id="56cdb-196">當您為商機選取 Microsoft 的協助時，需要客戶連絡人資訊。</span><span class="sxs-lookup"><span data-stu-id="56cdb-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="56cdb-197">如何確保參考會雙向同步處理？</span><span class="sxs-lookup"><span data-stu-id="56cdb-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="56cdb-198">請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="56cdb-198">Do the following steps:</span></span>

- <span data-ttu-id="56cdb-199">合作夥伴銷售人員必須確保他們已啟用與 CRM 區段中合作夥伴中心選項的 **同步** 。</span><span class="sxs-lookup"><span data-stu-id="56cdb-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="要求登入的錯誤訊息":::

- <span data-ttu-id="56cdb-201">銷售人員必須在符合潛在客戶時提供收入和結束日期。</span><span class="sxs-lookup"><span data-stu-id="56cdb-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="56cdb-202">如果在共同銷售商機的 [ **建立** ] 或 [ **更新** ] 階段中提供 CRM 識別碼，但在 crm 中找不到具有該識別碼的潛在客戶機會，則會忽略 [更新] 或 [建立]。</span><span class="sxs-lookup"><span data-stu-id="56cdb-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="56cdb-203">確定已在 Salesforce 環境上設定參考貨幣欄位。</span><span class="sxs-lookup"><span data-stu-id="56cdb-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="56cdb-204">如果連接器中斷連線，而您錯過了參考同步處理，該怎麼辦。</span><span class="sxs-lookup"><span data-stu-id="56cdb-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="56cdb-205">以下是您可以嘗試的幾個選項：</span><span class="sxs-lookup"><span data-stu-id="56cdb-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="56cdb-206">使用參考系統管理員角色檢查合作夥伴中心使用者的使用者名稱或密碼是否已過期。</span><span class="sxs-lookup"><span data-stu-id="56cdb-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="56cdb-207">您可以移至未同步處理的商機、進行次要更新，並觀察參考是否已同步處理。</span><span class="sxs-lookup"><span data-stu-id="56cdb-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="56cdb-208">如果流程已執行且失敗，請選取流程，然後重新提交失敗的執行。</span><span class="sxs-lookup"><span data-stu-id="56cdb-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="56cdb-209">當您收到拒絕存取的錯誤時，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="56cdb-210">請確定有適當的角色存在</span><span class="sxs-lookup"><span data-stu-id="56cdb-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="56cdb-211">合作夥伴中心賣方的推薦系統管理員角色</span><span class="sxs-lookup"><span data-stu-id="56cdb-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="56cdb-212">您 CRM 實例上的系統管理員或系統自訂員角色</span><span class="sxs-lookup"><span data-stu-id="56cdb-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="56cdb-213">確認 Power Automate flow 帳戶使用者事先登入 https://flow.microsoft.com 至少一次</span><span class="sxs-lookup"><span data-stu-id="56cdb-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="56cdb-214">如果您在建立共同銷售商機時看到 **客戶帳戶的國家/地區代碼** 遺失，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="56cdb-215">您必須將 ISO 兩個字母的國家/地區代碼新增至 CRM 中的客戶帳戶。</span><span class="sxs-lookup"><span data-stu-id="56cdb-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="56cdb-216">如果您在建立共同銷售商機時看到 **解決方案識別碼所需** 的錯誤，該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="56cdb-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="56cdb-217">若要建立共同銷售的參考，您需要 Microsoft 共同銷售準備就緒的解決方案。</span><span class="sxs-lookup"><span data-stu-id="56cdb-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="56cdb-218">當您看到在合作夥伴中心中建立且未同步處理至 CRM 的共同銷售商機時，該怎麼辦，即使沒有任何流程錯誤也是一樣：</span><span class="sxs-lookup"><span data-stu-id="56cdb-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="56cdb-219">執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="56cdb-219">Do the following:</span></span>

- <span data-ttu-id="56cdb-220">在合作夥伴中心中建立新的共同銷售交易之後，請檢查是否已叫用合作夥伴中心至 Dynamics 365 流程， (可能會) 叫用多次。</span><span class="sxs-lookup"><span data-stu-id="56cdb-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="56cdb-221">如果已叫用流程，請檢查所有叫用的流程，並識別會更新 CRM 的流程執行。</span><span class="sxs-lookup"><span data-stu-id="56cdb-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="56cdb-222">您可以遵循這些動作，並確認它是否已更新 CRM 或遇到問題。</span><span class="sxs-lookup"><span data-stu-id="56cdb-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="56cdb-223">檢查合作夥伴中心中的 [ \*新增交易\*\*]，查看是否已填入 CRM 識別碼。</span><span class="sxs-lookup"><span data-stu-id="56cdb-223">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="56cdb-224">確定在合作夥伴中心中，交易不會意外地關閉為「成功」或「遺失」。</span><span class="sxs-lookup"><span data-stu-id="56cdb-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56cdb-225">後續步驟</span><span class="sxs-lookup"><span data-stu-id="56cdb-225">Next steps</span></span>

- [<span data-ttu-id="56cdb-226">管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="56cdb-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="56cdb-227">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="56cdb-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)