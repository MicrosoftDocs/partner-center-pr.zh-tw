---
title: 遷移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將合格的 Dynamics 365 Business Edition 供應專案在到期前遷移至較新的版本。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436827"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="87954-103">將 Dynamics 365 商務版提供移轉至較新版本</span><span class="sxs-lookup"><span data-stu-id="87954-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="87954-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="87954-104">**Applies to**</span></span>

- <span data-ttu-id="87954-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="87954-105">Partner Center</span></span>

<span data-ttu-id="87954-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="87954-106">**Appropriate roles**</span></span>
- <span data-ttu-id="87954-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="87954-107">Global admin</span></span>
- <span data-ttu-id="87954-108">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="87954-108">User admin</span></span>
- <span data-ttu-id="87954-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="87954-109">Admin agent</span></span>
- <span data-ttu-id="87954-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="87954-110">Sales agent</span></span>

<span data-ttu-id="87954-111">自2019年1月1日起，使用 Dynamics 365 Business Edition 訂用帳戶的客戶將無法再續約這些舊版供應專案;現有的訂閱將不會在過期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="87954-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="87954-112">在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日]。</span><span class="sxs-lookup"><span data-stu-id="87954-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="87954-113">為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="87954-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="87954-114">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="87954-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="87954-115">如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="87954-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="87954-116">有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。</span><span class="sxs-lookup"><span data-stu-id="87954-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="87954-117">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="87954-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="87954-118">即將淘汰的 Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="87954-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="87954-119">Dynamics 365 for Finance and Operations，Business edition</span><span class="sxs-lookup"><span data-stu-id="87954-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="87954-120">Dynamics 365 的商務小組成員版本</span><span class="sxs-lookup"><span data-stu-id="87954-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="87954-121">Dynamics Business Central-Dynamics 365 Business Edition 的新優惠</span><span class="sxs-lookup"><span data-stu-id="87954-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="87954-122">透過新的 Dynamics Business Central 供應專案，您的客戶可以連接其財務、銷售、服務和營運，以簡化商務程式、改善客戶互動，並做出更好的決策。</span><span class="sxs-lookup"><span data-stu-id="87954-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="87954-123">Dynamics 365 Business Central 是以雲端為基礎，僅供雲端解決方案提供者（CSP）方案合作夥伴使用。</span><span class="sxs-lookup"><span data-stu-id="87954-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="87954-124">Dynamics 365 Business Edition 客戶有資格在2020年6月30日前獲得新的商業中心優惠折扣轉換定價。</span><span class="sxs-lookup"><span data-stu-id="87954-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="87954-125">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="87954-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="87954-126">將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：</span><span class="sxs-lookup"><span data-stu-id="87954-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="87954-127">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="87954-127">Purchase the new subscription</span></span>
- <span data-ttu-id="87954-128">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="87954-128">Reassign current user licenses</span></span>
- <span data-ttu-id="87954-129">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="87954-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="87954-130">為您的客戶購買新方案</span><span class="sxs-lookup"><span data-stu-id="87954-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="87954-131">從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="87954-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="87954-132">選取 [**新增訂**用帳戶]。</span><span class="sxs-lookup"><span data-stu-id="87954-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="87954-133">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="87954-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="87954-134">您的客戶現在會有舊的訂閱和新的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="87954-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="87954-135">下一個步驟是將授權重新指派給客戶的使用者。</span><span class="sxs-lookup"><span data-stu-id="87954-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="87954-136">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="87954-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="87954-137">選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="87954-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="87954-138">若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="87954-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="87954-139">在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="87954-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="87954-140">選取 [提交]。</span><span class="sxs-lookup"><span data-stu-id="87954-140">Select **Submit**.</span></span> <span data-ttu-id="87954-141">您將針對需要新授權的每位使用者執行此動作。</span><span class="sxs-lookup"><span data-stu-id="87954-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="87954-142">將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="87954-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="87954-143">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="87954-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="87954-144">在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="87954-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="87954-145">舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。</span><span class="sxs-lookup"><span data-stu-id="87954-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="87954-146">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="87954-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="87954-147">您的客戶將不會產生舊訂用帳戶的額外費用。</span><span class="sxs-lookup"><span data-stu-id="87954-147">Your customer will incur no additional costs for the old subscription.</span></span>
