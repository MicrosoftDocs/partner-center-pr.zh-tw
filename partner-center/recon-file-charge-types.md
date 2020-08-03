---
title: 對帳檔案費用類型
ms.topic: article
ms.date: 06/05/2020
description: 探索合作夥伴中心對帳檔案中的費用類型（例如，以授權為基礎、以使用量為基礎和一次性）、點數和折扣。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c12bd8b08f3f72c42d788cb677888a7e3cde85a5
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444771"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="e3afc-103">瞭解合作夥伴中心對帳檔案中的不同費用類型</span><span class="sxs-lookup"><span data-stu-id="e3afc-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="e3afc-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="e3afc-104">**Applies to**</span></span>

- <span data-ttu-id="e3afc-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e3afc-105">Partner Center</span></span>
- <span data-ttu-id="e3afc-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e3afc-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e3afc-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="e3afc-107">**Appropriate roles**</span></span>

- <span data-ttu-id="e3afc-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="e3afc-108">Admin agent</span></span>
- <span data-ttu-id="e3afc-109">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="e3afc-109">Billing admin</span></span>
- <span data-ttu-id="e3afc-110">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="e3afc-110">Global admin</span></span>

<span data-ttu-id="e3afc-111">本主題描述發票區段與您的對帳檔案上可能的相關收費類型之間的對應。</span><span class="sxs-lookup"><span data-stu-id="e3afc-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e3afc-112">您的發票會提供費用的摘要。</span><span class="sxs-lookup"><span data-stu-id="e3afc-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e3afc-113">您的對帳檔案提供明細專案交易的詳細細目，包括費用類型。</span><span class="sxs-lookup"><span data-stu-id="e3afc-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e3afc-114">如需有關對帳檔案的詳細資訊，請參閱[如何使用對帳](use-the-reconciliation-files.md)檔案。</span><span class="sxs-lookup"><span data-stu-id="e3afc-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e3afc-115">以[使用量為基礎的對](usage-based-recon-files.md)帳檔案和以[授權為基礎的對帳](license-based-recon-files.md)檔案，只會顯示使用量相關的交易和費用（耗用的單位和相關費用）。</span><span class="sxs-lookup"><span data-stu-id="e3afc-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e3afc-116">對帳檔案中不會顯示顯示在發票上做為**調整**的一次性信用額度、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="e3afc-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e3afc-117">將費用類型對應到發票費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="e3afc-118">若要在您的發票和對帳檔案之間交叉參考費用，請使用 Microsoft Excel 中的篩選選項。</span><span class="sxs-lookup"><span data-stu-id="e3afc-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e3afc-119">依對帳檔案上的收費類型進行篩選，將發票費用對應至對帳檔案的一組費用明細。</span><span class="sxs-lookup"><span data-stu-id="e3afc-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e3afc-120">授權型費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-120">License-based charges</span></span>

<span data-ttu-id="e3afc-121">若要將這些以授權為基礎的費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="e3afc-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e3afc-122">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="e3afc-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e3afc-123">收費說明</span><span class="sxs-lookup"><span data-stu-id="e3afc-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e3afc-124">啟用費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-124">Activation fee</span></span> | <span data-ttu-id="e3afc-125">購買後使用訂用帳戶時，向客戶收取的金額。</span><span class="sxs-lookup"><span data-stu-id="e3afc-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e3afc-126">取消費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-126">Cancel fee</span></span> | <span data-ttu-id="e3afc-127">當相關聯的授權變更時，會向客戶收取按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e3afc-128">取消執行個體按比例計算</span><span class="sxs-lookup"><span data-stu-id="e3afc-128">Cancel instance prorate</span></span> | <span data-ttu-id="e3afc-129">當具有每月訂用帳戶的客戶已暫停訂閱且相關聯的授權在同一個月內變更時，已取消按比例</span><span class="sxs-lookup"><span data-stu-id="e3afc-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="e3afc-130">循環費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-130">Cycle fee</span></span> | <span data-ttu-id="e3afc-131">訂用帳戶的定期費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e3afc-132">循環執行個體 (依比例計算)</span><span class="sxs-lookup"><span data-stu-id="e3afc-132">Cycle instance prorate</span></span> | <span data-ttu-id="e3afc-133">當相關聯的授權變更時，從客戶評估的按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="e3afc-134">取消時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-134">Prorate fees when cancel</span></span> | <span data-ttu-id="e3afc-135">取消時未使用的服務部分按比例計算。</span><span class="sxs-lookup"><span data-stu-id="e3afc-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e3afc-136">從目前的供應專案轉換時依比例分配費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="e3afc-137">從目前每月訂用帳戶轉換為年度訂閱之後，按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="e3afc-138">轉換成新的供應專案時依比例分配費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="e3afc-139">將每月訂閱轉換為新年度訂閱之後，按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="e3afc-140">購買時按比例計算之費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-140">Prorate fees when purchase</span></span> | <span data-ttu-id="e3afc-141">使用年度計費時，訂用帳戶的費用類型。</span><span class="sxs-lookup"><span data-stu-id="e3afc-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="e3afc-142">購買費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-142">Purchase fee</span></span> | <span data-ttu-id="e3afc-143">使用每月計費時，訂用帳戶的費用類型。</span><span class="sxs-lookup"><span data-stu-id="e3afc-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="e3afc-144">續約時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-144">Prorate fee when renew</span></span> | <span data-ttu-id="e3afc-145">訂閱更新時按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e3afc-146">續約費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-146">Renew fee</span></span> | <span data-ttu-id="e3afc-147">訂閱續約時的費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e3afc-148">啟用時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-148">Prorate fees when activate</span></span> | <span data-ttu-id="e3afc-149">從啟用到計費週期結束之前按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e3afc-150">一次性費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-150">One-time charges</span></span>

