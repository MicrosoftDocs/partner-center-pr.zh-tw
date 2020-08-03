---
title: 對帳檔案費用類型
ms.topic: article
ms.date: 06/05/2020
description: 探索合作夥伴中心對帳檔案中的費用類型（例如，以授權為基礎、以使用量為基礎和一次性）、點數和折扣。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f65c4a6496082934e8c38fbd924b96ef969be95b
ms.sourcegitcommit: e7931fbe7ce16a62124e00b2802520a17d7285b8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/31/2020
ms.locfileid: "87479111"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="c842b-103">瞭解合作夥伴中心對帳檔案中的不同費用類型</span><span class="sxs-lookup"><span data-stu-id="c842b-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="c842b-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="c842b-104">**Applies to**</span></span>

- <span data-ttu-id="c842b-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="c842b-105">Partner Center</span></span>
- <span data-ttu-id="c842b-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="c842b-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c842b-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="c842b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="c842b-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="c842b-108">Admin agent</span></span>
- <span data-ttu-id="c842b-109">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="c842b-109">Billing admin</span></span>
- <span data-ttu-id="c842b-110">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="c842b-110">Global admin</span></span>

<span data-ttu-id="c842b-111">本主題描述發票區段與您的對帳檔案上可能的相關收費類型之間的對應。</span><span class="sxs-lookup"><span data-stu-id="c842b-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="c842b-112">您的發票會提供費用的摘要。</span><span class="sxs-lookup"><span data-stu-id="c842b-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="c842b-113">您的對帳檔案提供明細專案交易的詳細細目，包括費用類型。</span><span class="sxs-lookup"><span data-stu-id="c842b-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="c842b-114">如需有關對帳檔案的詳細資訊，請參閱[如何使用對帳](use-the-reconciliation-files.md)檔案。</span><span class="sxs-lookup"><span data-stu-id="c842b-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="c842b-115">以[使用量為基礎的對](usage-based-recon-files.md)帳檔案和以[授權為基礎的對帳](license-based-recon-files.md)檔案，只會顯示使用量相關的交易和費用（耗用的單位和相關費用）。</span><span class="sxs-lookup"><span data-stu-id="c842b-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="c842b-116">對帳檔案中不會顯示顯示在發票上做為**調整**的一次性信用額度、折扣或退款。</span><span class="sxs-lookup"><span data-stu-id="c842b-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="c842b-117">將費用類型對應到發票費用</span><span class="sxs-lookup"><span data-stu-id="c842b-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="c842b-118">若要在您的發票和對帳檔案之間交叉參考費用，請使用 Microsoft Excel 中的篩選選項。</span><span class="sxs-lookup"><span data-stu-id="c842b-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="c842b-119">依對帳檔案上的收費類型進行篩選，將發票費用對應至對帳檔案的一組費用明細。</span><span class="sxs-lookup"><span data-stu-id="c842b-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="c842b-120">授權型費用</span><span class="sxs-lookup"><span data-stu-id="c842b-120">License-based charges</span></span>

<span data-ttu-id="c842b-121">若要將這些以授權為基礎的費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="c842b-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="c842b-122">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="c842b-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c842b-123">收費說明</span><span class="sxs-lookup"><span data-stu-id="c842b-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c842b-124">啟用費用</span><span class="sxs-lookup"><span data-stu-id="c842b-124">Activation fee</span></span> | <span data-ttu-id="c842b-125">購買後使用訂用帳戶時，向客戶收取的金額。</span><span class="sxs-lookup"><span data-stu-id="c842b-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="c842b-126">取消費用</span><span class="sxs-lookup"><span data-stu-id="c842b-126">Cancel fee</span></span> | <span data-ttu-id="c842b-127">當相關聯的授權變更時，會向客戶收取按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-127">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="c842b-128">取消執行個體按比例計算</span><span class="sxs-lookup"><span data-stu-id="c842b-128">Cancel instance prorate</span></span> | <span data-ttu-id="c842b-129">當具有每月訂用帳戶的客戶已暫停訂閱且相關聯的授權在同一個月內變更時，已取消按比例</span><span class="sxs-lookup"><span data-stu-id="c842b-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="c842b-130">循環費用</span><span class="sxs-lookup"><span data-stu-id="c842b-130">Cycle fee</span></span> | <span data-ttu-id="c842b-131">訂用帳戶的定期費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="c842b-132">循環執行個體 (依比例計算)</span><span class="sxs-lookup"><span data-stu-id="c842b-132">Cycle instance prorate</span></span> | <span data-ttu-id="c842b-133">當相關聯的授權變更時，從客戶評估的按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-133">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="c842b-134">取消時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="c842b-134">Prorate fees when cancel</span></span> | <span data-ttu-id="c842b-135">取消時未使用的服務部分按比例計算。</span><span class="sxs-lookup"><span data-stu-id="c842b-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="c842b-136">從目前的供應專案轉換時依比例分配費用</span><span class="sxs-lookup"><span data-stu-id="c842b-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="c842b-137">從目前每月訂用帳戶轉換為年度訂閱之後，按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="c842b-138">轉換成新的供應專案時依比例分配費用</span><span class="sxs-lookup"><span data-stu-id="c842b-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="c842b-139">將每月訂閱轉換為新年度訂閱之後，按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="c842b-140">購買時按比例計算之費用</span><span class="sxs-lookup"><span data-stu-id="c842b-140">Prorate fees when purchase</span></span> | <span data-ttu-id="c842b-141">使用每月或年度計費時的訂用帳戶費用類型。</span><span class="sxs-lookup"><span data-stu-id="c842b-141">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="c842b-142">續約時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="c842b-142">Prorate fee when renew</span></span> | <span data-ttu-id="c842b-143">訂閱更新時按比例計算費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-143">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="c842b-144">續約費用</span><span class="sxs-lookup"><span data-stu-id="c842b-144">Renew fee</span></span> | <span data-ttu-id="c842b-145">訂閱續約時的費用</span><span class="sxs-lookup"><span data-stu-id="c842b-145">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="c842b-146">啟用時按比例計算費用</span><span class="sxs-lookup"><span data-stu-id="c842b-146">Prorate fees when activate</span></span> | <span data-ttu-id="c842b-147">從啟用到計費週期結束之前按比例計算的費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-147">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="c842b-148">一次性費用</span><span class="sxs-lookup"><span data-stu-id="c842b-148">One-time charges</span></span>

<span data-ttu-id="c842b-149">若要將這些一次性費用對應到您的發票，請加總以授權為基礎的檔案中的**金額**資料行。</span><span class="sxs-lookup"><span data-stu-id="c842b-149">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="c842b-150">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="c842b-150">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c842b-151">收費說明</span><span class="sxs-lookup"><span data-stu-id="c842b-151">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c842b-152">新增</span><span class="sxs-lookup"><span data-stu-id="c842b-152">New</span></span> | <span data-ttu-id="c842b-153">在建立新購買時使用。</span><span class="sxs-lookup"><span data-stu-id="c842b-153">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="c842b-154">addQuantity</span><span class="sxs-lookup"><span data-stu-id="c842b-154">addQuantity</span></span> | <span data-ttu-id="c842b-155">用於原始購買的退款和增加後的新數量。</span><span class="sxs-lookup"><span data-stu-id="c842b-155">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="c842b-156">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="c842b-156">removeQuantity</span></span> | <span data-ttu-id="c842b-157">用於原始購買的退款和減少後的新數量。</span><span class="sxs-lookup"><span data-stu-id="c842b-157">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="c842b-158">取消</span><span class="sxs-lookup"><span data-stu-id="c842b-158">Cancel</span></span> | <span data-ttu-id="c842b-159">在取消訂用帳戶時使用。</span><span class="sxs-lookup"><span data-stu-id="c842b-159">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="c842b-160">轉換</span><span class="sxs-lookup"><span data-stu-id="c842b-160">Convert</span></span> | <span data-ttu-id="c842b-161">當授權升級，但授權數目維持不變時使用。</span><span class="sxs-lookup"><span data-stu-id="c842b-161">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="c842b-162">使用費用</span><span class="sxs-lookup"><span data-stu-id="c842b-162">Usage charges</span></span>

<span data-ttu-id="c842b-163">若要將這些使用量費用對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="c842b-163">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="c842b-164">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="c842b-164">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c842b-165">收費說明</span><span class="sxs-lookup"><span data-stu-id="c842b-165">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c842b-166">取消時的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="c842b-166">Assess usage fee when cancel</span></span> | <span data-ttu-id="c842b-167">存取在取消目前計費期間未付費使用量時的使用費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-167">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="c842b-168">目前週期的存取用量費用</span><span class="sxs-lookup"><span data-stu-id="c842b-168">Assess usage fee for current cycle</span></span> | <span data-ttu-id="c842b-169">存取目前計費期間的使用費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-169">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="c842b-170">學分</span><span class="sxs-lookup"><span data-stu-id="c842b-170">Credits</span></span>

<span data-ttu-id="c842b-171">若要將這些點數對應至您的發票：</span><span class="sxs-lookup"><span data-stu-id="c842b-171">To map these credits to your invoice:</span></span>

- <span data-ttu-id="c842b-172">加總以授權為基礎的檔案中的**TotalForCustomer** 。</span><span class="sxs-lookup"><span data-stu-id="c842b-172">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="c842b-173">加總以使用方式為基礎之檔案中的**PostTaxTotal**資料行。</span><span class="sxs-lookup"><span data-stu-id="c842b-173">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="c842b-174">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="c842b-174">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c842b-175">收費說明</span><span class="sxs-lookup"><span data-stu-id="c842b-175">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c842b-176">明細項目位移</span><span class="sxs-lookup"><span data-stu-id="c842b-176">Offset a line item</span></span> | <span data-ttu-id="c842b-177">明細項目的部分或完整退款，包括稅額。</span><span class="sxs-lookup"><span data-stu-id="c842b-177">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="c842b-178">用量型折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-178">Usage-based discounts</span></span>

<span data-ttu-id="c842b-179">若要將這些以使用量為基礎的折扣對應至您的發票，請將**計算 pretaxcharges**資料行與使用方式檔案加總。</span><span class="sxs-lookup"><span data-stu-id="c842b-179">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="c842b-180">費用描述（對帳檔案中的 ChargeType 資料行）</span><span class="sxs-lookup"><span data-stu-id="c842b-180">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="c842b-181">收費說明</span><span class="sxs-lookup"><span data-stu-id="c842b-181">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="c842b-182">啟用折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-182">Activation discount</span></span> | <span data-ttu-id="c842b-183">啟用訂用帳戶時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="c842b-183">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="c842b-184">循環折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-184">Cycle discount</span></span> | <span data-ttu-id="c842b-185">週期性費用所適用的折扣。</span><span class="sxs-lookup"><span data-stu-id="c842b-185">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="c842b-186">續約折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-186">Renew discount</span></span> | <span data-ttu-id="c842b-187">更新訂閱時所套用的折扣。</span><span class="sxs-lookup"><span data-stu-id="c842b-187">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="c842b-188">取消折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-188">Cancel discount</span></span> | <span data-ttu-id="c842b-189">當折扣取消時所適用的費用。</span><span class="sxs-lookup"><span data-stu-id="c842b-189">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="c842b-190">授權型折扣</span><span class="sxs-lookup"><span data-stu-id="c842b-190">License-based discounts</span></span>

<span data-ttu-id="c842b-191">若要將以授權為基礎的折扣對應至您的發票，請將**TotalOtherDiscount**資料行與授權檔加總。</span><span class="sxs-lookup"><span data-stu-id="c842b-191">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="c842b-192">*以授權為基礎的折扣可能適用于多種費用類型。*</span><span class="sxs-lookup"><span data-stu-id="c842b-192">*License-based discounts may be applied to multiple charge types.*</span></span>
