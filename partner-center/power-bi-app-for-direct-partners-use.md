---
title: 針對 Power BI 使用合作夥伴中心分析
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何使用 CSP) 中的直接合作夥伴適用於 Power BI 的合作夥伴中心分析應用程式 (來查看您的商務資料。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244cb852728d47360cf8ecd1d1e9ccb641466b1d
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215742"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="76e09-103">使用適用於 Microsoft Power BI 的合作夥伴中心分析應用程式來檢視業務資料</span><span class="sxs-lookup"><span data-stu-id="76e09-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="76e09-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="76e09-104">**Appropriate roles**</span></span>

- <span data-ttu-id="76e09-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="76e09-105">Global admin</span></span>
- <span data-ttu-id="76e09-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="76e09-106">User admin</span></span>
- <span data-ttu-id="76e09-107">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="76e09-107">Sales agent</span></span>
- <span data-ttu-id="76e09-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="76e09-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="76e09-109">檢視您的業務資料</span><span class="sxs-lookup"><span data-stu-id="76e09-109">View your business data</span></span>

<span data-ttu-id="76e09-110">使用適用於 Power BI 的合作夥伴中心分析應用程式，以視覺化方式呈現業務資料，包括：</span><span class="sxs-lookup"><span data-stu-id="76e09-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="76e09-111">您的客戶群、訂閱量及授權數的成長</span><span class="sxs-lookup"><span data-stu-id="76e09-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="76e09-112">Office 365、Microsoft Dynamics 及 Microsoft Azure 產品的使用狀況</span><span class="sxs-lookup"><span data-stu-id="76e09-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="76e09-113">過去 60 天中每個 Azure 訂閱的計量付費資源的每日消耗單位</span><span class="sxs-lookup"><span data-stu-id="76e09-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="76e09-114">預估費用 (根據最新費率卡計算)</span><span class="sxs-lookup"><span data-stu-id="76e09-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="76e09-115">能夠匯出資料集和建立自訂報表，包括每個客戶。</span><span class="sxs-lookup"><span data-stu-id="76e09-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="76e09-116">關於合作夥伴中心分析應用程式預覽版本</span><span class="sxs-lookup"><span data-stu-id="76e09-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="76e09-117">此應用程式僅適用於雲端解決方案提供者計畫中的直接提供者。</span><span class="sxs-lookup"><span data-stu-id="76e09-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="76e09-118">雲端解決方案提供者中的其他合作夥伴 (例如間接經銷商) 將無法登入。</span><span class="sxs-lookup"><span data-stu-id="76e09-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="76e09-119">所有預估費用皆為稅前計費/發票資料，不具法律效力。</span><span class="sxs-lookup"><span data-stu-id="76e09-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="76e09-120">預估費用只是要用來深入了解資料。</span><span class="sxs-lookup"><span data-stu-id="76e09-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="76e09-121">客戶資訊是根據訂閱來提供。</span><span class="sxs-lookup"><span data-stu-id="76e09-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="76e09-122">任何您最近為其建立帳戶但尚未擁有訂閱的客戶，不包括在計數中。</span><span class="sxs-lookup"><span data-stu-id="76e09-122">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span>

- <span data-ttu-id="76e09-123">預估費用是根據以雲端解決方案提供者定價為基礎的最新費率卡計算。</span><span class="sxs-lookup"><span data-stu-id="76e09-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="76e09-124">天數是日曆天數。</span><span class="sxs-lookup"><span data-stu-id="76e09-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="76e09-125">商業見解報告</span><span class="sxs-lookup"><span data-stu-id="76e09-125">Business Insights report</span></span>

- <span data-ttu-id="76e09-126">**客戶租用戶數**：已購買訂閱的客戶會有各種不同的 Azure AD 租用戶，其數目</span><span class="sxs-lookup"><span data-stu-id="76e09-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="76e09-127">**新增 (過去 30 天)**：在過去 30 天中購買至少一個訂閱的新客戶</span><span class="sxs-lookup"><span data-stu-id="76e09-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="76e09-128">變換 **(過去30天)**：沒有任何「作用中」、「寬限期」或「已停用」訂用帳戶的客戶</span><span class="sxs-lookup"><span data-stu-id="76e09-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="76e09-129">**新增 (過去 24 小時)**：在過去 24 小時中購買至少一個訂閱的新客戶</span><span class="sxs-lookup"><span data-stu-id="76e09-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="76e09-130">**過去 12 個月每月估計費用**：過去 12 個月期間每月彙總預估稅前發票金額的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="76e09-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="76e09-131">**依產品區分的過去 12 個月估計費用**：依過去 12 個月期間每月彙總預估稅前發票金額排序的已銷售產品。</span><span class="sxs-lookup"><span data-stu-id="76e09-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="76e09-132">此狀態表示最重要的產品會帶來最多的收益。</span><span class="sxs-lookup"><span data-stu-id="76e09-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="76e09-133">**過去 12 個月的客戶**：過去 12 個月期間每月彙總新客戶及流失客戶的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="76e09-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="76e09-134">**依客戶區分的過去 12 個月估計費用**：依過去 12 個月期間每月彙總預估稅前發票金額排序的客戶</span><span class="sxs-lookup"><span data-stu-id="76e09-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="76e09-135">此狀態表示最高的客戶會帶來最多的收益。</span><span class="sxs-lookup"><span data-stu-id="76e09-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="76e09-136">**依產品區分的客戶計數**：依相關聯客戶排序的已銷售產品。</span><span class="sxs-lookup"><span data-stu-id="76e09-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="76e09-137">此狀態表示銷售給大部分客戶的熱門產品。</span><span class="sxs-lookup"><span data-stu-id="76e09-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="76e09-138">訂閱見解報告</span><span class="sxs-lookup"><span data-stu-id="76e09-138">Subscription Insights report</span></span>

- <span data-ttu-id="76e09-139">**訂** 用帳戶狀態：</span><span class="sxs-lookup"><span data-stu-id="76e09-139">**Subscription status**:</span></span>

- <span data-ttu-id="76e09-140">作用中：屬於「作用中」或「寬限期」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="76e09-141">已暫止：屬於「已停用」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="76e09-142">解除布建：屬於「取消布建」或「已過期」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="76e09-143">**到期狀態**：</span><span class="sxs-lookup"><span data-stu-id="76e09-143">**Expiry status**:</span></span>

  - <span data-ttu-id="76e09-144">已過期：已經過期的訂閱 (已超過訂閱結束日期)</span><span class="sxs-lookup"><span data-stu-id="76e09-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="76e09-145">30 天後過期：將會在 30 天後過期的訂閱 (訂閱結束日期是在接下來 30 天之後)</span><span class="sxs-lookup"><span data-stu-id="76e09-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="76e09-146">30 天內即將到期：將會在接下來 30 天內到期的訂閱 (訂閱結束日期是在今天和接下來 30 天之內)</span><span class="sxs-lookup"><span data-stu-id="76e09-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="76e09-147">訂用帳戶 **總計**：處於「作用中」、「寬限期」或「已停用」狀態的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="76e09-148">**新增 (過去 30 天)**：客戶在過去 30 天內購買的新訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="76e09-149">**新增 (過去 24 小時)**：客戶在過去 24 小時內購買的新訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="76e09-150">**30 天內即將到期**：將會在接下來 30 天內到期的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="76e09-151">**流失 (過去 30 天)**：在過去 30 天內已解除佈建或已暫停 (已停用) 的訂閱</span><span class="sxs-lookup"><span data-stu-id="76e09-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="76e09-152">**依訂用帳戶類型散發**：依授權型和依使用量型訂用帳戶類型散發訂用帳戶總計的百分比</span><span class="sxs-lookup"><span data-stu-id="76e09-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="76e09-153">**依產品區分的使用中訂閱計數**：依使用中訂閱計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="76e09-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="76e09-154">**過去 12 個月的訂閱**：過去 12 個月期間每月彙總新訂閱及流失訂閱的月份趨勢</span><span class="sxs-lookup"><span data-stu-id="76e09-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="76e09-155">**客戶訂用帳戶詳細資料**：客戶、訂用帳戶和優惠的詳細觀點</span><span class="sxs-lookup"><span data-stu-id="76e09-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="76e09-156">授權見解報告：</span><span class="sxs-lookup"><span data-stu-id="76e09-156">License Insights report:</span></span>

- <span data-ttu-id="76e09-157">**授權總數**：在所有授權型訂用帳戶中匯總的授權總數</span><span class="sxs-lookup"><span data-stu-id="76e09-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="76e09-158">**新增 (過去 30 天)**：過去 30 天內增加的授權數</span><span class="sxs-lookup"><span data-stu-id="76e09-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="76e09-159">**流失 (過去 30 天)**：過去 30 天內減少的授權數</span><span class="sxs-lookup"><span data-stu-id="76e09-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="76e09-160">**新增 (過去 24 小時)**：過去 24 小時內增加的授權數</span><span class="sxs-lookup"><span data-stu-id="76e09-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="76e09-161">**過去 90 天的授權**：過去 90 天期間每月彙總的授權增減月份趨勢</span><span class="sxs-lookup"><span data-stu-id="76e09-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="76e09-162">**依產品區分的使用中授權計數**：依使用中授權計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="76e09-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="76e09-163">**依客戶的有效授權計數**：依有效授權計數排序的客戶</span><span class="sxs-lookup"><span data-stu-id="76e09-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="76e09-164">**過去90天的客戶授權事件詳細資料**：客戶、訂用帳戶和訂用帳戶事件的詳細觀點，包括事件日期、事件名稱、數量和數量變更。</span><span class="sxs-lookup"><span data-stu-id="76e09-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="76e09-165">授權使用狀況報告：</span><span class="sxs-lookup"><span data-stu-id="76e09-165">Licenses Usage report:</span></span>

- <span data-ttu-id="76e09-166">**依產品指派的授權**：依授權指派計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="76e09-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="76e09-167">**依產品區分的使用中授權**：依授權使用計數排序的已銷售產品</span><span class="sxs-lookup"><span data-stu-id="76e09-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="76e09-168">**已指派授權的客戶分佈情況**：依授權指派百分比 (按照 20% 範圍貯體劃分值區) 所區分的客戶總數分佈百分比</span><span class="sxs-lookup"><span data-stu-id="76e09-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="76e09-169">**使用中授權的客戶分佈情況**：依授權使用百分比 (按照 20% 範圍貯體劃分值區) 所區分的客戶總數分佈百分比</span><span class="sxs-lookup"><span data-stu-id="76e09-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="76e09-170">**依客戶區分的已指派授權**：包含已銷售授權以及依客戶與產品區分之已指派授權的詳細檢視</span><span class="sxs-lookup"><span data-stu-id="76e09-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="76e09-171">**依客戶區分的使用中授權**：包含已銷售授權以及依客戶與產品區分之使用中授權的詳細檢視</span><span class="sxs-lookup"><span data-stu-id="76e09-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="76e09-172">Azure 見解報告：</span><span class="sxs-lookup"><span data-stu-id="76e09-172">Azure Insights report:</span></span>

- <span data-ttu-id="76e09-173">**過去12個月內以使用量為基礎的客戶**：以新使用量為基礎之客戶的月間趨勢，以及流失以使用量為基礎的客戶，每月在過去12個月內匯總</span><span class="sxs-lookup"><span data-stu-id="76e09-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="76e09-174">**過去12個月的使用量型** 訂用帳戶：以新使用量為基礎的訂用帳戶和流失使用量為基礎的訂用帳戶在過去12個月期間內每月匯總的月趨勢</span><span class="sxs-lookup"><span data-stu-id="76e09-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="76e09-175">**過去60天內客戶的預估使用量成本**：依使用量為基礎的客戶，依照過去60天期間匯總的預估預付稅發票金額來排序。</span><span class="sxs-lookup"><span data-stu-id="76e09-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="76e09-176">此狀態表示以使用量為基礎的熱門客戶會帶來最多收益</span><span class="sxs-lookup"><span data-stu-id="76e09-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="76e09-177">**過去60天依類別的預估使用量成本**：依使用量排序的訂用帳戶計量類別，會依過去60天期間匯總的預估預付稅發票金額來排序。</span><span class="sxs-lookup"><span data-stu-id="76e09-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="76e09-178">**過去60天內依訂用帳戶的預估使用量成本**：依使用量計費的訂用帳戶，依過去60天期間匯總的預估預付稅發票金額。</span><span class="sxs-lookup"><span data-stu-id="76e09-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="76e09-179">**依消費預算區分的客戶估計使用費用**：依客戶目前使用量消費預算超過閾值 (100%) 百分比排序的客戶。</span><span class="sxs-lookup"><span data-stu-id="76e09-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="76e09-180">Azure 資源使用報告：</span><span class="sxs-lookup"><span data-stu-id="76e09-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="76e09-181">在 **所選期間內每天使用 Azure 資源**：每個使用量型訂用帳戶中每個計量資源的每日耗用量單位，在過去60天內所選期間內。</span><span class="sxs-lookup"><span data-stu-id="76e09-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="76e09-182">**所選期間的 Azure 資源預估使用量成本**：根據每個使用量型訂用帳戶中每個計量付費資源的最新費率卡片預估成本，在過去60天內選取的期間。</span><span class="sxs-lookup"><span data-stu-id="76e09-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="76e09-183">後續步驟</span><span class="sxs-lookup"><span data-stu-id="76e09-183">Next steps</span></span>

- [<span data-ttu-id="76e09-184">適用於 Power BI 的合作夥伴中心分析應用程式概觀</span><span class="sxs-lookup"><span data-stu-id="76e09-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="76e09-185">安裝和預覽適用於 Microsoft Power BI 的合作夥伴中心分析應用程式</span><span class="sxs-lookup"><span data-stu-id="76e09-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
