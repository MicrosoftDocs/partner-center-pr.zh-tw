---
title: 使用對帳檔案 | 合作夥伴中心
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 如需計費週期中每個費用的詳細明細專案查看，請從合作夥伴中心下載對帳檔案。
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753857"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="20ade-103">使用對帳檔案</span><span class="sxs-lookup"><span data-stu-id="20ade-103">Use the reconciliation files</span></span>

<span data-ttu-id="20ade-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="20ade-104">**Applies to**</span></span>

-  <span data-ttu-id="20ade-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="20ade-105">Partner Center</span></span>
-  <span data-ttu-id="20ade-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="20ade-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="20ade-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="20ade-107">**Appropriate roles**</span></span>

- <span data-ttu-id="20ade-108">帳單管理</span><span class="sxs-lookup"><span data-stu-id="20ade-108">Billing admin</span></span>
- <span data-ttu-id="20ade-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="20ade-109">Global admin</span></span>

<span data-ttu-id="20ade-110">如需計費週期中每個費用的詳細明細專案查看，請從合作夥伴中心下載對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="20ade-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="20ade-111">詳細資料包括每個客戶的訂閱費用，以及詳細事件 (例如，期中增加訂閱基座)。</span><span class="sxs-lookup"><span data-stu-id="20ade-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="20ade-112">格式化問題</span><span class="sxs-lookup"><span data-stu-id="20ade-112">Formatting issues</span></span>

<span data-ttu-id="20ade-113">有時候，您的偵察檔案可能會有格式問題。</span><span class="sxs-lookup"><span data-stu-id="20ade-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="20ade-114">（例如，如果未使用 EN-US 地區設定，就會發生這種情況）。請遵循下列步驟來修正這些問題。</span><span class="sxs-lookup"><span data-stu-id="20ade-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="20ade-115">在 Excel 中開啟 .csv 檔案，然後選取第一個資料行。</span><span class="sxs-lookup"><span data-stu-id="20ade-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="20ade-116">在功能區上，選取 [<strong>資料</strong>]，然後選取 [<strong>文字到資料行</strong>]。</span><span class="sxs-lookup"><span data-stu-id="20ade-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="20ade-117">在 [將文字轉換成資料行] Wizard 中，選取 [<strong>分隔檔案類型</strong>]，然後選取<strong>[下一步]</strong>。</span><span class="sxs-lookup"><span data-stu-id="20ade-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="20ade-118">在 [Delimeters] 欄位中，選取 [<strong>逗號</strong>]。</span><span class="sxs-lookup"><span data-stu-id="20ade-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="20ade-119">如果已選取 [ <strong>]</strong>索引標籤，您可以將它保留。</span><span class="sxs-lookup"><span data-stu-id="20ade-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="20ade-120">選取 <strong>\[下一步\]</strong>。</span><span class="sxs-lookup"><span data-stu-id="20ade-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="20ade-121">在 [資料行資料格式] 欄位中，選取 [<strong>日期： MDY</strong>]，然後選取<strong>[下一步]</strong>。</span><span class="sxs-lookup"><span data-stu-id="20ade-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="20ade-122">在 [資料行資料格式] 欄位中，針對 [所有數量] 資料行選取 [<strong>文字</strong>]，然後選取<strong>[完成]</strong>。</span><span class="sxs-lookup"><span data-stu-id="20ade-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="20ade-123">下載大型偵察檔案</span><span class="sxs-lookup"><span data-stu-id="20ade-123">Downloading a large recon file</span></span>

<span data-ttu-id="20ade-124">偵察檔案可能會變得非常大，有時很難以下載。</span><span class="sxs-lookup"><span data-stu-id="20ade-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="20ade-125">如需可協助下載大型偵察檔案的 PowerShell 腳本，請參閱[取得發票明細專案](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="20ade-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="20ade-126">依合作夥伴的列舉</span><span class="sxs-lookup"><span data-stu-id="20ade-126">Itemize by partner</span></span>


<span data-ttu-id="20ade-127">間接模型合作夥伴可以在授權型及用量型對帳檔案中使用這些額外欄位，以便依經銷商詳細列舉。</span><span class="sxs-lookup"><span data-stu-id="20ade-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20ade-128">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-128">MPN ID</span></span></th>
<th><span data-ttu-id="20ade-129">說明</span><span class="sxs-lookup"><span data-stu-id="20ade-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20ade-130">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="20ade-131">CSP 合作夥伴 (直接或間接) 的 Microsoft 合作夥伴網路 (MPN) 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-132">經銷商 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="20ade-133">只會出現在間接模型合作夥伴的對帳檔案上。</span><span class="sxs-lookup"><span data-stu-id="20ade-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="20ade-134">訂閱記錄中的經銷商 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20ade-135">這會對應到合作夥伴中心中針對特定訂閱列出的經銷商識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="20ade-136">eTo 觀看或更新轉銷商，從 [合作夥伴中心] 功能表選取 [<strong>客戶</strong>]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="20ade-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="20ade-137">在客戶功能表中，選取 \[訂閱\]，從清單中選擇訂閱。</span><span class="sxs-lookup"><span data-stu-id="20ade-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="20ade-138">選取 \[更新\] 以變更 \[經銷商 (MPN 識別碼)\]。</span><span class="sxs-lookup"><span data-stu-id="20ade-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="20ade-139">如果雲端解決方案提供者合作夥伴直接向客戶銷售訂閱，他們的 MPN 識別碼將會以 MPN 識別碼和經銷商 MPN 識別碼的形式列出兩次。</span><span class="sxs-lookup"><span data-stu-id="20ade-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="20ade-140">如果 CSP 合作夥伴具有沒有 MPN 識別碼的轉銷商，此值會改為設定為合作夥伴的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="20ade-141">如果雲端解決方案提供者合作夥伴移除經銷商識別碼，這個值將會設為 -1。</span><span class="sxs-lookup"><span data-stu-id="20ade-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="20ade-142">以授權為基礎的檔案欄位</span><span class="sxs-lookup"><span data-stu-id="20ade-142">License-based file fields</span></span>


