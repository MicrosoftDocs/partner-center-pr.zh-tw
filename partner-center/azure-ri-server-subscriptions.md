---
title: '& server 訂用帳戶的 Azure 保留專案'
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入瞭解雲端解決方案提供者的機會，以取得、布建及管理客戶的 Azure 保留和伺服器訂閱。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 408f0e59bb1d6da7caebdcf323ebcd242c49af97
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943945"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="82340-103">取得、布建、& 管理適用于客戶的 Azure 保留的 VM 實例（RI） + 伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="82340-104">適用於︰</span><span class="sxs-lookup"><span data-stu-id="82340-104">Applies to:</span></span>

- <span data-ttu-id="82340-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="82340-105">Partner Center</span></span>

<span data-ttu-id="82340-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="82340-106">**Appropriate roles**</span></span>

- <span data-ttu-id="82340-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="82340-107">Admin agent</span></span>
- <span data-ttu-id="82340-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="82340-108">Global admin</span></span>
- <span data-ttu-id="82340-109">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="82340-109">Helpdesk agent</span></span>
- <span data-ttu-id="82340-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="82340-110">Sales agent</span></span>
- <span data-ttu-id="82340-111">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="82340-111">User management admin</span></span>
 
## <a name="what-are-azure-reservations"></a><span data-ttu-id="82340-112">什麼是 Azure 保留項目？</span><span class="sxs-lookup"><span data-stu-id="82340-112">What are Azure Reservations?</span></span>

