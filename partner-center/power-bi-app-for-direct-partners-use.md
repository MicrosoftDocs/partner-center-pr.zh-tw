---
title: 使用合作夥伴中心分析進行 Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何使用適用于 CSP) 中的直接合作夥伴 Power BI (的合作夥伴中心分析應用程式來查看您的商務資料。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302284"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="6bf40-103">使用適用於 Microsoft Power BI 的合作夥伴中心分析應用程式來檢視業務資料</span><span class="sxs-lookup"><span data-stu-id="6bf40-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="6bf40-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="6bf40-104">**Applies to**</span></span>

- <span data-ttu-id="6bf40-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="6bf40-105">Partner Center</span></span>

<span data-ttu-id="6bf40-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="6bf40-106">**Appropriate roles**</span></span>

- <span data-ttu-id="6bf40-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="6bf40-107">Global admin</span></span>
- <span data-ttu-id="6bf40-108">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="6bf40-108">User admin</span></span>
- <span data-ttu-id="6bf40-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="6bf40-109">Sales agent</span></span>
- <span data-ttu-id="6bf40-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="6bf40-110">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="6bf40-111">檢視您的業務資料</span><span class="sxs-lookup"><span data-stu-id="6bf40-111">View your business data</span></span>

<span data-ttu-id="6bf40-112">使用適用於 Power BI 的合作夥伴中心分析應用程式，以視覺化方式呈現業務資料，包括：</span><span class="sxs-lookup"><span data-stu-id="6bf40-112">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="6bf40-113">您的客戶群、訂閱量及授權數的成長</span><span class="sxs-lookup"><span data-stu-id="6bf40-113">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="6bf40-114">Office 365、Microsoft Dynamics 及 Microsoft Azure 產品的使用狀況</span><span class="sxs-lookup"><span data-stu-id="6bf40-114">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="6bf40-115">過去 60 天中每個 Azure 訂閱的計量付費資源的每日消耗單位</span><span class="sxs-lookup"><span data-stu-id="6bf40-115">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="6bf40-116">預估費用 (根據最新費率卡計算)</span><span class="sxs-lookup"><span data-stu-id="6bf40-116">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="6bf40-117">能夠匯出資料集及建立自訂報表，包括每位客戶。</span><span class="sxs-lookup"><span data-stu-id="6bf40-117">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="6bf40-118">關於合作夥伴中心分析應用程式預覽版本</span><span class="sxs-lookup"><span data-stu-id="6bf40-118">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="6bf40-119">此應用程式僅適用於雲端解決方案提供者計畫中的直接提供者。</span><span class="sxs-lookup"><span data-stu-id="6bf40-119">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="6bf40-120">雲端解決方案提供者中的其他合作夥伴 (例如間接經銷商) 將無法登入。</span><span class="sxs-lookup"><span data-stu-id="6bf40-120">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="6bf40-121">所有預估費用皆為稅前計費/發票資料，不具法律效力。</span><span class="sxs-lookup"><span data-stu-id="6bf40-121">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="6bf40-122">預估費用只是要用來深入了解資料。</span><span class="sxs-lookup"><span data-stu-id="6bf40-122">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="6bf40-123">客戶資訊是根據訂閱來提供。</span><span class="sxs-lookup"><span data-stu-id="6bf40-123">Customer information is based on subscriptions.</span></span> <span data-ttu-id="6bf40-124">任何您最近為其建立帳戶但尚未擁有訂閱的客戶，不包括在計數中。</span><span class="sxs-lookup"><span data-stu-id="6bf40-124">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="6bf40-125">預估費用是根據以雲端解決方案提供者定價為基礎的最新費率卡計算。</span><span class="sxs-lookup"><span data-stu-id="6bf40-125">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="6bf40-126">天數是日曆天數。</span><span class="sxs-lookup"><span data-stu-id="6bf40-126">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="6bf40-127">商業見解報告</span><span class="sxs-lookup"><span data-stu-id="6bf40-127">Business Insights report</span></span>

- <span data-ttu-id="6bf40-128">**客戶租用戶數**：已購買訂閱的客戶會有各種不同的 Azure AD 租用戶，其數目</span><span class="sxs-lookup"><span data-stu-id="6bf40-128">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="6bf40-129">**新增 (過去 30 天)**：在過去 30 天中購買至少一個訂閱的新客戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-129">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="6bf40-130">\*\*過去30天) \*\*的變換 (：沒有任何「作用中」、「在寬限期」或「已停用」訂閱的客戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-130">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="6bf40-131">**新增 (過去 24 小時)**：在過去 24 小時中購買至少一個訂閱的新客戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-131">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="6bf40-132">**過去 12 個月每月估計費用**：過去 12 個月期間每月彙總預估稅前發票金額的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="6bf40-132">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6bf40-133">**依產品區分的過去 12 個月估計費用**：依過去 12 個月期間每月彙總預估稅前發票金額排序的已銷售產品。</span><span class="sxs-lookup"><span data-stu-id="6bf40-133">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="6bf40-134">此狀態表示最熱門的產品會帶來最多收益。</span><span class="sxs-lookup"><span data-stu-id="6bf40-134">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="6bf40-135">**過去 12 個月的客戶**：過去 12 個月期間每月彙總新客戶及流失客戶的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="6bf40-135">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6bf40-136">**依客戶區分的過去 12 個月估計費用**：依過去 12 個月期間每月彙總預估稅前發票金額排序的客戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-136">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="6bf40-137">此狀態表示頂尖客戶帶來最多收益。</span><span class="sxs-lookup"><span data-stu-id="6bf40-137">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="6bf40-138">**依產品區分的客戶計數**：依相關聯客戶排序的已銷售產品。</span><span class="sxs-lookup"><span data-stu-id="6bf40-138">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="6bf40-139">此狀態表示銷售給大多數客戶的熱門產品。</span><span class="sxs-lookup"><span data-stu-id="6bf40-139">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="6bf40-140">訂閱見解報告</span><span class="sxs-lookup"><span data-stu-id="6bf40-140">Subscription Insights report</span></span>

- <span data-ttu-id="6bf40-141">**訂**用帳戶狀態：</span><span class="sxs-lookup"><span data-stu-id="6bf40-141">**Subscription status**:</span></span>

- <span data-ttu-id="6bf40-142">作用中：屬於「作用中」或「處於寬限期」狀態的訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-142">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="6bf40-143">已暫止：屬於「已停用」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-143">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="6bf40-144">取消布建：屬於「已取消布建」或「已過期」狀態的訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-144">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="6bf40-145">**到期狀態**：</span><span class="sxs-lookup"><span data-stu-id="6bf40-145">**Expiry status**:</span></span>

  - <span data-ttu-id="6bf40-146">已過期：已經過期的訂閱 (已超過訂閱結束日期)</span><span class="sxs-lookup"><span data-stu-id="6bf40-146">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="6bf40-147">30 天後過期：將會在 30 天後過期的訂閱 (訂閱結束日期是在接下來 30 天之後)</span><span class="sxs-lookup"><span data-stu-id="6bf40-147">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="6bf40-148">30 天內即將到期：將會在接下來 30 天內到期的訂閱 (訂閱結束日期是在今天和接下來 30 天之內)</span><span class="sxs-lookup"><span data-stu-id="6bf40-148">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="6bf40-149">訂用帳戶**總計**：「作用中」、「寬限期」或「已停用」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-149">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="6bf40-150">**新增 (過去 30 天)**：客戶在過去 30 天內購買的新訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-150">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="6bf40-151">**新增 (過去 24 小時)**：客戶在過去 24 小時內購買的新訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-151">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="6bf40-152">**30 天內即將到期**：將會在接下來 30 天內到期的訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-152">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="6bf40-153">**流失 (過去 30 天)**：在過去 30 天內已解除佈建或已暫停 (已停用) 的訂閱</span><span class="sxs-lookup"><span data-stu-id="6bf40-153">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="6bf40-154">**依訂用帳戶類型的散發**：依授權型和以使用量為基礎的訂用帳戶類型來散發訂閱總數的%</span><span class="sxs-lookup"><span data-stu-id="6bf40-154">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="6bf40-155">**依產品區分的使用中訂閱計數**：依使用中訂閱計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="6bf40-155">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="6bf40-156">**過去 12 個月的訂閱**：過去 12 個月期間每月彙總新訂閱及流失訂閱的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="6bf40-156">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6bf40-157">**客戶訂用帳戶詳細資料**：客戶、訂閱和優惠的詳細觀點</span><span class="sxs-lookup"><span data-stu-id="6bf40-157">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="6bf40-158">授權見解報告：</span><span class="sxs-lookup"><span data-stu-id="6bf40-158">License Insights report:</span></span>

- <span data-ttu-id="6bf40-159">**授權總計**：匯總在所有授權型訂用帳戶中的授權總數</span><span class="sxs-lookup"><span data-stu-id="6bf40-159">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="6bf40-160">**新增 (過去 30 天)**：過去 30 天內增加的授權數</span><span class="sxs-lookup"><span data-stu-id="6bf40-160">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="6bf40-161">**流失 (過去 30 天)**：過去 30 天內減少的授權數</span><span class="sxs-lookup"><span data-stu-id="6bf40-161">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="6bf40-162">**新增 (過去 24 小時)**：過去 24 小時內增加的授權數</span><span class="sxs-lookup"><span data-stu-id="6bf40-162">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="6bf40-163">**過去 90 天的授權**：過去 90 天期間每月彙總的授權增減月份趨勢</span><span class="sxs-lookup"><span data-stu-id="6bf40-163">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="6bf40-164">**依產品區分的使用中授權計數**：依使用中授權計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="6bf40-164">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="6bf40-165">**依客戶的有效授權計數**：依有效授權計數排序的客戶</span><span class="sxs-lookup"><span data-stu-id="6bf40-165">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="6bf40-166">**過去90天的客戶授權事件詳細資料**：客戶、訂閱和訂用帳戶事件的詳細觀點，包括事件日期、事件名稱、數量和數量變更。</span><span class="sxs-lookup"><span data-stu-id="6bf40-166">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="6bf40-167">授權使用狀況報告：</span><span class="sxs-lookup"><span data-stu-id="6bf40-167">Licenses Usage report:</span></span>

- <span data-ttu-id="6bf40-168">**依產品指派的授權**：依授權指派計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="6bf40-168">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="6bf40-169">**依產品區分的使用中授權**：依授權使用計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="6bf40-169">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="6bf40-170">**已指派授權的客戶分佈情況**：依授權指派百分比 (按照 20% 範圍貯體劃分值區) 所區分的客戶總數分佈百分比</span><span class="sxs-lookup"><span data-stu-id="6bf40-170">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="6bf40-171">**使用中授權的客戶分佈情況**：依授權使用百分比 (按照 20% 範圍貯體劃分值區) 所區分的客戶總數分佈百分比</span><span class="sxs-lookup"><span data-stu-id="6bf40-171">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="6bf40-172">**依客戶區分的已指派授權**：包含已銷售授權以及依客戶與產品區分之已指派授權的詳細檢視</span><span class="sxs-lookup"><span data-stu-id="6bf40-172">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="6bf40-173">**依客戶區分的使用中授權**：包含已銷售授權以及依客戶與產品區分之使用中授權的詳細檢視</span><span class="sxs-lookup"><span data-stu-id="6bf40-173">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="6bf40-174">Azure 見解報告：</span><span class="sxs-lookup"><span data-stu-id="6bf40-174">Azure Insights report:</span></span>

- <span data-ttu-id="6bf40-175">**過去12個月內**的以使用量為基礎的客戶：以新使用量為基礎的客戶和變換以使用量為基礎的客戶在過去12個月期間內每月匯總的月趨勢</span><span class="sxs-lookup"><span data-stu-id="6bf40-175">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6bf40-176">**過去12個月內以使用量為基礎**的訂用帳戶：以新使用量為基礎的訂用帳戶和變換使用量為基礎的訂用帳戶，每月在過去12個月期間匯總了個月</span><span class="sxs-lookup"><span data-stu-id="6bf40-176">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="6bf40-177">**客戶過去60天的預估使用量成本**：以使用量為基礎的客戶依預估在過去60天期間匯總的預付稅發票金額排序。</span><span class="sxs-lookup"><span data-stu-id="6bf40-177">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="6bf40-178">此狀態表示以使用量為基礎的熱門客戶帶來最多收益</span><span class="sxs-lookup"><span data-stu-id="6bf40-178">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="6bf40-179">**過去60天內依類別目錄的預估使用成本**：以使用量為基礎之訂用帳戶的計量分類，依預估在過去60天期間匯總的預付稅發票金額排序。</span><span class="sxs-lookup"><span data-stu-id="6bf40-179">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="6bf40-180">**依訂用帳戶過去60天的預估使用成本**：以使用量為基礎的訂閱，依預估在過去60天期間匯總的預付稅發票金額。</span><span class="sxs-lookup"><span data-stu-id="6bf40-180">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="6bf40-181">**依消費預算區分的客戶估計使用費用**：依客戶目前使用量消費預算超過閾值 (100%) 百分比排序的客戶。</span><span class="sxs-lookup"><span data-stu-id="6bf40-181">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="6bf40-182">Azure 資源使用報告：</span><span class="sxs-lookup"><span data-stu-id="6bf40-182">Azure Resource Usage report:</span></span>

- <span data-ttu-id="6bf40-183">**針對選取的期間，每天使用 Azure 資源**：每個使用量型訂用帳戶中每個計量付費資源的每日耗用量單位（過去60天內所選期間）。</span><span class="sxs-lookup"><span data-stu-id="6bf40-183">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="6bf40-184">**所選期間的 Azure 資源估計使用成本**：根據每個以使用量為基礎的訂用帳戶中，每個計量付費資源在過去60天內所選期間的最新費率卡片的預估成本。</span><span class="sxs-lookup"><span data-stu-id="6bf40-184">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="6bf40-185">後續步驟</span><span class="sxs-lookup"><span data-stu-id="6bf40-185">Next steps</span></span>

- [<span data-ttu-id="6bf40-186">適用於 Power BI 的合作夥伴中心分析應用程式概觀</span><span class="sxs-lookup"><span data-stu-id="6bf40-186">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="6bf40-187">安裝和預覽適用於 Microsoft Power BI 的合作夥伴中心分析應用程式</span><span class="sxs-lookup"><span data-stu-id="6bf40-187">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
