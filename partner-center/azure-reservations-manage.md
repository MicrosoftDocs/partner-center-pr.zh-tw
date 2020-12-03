---
title: 管理客戶的 Azure 保留
description: 瞭解如何管理客戶的 Azure 保留，包括如何取消保留、交換保留或申請退款。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534755"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a><span data-ttu-id="7367a-103">管理、取消、交換或退款 Microsoft Azure 保留給客戶</span><span class="sxs-lookup"><span data-stu-id="7367a-103">Manage, cancel, exchange, or refund Microsoft Azure reservations for customers</span></span>

<span data-ttu-id="7367a-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="7367a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7367a-105">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="7367a-105">Admin agent</span></span>
- <span data-ttu-id="7367a-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7367a-106">Global admin</span></span>
- <span data-ttu-id="7367a-107">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="7367a-107">Helpdesk agent</span></span>
- <span data-ttu-id="7367a-108">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="7367a-108">Sales agent</span></span>
- <span data-ttu-id="7367a-109">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="7367a-109">User management admin</span></span>

<span data-ttu-id="7367a-110">本文說明如何管理客戶的 Azure 保留，包括如何取消保留、交換保留或申請退款。</span><span class="sxs-lookup"><span data-stu-id="7367a-110">This article explains how to manage Azure reservations for a customer, including how to cancel a reservation, exchange a reservation, or request a refund.</span></span>

