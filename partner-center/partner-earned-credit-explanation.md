---
title: 受控服務的合作夥伴所獲得信用點數
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入了解受控服務的 Microsoft 合作夥伴所獲得信用點數 (PEC) 如何計算及支付，以及如何確保您符合資格。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622162"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a><span data-ttu-id="1b4bd-103">合作夥伴所獲得信用點數如何計算及付費</span><span class="sxs-lookup"><span data-stu-id="1b4bd-103">How the partner earned credit is calculated and paid</span></span>

<span data-ttu-id="1b4bd-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="1b4bd-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1b4bd-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="1b4bd-105">Global admin</span></span>
- <span data-ttu-id="1b4bd-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="1b4bd-106">User admin</span></span>
- <span data-ttu-id="1b4bd-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="1b4bd-107">Admin agent</span></span>
- <span data-ttu-id="1b4bd-108">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="1b4bd-108">Billing admin</span></span>
- <span data-ttu-id="1b4bd-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="1b4bd-109">Sales agent</span></span>

<span data-ttu-id="1b4bd-110">針對受控服務 (PEC) 取得的合作夥伴所獲得信用點數，可辨識和獎勵合作夥伴，其擁有全天候 IT 營運控制及管理其客戶的部分或全部 Azure 環境。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-110">Partner earned credit for managed services (PEC) recognizes and rewards partners that own the 24x7 IT operational control and management of parts of, or the entire, Azure environment of their customers.</span></span> <span data-ttu-id="1b4bd-111">根據預設，在 CSP 中，合作夥伴會被授與客戶訂用帳戶的必要存取權，讓他們能夠執行全天候的作業管理，並控制訂用帳戶上的資源。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-111">By default, in CSP, partners are granted the necessary access rights to the customer's subscription allowing them to perform 24 X 7 operational management and control of the resources on the subscription.</span></span> <span data-ttu-id="1b4bd-112">下一節將說明客戶可以為交易合作夥伴佈建存取權的其他方式。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-112">Additional ways in which customer can provision access for transacting partner is described in the following section.</span></span> <span data-ttu-id="1b4bd-113">每月發票金額為合作夥伴所獲得信用點數的淨額。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-113">The monthly invoice amount is net of partner earned credit.</span></span> <span data-ttu-id="1b4bd-114">合作夥伴可以在他們的每月對帳檔案上查看 PEC 詳細資料。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-114">Partners can see the PEC details on their monthly recon file.</span></span> <span data-ttu-id="1b4bd-115">如需客戶可以為交易合作夥伴佈建存取權的其他方式，請參閱[管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-115">For additional ways in which a customer can provision access for the transacting partner, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="1b4bd-116">另請參閱[恢復 Azure CSP 訂用帳戶的系統管理員權限](revoke-reinstate-csp.md)</span><span class="sxs-lookup"><span data-stu-id="1b4bd-116">Also read [Reinstate admin privileges for Azure CSP subscriptions](revoke-reinstate-csp.md)</span></span>

## <a name="eligibility"></a><span data-ttu-id="1b4bd-117">資格</span><span class="sxs-lookup"><span data-stu-id="1b4bd-117">Eligibility</span></span>

<span data-ttu-id="1b4bd-118">若要接收合夥點數 (PEC)，必須滿足下列需求：</span><span class="sxs-lookup"><span data-stu-id="1b4bd-118">In order to receive the partner earned credit (PEC), the following requirements apply:</span></span> 

- <span data-ttu-id="1b4bd-119">您應具備作用中的 MPN 合約和有效的角色型存取控制 (RBAC) 角色，才能接收所管理之 Azure 資產的所獲得信用點數。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-119">You must have an active MPN agreement and valid role-based access control (RBAC) role to receive earned credit for the Azure assets you manage.</span></span>

- <span data-ttu-id="1b4bd-120">您必須具有在 CSP 中客戶 Azure 資源的全天候營運控制和管理。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-120">You must have 24x7 operational control and management of the customer's Azure resources in CSP.</span></span> <span data-ttu-id="1b4bd-121">這表示您必須在客戶的 Azure 訂用帳戶、Azure 資源群組、Azure 資源上擁有系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-121">This means you must have admin privileges on the customer’s Azure subscription, Azure resource group, Azure resource.</span></span> <span data-ttu-id="1b4bd-122">在間接提供者及其間接經銷商的案例中，如果間接提供者或間接經銷商或雙方都有此營運控制和管理，間接提供者就有資格使用 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-122">In the case of indirect providers and their indirect resellers, the indirect provider will be eligible for PEC if either the indirect provider or the indirect reseller or both have this operational control.</span></span> <span data-ttu-id="1b4bd-123">若要深入了解，請參閱[恢復 Azure CSP 訂用帳戶的系統管理員權限](https://docs.microsoft.com/partner-center/revoke-reinstate-csp)。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-123">To learn more about this, see [Reinstate admin privileges for Azure CSP subscriptions](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).</span></span>

