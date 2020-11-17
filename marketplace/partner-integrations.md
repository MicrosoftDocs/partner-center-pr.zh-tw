---
title: Azure Marketplace 合作夥伴整合
description: 瞭解與 Azure 環境整合 Azure Marketplace 的解決方案，並取得 Microsoft 合作夥伴提供的部署指南連結。
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691647"
---
# <a name="azure-marketplace-partner-integrations"></a><span data-ttu-id="5894d-103">Azure Marketplace 合作夥伴整合</span><span class="sxs-lookup"><span data-stu-id="5894d-103">Azure Marketplace partner integrations</span></span>

<span data-ttu-id="5894d-104">瞭解如何將合作夥伴解決方案整合到您的 Azure 環境。</span><span class="sxs-lookup"><span data-stu-id="5894d-104">Learn how to integrate partner solutions into your Azure environment.</span></span> <span data-ttu-id="5894d-105">本文提供每個解決方案的總覽，以及詳細部署指南的連結。</span><span class="sxs-lookup"><span data-stu-id="5894d-105">This article gives an overview of each solution and links to detailed deployment guides.</span></span> <span data-ttu-id="5894d-106">解決方案會依字母順序列出。</span><span class="sxs-lookup"><span data-stu-id="5894d-106">Solutions are listed in alphabetical order.</span></span> 

## <a name="apache-kafka-on-confluent-cloud"></a><span data-ttu-id="5894d-107">Confluent 雲端上的 Apache Kafka</span><span class="sxs-lookup"><span data-stu-id="5894d-107">Apache Kafka on Confluent Cloud</span></span>

![Confluent 雲端](./media/partners/confluent-cloud.png)

<span data-ttu-id="5894d-109">除了您的雲端應用程式之外，Azure 還可讓您與 Confluent Cloud 整合。</span><span class="sxs-lookup"><span data-stu-id="5894d-109">Azure lets you integrate with Confluent Cloud in addition to your cloud applications.</span></span> <span data-ttu-id="5894d-110">Confluent 客戶通常會在 Azure 入口網站與 Confluent 雲端之間流覽。</span><span class="sxs-lookup"><span data-stu-id="5894d-110">Confluent customers often navigate between the Azure portal and Confluent Cloud.</span></span> <span data-ttu-id="5894d-111">例如，使用者在 Azure Marketplace 購買 Confluent 雲端供應專案之後，他們就必須設定 Confluent Cloud 的帳戶。</span><span class="sxs-lookup"><span data-stu-id="5894d-111">For example, once a user purchases a Confluent Cloud offer in Azure Marketplace, they are then expected to set up an account with Confluent Cloud.</span></span> <span data-ttu-id="5894d-112">此程式增加了複雜性和時間，而且需要使用者管理兩個入口網站之間的設定和資源。</span><span class="sxs-lookup"><span data-stu-id="5894d-112">This process adds complexity and time, and requires users to manage configuration and resources between the two portals.</span></span> <span data-ttu-id="5894d-113">為了降低跨平臺管理的負擔，Microsoft 與 Confluent Cloud 合作，建立了從 Azure 到 Confluent Cloud 的整合布建層。</span><span class="sxs-lookup"><span data-stu-id="5894d-113">To reduce the burden of managing across platforms, Microsoft, in partnership with Confluent Cloud, built an integrated provisioning layer from Azure to Confluent Cloud.</span></span> <span data-ttu-id="5894d-114">解決方案可在 Azure Marketplace 中取得，並提供在 Azure 上使用 Confluent 雲端供應專案的無縫體驗</span><span class="sxs-lookup"><span data-stu-id="5894d-114">The solution is available in Azure Marketplace and  provides a seamless experience for using the Confluent Cloud offering on Azure</span></span>

<span data-ttu-id="5894d-115">解決方案會使用在 Azure 中啟用的資源提供者來布建 Confluent 雲端資源。</span><span class="sxs-lookup"><span data-stu-id="5894d-115">The solution uses a resource provider enabled in Azure to provision Confluent Cloud resources.</span></span> <span data-ttu-id="5894d-116">這可讓使用者透過 Azure 入口網站、Azure CLI 和 Azure Sdk 來存取即時事件串流。</span><span class="sxs-lookup"><span data-stu-id="5894d-116">This allows users to access real-time event streaming via the Azure portal, Azure CLI, and Azure SDKs.</span></span> <span data-ttu-id="5894d-117">Confluent Cloud 擁有並執行 SaaS 應用程式，其中包括環境、叢集、主題、API 金鑰和受控連接器。</span><span class="sxs-lookup"><span data-stu-id="5894d-117">Confluent Cloud owns and runs the SaaS application, which includes environments, clusters, topics, API keys, and managed connectors.</span></span>

<span data-ttu-id="5894d-118">與 Confluent Cloud 的深度整合可提供下列功能：</span><span class="sxs-lookup"><span data-stu-id="5894d-118">The deep integration with Confluent Cloud enables the following capabilities:</span></span>

