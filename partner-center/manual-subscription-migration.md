---
title: 遷移合格的 Dynamics 365 訂閱
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何從合格的基本 Dynamics 365 訂閱遷移至新的訂用帳戶，然後再讓現有的訂閱過期。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8575d87ab3c4c7970135a87b7ef7564c4fe06232
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436847"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="839cc-103">將 Dynamics 365 和 Customer Engagement Plan 從基本 （合格的供應項目） 移轉至較新版本</span><span class="sxs-lookup"><span data-stu-id="839cc-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="839cc-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="839cc-104">**Applies to**</span></span>

-  <span data-ttu-id="839cc-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="839cc-105">Partner Center</span></span>

<span data-ttu-id="839cc-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="839cc-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="839cc-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="839cc-107">Global admin</span></span>
-   <span data-ttu-id="839cc-108">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="839cc-108">User admin</span></span>
-   <span data-ttu-id="839cc-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="839cc-109">Admin agent</span></span>
-   <span data-ttu-id="839cc-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="839cc-110">Sales agent</span></span>

<span data-ttu-id="839cc-111">自2019年1月1日起，從基本（合格供應專案）訂用帳戶使用 Dynamics 365 for Sales/Customer Engagement 方案的客戶，已無法再續約這些舊供應專案;現有的訂閱將不會在過期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="839cc-111">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="839cc-112">在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日]。</span><span class="sxs-lookup"><span data-stu-id="839cc-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="839cc-113">為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="839cc-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="839cc-114">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="839cc-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="839cc-115">如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="839cc-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="839cc-116">有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。</span><span class="sxs-lookup"><span data-stu-id="839cc-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="839cc-117">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="839cc-117">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="839cc-118">Dynamics 365 提供淘汰</span><span class="sxs-lookup"><span data-stu-id="839cc-118">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="839cc-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （限定供應專案）教職員版</span><span class="sxs-lookup"><span data-stu-id="839cc-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="839cc-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）適用于學生</span><span class="sxs-lookup"><span data-stu-id="839cc-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-122">Dynamics 365 for Sales Enterprise Edition （政府定價） CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-123">來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-124">適用于教職員的 Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （限定供應專案））</span><span class="sxs-lookup"><span data-stu-id="839cc-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="839cc-125">Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （合格供應專案）適用于學生）</span><span class="sxs-lookup"><span data-stu-id="839cc-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-126">來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-127">適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-128">適用于教職員的 Dynamics 365 for Sales Enterprise Edition 附加元件</span><span class="sxs-lookup"><span data-stu-id="839cc-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="839cc-129">適用于學生的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-130">適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-130">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-131">Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-132">Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價） CRMOL Basic （合格優惠）</span><span class="sxs-lookup"><span data-stu-id="839cc-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-133">適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL 基本（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-133">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-134">Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）教職員版</span><span class="sxs-lookup"><span data-stu-id="839cc-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="839cc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition （政府定價），適用于 CRM Basic 的 SA （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-137">Dynamics 365 Customer Engagement 方案 Enterprise Edition （從 SA for CRM Basic （合格供應專案））學生專用</span><span class="sxs-lookup"><span data-stu-id="839cc-137">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-138">Dynamics 365 Customer Engagement 方案 Enterprise Edition，適用于教職員的 SA for CRM Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="839cc-139">適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-140">適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價）附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-140">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-141">適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-141">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="839cc-142">適用于教職員的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件</span><span class="sxs-lookup"><span data-stu-id="839cc-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="839cc-143">來自基本（合格供應專案）替代方案的 Dynamics 365 for Sales/Customer Engagement 方案</span><span class="sxs-lookup"><span data-stu-id="839cc-143">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="839cc-144">**淘汰的優惠**</span><span class="sxs-lookup"><span data-stu-id="839cc-144">**Retired offers**</span></span>   

- <span data-ttu-id="839cc-145">來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 for Sales （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-145">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="839cc-146">來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 Customer Engagement 方案（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="839cc-146">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="839cc-147">**取代選項**</span><span class="sxs-lookup"><span data-stu-id="839cc-147">**Replacement options**</span></span>
- <span data-ttu-id="839cc-148">Dynamics 365 for Sales 專業版（新）</span><span class="sxs-lookup"><span data-stu-id="839cc-148">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="839cc-149">Dynamics 365 for Sales 專業版（新）</span><span class="sxs-lookup"><span data-stu-id="839cc-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="839cc-150">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="839cc-150">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="839cc-151">Dynamics 365 Customer Engagement 方案或</span><span class="sxs-lookup"><span data-stu-id="839cc-151">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="839cc-152">Dynamics 365 團隊成員</span><span class="sxs-lookup"><span data-stu-id="839cc-152">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="839cc-153">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="839cc-153">Transition customers to new product plans</span></span>

<span data-ttu-id="839cc-154">將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：</span><span class="sxs-lookup"><span data-stu-id="839cc-154">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="839cc-155">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="839cc-155">Purchase the new subscription</span></span>
- <span data-ttu-id="839cc-156">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="839cc-156">Reassign current user licenses</span></span>
- <span data-ttu-id="839cc-157">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="839cc-157">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="839cc-158">為您的客戶購買新方案</span><span class="sxs-lookup"><span data-stu-id="839cc-158">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="839cc-159">從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="839cc-159">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="839cc-160">選取 [**新增訂**用帳戶]。</span><span class="sxs-lookup"><span data-stu-id="839cc-160">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="839cc-161">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="839cc-161">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="839cc-162">您的客戶現在會有舊的訂閱和新的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="839cc-162">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="839cc-163">下一個步驟是將授權重新指派給客戶的使用者。</span><span class="sxs-lookup"><span data-stu-id="839cc-163">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="839cc-164">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="839cc-164">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="839cc-165">選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="839cc-165">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="839cc-166">若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="839cc-166">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="839cc-167">在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="839cc-167">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="839cc-168">選取 [提交]。</span><span class="sxs-lookup"><span data-stu-id="839cc-168">Select **Submit**.</span></span> <span data-ttu-id="839cc-169">您將針對需要新授權的每位使用者執行此動作。</span><span class="sxs-lookup"><span data-stu-id="839cc-169">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="839cc-170">將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="839cc-170">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="839cc-171">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="839cc-171">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="839cc-172">在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="839cc-172">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="839cc-173">舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。</span><span class="sxs-lookup"><span data-stu-id="839cc-173">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="839cc-174">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="839cc-174">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="839cc-175">您的客戶將不會產生舊訂用帳戶的額外費用。</span><span class="sxs-lookup"><span data-stu-id="839cc-175">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



