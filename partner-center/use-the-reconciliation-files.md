---
title: 使用您的對帳檔案
ms.topic: article
ms.date: 03/10/2021
description: 深入瞭解合作夥伴中心的對帳檔案，以及如何針對指定的計費週期，解讀詳細的明細專案查看費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022769"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="2951d-103">瞭解如何讀取合作夥伴中心對帳檔案中的明細專案</span><span class="sxs-lookup"><span data-stu-id="2951d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="2951d-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="2951d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="2951d-105">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="2951d-105">Billing admin</span></span>
- <span data-ttu-id="2951d-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="2951d-106">Global admin</span></span>

<span data-ttu-id="2951d-107">您可以從合作夥伴中心下載您的對帳檔案，以取得計費週期中每個費用的詳細明細專案視圖。</span><span class="sxs-lookup"><span data-stu-id="2951d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="2951d-108">明細專案詳細資料包含每個客戶訂用帳戶的費用，以及詳細的事件 (例如，將授權新增至訂用帳戶) 。</span><span class="sxs-lookup"><span data-stu-id="2951d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="2951d-109">如需有關如何讀取 **發票** 的詳細資訊，請參閱 [閱讀帳單](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="2951d-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="2951d-110">瞭解對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="2951d-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="2951d-111">授權型對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="2951d-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="2951d-112">使用量型對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="2951d-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="2951d-113">每日評分的使用量對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="2951d-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="2951d-114">一次性購買 CSP 對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="2951d-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="2951d-115">瞭解對帳檔案中的費用類型</span><span class="sxs-lookup"><span data-stu-id="2951d-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="2951d-116">若要瞭解對帳檔案中的費用類型 (**ChargeType** 資料行) ，請參閱 [對帳檔案費用類型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="2951d-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="2951d-117">修正格式化問題</span><span class="sxs-lookup"><span data-stu-id="2951d-117">Fix formatting issues</span></span>

<span data-ttu-id="2951d-118">有時，對帳檔案可能會包含格式化問題。</span><span class="sxs-lookup"><span data-stu-id="2951d-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="2951d-119">例如，如果未使用 en-us 地區設定，就可能發生此問題。</span><span class="sxs-lookup"><span data-stu-id="2951d-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="2951d-120">請遵循下列步驟來修正對帳檔案中的任何格式問題：</span><span class="sxs-lookup"><span data-stu-id="2951d-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="2951d-121">在 Microsoft Excel 中，以 .csv 格式) 開啟對帳檔案 (。</span><span class="sxs-lookup"><span data-stu-id="2951d-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="2951d-122">選取檔案中的第一個資料行。</span><span class="sxs-lookup"><span data-stu-id="2951d-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="2951d-123">開啟 [ **將文字轉換成資料行] Wizard**。</span><span class="sxs-lookup"><span data-stu-id="2951d-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="2951d-124">在功能區上，選取 [ **資料**]，然後選取 [ **文字至資料行**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="2951d-125">在嚮導中，選取 [ **分隔檔案類型**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="2951d-126">然後，選取 [下一步]  。</span><span class="sxs-lookup"><span data-stu-id="2951d-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="2951d-127">在 [ **分隔符號** ] 欄位中，選取 [ **逗號**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="2951d-128"> (如果 **已** 選取索引標籤，您可以將此選項保留為已選取狀態。 ) 然後選取 **[下一步**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="2951d-129">在 [ **資料行資料格式** ] 欄位中，選取 [ **日期： MDY**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="2951d-130">然後，選取 [下一步]  。</span><span class="sxs-lookup"><span data-stu-id="2951d-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="2951d-131">在 [ **資料行資料格式** ] 欄位中，選取 [所有數量] 資料行的 [ **文字** ]。</span><span class="sxs-lookup"><span data-stu-id="2951d-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="2951d-132">然後選取 [完成]。</span><span class="sxs-lookup"><span data-stu-id="2951d-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="2951d-133">以程式設計方式下載對帳檔案</span><span class="sxs-lookup"><span data-stu-id="2951d-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="2951d-134">對帳檔案可能很大，有時很難下載。</span><span class="sxs-lookup"><span data-stu-id="2951d-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="2951d-135">若要以程式設計方式下載對帳檔案，請參閱 [取得發票明細專案](/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="2951d-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="2951d-136">地圖稅或 加值稅</span><span class="sxs-lookup"><span data-stu-id="2951d-136">Map taxes or VAT</span></span>

<span data-ttu-id="2951d-137">若要將稅金或加值稅 (加值稅) 對應至您的發票：</span><span class="sxs-lookup"><span data-stu-id="2951d-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="2951d-138">以授權為基礎的檔案加總 **稅額** 資料行。</span><span class="sxs-lookup"><span data-stu-id="2951d-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="2951d-139">加總以使用量為基礎之檔案中的 **TaxAmount** 資料行。</span><span class="sxs-lookup"><span data-stu-id="2951d-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="2951d-140">依夥伴進行對帳檔案的匯總</span><span class="sxs-lookup"><span data-stu-id="2951d-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="2951d-141">**間接模型** 中的合作夥伴可以在以授權為基礎和以使用量為基礎的對帳檔案中使用這些額外欄位，以依轉銷商將檔案加上詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="2951d-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="2951d-142">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="2951d-142">MPN ID</span></span> | <span data-ttu-id="2951d-143">Description</span><span class="sxs-lookup"><span data-stu-id="2951d-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="2951d-144">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="2951d-144">MPN ID</span></span> | <span data-ttu-id="2951d-145">Microsoft 合作夥伴網路 (MPN 雲端解決方案提供者的) 識別碼 (CSP) 合作夥伴 (直接或間接) 。</span><span class="sxs-lookup"><span data-stu-id="2951d-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="2951d-146">經銷商 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="2951d-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="2951d-147">訂用帳戶 [之記錄轉銷商的 MPN 識別碼](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="2951d-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="2951d-148">此欄位對應至合作夥伴中心內特定訂用帳戶所列的轉售商識別碼。</span><span class="sxs-lookup"><span data-stu-id="2951d-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="2951d-149">只會出現在間接模型合作夥伴的對帳檔案上。</span><span class="sxs-lookup"><span data-stu-id="2951d-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="2951d-150">經銷商 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="2951d-150">Reseller MPN ID</span></span>

<span data-ttu-id="2951d-151">如果 CSP 合作夥伴將訂用帳戶直接銷售給客戶，則會將其 **MPN 識別碼** 列為 **MPN 識別碼** 和 **轉售商 MPN 識別碼** 兩次。</span><span class="sxs-lookup"><span data-stu-id="2951d-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="2951d-152">如果 CSP 合作夥伴的轉銷商沒有 **MPN 識別碼**，此值會改為設定為夥伴的 **MPN 識別碼** 。</span><span class="sxs-lookup"><span data-stu-id="2951d-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="2951d-153">如果 CSP 合作夥伴移除 **轉售商 MPN 識別碼**，此值會設定為 *-1*。</span><span class="sxs-lookup"><span data-stu-id="2951d-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="2951d-154">若要查看或更新 **轉售商 MPN 識別碼**：</span><span class="sxs-lookup"><span data-stu-id="2951d-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="2951d-155">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="2951d-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="2951d-156">在 [合作夥伴中心] 功能表中，選取 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="2951d-157">從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="2951d-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="2951d-158">在 [客戶] 功能表中，選取 [ **訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="2951d-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="2951d-159">從清單中選擇訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="2951d-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="2951d-160">選取 \[更新\] 以變更 \[經銷商 (MPN 識別碼)\]。</span><span class="sxs-lookup"><span data-stu-id="2951d-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2951d-161">下一步</span><span class="sxs-lookup"><span data-stu-id="2951d-161">Next steps</span></span>

- [<span data-ttu-id="2951d-162">如何讀取帳單 & 偵察檔</span><span class="sxs-lookup"><span data-stu-id="2951d-162">How to read your bill & recon file</span></span>](read-your-bill.md) 