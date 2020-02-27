---
title: 客戶轉換至 Azure 方案 | 合作夥伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何輕鬆地將您的客戶移至 Azure 方案。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567234"
---
# <a name="transition-your-customers-to-azure-plan"></a>將您的客戶轉換為 Azure 方案

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員
- 技術服務代理人
- 銷售代理人
- 使用者管理系統管理員

間接提供者和直接帳單合作夥伴可以轉換為適用於 Azure 的 Microsoft 雲端服務提供者計畫 (CSP) 中所提供的新商務體驗。 (間接經銷商必須透過其間接提供者來運作)。客戶可以透過簡化的方式購買雲端服務，無論是向合作夥伴、Microsoft 賣方或直接在網路上購買。

轉換功能僅適用於轉換至適用於 Azure 新商務經驗的客戶，以及已簽署 Microsoft 客戶合約的使用者，而不是針對 CSP 中的其他供應項目，例如 Office 365 或 Dynamics 365。

## <a name="available-azure-services-in-azure-csp"></a>Azure CSP 中可用的 Azure 服務

本節將討論 Azure 雲端解決方案提供者 (CSP) 計畫中可用和不可用的 Azure 服務。 文中也會討論國家/地區雲端 [Microsoft Azure Germany](https://azure.microsoft.com/overview/clouds/germany/) 和 [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/) 中的服務可用性。

>[!Note]
>[Azure 中國]( https://www.azure.cn/)無法從 Azure CSP 計畫中取得。

### <a name="global-cloud"></a>全球雲端 

以 Azure Resource Manager 模型為基礎的所有服務都可在 CSP 計畫中取得。  非 Azure Resource Manager 服務則無法在 CSP 計畫中取得。  

### <a name="csp-specific-service-configurations"></a>CSP 特定服務的設定

下列服務需要在 CSP 中進行特殊設定：

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure 時間序列深入解析](https://azure.microsoft.com/services/time-series-insights/) 只有來自客戶租用戶的使用者可以存取其時間序列深入解析環境中的資料。 根據預設，合作夥伴可以管理其客戶的時間序列深入解析環境，但如果需要存取其中的資料，就必須已新增至客戶租用戶。 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

您現在可以從 Visual Studio Marketplace 購買下面列出的項目，但第三方擴充功能除外。

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Visual Studio 訂閱](https://www.visualstudio.com/subscriptions/)

- [Xamarin University 訓練](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

為了協助您開始使用，我們在 CSP 中製作了一些關於[如何設定、購買和管理 Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) 的影片和文件。

### <a name="azure-marketplace-items-in-azure-csp"></a>Azure CSP 中的 Azure Marketplace 項目

並非所有的 Azure Marketplace 項目目前都可在 Azure CSP 訂閱中使用。

- 以 Microsoft 為基礎的 Azure 服務：這些服務可供使用。 請檢閱先前的資料表和註解。

- 自備授權 (BYOL) 項目：這些項目都可供使用。 具有 BYOL 功能的 Azure Marketplace 項目完整清單可在 [Azure Marketplace BYOL 頁面](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)上取得。

- 隨用隨付第三方 Azure Marketplace 項目：如果提供者已發佈至 CSP 管道，則這些項目可供使用。 如需詳細資訊，請參閱[銷售 Azure Marketplace 產品的訂閱](https://aka.ms/marketplaceincsp)。   

- Citrix XenApp Essentials：合作夥伴可以在 CSP 中為客戶購買 XenApp Essentials。 如需詳細資訊，請參閱下列 Citrix 部落格 - [現在可透過 Microsoft 雲端解決方案提供者管道散發 XenApp Essentials](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/)。

### <a name="national-clouds"></a>國家/地區雲端 
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

### <a name="next-steps"></a>接下來的步驟

- [了解](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview)合作夥伴中心的 Azure 可用功能。

- 在 Azure CSP 中[建立](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer)您的第一個客戶，並部署 Azure 服務。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>將現有的 CSP 供應項目轉換為 Azure 方案

您可以透過合作夥伴中心內 CSP 計畫中的新商務體驗，將客戶從他們的現有 CSP Azure 供應項目轉換到 Azure 方案下的 Azure 服務。 若要這麼做，合作夥伴和客戶必須透過合作夥伴中心建立轉售商關係，而且客戶必須已簽署 Microsoft 客戶合約。

### <a name="select-transition-to-azure-plan"></a>選取轉換至 Azure 方案

1. 為您的客戶選取 Azure 方案。

2. 選取 [將計費轉換為 Azure 方案]  。

![轉換](images/azure/transition1.png)

3. 選取 [繼續] 

![轉換](images/azure/transition2.png)

您的客戶將會轉換為 Azure 方案。

**轉換工作流程會自動執行必要的步驟**：

- 購買 Azure 方案
- 在直接 CSP 案例中，每位客戶一個方案  
- 每個轉售商一個方案  

例如，合作夥伴購買了兩個 Microsoft Azure 供應項目，並在購買中包含兩個不同的 POR。 在此情況下，轉換工作流程會購買兩個 Azure 方案 (每個轉售商一個)，並自動對應 Azure 方案底下的個別 Azure 訂用帳戶。  

**將 Azure 訂用帳戶對應至 Azure 方案**

購買 Azure 方案之後，我們的系統會將現有的 Azure 訂用帳戶對應至 Azure 方案。 您可以在 Azure 入口網站和合作夥伴中心檢視進度。 

4. 返回客戶的合作夥伴中心 [訂用帳戶]  頁面，使用他們的當地貨幣更新其預算限制。 

![轉換](images/azure/transition3.png)

>[!NOTE]
>您在合作夥伴中心設定的預算不會帶到 Azure 入口網站。 您也應該在 Azure 入口網站中設定預算和警示。

當您移至 Azure 方案時，您無法再為此客戶購買 Azure 訂用帳戶。 您會在 Azure 入口網站中建立 Azure 方案底下的訂用帳戶。

>[!NOTE]
> 所有 Azure 方案底下透過 RBAC 購買的 Azure 訂用帳戶，都會以當地貨幣計價和計費。 將不會使用 FX 費率。

### <a name="track-your-transition-details"></a>追蹤您的轉換詳細資料

在 Azure 入口網站和合作夥伴中心追蹤進度。

![顯示詳細資料](images/azure/details1.png)

**對合作夥伴的計費影響**

如果您從現有的 CSP Azure 供應項目轉換客戶，將會有下列計費影響：

- 您將需支付截至結束原始 CSP Azure 訂用帳戶時間點，所有使用量的現有 CSP 發票費用。

- 如果您擁有現有 CSP 訂用帳戶的系統管理員存取權限，則在遷移該訂用帳戶時，您將會繼續擁有存取權。

若要將 CSP 和伺服器和雲端註冊的直接 Enterprise 合約轉換至Azure 服務，請參閱[取得 Microsoft 合作夥伴合約 Azure 訂用帳戶的計費擁有權](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

**稽核記錄**：

若要調解計費，請在 [訂用帳戶]  頁面上，檢視您的 "Microsoft Azure" (0145P) 訂用帳戶的歷程記錄。 

"Microsoft Azure" (0145P) 訂用帳戶由兩個部分組成：
1. 商務訂用帳戶 
2. Azure 訂用帳戶 (權利)

轉換完成時，會將 Azure 訂用帳戶移至新的 Azure 方案底下，並暫停商務訂用帳戶，這樣就不會再報告有使用量。  

>[注意]：當 Microsoft Azure (0145P) 訂用帳戶是在 CSP 中購買時，商務訂用帳戶和 Azure 訂用帳戶 (權利) 會具有相同值。 只有在計費擁有權變更或傳輸的情況下，這些值才會有所不同。 

**轉換問題**

轉換期間發生任何問題並不在預料之中。 如果發生失敗情況，我們會在轉換工作流程本身中為您更新。 Azure 使用量不會受到干擾。  

## <a name="next-steps"></a>接下來的步驟

- [管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)

- [合作夥伴所獲得信用點數 - 概觀](partner-earned-credit.md)



