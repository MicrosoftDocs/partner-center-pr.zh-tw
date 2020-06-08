---
title: Azure CSP 中可用的 Azure 服務
description: 本節將討論 Azure 雲端解決方案提供者 (CSP) 計畫中可用和不可用的 Azure 服務。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: dad65d2237a4446bd6a555a600193e7885bc6f5e
ms.sourcegitcommit: 775a13540d6576201a900e517a0696a6ff4897d8
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84458334"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Azure 雲端解決方案提供者 (CSP) 計畫中可用的 Azure 服務

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員
- 技術服務代理人
- 銷售代理人
- 使用者管理系統管理員

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP 中可用的 Azure 服務

本文列出 Azure 雲端解決方案提供者 (CSP) 計畫中可用和不可用的 Azure 服務。 文中也會討論國家/地區雲端 [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) 和 [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) 中的服務可用性。

>[!Note]
> [Azure 中國](https://www.azure.cn/)無法從 Azure CSP 計畫中取得。

## <a name="global-cloud"></a>全球雲端

以 Azure Resource Manager 模型為基礎的所有服務都可在 CSP 計畫中取得。  非 Azure Resource Manager 服務則無法在 CSP 計畫中取得。  

## <a name="csp-specific-service-configurations"></a>CSP 特定服務的設定

下列服務需要在 CSP 中進行特殊設定：

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure 時間序列深入解析](https://azure.microsoft.com/services/time-series-insights/) 只有來自客戶租用戶的使用者可以存取其時間序列深入解析環境中的資料。 根據預設，合作夥伴可以管理其客戶的時間序列深入解析環境，但如果需要存取其中的資料，就必須已新增至客戶租用戶。

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

您現在可以從 Visual Studio Marketplace 購買下面列出的項目，但第三方擴充功能除外。

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio 訂閱](https://www.visualstudio.com/subscriptions/)

- [Xamarin University 訓練](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

為了協助您開始使用，我們在 CSP 中製作了一些關於[如何設定、購買和管理 Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) 的影片和文件。

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP 中的 Azure Marketplace 項目

並非所有的 Azure Marketplace 項目目前都可在 Azure CSP 訂閱中使用。

- 以 Microsoft 為基礎的 Azure 服務：這些服務可供使用。 請檢閱先前的資料表和註解。

- 自備授權 (BYOL) 項目：這些項目都可供使用。 具有 BYOL 功能的 Azure Marketplace 項目完整清單可在 [Azure Marketplace BYOL 頁面](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)上取得。

- 隨用隨付第三方 Azure Marketplace 項目：如果提供者已發佈至 CSP 管道，則這些項目可供使用。 如需詳細資訊，請參閱[銷售 Azure Marketplace 產品的訂閱](https://aka.ms/marketplaceincsp)。

- Citrix XenApp Essentials：合作夥伴可以在 CSP 中為客戶購買 XenApp Essentials。 如需詳細資訊，請參閱下列 Citrix 部落格 - [現在可透過 Microsoft 雲端解決方案提供者管道散發 XenApp Essentials](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)。

## <a name="national-clouds"></a>國家/地區雲端

下表顯示國家/地區雲端中適用於 CSP、會定期更新的第一方 Azure 產品、服務和功能清單。

| Azure 產品、服務或功能 | 美國政府 | 德國 |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  虛擬機器  |  X  |  X  |
|  雲端服務  |    |    |
|  虛擬機器擴展集  |  X  |  X  |
|  函式  |    |    |
|  Azure Container Service  |    |    |
|  **網路功能**  |    |    |
|  Azure DNS  |    |    |
|  內容傳遞網路  |    |    |
|  流量管理員  |    |    |
|  ExpressRoute  |  X  |  X  |
|  虛擬網路  |  X  |  X  |
|  負載平衡器  |  X  |  X  |
|  VPN 閘道  |  X  |  X  |
|  應用計畫閘道  |  X  |  X  |
|  網路監看員  |  X  |  X  |
|  **儲存體**  |    |    |
|  存放裝置  |  X  |  X  |
|  備份  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  受控磁碟  |  X  |  X  |
|  **Web + 行動**  |    |    |
|  App Service  |  X  |  X  |
|  Linux 上的 App Service  |    |  X  |
|  API 管理  |  X  |    |
|  內容傳遞網路  |    |    |
|  媒體服務  |  X  |  X  |
|  通知中樞  |  X  |  X  |
|  Azure 搜尋服務  |    |    |
|  Azure App Service 的 Logic Apps 功能  |    |    |
|  **容器**  |    |    |
|  App Service  |  X  |  X  |
|  Linux 上的 App Service  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  容器執行個體  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **資料庫**  |    |    |
|  SQL 資料庫  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL 資料倉儲  |  X  |  X  |
|  Redis 快取  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  適用於 MySQL 的 Azure 資料庫  |    |    |
|  適用於 PostgreSQL 的 Azure 資料庫  |    |    |
|  **資料 + 分析**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  串流分析  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  資料目錄  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI + 認知服務**  |    |    |
|  機器學習  |    |  X  |
|  Azure Bot Service  |    |    |
|  認知服務  |    |    |
|  Azure Batch AI  |    |    |
|  **物聯網**  |    |    |
|  IoT 中樞  |  X  |  X  |
|  IoT Central  |    |    |
|  機器學習  |    |  X  |
|  串流分析  |    |  X  |
|  事件中樞  |  X  |  X  |
|  依位置提供的服務  |    |    |
|  通知中樞  |  X  |  X  |
|  時間序列深入解析  |    |    |
|  **企業整合**  |    |    |
|  StorSimple  |  X  |    |
|  API 管理  |    |    |
|  事件方格  |    |    |
|  Data Factory  |    |    |
|  服務匯流排  |  X  |  X  |
|  資料目錄  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Azure App Service 的 Logic Apps 功能  |    |    |
|  **安全性 + 身分識別**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  多重要素驗證  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  資訊安全中心  |  X  |  X  |
|  **開發人員工具**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **監視 + 管理**  |    |    |
|  Advisor  |    |    |
|  備份  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  排程器  |  X  |  X  |
|  自動化  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure 監視器  |    |    |
|  Azure 受控應用計畫  |    |    |
|  Azure Migrate  |    |    |
|  管理群組  |    |  

## <a name="next-steps"></a>接下來的步驟

- [了解](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview)合作夥伴中心的 Azure 可用功能。

- 在 Azure CSP 中[建立](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer)您的第一個客戶，並部署 Azure 服務。