- <span data-ttu-id="5894d-119">使用完全受控的基礎結構，從 Azure 入口網站布建新的 Confluent Cloud 組織資源。</span><span class="sxs-lookup"><span data-stu-id="5894d-119">Provision a new Confluent Cloud organization resource from the Azure portal with fully managed infrastructure.</span></span>
- <span data-ttu-id="5894d-120">使用 Azure Active Directory，簡化從 Azure 到 Confluent Cloud 的單一登入;Confluent Cloud 入口網站不需要個別的驗證。</span><span class="sxs-lookup"><span data-stu-id="5894d-120">Streamline single sign-on from Azure to Confluent Cloud with Azure Active Directory; no separate authentication needed from the Confluent Cloud portal.</span></span>
- <span data-ttu-id="5894d-121">透過 Azure 訂用帳戶發票來取得 Confluent 雲端耗用量費用的統一帳單。</span><span class="sxs-lookup"><span data-stu-id="5894d-121">Get unified billing of Confluent Cloud consumption charges through Azure subscription invoicing.</span></span>
- <span data-ttu-id="5894d-122">從 Azure 入口網站管理 Confluent 雲端資源，並在 [ **所有資源** ] 頁面中，連同您的 Azure 資源一起追蹤它們。</span><span class="sxs-lookup"><span data-stu-id="5894d-122">Manage Confluent Cloud resources from the Azure portal, and track them in the **All resources** page, alongside your Azure resources.</span></span>

[<span data-ttu-id="5894d-123">Confluent 雲端部署指南</span><span class="sxs-lookup"><span data-stu-id="5894d-123">Confluent Cloud deployment guides</span></span>](https://docs.confluent.io/current/cloud/marketplace/index.html)

<span data-ttu-id="5894d-124">關於 Confluent on Azure 的相關問題，請移至 [https://support.confluent.io](https://support.confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="5894d-124">For issues related to Confluent on Azure, go to [https://support.confluent.io](https://support.confluent.io).</span></span> <span data-ttu-id="5894d-125">如果您是第一次使用者，請先重設您的密碼，然後再登入 Confluent 支援入口網站。</span><span class="sxs-lookup"><span data-stu-id="5894d-125">If you are a first time user, reset your password before you sign in to the Confluent Support Portal.</span></span> <span data-ttu-id="5894d-126">如果您沒有包含 Confluent 的帳戶，請傳送電子郵件至 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。</span><span class="sxs-lookup"><span data-stu-id="5894d-126">If you do not have an account with Confluent, please send an email to [cloud-support@confluent.io](mailto:cloud-support@confluent.io).</span></span>

## <a name="datadog"></a><span data-ttu-id="5894d-127">Datadog</span><span class="sxs-lookup"><span data-stu-id="5894d-127">Datadog</span></span>

![DataDog 標誌](./media/partners/datadog.png)

<span data-ttu-id="5894d-129">Datadog 為 Azure 使用者提供可檢視性和安全性工具，以瞭解應用程式在混合式和多重雲端環境中的健全狀況和效能。</span><span class="sxs-lookup"><span data-stu-id="5894d-129">Datadog provides observability and security tools for Azure users to understand the health and performance of their applications across hybrid and multi-cloud environments.</span></span> <span data-ttu-id="5894d-130">但是，設定所需的整合通常需要在 Azure 入口網站和 Datadog 之間流覽。</span><span class="sxs-lookup"><span data-stu-id="5894d-130">But configuring the necessary integrations often requires navigating between the Azure portal and Datadog.</span></span> <span data-ttu-id="5894d-131">為了簡化跨入口網站的設定和資源管理，Microsoft 與 Datadog 合作，在 Azure 上建立整合式 Datadog 解決方案。</span><span class="sxs-lookup"><span data-stu-id="5894d-131">To simplify configuration and resource management across portals, Microsoft worked with Datadog to create an integrated Datadog solution on Azure.</span></span> <span data-ttu-id="5894d-132">此解決方案可透過 Azure Marketplace 提供順暢的體驗，讓 Azure 客戶能夠使用 Datadog 的雲端監視解決方案。</span><span class="sxs-lookup"><span data-stu-id="5894d-132">Available via the Azure Marketplace, this solution provides a seamless experience for Azure customers to use Datadog’s cloud monitoring solution.</span></span>

<span data-ttu-id="5894d-133">請參閱 [Azure 監視器檔](/azure/azure-monitor/platform/partners#datadog) ，以深入瞭解此解決方案並註冊公開預覽。</span><span class="sxs-lookup"><span data-stu-id="5894d-133">See the [Azure Monitor documentation](/azure/azure-monitor/platform/partners#datadog) to learn more about this solution and sign up for the public preview.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5894d-134">後續步驟</span><span class="sxs-lookup"><span data-stu-id="5894d-134">Next steps</span></span>

- [<span data-ttu-id="5894d-135">Azure Marketplace 線上商店</span><span class="sxs-lookup"><span data-stu-id="5894d-135">Azure Marketplace online store</span></span>](https://azure.microsoft.com/marketplace/)
- [<span data-ttu-id="5894d-136">Microsoft Learn：建立 Azure 帳戶</span><span class="sxs-lookup"><span data-stu-id="5894d-136">Microsoft Learn: Create an Azure account</span></span>](/learn/modules/create-an-azure-account/)
