---
title: 將 Dynamics 365 Business Edition 優惠遷移至較新的版本 |合作夥伴中心
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將您的 Dynamics 365 Business Edition 優惠遷移至較新版本，然後再將其到期。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 優惠，續約優惠，新的 Dynamics 365 Sku
ms.openlocfilehash: 8a6ff7c10854d3b4d4a3a57482b45c741d8e0321
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943571"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="3adc8-104">將 Dynamics 365 商務版提供移轉至較新版本</span><span class="sxs-lookup"><span data-stu-id="3adc8-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span> 

<span data-ttu-id="3adc8-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="3adc8-105">**Applies to**</span></span>

- <span data-ttu-id="3adc8-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="3adc8-106">Partner Center</span></span>

<span data-ttu-id="3adc8-107">自2019年1月1日起，使用 Dynamics 365 Business Edition 訂用帳戶的客戶將無法再續約這些舊版供應專案;現有的訂閱將不會在過期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="3adc8-107">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="3adc8-108">在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日。</span><span class="sxs-lookup"><span data-stu-id="3adc8-108">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="3adc8-109">為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="3adc8-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="3adc8-110">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="3adc8-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="3adc8-111">如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="3adc8-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="3adc8-112">有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。</span><span class="sxs-lookup"><span data-stu-id="3adc8-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="3adc8-113">您可以隨時將客戶移轉至新的方案。</span><span class="sxs-lookup"><span data-stu-id="3adc8-113">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="3adc8-114">即將淘汰的 Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="3adc8-114">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="3adc8-115">Dynamics 365 for Finance and Operations，Business edition</span><span class="sxs-lookup"><span data-stu-id="3adc8-115">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="3adc8-116">Dynamics 365 的商務小組成員版本</span><span class="sxs-lookup"><span data-stu-id="3adc8-116">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="3adc8-117">Dynamics Business Central-Dynamics 365 Business Edition 的新優惠</span><span class="sxs-lookup"><span data-stu-id="3adc8-117">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="3adc8-118">透過新的 Dynamics Business Central 供應專案，您的客戶可以連接其財務、銷售、服務和營運，以簡化商務程式、改善客戶互動，並做出更好的決策。</span><span class="sxs-lookup"><span data-stu-id="3adc8-118">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="3adc8-119">Dynamics 365 Business Central 是以雲端為基礎，僅供雲端解決方案提供者（CSP）方案合作夥伴使用。</span><span class="sxs-lookup"><span data-stu-id="3adc8-119">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="3adc8-120">Dynamics 365 Business Edition 客戶有資格在2020年6月30日前獲得新的商業中心優惠折扣轉換定價。</span><span class="sxs-lookup"><span data-stu-id="3adc8-120">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="3adc8-121">將客戶轉換到新產品方案</span><span class="sxs-lookup"><span data-stu-id="3adc8-121">Transition customers to new product plans</span></span>

 <span data-ttu-id="3adc8-122">將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：</span><span class="sxs-lookup"><span data-stu-id="3adc8-122">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="3adc8-123">購買新訂閱</span><span class="sxs-lookup"><span data-stu-id="3adc8-123">Purchase the new subscription</span></span>
- <span data-ttu-id="3adc8-124">重新指派目前的使用者授權</span><span class="sxs-lookup"><span data-stu-id="3adc8-124">Reassign current user licenses</span></span>
- <span data-ttu-id="3adc8-125">取消舊訂閱</span><span class="sxs-lookup"><span data-stu-id="3adc8-125">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="3adc8-126">為您的客戶購買新方案</span><span class="sxs-lookup"><span data-stu-id="3adc8-126">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="3adc8-127">從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="3adc8-127">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="3adc8-128">選取 [**新增訂**用帳戶]。</span><span class="sxs-lookup"><span data-stu-id="3adc8-128">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="3adc8-129">選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]** 。</span><span class="sxs-lookup"><span data-stu-id="3adc8-129">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="3adc8-130">您的客戶現在會有舊的訂閱和新的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="3adc8-130">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="3adc8-131">下一個步驟是將授權重新指派給客戶的使用者。</span><span class="sxs-lookup"><span data-stu-id="3adc8-131">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="3adc8-132">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="3adc8-132">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="3adc8-133">選取 **\[使用者和授權\]** 。</span><span class="sxs-lookup"><span data-stu-id="3adc8-133">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="3adc8-134">若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="3adc8-134">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="3adc8-135">在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="3adc8-135">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="3adc8-136">選取 **\[提交\]** 。</span><span class="sxs-lookup"><span data-stu-id="3adc8-136">Select **Submit**.</span></span> <span data-ttu-id="3adc8-137">您將針對需要新授權的每位使用者執行此動作。</span><span class="sxs-lookup"><span data-stu-id="3adc8-137">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="3adc8-138">將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="3adc8-138">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="3adc8-139">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="3adc8-139">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="3adc8-140">在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="3adc8-140">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="3adc8-141">舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。</span><span class="sxs-lookup"><span data-stu-id="3adc8-141">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="3adc8-142">暫停的訂閱將在 120 天後自動解除佈建。</span><span class="sxs-lookup"><span data-stu-id="3adc8-142">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="3adc8-143">您的客戶將不會產生舊訂用帳戶的額外費用。</span><span class="sxs-lookup"><span data-stu-id="3adc8-143">Your customer will incur no additional costs for the old subscription.</span></span>
