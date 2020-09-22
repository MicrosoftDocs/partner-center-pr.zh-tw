---
title: '& 伺服器訂用帳戶的 Azure 保留'
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何雲端解決方案提供者機會取得、布建及管理客戶的 Azure 保留專案和伺服器訂閱。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3c08e897a8f5d7c11b36627b0c24ad2da3f92329
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000202"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="b3d26-103">取得、布建、& 管理 Azure 保留的 VM 實例 (RI) + 適用于客戶的伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="b3d26-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="b3d26-104">Applies to:</span></span>

- <span data-ttu-id="b3d26-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="b3d26-105">Partner Center</span></span>

<span data-ttu-id="b3d26-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="b3d26-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b3d26-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="b3d26-107">Admin agent</span></span>
- <span data-ttu-id="b3d26-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="b3d26-108">Global admin</span></span>
- <span data-ttu-id="b3d26-109">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="b3d26-109">Helpdesk agent</span></span>
- <span data-ttu-id="b3d26-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="b3d26-110">Sales agent</span></span>
- <span data-ttu-id="b3d26-111">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="b3d26-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="b3d26-112">本文僅適用于雲端解決方案提供者 (CSP) 計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="b3d26-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="b3d26-113">使用其他類型訂用帳戶的客戶 (例如隨用隨付、個別、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀 [此 Azure 保留檔](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="b3d26-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="b3d26-114">什麼是 Azure 保留項目？</span><span class="sxs-lookup"><span data-stu-id="b3d26-114">What are Azure Reservations?</span></span>

<span data-ttu-id="b3d26-115">Azure 保留可協助您藉由預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="b3d26-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="b3d26-116">預先支付費用可讓您在所使用的資源上取得折扣。</span><span class="sxs-lookup"><span data-stu-id="b3d26-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="b3d26-117">相較于隨用隨付價格，保留可以大幅減少72% 的虛擬機器、SQL 資料庫計算、Azure Cosmos DB 和其他資源成本。</span><span class="sxs-lookup"><span data-stu-id="b3d26-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="b3d26-118">保留會提供計費折扣，且不會影響資源的執行階段狀態。</span><span class="sxs-lookup"><span data-stu-id="b3d26-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="b3d26-119">如需詳細資訊，請參閱 [什麼是 Azure 保留？](/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="b3d26-119">For more information see [What are Azure Reservations?](/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="b3d26-120">客戶為什麼要購買保留？</span><span class="sxs-lookup"><span data-stu-id="b3d26-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="b3d26-121">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留可提供給他們最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="b3d26-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="b3d26-122">例如，如果客戶持續在沒有保留的情況下執行服務的四個實例，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="b3d26-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="b3d26-123">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="b3d26-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="b3d26-124">那些資源將不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="b3d26-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="b3d26-125">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="b3d26-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="b3d26-126">藉由將 Azure 保留專案和伺服器訂用帳戶帶入其 CSP 方案，Microsoft 更能讓其合作夥伴滿足快速成長的客戶需求，以獲得更符合成本效益的解決方案，以支援高度可預測、持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="b3d26-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="b3d26-127">CSP 方案可讓合作夥伴透過 Microsoft 合作夥伴中心和 Azure 入口網站，代表商業客戶取得、布建及管理 Azure 保留專案和伺服器訂閱。</span><span class="sxs-lookup"><span data-stu-id="b3d26-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="b3d26-128">我們甚至會提供 CSP 方案中的合作夥伴方案選擇，以瞭解如何購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="b3d26-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="b3d26-129">CSP 合作夥伴可以 [代表客戶購買 Azure 保留](azure-reservations-buying.md) ，也可以讓客戶從合作夥伴為其購買的先前 Azure 訂用帳戶 [購買自己的保留](give-customers-permission.md) 。</span><span class="sxs-lookup"><span data-stu-id="b3d26-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="b3d26-130">Azure 保留可為客戶提供各種運算解決方案的虛擬化彈性，包括開發和測試、執行應用程式以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="b3d26-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="b3d26-131">使用 [Azure 保留的 VM 執行個體](https://azure.microsoft.com/pricing/reserved-vm-instances/) 例如，商業客戶現在可以透過購買或「保留」（為期1年或3年期的虛擬機器），省下最多72% 與隨用隨付的 Azure VM 定價。</span><span class="sxs-lookup"><span data-stu-id="b3d26-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="b3d26-132">具備 Azure Hybrid Benefit (隨附於軟體保證) 的 Windows Server 客戶，相較於隨付隨用定價方式，則可節省高達 80%。</span><span class="sxs-lookup"><span data-stu-id="b3d26-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="b3d26-133">由於有無可匹敵的定價和無與倫比的部署彈性，客戶在選擇 Azure 保留時，將會看到最佳的整體價值：</span><span class="sxs-lookup"><span data-stu-id="b3d26-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="b3d26-134">Azure 保留</span><span class="sxs-lookup"><span data-stu-id="b3d26-134">Azure reservations</span></span>

- <span data-ttu-id="b3d26-135">Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="b3d26-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="b3d26-136">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="b3d26-136">SQL DB Reservations</span></span>
- <span data-ttu-id="b3d26-137">SQL 受控執行個體</span><span class="sxs-lookup"><span data-stu-id="b3d26-137">SQL Managed Instance</span></span>
- <span data-ttu-id="b3d26-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="b3d26-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="b3d26-139">Azure SQL 資料倉儲</span><span class="sxs-lookup"><span data-stu-id="b3d26-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="b3d26-140">應用程式服務</span><span class="sxs-lookup"><span data-stu-id="b3d26-140">App Services</span></span>
- <span data-ttu-id="b3d26-141">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="b3d26-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="b3d26-142">受控磁碟</span><span class="sxs-lookup"><span data-stu-id="b3d26-142">Managed Disk</span></span>
- <span data-ttu-id="b3d26-143">區塊 Blob</span><span class="sxs-lookup"><span data-stu-id="b3d26-143">Block blob</span></span>
- <span data-ttu-id="b3d26-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="b3d26-144">MySQL</span></span>
- <span data-ttu-id="b3d26-145">Azure 資料瀏覽器</span><span class="sxs-lookup"><span data-stu-id="b3d26-145">Azure Data explorer</span></span>
- <span data-ttu-id="b3d26-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="b3d26-146">MariaDB</span></span>
- <span data-ttu-id="b3d26-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="b3d26-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="b3d26-148">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-148">Server subscriptions</span></span>

- <span data-ttu-id="b3d26-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="b3d26-149">Windows Server</span></span>
- <span data-ttu-id="b3d26-150">遠端桌面服務 (RDS) Cal</span><span class="sxs-lookup"><span data-stu-id="b3d26-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="b3d26-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="b3d26-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="b3d26-152">Linux ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="b3d26-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="b3d26-153">SUSE Linux</span></span>
- <span data-ttu-id="b3d26-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="b3d26-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="b3d26-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="b3d26-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="b3d26-156">ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="b3d26-157">由 CloudSimple 提供的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="b3d26-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="b3d26-158">開始使用</span><span class="sxs-lookup"><span data-stu-id="b3d26-158">Getting started</span></span>

<span data-ttu-id="b3d26-159">若要瞭解如何將 Azure 保留區與客戶定位，並儘快啟動並執行，我們建議使用下列方法來複習準備教材：</span><span class="sxs-lookup"><span data-stu-id="b3d26-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="b3d26-160">檢閱《概觀簡報》及相關客戶價值主張與定位的網路研討會</span><span class="sxs-lookup"><span data-stu-id="b3d26-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="b3d26-161">檢視並了解《現代商務營運指南》(Modern Commerce Operating Guide)</span><span class="sxs-lookup"><span data-stu-id="b3d26-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="b3d26-162">檢視 Azure RI 和伺服器訂閱常見問題</span><span class="sxs-lookup"><span data-stu-id="b3d26-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="b3d26-163">了解[合作夥伴中心 API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure Reservations 和伺服器訂閱更新</span><span class="sxs-lookup"><span data-stu-id="b3d26-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="b3d26-164">資源</span><span class="sxs-lookup"><span data-stu-id="b3d26-164">Resources</span></span>

<span data-ttu-id="b3d26-165">以下提供完整的資源清單，可協助您快速上線以在合作夥伴中心交易 Azure Reservations：</span><span class="sxs-lookup"><span data-stu-id="b3d26-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="b3d26-166">銷售就緒程度</span><span class="sxs-lookup"><span data-stu-id="b3d26-166">Sales readiness</span></span>

- [<span data-ttu-id="b3d26-167">具有 Azure Hybrid Benefit 總覽的 Azure 保留專案和伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="b3d26-168">銷售資料表</span><span class="sxs-lookup"><span data-stu-id="b3d26-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="b3d26-169">Azure 保留的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="b3d26-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="b3d26-170">Azure 保留和 SQL DB 的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="b3d26-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="b3d26-171">遠端桌面服務 (RDS) 用戶端存取許可證 (CAL)  (公告) </span><span class="sxs-lookup"><span data-stu-id="b3d26-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="b3d26-172">Azure 保留的 VM 執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="b3d26-172">Azure Reserved VM Instances (Azure portal)</span></span>](/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="b3d26-173">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="b3d26-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="b3d26-174">Azure 中的 SQL DB 總覽</span><span class="sxs-lookup"><span data-stu-id="b3d26-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="b3d26-175">SQL DB 保留 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="b3d26-175">SQL DB Reservations (Azure portal)</span></span>](/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="b3d26-176">Azure Cosmos DB (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="b3d26-176">Azure Cosmos DB (Azure portal)</span></span>](/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="b3d26-177">SQL 受控執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="b3d26-177">SQL Managed Instance (Azure portal)</span></span>](/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="b3d26-178">SUSE 和 Red Hat Enterprise Linux (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="b3d26-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="b3d26-179">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="b3d26-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="b3d26-180">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="b3d26-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="b3d26-181">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="b3d26-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="b3d26-182">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="b3d26-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="b3d26-183">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="b3d26-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="b3d26-184">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="b3d26-184">Azure Databricks unit reservations</span></span>](/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="b3d26-185">CSP 價位清單： **Microsoft Azure 的保留實例** 和 **軟體** 訂用帳戶價格清單都位於合作夥伴中心 [定價 &](https://partner.microsoft.com/pcv/sales) 供應專案] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="b3d26-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="b3d26-186">訓練</span><span class="sxs-lookup"><span data-stu-id="b3d26-186">Training</span></span>

<span data-ttu-id="b3d26-187">註冊以查看 [商業授權就緒網路研討會](https://commercial-licensing.eventbuilder.com/FY2019_ALL) 和隨選事件。</span><span class="sxs-lookup"><span data-stu-id="b3d26-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="b3d26-188">授權就緒隨選事件包括下列主題：</span><span class="sxs-lookup"><span data-stu-id="b3d26-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="b3d26-189">CSP 線上服務、CSP Azure 和一般授權更新，包括 Azure (2018 年11月) </span><span class="sxs-lookup"><span data-stu-id="b3d26-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="b3d26-190">SQL 資料庫保留容量 & 實例大小彈性 (2018 年8月) </span><span class="sxs-lookup"><span data-stu-id="b3d26-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="b3d26-191">CSP 中的伺服器訂閱 (2018 年7月) </span><span class="sxs-lookup"><span data-stu-id="b3d26-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="b3d26-192">CSP 中的 Azure 保留專案總覽 (5 月 2018) </span><span class="sxs-lookup"><span data-stu-id="b3d26-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="b3d26-193">其他有用的訓練包含 [合作夥伴大學上的 Azure 授權模組](https://aka.ms/azure_partner_licensing)。</span><span class="sxs-lookup"><span data-stu-id="b3d26-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="b3d26-194">Operations</span><span class="sxs-lookup"><span data-stu-id="b3d26-194">Operations</span></span>

- <span data-ttu-id="b3d26-195">[新式商務操作指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (更新) ：涵蓋重要原則和操作層面的完整指南，例如合約、透過合作夥伴中心、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和 Azure 合作夥伴共用服務進行排序。</span><span class="sxs-lookup"><span data-stu-id="b3d26-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="b3d26-196">現代化優惠國家/地區可用性和客戶貨幣矩陣</span><span class="sxs-lookup"><span data-stu-id="b3d26-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="b3d26-197">銷售 Microsoft Azure 保留的執行個體</span><span class="sxs-lookup"><span data-stu-id="b3d26-197">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md)
- [<span data-ttu-id="b3d26-198">代表您的客戶購買 Microsoft Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="b3d26-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](azure-reservations-buying.md)
- [<span data-ttu-id="b3d26-199">代表您的客戶管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="b3d26-199">Manage Azure reservations on behalf of your customers</span></span>](azure-reservations-manage.md)
- [<span data-ttu-id="b3d26-200">Azure Reservations 的帳單</span><span class="sxs-lookup"><span data-stu-id="b3d26-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="b3d26-201">調整 VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="b3d26-201">VM sizing for maximum reservation usage</span></span>](azure-usage.md)
- [<span data-ttu-id="b3d26-202">合作夥伴中心 API (API/SDK) </span><span class="sxs-lookup"><span data-stu-id="b3d26-202">Partner Center API (API/SDK)</span></span>](/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="b3d26-203">遠端桌面服務</span><span class="sxs-lookup"><span data-stu-id="b3d26-203">Remote Desktop Services</span></span>](/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="b3d26-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="b3d26-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="b3d26-205">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) 可協助您從您的 Windows Server 授權獲得更多價值，並可節省高達 \*47% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="b3d26-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="b3d26-206">您可以將權益搭配用於軟體保證所涵蓋的 Windows Server Datacenter 和 Standard Edition 授權。</span><span class="sxs-lookup"><span data-stu-id="b3d26-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="b3d26-207">視版本而定，您可以轉換或重複使用您的授權，以在 Azure 中執行 Windows Server 虛擬機器，並以較低的基礎計算費率)  (Linux 虛擬機器費率。</span><span class="sxs-lookup"><span data-stu-id="b3d26-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="b3d26-208">請參閱 [Azure Hybrid Benefit 常見問題集](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="b3d26-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="b3d26-209">\* 實際節省的金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="b3d26-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