> [!NOTE]
> <span data-ttu-id="7367a-111">本文僅適用于雲端解決方案提供者 (CSP) 計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="7367a-111">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="7367a-112">使用其他類型訂用帳戶的客戶 (例如隨用隨付、個別、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀 [此 Azure 保留檔](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="7367a-112">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="7367a-113">若要在購買後管理客戶的 Azure 保留，您將在合作夥伴中心中選取您想要管理的客戶和保留，然後對 Azure 入口網站中的保留進行變更。</span><span class="sxs-lookup"><span data-stu-id="7367a-113">To manage your customers' Azure reservations post-purchase, you'll select the customer and reservation you want to manage in Partner Center, and then make changes to the reservation in the Azure portal.</span></span>

1. <span data-ttu-id="7367a-114">若要開始使用，請從 [合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取您想要管理其保留的客戶。</span><span class="sxs-lookup"><span data-stu-id="7367a-114">To get started, select **Customers** from the Partner Center menu and then select the customer whose reservations you want to manage.</span></span> 

2. <span data-ttu-id="7367a-115">在客戶的詳細資料頁面功能表上，選取 [ **Azure 保留** ]，然後選取您想要管理的特定保留。</span><span class="sxs-lookup"><span data-stu-id="7367a-115">On the customer's detail page menu, select **Azure reservations** and then select the specific reservation you want to manage.</span></span>  

3. <span data-ttu-id="7367a-116">在 [ **動作**] 底下，選取 [ **管理** ] 以移至 Azure 入口網站中客戶的保留記錄。</span><span class="sxs-lookup"><span data-stu-id="7367a-116">Under **Actions**, select **Manage** to go to the customer's reservation record in the Azure portal.</span></span> <span data-ttu-id="7367a-117">在保留區詳細資料頁面上，依照下列步驟以完成任務。</span><span class="sxs-lookup"><span data-stu-id="7367a-117">On the reservation detail page, follow the steps below to complete tasks.</span></span>  

    | <span data-ttu-id="7367a-118">**選取**</span><span class="sxs-lookup"><span data-stu-id="7367a-118">**Select**</span></span>   | <span data-ttu-id="7367a-119">**若要**</span><span class="sxs-lookup"><span data-stu-id="7367a-119">**To**</span></span>    |
    |:-----------------------------|:-----------------|
    | <span data-ttu-id="7367a-120">**概觀**</span><span class="sxs-lookup"><span data-stu-id="7367a-120">**Overview**</span></span>   | <span data-ttu-id="7367a-121">查看客戶保留的詳細資料，包括到期日、範圍和使用量資料。</span><span class="sxs-lookup"><span data-stu-id="7367a-121">View details of a customer's reservation, including expiration date, scope, and utilization data.</span></span> <span data-ttu-id="7367a-122">**注意** 選擇 **\[退款\]** 可建立按比例計算的退款支援要求。</span><span class="sxs-lookup"><span data-stu-id="7367a-122">**NOTE** Select **Refund** to create a support request for a pro-rated refund.</span></span> <span data-ttu-id="7367a-123">選取 **\[交換\]** 可建立交換未使用的保留區期限的支援要求。</span><span class="sxs-lookup"><span data-stu-id="7367a-123">Select **Exchange** to create a support request to exchange the unused portion of your reservation term.</span></span>  
    | <span data-ttu-id="7367a-124">**存取控制 (IAM)**</span><span class="sxs-lookup"><span data-stu-id="7367a-124">**Access Control (IAM)**</span></span>   | <span data-ttu-id="7367a-125">管理客戶保留資訊的存取權。</span><span class="sxs-lookup"><span data-stu-id="7367a-125">Manage access to the customer's reservation information.</span></span>|
    | <span data-ttu-id="7367a-126">**設定**</span><span class="sxs-lookup"><span data-stu-id="7367a-126">**Configuration**</span></span>   | <span data-ttu-id="7367a-127">變更保留的範圍及/或與保留相關聯的 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7367a-127">Change the reservation's scope and/or the Azure subscription the reservation is associated with.</span></span>    |
    | <span data-ttu-id="7367a-128">**屬性**</span><span class="sxs-lookup"><span data-stu-id="7367a-128">**Properties**</span></span>   | <span data-ttu-id="7367a-129">查看保留的屬性，並將保留識別碼和保留訂單識別碼複製到剪貼簿。</span><span class="sxs-lookup"><span data-stu-id="7367a-129">View the reservation's properties and copy to the clipboard the reservation ID and reservation order ID.</span></span> <span data-ttu-id="7367a-130">**注意** 當您代表客戶要求支援時，支援人員可能會請您提供保留區識別碼和保留區訂單識別碼。</span><span class="sxs-lookup"><span data-stu-id="7367a-130">**NOTE** Support may ask you for the reservation ID and reservation order ID when you request support on behalf of a customer.</span></span>    |
    | <span data-ttu-id="7367a-131">**新增支援要求**</span><span class="sxs-lookup"><span data-stu-id="7367a-131">**New support request**</span></span>    | <span data-ttu-id="7367a-132">向 Microsoft 支援服務要求協助。</span><span class="sxs-lookup"><span data-stu-id="7367a-132">Request help from Microsoft Support.</span></span>   |
 
## <a name="cancel-or-exchange-a-reservation"></a><span data-ttu-id="7367a-133">取消或交換保留區</span><span class="sxs-lookup"><span data-stu-id="7367a-133">Cancel or exchange a reservation</span></span>

<span data-ttu-id="7367a-134">如果客戶的商務需求有所改變，他們可能會想要取消保留，並取得退款或交換保留的按比例退款金額，以用於新的保留。</span><span class="sxs-lookup"><span data-stu-id="7367a-134">If at any point a customer's business needs change, they may want to cancel a reservation and get a refund or exchange a reservation's prorated refund amount to be used toward the price of a new reservation.</span></span>

<span data-ttu-id="7367a-135">在這兩種情況下，Microsoft 會退款給您，讓您可以管理客戶所產生的財務交易。</span><span class="sxs-lookup"><span data-stu-id="7367a-135">In both of these scenarios, Microsoft refunds the amount to you so that you can then manage the resulting financial transactions with your customers.</span></span> <span data-ttu-id="7367a-136">Microsoft 不會直接與客戶聯繫帳單、取消或退款。</span><span class="sxs-lookup"><span data-stu-id="7367a-136">Microsoft does not contact customers directly about billing, cancellations, or refunds.</span></span>

### <a name="how-cancellations-work"></a><span data-ttu-id="7367a-137">取消的運作方式</span><span class="sxs-lookup"><span data-stu-id="7367a-137">How cancellations work</span></span>

<span data-ttu-id="7367a-138">客戶隨時都可以要求取消保留， (每年 $50000 上限的退款金額) 。</span><span class="sxs-lookup"><span data-stu-id="7367a-138">Customers can request to cancel a reservation at any time (refund amount capped at $50,000 per year).</span></span> <span data-ttu-id="7367a-139">取消保留可讓客戶傳回 Azure 保留的剩餘月份數量，以獲得提早終止費用。</span><span class="sxs-lookup"><span data-stu-id="7367a-139">Canceling a reservation allows the customer to return the amount of the remaining months of an Azure reservation for an early termination fee.</span></span> <span data-ttu-id="7367a-140">剩餘的計費餘額（減去提早終止費）會退款給您的帳戶，讓您可以退款客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="7367a-140">The remaining prorated balance, minus the early termination fee, is refunded to your account so that you can refund the customer's account.</span></span> 

<span data-ttu-id="7367a-141">請參閱下方的取消詳細資料和費用。</span><span class="sxs-lookup"><span data-stu-id="7367a-141">See below for cancellation details and fees.</span></span>


|<span data-ttu-id="7367a-142">**取消日期**</span><span class="sxs-lookup"><span data-stu-id="7367a-142">**Cancellation date**</span></span><br> <span data-ttu-id="7367a-143"> (天) </span><span class="sxs-lookup"><span data-stu-id="7367a-143">(days)</span></span>   |<span data-ttu-id="7367a-144">**使用方式**</span><span class="sxs-lookup"><span data-stu-id="7367a-144">**Usage**</span></span>    |<span data-ttu-id="7367a-145">**點數**</span><span class="sxs-lookup"><span data-stu-id="7367a-145">**Credit**</span></span>  |<span data-ttu-id="7367a-146">**提早終止**</span><span class="sxs-lookup"><span data-stu-id="7367a-146">**Early termination**</span></span><br> <span data-ttu-id="7367a-147">費用</span><span class="sxs-lookup"><span data-stu-id="7367a-147">fee</span></span>    |<span data-ttu-id="7367a-148">**退款上限**</span><span class="sxs-lookup"><span data-stu-id="7367a-148">**Refund cap**</span></span> | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|<span data-ttu-id="7367a-149">5或更少</span><span class="sxs-lookup"><span data-stu-id="7367a-149">5 or fewer</span></span>                         | <span data-ttu-id="7367a-150">否</span><span class="sxs-lookup"><span data-stu-id="7367a-150">No</span></span>          | <span data-ttu-id="7367a-151">100%</span><span class="sxs-lookup"><span data-stu-id="7367a-151">100%</span></span>       | <span data-ttu-id="7367a-152">否</span><span class="sxs-lookup"><span data-stu-id="7367a-152">No</span></span>                              | <span data-ttu-id="7367a-153">$50000 美元</span><span class="sxs-lookup"><span data-stu-id="7367a-153">$50,000 USD</span></span>   |
|<span data-ttu-id="7367a-154">5或更少</span><span class="sxs-lookup"><span data-stu-id="7367a-154">5 or fewer</span></span>                         | <span data-ttu-id="7367a-155">是</span><span class="sxs-lookup"><span data-stu-id="7367a-155">Yes</span></span>         | <span data-ttu-id="7367a-156">依比例</span><span class="sxs-lookup"><span data-stu-id="7367a-156">Pro-rated</span></span>  | <span data-ttu-id="7367a-157">否</span><span class="sxs-lookup"><span data-stu-id="7367a-157">No</span></span>                              | <span data-ttu-id="7367a-158">$50000 美元</span><span class="sxs-lookup"><span data-stu-id="7367a-158">$50,000 USD</span></span>   |
|<span data-ttu-id="7367a-159">超過5個</span><span class="sxs-lookup"><span data-stu-id="7367a-159">More than 5</span></span>                        | <span data-ttu-id="7367a-160">否</span><span class="sxs-lookup"><span data-stu-id="7367a-160">No</span></span>          | <span data-ttu-id="7367a-161">依比例</span><span class="sxs-lookup"><span data-stu-id="7367a-161">Pro-rated</span></span>  | <span data-ttu-id="7367a-162">12%</span><span class="sxs-lookup"><span data-stu-id="7367a-162">12%</span></span>                             | <span data-ttu-id="7367a-163">$50000 美元</span><span class="sxs-lookup"><span data-stu-id="7367a-163">$50,000 USD</span></span>   |
|<span data-ttu-id="7367a-164">超過5個</span><span class="sxs-lookup"><span data-stu-id="7367a-164">More than 5</span></span>                        | <span data-ttu-id="7367a-165">是</span><span class="sxs-lookup"><span data-stu-id="7367a-165">Yes</span></span>         | <span data-ttu-id="7367a-166">依比例</span><span class="sxs-lookup"><span data-stu-id="7367a-166">Pro-rated</span></span>  | <span data-ttu-id="7367a-167">12%</span><span class="sxs-lookup"><span data-stu-id="7367a-167">12%</span></span>                             | <span data-ttu-id="7367a-168">$50000 美元</span><span class="sxs-lookup"><span data-stu-id="7367a-168">$50,000 USD</span></span>   |

### <a name="how-exchanges-work"></a><span data-ttu-id="7367a-169">交換的運作方式</span><span class="sxs-lookup"><span data-stu-id="7367a-169">How exchanges work</span></span> 

<span data-ttu-id="7367a-170">如果客戶想要購買的保留量與您原本向您購買的不同，他們可以要求交換。</span><span class="sxs-lookup"><span data-stu-id="7367a-170">If a customer wants to buy a different reservation than the one they originally bought from you, they can request an exchange.</span></span> <span data-ttu-id="7367a-171">交換保留可能是取消保留的好方法，因為它可讓客戶使用按比例計算的退款金額來接近新的保留價格。</span><span class="sxs-lookup"><span data-stu-id="7367a-171">Exchanging a reservation can be an attractive alternative to canceling a reservation because it allows the customer to use the prorated refund amount toward the price of the new reservation.</span></span> 

<span data-ttu-id="7367a-172">按比例計算的退款金額會折算到您的帳戶，讓您可以為客戶提供交換。</span><span class="sxs-lookup"><span data-stu-id="7367a-172">The prorated refund amount is credited to your account so that you can offer the customer an exchange.</span></span>

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a><span data-ttu-id="7367a-173">代表客戶要求退款或交換</span><span class="sxs-lookup"><span data-stu-id="7367a-173">Request a refund or exchange on behalf of a customer</span></span>

<span data-ttu-id="7367a-174">若要代表客戶提出退款或交換的支援要求，請在合作夥伴中心中選取客戶和保留，然後在 Azure 入口網站中建立支援要求。</span><span class="sxs-lookup"><span data-stu-id="7367a-174">To file a support request for a refund or exchange on behalf of your customers, you'll select the customer and reservation in Partner Center, and then create the support request in the Azure portal.</span></span> 

>[!NOTE]
><span data-ttu-id="7367a-175">Microsoft 支援服務專員可能會請您提供保留區識別碼和保留區訂單識別碼。</span><span class="sxs-lookup"><span data-stu-id="7367a-175">Microsoft Support agents may ask you to provide the reservation ID and reservation order ID.</span></span> <span data-ttu-id="7367a-176">您可以在 Azure 入口網站的保留的 [內容 **] 頁面上** 找到這項資訊。</span><span class="sxs-lookup"><span data-stu-id="7367a-176">You can find this information on the reservation's **Properties** page in the Azure portal.</span></span>

1. <span data-ttu-id="7367a-177">若要開始使用，請從 [合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取想要退款的客戶。</span><span class="sxs-lookup"><span data-stu-id="7367a-177">To get started, select **Customers** from the Partner Center menu and then select the customer who wants a refund.</span></span> 

2. <span data-ttu-id="7367a-178">在客戶的詳細資料頁面上，選取 [ **Azure 保留** ]，然後選取客戶想要退款的特定保留。</span><span class="sxs-lookup"><span data-stu-id="7367a-178">On the customer's detail page, select **Azure reservations** and then select the specific reservation the customer wants refunded.</span></span>  

3. <span data-ttu-id="7367a-179">在 [ **動作**] 底下，選取 [ **退款** ] 以移至 Azure 入口網站中的客戶保留記錄，並起始支援要求。</span><span class="sxs-lookup"><span data-stu-id="7367a-179">Under **Actions**, select **Refund** to go to the customer's reservation record in the Azure portal and initiate a support request.</span></span>  

4. <span data-ttu-id="7367a-180">在 **\[新的支援要求\]** 頁面上，依照下列步驟來要求退款。</span><span class="sxs-lookup"><span data-stu-id="7367a-180">On the **New support request** page, follow the steps below to request a refund.</span></span> <span data-ttu-id="7367a-181">每個步驟之後選取 **\[下一步\]**。</span><span class="sxs-lookup"><span data-stu-id="7367a-181">Select **Next** after each step.</span></span> 

   |<span data-ttu-id="7367a-182">**Step**</span><span class="sxs-lookup"><span data-stu-id="7367a-182">**Step**</span></span>                    |<span data-ttu-id="7367a-183">**選項**</span><span class="sxs-lookup"><span data-stu-id="7367a-183">**Selections**</span></span>    |
   |:---------------------------|:-----------------|
   |<span data-ttu-id="7367a-184">**1個基本概念**</span><span class="sxs-lookup"><span data-stu-id="7367a-184">**1 Basics**</span></span>                |<span data-ttu-id="7367a-185">問題類型：計費</span><span class="sxs-lookup"><span data-stu-id="7367a-185">Issue type: Billing.</span></span>  |
   |<span data-ttu-id="7367a-186">**2 問題**</span><span class="sxs-lookup"><span data-stu-id="7367a-186">**2 Problem**</span></span>               |<span data-ttu-id="7367a-187">問題類型︰ 保留區管理。</span><span class="sxs-lookup"><span data-stu-id="7367a-187">Problem type: Reservation management.</span></span> <span data-ttu-id="7367a-188">分類：交換與退款。</span><span class="sxs-lookup"><span data-stu-id="7367a-188">Category: Exchanges and refunds.</span></span> |
   |<span data-ttu-id="7367a-189">**3 連絡人資訊**</span><span class="sxs-lookup"><span data-stu-id="7367a-189">**3 Contact information**</span></span>   |<span data-ttu-id="7367a-190">選取您的喜好設定，然後輸入所需的資訊。</span><span class="sxs-lookup"><span data-stu-id="7367a-190">Select your preferences and enter the required information.</span></span> 

5. <span data-ttu-id="7367a-191">完成後選取 [建立]。</span><span class="sxs-lookup"><span data-stu-id="7367a-191">Select **Create** when done.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="7367a-192">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="7367a-192">Azure reservations resources</span></span>

|<span data-ttu-id="7367a-193">**如需下列資訊**</span><span class="sxs-lookup"><span data-stu-id="7367a-193">**For information about**</span></span>   |<span data-ttu-id="7367a-194">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="7367a-194">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="7367a-195">雲端解決方案提供者中的 Azure Reservations 概觀</span><span class="sxs-lookup"><span data-stu-id="7367a-195">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="7367a-196">銷售 Microsoft Azure 保留的執行個體</span><span class="sxs-lookup"><span data-stu-id="7367a-196">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="7367a-197">在合作夥伴中心中為您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="7367a-197">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="7367a-198">購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="7367a-198">Buy Azure reservations</span></span>](azure-reservations-buying.md) |
|<span data-ttu-id="7367a-199">判斷正確的 VM 大小，並確認客戶 VM 使用率</span><span class="sxs-lookup"><span data-stu-id="7367a-199">Determine the correct VM size and verify customer VM usage</span></span>   | [<span data-ttu-id="7367a-200">調整 VM 大小以提供最大 Azure Reservations 使用率</span><span class="sxs-lookup"><span data-stu-id="7367a-200">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="7367a-201">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="7367a-201">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="7367a-202">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="7367a-202">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="7367a-203">提供客戶從您購買的訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="7367a-203">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="7367a-204">提供客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="7367a-204">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |