---
title: Azure 保留與伺服器訂閱 |合作夥伴中心
ms.topic: article
ms.date: 04/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解雲端解決方案提供者如何取得、布建及管理其客戶的 Azure 保留和伺服器訂閱。
author: LauraBrenner
ms.author: labrenne
keywords: Azure，訂用帳戶，VM，保留，保留實例
ms.localizationpriority: medium
ms.openlocfilehash: d0a3fde651db86f8aeed160764fc330a25c0df04
ms.sourcegitcommit: ee7f8600f566799838bda64e26c54799137f2cd5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/11/2020
ms.locfileid: "81123272"
---
<!-- Mike Aasen wrote and owns this topic -->

# <a name="azure-reserved-vm-instances-ri--server-subscriptions-for-azure"></a><span data-ttu-id="eb6fc-104">Azure 保留的 VM 執行個體 (RI) + Azure 伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-104">Azure reserved VM instances (RI) + server subscriptions for Azure</span></span>

<span data-ttu-id="eb6fc-105">適用於：</span><span class="sxs-lookup"><span data-stu-id="eb6fc-105">Applies to:</span></span>

- <span data-ttu-id="eb6fc-106">夥伴中心</span><span class="sxs-lookup"><span data-stu-id="eb6fc-106">Partner Center</span></span>

<span data-ttu-id="eb6fc-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="eb6fc-107">**Appropriate roles**</span></span>

- <span data-ttu-id="eb6fc-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="eb6fc-108">Admin agent</span></span>
- <span data-ttu-id="eb6fc-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="eb6fc-109">Global admin</span></span>
- <span data-ttu-id="eb6fc-110">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="eb6fc-110">Helpdesk agent</span></span>
- <span data-ttu-id="eb6fc-111">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="eb6fc-111">Sales agent</span></span>
- <span data-ttu-id="eb6fc-112">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="eb6fc-112">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="eb6fc-113">什麼是 Azure 保留專案？</span><span class="sxs-lookup"><span data-stu-id="eb6fc-113">What are Azure Reservations?</span></span>

