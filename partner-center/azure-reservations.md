---
title: 銷售客戶 Microsoft Azure 保留
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 身為雲端解決方案提供者，您可以購買、銷售或管理客戶的 Azure 保留專案。 使用合作夥伴中心、Azure 入口網站或合作夥伴中心 API。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, 管理, 帳單, 購買, Azure RI, Azure 保留的執行個體
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5393e757b209de5a7df22b35a0cee0703419bef4
ms.sourcegitcommit: 595b7de03963a4a78cad8344bd4b5d4f5cff9802
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/22/2020
ms.locfileid: "85198636"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="9a9f4-105">使用合作夥伴中心、Azure 入口網站或 Api，為客戶銷售 Microsoft Azure 預約</span><span class="sxs-lookup"><span data-stu-id="9a9f4-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="9a9f4-106">**適用於**</span><span class="sxs-lookup"><span data-stu-id="9a9f4-106">**Applies to**</span></span>

- <span data-ttu-id="9a9f4-107">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="9a9f4-107">Partner Center</span></span>
- <span data-ttu-id="9a9f4-108">Microsoft Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="9a9f4-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="9a9f4-109">雲端解決方案提供者中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="9a9f4-109">Partners in CSP</span></span>

<span data-ttu-id="9a9f4-110">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="9a9f4-110">**Appropriate roles**</span></span>

- <span data-ttu-id="9a9f4-111">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="9a9f4-111">Admin agent</span></span>
- <span data-ttu-id="9a9f4-112">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="9a9f4-112">Global admin</span></span>
- <span data-ttu-id="9a9f4-113">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="9a9f4-113">Helpdesk agent</span></span>
- <span data-ttu-id="9a9f4-114">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="9a9f4-114">Sales agent</span></span>
- <span data-ttu-id="9a9f4-115">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="9a9f4-115">User management admin</span></span>

<span data-ttu-id="9a9f4-116">雲端解決方案提供者方案（CSP）中的合作夥伴可以提供客戶 Microsoft Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="9a9f4-117">如果客戶事先保留，即可獲得大幅節省。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="9a9f4-118">Azure 保留專案以下列方式提供客戶簡單性和彈性：</span><span class="sxs-lookup"><span data-stu-id="9a9f4-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="9a9f4-119">一年或三年保留期限</span><span class="sxs-lookup"><span data-stu-id="9a9f4-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="9a9f4-120">輕鬆入門；在數秒內完成設定</span><span class="sxs-lookup"><span data-stu-id="9a9f4-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="9a9f4-121">隨時可取消或交換保留的執行個體以調整退款</span><span class="sxs-lookup"><span data-stu-id="9a9f4-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="9a9f4-122">可在組織或個別部門層級管理保留的執行個體使用率</span><span class="sxs-lookup"><span data-stu-id="9a9f4-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="9a9f4-123">Azure 保留可透過下列方式吸引客戶：</span><span class="sxs-lookup"><span data-stu-id="9a9f4-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="9a9f4-124">保留可透過隨用隨付（PAYG）定價提供可觀的節約</span><span class="sxs-lookup"><span data-stu-id="9a9f4-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="9a9f4-125">事先支付一年或三年期限，能更理想掌控預算和預測</span><span class="sxs-lookup"><span data-stu-id="9a9f4-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="9a9f4-126">優先使用最接近辦公室的 Azure 區域運算容量</span><span class="sxs-lookup"><span data-stu-id="9a9f4-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="9a9f4-127">Azure 保留專案可提供端對端基礎結構解決方案的基礎，並結合 Microsoft Windows Server 和 Azure SQL Database 這類軟體</span><span class="sxs-lookup"><span data-stu-id="9a9f4-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="9a9f4-128">您可以在合作夥伴中心和 Azure 入口網站中購買、銷售和管理 Azure 保留專案，以及使用合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="9a9f4-129">您也可以授與客戶從您購買的 Azure 訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="9a9f4-130">請依照下列連結以深入了解。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="9a9f4-131">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="9a9f4-131">Azure reservations resources</span></span>

|<span data-ttu-id="9a9f4-132">**如需下列資訊**</span><span class="sxs-lookup"><span data-stu-id="9a9f4-132">**For information about**</span></span>   |<span data-ttu-id="9a9f4-133">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="9a9f4-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="9a9f4-134">適用于您客戶的 Azure 保留檔</span><span class="sxs-lookup"><span data-stu-id="9a9f4-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="9a9f4-135">什麼是 Azure 保留專案？</span><span class="sxs-lookup"><span data-stu-id="9a9f4-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="9a9f4-136">在合作夥伴中心為您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="9a9f4-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="9a9f4-137">購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="9a9f4-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="9a9f4-138">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="9a9f4-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="9a9f4-139">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="9a9f4-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="9a9f4-140">判斷正確的 VM 大小，並確認客戶 VM 使用量</span><span class="sxs-lookup"><span data-stu-id="9a9f4-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="9a9f4-141">調整 VM 大小以提供最大 Azure Reservations 使用率</span><span class="sxs-lookup"><span data-stu-id="9a9f4-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="9a9f4-142">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="9a9f4-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="9a9f4-143">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="9a9f4-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="9a9f4-144">提供客戶從您的 CSP 訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="9a9f4-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="9a9f4-145">授與客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="9a9f4-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