<span data-ttu-id="82340-113">Azure 保留可協助您透過預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="82340-113">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="82340-114">預先支付費用可讓您在所使用的資源上取得折扣。</span><span class="sxs-lookup"><span data-stu-id="82340-114">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="82340-115">相較于隨用隨付價格，保留可以大幅降低您的虛擬機器、SQL database 計算、Azure Cosmos DB 和其他資源成本，最高可達72%。</span><span class="sxs-lookup"><span data-stu-id="82340-115">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="82340-116">保留會提供計費折扣，且不會影響資源的執行階段狀態。</span><span class="sxs-lookup"><span data-stu-id="82340-116">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="82340-117">如需詳細資訊，請參閱[什麼是 Azure 保留專案？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="82340-117">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="82340-118">為什麼客戶要購買保留？</span><span class="sxs-lookup"><span data-stu-id="82340-118">Why should customers buy a reservation?</span></span>

<span data-ttu-id="82340-119">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留會使其成為最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="82340-119">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="82340-120">例如，如果客戶連續執行服務的四個實例，而沒有保留，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="82340-120">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="82340-121">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="82340-121">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="82340-122">那些資源將不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="82340-122">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="82340-123">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="82340-123">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="82340-124">Microsoft 藉由將 Azure 保留和伺服器訂用帳戶帶入其 CSP 計畫，讓其合作夥伴能夠解決快速成長的客戶需求，以提供更符合成本效益的解決方案，以支援高度可預測且持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="82340-124">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="82340-125">CSP 計畫可讓合作夥伴透過 Microsoft 合作夥伴中心和 Azure 入口網站，代表商業客戶取得、布建及管理 Azure 保留專案和伺服器訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="82340-125">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="82340-126">我們甚至會在我們的 CSP 方案中，為合作夥伴提供如何購買 Azure 保留的相關選擇。</span><span class="sxs-lookup"><span data-stu-id="82340-126">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="82340-127">CSP 合作夥伴可以[代表客戶購買 Azure 保留](azure-reservations-buying.md)，或可讓客戶從合作夥伴購買的先前 azure 訂用帳戶[購買自己的保留](give-customers-permission.md)。</span><span class="sxs-lookup"><span data-stu-id="82340-127">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="82340-128">Azure 保留可為客戶提供各種運算解決方案的虛擬化彈性，包括開發和測試、執行應用程式以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="82340-128">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="82340-129">例如，透過[Azure 保留的 VM 執行個體](https://azure.microsoft.com/pricing/reserved-vm-instances/)，商業客戶現在只要購買或「保留」，即可省下高達72% 的「隨用隨付」 Azure VM 定價（1或3年期的虛擬機器）。</span><span class="sxs-lookup"><span data-stu-id="82340-129">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="82340-130">具備 Azure Hybrid Benefit (隨附於軟體保證) 的 Windows Server 客戶，相較於隨付隨用定價方式，則可節省高達 80%。</span><span class="sxs-lookup"><span data-stu-id="82340-130">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="82340-131">透過無與倫比的定價和無與倫比的部署彈性組合，客戶在選擇 Azure 保留時，將會看到最佳的整體價值：</span><span class="sxs-lookup"><span data-stu-id="82340-131">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="82340-132">Azure 保留</span><span class="sxs-lookup"><span data-stu-id="82340-132">Azure reservations</span></span>

- <span data-ttu-id="82340-133">Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="82340-133">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="82340-134">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="82340-134">SQL DB Reservations</span></span>
- <span data-ttu-id="82340-135">SQL 受控執行個體</span><span class="sxs-lookup"><span data-stu-id="82340-135">SQL Managed Instance</span></span>
- <span data-ttu-id="82340-136">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="82340-136">Azure Cosmos DB</span></span>
- <span data-ttu-id="82340-137">Azure SQL 資料倉儲</span><span class="sxs-lookup"><span data-stu-id="82340-137">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="82340-138">應用程式服務</span><span class="sxs-lookup"><span data-stu-id="82340-138">App Services</span></span>
- <span data-ttu-id="82340-139">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="82340-139">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="82340-140">受控磁碟</span><span class="sxs-lookup"><span data-stu-id="82340-140">Managed Disk</span></span>
- <span data-ttu-id="82340-141">區塊 Blob</span><span class="sxs-lookup"><span data-stu-id="82340-141">Block blob</span></span>
- <span data-ttu-id="82340-142">MySQL</span><span class="sxs-lookup"><span data-stu-id="82340-142">MySQL</span></span>
- <span data-ttu-id="82340-143">Azure 資料 explorer</span><span class="sxs-lookup"><span data-stu-id="82340-143">Azure Data explorer</span></span>
- <span data-ttu-id="82340-144">MariaDB</span><span class="sxs-lookup"><span data-stu-id="82340-144">MariaDB</span></span>
- <span data-ttu-id="82340-145">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="82340-145">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="82340-146">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-146">Server subscriptions</span></span>

- <span data-ttu-id="82340-147">Windows Server</span><span class="sxs-lookup"><span data-stu-id="82340-147">Windows Server</span></span>
- <span data-ttu-id="82340-148">遠端桌面服務（RDS） Cal</span><span class="sxs-lookup"><span data-stu-id="82340-148">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="82340-149">SQL Server</span><span class="sxs-lookup"><span data-stu-id="82340-149">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="82340-150">Linux ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-150">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="82340-151">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="82340-151">SUSE Linux</span></span>
- <span data-ttu-id="82340-152">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="82340-152">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="82340-153">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="82340-153">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="82340-154">ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-154">ISV annual subscriptions</span></span>

- <span data-ttu-id="82340-155">由 CloudSimple 提供的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="82340-155">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="82340-156">開始使用</span><span class="sxs-lookup"><span data-stu-id="82340-156">Getting started</span></span>

<span data-ttu-id="82340-157">若要瞭解如何將 Azure 保留與您的客戶進行定位，並儘快啟動並執行操作，我們建議您採用下列方法來審查準備就緒資料：</span><span class="sxs-lookup"><span data-stu-id="82340-157">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="82340-158">檢閱《概觀簡報》及相關客戶價值主張與定位的網路研討會</span><span class="sxs-lookup"><span data-stu-id="82340-158">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="82340-159">檢視並了解《現代商務營運指南》(Modern Commerce Operating Guide)</span><span class="sxs-lookup"><span data-stu-id="82340-159">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="82340-160">檢視 Azure RI 和伺服器訂閱常見問題</span><span class="sxs-lookup"><span data-stu-id="82340-160">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="82340-161">了解[合作夥伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure Reservations 和伺服器訂閱更新</span><span class="sxs-lookup"><span data-stu-id="82340-161">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="82340-162">資源</span><span class="sxs-lookup"><span data-stu-id="82340-162">Resources</span></span>

<span data-ttu-id="82340-163">以下提供完整的資源清單，可協助您快速上線以在合作夥伴中心交易 Azure Reservations：</span><span class="sxs-lookup"><span data-stu-id="82340-163">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="82340-164">銷售就緒</span><span class="sxs-lookup"><span data-stu-id="82340-164">Sales readiness</span></span>

- [<span data-ttu-id="82340-165">具有 Azure Hybrid Benefit 總覽的 Azure 保留和伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-165">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="82340-166">銷售資料表</span><span class="sxs-lookup"><span data-stu-id="82340-166">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="82340-167">Azure 保留的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="82340-167">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="82340-168">Azure 保留和 SQL DB 的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="82340-168">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="82340-169">遠端桌面服務（RDS）用戶端存取許可證（CAL）（公告）</span><span class="sxs-lookup"><span data-stu-id="82340-169">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="82340-170">Azure 保留的 VM 執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="82340-170">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="82340-171">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="82340-171">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="82340-172">Azure 中的 SQL DB 總覽</span><span class="sxs-lookup"><span data-stu-id="82340-172">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="82340-173">SQL DB 保留（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="82340-173">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="82340-174">Azure Cosmos DB （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="82340-174">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="82340-175">SQL 受控執行個體（Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="82340-175">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="82340-176">SUSE 和 Red Hat Enterprise Linux （Azure 入口網站）</span><span class="sxs-lookup"><span data-stu-id="82340-176">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="82340-177">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="82340-177">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="82340-178">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="82340-178">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="82340-179">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="82340-179">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="82340-180">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="82340-180">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="82340-181">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="82340-181">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="82340-182">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="82340-182">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="82340-183">CSP 價目表： **Microsoft Azure 保留實例**和**軟體**訂用帳戶價格清單都位於合作夥伴中心[定價 &](https://partner.microsoft.com/pcv/sales)供應專案] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="82340-183">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="82340-184">訓練</span><span class="sxs-lookup"><span data-stu-id="82340-184">Training</span></span>

<span data-ttu-id="82340-185">註冊以觀看[商業授權就緒網路研討會](https://commercial-licensing.eventbuilder.com/FY2019_ALL)和隨選活動。</span><span class="sxs-lookup"><span data-stu-id="82340-185">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="82340-186">授權的隨選準備事件包括如下的主題：</span><span class="sxs-lookup"><span data-stu-id="82340-186">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="82340-187">CSP 線上服務、CSP Azure 和一般授權更新，包括 Azure （2018年11月）</span><span class="sxs-lookup"><span data-stu-id="82340-187">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="82340-188">SQL DB 保留容量 & 實例大小彈性（2018年8月）</span><span class="sxs-lookup"><span data-stu-id="82340-188">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="82340-189">CSP 中的伺服器訂閱（2018年7月）</span><span class="sxs-lookup"><span data-stu-id="82340-189">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="82340-190">CSP 中的 Azure 保留總覽（5月2018）</span><span class="sxs-lookup"><span data-stu-id="82340-190">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="82340-191">其他實用的訓練課程包含[合作夥伴大學的 Azure 授權模組](https://aka.ms/azure_partner_licensing)。</span><span class="sxs-lookup"><span data-stu-id="82340-191">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="82340-192">作業</span><span class="sxs-lookup"><span data-stu-id="82340-192">Operations</span></span>

- <span data-ttu-id="82340-193">[現代化商務營運指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx)（更新）：涵蓋主要原則和操作層面的完整指南，例如合約、透過合作夥伴中心訂購、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和 Azure 合作夥伴共用服務。</span><span class="sxs-lookup"><span data-stu-id="82340-193">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="82340-194">現代化優惠國家/地區可用性和客戶貨幣矩陣</span><span class="sxs-lookup"><span data-stu-id="82340-194">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="82340-195">銷售 Microsoft Azure 保留的執行個體</span><span class="sxs-lookup"><span data-stu-id="82340-195">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="82340-196">代表您的客戶購買 Microsoft Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="82340-196">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="82340-197">代表您的客戶管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="82340-197">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="82340-198">Azure Reservations 的帳單</span><span class="sxs-lookup"><span data-stu-id="82340-198">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="82340-199">調整 VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="82340-199">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="82340-200">合作夥伴中心 API （API/SDK）</span><span class="sxs-lookup"><span data-stu-id="82340-200">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="82340-201">遠端桌面服務</span><span class="sxs-lookup"><span data-stu-id="82340-201">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="82340-202">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="82340-202">Azure Hybrid Benefit</span></span>

<span data-ttu-id="82340-203">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) 可協助您從您的 Windows Server 授權獲得更多價值，並可節省高達 \*47% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="82340-203">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="82340-204">您可以將權益搭配用於軟體保證所涵蓋的 Windows Server Datacenter 和 Standard Edition 授權。</span><span class="sxs-lookup"><span data-stu-id="82340-204">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="82340-205">視版本而定，您可以轉換或重複使用您的授權，在 Azure 中執行 Windows Server 虛擬機器，並以較低的基礎計算費率支付（Linux 虛擬機器費率）。</span><span class="sxs-lookup"><span data-stu-id="82340-205">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="82340-206">請參閱 [Azure Hybrid Benefit 常見問題集](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="82340-206">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="82340-207">\* 實際的節省金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="82340-207">\*Actual savings may vary based on region, instance type, or usage.</span></span>
