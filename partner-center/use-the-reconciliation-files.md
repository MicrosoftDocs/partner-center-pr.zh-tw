---
title: 使用您的對帳檔案
ms.topic: article
ms.date: 06/08/2020
description: 瞭解合作夥伴中心的對帳檔案，以及如何解讀特定計費週期的詳細、明細專案的費用觀點。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a53a0f3d37183c67d5d1d44472192ed15f6ed62e
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/09/2020
ms.locfileid: "84603797"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="a35e3-103">瞭解如何讀取合作夥伴中心對帳檔案中的明細專案</span><span class="sxs-lookup"><span data-stu-id="a35e3-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="a35e3-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="a35e3-104">Applies to:</span></span>

- <span data-ttu-id="a35e3-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a35e3-105">Partner Center</span></span>
- <span data-ttu-id="a35e3-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a35e3-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="a35e3-107">您可以從合作夥伴中心下載您的對帳檔案，以取得計費週期中每個費用的詳細明細專案。</span><span class="sxs-lookup"><span data-stu-id="a35e3-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="a35e3-108">明細專案詳細資料包括每個客戶的訂用帳戶的費用，以及詳細的事件（例如，將基座加入訂用帳戶中）。</span><span class="sxs-lookup"><span data-stu-id="a35e3-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

<span data-ttu-id="a35e3-109">適當的角色：</span><span class="sxs-lookup"><span data-stu-id="a35e3-109">Appropriate roles:</span></span>

- <span data-ttu-id="a35e3-110">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="a35e3-110">Billing admin</span></span>
- <span data-ttu-id="a35e3-111">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a35e3-111">Global admin</span></span>

