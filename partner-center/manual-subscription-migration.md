---
title: 遷移合格的 Dynamics 365 訂閱
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何從合格的基本 Dynamics 365 訂閱遷移至新的訂用帳戶，然後再讓現有的訂閱過期。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 優惠，續約優惠，新的 Dynamics 365 Sku
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795996"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="819a4-104">將 Dynamics 365 和 Customer Engagement Plan 從基本 （合格的供應項目） 移轉至較新版本</span><span class="sxs-lookup"><span data-stu-id="819a4-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="819a4-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="819a4-105">**Applies to**</span></span>

-  <span data-ttu-id="819a4-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="819a4-106">Partner Center</span></span>

<span data-ttu-id="819a4-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="819a4-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="819a4-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="819a4-108">Global admin</span></span>
-   <span data-ttu-id="819a4-109">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="819a4-109">User admin</span></span>
-   <span data-ttu-id="819a4-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="819a4-110">Admin agent</span></span>
-   <span data-ttu-id="819a4-111">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="819a4-111">Sales agent</span></span>

<span data-ttu-id="819a4-112">自2019年1月1日起，從基本（合格供應專案）訂用帳戶使用 Dynamics 365 for Sales/Customer Engagement 方案的客戶，已無法再續約這些舊供應專案;現有的訂閱將不會在過期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="819a4-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="819a4-113">在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日]。</span><span class="sxs-lookup"><span data-stu-id="819a4-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="819a4-114">為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="819a4-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="819a4-115">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="819a4-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="819a4-116">如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="819a4-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="819a4-117">有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。</span><span class="sxs-lookup"><span data-stu-id="819a4-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="819a4-118">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="819a4-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="819a4-119">Dynamics 365 提供淘汰</span><span class="sxs-lookup"><span data-stu-id="819a4-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="819a4-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （限定供應專案）教職員版</span><span class="sxs-lookup"><span data-stu-id="819a4-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="819a4-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）適用于學生</span><span class="sxs-lookup"><span data-stu-id="819a4-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-123">Dynamics 365 for Sales Enterprise Edition （政府定價） CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-124">來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-125">適用于教職員的 Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （限定供應專案））</span><span class="sxs-lookup"><span data-stu-id="819a4-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="819a4-126">Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （合格供應專案）適用于學生）</span><span class="sxs-lookup"><span data-stu-id="819a4-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-127">來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-128">適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-129">適用于教職員的 Dynamics 365 for Sales Enterprise Edition 附加元件</span><span class="sxs-lookup"><span data-stu-id="819a4-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="819a4-130">適用于學生的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-131">適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-132">Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-133">Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價） CRMOL Basic （合格優惠）</span><span class="sxs-lookup"><span data-stu-id="819a4-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-134">適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL 基本（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-135">Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）教職員版</span><span class="sxs-lookup"><span data-stu-id="819a4-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="819a4-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-137">Dynamics 365 Customer Engagement Plan Enterprise Edition （政府定價），適用于 CRM Basic 的 SA （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-138">Dynamics 365 Customer Engagement 方案 Enterprise Edition （從 SA for CRM Basic （合格供應專案））學生專用</span><span class="sxs-lookup"><span data-stu-id="819a4-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-139">Dynamics 365 Customer Engagement 方案 Enterprise Edition，適用于教職員的 SA for CRM Basic （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="819a4-140">適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-141">適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價）附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-142">適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="819a4-143">適用于教職員的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件</span><span class="sxs-lookup"><span data-stu-id="819a4-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="819a4-144">來自基本（合格供應專案）替代方案的 Dynamics 365 for Sales/Customer Engagement 方案</span><span class="sxs-lookup"><span data-stu-id="819a4-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="819a4-145">**淘汰的優惠**</span><span class="sxs-lookup"><span data-stu-id="819a4-145">**Retired offers**</span></span>   

- <span data-ttu-id="819a4-146">來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 for Sales （合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="819a4-147">來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 Customer Engagement 方案（合格供應專案）</span><span class="sxs-lookup"><span data-stu-id="819a4-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="819a4-148">**取代選項**</span><span class="sxs-lookup"><span data-stu-id="819a4-148">**Replacement options**</span></span>
- <span data-ttu-id="819a4-149">Dynamics 365 for Sales 專業版（新）</span><span class="sxs-lookup"><span data-stu-id="819a4-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="819a4-150">Dynamics 365 for Sales 專業版（新）</span><span class="sxs-lookup"><span data-stu-id="819a4-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="819a4-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="819a4-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="819a4-152">Dynamics 365 Customer Engagement 方案或</span><span class="sxs-lookup"><span data-stu-id="819a4-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="819a4-153">Dynamics 365 團隊成員</span><span class="sxs-lookup"><span data-stu-id="819a4-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="819a4-154">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="819a4-154">Transition customers to new product plans</span></span>

<span data-ttu-id="819a4-155">將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：</span><span class="sxs-lookup"><span data-stu-id="819a4-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="819a4-156">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="819a4-156">Purchase the new subscription</span></span>
- <span data-ttu-id="819a4-157">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="819a4-157">Reassign current user licenses</span></span>
- <span data-ttu-id="819a4-158">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="819a4-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="819a4-159">為您的客戶購買新方案</span><span class="sxs-lookup"><span data-stu-id="819a4-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="819a4-160">從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="819a4-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="819a4-161">選取 [**新增訂**用帳戶]。</span><span class="sxs-lookup"><span data-stu-id="819a4-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="819a4-162">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="819a4-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="819a4-163">您的客戶現在會有舊的訂閱和新的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="819a4-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="819a4-164">下一個步驟是將授權重新指派給客戶的使用者。</span><span class="sxs-lookup"><span data-stu-id="819a4-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="819a4-165">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="819a4-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="819a4-166">選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="819a4-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="819a4-167">若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="819a4-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="819a4-168">在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="819a4-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="819a4-169">選取 [提交]  。</span><span class="sxs-lookup"><span data-stu-id="819a4-169">Select **Submit**.</span></span> <span data-ttu-id="819a4-170">您將針對需要新授權的每位使用者執行此動作。</span><span class="sxs-lookup"><span data-stu-id="819a4-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="819a4-171">將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="819a4-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="819a4-172">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="819a4-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="819a4-173">在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="819a4-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="819a4-174">舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。</span><span class="sxs-lookup"><span data-stu-id="819a4-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="819a4-175">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="819a4-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="819a4-176">您的客戶將不會產生舊訂用帳戶的額外費用。</span><span class="sxs-lookup"><span data-stu-id="819a4-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



