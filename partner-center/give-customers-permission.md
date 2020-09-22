---
title: 讓客戶在 CSP 中購買自己的服務
description: 瞭解 CSP 方案合作夥伴如何讓客戶為在合作夥伴中心中購買的訂用帳戶購買自己的服務（例如 Azure 保留）。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000462"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a><span data-ttu-id="7377d-103">提供客戶合作夥伴中心的許可權，以購買自己的產品或服務</span><span class="sxs-lookup"><span data-stu-id="7377d-103">Give customers permission in Partner Center to buy their own products or services</span></span>

<span data-ttu-id="7377d-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="7377d-104">**Applies to**</span></span>

- <span data-ttu-id="7377d-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="7377d-105">Partner Center</span></span>
- <span data-ttu-id="7377d-106">雲端解決方案提供者方案中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="7377d-106">Partners in the CSP program</span></span>

<span data-ttu-id="7377d-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="7377d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7377d-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="7377d-108">Admin agent</span></span>
- <span data-ttu-id="7377d-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="7377d-109">Sales agent</span></span>

<span data-ttu-id="7377d-110">本文說明雲端解決方案提供者 (CSP) 方案中的合作夥伴如何為客戶提供購買某些服務或資源的許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-110">This article shows how a partner in the Cloud Solution Provider (CSP) program can give a customer permission to buy some of their own services or resources.</span></span>

<span data-ttu-id="7377d-111">CSP 方案中的合作夥伴通常會使用合作夥伴中心及其商業市場，為其客戶購買解決方案和服務。</span><span class="sxs-lookup"><span data-stu-id="7377d-111">Partners in the CSP program often use Partner Center and its commercial marketplace to buy solutions and services for their customers.</span></span> <span data-ttu-id="7377d-112">合作夥伴接著會讓某些客戶直接從 Azure 入口網站自行布建這些服務。</span><span class="sxs-lookup"><span data-stu-id="7377d-112">Partners then allow some customers to provision these services themselves directly from the Azure portal.</span></span>

<span data-ttu-id="7377d-113">以下為範例。</span><span class="sxs-lookup"><span data-stu-id="7377d-113">Here's an example.</span></span> <span data-ttu-id="7377d-114">假設您在合作夥伴中心中為客戶購買 Azure 方案訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-114">Let's say you buy an Azure Plan subscription for a customer in Partner Center.</span></span> <span data-ttu-id="7377d-115">然後，您決定將其他資源或服務代表客戶新增至該訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-115">You then decide to add other resources or services to that subscription on the customer's behalf.</span></span> <span data-ttu-id="7377d-116">在此情況下，您可以將 Azure 保留新增至客戶的訂用帳戶， (例如新增保留的虛擬機器實例) 。</span><span class="sxs-lookup"><span data-stu-id="7377d-116">In this case, you might add Azure reservations to the customer's subscription (such as, adding reserved, virtual machine instances).</span></span> <span data-ttu-id="7377d-117">然後，您可以讓客戶在 Azure 入口網站中進一步布建 Azure 保留資源。</span><span class="sxs-lookup"><span data-stu-id="7377d-117">You might then allow the customer to further provision the Azure reservation resources themselves in the Azure portal.</span></span>

<span data-ttu-id="7377d-118">現在，有了 **客戶許可權** 功能，您可以為客戶提供更多使用 Azure 資源的自助服務選項。</span><span class="sxs-lookup"><span data-stu-id="7377d-118">Now, with the **Customer permissions** feature, you give customers more self-service options with Azure resources.</span></span> <span data-ttu-id="7377d-119">藉由開啟客戶的許可權，您可讓客戶購買自己的資源 (例如，購買自己的 Azure 保留) 。</span><span class="sxs-lookup"><span data-stu-id="7377d-119">By turning on permissions for the customer, you allow customers to buy their own resources (such as, buying their own Azure reservations).</span></span>  

## <a name="overview-of-customer-permissions-in-partner-center"></a><span data-ttu-id="7377d-120">合作夥伴中心中的客戶許可權總覽</span><span class="sxs-lookup"><span data-stu-id="7377d-120">Overview of customer permissions in Partner Center</span></span>