<span data-ttu-id="a35e3-112">如需有關如何讀取**發票**的詳細資訊，請參閱[閱讀您的帳單](read-your-bill.md)。</span><span class="sxs-lookup"><span data-stu-id="a35e3-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="a35e3-113">瞭解對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="a35e3-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="a35e3-114">以授權為基礎的對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="a35e3-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="a35e3-115">基於使用方式的對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="a35e3-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="a35e3-116">一次性和週期性的對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="a35e3-116">One-time and recurring reconciliation file fields</span></span>](one-time-recurring-recon-files.md)
- [<span data-ttu-id="a35e3-117">每日評分的使用量對帳檔案欄位</span><span class="sxs-lookup"><span data-stu-id="a35e3-117">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="a35e3-118">瞭解對帳檔案中的收費類型</span><span class="sxs-lookup"><span data-stu-id="a35e3-118">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="a35e3-119">若要瞭解對帳檔案中的費用類型（ **ChargeType**資料行），請參閱[對帳檔案費用類型](recon-file-charge-types.md)。</span><span class="sxs-lookup"><span data-stu-id="a35e3-119">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="a35e3-120">修正格式問題</span><span class="sxs-lookup"><span data-stu-id="a35e3-120">Fix formatting issues</span></span>

<span data-ttu-id="a35e3-121">對帳檔案有時可能會包含格式問題。</span><span class="sxs-lookup"><span data-stu-id="a35e3-121">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="a35e3-122">例如，如果未使用 en-us 地區設定，則可能會發生此問題。</span><span class="sxs-lookup"><span data-stu-id="a35e3-122">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="a35e3-123">請遵循下列步驟來修正對帳檔案中的任何格式設定問題：</span><span class="sxs-lookup"><span data-stu-id="a35e3-123">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="a35e3-124">在 Microsoft Excel 中開啟對帳檔案（格式為 .csv）。</span><span class="sxs-lookup"><span data-stu-id="a35e3-124">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="a35e3-125">選取檔案中的第一個資料行。</span><span class="sxs-lookup"><span data-stu-id="a35e3-125">Select the first column in the file.</span></span>
3. <span data-ttu-id="a35e3-126">開啟 [**將文字轉換成資料行] Wizard**。</span><span class="sxs-lookup"><span data-stu-id="a35e3-126">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="a35e3-127">在功能區上，選取 [**資料**]，然後選取 [**文字到資料行**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-127">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="a35e3-128">在嚮導中，選取 [**分隔檔案類型**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-128">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="a35e3-129">然後，選取 [下一步]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-129">Then, select **Next**.</span></span>
5. <span data-ttu-id="a35e3-130">在 [**分隔符號**] 欄位中，選取 [**逗號**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-130">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="a35e3-131">（如果已選取索引標籤，您可以將此選項保留為 [已選取 **]** ）。然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="a35e3-131">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="a35e3-132">在 [**資料行資料格式**] 欄位中，選取 [**日期： MDY**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-132">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="a35e3-133">然後，選取 [下一步]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-133">Then, select **Next**.</span></span>
7. <span data-ttu-id="a35e3-134">在 [**資料行資料格式**] 欄位中，針對 [所有數量] 資料行選取 [**文字**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-134">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="a35e3-135">然後，選取 [完成]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-135">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="a35e3-136">以程式設計方式下載對帳檔案</span><span class="sxs-lookup"><span data-stu-id="a35e3-136">Download reconciliation files programmatically</span></span>

<span data-ttu-id="a35e3-137">對帳檔案可能非常大，有時很難以下載。</span><span class="sxs-lookup"><span data-stu-id="a35e3-137">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="a35e3-138">若要以程式設計方式下載對帳檔案，請參閱[取得發票明細專案](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。</span><span class="sxs-lookup"><span data-stu-id="a35e3-138">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="a35e3-139">地圖稅額或 加值稅</span><span class="sxs-lookup"><span data-stu-id="a35e3-139">Map taxes or VAT</span></span>

<span data-ttu-id="a35e3-140">若要將稅金或加值稅（加值稅）對應到您的發票：</span><span class="sxs-lookup"><span data-stu-id="a35e3-140">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="a35e3-141">加總以授權為基礎的檔案中的**稅務**資料行。</span><span class="sxs-lookup"><span data-stu-id="a35e3-141">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="a35e3-142">加總以使用方式為基礎之檔案中的**TaxAmount**資料行。</span><span class="sxs-lookup"><span data-stu-id="a35e3-142">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="a35e3-143">依合作夥伴的逐條對帳檔案</span><span class="sxs-lookup"><span data-stu-id="a35e3-143">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="a35e3-144">**間接模型**中的合作夥伴可以在以授權為基礎和以使用量為基礎的對帳檔案中使用這些額外的欄位，以根據轉售商將檔案加上。</span><span class="sxs-lookup"><span data-stu-id="a35e3-144">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="a35e3-145">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="a35e3-145">MPN ID</span></span> | <span data-ttu-id="a35e3-146">描述</span><span class="sxs-lookup"><span data-stu-id="a35e3-146">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="a35e3-147">MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="a35e3-147">MPN ID</span></span> | <span data-ttu-id="a35e3-148">雲端解決方案提供者（CSP）合作夥伴（直接或間接）的 Microsoft 合作夥伴網路（MPN）識別碼。</span><span class="sxs-lookup"><span data-stu-id="a35e3-148">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="a35e3-149">經銷商 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="a35e3-149">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="a35e3-150">訂用帳戶[之記錄轉銷商的 MPN 識別碼](#reseller-mpn-id)。</span><span class="sxs-lookup"><span data-stu-id="a35e3-150">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="a35e3-151">此欄位對應至合作夥伴中心內的特定訂用帳戶所列的轉售商識別碼。</span><span class="sxs-lookup"><span data-stu-id="a35e3-151">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="a35e3-152">只會出現在間接模型合作夥伴的對帳檔案上。</span><span class="sxs-lookup"><span data-stu-id="a35e3-152">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="a35e3-153">經銷商 MPN 識別碼</span><span class="sxs-lookup"><span data-stu-id="a35e3-153">Reseller MPN ID</span></span>

<span data-ttu-id="a35e3-154">如果 CSP 合作夥伴直接將訂用帳戶銷售給客戶，其**MPN 識別碼**會列出兩次，同時做為**MPN 識別碼**和**轉售商 MPN 識別碼**。</span><span class="sxs-lookup"><span data-stu-id="a35e3-154">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="a35e3-155">如果 CSP 合作夥伴具有沒有**MPN 識別碼**的轉銷商，此值會改為設定為合作夥伴的**MPN 識別碼**。</span><span class="sxs-lookup"><span data-stu-id="a35e3-155">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="a35e3-156">如果 CSP 合作夥伴移除**轉售商 MPN 識別碼**，此值將會設定為 *-1*。</span><span class="sxs-lookup"><span data-stu-id="a35e3-156">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="a35e3-157">若要查看或更新**轉售商 MPN 識別碼**：</span><span class="sxs-lookup"><span data-stu-id="a35e3-157">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="a35e3-158">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a35e3-158">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="a35e3-159">在 [合作夥伴中心] 功能表中，選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-159">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="a35e3-160">從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a35e3-160">Choose the customer from the list.</span></span>
4. <span data-ttu-id="a35e3-161">在 [客戶] 功能表中，選取 [**訂閱**]。</span><span class="sxs-lookup"><span data-stu-id="a35e3-161">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="a35e3-162">從清單中選擇訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a35e3-162">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="a35e3-163">選取 \[更新\]\*\*\*\* 以變更 \[經銷商 (MPN 識別碼)\]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="a35e3-163">Select **update** to change the **Reseller (MPN ID)**.</span></span>