<span data-ttu-id="20ade-143">若要針對您對客戶訂單的費用來對帳，請比較對帳檔案中的 Syndication\_Partner\_Subscription\_Number 與合作夥伴中心的訂閱識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20ade-144"><strong>排</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="20ade-145"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="20ade-146"><strong>範例值</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20ade-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="20ade-148">特定帳單實體的唯一識別碼 (GUID 格式)。</span><span class="sxs-lookup"><span data-stu-id="20ade-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20ade-149">對帳時不需要，但可能是很有用的資訊。</span><span class="sxs-lookup"><span data-stu-id="20ade-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20ade-150">在所有資料列中都是如此。</span><span class="sxs-lookup"><span data-stu-id="20ade-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="20ade-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="20ade-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20ade-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="20ade-153">用來識別客戶的唯一 Microsoft ID（GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20ade-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="20ade-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="20ade-155">OrderID</span></span></td>
<td><p><span data-ttu-id="20ade-156">訂單在 Microsoft 帳單平台中的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20ade-157">可在連絡支援時方便識別訂單，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20ade-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20ade-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20ade-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20ade-160">訂閱在 Microsoft 帳單平台中的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20ade-161">可在連絡支援時方便識別訂閱，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20ade-162">這與合作夥伴管理主控台上的訂閱識別碼不一樣。</span><span class="sxs-lookup"><span data-stu-id="20ade-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="20ade-163">請參閱 Syndication_Partner_Subscription_Number。</span><span class="sxs-lookup"><span data-stu-id="20ade-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="20ade-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20ade-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="20ade-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="20ade-166">訂閱的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="20ade-167">客戶可針對同一方案擁有多項訂閱，因此這對於對帳檔案分析而言很重要。</span><span class="sxs-lookup"><span data-stu-id="20ade-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="20ade-168">這個欄位對應到合作夥伴管理主控台中的訂閱識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20ade-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="20ade-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="20ade-170">OfferID</span></span></td>
<td><p><span data-ttu-id="20ade-171">唯一的優惠識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-171">Unique offer ID.</span></span> <span data-ttu-id="20ade-172">根據價目表的標準優惠識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="20ade-173"><b>注意</b>：這個值不符合價目表上的優惠識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="20ade-174">請參閱下方的 DurableOfferID。</span><span class="sxs-lookup"><span data-stu-id="20ade-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="20ade-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="20ade-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="20ade-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="20ade-177">唯一的持續性優惠識別碼，如價目表中所定義。</span><span class="sxs-lookup"><span data-stu-id="20ade-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="20ade-178"><b>注意</b>：這個值符合價目表上的優惠識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="20ade-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="20ade-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="20ade-180">OfferName</span></span></td>
<td><p><span data-ttu-id="20ade-181">客戶購買的服務優惠名稱，如價目表中所定義。</span><span class="sxs-lookup"><span data-stu-id="20ade-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="20ade-182">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="20ade-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="20ade-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="20ade-184">訂閱開始日期設定為送出訂單之後的隔日。</span><span class="sxs-lookup"><span data-stu-id="20ade-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="20ade-185">藉由同時查看訂閱開始日期與結束日期，您就可以判斷客戶是否仍在第一年訂閱期內，或下一年的訂閱已續約。</span><span class="sxs-lookup"><span data-stu-id="20ade-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="20ade-186">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20ade-187">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20ade-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="20ade-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="20ade-189">訂閱結束日期：開始日期之後的 12 個月 + x 天 (與合作夥伴帳單日期配合) 或自續約日期起 12 個月。</span><span class="sxs-lookup"><span data-stu-id="20ade-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="20ade-190">續約時，價格會更新至目前的價目表。</span><span class="sxs-lookup"><span data-stu-id="20ade-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="20ade-191">自動續約之前，可能需要與客戶連絡。</span><span class="sxs-lookup"><span data-stu-id="20ade-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="20ade-192">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20ade-193">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20ade-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20ade-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20ade-195">開始計算費用的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="20ade-196">當客戶變更基座數目時，此數字用於計算每日 (按比例) 的費用。</span><span class="sxs-lookup"><span data-stu-id="20ade-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20ade-197">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20ade-198">2/1/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="20ade-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20ade-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20ade-200">結束計算費用的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="20ade-201">當客戶變更基座數目時，此數字用於計算每日 (按比例) 的費用。</span><span class="sxs-lookup"><span data-stu-id="20ade-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="20ade-202">時間一律是一天的結束時間 (23:59)。</span><span class="sxs-lookup"><span data-stu-id="20ade-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20ade-203">2/28/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="20ade-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20ade-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="20ade-205">費用或調整的類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-205">The type of charge or adjustment.</span></span> <span data-ttu-id="20ade-206">請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></span><span class="sxs-lookup"><span data-stu-id="20ade-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20ade-207">請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></span><span class="sxs-lookup"><span data-stu-id="20ade-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="20ade-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="20ade-209">每一基座價格，即購買時價目表中所公佈的價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20ade-210">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20ade-211">6.82</span><span class="sxs-lookup"><span data-stu-id="20ade-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-212">數量</span><span class="sxs-lookup"><span data-stu-id="20ade-212">Quantity</span></span></td>
<td><p><span data-ttu-id="20ade-213">基座數目。</span><span class="sxs-lookup"><span data-stu-id="20ade-213">Number of seats.</span></span> <span data-ttu-id="20ade-214">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="20ade-215">2</span><span class="sxs-lookup"><span data-stu-id="20ade-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-216">金額</span><span class="sxs-lookup"><span data-stu-id="20ade-216">Amount</span></span></td>
<td><p><span data-ttu-id="20ade-217">數量總價。</span><span class="sxs-lookup"><span data-stu-id="20ade-217">Total of price for quantity.</span></span> <span data-ttu-id="20ade-218">檢查計算金額與您用來為客戶計算此項目的方式是否相符時很有用。</span><span class="sxs-lookup"><span data-stu-id="20ade-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="20ade-219">13.32</span><span class="sxs-lookup"><span data-stu-id="20ade-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="20ade-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="20ade-221">套用至這些費用的折扣金額。</span><span class="sxs-lookup"><span data-stu-id="20ade-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="20ade-222">專長認證或對應或符合獎勵資格的新訂用帳戶所含的產品授權也會在本專欄中包含折扣金額。</span><span class="sxs-lookup"><span data-stu-id="20ade-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="20ade-223">2.32</span><span class="sxs-lookup"><span data-stu-id="20ade-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-224">小計</span><span class="sxs-lookup"><span data-stu-id="20ade-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="20ade-225">稅前總計。</span><span class="sxs-lookup"><span data-stu-id="20ade-225">Total before tax.</span></span> <span data-ttu-id="20ade-226">如果有折扣，可檢查小計是否和預期的總金額相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="20ade-227">11</span><span class="sxs-lookup"><span data-stu-id="20ade-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-228">稅</span><span class="sxs-lookup"><span data-stu-id="20ade-228">Tax</span></span></td>
<td><p><span data-ttu-id="20ade-229">稅金金額費用，以您的市場&#39;稅務規則和特定情況為基礎。</span><span class="sxs-lookup"><span data-stu-id="20ade-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20ade-230">0</span><span class="sxs-lookup"><span data-stu-id="20ade-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="20ade-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="20ade-232">稅後總計。</span><span class="sxs-lookup"><span data-stu-id="20ade-232">Total after tax.</span></span> <span data-ttu-id="20ade-233">檢查發票中是否向您收取稅金。</span><span class="sxs-lookup"><span data-stu-id="20ade-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="20ade-234">11</span><span class="sxs-lookup"><span data-stu-id="20ade-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-235">Currency</span><span class="sxs-lookup"><span data-stu-id="20ade-235">Currency</span></span></td>
<td><p><span data-ttu-id="20ade-236">貨幣類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-236">Currency type.</span></span> <span data-ttu-id="20ade-237">每一帳單實體都只有一種貨幣。</span><span class="sxs-lookup"><span data-stu-id="20ade-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="20ade-238">檢查是否與您的第一張發票相符，然後在進行任何重大帳單平台更新之後檢查。</span><span class="sxs-lookup"><span data-stu-id="20ade-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20ade-239">EUR</span><span class="sxs-lookup"><span data-stu-id="20ade-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20ade-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="20ade-241">合作夥伴&#39;中心所回報的客戶組織名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="20ade-242">這在使用您的系統資訊對帳發票時非常重要。</span><span class="sxs-lookup"><span data-stu-id="20ade-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20ade-243">測試客戶 A</span><span class="sxs-lookup"><span data-stu-id="20ade-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-244">MPNID</span></span></td>
<td><p><span data-ttu-id="20ade-245">雲端解決方案提供者合作夥伴的 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="20ade-246">4390934</span><span class="sxs-lookup"><span data-stu-id="20ade-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20ade-248">訂閱記錄中的經銷商 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20ade-249">請參閱<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">依合作夥伴詳細列舉</a>。</span><span class="sxs-lookup"><span data-stu-id="20ade-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="20ade-250">4390934</span><span class="sxs-lookup"><span data-stu-id="20ade-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="20ade-251">DomainName</span></span></td>
<td><p><span data-ttu-id="20ade-252">客戶&#39;的功能變數名稱，用來協助識別客戶。</span><span class="sxs-lookup"><span data-stu-id="20ade-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="20ade-253">這不應該用來唯一識別客戶，因為客戶/合作夥伴可以透過 O365 入口網站更新虛名/預設網域。</span><span class="sxs-lookup"><span data-stu-id="20ade-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20ade-254">在下一個帳單週期之前，此欄位會是空白的。</span><span class="sxs-lookup"><span data-stu-id="20ade-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20ade-255">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20ade-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20ade-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20ade-257">訂閱暱稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-257">Subscription nickname.</span></span> <span data-ttu-id="20ade-258">如果未指定任何暱稱，合作夥伴中心會使用 OfferName。</span><span class="sxs-lookup"><span data-stu-id="20ade-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="20ade-259">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="20ade-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20ade-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20ade-261">客戶購買的服務優惠名稱，如價目表中所定義。</span><span class="sxs-lookup"><span data-stu-id="20ade-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20ade-262">（這是優惠名稱的相同欄位）。</span><span class="sxs-lookup"><span data-stu-id="20ade-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="20ade-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span><span class="sxs-lookup"><span data-stu-id="20ade-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="20ade-264">以使用方式為基礎的檔案欄位</span><span class="sxs-lookup"><span data-stu-id="20ade-264">Usage-based file fields</span></span>


