---
title: Azure 保留的 VM 執行個體 (RI) + Azure 伺服器訂閱 | 合作夥伴中心
ms.topic: article
ms.date: 12/02/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解雲端解決方案提供者如何取得、布建及管理其客戶的 Azure 保留和伺服器訂閱。
author: LauraBrenner
ms.author: labrenne
keywords: Azure，訂用帳戶，VM，保留，保留實例
ms.localizationpriority: medium
ms.openlocfilehash: 22ba6af523bf73d9d7778940ef7495e6581a0730
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722261"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="dc695-104">Azure 保留的 VM 執行個體 (RI) + Azure 伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="dc695-105">適用於：</span><span class="sxs-lookup"><span data-stu-id="dc695-105">Applies to:</span></span>

- <span data-ttu-id="dc695-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="dc695-106">Partner Center</span></span>

<span data-ttu-id="dc695-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="dc695-107">**Appropriate roles**</span></span>

- <span data-ttu-id="dc695-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="dc695-108">Admin agent</span></span>
- <span data-ttu-id="dc695-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="dc695-109">Global admin</span></span>
- <span data-ttu-id="dc695-110">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="dc695-110">Helpdesk agent</span></span>
- <span data-ttu-id="dc695-111">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="dc695-111">Sales agent</span></span>
- <span data-ttu-id="dc695-112">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="dc695-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="dc695-113">什麼是 Azure 保留專案？</span><span class="sxs-lookup"><span data-stu-id="dc695-113">What are Azure Reservations?</span></span>

<span data-ttu-id="dc695-114">Azure 保留可協助您透過預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="dc695-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="dc695-115">預先付款可讓您獲得所用資源的折扣。</span><span class="sxs-lookup"><span data-stu-id="dc695-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="dc695-116">相較於隨付隨用價格，保留區可將虛擬機器、SQL Database 計算、Azure Cosmos DB 和其他資源的成本大幅降低至最多 72%。</span><span class="sxs-lookup"><span data-stu-id="dc695-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="dc695-117">保留會提供計費折扣，且不會影響資源的執行時間狀態。如需詳細資訊，請參閱[什麼是 Azure 保留專案？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="dc695-117">Reservations provide a billing discount and don't affect the runtime state of your resources.For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="dc695-118">為什麼客戶要購買保留？</span><span class="sxs-lookup"><span data-stu-id="dc695-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="dc695-119">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留會使其成為最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="dc695-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="dc695-120">例如，如果客戶連續執行服務的四個實例，而沒有保留，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="dc695-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="dc695-121">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="dc695-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="dc695-122">資源不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="dc695-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="dc695-123">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="dc695-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="dc695-124">Microsoft 藉由將 Azure 保留和伺服器訂用帳戶帶入其 CSP 計畫，讓其合作夥伴能夠解決快速成長的客戶需求，以提供更符合成本效益的解決方案，以支援高度可預測且持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="dc695-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="dc695-125">CSP 計畫可讓合作夥伴透過 Microsoft 合作夥伴中心和 Azure 入口網站，代表商業客戶取得、布建及管理 Azure 保留專案和伺服器訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="dc695-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure Portal.</span></span>

<span data-ttu-id="dc695-126">Azure 保留可為客戶提供各種運算解決方案的虛擬化彈性，包括開發和測試、執行應用程式以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="dc695-126">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="dc695-127">例如，透過[Azure 保留的 VM 執行個體](https://azure.microsoft.com/pricing/reserved-vm-instances/)，商業客戶現在只要購買或「保留」，即可省下高達72% 的「隨用隨付」 Azure VM 定價（1或3年期的虛擬機器）。</span><span class="sxs-lookup"><span data-stu-id="dc695-127">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or “reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="dc695-128">具備 Azure Hybrid Benefit (隨附於軟體保證) 的 Windows Server 客戶，相較於隨付隨用定價方式，則可節省高達 80%。</span><span class="sxs-lookup"><span data-stu-id="dc695-128">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="dc695-129">透過無與倫比的定價和無與倫比的部署彈性組合，客戶在選擇 Azure 保留時，將會看到最佳的整體價值：</span><span class="sxs-lookup"><span data-stu-id="dc695-129">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="dc695-130">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="dc695-130">Azure reservations</span></span>

- <span data-ttu-id="dc695-131">Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="dc695-131">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="dc695-132">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="dc695-132">SQL DB Reservations</span></span>
- <span data-ttu-id="dc695-133">SQL 受控執行個體</span><span class="sxs-lookup"><span data-stu-id="dc695-133">SQL Managed Instance</span></span>
- <span data-ttu-id="dc695-134">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="dc695-134">Azure Cosmos DB</span></span>
- <span data-ttu-id="dc695-135">Azure SQL 資料倉儲</span><span class="sxs-lookup"><span data-stu-id="dc695-135">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="dc695-136">應用程式服務</span><span class="sxs-lookup"><span data-stu-id="dc695-136">App Services</span></span>
- <span data-ttu-id="dc695-137">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="dc695-137">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="dc695-138">受控磁片</span><span class="sxs-lookup"><span data-stu-id="dc695-138">Managed Disk</span></span>
- <span data-ttu-id="dc695-139">Blockblob</span><span class="sxs-lookup"><span data-stu-id="dc695-139">Blockblob</span></span>
- <span data-ttu-id="dc695-140">MySQL</span><span class="sxs-lookup"><span data-stu-id="dc695-140">MySQL</span></span>
- <span data-ttu-id="dc695-141">Azure 資料 explorer</span><span class="sxs-lookup"><span data-stu-id="dc695-141">Azure Data explorer</span></span>
- <span data-ttu-id="dc695-142">MariaDB</span><span class="sxs-lookup"><span data-stu-id="dc695-142">MariaDB</span></span>
- <span data-ttu-id="dc695-143">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="dc695-143">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="dc695-144">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-144">Server subscriptions</span></span>

- <span data-ttu-id="dc695-145">WIN ENT LTSB 2016 Estonian 64 Bits</span><span class="sxs-lookup"><span data-stu-id="dc695-145">Windows Server</span></span>
- <span data-ttu-id="dc695-146">遠端桌面服務（RDS） Cal</span><span class="sxs-lookup"><span data-stu-id="dc695-146">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="dc695-147">SQL Server</span><span class="sxs-lookup"><span data-stu-id="dc695-147">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="dc695-148">Linux ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-148">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="dc695-149">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="dc695-149">SUSE Linux</span></span>
- <span data-ttu-id="dc695-150">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="dc695-150">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="dc695-151">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="dc695-151">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="dc695-152">ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-152">ISV annual subscriptions</span></span>

- <span data-ttu-id="dc695-153">依 CloudSimple 的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="dc695-153">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="dc695-154">開始使用</span><span class="sxs-lookup"><span data-stu-id="dc695-154">Getting started</span></span>

<span data-ttu-id="dc695-155">若想了解如何針對您的客戶定位 Azure Reservations 以及盡快開始營運，建議採用下列方式來檢視整備材料：</span><span class="sxs-lookup"><span data-stu-id="dc695-155">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible we recommend the following approach for reviewing the readiness materials:</span></span>

1. <span data-ttu-id="dc695-156">檢閱《概觀簡報》及相關客戶價值主張與定位的網路研討會</span><span class="sxs-lookup"><span data-stu-id="dc695-156">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="dc695-157">檢視並了解《現代商務營運指南》(Modern Commerce Operating Guide)</span><span class="sxs-lookup"><span data-stu-id="dc695-157">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="dc695-158">檢視 Azure RI 和伺服器訂閱常見問題</span><span class="sxs-lookup"><span data-stu-id="dc695-158">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="dc695-159">了解[合作夥伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure Reservations 和伺服器訂閱更新</span><span class="sxs-lookup"><span data-stu-id="dc695-159">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="dc695-160">資源</span><span class="sxs-lookup"><span data-stu-id="dc695-160">Resources</span></span>

<span data-ttu-id="dc695-161">以下提供完整的資源清單，可協助您快速上線以在合作夥伴中心交易 Azure Reservations：</span><span class="sxs-lookup"><span data-stu-id="dc695-161">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="dc695-162">銷售就緒</span><span class="sxs-lookup"><span data-stu-id="dc695-162">Sales readiness</span></span>

- [<span data-ttu-id="dc695-163">具有 Azure Hybrid Benefit 總覽的 Azure 保留和伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-163">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="dc695-164">銷售資料表</span><span class="sxs-lookup"><span data-stu-id="dc695-164">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="dc695-165">Azure 保留的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="dc695-165">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="dc695-166">Azure Reservations 和 SQL DB 合作夥伴常見問題集</span><span class="sxs-lookup"><span data-stu-id="dc695-166">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="dc695-167">遠端桌面服務（RDS） Cal （公告）</span><span class="sxs-lookup"><span data-stu-id="dc695-167">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="dc695-168">Azure 保留的 VM 執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="dc695-168">Azure Reserved VM Instances (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="dc695-169">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="dc695-169">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="dc695-170">Azure 中的 SQL DB 總覽</span><span class="sxs-lookup"><span data-stu-id="dc695-170">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="dc695-171">SQL DB 保留（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="dc695-171">SQL DB Reservations (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="dc695-172">Azure Cosmos DB （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="dc695-172">Azure Cosmos DB (Azure Portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="dc695-173">SQL 受控執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="dc695-173">SQL Managed Instance (Azure Portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="dc695-174">SUSE 和 Red Hat Enterprise Linux （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="dc695-174">SUSE and Red Hat Enterprise Linux (Azure Portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="dc695-175">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="dc695-175">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="dc695-176">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="dc695-176">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="dc695-177">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="dc695-177">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="dc695-178">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="dc695-178">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="dc695-179">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="dc695-179">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="dc695-180">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="dc695-180">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="dc695-181">CSP 價目表： **Microsoft Azure 保留實例**和**軟體**訂用帳戶價格清單都位於合作夥伴中心[定價 &](https://partner.microsoft.com/pcv/sales)供應專案 頁面上。</span><span class="sxs-lookup"><span data-stu-id="dc695-181">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="dc695-182">訓練</span><span class="sxs-lookup"><span data-stu-id="dc695-182">Training</span></span>

- <span data-ttu-id="dc695-183">[2018 年11月的商業授權就緒網路研討會](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0)，涵蓋 Csp 線上服務、CSP Azure 和一般授權更新（包括 Azure）</span><span class="sxs-lookup"><span data-stu-id="dc695-183">[November 2018 Commercial Licensing Readiness Webinars](https://na01.safelinks.protection.outlook.com/?url=https%3A%2F%2Fcommercial-licensing.eventbuilder.com%2F%3Flandingpageid%3DV0Bx6L&data=02%7C01%7Cv-oumaki%40microsoft.com%7C96e24687952242e1ff0c08d62ada13f3%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636743513471330495&sdata=DjPAKnW%2BpVekRS3Zngy2uwAkTpU4z1O%2Fh56NuTOmCzM%3D&reserved=0) covering CSP Online Services, CSP Azure and a general licensing update (including Azure)</span></span>
- [<span data-ttu-id="dc695-184">8月 SQL 資料庫保留容量 & 實例大小彈性-授權網路研討會</span><span class="sxs-lookup"><span data-stu-id="dc695-184">August SQL DB Reserved Capacity & Instance Size Flexibility - Licensing Webinar</span></span>](https://commercial-licensing.eventbuilder.com/view?eventid=d0t9g4)
- [<span data-ttu-id="dc695-185">CSP 2018 年7月的伺服器訂閱網路研討會</span><span class="sxs-lookup"><span data-stu-id="dc695-185">July 2018 Server Subscriptions in CSP Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Server_Subscriptions_in_CSP_P2_July)
- [<span data-ttu-id="dc695-186">5月 2018 Azure 保留總覽網路研討會</span><span class="sxs-lookup"><span data-stu-id="dc695-186">May 2018 Azure Reservations Overview Webinar</span></span>](https://commercial-licensing.eventbuilder.com/Reserved_Instances_in_CSP_May_Option_1)
- [<span data-ttu-id="dc695-187">合作夥伴大學上的 Azure 授權模組</span><span class="sxs-lookup"><span data-stu-id="dc695-187">Azure Licensing Module on Partner University</span></span>](https://aka.ms/azure_partner_licensing)

### <a name="operations"></a><span data-ttu-id="dc695-188">操作</span><span class="sxs-lookup"><span data-stu-id="dc695-188">Operations</span></span>

- <span data-ttu-id="dc695-189">[現代化商務營運指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)（更新）：涵蓋主要原則和作業層面（例如合約、透過合作夥伴中心排序、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和）的完整指南Azure 合作夥伴共用服務。</span><span class="sxs-lookup"><span data-stu-id="dc695-189">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="dc695-190">新式優惠國家/地區可用性和客戶貨幣矩陣</span><span class="sxs-lookup"><span data-stu-id="dc695-190">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="dc695-191">銷售 Microsoft Azure 保留實例</span><span class="sxs-lookup"><span data-stu-id="dc695-191">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="dc695-192">代表您的客戶購買 Microsoft Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="dc695-192">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="dc695-193">代表您的客戶管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="dc695-193">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="dc695-194">Azure 保留專案的計費</span><span class="sxs-lookup"><span data-stu-id="dc695-194">Billing for Azure reservations</span></span>](https://go.microsoft.com/fwlink/?linkid=872809)
- [<span data-ttu-id="dc695-195">調整 VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="dc695-195">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="dc695-196">合作夥伴中心 API （API/SDK）</span><span class="sxs-lookup"><span data-stu-id="dc695-196">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="dc695-197">遠端桌面服務</span><span class="sxs-lookup"><span data-stu-id="dc695-197">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="dc695-198">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="dc695-198">Azure Hybrid Benefit</span></span>

<span data-ttu-id="dc695-199">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) 可協助您從您的 Windows Server 授權獲得更多價值，並可節省高達 \*47% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="dc695-199">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="dc695-200">您可以與軟體保證所涵蓋的 Windows Server Datacenter 和 Standard 版本資料中心授權搭配使用權益。</span><span class="sxs-lookup"><span data-stu-id="dc695-200">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="dc695-201">根據版本，您可以轉換或重複使用在 Azure 中執行 Windows Server 虛擬機器的授權，並支付較低的基底運算費率 (Linux 虛擬機器費率)。</span><span class="sxs-lookup"><span data-stu-id="dc695-201">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="dc695-202">請參閱 [Azure Hybrid Benefit 常見問題集](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="dc695-202">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="dc695-203">\* 實際的節省金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="dc695-203">\*Actual savings may vary based on region, instance type, or usage.</span></span>
