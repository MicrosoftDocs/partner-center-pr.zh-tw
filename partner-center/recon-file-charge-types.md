---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a><span data-ttu-id="bc9ed-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="bc9ed-103">Understand charge types</span></span>

<span data-ttu-id="bc9ed-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="bc9ed-104">Applies to:</span></span>

- <span data-ttu-id="bc9ed-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="bc9ed-105">Partner Center</span></span>
- <span data-ttu-id="bc9ed-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="bc9ed-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="bc9ed-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="bc9ed-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="bc9ed-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="bc9ed-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="bc9ed-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="bc9ed-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="bc9ed-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="bc9ed-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="bc9ed-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="bc9ed-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="bc9ed-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="bc9ed-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="bc9ed-116">授權型費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-116">License-based charges</span></span>

<span data-ttu-id="bc9ed-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bc9ed-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bc9ed-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="bc9ed-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bc9ed-120">啟用費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-120">Activation fee</span></span> | <span data-ttu-id="bc9ed-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="bc9ed-122">取消費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-122">Cancel fee</span></span> | <span data-ttu-id="bc9ed-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="bc9ed-124">循環費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-124">Cycle fee</span></span> | <span data-ttu-id="bc9ed-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="bc9ed-126">循環執行個體 (依比例計算)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-126">Cycle instance prorate</span></span> | <span data-ttu-id="bc9ed-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="bc9ed-128">取消時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-128">Prorate fees when cancel</span></span> | <span data-ttu-id="bc9ed-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="bc9ed-130">購買時按比例計算之費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-130">Prorate fees when purchase</span></span> | <span data-ttu-id="bc9ed-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="bc9ed-132">購買費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-132">Purchase fee</span></span> | <span data-ttu-id="bc9ed-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="bc9ed-134">續約時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-134">Prorate fee when renew</span></span> | <span data-ttu-id="bc9ed-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="bc9ed-136">續約費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-136">Renew fee</span></span> | <span data-ttu-id="bc9ed-137">訂閱續約時的費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="bc9ed-138">啟用時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-138">Prorate fees when activate</span></span> | <span data-ttu-id="bc9ed-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="bc9ed-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="bc9ed-140">One-time charges</span></span>

<span data-ttu-id="bc9ed-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="bc9ed-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bc9ed-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="bc9ed-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bc9ed-144">新的</span><span class="sxs-lookup"><span data-stu-id="bc9ed-144">New</span></span> | <span data-ttu-id="bc9ed-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="bc9ed-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="bc9ed-146">addQuantity</span></span> | <span data-ttu-id="bc9ed-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="bc9ed-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="bc9ed-148">removeQuantity</span></span> | <span data-ttu-id="bc9ed-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="bc9ed-150">[取消]</span><span class="sxs-lookup"><span data-stu-id="bc9ed-150">Cancel</span></span> | <span data-ttu-id="bc9ed-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="bc9ed-152">轉換</span><span class="sxs-lookup"><span data-stu-id="bc9ed-152">Convert</span></span> | <span data-ttu-id="bc9ed-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="bc9ed-154">使用量費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-154">Usage charges</span></span>

<span data-ttu-id="bc9ed-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bc9ed-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bc9ed-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="bc9ed-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bc9ed-158">取消時的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="bc9ed-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="bc9ed-160">目前週期的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="bc9ed-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="bc9ed-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="bc9ed-162">點數</span><span class="sxs-lookup"><span data-stu-id="bc9ed-162">Credits</span></span>

<span data-ttu-id="bc9ed-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="bc9ed-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="bc9ed-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="bc9ed-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="bc9ed-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bc9ed-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="bc9ed-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bc9ed-168">明細項目位移</span><span class="sxs-lookup"><span data-stu-id="bc9ed-168">Offset a line item</span></span> | <span data-ttu-id="bc9ed-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="bc9ed-170">用量型折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-170">Usage-based discounts</span></span>

<span data-ttu-id="bc9ed-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="bc9ed-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="bc9ed-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="bc9ed-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="bc9ed-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="bc9ed-174">啟用折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-174">Activation discount</span></span> | <span data-ttu-id="bc9ed-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="bc9ed-176">循環折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-176">Cycle discount</span></span> | <span data-ttu-id="bc9ed-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="bc9ed-178">續約折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-178">Renew discount</span></span> | <span data-ttu-id="bc9ed-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="bc9ed-180">取消折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-180">Cancel discount</span></span> | <span data-ttu-id="bc9ed-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="bc9ed-182">授權型折扣</span><span class="sxs-lookup"><span data-stu-id="bc9ed-182">License-based discounts</span></span>

<span data-ttu-id="bc9ed-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="bc9ed-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="bc9ed-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="bc9ed-184">*License-based discounts may be applied to multiple charge types.*</span></span>