<span data-ttu-id="20ade-265">若要針對您客戶使用量的費用來對帳，請比較對帳檔案中的 ResellerID/ResellerName/ResellerBillableAccount、客戶名稱，與合作夥伴中心的訂閱識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="20ade-266">下列欄位說明使用哪些服務及費率。</span><span class="sxs-lookup"><span data-stu-id="20ade-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="20ade-267"><strong>排</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="20ade-268"><strong>描述</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="20ade-269"><strong>範例值</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="20ade-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="20ade-271">合作夥伴識別碼 (GUID 格式)。</span><span class="sxs-lookup"><span data-stu-id="20ade-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="20ade-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20ade-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20ade-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="20ade-274">合作夥伴名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="20ade-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="20ade-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="20ade-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="20ade-277">合作夥伴帳戶識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="20ade-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="20ade-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="20ade-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="20ade-280">合作夥伴&#39;中心所回報的客戶組織名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="20ade-281">這在使用您的系統資訊對帳發票時非常重要。</span><span class="sxs-lookup"><span data-stu-id="20ade-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="20ade-282">測試客戶 A</span><span class="sxs-lookup"><span data-stu-id="20ade-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-283">MPNID</span></span></td>
<td><p><span data-ttu-id="20ade-284">雲端解決方案提供者合作夥伴的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="20ade-285">4390934</span><span class="sxs-lookup"><span data-stu-id="20ade-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="20ade-287">訂閱記錄中的經銷商 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20ade-288">請參閱<a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">依合作夥伴詳細列舉</a>。</span><span class="sxs-lookup"><span data-stu-id="20ade-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="20ade-289">4390934</span><span class="sxs-lookup"><span data-stu-id="20ade-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20ade-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20ade-291">交易的指定位置顯示的發票號碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="20ade-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="20ade-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20ade-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20ade-294">計費週期的開始日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</span><span class="sxs-lookup"><span data-stu-id="20ade-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20ade-295">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="20ade-296">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20ade-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20ade-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20ade-298">計費週期的結束日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</span><span class="sxs-lookup"><span data-stu-id="20ade-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="20ade-299">時間一律是一天的結束時間 (23:59)。</span><span class="sxs-lookup"><span data-stu-id="20ade-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="20ade-300">2/28/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="20ade-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="20ade-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="20ade-302">訂閱在 Microsoft 帳單平台中的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20ade-303">可在連絡支援時方便識別訂閱，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="20ade-304">這與合作夥伴管理主控台上的訂閱識別碼不一樣。</span><span class="sxs-lookup"><span data-stu-id="20ade-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="20ade-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="20ade-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="20ade-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="20ade-307">服務優惠的暱稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="20ade-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20ade-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="20ade-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="20ade-310">服務優惠的企業營運</span><span class="sxs-lookup"><span data-stu-id="20ade-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="20ade-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="20ade-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="20ade-312">OrderID</span></span></td>
<td><p><span data-ttu-id="20ade-313">訂單在 Microsoft 帳單平台中的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="20ade-314">可在連絡支援時方便識別訂閱，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="20ade-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="20ade-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="20ade-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="20ade-317">要求的 Azure 服務名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="20ade-318">虛擬機器</span><span class="sxs-lookup"><span data-stu-id="20ade-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="20ade-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="20ade-320">Microsoft Azure 服務的特定類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20ade-321">服務匯流排-個人或套件</span><span class="sxs-lookup"><span data-stu-id="20ade-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="20ade-322">SQL Azure 資料庫-Business 或 Web Edition</span><span class="sxs-lookup"><span data-stu-id="20ade-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="20ade-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="20ade-324">所有服務資料與定價結構的特定唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="20ade-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="20ade-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-326">Resource Name</span><span class="sxs-lookup"><span data-stu-id="20ade-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="20ade-327">Azure 資源的名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="20ade-328">資料轉入 (GB)</span><span class="sxs-lookup"><span data-stu-id="20ade-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="20ade-329">資料轉出 (GB)</span><span class="sxs-lookup"><span data-stu-id="20ade-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-330">地區</span><span class="sxs-lookup"><span data-stu-id="20ade-330">Region</span></span></td>
<td><p><span data-ttu-id="20ade-331">使用量適用的地區。</span><span class="sxs-lookup"><span data-stu-id="20ade-331">The region the usage applies to.</span></span> <span data-ttu-id="20ade-332">主要用來指定資料傳輸速率，費率因地區而異。</span><span class="sxs-lookup"><span data-stu-id="20ade-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="20ade-333">亞太地區、歐洲、拉丁美洲、北美洲</span><span class="sxs-lookup"><span data-stu-id="20ade-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-334">SKU</span><span class="sxs-lookup"><span data-stu-id="20ade-334">SKU</span></span></td>
<td><p><span data-ttu-id="20ade-335">優惠的 MSFT 唯一識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="20ade-336">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="20ade-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="20ade-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="20ade-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="20ade-338">用於詳細列出指定計費期間中，服務或資源不同費率的識別碼和數量。</span><span class="sxs-lookup"><span data-stu-id="20ade-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="20ade-339">對於 Azure 分層評分，到某個數量的計費單位會有一個評分，之後則有不同評分。</span><span class="sxs-lookup"><span data-stu-id="20ade-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="20ade-340">1</span><span class="sxs-lookup"><span data-stu-id="20ade-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="20ade-342">報表期間耗用的服務量 (小時、GB 等等)</span><span class="sxs-lookup"><span data-stu-id="20ade-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="20ade-343">同時包括先前報表期間任何未計費的使用量。</span><span class="sxs-lookup"><span data-stu-id="20ade-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="20ade-344">11</span><span class="sxs-lookup"><span data-stu-id="20ade-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="20ade-346">包含在優惠中的單位。</span><span class="sxs-lookup"><span data-stu-id="20ade-346">Units included as part of the offer.</span></span> <span data-ttu-id="20ade-347">通常不會出現在雲端解決方案提供者中。</span><span class="sxs-lookup"><span data-stu-id="20ade-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="20ade-348">0</span><span class="sxs-lookup"><span data-stu-id="20ade-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="20ade-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="20ade-350">不包含在優惠中的單位，必須由合作夥伴支付。</span><span class="sxs-lookup"><span data-stu-id="20ade-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="20ade-351">等同於 ConsumedQuantity - IncludedQuantity。</span><span class="sxs-lookup"><span data-stu-id="20ade-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="20ade-352">11</span><span class="sxs-lookup"><span data-stu-id="20ade-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="20ade-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="20ade-354">訂閱開始日期的生效優惠價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="20ade-355">$0.0808</span><span class="sxs-lookup"><span data-stu-id="20ade-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="20ade-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="20ade-357">ListPrist 乘以 OverageQuantity，四捨五入至美分。</span><span class="sxs-lookup"><span data-stu-id="20ade-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20ade-358">$0.085</span><span class="sxs-lookup"><span data-stu-id="20ade-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="20ade-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="20ade-360">稅金金額費用，以您的市場&#39;稅務規則和特定情況為基礎。</span><span class="sxs-lookup"><span data-stu-id="20ade-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="20ade-361">$0.08</span><span class="sxs-lookup"><span data-stu-id="20ade-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="20ade-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="20ade-363">稅後總計 (當適用稅金時)。</span><span class="sxs-lookup"><span data-stu-id="20ade-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="20ade-364">$0.93</span><span class="sxs-lookup"><span data-stu-id="20ade-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-365">Currency</span><span class="sxs-lookup"><span data-stu-id="20ade-365">Currency</span></span></td>
<td><p><span data-ttu-id="20ade-366">貨幣類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-366">Currency type.</span></span> <span data-ttu-id="20ade-367">每一帳單實體都只有一種貨幣。</span><span class="sxs-lookup"><span data-stu-id="20ade-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="20ade-368">檢查是否與您的第一張發票相符，然後在進行任何重大帳單平台更新之後檢查。</span><span class="sxs-lookup"><span data-stu-id="20ade-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="20ade-369">EUR</span><span class="sxs-lookup"><span data-stu-id="20ade-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20ade-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20ade-371">每個單位的稅前價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-371">Pretax price per unit.</span></span> <span data-ttu-id="20ade-372">等於 PretaxCharges / OverageQuantity, 四捨五入至美分。</span><span class="sxs-lookup"><span data-stu-id="20ade-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20ade-373">$0.08</span><span class="sxs-lookup"><span data-stu-id="20ade-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="20ade-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="20ade-375">每個單位的稅後價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-375">Post tax price per unit.</span></span> <span data-ttu-id="20ade-376">等於 PostTaxTotal / OverageQuantity，或 PretaxEffectiveRate + 每單位數量稅率，四捨五入至美分。</span><span class="sxs-lookup"><span data-stu-id="20ade-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="20ade-377">$0.08</span><span class="sxs-lookup"><span data-stu-id="20ade-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="20ade-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="20ade-379">費用或調整的類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-379">The type of charge or adjustment.</span></span> <span data-ttu-id="20ade-380">請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></span><span class="sxs-lookup"><span data-stu-id="20ade-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="20ade-381">請參閱<a href="#charge_types">對應發票和對帳檔案之間的費用</a></span><span class="sxs-lookup"><span data-stu-id="20ade-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="20ade-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="20ade-383">MSFT 帳單平台的唯一帳戶識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="20ade-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="20ade-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="20ade-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="20ade-386">服務部署的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="20ade-387">2/1/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="20ade-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="20ade-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="20ade-389">此欄可識別適用及填入此項目之服務地區內的資料中心的位置。</span><span class="sxs-lookup"><span data-stu-id="20ade-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="20ade-390">東亞、東南亞、北歐、西歐、美國中北部、美國中南部</span><span class="sxs-lookup"><span data-stu-id="20ade-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="20ade-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="20ade-392">此欄是用來追蹤可能未在 \[服務名稱\] 欄中特別指出的個別 Microsoft Azure 服務。</span><span class="sxs-lookup"><span data-stu-id="20ade-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="20ade-393">例如，在 \[服務名稱\] 欄中，資料傳輸是回報為 &quot;Microsoft Azure - 所有服務&quot;。</span><span class="sxs-lookup"><span data-stu-id="20ade-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="20ade-394">此 MeteredService 欄會指出使用量與哪個特定服務有關。</span><span class="sxs-lookup"><span data-stu-id="20ade-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="20ade-395">AccessControl、CDN、Compute、Database、ServiceBus、Storage</span><span class="sxs-lookup"><span data-stu-id="20ade-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="20ade-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="20ade-397">進一步釐清超出 MeteredService 欄位提供之層級的個別 Microsoft Azure 服務副標題。</span><span class="sxs-lookup"><span data-stu-id="20ade-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="20ade-398">外部</span><span class="sxs-lookup"><span data-stu-id="20ade-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-399">投影</span><span class="sxs-lookup"><span data-stu-id="20ade-399">Project</span></span></td>
<td><p><span data-ttu-id="20ade-400">客戶為其服務執行個體定義的名稱</span><span class="sxs-lookup"><span data-stu-id="20ade-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="20ade-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20ade-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="20ade-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="20ade-403">於某一天佈建及使用的 ServiceBus 連線數目。</span><span class="sxs-lookup"><span data-stu-id="20ade-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="20ade-404">例如：如果您在每月30天內有個別布建的連線，服務資訊1會讀取「1.000000 連線/30 天」。</span><span class="sxs-lookup"><span data-stu-id="20ade-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="20ade-405">如果您已布建25部的故障匯流排連線，而您在該天內使用了1個，則當天的每日使用方式聲明會指出「25個連接/30 天-已使用：1.000000」。</span><span class="sxs-lookup"><span data-stu-id="20ade-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="20ade-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="20ade-407">用來識別客戶的唯一 Microsoft ID（GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="20ade-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="20ade-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="20ade-409">DomainName</span></span></td>
<td><p><span data-ttu-id="20ade-410">客戶&#39;的功能變數名稱，用來協助識別客戶。</span><span class="sxs-lookup"><span data-stu-id="20ade-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="20ade-411">在下一個帳單週期之前，此欄位會是空白的。</span><span class="sxs-lookup"><span data-stu-id="20ade-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="20ade-412">example.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="20ade-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-413">單位</span><span class="sxs-lookup"><span data-stu-id="20ade-413">Unit</span></span></td>
<td><p><span data-ttu-id="20ade-414">資源名稱的單位</span><span class="sxs-lookup"><span data-stu-id="20ade-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="20ade-415">GB 或 HOURS</span><span class="sxs-lookup"><span data-stu-id="20ade-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="20ade-416">一次性和週期性的檔案欄位</span><span class="sxs-lookup"><span data-stu-id="20ade-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20ade-417">Column</span><span class="sxs-lookup"><span data-stu-id="20ade-417">Column</span></span></th>
<th><span data-ttu-id="20ade-418">說明</span><span class="sxs-lookup"><span data-stu-id="20ade-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="20ade-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20ade-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="20ade-420">特定計費實體的唯一 Microsoft Azure Active Directory 租使用者識別碼（GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="20ade-421">對帳時不需要，但可能是很有用的資訊。</span><span class="sxs-lookup"><span data-stu-id="20ade-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="20ade-422">在所有資料列中都是如此。</span><span class="sxs-lookup"><span data-stu-id="20ade-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-423">客戶識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="20ade-424">用來識別客戶的唯一 Microsoft Azure Active Directory 租使用者識別碼（GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-425">[客戶名稱]</span><span class="sxs-lookup"><span data-stu-id="20ade-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="20ade-426">合作夥伴中心中回報的客戶組織名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20ade-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="20ade-428">用來協助識別客戶的客戶網域名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="20ade-429">這不應該用來唯一識別客戶，因為客戶/合作夥伴可以透過 O365 入口網站更新虛名/預設網域。</span><span class="sxs-lookup"><span data-stu-id="20ade-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="20ade-430">在下一個帳單週期之前，此欄位會是空白的。</span><span class="sxs-lookup"><span data-stu-id="20ade-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-431">客戶國家/地區</span><span class="sxs-lookup"><span data-stu-id="20ade-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="20ade-432">客戶所在的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="20ade-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-433">發票號碼</span><span class="sxs-lookup"><span data-stu-id="20ade-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="20ade-434">交易的指定位置顯示的發票號碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="20ade-435">MpnId</span></span></td>
<td><p><span data-ttu-id="20ade-436">雲端解決方案提供者合作夥伴的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-437">轉售商 MpnId</span><span class="sxs-lookup"><span data-stu-id="20ade-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="20ade-438">訂閱記錄中的經銷商 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-439">訂單識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-439">Order ID</span></span></td>
<td><p><span data-ttu-id="20ade-440">Microsoft 商務平臺中訂單的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="20ade-441">可在連絡支援時方便識別訂單，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-442">訂單日期</span><span class="sxs-lookup"><span data-stu-id="20ade-442">Order date</span></span></td>
<td><p><span data-ttu-id="20ade-443">下訂單的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="20ade-444">ProductId</span></span></td>
<td><p><span data-ttu-id="20ade-445">產品的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="20ade-446">SkuId</span></span></td>
<td><p><span data-ttu-id="20ade-447">特定 SKU 的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20ade-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="20ade-449">特定可用性的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-449">The ID for a particular Availability.</span></span> <span data-ttu-id="20ade-450">「可用性」指的是特定 SKU 是否可針對指定的國家/地區、貨幣、產業區段等購買。</span><span class="sxs-lookup"><span data-stu-id="20ade-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-451">SKU 名稱</span><span class="sxs-lookup"><span data-stu-id="20ade-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="20ade-452">特定 SKU 的標題。</span><span class="sxs-lookup"><span data-stu-id="20ade-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-453">[產品名稱]</span><span class="sxs-lookup"><span data-stu-id="20ade-453">Product name</span></span></td>
<td><p><span data-ttu-id="20ade-454">產品的名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="20ade-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="20ade-456">產品發行者的名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="20ade-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="20ade-458">此發行者的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-459">訂用帳戶描述</span><span class="sxs-lookup"><span data-stu-id="20ade-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="20ade-460">訂用帳戶的易記名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-461">[訂閱識別碼]</span><span class="sxs-lookup"><span data-stu-id="20ade-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="20ade-462">Microsoft commerce 平臺中訂用帳戶的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="20ade-463">可在連絡支援時方便識別訂閱，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="20ade-464">這與合作夥伴管理主控台上的訂閱識別碼不一樣。</span><span class="sxs-lookup"><span data-stu-id="20ade-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20ade-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20ade-466">開始計算費用的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-466">Start day of the charges.</span></span> <span data-ttu-id="20ade-467">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20ade-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20ade-469">結束計算費用的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-469">End day of the charges.</span></span> <span data-ttu-id="20ade-470">時間一律是一天的結束時間 (23:59)。</span><span class="sxs-lookup"><span data-stu-id="20ade-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-471">詞彙和 Billingcycle</span><span class="sxs-lookup"><span data-stu-id="20ade-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="20ade-472">購買的詞彙長度和計費週期。</span><span class="sxs-lookup"><span data-stu-id="20ade-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="20ade-473">例如，「1年、每月」。</span><span class="sxs-lookup"><span data-stu-id="20ade-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-474">收費類型</span><span class="sxs-lookup"><span data-stu-id="20ade-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="20ade-475">費用或調整的類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-476">單價</span><span class="sxs-lookup"><span data-stu-id="20ade-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="20ade-477">購買時，在價目表中發佈的價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20ade-478">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-479">有效單位價格</span><span class="sxs-lookup"><span data-stu-id="20ade-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="20ade-480">進行調整後的單位價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-481">數量</span><span class="sxs-lookup"><span data-stu-id="20ade-481">Quantity</span></span></td>
<td><p><span data-ttu-id="20ade-482">單位數。</span><span class="sxs-lookup"><span data-stu-id="20ade-482">Number of units.</span></span> <span data-ttu-id="20ade-483">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-484">單位類型</span><span class="sxs-lookup"><span data-stu-id="20ade-484">Unit type</span></span></td>
<td><p><span data-ttu-id="20ade-485">所購買的單位類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="20ade-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="20ade-487">任何適用折扣的說明。</span><span class="sxs-lookup"><span data-stu-id="20ade-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-488">子總計</span><span class="sxs-lookup"><span data-stu-id="20ade-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="20ade-489">稅前總計。</span><span class="sxs-lookup"><span data-stu-id="20ade-489">Total before tax.</span></span> <span data-ttu-id="20ade-490">如果有折扣，可檢查小計是否和預期的總金額相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-491">稅金總計</span><span class="sxs-lookup"><span data-stu-id="20ade-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="20ade-492">稅金費用 (根據您所在市場的稅金規則與特定情況)。</span><span class="sxs-lookup"><span data-stu-id="20ade-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-493">總計</span><span class="sxs-lookup"><span data-stu-id="20ade-493">Total</span></span></td>
<td><p><span data-ttu-id="20ade-494">稅後總計。</span><span class="sxs-lookup"><span data-stu-id="20ade-494">Total after tax.</span></span> <span data-ttu-id="20ade-495">檢查發票中是否向您收取稅金。</span><span class="sxs-lookup"><span data-stu-id="20ade-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-496">Currency</span><span class="sxs-lookup"><span data-stu-id="20ade-496">Currency</span></span></td>
<td><p><span data-ttu-id="20ade-497">貨幣類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-497">Currency type.</span></span> <span data-ttu-id="20ade-498">每一帳單實體都只有一種貨幣。</span><span class="sxs-lookup"><span data-stu-id="20ade-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="20ade-499">檢查是否與您的第一張發票相符，然後在進行任何重大帳單平台更新之後檢查。</span><span class="sxs-lookup"><span data-stu-id="20ade-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-500">替代識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="20ade-501">訂單識別碼的替代識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="20ade-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="20ade-503">當每月計費啟用時，會顯示每月。</span><span class="sxs-lookup"><span data-stu-id="20ade-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="20ade-504">否則為空白。</span><span class="sxs-lookup"><span data-stu-id="20ade-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="20ade-506">代表已購買或耗用的單位總數。</span><span class="sxs-lookup"><span data-stu-id="20ade-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-507">pricingCurrency</span><span class="sxs-lookup"><span data-stu-id="20ade-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="20ade-508">列出資源或供應專案的價格</span><span class="sxs-lookup"><span data-stu-id="20ade-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="20ade-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="20ade-510">定價貨幣對（客戶）計費貨幣的匯率</span><span class="sxs-lookup"><span data-stu-id="20ade-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="20ade-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="20ade-512">決定計費貨幣匯率的定價日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="20ade-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="20ade-514">耗用量明細專案的計量描述</span><span class="sxs-lookup"><span data-stu-id="20ade-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="20ade-515">每日評分的使用量檔案欄位</span><span class="sxs-lookup"><span data-stu-id="20ade-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="20ade-516">Column</span><span class="sxs-lookup"><span data-stu-id="20ade-516">Column</span></span></th>
<th><span data-ttu-id="20ade-517">說明</span><span class="sxs-lookup"><span data-stu-id="20ade-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="20ade-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="20ade-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="20ade-519">合作夥伴識別碼 (GUID 格式)。</span><span class="sxs-lookup"><span data-stu-id="20ade-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="20ade-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="20ade-521">合作夥伴名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="20ade-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="20ade-523">用來識別客戶的唯一 Microsoft ID（GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="20ade-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="20ade-525">合作夥伴中心中回報的客戶組織名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="20ade-526">這在使用您的系統資訊對帳發票時非常重要。</span><span class="sxs-lookup"><span data-stu-id="20ade-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="20ade-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="20ade-528">客戶的功能變數名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-528">The customer's domain name.</span></span> <span data-ttu-id="20ade-529">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-530">客戶國家/地區</span><span class="sxs-lookup"><span data-stu-id="20ade-530">Customer country</span></span></td>
<td><p><span data-ttu-id="20ade-531">客戶所在的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="20ade-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-532">MPNID</span></span></td>
<td><p><span data-ttu-id="20ade-533">雲端解決方案提供者合作夥伴的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-534">轉售商 MPNID</span><span class="sxs-lookup"><span data-stu-id="20ade-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="20ade-535">訂閱記錄中的經銷商 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="20ade-536">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="20ade-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="20ade-538">交易的指定位置顯示的發票號碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="20ade-539">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="20ade-540">ProductId</span></span></td>
<td><p><span data-ttu-id="20ade-541">產品的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="20ade-542">SkuId</span></span></td>
<td><p><span data-ttu-id="20ade-543">特定 SKU 的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="20ade-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="20ade-545">特定可用性的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-545">The ID for a particular Availability.</span></span> <span data-ttu-id="20ade-546">「可用性」指的是特定 SKU 是否可針對指定的國家/地區、貨幣、產業區段等購買。</span><span class="sxs-lookup"><span data-stu-id="20ade-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-547">SKU 名稱</span><span class="sxs-lookup"><span data-stu-id="20ade-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="20ade-548">特定 SKU 的標題。</span><span class="sxs-lookup"><span data-stu-id="20ade-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="20ade-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="20ade-550">發行者的名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="20ade-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="20ade-552">發行者的識別碼（以 GUID 格式）。</span><span class="sxs-lookup"><span data-stu-id="20ade-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="20ade-553">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-554">訂用帳戶描述</span><span class="sxs-lookup"><span data-stu-id="20ade-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="20ade-555">客戶購買的服務優惠名稱，如價目表中所定義。</span><span class="sxs-lookup"><span data-stu-id="20ade-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="20ade-556">（這是優惠名稱的相同欄位）。</span><span class="sxs-lookup"><span data-stu-id="20ade-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-557">[訂閱識別碼]</span><span class="sxs-lookup"><span data-stu-id="20ade-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="20ade-558">訂閱在 Microsoft 帳單平台中的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="20ade-559">可在連絡支援時方便識別訂閱，但不是用於對帳。</span><span class="sxs-lookup"><span data-stu-id="20ade-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="20ade-560">這與合作夥伴管理主控台上的訂閱識別碼不一樣。</span><span class="sxs-lookup"><span data-stu-id="20ade-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="20ade-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="20ade-562">計費週期的開始日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</span><span class="sxs-lookup"><span data-stu-id="20ade-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="20ade-563">時間一律是一天的開始時間 (0:00)。</span><span class="sxs-lookup"><span data-stu-id="20ade-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="20ade-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="20ade-565">計費週期的結束日期，當顯示之前未收取潛在使用量資料費用的日期時除外 (從前一個計費週期開始)。</span><span class="sxs-lookup"><span data-stu-id="20ade-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="20ade-566">時間一律是一天的結束時間 (23:59)。</span><span class="sxs-lookup"><span data-stu-id="20ade-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-567">使用日期</span><span class="sxs-lookup"><span data-stu-id="20ade-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="20ade-568">服務使用量的日期。</span><span class="sxs-lookup"><span data-stu-id="20ade-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-569">計量類型</span><span class="sxs-lookup"><span data-stu-id="20ade-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="20ade-570">計量的類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-571">計量類別</span><span class="sxs-lookup"><span data-stu-id="20ade-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="20ade-572">使用的最上層服務。</span><span class="sxs-lookup"><span data-stu-id="20ade-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-573">計量識別碼</span><span class="sxs-lookup"><span data-stu-id="20ade-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="20ade-574">所使用之計量的識別碼。</span><span class="sxs-lookup"><span data-stu-id="20ade-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-575">計量子類別</span><span class="sxs-lookup"><span data-stu-id="20ade-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="20ade-576">可能會影響費率的 Azure 服務類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-577">計量名稱</span><span class="sxs-lookup"><span data-stu-id="20ade-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="20ade-578">所耗用計量的測量單位。</span><span class="sxs-lookup"><span data-stu-id="20ade-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-579">計量區域</span><span class="sxs-lookup"><span data-stu-id="20ade-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="20ade-580">此欄可識別適用及填入此項目之服務地區內的資料中心的位置。</span><span class="sxs-lookup"><span data-stu-id="20ade-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-581">單位</span><span class="sxs-lookup"><span data-stu-id="20ade-581">Unit</span></span></td>
<td><p><span data-ttu-id="20ade-582">資源名稱的單位。</span><span class="sxs-lookup"><span data-stu-id="20ade-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-583">已耗用數量</span><span class="sxs-lookup"><span data-stu-id="20ade-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="20ade-584">報表期間耗用的服務量 (小時、GB 等等)</span><span class="sxs-lookup"><span data-stu-id="20ade-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="20ade-585">同時包括先前報表期間任何未計費的使用量。</span><span class="sxs-lookup"><span data-stu-id="20ade-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-586">資源位置</span><span class="sxs-lookup"><span data-stu-id="20ade-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="20ade-587">正在執行計量的資料中心。</span><span class="sxs-lookup"><span data-stu-id="20ade-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-588">已使用服務</span><span class="sxs-lookup"><span data-stu-id="20ade-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="20ade-589">您所使用的 Azure 平臺服務。</span><span class="sxs-lookup"><span data-stu-id="20ade-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="20ade-590">資源 URI</span><span class="sxs-lookup"><span data-stu-id="20ade-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="20ade-591">所使用資源的 URI。</span><span class="sxs-lookup"><span data-stu-id="20ade-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-592">收費類型</span><span class="sxs-lookup"><span data-stu-id="20ade-592">Charge type</span></span></td>
<td><p><span data-ttu-id="20ade-593">費用或調整的類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-593">The type of charge or adjustment.</span></span> <span data-ttu-id="20ade-594">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-595">單價</span><span class="sxs-lookup"><span data-stu-id="20ade-595">Unit price</span></span></td>
<td><p><span data-ttu-id="20ade-596">每份授權的價格，在購買時于價目表中發行。</span><span class="sxs-lookup"><span data-stu-id="20ade-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="20ade-597">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-598">數量</span><span class="sxs-lookup"><span data-stu-id="20ade-598">Quantity</span></span></td>
<td><p><span data-ttu-id="20ade-599">授權數目。</span><span class="sxs-lookup"><span data-stu-id="20ade-599">Number of licenses.</span></span> <span data-ttu-id="20ade-600">請確定這與對帳期間儲存在您帳單系統中的資訊相符。</span><span class="sxs-lookup"><span data-stu-id="20ade-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-601">單位類型</span><span class="sxs-lookup"><span data-stu-id="20ade-601">Unit type</span></span></td>
<td><p><span data-ttu-id="20ade-602">計量計費的單位類型。</span><span class="sxs-lookup"><span data-stu-id="20ade-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="20ade-603">目前的活動無法使用。</span><span class="sxs-lookup"><span data-stu-id="20ade-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-604">計費預付稅</span><span class="sxs-lookup"><span data-stu-id="20ade-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="20ade-605">稅金之前的總金額。</span><span class="sxs-lookup"><span data-stu-id="20ade-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-606">計費貨幣</span><span class="sxs-lookup"><span data-stu-id="20ade-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="20ade-607">客戶地理區域中的貨幣</span><span class="sxs-lookup"><span data-stu-id="20ade-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-608">定價稅前總計</span><span class="sxs-lookup"><span data-stu-id="20ade-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="20ade-609">新增稅額前的價格。</span><span class="sxs-lookup"><span data-stu-id="20ade-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-610">定價貨幣</span><span class="sxs-lookup"><span data-stu-id="20ade-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="20ade-611">價目表中的貨幣。</span><span class="sxs-lookup"><span data-stu-id="20ade-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-612">服務資訊1</span><span class="sxs-lookup"><span data-stu-id="20ade-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="20ade-613">於某一天佈建及使用的 ServiceBus 連線數目。</span><span class="sxs-lookup"><span data-stu-id="20ade-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="20ade-614">服務資訊2</span><span class="sxs-lookup"><span data-stu-id="20ade-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="20ade-615">舊版欄位，可捕捉選擇性的服務特定中繼資料。</span><span class="sxs-lookup"><span data-stu-id="20ade-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="20ade-616">其他資訊</span><span class="sxs-lookup"><span data-stu-id="20ade-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="20ade-617">其他資料行中未涵蓋的任何其他資訊。</span><span class="sxs-lookup"><span data-stu-id="20ade-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="20ade-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="20ade-619">每個單位的實際計費值（包括折扣、獲得點數等等）。</span><span class="sxs-lookup"><span data-stu-id="20ade-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="20ade-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="20ade-621">定價貨幣對（客戶）計費貨幣的匯率。</span><span class="sxs-lookup"><span data-stu-id="20ade-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="20ade-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="20ade-623">決定計費貨幣匯率的定價貨幣。</span><span class="sxs-lookup"><span data-stu-id="20ade-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="20ade-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="20ade-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="20ade-625">代表 Azure subscriptionID。</span><span class="sxs-lookup"><span data-stu-id="20ade-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="20ade-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="20ade-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="20ade-627">代表 Azure 訂用帳戶的名稱。</span><span class="sxs-lookup"><span data-stu-id="20ade-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="20ade-628">發票與對帳檔案之間的對應費用</span><span class="sxs-lookup"><span data-stu-id="20ade-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="20ade-629">您的發票提供費用摘要，而對帳檔案則提供包括費用類型等明細項目交易的詳細細項。</span><span class="sxs-lookup"><span data-stu-id="20ade-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="20ade-630">若要交互參照發票和對帳檔案之間的費用金額，您可以使用 Microsoft Excel 篩選選項，在對帳檔案上依費用類型篩選，以便將發票費用對應到對帳檔案上的一組費用細項。</span><span class="sxs-lookup"><span data-stu-id="20ade-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="20ade-631">用量型和授權型訂閱的對帳檔案只會顯示交易和費用的相關使用量 (耗用單位和相關的費用)。</span><span class="sxs-lookup"><span data-stu-id="20ade-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="20ade-632">對帳檔案不會顯示在發票上顯示為「調整」的一個信用額度、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="20ade-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="20ade-633">下表顯示發票區段和對帳檔案上可能會顯示之相關費用類型之間的對應。</span><span class="sxs-lookup"><span data-stu-id="20ade-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="20ade-634"><strong>發票費用描述</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-635"><strong>對帳檔案費用描述（ChargeType 資料行）</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-636"><strong>這會產生什麼費用？</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-637"><strong>如何? 將這些 ChargeTypes 對應至發票？</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="20ade-638"><strong>以授權為基礎的費用</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-639">啟用費用</span><span class="sxs-lookup"><span data-stu-id="20ade-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-640">當客戶購買後使用訂閱時，向客戶收取的金額</span><span class="sxs-lookup"><span data-stu-id="20ade-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="20ade-641">從授權型檔案，加總 <strong>Amount</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-642">取消費用</span><span class="sxs-lookup"><span data-stu-id="20ade-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-643">當關聯的基座變更時，按比例計算退款給客戶的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-644">循環費用</span><span class="sxs-lookup"><span data-stu-id="20ade-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-645">訂閱的定期費用</span><span class="sxs-lookup"><span data-stu-id="20ade-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-646">循環執行個體 (依比例計算)</span><span class="sxs-lookup"><span data-stu-id="20ade-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-647">當關聯的基座變更時，按比例計算向客戶收取的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-648">取消時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="20ade-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-649">取消時服務未使用部分之按比例計算的退款</span><span class="sxs-lookup"><span data-stu-id="20ade-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-650">購買時按比例計算之費用</span><span class="sxs-lookup"><span data-stu-id="20ade-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-651">使用年度計費時的訂用帳戶費用類型</span><span class="sxs-lookup"><span data-stu-id="20ade-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-652">購買費用</span><span class="sxs-lookup"><span data-stu-id="20ade-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-653">使用每月計費時的訂用帳戶費用類型</span><span class="sxs-lookup"><span data-stu-id="20ade-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-654">續約時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="20ade-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-655">訂閱續約時按比例計算的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="20ade-656">續約費用</span><span class="sxs-lookup"><span data-stu-id="20ade-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-657">訂閱續約時的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-658">啟用時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="20ade-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-659">從啟用到計費期間結束時按比例計算的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="20ade-660"><strong>一次性費用</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="20ade-661">新的</span><span class="sxs-lookup"><span data-stu-id="20ade-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-662">在建立新購買時使用</span><span class="sxs-lookup"><span data-stu-id="20ade-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-664">用於原始購買的退款和增加後的新數量</span><span class="sxs-lookup"><span data-stu-id="20ade-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="20ade-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-666">用於原始購買的退款和減少後的新數量</span><span class="sxs-lookup"><span data-stu-id="20ade-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-667">[取消]</span><span class="sxs-lookup"><span data-stu-id="20ade-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-668">在取消訂用帳戶時使用</span><span class="sxs-lookup"><span data-stu-id="20ade-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-669">轉換</span><span class="sxs-lookup"><span data-stu-id="20ade-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-670">當授權已升級，但基座數目維持不變時使用</span><span class="sxs-lookup"><span data-stu-id="20ade-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="20ade-671"><strong>使用費用</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-672">取消時的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="20ade-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-673">在目前計費期間中取消時，未支付之使用量的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="20ade-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="20ade-674">從用量型檔案，加總 <strong>PretaxCharges</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-675">目前週期的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="20ade-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-676">目前計費期間的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="20ade-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="20ade-677"><strong>信用</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-678">明細項目位移</span><span class="sxs-lookup"><span data-stu-id="20ade-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-679">明細項目的部分或完整退款 (含稅)</span><span class="sxs-lookup"><span data-stu-id="20ade-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-680">從授權型檔案，加總 <strong>TotalForCustomer</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="20ade-681">從用量型檔案，加總 <strong>PostTaxTotal</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="20ade-682"><strong>以使用量為基礎的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-683">啟用折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-684">啟用訂閱時套用的折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="20ade-685">從用量型檔案，加總 <strong>PretaxCharges</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-686">循環折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-687">套用至定期費用的折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-688">續約折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-689">訂閱續約時套用的折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-690">取消折扣</span><span class="sxs-lookup"><span data-stu-id="20ade-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-691">折扣取消時收取的費用</span><span class="sxs-lookup"><span data-stu-id="20ade-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="20ade-692"><strong>以授權為基礎的折扣</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-693"><em>可套用至多個費用類型</em></span><span class="sxs-lookup"><span data-stu-id="20ade-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="20ade-694">從授權型檔案，加總 <strong>TotalOtherDiscount</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="20ade-695"><strong>稅金</strong>&nbsp;或&nbsp;<strong>加值稅</strong></span><span class="sxs-lookup"><span data-stu-id="20ade-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-696"><em>可套用至多個費用類型</em></span><span class="sxs-lookup"><span data-stu-id="20ade-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="20ade-697"><em>例外狀況： &quot;Offset &quot; 已包含稅金的明細專案。請參閱上方的信用額度。</em></span><span class="sxs-lookup"><span data-stu-id="20ade-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-698">稅金或加值稅 (VAT)</span><span class="sxs-lookup"><span data-stu-id="20ade-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="20ade-699">從授權型檔案，加總 <strong>Tax</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="20ade-700">從用量型檔案，加總 <strong>TaxAmount</strong> 欄</span><span class="sxs-lookup"><span data-stu-id="20ade-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
