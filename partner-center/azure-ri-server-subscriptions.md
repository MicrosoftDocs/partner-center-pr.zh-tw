---
title: '& 伺服器訂用帳戶的 Azure 保留'
ms.topic: article
ms.date: 11/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何雲端解決方案提供者機會取得、布建及管理客戶的 Azure 保留專案和伺服器訂閱。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0434ad2e6494f5efc1b1e5e2aa003dc6587d7b4e
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691345"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="12501-103">取得、布建、& 管理 Azure 保留的 VM 實例 (RI) + 適用于客戶的伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="12501-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>


<span data-ttu-id="12501-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="12501-104">**Appropriate roles**</span></span>

- <span data-ttu-id="12501-105">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="12501-105">Admin agent</span></span>
- <span data-ttu-id="12501-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="12501-106">Global admin</span></span>
- <span data-ttu-id="12501-107">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="12501-107">Helpdesk agent</span></span>
- <span data-ttu-id="12501-108">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="12501-108">Sales agent</span></span>
- <span data-ttu-id="12501-109">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="12501-109">User management admin</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="12501-110">什麼是 Azure 保留項目？</span><span class="sxs-lookup"><span data-stu-id="12501-110">What are Azure Reservations?</span></span>

<span data-ttu-id="12501-111">Azure 保留可協助您藉由預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="12501-111">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="12501-112">預先支付費用可讓您在所使用的資源上取得折扣。</span><span class="sxs-lookup"><span data-stu-id="12501-112">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="12501-113">相較于隨用隨付價格，保留可以大幅減少72% 的虛擬機器、SQL 資料庫計算、Azure Cosmos DB 和其他資源成本。</span><span class="sxs-lookup"><span data-stu-id="12501-113">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="12501-114">保留會提供計費折扣，且不會影響資源的執行階段狀態。</span><span class="sxs-lookup"><span data-stu-id="12501-114">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="12501-115">如需詳細資訊，請參閱 [什麼是 Azure 保留？](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="12501-115">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="12501-116">客戶為什麼要購買保留？</span><span class="sxs-lookup"><span data-stu-id="12501-116">Why should customers buy a reservation?</span></span>

<span data-ttu-id="12501-117">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留可提供給他們最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="12501-117">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="12501-118">例如，如果客戶持續在沒有保留的情況下執行服務的四個實例，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="12501-118">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="12501-119">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="12501-119">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="12501-120">那些資源將不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="12501-120">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="12501-121">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="12501-121">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="12501-122">藉由將 Azure 保留專案和伺服器訂用帳戶帶入其 CSP 方案，Microsoft 更能讓其合作夥伴滿足快速成長的客戶需求，以獲得更符合成本效益的解決方案，以支援高度可預測、持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="12501-122">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="12501-123">CSP 方案可讓合作夥伴透過 Microsoft 合作夥伴中心和 Azure 入口網站，代表商業客戶取得、布建及管理 Azure 保留專案和伺服器訂閱。</span><span class="sxs-lookup"><span data-stu-id="12501-123">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>
<span data-ttu-id="12501-124">我們甚至會提供 CSP 方案中的合作夥伴方案選擇，以瞭解如何購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="12501-124">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="12501-125">CSP 合作夥伴可以 [代表客戶購買 Azure 保留](azure-reservations-buying.md) ，也可以讓客戶從合作夥伴為其購買的先前 Azure 訂用帳戶 [購買自己的保留](give-customers-permission.md) 。</span><span class="sxs-lookup"><span data-stu-id="12501-125">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="12501-126">Azure 保留可為客戶提供各種運算解決方案的虛擬化彈性，包括開發和測試、執行應用程式以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="12501-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="12501-127">使用 [Azure 保留的 VM 執行個體](https://azure.microsoft.com/pricing/reserved-vm-instances/) 例如，商業客戶現在可以透過購買或「保留」（為期1年或3年期的虛擬機器），省下最多72% 與隨用隨付的 Azure VM 定價。</span><span class="sxs-lookup"><span data-stu-id="12501-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="12501-128">具備 Azure Hybrid Benefit (隨附於軟體保證) 的 Windows Server 客戶，相較於隨付隨用定價方式，則可節省高達 80%。</span><span class="sxs-lookup"><span data-stu-id="12501-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="12501-129">由於有無可匹敵的定價與無與倫比的部署彈性，客戶在選擇 Azure 保留時，將會看到最佳的整體價值。</span><span class="sxs-lookup"><span data-stu-id="12501-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations.</span></span>

- <span data-ttu-id="12501-130">請參閱 Azure 入口網站上的 [購買保留](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) 。</span><span class="sxs-lookup"><span data-stu-id="12501-130">See [Purchase Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/prepare-buy-reservation#purchase-reservations) on the Azure Portal.</span></span>

- <span data-ttu-id="12501-131">如需軟體訂用帳戶和 Linux ISV 年度訂閱的合作夥伴中心，請參閱 [[定價和](https://partner.microsoft.com/dashboard/sell/pricingandoffers)供應專案] 頁面的 [ **Microsoft Azure 保留實例**] 類別下的 [ **Azure RI CSP 商業價位表**]。</span><span class="sxs-lookup"><span data-stu-id="12501-131">See the **Azure RI CSP Commercial Price List** under the **Microsoft Azure Reserved Instances** category on the [Pricing and Offers](https://partner.microsoft.com/dashboard/sell/pricingandoffers) page in Partner Center for software subscriptions and Linux ISV annual subscriptions.</span></span>


 
<span data-ttu-id="12501-132">**Linux ISV 年度訂閱**</span><span class="sxs-lookup"><span data-stu-id="12501-132">**Linux ISV annual subscriptions**</span></span>

- <span data-ttu-id="12501-133">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="12501-133">SUSE Linux</span></span>
- <span data-ttu-id="12501-134">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="12501-134">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="12501-135">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="12501-135">Azure Red Hat OpenShift</span></span>

<span data-ttu-id="12501-136">**ISV 年度訂閱**</span><span class="sxs-lookup"><span data-stu-id="12501-136">**ISV annual subscriptions**</span></span>

- <span data-ttu-id="12501-137">由 CloudSimple 提供的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="12501-137">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="12501-138">開始使用</span><span class="sxs-lookup"><span data-stu-id="12501-138">Getting started</span></span>

<span data-ttu-id="12501-139">若要瞭解如何將 Azure 保留區與客戶定位，並儘快啟動並執行，我們建議使用下列方法來複習準備教材：</span><span class="sxs-lookup"><span data-stu-id="12501-139">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="12501-140">複習並瞭解 [合作夥伴中心的新商務操作指南](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)。</span><span class="sxs-lookup"><span data-stu-id="12501-140">Review and understand the [Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf).</span></span>

2. <span data-ttu-id="12501-141">瞭解 [合作夥伴中心 api (api/SDK) ](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)中的 Azure 保留專案和伺服器訂閱的更新。</span><span class="sxs-lookup"><span data-stu-id="12501-141">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances).</span></span>


### <a name="sales-readiness"></a><span data-ttu-id="12501-142">銷售就緒程度</span><span class="sxs-lookup"><span data-stu-id="12501-142">Sales readiness</span></span>

- [<span data-ttu-id="12501-143">遠端桌面服務 (RDS) 用戶端存取許可證 (CAL)  (公告) </span><span class="sxs-lookup"><span data-stu-id="12501-143">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)

- [<span data-ttu-id="12501-144">Azure 保留的 VM 執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="12501-144">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)

- [<span data-ttu-id="12501-145">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="12501-145">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)

- [<span data-ttu-id="12501-146">SQL DB 保留 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="12501-146">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)

- [<span data-ttu-id="12501-147">Azure Cosmos DB (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="12501-147">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)

- [<span data-ttu-id="12501-148">SQL 受控執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="12501-148">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)

- [<span data-ttu-id="12501-149">SUSE 和 Red Hat Enterprise Linux (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="12501-149">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)

- [<span data-ttu-id="12501-150">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="12501-150">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)

- [<span data-ttu-id="12501-151">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="12501-151">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)

- [<span data-ttu-id="12501-152">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="12501-152">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)

- [<span data-ttu-id="12501-153">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="12501-153">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)

- [<span data-ttu-id="12501-154">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="12501-154">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)

- [<span data-ttu-id="12501-155">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="12501-155">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)


## <a name="training"></a><span data-ttu-id="12501-156">訓練</span><span class="sxs-lookup"><span data-stu-id="12501-156">Training</span></span>

<span data-ttu-id="12501-157">註冊以查看 [商業授權就緒網路研討會](https://commercial-licensing.eventbuilder.com/FY2019_ALL) 和隨選事件。</span><span class="sxs-lookup"><span data-stu-id="12501-157">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>
<span data-ttu-id="12501-158">先前錄製的授權就緒隨選事件包括如下的主題：</span><span class="sxs-lookup"><span data-stu-id="12501-158">Previously recorded Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="12501-159">CSP 線上服務、CSP Azure 和一般授權更新，包括 Azure (2018 年11月) </span><span class="sxs-lookup"><span data-stu-id="12501-159">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>

- <span data-ttu-id="12501-160">SQL 資料庫保留容量 & 實例大小彈性 (2018 年8月) </span><span class="sxs-lookup"><span data-stu-id="12501-160">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>

- <span data-ttu-id="12501-161">CSP 中的伺服器訂閱 (2018 年7月) </span><span class="sxs-lookup"><span data-stu-id="12501-161">Server Subscriptions in CSP (July 2018)</span></span>

- <span data-ttu-id="12501-162">CSP 中的 Azure 保留專案總覽 (5 月 2018) </span><span class="sxs-lookup"><span data-stu-id="12501-162">Azure Reservations Overview in CSP (May 2018)</span></span>

## <a name="operations"></a><span data-ttu-id="12501-163">Operations</span><span class="sxs-lookup"><span data-stu-id="12501-163">Operations</span></span>

<span data-ttu-id="12501-164">[合作夥伴中心新的商務操作指南](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)：涵蓋重要原則和操作方面的完整指南，例如合約、依合作夥伴中心、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和 Azure 合作夥伴共用服務的排序。</span><span class="sxs-lookup"><span data-stu-id="12501-164">[Partner Center new commerce operations guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf):  Comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="12501-165">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="12501-165">Azure Hybrid Benefit</span></span>

<span data-ttu-id="12501-166">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit)是具有軟體保證授權之客戶的定價權益，可協助您在遷移至 Azure 時，將現有內部部署 Windows Server 和/或 SQL Server 授權投資的價值最大化。</span><span class="sxs-lookup"><span data-stu-id="12501-166">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) is a pricing benefit for customers who have licenses with Software Assurance, which helps maximize the value of existing on-premises Windows Server and/or SQL Server license investments when migrating to Azure.</span></span> <span data-ttu-id="12501-167">符合資格的客戶可在 Azure 虛擬機器上省下最多 40% \* 的 (基礎結構即服務或 IaaS) ，最高可省下55% 的 Azure SQL Database (平臺即服務，或在 Azure 虛擬機器上的平臺即服務，或 PaaS) 和 SQL Server 的 Azure 虛擬機器上使用 (，這會隨著 Azure 保留實例而增加至80%。</span><span class="sxs-lookup"><span data-stu-id="12501-167">Eligible customers can save up to 40%\* on Azure Virtual Machines (infrastructure as a service, or IaaS), and save up to 55% on Azure SQL Database (platform as a service, or PaaS) and SQL Server on Azure Virtual Machines (IaaS) with Azure Hybrid Benefit, which increases to up to 80% when combined with Azure Reserved Instances.</span></span>

## <a name="next-steps"></a><span data-ttu-id="12501-168">後續步驟</span><span class="sxs-lookup"><span data-stu-id="12501-168">Next steps</span></span>

- [<span data-ttu-id="12501-169">Azure Hybrid Benefit 常見問題</span><span class="sxs-lookup"><span data-stu-id="12501-169">Azure Hybrid Benefit FAQ</span></span>](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)

<span data-ttu-id="12501-170">\* 實際節省的金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="12501-170">\*Actual savings may vary based on region, instance type, or usage.</span></span>
