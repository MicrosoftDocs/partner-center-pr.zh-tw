---
title: 對帳檔案收費類型 |合作夥伴中心
ms.topic: article
ms.date: 08/26/2019
description: 合作夥伴中心對帳檔案的費用類型（以授權為基礎、使用方式和一次性）、點數和折扣。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389806"
---
# <a name="understand-charge-types"></a><span data-ttu-id="111ee-103">瞭解費用類型</span><span class="sxs-lookup"><span data-stu-id="111ee-103">Understand charge types</span></span>

<span data-ttu-id="111ee-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="111ee-104">Applies to:</span></span>

- <span data-ttu-id="111ee-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="111ee-105">Partner Center</span></span>
- <span data-ttu-id="111ee-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="111ee-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="111ee-107">本主題描述發票區段與您的對帳檔案上可能的相關收費類型之間的對應。</span><span class="sxs-lookup"><span data-stu-id="111ee-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="111ee-108">您的發票會提供費用的摘要。</span><span class="sxs-lookup"><span data-stu-id="111ee-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="111ee-109">您的對帳檔案提供明細專案交易的詳細細目，包括費用類型。</span><span class="sxs-lookup"><span data-stu-id="111ee-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="111ee-110">如需有關對帳檔案的詳細資訊，請參閱[如何使用對帳](use-the-reconciliation-files.md)檔案。</span><span class="sxs-lookup"><span data-stu-id="111ee-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="111ee-111">以[使用量為基礎的對](usage-based-recon-files.md)帳檔案和以[授權為基礎的對帳](license-based-recon-files.md)檔案，只會顯示使用量相關的交易和費用（耗用的單位和相關費用）。</span><span class="sxs-lookup"><span data-stu-id="111ee-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="111ee-112">對帳檔案中不會顯示顯示在發票上做為**調整**的一次性信用額度、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="111ee-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="111ee-113">將費用類型對應到發票費用</span><span class="sxs-lookup"><span data-stu-id="111ee-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="111ee-114">若要在您的發票和對帳檔案之間交叉參考費用，請使用 Microsoft Excel 中的篩選選項。</span><span class="sxs-lookup"><span data-stu-id="111ee-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="111ee-115">依對帳檔案上的收費類型進行篩選，將發票費用對應至對帳檔案的一組費用明細。</span><span class="sxs-lookup"><span data-stu-id="111ee-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="111ee-116">授權型費用</span><span class="sxs-lookup"><span data-stu-id="111ee-116">License-based charges</span></span>

<span data-ttu-id="111ee-117">若要將這些以授權為基礎的費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="111ee-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="111ee-118">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="111ee-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="111ee-119">收費說明</span><span class="sxs-lookup"><span data-stu-id="111ee-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="111ee-120">啟用費用</span><span class="sxs-lookup"><span data-stu-id="111ee-120">Activation fee</span></span> | <span data-ttu-id="111ee-121">購買後使用訂用帳戶時，向客戶收取的金額。</span><span class="sxs-lookup"><span data-stu-id="111ee-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="111ee-122">取消費用</span><span class="sxs-lookup"><span data-stu-id="111ee-122">Cancel fee</span></span> | <span data-ttu-id="111ee-123">當相關聯的基座變更時，會向客戶收取按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="111ee-124">循環費用</span><span class="sxs-lookup"><span data-stu-id="111ee-124">Cycle fee</span></span> | <span data-ttu-id="111ee-125">訂用帳戶的定期費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="111ee-126">循環執行個體 (依比例計算)</span><span class="sxs-lookup"><span data-stu-id="111ee-126">Cycle instance prorate</span></span> | <span data-ttu-id="111ee-127">當相關聯的基座變更時，從客戶評估的按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="111ee-128">取消時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="111ee-128">Prorate fees when cancel</span></span> | <span data-ttu-id="111ee-129">取消時未使用的服務部分按比例計算。</span><span class="sxs-lookup"><span data-stu-id="111ee-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="111ee-130">購買時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="111ee-130">Prorate fees when purchase</span></span> | <span data-ttu-id="111ee-131">使用年度計費時，訂用帳戶的費用類型。</span><span class="sxs-lookup"><span data-stu-id="111ee-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="111ee-132">購買費用</span><span class="sxs-lookup"><span data-stu-id="111ee-132">Purchase fee</span></span> | <span data-ttu-id="111ee-133">使用每月計費時，訂用帳戶的費用類型。</span><span class="sxs-lookup"><span data-stu-id="111ee-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="111ee-134">續約時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="111ee-134">Prorate fee when renew</span></span> | <span data-ttu-id="111ee-135">訂閱更新時按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="111ee-136">續約費用</span><span class="sxs-lookup"><span data-stu-id="111ee-136">Renew fee</span></span> | <span data-ttu-id="111ee-137">訂閱續約時的費用</span><span class="sxs-lookup"><span data-stu-id="111ee-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="111ee-138">啟用時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="111ee-138">Prorate fees when activate</span></span> | <span data-ttu-id="111ee-139">從啟用到計費週期結束之前，> 按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="111ee-140">一次性費用</span><span class="sxs-lookup"><span data-stu-id="111ee-140">One-time charges</span></span>

