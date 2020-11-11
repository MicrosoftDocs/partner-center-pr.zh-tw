---
title: 有效的單位價格計算
ms.topic: how-to
ms.date: 11/10/2020
description: 深入瞭解有效的價格單位以及其計算方式。 包含範例計算。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498555"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="a5e0a-104">適用于 Azure 方案耗用量的有效單位價格計算</span><span class="sxs-lookup"><span data-stu-id="a5e0a-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="a5e0a-105">有效單位價格</span><span class="sxs-lookup"><span data-stu-id="a5e0a-105">The effective unit price</span></span>

<span data-ttu-id="a5e0a-106">有效單位價格是在計量層級 (計算，而不是資源層級) ，而且會根據計量使用量進行每日調整。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="a5e0a-107">我們會使用下列三個因素來計算有效的單價：</span><span class="sxs-lookup"><span data-stu-id="a5e0a-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="a5e0a-108">在整個計費週期內每天監視的耗用量</span><span class="sxs-lookup"><span data-stu-id="a5e0a-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="a5e0a-109">計量的計費成本</span><span class="sxs-lookup"><span data-stu-id="a5e0a-109">Billable cost for the meter</span></span>
- <span data-ttu-id="a5e0a-110">分層 (（如果適用）) </span><span class="sxs-lookup"><span data-stu-id="a5e0a-110">Tiering (if applicable)</span></span>

<span data-ttu-id="a5e0a-111">由於我們每天都會監視計費週期的耗用量，因此有效的單位價格將會波動。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="a5e0a-112">在停止耗用量計算並關閉計費期間之後，將可使用指定計費週期的最終價格。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="a5e0a-113">您將會看到在第四或第五個小數位數之後的耗用量變更。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="a5e0a-114">瞭解您的計量是否使用分層定價</span><span class="sxs-lookup"><span data-stu-id="a5e0a-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="a5e0a-115">如果您不知道您的計量是否使用分層定價，請使用下列程式來找出。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="a5e0a-116">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="a5e0a-117">選取 [ **銷售** ]、選取 [ **定價和** 供應專案]，然後選取 [ **Azure 方案定價** ]。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="a5e0a-118">依識別碼找出您的計量，然後下載您的定價資料。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="a5e0a-119">範例計算</span><span class="sxs-lookup"><span data-stu-id="a5e0a-119">Sample calculation</span></span>

<span data-ttu-id="a5e0a-120">下表提供如何在開啟期間計算有效單位價格的範例。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="a5e0a-121">在資料表中，下列值適用：</span><span class="sxs-lookup"><span data-stu-id="a5e0a-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="a5e0a-122">**高** = 資源/小時的單位價格 = 0.868</span><span class="sxs-lookup"><span data-stu-id="a5e0a-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="a5e0a-123">**BCU** = 計量的計費耗用量單位</span><span class="sxs-lookup"><span data-stu-id="a5e0a-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="a5e0a-124">**BC** = 計量 = BCU \* UP \* 0.85 的計費成本。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="a5e0a-125">這會反映 15% PEC 折扣的調整。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="a5e0a-126">接著，我們會使用函式的下限，將值限制在小數點後面的兩位數，以收費最小金額。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="a5e0a-127">**有效單位價格** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="a5e0a-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="a5e0a-128">注意：此範例中的計量表沒有定價層。</span><span class="sxs-lookup"><span data-stu-id="a5e0a-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="a5e0a-129">Date</span><span class="sxs-lookup"><span data-stu-id="a5e0a-129">Date</span></span> | <span data-ttu-id="a5e0a-130">BCU (計費耗用量單位) </span><span class="sxs-lookup"><span data-stu-id="a5e0a-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="a5e0a-131">BC (計費成本) </span><span class="sxs-lookup"><span data-stu-id="a5e0a-131">BC (Billable cost)</span></span> | <span data-ttu-id="a5e0a-132">有效單位價格</span><span class="sxs-lookup"><span data-stu-id="a5e0a-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="a5e0a-133">3-8 月</span><span class="sxs-lookup"><span data-stu-id="a5e0a-133">3-Aug</span></span> | <span data-ttu-id="a5e0a-134">29</span><span class="sxs-lookup"><span data-stu-id="a5e0a-134">29</span></span> | <span data-ttu-id="a5e0a-135">21.39</span><span class="sxs-lookup"><span data-stu-id="a5e0a-135">21.39</span></span> | <span data-ttu-id="a5e0a-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="a5e0a-136">0.737586206896552</span></span> |
| <span data-ttu-id="a5e0a-137">10-8 月</span><span class="sxs-lookup"><span data-stu-id="a5e0a-137">10-Aug</span></span> | <span data-ttu-id="a5e0a-138">210.950039</span><span class="sxs-lookup"><span data-stu-id="a5e0a-138">210.950039</span></span> | <span data-ttu-id="a5e0a-139">155.63</span><span class="sxs-lookup"><span data-stu-id="a5e0a-139">155.63</span></span> | <span data-ttu-id="a5e0a-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="a5e0a-140">0.737757626107858</span></span> |
| <span data-ttu-id="a5e0a-141">25-8 月</span><span class="sxs-lookup"><span data-stu-id="a5e0a-141">25-Aug</span></span> | <span data-ttu-id="a5e0a-142">555.950039</span><span class="sxs-lookup"><span data-stu-id="a5e0a-142">555.950039</span></span> | <span data-ttu-id="a5e0a-143">410.17</span><span class="sxs-lookup"><span data-stu-id="a5e0a-143">410.17</span></span> | <span data-ttu-id="a5e0a-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="a5e0a-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="a5e0a-145">後續步驟</span><span class="sxs-lookup"><span data-stu-id="a5e0a-145">Next steps</span></span>

- [<span data-ttu-id="a5e0a-146">帳單與稅金</span><span class="sxs-lookup"><span data-stu-id="a5e0a-146">Billing and taxes</span></span>](billing.md)
