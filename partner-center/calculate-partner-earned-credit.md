---
title: 合作夥伴的點數計算方式 |合作夥伴中心
ms.topic: article
ms.date: 09/17/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 如何計算合作夥伴如何取得 Azure 方案的信用額度
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 402ee0e2084191c7d4f592dd91480be8e1bd0341
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653713"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="81e99-103">如何計算合作夥伴的點數（PEC）</span><span class="sxs-lookup"><span data-stu-id="81e99-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="81e99-104">擁有雲端的全天候 IT 營運管理或其客戶在 CSP 中整個 Azure 環境的合作夥伴，會獲得 PEC 的獎勵。</span><span class="sxs-lookup"><span data-stu-id="81e99-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="81e99-105">PEC 會當做發票的一部分提供給與 Microsoft 直接計費關係的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="81e99-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="81e99-106">每日會計算點數，並反映在每月發票中。</span><span class="sxs-lookup"><span data-stu-id="81e99-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="81e99-107">根據預設，在 CSP 中，合作夥伴會被授與客戶訂用帳戶所需的存取權限，讓他們能夠全天候進行作業管理，並控制訂用帳戶上的資源。</span><span class="sxs-lookup"><span data-stu-id="81e99-107">By default, in CSP, partners are granted the necessary access rights to the customer's subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="81e99-108">下一節將說明客戶可以布建交易合作夥伴存取權的其他方式。</span><span class="sxs-lookup"><span data-stu-id="81e99-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="81e99-109">重要的資格和計算需求：</span><span class="sxs-lookup"><span data-stu-id="81e99-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="81e99-110">合作夥伴應具備作用中的 MPN 合約和以規則為基礎的有效帳戶 C （RBAC）角色，以接收所管理之 azure 資產的點數。</span><span class="sxs-lookup"><span data-stu-id="81e99-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="81e99-111">深入瞭解 [有效的 RBAC 角色]</span><span class="sxs-lookup"><span data-stu-id="81e99-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="81e99-112">如果間接提供者或其間接轉銷商，或兩者都有全天候作業控制和管理客戶在 CSP 中的 Azure 資源，則會符合 PEC 的資格。</span><span class="sxs-lookup"><span data-stu-id="81e99-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="81e99-113">PEC 會與合作夥伴所管理之客戶 Azure 資產的收費（收費）耗用量相關聯。</span><span class="sxs-lookup"><span data-stu-id="81e99-113">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="81e99-114">PEC 僅適用于由 Microsoft （間接提供者和直接帳單合作夥伴）計費的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="81e99-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="81e99-115">合格服務：合作夥伴獲得的信用額度適用于價格清單上的所有 Azure 1PP Azure 耗用量。</span><span class="sxs-lookup"><span data-stu-id="81e99-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="81e99-116">有一些例外狀況，包括但不限於3PP 和 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="81e99-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="81e99-117">PEC 會每日計算，並可在每日偵察檔案中查看。</span><span class="sxs-lookup"><span data-stu-id="81e99-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="81e99-118">合作夥伴（提供者或轉銷商（透過其提供者）必須具有整天（全天候）的存取權，以確保他們獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="81e99-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="81e99-119">PEC 會向下取得 Azure 資源層級。</span><span class="sxs-lookup"><span data-stu-id="81e99-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="81e99-120">如果合作夥伴在訂用帳戶或資源群組層級具有有效存取權，則每個位於較高實體之角色的資源都會獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="81e99-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="81e99-121">PEC 會包含在合作夥伴的每月發票上。</span><span class="sxs-lookup"><span data-stu-id="81e99-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="81e99-122">發票是費用的淨額。</span><span class="sxs-lookup"><span data-stu-id="81e99-122">The invoice is net of charges.</span></span> <span data-ttu-id="81e99-123">詳細資料會顯示在發票偵察檔案中。</span><span class="sxs-lookup"><span data-stu-id="81e99-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="81e99-124">如需取得管理 Azure 訂用帳戶的存取權，以及如何將您的 MPN ID 連結至 RBAC 角色的詳細資訊，請參閱[管理 azure 方案下的訂用帳戶和資源](azure-plan-manage.md)。</span><span class="sxs-lookup"><span data-stu-id="81e99-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="81e99-125">其他資訊</span><span class="sxs-lookup"><span data-stu-id="81e99-125">For more information</span></span>

- [<span data-ttu-id="81e99-126">Azure 方案-計費</span><span class="sxs-lookup"><span data-stu-id="81e99-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="81e99-127">CSP 中新商務體驗的價目表</span><span class="sxs-lookup"><span data-stu-id="81e99-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)