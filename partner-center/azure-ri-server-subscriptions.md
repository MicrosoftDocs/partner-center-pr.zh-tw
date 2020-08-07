---
title: '& server 訂用帳戶的 Azure 保留專案'
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入瞭解雲端解決方案提供者的機會，以取得、布建及管理客戶的 Azure 保留和伺服器訂閱。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b8a9cf07f8dace47346c68ade3707d6b12a1532
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900088"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="323c8-103">取得、布建、& 管理適用于客戶的 Azure 保留的 VM 實例 (RI) + 伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="323c8-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="323c8-104">Applies to:</span></span>

- <span data-ttu-id="323c8-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="323c8-105">Partner Center</span></span>

<span data-ttu-id="323c8-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="323c8-106">**Appropriate roles**</span></span>

- <span data-ttu-id="323c8-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="323c8-107">Admin agent</span></span>
- <span data-ttu-id="323c8-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="323c8-108">Global admin</span></span>
- <span data-ttu-id="323c8-109">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="323c8-109">Helpdesk agent</span></span>
- <span data-ttu-id="323c8-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="323c8-110">Sales agent</span></span>
- <span data-ttu-id="323c8-111">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="323c8-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="323c8-112">本文僅適用于雲端解決方案提供者 (CSP) 方案中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="323c8-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="323c8-113">使用其他類型之訂用帳戶的客戶 (例如，隨用隨付、個人、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀[此 Azure 保留檔](https://docs.microsoft.com/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="323c8-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="323c8-114">什麼是 Azure 保留項目？</span><span class="sxs-lookup"><span data-stu-id="323c8-114">What are Azure Reservations?</span></span>

<span data-ttu-id="323c8-115">Azure 保留可協助您透過預先支付一年或三年的虛擬機器、SQL Database 計算容量、Azure Cosmos DB 輸送量或其他 Azure 資源來節省成本。</span><span class="sxs-lookup"><span data-stu-id="323c8-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="323c8-116">預先支付費用可讓您在所使用的資源上取得折扣。</span><span class="sxs-lookup"><span data-stu-id="323c8-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="323c8-117">相較于隨用隨付價格，保留可以大幅降低您的虛擬機器、SQL database 計算、Azure Cosmos DB 和其他資源成本，最高可達72%。</span><span class="sxs-lookup"><span data-stu-id="323c8-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="323c8-118">保留會提供計費折扣，且不會影響資源的執行階段狀態。</span><span class="sxs-lookup"><span data-stu-id="323c8-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="323c8-119">如需詳細資訊，請參閱[什麼是 Azure 保留專案？](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="323c8-119">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="323c8-120">為什麼客戶要購買保留？</span><span class="sxs-lookup"><span data-stu-id="323c8-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="323c8-121">如果客戶有很長一段時間執行的虛擬機器、Azure Cosmos DB 或 SQL 資料庫，則購買保留會使其成為最符合成本效益的選項。</span><span class="sxs-lookup"><span data-stu-id="323c8-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="323c8-122">例如，如果客戶連續執行服務的四個實例，而沒有保留，則會以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="323c8-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="323c8-123">如果他們為這些資源購買保留，則會立即取得保留折扣。</span><span class="sxs-lookup"><span data-stu-id="323c8-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="323c8-124">那些資源將不再以隨用隨付費率計費。</span><span class="sxs-lookup"><span data-stu-id="323c8-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="323c8-125">雲端解決方案提供者中嶄新的 Azure 供應項目</span><span class="sxs-lookup"><span data-stu-id="323c8-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="323c8-126">Microsoft 藉由將 Azure 保留和伺服器訂用帳戶帶入其 CSP 計畫，讓其合作夥伴能夠解決快速成長的客戶需求，以提供更符合成本效益的解決方案，以支援高度可預測且持續的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="323c8-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="323c8-127">CSP 計畫可讓合作夥伴透過 Microsoft 合作夥伴中心和 Azure 入口網站，代表商業客戶取得、布建及管理 Azure 保留專案和伺服器訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="323c8-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="323c8-128">我們甚至會在我們的 CSP 方案中，為合作夥伴提供如何購買 Azure 保留的相關選擇。</span><span class="sxs-lookup"><span data-stu-id="323c8-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="323c8-129">CSP 合作夥伴可以[代表客戶購買 Azure 保留](azure-reservations-buying.md)，或可讓客戶從合作夥伴購買的先前 azure 訂用帳戶[購買自己的保留](give-customers-permission.md)。</span><span class="sxs-lookup"><span data-stu-id="323c8-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="323c8-130">Azure 保留可為客戶提供各種運算解決方案的虛擬化彈性，包括開發和測試、執行應用程式以及擴充資料中心。</span><span class="sxs-lookup"><span data-stu-id="323c8-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="323c8-131">例如，透過[Azure 保留的 VM 執行個體](https://azure.microsoft.com/pricing/reserved-vm-instances/)，商業客戶現在只要購買或「保留」，即可省下高達72% 的「隨用隨付」 Azure VM 定價（1或3年期的虛擬機器）。</span><span class="sxs-lookup"><span data-stu-id="323c8-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="323c8-132">具備 Azure Hybrid Benefit (隨附於軟體保證) 的 Windows Server 客戶，相較於隨付隨用定價方式，則可節省高達 80%。</span><span class="sxs-lookup"><span data-stu-id="323c8-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="323c8-133">透過無與倫比的定價和無與倫比的部署彈性組合，客戶在選擇 Azure 保留時，將會看到最佳的整體價值：</span><span class="sxs-lookup"><span data-stu-id="323c8-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="323c8-134">Azure 保留</span><span class="sxs-lookup"><span data-stu-id="323c8-134">Azure reservations</span></span>

- <span data-ttu-id="323c8-135">Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="323c8-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="323c8-136">SQL DB 保留</span><span class="sxs-lookup"><span data-stu-id="323c8-136">SQL DB Reservations</span></span>
- <span data-ttu-id="323c8-137">SQL 受控執行個體</span><span class="sxs-lookup"><span data-stu-id="323c8-137">SQL Managed Instance</span></span>
- <span data-ttu-id="323c8-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="323c8-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="323c8-139">Azure SQL 資料倉儲</span><span class="sxs-lookup"><span data-stu-id="323c8-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="323c8-140">應用程式服務</span><span class="sxs-lookup"><span data-stu-id="323c8-140">App Services</span></span>
- <span data-ttu-id="323c8-141">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="323c8-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="323c8-142">受控磁碟</span><span class="sxs-lookup"><span data-stu-id="323c8-142">Managed Disk</span></span>
- <span data-ttu-id="323c8-143">區塊 Blob</span><span class="sxs-lookup"><span data-stu-id="323c8-143">Block blob</span></span>
- <span data-ttu-id="323c8-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="323c8-144">MySQL</span></span>
- <span data-ttu-id="323c8-145">Azure 資料 explorer</span><span class="sxs-lookup"><span data-stu-id="323c8-145">Azure Data explorer</span></span>
- <span data-ttu-id="323c8-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="323c8-146">MariaDB</span></span>
- <span data-ttu-id="323c8-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="323c8-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="323c8-148">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-148">Server subscriptions</span></span>

- <span data-ttu-id="323c8-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="323c8-149">Windows Server</span></span>
- <span data-ttu-id="323c8-150">遠端桌面服務 (RDS) Cal</span><span class="sxs-lookup"><span data-stu-id="323c8-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="323c8-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="323c8-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="323c8-152">Linux ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="323c8-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="323c8-153">SUSE Linux</span></span>
- <span data-ttu-id="323c8-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="323c8-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="323c8-155">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="323c8-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="323c8-156">ISV 年度訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="323c8-157">由 CloudSimple 提供的 Azure VMware 解決方案</span><span class="sxs-lookup"><span data-stu-id="323c8-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="323c8-158">開始使用</span><span class="sxs-lookup"><span data-stu-id="323c8-158">Getting started</span></span>

<span data-ttu-id="323c8-159">若要瞭解如何將 Azure 保留與您的客戶進行定位，並儘快啟動並執行操作，我們建議您採用下列方法來審查準備就緒資料：</span><span class="sxs-lookup"><span data-stu-id="323c8-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="323c8-160">檢閱《概觀簡報》及相關客戶價值主張與定位的網路研討會</span><span class="sxs-lookup"><span data-stu-id="323c8-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="323c8-161">檢視並了解《現代商務營運指南》(Modern Commerce Operating Guide)</span><span class="sxs-lookup"><span data-stu-id="323c8-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="323c8-162">檢視 Azure RI 和伺服器訂閱常見問題</span><span class="sxs-lookup"><span data-stu-id="323c8-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="323c8-163">了解[合作夥伴中心 API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances) 中的 Azure Reservations 和伺服器訂閱更新</span><span class="sxs-lookup"><span data-stu-id="323c8-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="323c8-164">資源</span><span class="sxs-lookup"><span data-stu-id="323c8-164">Resources</span></span>

<span data-ttu-id="323c8-165">以下提供完整的資源清單，可協助您快速上線以在合作夥伴中心交易 Azure Reservations：</span><span class="sxs-lookup"><span data-stu-id="323c8-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="323c8-166">銷售就緒</span><span class="sxs-lookup"><span data-stu-id="323c8-166">Sales readiness</span></span>

- [<span data-ttu-id="323c8-167">具有 Azure Hybrid Benefit 總覽的 Azure 保留和伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="323c8-168">銷售資料表</span><span class="sxs-lookup"><span data-stu-id="323c8-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="323c8-169">Azure 保留的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="323c8-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="323c8-170">Azure 保留和 SQL DB 的合作夥伴常見問題</span><span class="sxs-lookup"><span data-stu-id="323c8-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="323c8-171">遠端桌面服務 (RDS) 用戶端存取許可證 (CAL)  (公告) </span><span class="sxs-lookup"><span data-stu-id="323c8-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="323c8-172">Azure 保留的 VM 執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="323c8-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="323c8-173">伺服器訂閱</span><span class="sxs-lookup"><span data-stu-id="323c8-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="323c8-174">Azure 中的 SQL DB 總覽</span><span class="sxs-lookup"><span data-stu-id="323c8-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="323c8-175">Azure 入口網站) 的 SQL DB 保留 (</span><span class="sxs-lookup"><span data-stu-id="323c8-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="323c8-176">Azure Cosmos DB (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="323c8-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="323c8-177">SQL 受控執行個體 (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="323c8-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="323c8-178">SUSE 和 Red Hat Enterprise Linux (Azure 入口網站) </span><span class="sxs-lookup"><span data-stu-id="323c8-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="323c8-179">Azure 上的 Red Hat Linux</span><span class="sxs-lookup"><span data-stu-id="323c8-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="323c8-180">Azure 上的 SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="323c8-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="323c8-181">Azure 上的 Linux</span><span class="sxs-lookup"><span data-stu-id="323c8-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="323c8-182">Azure 定價概觀</span><span class="sxs-lookup"><span data-stu-id="323c8-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="323c8-183">Azure 定價計算機</span><span class="sxs-lookup"><span data-stu-id="323c8-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="323c8-184">Azure Databricks 單位保留</span><span class="sxs-lookup"><span data-stu-id="323c8-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="323c8-185">CSP 價目表： **Microsoft Azure 保留實例**和**軟體**訂用帳戶價格清單都位於合作夥伴中心[定價 &](https://partner.microsoft.com/pcv/sales)供應專案] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="323c8-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="323c8-186">訓練</span><span class="sxs-lookup"><span data-stu-id="323c8-186">Training</span></span>

<span data-ttu-id="323c8-187">註冊以觀看[商業授權就緒網路研討會](https://commercial-licensing.eventbuilder.com/FY2019_ALL)和隨選活動。</span><span class="sxs-lookup"><span data-stu-id="323c8-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="323c8-188">授權的隨選準備事件包括如下的主題：</span><span class="sxs-lookup"><span data-stu-id="323c8-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="323c8-189">CSP 線上服務、CSP Azure 和一般授權更新（包括 Azure (2018 年11月）) </span><span class="sxs-lookup"><span data-stu-id="323c8-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="323c8-190">SQL DB 保留容量 & 實例大小彈性 (2018 年8月) </span><span class="sxs-lookup"><span data-stu-id="323c8-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="323c8-191">CSP 中的伺服器訂閱 (2018 年7月) </span><span class="sxs-lookup"><span data-stu-id="323c8-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="323c8-192">CSP 中的 Azure 保留總覽 (5 月 2018) </span><span class="sxs-lookup"><span data-stu-id="323c8-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="323c8-193">其他實用的訓練課程包含[合作夥伴大學的 Azure 授權模組](https://aka.ms/azure_partner_licensing)。</span><span class="sxs-lookup"><span data-stu-id="323c8-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="323c8-194">作業</span><span class="sxs-lookup"><span data-stu-id="323c8-194">Operations</span></span>

- <span data-ttu-id="323c8-195">[新式商務操作指南](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (更新) ：涵蓋主要原則和作業層面（例如合約、透過合作夥伴中心排序、發票、價目表詳細資料、獎勵、對帳檔案、API/SDK、沙箱和 Azure 合作夥伴共用服務）的完整指南。</span><span class="sxs-lookup"><span data-stu-id="323c8-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="323c8-196">現代化優惠國家/地區可用性和客戶貨幣矩陣</span><span class="sxs-lookup"><span data-stu-id="323c8-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="323c8-197">銷售 Microsoft Azure 保留的執行個體</span><span class="sxs-lookup"><span data-stu-id="323c8-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="323c8-198">代表您的客戶購買 Microsoft Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="323c8-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="323c8-199">代表您的客戶管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="323c8-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="323c8-200">Azure Reservations 的帳單</span><span class="sxs-lookup"><span data-stu-id="323c8-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="323c8-201">調整 VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="323c8-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="323c8-202">合作夥伴中心 API (API/SDK) </span><span class="sxs-lookup"><span data-stu-id="323c8-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="323c8-203">遠端桌面服務</span><span class="sxs-lookup"><span data-stu-id="323c8-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="323c8-204">Azure Hybrid Benefit</span><span class="sxs-lookup"><span data-stu-id="323c8-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="323c8-205">[Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) 可協助您從您的 Windows Server 授權獲得更多價值，並可節省高達 \*47% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="323c8-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="323c8-206">您可以將權益搭配用於軟體保證所涵蓋的 Windows Server Datacenter 和 Standard Edition 授權。</span><span class="sxs-lookup"><span data-stu-id="323c8-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="323c8-207">視版本而定，您可以轉換或重複使用您的授權，在 Azure 中執行 Windows Server 虛擬機器，並以較低的基礎計算費率支付 (Linux 虛擬機器費率) 。</span><span class="sxs-lookup"><span data-stu-id="323c8-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="323c8-208">請參閱 [Azure Hybrid Benefit 常見問題集](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="323c8-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="323c8-209">\* 實際的節省金額可能會根據區域、實例類型或使用方式而有所不同。</span><span class="sxs-lookup"><span data-stu-id="323c8-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
