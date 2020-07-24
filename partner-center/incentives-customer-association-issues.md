---
title: 客戶關聯問題
description: 瞭解如何解決使用已宣告的記錄夥伴（CPOR）客戶關聯時所出現的問題。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: 63138dd6eaa16534cb73f41655ba728cb0c7a430
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114523"
---
# <a name="customer-association-issues"></a><span data-ttu-id="e1530-103">客戶關聯問題</span><span class="sxs-lookup"><span data-stu-id="e1530-103">Customer association issues</span></span>

<span data-ttu-id="e1530-104">適用於︰</span><span class="sxs-lookup"><span data-stu-id="e1530-104">Applies to:</span></span>

- <span data-ttu-id="e1530-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e1530-105">Partner Center</span></span>

<span data-ttu-id="e1530-106">下列內容將協助您解決當您使用客戶關聯時可能會出現的問題。</span><span class="sxs-lookup"><span data-stu-id="e1530-106">The content below will help you solve issues that can come up when you work with customer associations.</span></span>

<span data-ttu-id="e1530-107">適當的角色：</span><span class="sxs-lookup"><span data-stu-id="e1530-107">Appropriate roles:</span></span>

- <span data-ttu-id="e1530-108">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="e1530-108">Billing admin</span></span>
- <span data-ttu-id="e1530-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="e1530-109">Global admin</span></span>
- <span data-ttu-id="e1530-110">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="e1530-110">Incentives admin</span></span>

## <a name="domain-tenant-mismatch"></a><span data-ttu-id="e1530-111">網域-租使用者不符</span><span class="sxs-lookup"><span data-stu-id="e1530-111">Domain-tenant mismatch</span></span>

<span data-ttu-id="e1530-112">在領取的記錄（CPOR）關聯宣告流程合作夥伴中，系統會要求您提供客戶租使用者識別碼和子域。</span><span class="sxs-lookup"><span data-stu-id="e1530-112">In the Claimed Partner of Record (CPOR) association claim flow, you will be asked to provide the customer tenant ID and subdomain.</span></span> <span data-ttu-id="e1530-113">如果您收到錯誤訊息，指出它們不相符，請洽詢您的客戶，以確保您有正確的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="e1530-113">If you receive an error stating that they don’t match, contact your customer to ensure you have the correct details.</span></span>

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a><span data-ttu-id="e1530-114">CPOR 關聯宣告流程中的訂用帳戶錯誤</span><span class="sxs-lookup"><span data-stu-id="e1530-114">Subscription errors in the CPOR association claim flow</span></span>

<span data-ttu-id="e1530-115">在 CPOR 關聯宣告流程中，系統可能會要求您透過 Business Applications （Dynamics 365）為您嘗試宣告的產品提供訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="e1530-115">In the CPOR association claim flow, you may be asked to provide a subscription for a product that you're trying to claim via Business Applications (Dynamics 365).</span></span> <span data-ttu-id="e1530-116">我們會要求您提供訂用帳戶，因為我們會動態檢查產品和訂用帳戶是否屬於所宣告的租使用者。</span><span class="sxs-lookup"><span data-stu-id="e1530-116">We ask for the subscription because we're dynamically checking that the product and subscription belong to the tenant being claimed for.</span></span> <span data-ttu-id="e1530-117">我們也正在檢查訂用帳戶是否為使用中/處於「寬限期」狀態。</span><span class="sxs-lookup"><span data-stu-id="e1530-117">We're also checking that the subscription is in active/in grace status.</span></span>

<span data-ttu-id="e1530-118">如果您收到錯誤，可能有幾個原因：</span><span class="sxs-lookup"><span data-stu-id="e1530-118">If you receive the error, it could be for several reasons:</span></span>

- <span data-ttu-id="e1530-119">選取的產品不存在於客戶的租用戶上</span><span class="sxs-lookup"><span data-stu-id="e1530-119">The product selected doesn’t exist on the customer’s tenant</span></span>
- <span data-ttu-id="e1530-120">提供的訂用帳戶不適用於 Dynamics</span><span class="sxs-lookup"><span data-stu-id="e1530-120">The subscription provided isn't for Dynamics</span></span>
- <span data-ttu-id="e1530-121">提供的訂閱適用於 CSP</span><span class="sxs-lookup"><span data-stu-id="e1530-121">The subscription provided is for CSP</span></span>
- <span data-ttu-id="e1530-122">客戶尚未啟用/布建該訂用帳戶的產品</span><span class="sxs-lookup"><span data-stu-id="e1530-122">The customer hasn't yet activated/provisioned the products for that subscription</span></span>
- <span data-ttu-id="e1530-123">該訂閱已經宣告過</span><span class="sxs-lookup"><span data-stu-id="e1530-123">The subscription has already been claimed</span></span>
- <span data-ttu-id="e1530-124">提供的識別碼不是訂用帳戶 ID</span><span class="sxs-lookup"><span data-stu-id="e1530-124">The identifier provided isn't a subscription ID</span></span>

