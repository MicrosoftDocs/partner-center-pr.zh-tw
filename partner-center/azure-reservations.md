---
title: 銷售客戶 Microsoft Azure 保留
description: 雲端解決方案提供者，您可以為客戶購買、銷售或管理 Azure 保留。 使用合作夥伴中心、Azure 入口網站或合作夥伴中心 API。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000232"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="a87a1-104">使用合作夥伴中心、Azure 入口網站或 Api 銷售 Microsoft Azure 保留給客戶</span><span class="sxs-lookup"><span data-stu-id="a87a1-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="a87a1-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="a87a1-105">**Applies to**</span></span>

- <span data-ttu-id="a87a1-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a87a1-106">Partner Center</span></span>
- <span data-ttu-id="a87a1-107">Microsoft Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="a87a1-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="a87a1-108">雲端解決方案提供者方案中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a87a1-108">Partners in the CSP program</span></span>

<span data-ttu-id="a87a1-109">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="a87a1-109">**Appropriate roles**</span></span>

- <span data-ttu-id="a87a1-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="a87a1-110">Admin agent</span></span>
- <span data-ttu-id="a87a1-111">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a87a1-111">Global admin</span></span>
- <span data-ttu-id="a87a1-112">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="a87a1-112">Helpdesk agent</span></span>
- <span data-ttu-id="a87a1-113">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="a87a1-113">Sales agent</span></span>
- <span data-ttu-id="a87a1-114">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="a87a1-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="a87a1-115">本文僅適用于雲端解決方案提供者 (CSP) 計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="a87a1-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="a87a1-116">使用其他類型訂用帳戶的客戶 (例如隨用隨付、個別、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀 [此 Azure 保留檔](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="a87a1-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="a87a1-117">CSP 方案中的合作夥伴可以為客戶提供 Microsoft Azure 的保留。</span><span class="sxs-lookup"><span data-stu-id="a87a1-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="a87a1-118">如果客戶事先保留，即可獲得大幅節省。</span><span class="sxs-lookup"><span data-stu-id="a87a1-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="a87a1-119">Azure 保留專案以下列方式提供客戶簡單性和彈性：</span><span class="sxs-lookup"><span data-stu-id="a87a1-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="a87a1-120">一年或三年保留期限</span><span class="sxs-lookup"><span data-stu-id="a87a1-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="a87a1-121">輕鬆入門；在數秒內完成設定</span><span class="sxs-lookup"><span data-stu-id="a87a1-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="a87a1-122">隨時可取消或交換保留的執行個體以調整退款</span><span class="sxs-lookup"><span data-stu-id="a87a1-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="a87a1-123">可在組織或個別部門層級管理保留的執行個體使用率</span><span class="sxs-lookup"><span data-stu-id="a87a1-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="a87a1-124">Azure 保留可透過下列方式吸引客戶：</span><span class="sxs-lookup"><span data-stu-id="a87a1-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="a87a1-125">保留可提供隨用隨付的大量節省 (PAYG) 定價</span><span class="sxs-lookup"><span data-stu-id="a87a1-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="a87a1-126">事先支付一年或三年期限，能更理想掌控預算和預測</span><span class="sxs-lookup"><span data-stu-id="a87a1-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="a87a1-127">優先使用最接近辦公室的 Azure 區域運算容量</span><span class="sxs-lookup"><span data-stu-id="a87a1-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="a87a1-128">Azure 保留會在結合 Microsoft Windows Server 和 Azure SQL Database 等軟體時，提供端對端基礎結構解決方案的基礎</span><span class="sxs-lookup"><span data-stu-id="a87a1-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="a87a1-129">您可以在合作夥伴中心和 Azure 入口網站中購買、銷售及管理 Azure 保留，以及使用合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="a87a1-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="a87a1-130">您也可以為您的客戶提供向您購買的 azure 訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="a87a1-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="a87a1-131">請依照下列連結以深入了解。</span><span class="sxs-lookup"><span data-stu-id="a87a1-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="a87a1-132">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="a87a1-132">Azure reservations resources</span></span>

|<span data-ttu-id="a87a1-133">**如需下列資訊**</span><span class="sxs-lookup"><span data-stu-id="a87a1-133">**For information about**</span></span>   |<span data-ttu-id="a87a1-134">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="a87a1-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="a87a1-135">適用于您客戶的 Azure 保留檔</span><span class="sxs-lookup"><span data-stu-id="a87a1-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="a87a1-136">什麼是 Azure 保留？</span><span class="sxs-lookup"><span data-stu-id="a87a1-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="a87a1-137">在合作夥伴中心中為您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="a87a1-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="a87a1-138">購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="a87a1-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="a87a1-139">在合作夥伴中心中管理 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="a87a1-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="a87a1-140">在合作夥伴中心中管理 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="a87a1-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="a87a1-141">判斷正確的 VM 大小並確認客戶 VM 使用量</span><span class="sxs-lookup"><span data-stu-id="a87a1-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="a87a1-142">調整 VM 大小以提供最大 Azure Reservations 使用率</span><span class="sxs-lookup"><span data-stu-id="a87a1-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="a87a1-143">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="a87a1-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="a87a1-144">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="a87a1-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="a87a1-145">提供客戶從您的 CSP 訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="a87a1-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="a87a1-146">提供客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="a87a1-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |