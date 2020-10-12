---
title: 受控服務的合作夥伴所獲得信用點數
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入了解受控服務的 Microsoft 合作夥伴所獲得信用點數 (PEC) 如何計算及支付，以及如何確保您符合資格。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3ceb2ded6e52083ad0d74a411026558fbce2f642
ms.sourcegitcommit: 883c332a10f51b41b72c2f3fe08bb9593b569d28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/08/2020
ms.locfileid: "91852583"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="45c27-103">合作夥伴所獲得信用點數如何計算及付費</span><span class="sxs-lookup"><span data-stu-id="45c27-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="45c27-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="45c27-104">**Appropriate roles**</span></span>

- <span data-ttu-id="45c27-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="45c27-105">Global admin</span></span>
- <span data-ttu-id="45c27-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="45c27-106">User admin</span></span>
- <span data-ttu-id="45c27-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="45c27-107">Admin agent</span></span>
- <span data-ttu-id="45c27-108">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="45c27-108">Billing admin</span></span>
- <span data-ttu-id="45c27-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="45c27-109">Sales agent</span></span>

<span data-ttu-id="45c27-110">針對受控服務 (PEC) 取得的合作夥伴所獲得信用點數，可辨識和獎勵合作夥伴，其擁有全天候 IT 營運控制及管理其客戶的部分或全部 Azure 環境。</span><span class="sxs-lookup"><span data-stu-id="45c27-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="45c27-111">根據預設，在 CSP 中，合作夥伴會被授與客戶訂用帳戶的必要存取權，讓他們能夠執行全天候的作業管理，並控制訂用帳戶上的資源。</span><span class="sxs-lookup"><span data-stu-id="45c27-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="45c27-112">下一節將說明客戶可以為交易合作夥伴佈建存取權的其他方式。</span><span class="sxs-lookup"><span data-stu-id="45c27-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="45c27-113">每月發票金額為合作夥伴所獲得信用點數的淨額。</span><span class="sxs-lookup"><span data-stu-id="45c27-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="45c27-114">合作夥伴可以在他們的每月對帳檔案上查看 PEC 詳細資料。</span><span class="sxs-lookup"><span data-stu-id="45c27-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="45c27-115">如需客戶可以為交易合作夥伴佈建存取權的其他方式，請參閱[管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)。</span><span class="sxs-lookup"><span data-stu-id="45c27-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="45c27-116">另請參閱[恢復 Azure CSP 訂用帳戶的系統管理員權限](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="45c27-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="important-eligibility-and-calculation-information"></a><span data-ttu-id="45c27-117">重要的資格和計算資訊</span><span class="sxs-lookup"><span data-stu-id="45c27-117">Important eligibility and calculation information</span></span>

- <span data-ttu-id="45c27-118">合作夥伴應具備作用中的 MPN 合約和有效的 RBAC 角色，才能獲得所管理 Azure 資產的所獲得信用點數。</span><span class="sxs-lookup"><span data-stu-id="45c27-118">Partner should have an active MPN agreement and valid RBAC role to receive earned credit for the Azure assets they manage.</span></span> 

- <span data-ttu-id="45c27-119">在間接提供者及其間接經銷商的案例中，如果間接提供者或間接經銷商或雙方都有全天候在 CSP 中對於客戶 Azure 資源的營運控制和管理，間接提供者就有資格使用 PEC。</span><span class="sxs-lookup"><span data-stu-id="45c27-119">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider, or the indirect reseller or both have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span>

- <span data-ttu-id="45c27-120">PEC 會與合作夥伴所管理 CSP 中客戶 Azure 資產的計費 (可收費) 耗用量相關聯。</span><span class="sxs-lookup"><span data-stu-id="45c27-120">PEC is associated to billed (chargeable) consumption of customer's Azure estate in CSP managed by the partner.</span></span> <span data-ttu-id="45c27-121">PEC 僅適用於由 Microsoft (間接提供者和直接計費合作夥伴) 所計費的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="45c27-121">PEC is made available only to partners in CSP billed by Microsoft (indirect provider and direct bill partner).</span></span> 

- <span data-ttu-id="45c27-122">合格的服務：合作夥伴所獲得信用點數適用於 **Azure 方案使用定價**中所列的服務，合作夥伴可以從 [Azure 方案定價](https://partner.microsoft.com/commerce/sales)頁面匯出。</span><span class="sxs-lookup"><span data-stu-id="45c27-122">Eligible services: Partner earned credit is applicable to services listed in the **Azure plan consumption pricing** which partners can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span> <span data-ttu-id="45c27-123">合作夥伴所獲得信用點數不適用於 Azure 方案使用價目表、Azure 方案保留、Marketplace 價目表中的產品和 [Azure Spot 虛擬機器](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)的 [標記] 資料行中，識別為 [協力廠商] 的協力廠商產品。</span><span class="sxs-lookup"><span data-stu-id="45c27-123">Partner earned credit is not applicable to third-party products identified as **Third Party** in the **Tags column** of the Azure plan consumption price list, Azure Plan reservations, products in the Marketplace price list and [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/).</span></span>

- <span data-ttu-id="45c27-124">PEC 會每日計算，並可在每日使用量檔案和每月發票對帳檔案中檢視。</span><span class="sxs-lookup"><span data-stu-id="45c27-124">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="45c27-125">合作夥伴 (間接提供者或間接經銷商) 必須具有整天 (全天候) 的存取權，以確保他們獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="45c27-125">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="45c27-126">PEC 會在受控 Azure 資產上每日進行計算。</span><span class="sxs-lookup"><span data-stu-id="45c27-126">PEC is calculated on daily basis on the managed Azure assets.</span></span> <span data-ttu-id="45c27-127">指定計費週期 (月) 的最大 PEC 為 15%。</span><span class="sxs-lookup"><span data-stu-id="45c27-127">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="45c27-128">在整個月 (存取跨度) 和所有合格資源 (存取範圍) 內保留永續性特殊權限存取的合作夥伴，將獲得 15% 的完整 PEC。</span><span class="sxs-lookup"><span data-stu-id="45c27-128">Partners retaining persistent privileged access through the month(span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="45c27-129">範圍和跨度縮減會導致該月的 PEC 率降低。</span><span class="sxs-lookup"><span data-stu-id="45c27-129">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="45c27-130">每日評等使用量檔案會每日根據 Azure 資產上是否套用 PEC 來顯示。</span><span class="sxs-lookup"><span data-stu-id="45c27-130">Daily rated usage file shows on daily basis on an Azure asset whether PEC is applied or not.</span></span> <span data-ttu-id="45c27-131">合作夥伴還可以註冊警示，以偵測永續性特殊權限存取是否發生變更。</span><span class="sxs-lookup"><span data-stu-id="45c27-131">Partners can also enroll in alerts to detect if there are changes to persistent privileged access.</span></span>

- <span data-ttu-id="45c27-132">PEC 會向下獲得至 Azure 資源層級。</span><span class="sxs-lookup"><span data-stu-id="45c27-132">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="45c27-133">如果合作夥伴在訂用帳戶或資源群組層級上具有有效存取權，每個資源具有較高實體的角色，則合作夥伴可以獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="45c27-133">If the partner has valid access at the subscription, or resource group level, each resource that roles up to the higher entity will earn PEC.</span></span>  

- <span data-ttu-id="45c27-134">[Azure 成本管理](/azure/cost-management-billing/costs/get-started-partners)也提供 PEC 詳細資料</span><span class="sxs-lookup"><span data-stu-id="45c27-134">PEC details will also be available on [Azure Cost management](/azure/cost-management-billing/costs/get-started-partners)</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="45c27-135">Azure 成本管理</span><span class="sxs-lookup"><span data-stu-id="45c27-135">Azure Cost Management</span></span>

<span data-ttu-id="45c27-136">使用成本分析的 Azure 成本管理 (ACM) 可讓您成為合作夥伴，查看已獲得 PEC 優勢的成本。</span><span class="sxs-lookup"><span data-stu-id="45c27-136">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="45c27-137">在 [Azure 入口網站](https://portal.azure.com)中，登入您的合作夥伴租用戶，然後選取 [成本管理 + 帳單]。</span><span class="sxs-lookup"><span data-stu-id="45c27-137">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="45c27-138">選取 [Azure 成本管理]</span><span class="sxs-lookup"><span data-stu-id="45c27-138">Select **Cost management**</span></span>

3. <span data-ttu-id="45c27-139">選取 [成本分析]</span><span class="sxs-lookup"><span data-stu-id="45c27-139">Select **Cost Analysis**</span></span>

   <span data-ttu-id="45c27-140">[成本分析] 視圖會顯示您計費帳戶的成本，適用於以您支付 Microsoft 的價格所購買及使用的所有服務。</span><span class="sxs-lookup"><span data-stu-id="45c27-140">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="45c27-141">在樞紐分析表的下拉式清單中選取 **PartnerEarnedCreditApplied**，以查看已套用 PEC 的成本。</span><span class="sxs-lookup"><span data-stu-id="45c27-141">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="45c27-142">當 **PartnerEarnedCreditApplied** 屬性為 True 時，相關聯的成本就會享有合作夥伴所取得信用額度的權益。</span><span class="sxs-lookup"><span data-stu-id="45c27-142">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

<span data-ttu-id="45c27-143">當 PartnerEarnedCreditApplied 屬性為 False 時，相關聯的成本尚不符合所需的信用額度資格，或所購買的服務不符合合作夥伴所取得的信用額度。</span><span class="sxs-lookup"><span data-stu-id="45c27-143">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

>[!NOTE] 
><span data-ttu-id="45c27-144">一般而言，服務的使用量需要8-24 小時才會出現在 [成本管理] 中，而 PEC 信用額度會在 Azure 成本管理的存取時間起 48 小時內出現。</span><span class="sxs-lookup"><span data-stu-id="45c27-144">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="45c27-145">您也可以使用 [分組依據及新增] 篩選功能，依據 PartnerEarnedCreditApplied 屬性分組及篩選，以深入瞭解具有 PEC 的成本，以及未套用任何 PEC 的成本。</span><span class="sxs-lookup"><span data-stu-id="45c27-145">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="45c27-146">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="45c27-146">Next steps</span></span>

- [<span data-ttu-id="45c27-147">合作夥伴所獲得信用點數 - 概觀</span><span class="sxs-lookup"><span data-stu-id="45c27-147">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="45c27-148">合作夥伴所獲得信用點數計算的詳細範例在價目表上，您可以透過合作夥伴中心儀表板取得 (需要登入)。</span><span class="sxs-lookup"><span data-stu-id="45c27-148">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="45c27-149">移至 Azure 方案 - 開始使用</span><span class="sxs-lookup"><span data-stu-id="45c27-149">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="45c27-150">管理 Azure 方案下的訂用帳戶和資源</span><span class="sxs-lookup"><span data-stu-id="45c27-150">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="45c27-151">撤銷或恢復 Azure CSP 訂用帳戶的系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="45c27-151">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