<span data-ttu-id="eb6fc-114">Azure 保留可協助您透過預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-114">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="eb6fc-115">預先付款可讓您獲得所用資源的折扣。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-115">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="eb6fc-116">相較於隨付隨用價格，保留區可將虛擬機器、SQL Database 計算、Azure Cosmos DB 和其他資源的成本大幅降低至最多 72%。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-116">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="eb6fc-117">保留會提供計費折扣，且不會影響資源的執行時間狀態。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-117">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="eb6fc-118">如需詳細資訊，請參閱[什麼是 Azure 保留專案？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="eb6fc-118">For more information, see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="eb6fc-119">為什麼客戶要購買保留？</span><span class="sxs-lookup"><span data-stu-id="eb6fc-119">Why should customers buy a reservation?</span></span>

<span data-ttu-id="eb6fc-120">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留會使其成為最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-120">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="eb6fc-121">例如，如果客戶連續執行服務的四個實例，而沒有保留，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-121">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="eb6fc-122">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-122">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="eb6fc-123">資源不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-123">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="eb6fc-124">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="eb6fc-124">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="eb6fc-125">藉由將 Azure 保留和伺服器訂用帳戶帶入其 CSP 計畫，Microsoft 可讓合作夥伴更有效地解決快速成長的客戶需求。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-125">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft allows partners to better address fast-growing customer demand.</span></span> <span data-ttu-id="eb6fc-126">這包括增加客戶需求，以提供更符合成本效益的解決方案，以支援高度可預測且持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-126">This includes increased customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="eb6fc-127">CSP 計畫可讓合作夥伴代表商業客戶取得、布建及管理 Azure 保留和伺服器訂閱。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-127">The CSP program enables partners to acquire, provision, and manage Azure Reservations and Server Subscriptions on behalf of commercial customers.</span></span> <span data-ttu-id="eb6fc-128">合作夥伴可以透過 Microsoft 合作夥伴中心和 Azure 入口網站來執行這些工作。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-128">Partners can perform these tasks via Microsoft Partner Center and the Azure portal.</span></span>

<span data-ttu-id="eb6fc-129">Azure 保留可為客戶提供各種計算解決方案的虛擬化彈性。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-129">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions.</span></span> <span data-ttu-id="eb6fc-130">這類解決方案可以包括開發和測試、執行應用程式，以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-130">Such solutions can include development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="eb6fc-131">例如，透過 Azure 保留的 VM 執行個體，商業客戶現在只要購買或「保留」-一年或三年期的虛擬機器，即可省下高達72% 的隨用隨付 Azure VM 定價。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-131">With Azure Reserved VM Instances, for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="eb6fc-132">包含軟體保證之 Azure Hybrid Benefit 的 Windows Server 客戶可以省下高達80% 與隨用隨付定價的費用。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, can save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="eb6fc-133">透過無與倫比的定價和無與倫比的部署彈性組合，客戶在選擇 Azure 保留時，將會看到最佳的整體價值：</span><span class="sxs-lookup"><span data-stu-id="eb6fc-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="eb6fc-134">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="eb6fc-134">Azure reservations</span></span>

- <span data-ttu-id="eb6fc-135">Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="eb6fc-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="eb6fc-136">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="eb6fc-136">SQL DB Reservations</span></span>
- <span data-ttu-id="eb6fc-137">SQL 受控執行個體</span><span class="sxs-lookup"><span data-stu-id="eb6fc-137">SQL Managed Instance</span></span>
- <span data-ttu-id="eb6fc-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="eb6fc-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="eb6fc-139">Azure SQL 資料倉儲</span><span class="sxs-lookup"><span data-stu-id="eb6fc-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="eb6fc-140">應用程式服務</span><span class="sxs-lookup"><span data-stu-id="eb6fc-140">App Services</span></span>
- <span data-ttu-id="eb6fc-141">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="eb6fc-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="eb6fc-142">受控磁片</span><span class="sxs-lookup"><span data-stu-id="eb6fc-142">Managed Disk</span></span>
- <span data-ttu-id="eb6fc-143">Blockblob</span><span class="sxs-lookup"><span data-stu-id="eb6fc-143">Blockblob</span></span>
- <span data-ttu-id="eb6fc-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="eb6fc-144">MySQL</span></span>
- <span data-ttu-id="eb6fc-145">Azure 資料 explorer</span><span class="sxs-lookup"><span data-stu-id="eb6fc-145">Azure Data explorer</span></span>
- <span data-ttu-id="eb6fc-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="eb6fc-146">MariaDB</span></span>
- <span data-ttu-id="eb6fc-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="eb6fc-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="eb6fc-148">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-148">Server subscriptions</span></span>

- <span data-ttu-id="eb6fc-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="eb6fc-149">Windows Server</span></span>
- <span data-ttu-id="eb6fc-150">遠端桌面服務（RDS） Cal</span><span class="sxs-lookup"><span data-stu-id="eb6fc-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="eb6fc-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="eb6fc-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="eb6fc-152">Linux ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="eb6fc-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="eb6fc-153">SUSE Linux</span></span>
- <span data-ttu-id="eb6fc-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="eb6fc-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="eb6fc-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="eb6fc-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="eb6fc-156">ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="eb6fc-157">依 CloudSimple 的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="eb6fc-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="eb6fc-158">開始使用</span><span class="sxs-lookup"><span data-stu-id="eb6fc-158">Getting started</span></span>

<span data-ttu-id="eb6fc-159">若要瞭解如何將 Azure 保留與您的客戶進行定位，並儘快啟動並執行操作，我們建議您採用下列方法來審查準備就緒資料：</span><span class="sxs-lookup"><span data-stu-id="eb6fc-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="eb6fc-160">檢閱《概觀簡報》及相關客戶價值主張與定位的網路研討會</span><span class="sxs-lookup"><span data-stu-id="eb6fc-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="eb6fc-161">檢視並了解《現代商務營運指南》(Modern Commerce Operating Guide)</span><span class="sxs-lookup"><span data-stu-id="eb6fc-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="eb6fc-162">檢視 Azure RI 和伺服器訂閱常見問題</span><span class="sxs-lookup"><span data-stu-id="eb6fc-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="eb6fc-163">了解[合作夥伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure Reservations 和伺服器訂閱更新</span><span class="sxs-lookup"><span data-stu-id="eb6fc-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="eb6fc-164">資源</span><span class="sxs-lookup"><span data-stu-id="eb6fc-164">Resources</span></span>

<span data-ttu-id="eb6fc-165">以下提供完整的資源清單，可協助您快速上線以在合作夥伴中心交易 Azure Reservations：</span><span class="sxs-lookup"><span data-stu-id="eb6fc-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="eb6fc-166">銷售就緒</span><span class="sxs-lookup"><span data-stu-id="eb6fc-166">Sales readiness</span></span>

- [<span data-ttu-id="eb6fc-167">具有 Azure Hybrid Benefit 總覽的 Azure 保留和伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="eb6fc-168">銷售資料表</span><span class="sxs-lookup"><span data-stu-id="eb6fc-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="eb6fc-169">Azure 保留的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="eb6fc-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="eb6fc-170">Azure Reservations 和 SQL DB 合作夥伴常見問題集</span><span class="sxs-lookup"><span data-stu-id="eb6fc-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="eb6fc-171">遠端桌面服務（RDS） Cal （公告）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-171">Remote Desktop Services (RDS) CALs (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="eb6fc-172">Azure 保留的 VM 執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="eb6fc-173">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="eb6fc-173">Server Subscriptions</span></span>](https://docs.microsoft.com/partner-center/csp-software-subscriptions)
- [<span data-ttu-id="eb6fc-174">Azure 中的 SQL DB 總覽</span><span class="sxs-lookup"><span data-stu-id="eb6fc-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="eb6fc-175">SQL DB 保留（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="eb6fc-176">Azure Cosmos DB （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="eb6fc-177">SQL 受控執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="eb6fc-178">SUSE 和 Red Hat Enterprise Linux （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="eb6fc-179">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="eb6fc-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="eb6fc-180">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="eb6fc-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="eb6fc-181">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="eb6fc-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="eb6fc-182">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="eb6fc-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="eb6fc-183">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="eb6fc-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="eb6fc-184">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="eb6fc-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="eb6fc-185">CSP 價目表： **Microsoft Azure 保留實例**和**軟體**訂用帳戶價格清單都位於合作夥伴中心[定價 &](https://partner.microsoft.com/pcv/sales)供應專案 頁面上。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="eb6fc-186">訓練</span><span class="sxs-lookup"><span data-stu-id="eb6fc-186">Training</span></span>

<span data-ttu-id="eb6fc-187">註冊以觀看[商業授權就緒網路研討會](https://commercial-licensing.eventbuilder.com/FY2019_ALL)和隨選活動。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="eb6fc-188">授權的隨選準備事件包括如下的主題：</span><span class="sxs-lookup"><span data-stu-id="eb6fc-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="eb6fc-189">CSP 線上服務、CSP Azure 和一般授權更新，包括 Azure （2018年11月）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="eb6fc-190">SQL DB 保留容量 & 實例大小彈性（2018年8月）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="eb6fc-191">CSP 中的伺服器訂閱（2018年7月）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="eb6fc-192">CSP 中的 Azure 保留總覽（5月2018）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="eb6fc-193">其他實用的訓練課程包含[合作夥伴大學的 Azure 授權模組](https://aka.ms/azure_partner_licensing)。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="eb6fc-194">操作</span><span class="sxs-lookup"><span data-stu-id="eb6fc-194">Operations</span></span>

- <span data-ttu-id="eb6fc-195">[現代化商務營運指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)（更新）：涵蓋主要原則和操作層面的完整指南，例如合約、透過合作夥伴中心訂購、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和 Azure 合作夥伴共用服務。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="eb6fc-196">新式優惠國家/地區可用性和客戶貨幣矩陣</span><span class="sxs-lookup"><span data-stu-id="eb6fc-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="eb6fc-197">銷售 Microsoft Azure 保留實例</span><span class="sxs-lookup"><span data-stu-id="eb6fc-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="eb6fc-198">代表您的客戶購買 Microsoft Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="eb6fc-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="eb6fc-199">代表您的客戶管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="eb6fc-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="eb6fc-200">Azure 保留專案的計費</span><span class="sxs-lookup"><span data-stu-id="eb6fc-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="eb6fc-201">調整 VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="eb6fc-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="eb6fc-202">合作夥伴中心 API （API/SDK）</span><span class="sxs-lookup"><span data-stu-id="eb6fc-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- <span data-ttu-id="eb6fc-203">[Host desktops and apps in Remote Desktop Services on Azure](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds) (主機桌上型電腦和應用程式在 Azure 上的遠端桌面服務)</span><span class="sxs-lookup"><span data-stu-id="eb6fc-203">[Remote Desktop Services](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)</span></span>

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="eb6fc-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="eb6fc-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="eb6fc-205">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) 可協助您從您的 Windows Server 授權獲得更多價值，並可節省高達 \*47% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="eb6fc-206">您可以與軟體保證所涵蓋的 Windows Server Datacenter 和 Standard 版本資料中心授權搭配使用權益。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="eb6fc-207">視版本而定，您可以轉換或重複使用您的授權，在 Azure 中執行 Windows Server 虛擬機器，並以較低的基礎計算費率支付（Linux 虛擬機器費率）。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="eb6fc-208">請參閱 [Azure Hybrid Benefit 常見問題集](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="eb6fc-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="eb6fc-209">\* 實際的節省金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="eb6fc-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
