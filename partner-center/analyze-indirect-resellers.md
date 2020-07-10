---
title: 分析間接經銷商績效
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 流量分析來瞭解間接轉銷商的表現，包括成功和可能需要注意的區域。
author: amitravat
ms.author: amrava
ms.topic: article
keywords: 業務資料
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 33d435b6497f84d87ce866624deb47e2bd6ebc89
ms.sourcegitcommit: cba3c73520b8f72d0ba9ca3725f355cab79342c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/09/2020
ms.locfileid: "86175966"
---
# <a name="use-analytics-to-analyze-performance-of-your-indirect-resellers"></a><span data-ttu-id="53b38-104">流量分析來分析間接轉銷商的效能</span><span class="sxs-lookup"><span data-stu-id="53b38-104">Use analytics to analyze performance of your indirect resellers</span></span>

<span data-ttu-id="53b38-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="53b38-105">**Applies to**</span></span>

- <span data-ttu-id="53b38-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="53b38-106">Partner Center</span></span>
- <span data-ttu-id="53b38-107">雲端解決方案提供者計畫合作夥伴</span><span class="sxs-lookup"><span data-stu-id="53b38-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="53b38-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="53b38-108">**Appropriate roles**</span></span>

- <span data-ttu-id="53b38-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="53b38-109">Global admin</span></span>
- <span data-ttu-id="53b38-110">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="53b38-110">User management admin</span></span>
- <span data-ttu-id="53b38-111">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="53b38-111">Admin agent</span></span>
- <span data-ttu-id="53b38-112">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="53b38-112">Sales agent</span></span>

<span data-ttu-id="53b38-113">資料推動業務決策。</span><span class="sxs-lookup"><span data-stu-id="53b38-113">Data drives business decisions.</span></span> <span data-ttu-id="53b38-114">使用**經銷商分析**頁面上的計量，找出您的成功之處、您間接經銷商的成功之處，以及需要注意的領域。</span><span class="sxs-lookup"><span data-stu-id="53b38-114">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="53b38-115">在規劃新的業務務目標時，請使用此資訊。</span><span class="sxs-lookup"><span data-stu-id="53b38-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="53b38-116">間接經銷商分析僅適用於雲端解決方案提供者計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="53b38-116">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a><span data-ttu-id="53b38-117">您可以查看的轉銷商分析計量類型</span><span class="sxs-lookup"><span data-stu-id="53b38-117">Types of reseller analytics metrics you can view</span></span>

<span data-ttu-id="53b38-118">我們正在追蹤下列計量︰</span><span class="sxs-lookup"><span data-stu-id="53b38-118">We are tracking the following metrics:</span></span>

<span data-ttu-id="53b38-119">**摘要**</span><span class="sxs-lookup"><span data-stu-id="53b38-119">**Summary**</span></span>  
 - <span data-ttu-id="53b38-120">**經銷商總數**：在訂閱最後一天的使用中經銷商計數</span><span class="sxs-lookup"><span data-stu-id="53b38-120">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="53b38-121">**新經銷商**：在指定的時段中新的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="53b38-121">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="53b38-122">**使用中經銷商**：MPNID 至少有 1 個訂閱，以及訂閱狀態不是取消佈建的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="53b38-122">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="53b38-123">**交易中經銷商**：在指定的時段中有售出訂閱的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="53b38-123">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="53b38-124">**依市場分類的經銷商**</span><span class="sxs-lookup"><span data-stu-id="53b38-124">**Resellers by market**</span></span>  
 - <span data-ttu-id="53b38-125">依照地理位置分類的經銷商總數</span><span class="sxs-lookup"><span data-stu-id="53b38-125">Total resellers by geographic location</span></span>  

<span data-ttu-id="53b38-126">**依照售出訂閱分類的熱門經銷商**</span><span class="sxs-lookup"><span data-stu-id="53b38-126">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="53b38-127">依照售出訂閱數量排序的經銷商清單</span><span class="sxs-lookup"><span data-stu-id="53b38-127">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="53b38-128">**依訂閱計數排序的熱門產品**</span><span class="sxs-lookup"><span data-stu-id="53b38-128">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="53b38-129">**Dynamics 365**：依售出訂閱排序的 Dynamics 365 產品</span><span class="sxs-lookup"><span data-stu-id="53b38-129">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="53b38-130">**EMS**：售出的企業管理服務訂閱數量</span><span class="sxs-lookup"><span data-stu-id="53b38-130">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="53b38-131">**Microsoft 365**：售出的 Microsoft 365 訂閱數量</span><span class="sxs-lookup"><span data-stu-id="53b38-131">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="53b38-132">**Office 365**：依售出訂閱排序的 Office 365 產品</span><span class="sxs-lookup"><span data-stu-id="53b38-132">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="53b38-133">**新增訂閱**</span><span class="sxs-lookup"><span data-stu-id="53b38-133">**New subscriptions**</span></span>  
 - <span data-ttu-id="53b38-134">依日期新增的新訂閱數量</span><span class="sxs-lookup"><span data-stu-id="53b38-134">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="53b38-135">**訂閱流失**</span><span class="sxs-lookup"><span data-stu-id="53b38-135">**Subscription churn**</span></span>  
 - <span data-ttu-id="53b38-136">**新訂閱**：依日期新增的新訂閱計數</span><span class="sxs-lookup"><span data-stu-id="53b38-136">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="53b38-137">**取消佈建的訂閱**：依日期的取消佈建或暫停訂閱計數</span><span class="sxs-lookup"><span data-stu-id="53b38-137">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="53b38-138">**新經銷商詳細資料**</span><span class="sxs-lookup"><span data-stu-id="53b38-138">**New reseller details**</span></span>  
 - <span data-ttu-id="53b38-139">**經銷商名稱**：間接經銷商的名稱</span><span class="sxs-lookup"><span data-stu-id="53b38-139">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="53b38-140">**位置**：間接經銷商營運的市場</span><span class="sxs-lookup"><span data-stu-id="53b38-140">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="53b38-141">**訂閱**：經銷商售出的訂閱數</span><span class="sxs-lookup"><span data-stu-id="53b38-141">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="53b38-142">**授權**：經銷商在所有訂閱中已售出的授權總數</span><span class="sxs-lookup"><span data-stu-id="53b38-142">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
## <a name="next-steps"></a><span data-ttu-id="53b38-143">後續步驟</span><span class="sxs-lookup"><span data-stu-id="53b38-143">Next steps</span></span>

- [<span data-ttu-id="53b38-144">分析訂用帳戶和授權，以協助推動商業決策</span><span class="sxs-lookup"><span data-stu-id="53b38-144">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)