<span data-ttu-id="e1530-125">如果您有關于訂用帳戶精確度的問題，請與您的客戶合作，以確保訂用帳戶正確，且您使用的是正確的租使用者識別碼。</span><span class="sxs-lookup"><span data-stu-id="e1530-125">If you have a question about the accuracy of your subscription, work with your customer to ensure the subscription is correct and that you're using the correct tenant ID.</span></span>

<span data-ttu-id="e1530-126">如果此路由尚未解決您的問題，請聯絡[支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。</span><span class="sxs-lookup"><span data-stu-id="e1530-126">If this route hasn't resolved your issue, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="when-subscriptions-will-be-available-to-claim"></a><span data-ttu-id="e1530-127">當訂閱將可供宣告</span><span class="sxs-lookup"><span data-stu-id="e1530-127">When subscriptions will be available to claim</span></span>

<span data-ttu-id="e1530-128">在宣告訂用帳戶時，如果尚未布建訂用帳戶，您將會收到錯誤。</span><span class="sxs-lookup"><span data-stu-id="e1530-128">When claiming for a subscription, you will receive an error if the subscription hasn't been provisioned yet.</span></span> <span data-ttu-id="e1530-129">客戶必須採取幾個步驟，訂用帳戶才可供 CPOR 平臺進行挑選，並使其可供索取。</span><span class="sxs-lookup"><span data-stu-id="e1530-129">There are several steps the customer needs to take for the subscription to become available for the CPOR platform to pick it up and make it available to claim.</span></span> <span data-ttu-id="e1530-130">如果您在嘗試宣告訂用帳戶時收到錯誤，請洽詢您的客戶，確保其已布建，且您所索取的訂用帳戶正確無誤。</span><span class="sxs-lookup"><span data-stu-id="e1530-130">If you're receiving an error when trying to claim a subscription, contact your customer to ensure that it has been provisioned and the subscription you're claiming is correct.</span></span> <span data-ttu-id="e1530-131">如果您已經取得此路由，請聯絡[支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。</span><span class="sxs-lookup"><span data-stu-id="e1530-131">If you have taken this route already, contact [support](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).</span></span>

## <a name="which-activity-do-i-choose"></a><span data-ttu-id="e1530-132">我要選擇哪一個活動？</span><span class="sxs-lookup"><span data-stu-id="e1530-132">Which activity do I choose?</span></span>

<span data-ttu-id="e1530-133">CPOR 聲稱平臺允許與 Business Applications 和 Microsoft 365 解決方案區域相關的 CPOR 關聯宣告。</span><span class="sxs-lookup"><span data-stu-id="e1530-133">The CPOR claiming platform allows for CPOR association claims related to Business Applications and Microsoft 365 solution areas.</span></span> <span data-ttu-id="e1530-134">適用于每個解決方案區域的活動如下。</span><span class="sxs-lookup"><span data-stu-id="e1530-134">The activities that are applicable to each solution area are below.</span></span> <span data-ttu-id="e1530-135">根據描述來選取正確的活動，以避免未來需要回收。</span><span class="sxs-lookup"><span data-stu-id="e1530-135">Select the correct activity based on the descriptions to avoid having to reclaim in the future.</span></span> <span data-ttu-id="e1530-136">宣告不正確的活動可能會導致缺少資格和獎勵收益。</span><span class="sxs-lookup"><span data-stu-id="e1530-136">Claiming with an incorrect activity may result in missed eligibility and incentive earnings.</span></span>


| <span data-ttu-id="e1530-137">解決方案領域</span><span class="sxs-lookup"><span data-stu-id="e1530-137">Solution area</span></span> | <span data-ttu-id="e1530-138">活動</span><span class="sxs-lookup"><span data-stu-id="e1530-138">Activity</span></span> | <span data-ttu-id="e1530-139">適用于</span><span class="sxs-lookup"><span data-stu-id="e1530-139">Applicable for</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="e1530-140">商務應用程式</span><span class="sxs-lookup"><span data-stu-id="e1530-140">Business applications</span></span>      | <span data-ttu-id="e1530-141">售前</span><span class="sxs-lookup"><span data-stu-id="e1530-141">Presales</span></span>   | <span data-ttu-id="e1530-142">如果您影響其購買合格產品，而且想要申請售前獎勵，請選取此項。</span><span class="sxs-lookup"><span data-stu-id="e1530-142">Select if you influenced their purchase of an eligible product, and want to apply for pre-sale incentives.</span></span> <span data-ttu-id="e1530-143">只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。</span><span class="sxs-lookup"><span data-stu-id="e1530-143">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    |  <span data-ttu-id="e1530-144">使用方式</span><span class="sxs-lookup"><span data-stu-id="e1530-144">Usage</span></span>  | <span data-ttu-id="e1530-145">如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。</span><span class="sxs-lookup"><span data-stu-id="e1530-145">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> <span data-ttu-id="e1530-146">只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。</span><span class="sxs-lookup"><span data-stu-id="e1530-146">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span> |
|    | <span data-ttu-id="e1530-147">收益關聯</span><span class="sxs-lookup"><span data-stu-id="e1530-147">Revenue association</span></span>   | <span data-ttu-id="e1530-148">如果您將其合格產品的選取範圍影響為商業影響因素，請選取此選項。</span><span class="sxs-lookup"><span data-stu-id="e1530-148">Select if you influenced their selection of an eligible product as a Business Influencer.</span></span> <span data-ttu-id="e1530-149">此選項僅適用于收益關聯，而不是獎勵付款。</span><span class="sxs-lookup"><span data-stu-id="e1530-149">This option is for revenue association only, not for incentive payments.</span></span> <span data-ttu-id="e1530-150">只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。</span><span class="sxs-lookup"><span data-stu-id="e1530-150">This option is only applicable if the customer purchased these products via Volume Licensing agreement or Web-Direct.</span></span>   |
| <span data-ttu-id="e1530-151">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e1530-151">Microsoft 365</span></span>   | <span data-ttu-id="e1530-152">使用方式</span><span class="sxs-lookup"><span data-stu-id="e1530-152">Usage</span></span>   | <span data-ttu-id="e1530-153">如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。</span><span class="sxs-lookup"><span data-stu-id="e1530-153">Select if you drive their adoption and usage of an eligible workload, and want to apply for usage incentives.</span></span> |

## <a name="which-mpn-do-i-choose"></a><span data-ttu-id="e1530-154">我要選擇哪一種 MPN？</span><span class="sxs-lookup"><span data-stu-id="e1530-154">Which MPN do I choose?</span></span>

<span data-ttu-id="e1530-155">在 CPOR 關聯宣告流程中，系統會要求您選擇應該與您在終端客戶所宣稱之工作相關聯的公司 MPN。</span><span class="sxs-lookup"><span data-stu-id="e1530-155">In the CPOR association claim flow, you will be asked to choose a company MPN that should be associated to the work you're claiming for at the end customer.</span></span> <span data-ttu-id="e1530-156">您的公司可能有許多 MPNs，其中一些可能已在獎勵計畫中註冊，而其他人則與合作夥伴類型（例如 FRP FastTrack）相關聯。</span><span class="sxs-lookup"><span data-stu-id="e1530-156">Your company may have many MPNs, some of which may be enrolled in incentive programs, and others associated with a partner type such as FRP FastTrack.</span></span> <span data-ttu-id="e1530-157">CPOR 關聯宣告流程會識別在獎勵計畫中註冊哪個 MPNs，但不會告訴您它是否為特定的夥伴類型 MPN。</span><span class="sxs-lookup"><span data-stu-id="e1530-157">The CPOR association claim flow will identify which MPNs are enrolled in an incentive program, but it will not tell you if it is a specific partner type MPN.</span></span> <span data-ttu-id="e1530-158">請務必選取正確的 MPN，以避免未來需要回收。</span><span class="sxs-lookup"><span data-stu-id="e1530-158">It’s important to select the correct MPN, to avoid having to reclaim in the future.</span></span> <span data-ttu-id="e1530-159">宣告不正確的 MPN 可能會導致缺少資格和獎勵收益。</span><span class="sxs-lookup"><span data-stu-id="e1530-159">Claiming with an incorrect MPN may result in missed eligibility and incentive earnings.</span></span>

<span data-ttu-id="e1530-160">如果您不知道要使用哪個 MPN，請洽詢您的全域管理員。</span><span class="sxs-lookup"><span data-stu-id="e1530-160">If you do not know which MPN to use, contact your global admin.</span></span>

<span data-ttu-id="e1530-161">如果您想要使用的 MPN 尚未註冊，您可以在 [[獎勵總覽]](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)索引標籤中進行管理。</span><span class="sxs-lookup"><span data-stu-id="e1530-161">If the MPN you're wanting to use isn't enrolled, you can manage that in the [Incentives overview tab](https://partner.microsoft.com/dashboard/incentives/enrollment/summary).</span></span>

## <a name="choosing-a-product-vs-entering-a-subscription"></a><span data-ttu-id="e1530-162">選擇產品與輸入訂用帳戶的比較</span><span class="sxs-lookup"><span data-stu-id="e1530-162">Choosing a product vs entering a subscription</span></span>

<span data-ttu-id="e1530-163">當 Dynamics 產品已領取並核准時，合作夥伴可以在 CPOR association 宣告本身中查看訂用帳戶識別碼。</span><span class="sxs-lookup"><span data-stu-id="e1530-163">When a Dynamics product is claimed and approved, the partner can view the subscription ID in the CPOR association claim itself.</span></span> <span data-ttu-id="e1530-164">當此訂用帳戶被宣告時，它會處於作用中或處於寬限狀態，但可能會有一段時間結束訂用帳戶，而且必須在個別的 CPOR 關聯宣告中領取新的訂閱。</span><span class="sxs-lookup"><span data-stu-id="e1530-164">When this subscription is claimed, it is in active or in grace status, but there may be a time when the subscription ends, and the new subscriptions will need to be claimed in a separate CPOR association claim.</span></span>

## <a name="competing-claims"></a><span data-ttu-id="e1530-165">競爭宣告</span><span class="sxs-lookup"><span data-stu-id="e1530-165">Competing claims</span></span>

<span data-ttu-id="e1530-166">如果您要為客戶建立 CPOR 關聯宣告，而其產品已與另一個合作夥伴相關聯，您的宣告將會通過仲裁：</span><span class="sxs-lookup"><span data-stu-id="e1530-166">If you're creating a CPOR association claim for a customer and their product(s) that is already associated with another partner, your claim will go through arbitration:</span></span>

1. <span data-ttu-id="e1530-167">在您建立新的客戶關聯後，Microsoft 將會驗證所提供關聯和執行證明的詳細資料，以確保其正確性。</span><span class="sxs-lookup"><span data-stu-id="e1530-167">After you create a new customer association, Microsoft will verify the details of the association and proof of execution provided to ensure its accuracy.</span></span>

2. <span data-ttu-id="e1530-168">如果您和其他合作夥伴宣告相同的客戶和產品/工作負載，Microsoft 將會回顧每個合作夥伴的執行證明檔，以決定要核准哪一個夥伴。</span><span class="sxs-lookup"><span data-stu-id="e1530-168">If you and another partner claim the same customer and product/workload, Microsoft will review each partner's proof of execution documentation to determine which partner to approve.</span></span>

3. <span data-ttu-id="e1530-169">可能會從兩個夥伴要求其他資訊，這可能會導致處理您的關聯要求延遲。</span><span class="sxs-lookup"><span data-stu-id="e1530-169">Additional information might be requested from both partners, which could cause delays in processing your association request.</span></span>

4. <span data-ttu-id="e1530-170">您的 CPOR 關聯宣告仍然會在五個工作天內進行檢查，但其狀態可能_會在較_長的時間內保持不變。</span><span class="sxs-lookup"><span data-stu-id="e1530-170">Your CPOR association claim will still be reviewed within five business days, although its status may stay as _Under Review_ for a longer period of time.</span></span> <span data-ttu-id="e1530-171">當 Microsoft 與目前擁有產品/工作負載的合作夥伴合作時，就可能發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="e1530-171">This scenario can happen when Microsoft works with the partner currently owning the product/workload.</span></span> <span data-ttu-id="e1530-172">如果是這種情況，您將會在宣告的 [批註] 區段中收到通知。</span><span class="sxs-lookup"><span data-stu-id="e1530-172">You will be notified within the comments section of your claim if that is the case.</span></span> 

>[!IMPORTANT]
><span data-ttu-id="e1530-173">如果我們需要其他資訊來驗證您的 CPOR association PoE，我們會透過 CPOR 關聯宣告批註一節來聯絡您。</span><span class="sxs-lookup"><span data-stu-id="e1530-173">If we require additional information to verify your CPOR association PoE, we'll contact you via CPOR association claim comments section.</span></span>
