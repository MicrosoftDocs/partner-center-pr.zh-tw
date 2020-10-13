---
title: 將 azure 訂用帳戶的 azure 訂用帳戶轉移給另一個 CSP 合作夥伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在 Azure 方案下變更與客戶的 Azure 訂用帳戶相關聯的雲端解決方案提供者方案合作夥伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/13/2020
ms.locfileid: "91980259"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="a52dd-103">將客戶的 Azure 方案訂用帳戶轉移至不同的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

## <a name="applies-to"></a><span data-ttu-id="a52dd-104">適用於</span><span class="sxs-lookup"><span data-stu-id="a52dd-104">Applies to</span></span>

- <span data-ttu-id="a52dd-105">雲端解決方案提供者 (CSP) 計畫中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="a52dd-106">本文說明客戶如何將 Azure 方案下的 azure 訂用帳戶從一個雲端解決方案提供者 (CSP) 切換至另一個。</span><span class="sxs-lookup"><span data-stu-id="a52dd-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="a52dd-107">若要從不同的夥伴切換客戶的 Azure 訂用帳戶，請遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="a52dd-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="a52dd-108">夥伴和客戶都有完成的步驟。</span><span class="sxs-lookup"><span data-stu-id="a52dd-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="a52dd-109">只有與 Microsoft 具有直接計費關係的合作夥伴可以存取轉換工具。</span><span class="sxs-lookup"><span data-stu-id="a52dd-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="a52dd-110">間接轉銷商必須與間接提供者合作，以利用這種轉換工具。</span><span class="sxs-lookup"><span data-stu-id="a52dd-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="a52dd-111">客戶必須與這兩個夥伴交談 (目前和未來的) ，才能運用這項工具。</span><span class="sxs-lookup"><span data-stu-id="a52dd-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="a52dd-112">離線對話必須能夠避免混淆和流失。</span><span class="sxs-lookup"><span data-stu-id="a52dd-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="a52dd-113">此外，合作夥伴和客戶應該在起始轉換之前，先瞭解這些考慮和必要條件：</span><span class="sxs-lookup"><span data-stu-id="a52dd-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="a52dd-114">**重要考慮：**</span><span class="sxs-lookup"><span data-stu-id="a52dd-114">**Key considerations:**</span></span>

- <span data-ttu-id="a52dd-115">Azure 保留專案不會隨訂用帳戶移至未來合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="a52dd-116">目前合作夥伴下的 Azure 服務 CSP 定價不會轉換</span><span class="sxs-lookup"><span data-stu-id="a52dd-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="a52dd-117">客戶的支援責任將移至未來的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="a52dd-118">計費和發票開立將在傳輸時移至未來合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="a52dd-119">Azure Role-Based 存取控制 (RBAC) 不受傳輸影響</span><span class="sxs-lookup"><span data-stu-id="a52dd-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="a52dd-120">系統管理員代表 (AOBO) 預設不會授與未來合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a52dd-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="a52dd-121">只要產品通過 Marketplace 資格檢查，就會傳輸協力廠商 marketplace 產品。</span><span class="sxs-lookup"><span data-stu-id="a52dd-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="a52dd-122">沒有特殊的折扣或區域限制</span><span class="sxs-lookup"><span data-stu-id="a52dd-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="a52dd-123">非訂用帳戶為基礎的產品</span><span class="sxs-lookup"><span data-stu-id="a52dd-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="a52dd-124">未來的夥伴應與發行者合作，以確保他們位於產品部署的允許清單中</span><span class="sxs-lookup"><span data-stu-id="a52dd-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="a52dd-125">如果未符合上述所有條件，則必須取消 Azure 訂用帳戶，然後再以新的合作夥伴重新購買 Marketplace 產品的傳送</span><span class="sxs-lookup"><span data-stu-id="a52dd-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="a52dd-126">**必要條件：**</span><span class="sxs-lookup"><span data-stu-id="a52dd-126">**Prerequisites:**</span></span>

- <span data-ttu-id="a52dd-127">客戶參與目前的 CSP 合作夥伴，以進行轉換</span><span class="sxs-lookup"><span data-stu-id="a52dd-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="a52dd-128">未來的 CSP 合作夥伴會與客戶合作，以確保符合客戶需求</span><span class="sxs-lookup"><span data-stu-id="a52dd-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="a52dd-129">未來的 CSP 合作夥伴會在轉換開始前與客戶建立關聯性</span><span class="sxs-lookup"><span data-stu-id="a52dd-129">Future CSP partner establishes a relationship with customer before transition begins</span></span>  
- <span data-ttu-id="a52dd-130">客戶必須使用未來的 CSP 合作夥伴簽署 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="a52dd-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="a52dd-131">未來的 CSP 合作夥伴必須已簽署 Microsoft 合作夥伴合約才能使用此工具</span><span class="sxs-lookup"><span data-stu-id="a52dd-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="a52dd-132">要完成的客戶工作</span><span class="sxs-lookup"><span data-stu-id="a52dd-132">Customer tasks to be completed</span></span>

<span data-ttu-id="a52dd-133">若要轉移 azure 訂用帳戶下的 Azure 訂用帳戶，客戶必須聯絡其目前的合作夥伴來開始此程式。</span><span class="sxs-lookup"><span data-stu-id="a52dd-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="a52dd-134">他們應該收集其目前合作夥伴的公司名稱和網域，讓其未來的合作夥伴可以代表他們完成傳送申請表單。</span><span class="sxs-lookup"><span data-stu-id="a52dd-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="a52dd-135">客戶也必須識別他們想要從目前合作夥伴轉移的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a52dd-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="a52dd-136">您無法變更 Office 365、Enterprise 行動套件或 Microsoft Dynamics CRM 訂閱的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="a52dd-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="a52dd-137">未來的合作夥伴必須負責完成傳送要求表單，以起始傳輸程式。</span><span class="sxs-lookup"><span data-stu-id="a52dd-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="a52dd-138">Microsoft 無法代表客戶或目前的夥伴介入。</span><span class="sxs-lookup"><span data-stu-id="a52dd-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="a52dd-139">客戶應該規劃與其未來和目前的合作夥伴密切合作，以順利進行轉換。</span><span class="sxs-lookup"><span data-stu-id="a52dd-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="a52dd-140">未來要完成的夥伴工作</span><span class="sxs-lookup"><span data-stu-id="a52dd-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="a52dd-141">訂用帳戶的未來夥伴需要從合作夥伴中心完成傳送要求表單，以要求訂用帳戶轉移：</span><span class="sxs-lookup"><span data-stu-id="a52dd-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="a52dd-142">從 [合作夥伴中心] 功能表選取 [ **客戶**]，然後選取您想要代表的客戶完成傳送申請表單。</span><span class="sxs-lookup"><span data-stu-id="a52dd-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="a52dd-143">從 [客戶] 功能表選取 [ **訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="a52dd-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="a52dd-144">選取 [ **轉移要求** ] 區段。</span><span class="sxs-lookup"><span data-stu-id="a52dd-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="a52dd-145">從 [ **轉移要求] 區段**中，選取 [ **加入新要求**]。</span><span class="sxs-lookup"><span data-stu-id="a52dd-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="傳輸區段":::

5.  <span data-ttu-id="a52dd-147">完成 **新的傳送要求** 表單。</span><span class="sxs-lookup"><span data-stu-id="a52dd-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="a52dd-148">選取 [傳送**轉移要求**  >  **傳送]**。</span><span class="sxs-lookup"><span data-stu-id="a52dd-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="傳輸區段":::

7.  <span data-ttu-id="a52dd-150">檢查傳輸要求確認</span><span class="sxs-lookup"><span data-stu-id="a52dd-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="傳輸區段":::

    >[!Note]
    ><span data-ttu-id="a52dd-152">未來的夥伴只要在傳輸要求狀態為「擱置中」時，在右上角選取 [ **取消要求** ]，即可取消轉移要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="a52dd-153">當傳輸要求狀態為「進行中」或「完成」時，將無法取消。</span><span class="sxs-lookup"><span data-stu-id="a52dd-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="a52dd-154">目前要完成的夥伴工作</span><span class="sxs-lookup"><span data-stu-id="a52dd-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="a52dd-155">客戶目前的夥伴管理員代理程式會收到一封電子郵件，指出其客戶要求轉移其訂用帳戶：</span><span class="sxs-lookup"><span data-stu-id="a52dd-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="傳輸區段":::

<span data-ttu-id="a52dd-157">請檢查並接受合作夥伴中心的轉移要求表單，以完成訂用帳戶轉移。</span><span class="sxs-lookup"><span data-stu-id="a52dd-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="a52dd-158">如果目前合作夥伴在30天內未採取任何動作，則要求將會過期，而未來的夥伴將會有一個來建立新的轉移要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="a52dd-159">選取電子郵件中的 **審核轉移要求** 或</span><span class="sxs-lookup"><span data-stu-id="a52dd-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="a52dd-160">從 [合作夥伴中心] 功能表中，選取 [ **Customers**]，然後選取代表已提交轉移要求的客戶。</span><span class="sxs-lookup"><span data-stu-id="a52dd-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="a52dd-161">從 [客戶] 功能表選取 [ **訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="a52dd-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="a52dd-162">選取 [ **轉移要求** ] 區段。</span><span class="sxs-lookup"><span data-stu-id="a52dd-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="a52dd-163">在 [**收到的要求**] 底下選取所選的**傳輸要求識別碼**，以展開 [傳送資訊]</span><span class="sxs-lookup"><span data-stu-id="a52dd-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="傳輸區段":::