- <span data-ttu-id="1b4bd-124">除了以上要求，PEC 僅適用於 Azure 方案耗用量價格中所列的服務，您可以從 [Azure 方案價格](https://partner.microsoft.com/commerce/sales)頁面匯出這些資訊。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-124">In addition to the requirements above, PEC is only applicable to services listed in the Azure plan consumption pricing, which you can export from the [Azure plan pricing](https://partner.microsoft.com/commerce/sales) page.</span></span>

- <span data-ttu-id="1b4bd-125">PEC **不** 適用於下列服務：</span><span class="sxs-lookup"><span data-stu-id="1b4bd-125">PEC is **not** applicable to the following services:</span></span>
    - <span data-ttu-id="1b4bd-126">Azure 方案保留</span><span class="sxs-lookup"><span data-stu-id="1b4bd-126">Azure Plan reservations</span></span>
    - <span data-ttu-id="1b4bd-127">在 Azure 方案耗用量價格的標記資料行中，識別為「第三方」的第三方產品</span><span class="sxs-lookup"><span data-stu-id="1b4bd-127">Third-party products identified as Third Party in the Tags column of the Azure plan consumption price</span></span>
    - <span data-ttu-id="1b4bd-128">Marketplace 價目表中的產品</span><span class="sxs-lookup"><span data-stu-id="1b4bd-128">Products in the Marketplace price list</span></span>
    - [<span data-ttu-id="1b4bd-129">Azure Spot 虛擬機器</span><span class="sxs-lookup"><span data-stu-id="1b4bd-129">Azure Spot Virtual Machines</span></span>](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- <span data-ttu-id="1b4bd-130">PEC 會向下獲得至 Azure 資源層級。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-130">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="1b4bd-131">如果您在訂用帳戶或資源群組層級上具有有效存取權，每個具有較高實體的資源可以獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-131">If you have valid access at either the subscription or resource group level, each resource that rolls up to the higher entity will earn PEC.</span></span>

- <span data-ttu-id="1b4bd-132">您也可以在 [Azure 成本管理](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners)頁面上取得 PEC 的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-132">Details on PEC are also available on the [Azure Cost management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners) page.</span></span>

### <a name="calculation"></a><span data-ttu-id="1b4bd-133">計算</span><span class="sxs-lookup"><span data-stu-id="1b4bd-133">Calculation</span></span>

<span data-ttu-id="1b4bd-134">PEC 會每日計算，並可在每日使用量檔案和每月發票對帳檔案中檢視。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-134">PEC is calculated daily and can be viewed in the daily usage file and monthly invoice recon file.</span></span> <span data-ttu-id="1b4bd-135">合作夥伴 (間接提供者或間接經銷商) 必須具有整天 (全天候) 的存取權，以確保他們獲得 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-135">A partner (indirect provider or indirect reseller) must have access for the entire day (24x7) to ensure they earn PEC.</span></span> <span data-ttu-id="1b4bd-136">系統會在受控 Azure 資產上每日計算 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-136">PEC is calculated on a daily basis on the managed Azure assets.</span></span> <span data-ttu-id="1b4bd-137">指定計費週期 (月) 的最大 PEC 為 15%。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-137">The maximum PEC for a given billing period (Month) is 15%.</span></span> <span data-ttu-id="1b4bd-138">在整個月 (存取跨度) 和所有合格資源 (存取範圍) 內保留永續性特殊權限存取的合作夥伴，將獲得 15% 的完整 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-138">Partners retaining persistent privileged access through the month (span of access) and for all the eligible resources (scope of access) will earn full PEC of 15%.</span></span> <span data-ttu-id="1b4bd-139">範圍和跨度縮減會導致該月的 PEC 率降低。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-139">Scope and span reduction will result in lower PEC rate for the month.</span></span> <span data-ttu-id="1b4bd-140">每日評等使用量檔案會每日顯示是否在 Azure 資產上套用 PEC。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-140">Daily rated usage file shows on a daily basis on an Azure asset, whether PEC is applied or not.</span></span> <span data-ttu-id="1b4bd-141">合作夥伴還可以註冊警示，以監視永續性特殊權限存取是否發生變更。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-141">Partners can also enroll in alerts to monitor changes to persistent privileged access.</span></span>

## <a name="azure-cost-management"></a><span data-ttu-id="1b4bd-142">Azure 成本管理</span><span class="sxs-lookup"><span data-stu-id="1b4bd-142">Azure Cost Management</span></span>

<span data-ttu-id="1b4bd-143">使用成本分析的 Azure 成本管理 (ACM) 可讓您成為合作夥伴，查看已獲得 PEC 優勢的成本。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-143">Azure Cost Management (ACM) using Cost Analysis enables you as a partner to view the costs that have received the benefit of PEC.</span></span>  

1. <span data-ttu-id="1b4bd-144">在 [Azure 入口網站](https://portal.azure.com)中，登入您的合作夥伴租用戶，然後選取 [成本管理 + 帳單]。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-144">In the [Azure portal](https://portal.azure.com), sign into your partner tenant and select **Cost Management + Billing**.</span></span>

2. <span data-ttu-id="1b4bd-145">選取 [Azure 成本管理]</span><span class="sxs-lookup"><span data-stu-id="1b4bd-145">Select **Cost management**</span></span>

3. <span data-ttu-id="1b4bd-146">選取 [成本分析]</span><span class="sxs-lookup"><span data-stu-id="1b4bd-146">Select **Cost Analysis**</span></span>

   <span data-ttu-id="1b4bd-147">[成本分析] 視圖會顯示您計費帳戶的成本，適用於以您支付 Microsoft 的價格所購買及使用的所有服務。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-147">The Cost Analysis view will display the costs for your billing account, for all the services purchased and consumed at the prices that you pay Microsoft.</span></span>

4. <span data-ttu-id="1b4bd-148">在樞紐分析表的下拉式清單中選取 **PartnerEarnedCreditApplied**，以查看已套用 PEC 的成本。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-148">Select **PartnerEarnedCreditApplied** in the drop down on a pivot chart to see costs that have PEC applied.</span></span> <span data-ttu-id="1b4bd-149">當 **PartnerEarnedCreditApplied** 屬性為 True 時，相關聯的成本就會享有合作夥伴所取得信用額度的權益。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-149">When **PartnerEarnedCreditApplied** property is True, the associated cost has the benefit of the partner earned credit.</span></span> 

   <span data-ttu-id="1b4bd-150">當 PartnerEarnedCreditApplied 屬性為 False 時，相關聯的成本尚不符合所需的信用額度資格，或所購買的服務不符合合作夥伴所取得的信用額度。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-150">When the PartnerEarnedCreditApplied property is False, the associated cost has not met the required eligibility for the credit or the service purchased is not eligible for partner earned credit.</span></span>

   >[!NOTE] 
   ><span data-ttu-id="1b4bd-151">一般而言，服務的使用量需要8-24 小時才會出現在 [成本管理] 中，而 PEC 信用額度會在 Azure 成本管理的存取時間起 48 小時內出現。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-151">Typically, usage for services takes 8-24 hours to appear in **Cost Management** and the PEC credits will appear within 48 hours from time of access in Azure Cost Management.</span></span>

5. <span data-ttu-id="1b4bd-152">您也可以使用 [分組依據及新增] 篩選功能，依據 PartnerEarnedCreditApplied 屬性分組及篩選，以深入瞭解具有 PEC 的成本，以及未套用任何 PEC 的成本。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-152">You can also group by, and filter by, the **PartnerEarnedCreditApplied** property using the **Group by and Add** filter features to drill into costs that have PEC and the costs that have no PEC applied.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b4bd-153">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="1b4bd-153">Next steps</span></span>

- [<span data-ttu-id="1b4bd-154">合作夥伴所獲得信用點數 - 概觀</span><span class="sxs-lookup"><span data-stu-id="1b4bd-154">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- <span data-ttu-id="1b4bd-155">合作夥伴所獲得信用點數計算的詳細範例在價目表上，您可以透過合作夥伴中心儀表板取得 (需要登入)。</span><span class="sxs-lookup"><span data-stu-id="1b4bd-155">Detailed examples of partner earned credit calculations are located on the price list which you can reach through the Partner Center dashboard (sign-in required).</span></span>

- [<span data-ttu-id="1b4bd-156">移至 Azure 方案 - 開始使用</span><span class="sxs-lookup"><span data-stu-id="1b4bd-156">Move to Azure plan - get started</span></span>](azure-plan-get-started.md)

- [<span data-ttu-id="1b4bd-157">管理 Azure 方案下的訂用帳戶和資源</span><span class="sxs-lookup"><span data-stu-id="1b4bd-157">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)

- [<span data-ttu-id="1b4bd-158">撤銷或恢復 Azure CSP 訂用帳戶的系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="1b4bd-158">Revoke or re-instate admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)