<span data-ttu-id="7377d-121">您可以使用 [客戶 **帳戶** ] 頁面來開啟 (，或關閉) 的客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-121">Use the Customer **Account** page to turn on (or turn off) customer permissions.</span></span> <span data-ttu-id="7377d-122">目前，這項功能支援：</span><span class="sxs-lookup"><span data-stu-id="7377d-122">Currently, this feature supports:</span></span>

- <span data-ttu-id="7377d-123">**Azure 保留：** 開啟此許可權可讓客戶針對您為其購買的特定 Azure 訂用帳戶購買自己的 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-123">**Azure reservations:** Turning on this permission allows the customer to purchase their own Azure reservations for a specific Azure subscription you've purchased for them.</span></span>

<span data-ttu-id="7377d-124">在您開啟客戶許可權之前，請注意下列重點：</span><span class="sxs-lookup"><span data-stu-id="7377d-124">Before you turn on customer permissions, note these important points:</span></span>

- <span data-ttu-id="7377d-125">根據預設，客戶許可權會自動停用 (關閉合作夥伴中心中的) 。</span><span class="sxs-lookup"><span data-stu-id="7377d-125">By default, customer permissions are automatically disabled (turned off) in Partner Center.</span></span>

- <span data-ttu-id="7377d-126">您必須在合作夥伴中心中指派系統管理員代理程式角色，才能開啟 (或關閉客戶) 許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-126">Before you can turn on (or turn off) permissions for a customer, you must be assigned the role of Admin Agent in Partner Center.</span></span>

  <span data-ttu-id="7377d-127">獲指派銷售專員或服務中心代理程式角色的夥伴擁有唯讀存取權，無法開啟或關閉客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-127">Partners assigned the role of Sales Agent or Help Desk Agent have read-only access and can't turn customer permissions on or off.</span></span>

- <span data-ttu-id="7377d-128">您可以開啟 (針對您選擇的任何客戶啟用) 許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-128">You can turn on (enable) permissions for any customer you choose.</span></span>

- <span data-ttu-id="7377d-129">您可以使用合作夥伴中心儀表板或 [合作夥伴中心 api](/partner-center/develop/manage-customers)來開啟 (或關閉) 的客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-129">You can turn on (or turn off) customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

- <span data-ttu-id="7377d-130">當您開啟 (啟用特定客戶的) 許可權之後，您將負責支付該客戶的任何後續購買款項。</span><span class="sxs-lookup"><span data-stu-id="7377d-130">After you turn on (enable) permissions for a specific customer, you will be responsible to pay for any subsequent purchases made by that customer.</span></span> <span data-ttu-id="7377d-131">如果客戶想要交換、取消或更新購買 (或想要變更保留) 的初始範圍，他們本身將無法執行此作業。</span><span class="sxs-lookup"><span data-stu-id="7377d-131">If customers want to exchange, cancel or renew a purchase they've made (or they want to change the initial scope of a reservation), they will not be able to do so themselves.</span></span> <span data-ttu-id="7377d-132">他們需要以合作夥伴的身份要求您，以協助他們交換、取消和續約購買專案，或在日後變更保留範圍。</span><span class="sxs-lookup"><span data-stu-id="7377d-132">They need to ask you, as the partner, to help them exchange, cancel, and renew purchases, or make later changes to a reservation's scope.</span></span>  

- <span data-ttu-id="7377d-133">當您開啟特定客戶的許可權之後，系統將 **不會** 通知您任何稍後由客戶進行的購買。</span><span class="sxs-lookup"><span data-stu-id="7377d-133">After you turn on permissions for a specific customer, you will **not be** notified of any later purchases made by the customer.</span></span>

- <span data-ttu-id="7377d-134">客戶的後續購買將會隨您在合作夥伴中心中顯示。</span><span class="sxs-lookup"><span data-stu-id="7377d-134">Later purchases made by the customer will appear in Partner Center along with any purchases made by you.</span></span> <span data-ttu-id="7377d-135">您可以在客戶的 **訂單歷程記錄** 頁面、其 **保留** 頁面或 [**活動記錄**](activity-logs.md)中找到這些購買專案。</span><span class="sxs-lookup"><span data-stu-id="7377d-135">You can find these purchases on the customer's **Order history** page, their **Reservations** page, or in the [**Activity Log**](activity-logs.md).</span></span>