<span data-ttu-id="111ee-141">若要將這些一次性費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="111ee-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="111ee-142">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="111ee-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="111ee-143">收費說明</span><span class="sxs-lookup"><span data-stu-id="111ee-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="111ee-144">新增</span><span class="sxs-lookup"><span data-stu-id="111ee-144">New</span></span> | <span data-ttu-id="111ee-145">在建立新購買時使用。</span><span class="sxs-lookup"><span data-stu-id="111ee-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="111ee-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="111ee-146">addQuantity</span></span> | <span data-ttu-id="111ee-147">用於原始購買的退款和增加後的新數量。</span><span class="sxs-lookup"><span data-stu-id="111ee-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="111ee-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="111ee-148">removeQuantity</span></span> | <span data-ttu-id="111ee-149">用於原始購買的退款和減少後的新數量。</span><span class="sxs-lookup"><span data-stu-id="111ee-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="111ee-150">取消</span><span class="sxs-lookup"><span data-stu-id="111ee-150">Cancel</span></span> | <span data-ttu-id="111ee-151">在取消訂用帳戶時使用。</span><span class="sxs-lookup"><span data-stu-id="111ee-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="111ee-152">轉換</span><span class="sxs-lookup"><span data-stu-id="111ee-152">Convert</span></span> | <span data-ttu-id="111ee-153">當授權升級，但基座數目維持不變時使用。</span><span class="sxs-lookup"><span data-stu-id="111ee-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="111ee-154">使用量費用</span><span class="sxs-lookup"><span data-stu-id="111ee-154">Usage charges</span></span>

<span data-ttu-id="111ee-155">若要將這些使用量費用對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="111ee-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="111ee-156">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="111ee-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="111ee-157">收費說明</span><span class="sxs-lookup"><span data-stu-id="111ee-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="111ee-158">取消時的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="111ee-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="111ee-159">在目前計費期間，取消未付款使用量時，存取使用費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="111ee-160">目前週期的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="111ee-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="111ee-161">存取目前計費週期的使用費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="111ee-162">點數</span><span class="sxs-lookup"><span data-stu-id="111ee-162">Credits</span></span>

<span data-ttu-id="111ee-163">若要將這些點數對應至您的發票：</span><span class="sxs-lookup"><span data-stu-id="111ee-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="111ee-164">加總以授權為基礎的檔案中的**TotalForCustomer** 。</span><span class="sxs-lookup"><span data-stu-id="111ee-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="111ee-165">加總以使用方式為基礎之檔案中的**PostTaxTotal**資料行。</span><span class="sxs-lookup"><span data-stu-id="111ee-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="111ee-166">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="111ee-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="111ee-167">收費說明</span><span class="sxs-lookup"><span data-stu-id="111ee-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="111ee-168">明細項目位移</span><span class="sxs-lookup"><span data-stu-id="111ee-168">Offset a line item</span></span> | <span data-ttu-id="111ee-169">明細專案的部分或全部退款，包括稅金。</span><span class="sxs-lookup"><span data-stu-id="111ee-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="111ee-170">用量型折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-170">Usage-based discounts</span></span>

<span data-ttu-id="111ee-171">若要將這些以使用量為基礎的折扣對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="111ee-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="111ee-172">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="111ee-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="111ee-173">收費說明</span><span class="sxs-lookup"><span data-stu-id="111ee-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="111ee-174">啟用折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-174">Activation discount</span></span> | <span data-ttu-id="111ee-175">啟用訂用帳戶時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="111ee-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="111ee-176">循環折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-176">Cycle discount</span></span> | <span data-ttu-id="111ee-177">定期費用所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="111ee-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="111ee-178">續約折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-178">Renew discount</span></span> | <span data-ttu-id="111ee-179">更新訂閱時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="111ee-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="111ee-180">取消折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-180">Cancel discount</span></span> | <span data-ttu-id="111ee-181">取消折扣時所套用的費用。</span><span class="sxs-lookup"><span data-stu-id="111ee-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="111ee-182">授權型折扣</span><span class="sxs-lookup"><span data-stu-id="111ee-182">License-based discounts</span></span>

<span data-ttu-id="111ee-183">若要將以授權為基礎的折扣對應至您的發票，請將**TotalOtherDiscount**資料行與授權檔加總。</span><span class="sxs-lookup"><span data-stu-id="111ee-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="111ee-184">*以授權為基礎的折扣可能適用于多種費用類型。*</span><span class="sxs-lookup"><span data-stu-id="111ee-184">*License-based discounts may be applied to multiple charge types.*</span></span>
