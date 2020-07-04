---
title: 分析間接經銷商績效
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 流量分析來瞭解間接轉銷商的表現，包括成功和可能需要注意的區域。
author: amrava
ms.author: amrava
ms.topic: article
keywords: 業務資料
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3bdc3e149d445a1d43f24d54e16c04464bea807e
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947413"
---
# <a name="use-analytics-to-analyze-performance-of-your-indirect-resellers"></a><span data-ttu-id="0e8b1-104">流量分析來分析間接轉銷商的效能</span><span class="sxs-lookup"><span data-stu-id="0e8b1-104">Use analytics to analyze performance of your indirect resellers</span></span>

<span data-ttu-id="0e8b1-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-105">**Applies to**</span></span>

- <span data-ttu-id="0e8b1-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="0e8b1-106">Partner Center</span></span>
- <span data-ttu-id="0e8b1-107">雲端解決方案提供者計畫合作夥伴</span><span class="sxs-lookup"><span data-stu-id="0e8b1-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="0e8b1-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-108">**Appropriate roles**</span></span>

- <span data-ttu-id="0e8b1-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="0e8b1-109">Global admin</span></span>
- <span data-ttu-id="0e8b1-110">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="0e8b1-110">User management admin</span></span>
- <span data-ttu-id="0e8b1-111">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="0e8b1-111">Admin agent</span></span>
- <span data-ttu-id="0e8b1-112">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="0e8b1-112">Sales agent</span></span>

<span data-ttu-id="0e8b1-113">資料推動業務決策。</span><span class="sxs-lookup"><span data-stu-id="0e8b1-113">Data drives business decisions.</span></span> <span data-ttu-id="0e8b1-114">使用**經銷商分析**頁面上的計量，找出您的成功之處、您間接經銷商的成功之處，以及需要注意的領域。</span><span class="sxs-lookup"><span data-stu-id="0e8b1-114">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="0e8b1-115">在規劃新的業務務目標時，請使用此資訊。</span><span class="sxs-lookup"><span data-stu-id="0e8b1-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="0e8b1-116">間接經銷商分析僅適用於雲端解決方案提供者計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="0e8b1-116">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="0e8b1-117">我們正在追蹤下列計量︰</span><span class="sxs-lookup"><span data-stu-id="0e8b1-117">We are tracking the following metrics:</span></span>

<span data-ttu-id="0e8b1-118">**摘要**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-118">**Summary**</span></span>  
 - <span data-ttu-id="0e8b1-119">**經銷商總數**：在訂閱最後一天的使用中經銷商計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-119">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="0e8b1-120">**新經銷商**：在指定的時段中新的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-120">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="0e8b1-121">**使用中經銷商**：MPNID 至少有 1 個訂閱，以及訂閱狀態不是取消佈建的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-121">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="0e8b1-122">**交易中經銷商**：在指定的時段中有售出訂閱的間接經銷商計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-122">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="0e8b1-123">**依市場分類的經銷商**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-123">**Resellers by market**</span></span>  
 - <span data-ttu-id="0e8b1-124">依照地理位置分類的經銷商總數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-124">Total resellers by geographic location</span></span>  

<span data-ttu-id="0e8b1-125">**依照售出訂閱分類的熱門經銷商**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-125">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="0e8b1-126">依照售出訂閱數量排序的經銷商清單</span><span class="sxs-lookup"><span data-stu-id="0e8b1-126">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="0e8b1-127">**依訂閱計數排序的熱門產品**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-127">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="0e8b1-128">**Dynamics 365**：依售出訂閱排序的 Dynamics 365 產品</span><span class="sxs-lookup"><span data-stu-id="0e8b1-128">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="0e8b1-129">**EMS**：售出的企業管理服務訂閱數量</span><span class="sxs-lookup"><span data-stu-id="0e8b1-129">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="0e8b1-130">**Microsoft 365**：售出的 Microsoft 365 訂閱數量</span><span class="sxs-lookup"><span data-stu-id="0e8b1-130">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="0e8b1-131">**Office 365**：依售出訂閱排序的 Office 365 產品</span><span class="sxs-lookup"><span data-stu-id="0e8b1-131">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="0e8b1-132">**新增訂閱**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-132">**New subscriptions**</span></span>  
 - <span data-ttu-id="0e8b1-133">依日期新增的新訂閱數量</span><span class="sxs-lookup"><span data-stu-id="0e8b1-133">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="0e8b1-134">**訂閱流失**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-134">**Subscription churn**</span></span>  
 - <span data-ttu-id="0e8b1-135">**新訂閱**：依日期新增的新訂閱計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-135">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="0e8b1-136">**取消佈建的訂閱**：依日期的取消佈建或暫停訂閱計數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-136">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="0e8b1-137">**新經銷商詳細資料**</span><span class="sxs-lookup"><span data-stu-id="0e8b1-137">**New reseller details**</span></span>  
 - <span data-ttu-id="0e8b1-138">**經銷商名稱**：間接經銷商的名稱</span><span class="sxs-lookup"><span data-stu-id="0e8b1-138">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="0e8b1-139">**位置**：間接經銷商營運的市場</span><span class="sxs-lookup"><span data-stu-id="0e8b1-139">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="0e8b1-140">**訂閱**：經銷商售出的訂閱數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-140">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="0e8b1-141">**授權**：經銷商在所有訂閱中已售出的授權總數</span><span class="sxs-lookup"><span data-stu-id="0e8b1-141">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
  