>[!NOTE]
> <span data-ttu-id="7377d-136">如需客戶將支付的價格以及如何協助客戶管理其購買的相關資訊，請參閱 [協助客戶管理購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="7377d-136">For information about prices the customer will pay and how to help customers manage their purchases, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a><span data-ttu-id="7377d-137">提供客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="7377d-137">Give customers permission to buy their own Azure reservations</span></span>

<span data-ttu-id="7377d-138">Azure 保留是以折扣價購買 Azure 服務的絕佳方式。</span><span class="sxs-lookup"><span data-stu-id="7377d-138">Azure reservations are a great way to buy Azure services at a discounted rate.</span></span> <span data-ttu-id="7377d-139">若要深入瞭解 Azure 保留的優點，請參閱 [什麼是 Azure 保留專案？](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="7377d-139">To learn more about the benefits of Azure reservations, see [What are Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)</span></span>

<span data-ttu-id="7377d-140">現在您可以選擇代表客戶購買 Azure 保留，因為您可能已經完成。</span><span class="sxs-lookup"><span data-stu-id="7377d-140">Now you have the choice to buy Azure reservations on behalf of your customers, as you may have already been doing.</span></span> <span data-ttu-id="7377d-141">或者，您可以授與客戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-141">Or, you can give customers permission to buy their own Azure reservations.</span></span>

>[!NOTE]
> <span data-ttu-id="7377d-142">在您授與客戶購買自己的 Azure 保留的許可權之後，請協助他們管理任何購買的保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-142">After you give customers permission to buy their own Azure reservations, help them manage any reservations they purchase.</span></span> <span data-ttu-id="7377d-143">如需詳細資訊，請參閱 [協助客戶管理購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。</span><span class="sxs-lookup"><span data-stu-id="7377d-143">For more information, see [Help customers manage reservations they purchase](give-customers-permission.md#help-customers-manage-reservations-they-purchase).</span></span>

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a><span data-ttu-id="7377d-144">讓客戶購買自己的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="7377d-144">To enable customers to buy their own Azure reservations</span></span>

1. <span data-ttu-id="7377d-145">確認客戶有您購買的現有 Azure 方案或 Azure 全域訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-145">Verify the customer has an existing Azure Plan or Azure Global subscription you purchased on their behalf.</span></span>

2. <span data-ttu-id="7377d-146">確認客戶已獲指派此訂用帳戶的 **擁有** 者角色。</span><span class="sxs-lookup"><span data-stu-id="7377d-146">Verify the customer has been assigned the **Owner** role for this subscription.</span></span>

3. <span data-ttu-id="7377d-147">啟用客戶許可權 (**在) 上** 開啟此功能，以購買自己的 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-147">Enable customer permissions (turn this feature **On**) to purchase their own Azure reservations.</span></span>

<span data-ttu-id="7377d-148">每個步驟都會顯示在下方。</span><span class="sxs-lookup"><span data-stu-id="7377d-148">Each step appears below.</span></span>

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a><span data-ttu-id="7377d-149">確認客戶擁有現有的 Azure 訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="7377d-149">Verify the customer has an existing Azure subscription</span></span>

<span data-ttu-id="7377d-150">在您授與客戶購買自己的 Azure 保留的許可權之前，您必須確認客戶已有現有的 Azure 方案或 Azure 全域訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-150">Before you give customers permission to buy their own Azure reservations, you must verify the customer has an existing Azure Plan or Azure Global subscription.</span></span> <span data-ttu-id="7377d-151">如果客戶未在合作夥伴中心中顯示目前的 Azure 訂用帳戶，您必須先為他們購買訂用帳戶，才能開啟其客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-151">If the customer shows no current Azure subscription in Partner Center, you must buy a subscription for them before you turn on their customer permissions.</span></span>

- <span data-ttu-id="7377d-152">若要查看客戶是否已有 Azure 訂用帳戶，請登入合作夥伴中心儀表板，然後選取 [ **CSP** ]，再選取 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="7377d-152">To see if a customer already has an Azure subscription, sign into the Partner Center dashboard, then select **CSP** followed by **Customers**.</span></span> <span data-ttu-id="7377d-153">從清單中選取特定的客戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-153">Select the specific customer from the list.</span></span> <span data-ttu-id="7377d-154">**然後選取訂**用帳戶，並尋找 azure 方案或 azure Global 的任何以使用量為基礎的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-154">Then select **Subscriptions** and look for any usage-based subscriptions for either Azure Plan or Azure Global.</span></span>

- <span data-ttu-id="7377d-155">如果客戶沒有現有的 Azure 訂用帳戶，您可以為他們購買訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-155">If a customer doesn't have an existing Azure subscription, you can buy a subscription for them.</span></span> <span data-ttu-id="7377d-156">請參閱 [購買 Azure 方案](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="7377d-156">See [Purchase the Azure Plan](purchase-azure-plan.md).</span></span>

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a><span data-ttu-id="7377d-157">確認已在 Azure 中將正確的角色指派給客戶</span><span class="sxs-lookup"><span data-stu-id="7377d-157">Verify the customer has been assigned the correct role in Azure</span></span>

<span data-ttu-id="7377d-158">在您確認客戶擁有現有的 Azure 訂用帳戶之後，您也需要確認與客戶相關聯的金鑰使用者已獲指派該 Azure 訂用帳戶的正確 **擁有** 者角色。</span><span class="sxs-lookup"><span data-stu-id="7377d-158">After you verify the customer has an existing Azure subscription, you also need to verify the key users associated with your customer have been assigned the correct **Owner** role for that Azure subscription.</span></span> <span data-ttu-id="7377d-159">這是以角色為基礎的存取 (RBAC) 客戶必須為您購買的 Azure 訂用帳戶購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-159">This is the role-based access (RBAC) the customer needs to buy Azure reservations for an Azure subscription you purchased.</span></span>

<span data-ttu-id="7377d-160">某些夥伴可能已將 **擁有** 者角色指派給想要主動管理及布建自己的 Azure 資源的客戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-160">Some partners may have already assigned the **Owner** role to customers wanting to actively manage and provision their own Azure resources.</span></span> <span data-ttu-id="7377d-161">如果您已將 **擁有** 者狀態指派給客戶，以管理您為其購買的先前訂用帳戶，您可以略過此步驟。</span><span class="sxs-lookup"><span data-stu-id="7377d-161">If you have already assigned **Owner** status to a customer to manage prior subscriptions you've purchased for them, you can skip this step.</span></span>  

> [!IMPORTANT]
> <span data-ttu-id="7377d-162">如果客戶未獲指派 **擁有** 者角色，他們將會在 Azure 入口網站中收到錯誤，使其無法購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-162">If a customer has not been assigned the **Owner** role, they will receive an error in the Azure portal preventing them from buying Azure reservations.</span></span>

<span data-ttu-id="7377d-163">若要確認客戶已獲指派 Azure 訂用帳戶的 **擁有** 者角色：</span><span class="sxs-lookup"><span data-stu-id="7377d-163">To verify the customer has been assigned the **Owner** role for an Azure subscription:</span></span>

1. <span data-ttu-id="7377d-164">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="7377d-164">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7377d-165">選取 [ **CSP**]，然後選取 [ **客戶** ]，然後選取特定的客戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-165">Select **CSP**, then **Customers** and select the specific customer.</span></span>

3. <span data-ttu-id="7377d-166">選取 **該客戶的訂** 用帳戶，並找出特定的 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7377d-166">Select **Subscriptions** for that customer and locate the specific Azure subscription.</span></span>

4. <span data-ttu-id="7377d-167">選取該客戶訂用帳戶旁邊的 [ **管理** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="7377d-167">Select the **Manage** button next to that customer's subscription.</span></span> <span data-ttu-id="7377d-168">這麼做會開啟 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="7377d-168">Doing so opens the [Azure portal](https://portal.azure.com/).</span></span>

5. <span data-ttu-id="7377d-169">若要將 **擁有** 者角色指派給特定使用者，請遵循下列步驟， [將使用者指派為系統管理員](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。</span><span class="sxs-lookup"><span data-stu-id="7377d-169">To assign the **Owner** role to a specific user, follow these steps [To assign a user as an administrator](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).</span></span>

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a><span data-ttu-id="7377d-170">開啟或關閉客戶許可權以購買自己的 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="7377d-170">Turn on or turn off customer permissions to purchase their own Azure reservations</span></span>

<span data-ttu-id="7377d-171">在您確認客戶擁有現有的 Azure 訂用帳戶，且已將該訂用帳戶的 **擁有** 者角色指派給使用者之後，您就可以開啟 (啟用) 的客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-171">After you verify the customer has an existing Azure subscription and users are assigned the **Owner** role for that subscription, you're ready to turn on (enable) customer permissions.</span></span> <span data-ttu-id="7377d-172">您也可以使用這些步驟關閉 (停用) 客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-172">You can also use these steps to turn off (disable) customer permissions.</span></span> <span data-ttu-id="7377d-173">您可以使用合作夥伴中心儀表板或 [合作夥伴中心 api](/partner-center/develop/manage-customers)來啟用或停用客戶許可權。</span><span class="sxs-lookup"><span data-stu-id="7377d-173">You can enable or disable customer permissions using either the Partner Center dashboard or [Partner Center APIs](/partner-center/develop/manage-customers).</span></span>

<span data-ttu-id="7377d-174">若要開啟 (或關閉合作夥伴中心中的) 客戶許可權：</span><span class="sxs-lookup"><span data-stu-id="7377d-174">To turn on (or turn off) customer permissions in Partner Center:</span></span>

1. <span data-ttu-id="7377d-175">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="7377d-175">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="7377d-176">從左側導覽功能表中，選取 [ **CSP**]，然後選取 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="7377d-176">From the left navigation menu, select **CSP**, then **Customers**.</span></span> <span data-ttu-id="7377d-177">客戶清單隨即出現。</span><span class="sxs-lookup"><span data-stu-id="7377d-177">A customer list appears.</span></span>

3. <span data-ttu-id="7377d-178">選取特定的客戶名稱。</span><span class="sxs-lookup"><span data-stu-id="7377d-178">Select a specific customer name.</span></span>

4. <span data-ttu-id="7377d-179">從 [客戶] 功能表中選取 [ **帳戶** ]。</span><span class="sxs-lookup"><span data-stu-id="7377d-179">Select **Account** from the customer menu.</span></span> <span data-ttu-id="7377d-180">[客戶 **帳戶** ] 頁面隨即出現。</span><span class="sxs-lookup"><span data-stu-id="7377d-180">The customer **Account** page appears.</span></span>

5. <span data-ttu-id="7377d-181">在頁面底部找出 [ **客戶許可權** ] 區域。</span><span class="sxs-lookup"><span data-stu-id="7377d-181">Locate the **Customer permissions** area at the bottom of the page.</span></span>

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="帳戶頁面上的客戶許可權。" border="true":::

6. <span data-ttu-id="7377d-183">在 [ **Azure 保留**] 底下，找出 [ **允許客戶購買** ] 選項。</span><span class="sxs-lookup"><span data-stu-id="7377d-183">Under **Azure reservations**, locate the **Allow customer to purchase** option.</span></span>

7. <span data-ttu-id="7377d-184">若要開啟客戶許可權，請將此選項旁邊的開關移至 [ **開啟** ] 位置。</span><span class="sxs-lookup"><span data-stu-id="7377d-184">To turn on customer permissions, move the switch next to this option to the **On** position.</span></span> <span data-ttu-id="7377d-185">若要關閉客戶許可權，請將開關移至 [ **關閉** ] 位置。</span><span class="sxs-lookup"><span data-stu-id="7377d-185">To turn off customer permissions, move the switch to the **Off** position.</span></span>

>[!NOTE]
> <span data-ttu-id="7377d-186">若要瞭解當您開啟客戶的許可權來購買自己的 Azure 保留時，會發生什麼情況，請參閱 [合作夥伴中心中的客戶許可權總覽](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="7377d-186">To learn what else happens when you turn on a customer's permissions to purchase their own Azure reservations, see [Overview of customer permissions in Partner Center](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).</span></span>
>
><span data-ttu-id="7377d-187">當您開啟 (或關閉) 客戶許可權時，活動記錄會記錄每個動作。</span><span class="sxs-lookup"><span data-stu-id="7377d-187">When you turn on (or turn off) customer permissions, the Activity log records each action.</span></span> <span data-ttu-id="7377d-188">當您選取合作夥伴中心儀表板) 頂端的齒輪圖示時， (可以存取此記錄檔。</span><span class="sxs-lookup"><span data-stu-id="7377d-188">(This log is accessible when you select the Gear icon from the top of the Partner Center dashboard).</span></span> <span data-ttu-id="7377d-189">當您開啟或關閉客戶許可權時，此動作會顯示為 [ **建立客戶購買許可權** ] 或 [ **刪除客戶購買許可權** ] 活動記錄。</span><span class="sxs-lookup"><span data-stu-id="7377d-189">When you turn customer permissions on or off, the action will appear as either **Create Customer Purchase Permissions** or **Delete Customer Purchase Permissions** in the Activity log.</span></span>

## <a name="help-customers-manage-reservations-they-purchase"></a><span data-ttu-id="7377d-190">協助客戶管理他們購買的保留</span><span class="sxs-lookup"><span data-stu-id="7377d-190">Help customers manage reservations they purchase</span></span>

<span data-ttu-id="7377d-191">一旦您授與客戶購買自己的 Azure 保留的許可權，您可以協助他們更妥善地管理購買的任何資源。</span><span class="sxs-lookup"><span data-stu-id="7377d-191">Once you give customers permission to purchase their own Azure reservations, you can help them better manage any resources they purchase.</span></span> <span data-ttu-id="7377d-192">客戶可以直接從 [Azure 入口網站](https://portal.azure.com/)管理 Azure 保留的許多層面。</span><span class="sxs-lookup"><span data-stu-id="7377d-192">Customers can manage many aspects of Azure reservations themselves directly from the [Azure portal](https://portal.azure.com/).</span></span> <span data-ttu-id="7377d-193">在您的 CSP 訂用帳戶內購買 Azure 保留專案的其他部分時，他們將需要您的協助。</span><span class="sxs-lookup"><span data-stu-id="7377d-193">They will need your help managing a few, other aspects of Azure reservations they purchase within your CSP subscription.</span></span>  

<span data-ttu-id="7377d-194">協助客戶深入瞭解如何管理 Azure 保留的下列各方面：</span><span class="sxs-lookup"><span data-stu-id="7377d-194">Help customers understand more about managing these aspects of Azure reservations:</span></span>

- <span data-ttu-id="7377d-195">客戶將支付 Azure 保留費用</span><span class="sxs-lookup"><span data-stu-id="7377d-195">Prices customers will pay for Azure reservations</span></span>
- <span data-ttu-id="7377d-196">客戶如何優化 Azure 保留的使用</span><span class="sxs-lookup"><span data-stu-id="7377d-196">How customers can optimize use of Azure reservations</span></span>
- <span data-ttu-id="7377d-197">當客戶購買具有共用範圍的保留時，會發生什麼事？</span><span class="sxs-lookup"><span data-stu-id="7377d-197">What happens when customers purchase reservations with a shared scope?</span></span>
- <span data-ttu-id="7377d-198">如果客戶想要變更、取消和更新保留，或變更其範圍，會發生什麼事？</span><span class="sxs-lookup"><span data-stu-id="7377d-198">What happens if customers want to change, cancel, and renew a reservation, or change its scope?</span></span>

<span data-ttu-id="7377d-199">**客戶的價格將支付其保留費用。**</span><span class="sxs-lookup"><span data-stu-id="7377d-199">**Prices customers will pay for their reservations.**</span></span> <span data-ttu-id="7377d-200">您的客戶將會根據您先前在 CSP 合作夥伴計費帳戶中購買的訂用帳戶來購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-200">Your customer will be purchasing Azure reservations based on a subscription you previously bought for them in your CSP partner billing account.</span></span> <span data-ttu-id="7377d-201">客戶根據此訂用帳戶購買之任何 Azure 保留的價格也是由您所設定。</span><span class="sxs-lookup"><span data-stu-id="7377d-201">The customer's price for any Azure reservations they purchase based on this subscription is also set by you.</span></span> <span data-ttu-id="7377d-202">此價格可能與客戶在 Azure 入口網站中看到的 Web Direct 價格不同。</span><span class="sxs-lookup"><span data-stu-id="7377d-202">This price may be different from the Web Direct price the customer sees in the Azure portal.</span></span>

<span data-ttu-id="7377d-203">**客戶可如何將保留的使用優化。**</span><span class="sxs-lookup"><span data-stu-id="7377d-203">**How customers can optimize their use of a reservation.**</span></span> <span data-ttu-id="7377d-204">某些客戶可能會受益于深入瞭解如何將保留的使用優化，或如何在購買期間指派保留的初始範圍。</span><span class="sxs-lookup"><span data-stu-id="7377d-204">Some customers might benefit from learning more about how to optimize their use of a reservation or how to assign a reservation’s initial scope during their purchase.</span></span> <span data-ttu-id="7377d-205">如需詳細資訊，請要求客戶閱讀 [Azure 資源的管理保留](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。</span><span class="sxs-lookup"><span data-stu-id="7377d-205">For more information, ask customers to read [Manage reservations for Azure resources](/azure/cost-management-billing/reservations/manage-reserved-vm-instance).</span></span>

<span data-ttu-id="7377d-206">**當客戶購買具有共用範圍的保留時，會發生什麼事？**</span><span class="sxs-lookup"><span data-stu-id="7377d-206">**What happens when a customer purchases a reservation with a shared scope?**</span></span> <span data-ttu-id="7377d-207">當客戶購買以先前的 CSP 訂用帳戶為基礎的保留，並將共用範圍指派給該保留時，由 CSP 提供給該客戶的所有訂用帳戶折扣將會套用至 CSP 合作夥伴為該客戶購買之所有訂用帳戶的相符使用量。</span><span class="sxs-lookup"><span data-stu-id="7377d-207">When customers purchase a reservation based on a prior CSP subscription and assign a shared scope to that reservation, any discounts the customer has been given by the CSP will apply to matching usage for all subscriptions the CSP partner has purchased for that customer.</span></span>

<span data-ttu-id="7377d-208">**如果客戶想要交換、取消或續約他們所做的購買，或變更保留的初始範圍，該怎麼辦？**</span><span class="sxs-lookup"><span data-stu-id="7377d-208">**What should customers do if they want to exchange, cancel, or renew a purchase they have made, or change the initial scope of a reservation?**</span></span> <span data-ttu-id="7377d-209">客戶必須要求合作夥伴協助他們變更保留的初始範圍。</span><span class="sxs-lookup"><span data-stu-id="7377d-209">Customers need to ask their partner to help them change a reservation's initial scope.</span></span> <span data-ttu-id="7377d-210">他們也需要合作夥伴的協助，以交換、取消或更新保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-210">They also need a partner's help to exchange, cancel, or renew a reservation.</span></span> <span data-ttu-id="7377d-211">他們無法以 CSP 合作夥伴購買的訂用帳戶為基礎，執行這些工作本身的保留。</span><span class="sxs-lookup"><span data-stu-id="7377d-211">They cannot perform these tasks themselves with reservations based on subscriptions purchased for them by a CSP partner.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7377d-212">下一步</span><span class="sxs-lookup"><span data-stu-id="7377d-212">Next steps</span></span>

- [<span data-ttu-id="7377d-213">代表您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="7377d-213">Buy Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)

- [<span data-ttu-id="7377d-214">合作夥伴中心-銷售 Microsoft 保留專案</span><span class="sxs-lookup"><span data-stu-id="7377d-214">Partner Center - Sell Microsoft reservations</span></span>](azure-reservations.md)

- [<span data-ttu-id="7377d-215">代表您的客戶管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="7377d-215">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)