5.  <span data-ttu-id="a52dd-165">查看轉移要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-165">Review transfer request.</span></span> <span data-ttu-id="a52dd-166">選取要傳送的要求 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a52dd-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="a52dd-167">繼續進行之前，請注意：您將無法再存取選取的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a52dd-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="a52dd-168">您將不會獲得進一步使用的發票。</span><span class="sxs-lookup"><span data-stu-id="a52dd-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="a52dd-169">Azure 保留專案不會與訂用帳戶一起轉移。</span><span class="sxs-lookup"><span data-stu-id="a52dd-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="a52dd-170">然後選取 [ **接受並傳送** ] 以完成傳送程式。</span><span class="sxs-lookup"><span data-stu-id="a52dd-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="傳輸區段":::

7.  <span data-ttu-id="a52dd-172">查看傳輸接受確認。</span><span class="sxs-lookup"><span data-stu-id="a52dd-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="a52dd-173">此時，未來的夥伴、客戶和目前的合作夥伴將會透過電子郵件通知已接受的轉移要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="a52dd-174">之後，在系統更新時，傳輸狀態可能會維持暫止最多15分鐘的時間，以接受轉換。</span><span class="sxs-lookup"><span data-stu-id="a52dd-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="a52dd-175">如果需要較長的時間，系統會繼續嘗試三天。</span><span class="sxs-lookup"><span data-stu-id="a52dd-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="a52dd-176">如果傳輸狀態仍保持擱置，則夥伴應提交服務要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="a52dd-177">一旦傳輸完成後，要求中所包含的訂用帳戶將會出現在未來合作夥伴的 Azure 方案中，且不再與您一起列出。</span><span class="sxs-lookup"><span data-stu-id="a52dd-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="a52dd-178">若為間接提供者：請通知您的間接轉銷商已接受轉移要求。</span><span class="sxs-lookup"><span data-stu-id="a52dd-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="a52dd-179">管理您已轉移的客戶訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a52dd-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="a52dd-180">使用 Azure 角色型存取控制 (RBAC) 為現有使用者、群組或服務主體指派的存取權，在轉換期間不受影響。</span><span class="sxs-lookup"><span data-stu-id="a52dd-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="a52dd-181">Azure 角色型存取控制 [ (AZURE RBAC) ](/azure/role-based-access-control/overview) 協助客戶管理可存取 azure 資源的人員、這些資源的使用方式，以及他們有權存取的區域。</span><span class="sxs-lookup"><span data-stu-id="a52dd-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="a52dd-182">作為新的合作夥伴，您不會在訂用帳戶轉移之後，對客戶的資源提供任何 RBAC 存取權。</span><span class="sxs-lookup"><span data-stu-id="a52dd-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="a52dd-183">您客戶的先前合作夥伴會保留其 RBAC 存取權。</span><span class="sxs-lookup"><span data-stu-id="a52dd-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="a52dd-184">與您的客戶合作，瞭解誰有見解的訂閱，以及如何進行任何想要的變更。</span><span class="sxs-lookup"><span data-stu-id="a52dd-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="a52dd-185">因此，請務必讓您的客戶移除其先前合作夥伴的 Azure RBAC 存取權，並加入新夥伴的存取權。</span><span class="sxs-lookup"><span data-stu-id="a52dd-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="a52dd-186">如需提供新存取權的客戶詳細資訊，請參閱 [什麼是 AZURE RBAC)  (azure 角色型存取控制？](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="a52dd-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="a52dd-187">如需移除先前合作夥伴 RBAC 存取權的客戶詳細資訊，請參閱 [移除角色指派](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。</span><span class="sxs-lookup"><span data-stu-id="a52dd-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="a52dd-188">此外，您不會自動 [代表 (AOBO ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 取得訂用帳戶的) 存取權。</span><span class="sxs-lookup"><span data-stu-id="a52dd-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="a52dd-189">需要 AOBO，才能代表合作夥伴管理其客戶的 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a52dd-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="a52dd-190">如需有關 Azure 許可權的詳細資訊，請參閱 [取得管理客戶服務或訂用帳戶的許可權。](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="a52dd-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="a52dd-191">後續步驟：</span><span class="sxs-lookup"><span data-stu-id="a52dd-191">Next steps:</span></span>

- [<span data-ttu-id="a52dd-192"> (Azure RBAC) </span><span class="sxs-lookup"><span data-stu-id="a52dd-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="a52dd-193">取得管理客戶服務或訂用帳戶的許可權。</span><span class="sxs-lookup"><span data-stu-id="a52dd-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)