<span data-ttu-id="e3afc-151">若要將這些一次性費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="e3afc-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e3afc-152">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="e3afc-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e3afc-153">收費說明</span><span class="sxs-lookup"><span data-stu-id="e3afc-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e3afc-154">新增</span><span class="sxs-lookup"><span data-stu-id="e3afc-154">New</span></span> | <span data-ttu-id="e3afc-155">在建立新購買時使用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e3afc-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e3afc-156">addQuantity</span></span> | <span data-ttu-id="e3afc-157">用於原始購買的退款和增加後的新數量。</span><span class="sxs-lookup"><span data-stu-id="e3afc-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e3afc-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e3afc-158">removeQuantity</span></span> | <span data-ttu-id="e3afc-159">用於原始購買的退款和減少後的新數量。</span><span class="sxs-lookup"><span data-stu-id="e3afc-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e3afc-160">取消</span><span class="sxs-lookup"><span data-stu-id="e3afc-160">Cancel</span></span> | <span data-ttu-id="e3afc-161">在取消訂用帳戶時使用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="e3afc-162">轉換</span><span class="sxs-lookup"><span data-stu-id="e3afc-162">Convert</span></span> | <span data-ttu-id="e3afc-163">當授權升級，但授權數目維持不變時使用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-163">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e3afc-164">使用費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-164">Usage charges</span></span>

<span data-ttu-id="e3afc-165">若要將這些使用量費用對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="e3afc-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e3afc-166">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="e3afc-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e3afc-167">收費說明</span><span class="sxs-lookup"><span data-stu-id="e3afc-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e3afc-168">取消時的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="e3afc-169">存取在取消目前計費期間未付費使用量時的使用費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e3afc-170">目前週期的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="e3afc-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e3afc-171">存取目前計費期間的使用費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e3afc-172">學分</span><span class="sxs-lookup"><span data-stu-id="e3afc-172">Credits</span></span>

<span data-ttu-id="e3afc-173">若要將這些點數對應至您的發票：</span><span class="sxs-lookup"><span data-stu-id="e3afc-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e3afc-174">加總以授權為基礎的檔案中的**TotalForCustomer** 。</span><span class="sxs-lookup"><span data-stu-id="e3afc-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e3afc-175">加總以使用方式為基礎之檔案中的**PostTaxTotal**資料行。</span><span class="sxs-lookup"><span data-stu-id="e3afc-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e3afc-176">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="e3afc-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e3afc-177">收費說明</span><span class="sxs-lookup"><span data-stu-id="e3afc-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e3afc-178">明細項目位移</span><span class="sxs-lookup"><span data-stu-id="e3afc-178">Offset a line item</span></span> | <span data-ttu-id="e3afc-179">明細項目的部分或完整退款，包括稅額。</span><span class="sxs-lookup"><span data-stu-id="e3afc-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e3afc-180">用量型折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-180">Usage-based discounts</span></span>

<span data-ttu-id="e3afc-181">若要將這些以使用量為基礎的折扣對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="e3afc-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e3afc-182">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="e3afc-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e3afc-183">收費說明</span><span class="sxs-lookup"><span data-stu-id="e3afc-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e3afc-184">啟用折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-184">Activation discount</span></span> | <span data-ttu-id="e3afc-185">啟用訂用帳戶時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="e3afc-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e3afc-186">循環折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-186">Cycle discount</span></span> | <span data-ttu-id="e3afc-187">週期性費用所適用的折扣。</span><span class="sxs-lookup"><span data-stu-id="e3afc-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e3afc-188">續約折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-188">Renew discount</span></span> | <span data-ttu-id="e3afc-189">更新訂閱時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="e3afc-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e3afc-190">取消折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-190">Cancel discount</span></span> | <span data-ttu-id="e3afc-191">當折扣取消時所適用的費用。</span><span class="sxs-lookup"><span data-stu-id="e3afc-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e3afc-192">授權型折扣</span><span class="sxs-lookup"><span data-stu-id="e3afc-192">License-based discounts</span></span>

<span data-ttu-id="e3afc-193">若要將以授權為基礎的折扣對應至您的發票，請將**TotalOtherDiscount**資料行與授權檔加總。</span><span class="sxs-lookup"><span data-stu-id="e3afc-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e3afc-194">*以授權為基礎的折扣可能適用于多種費用類型。*</span><span class="sxs-lookup"><span data-stu-id="e3afc-194">*License-based discounts may be applied to multiple charge types.*</span></span>
