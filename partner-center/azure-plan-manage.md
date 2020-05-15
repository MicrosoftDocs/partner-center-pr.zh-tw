---
title: Azure 方案 - 管理訂用帳戶與資源
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作夥伴如何使用不同的角色型存取控制 (RBAC) 選項，來對客戶 Azure 資源的操作進行控制和管理。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 65362d9f71882d9edff34039f7fc985a202c4aa0
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908343"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>管理 Azure 方案下的訂用帳戶和資源

當您將客戶轉換至 Azure 方案時，預設會在 Azure 中獲指派特殊系統管理權限 (透過代表管理員的訂用帳戶擁有者權限)。

 > [!NOTE]
 > 客戶可以在訂用帳戶、資源群組或工作負載層級移除 Azure 訂用帳戶的系統管理員權限。 

 合作夥伴可以使用透過角色型存取控制功能 (RBAC) 提供的不同選項，在 CSP 中取得客戶 Azure 資源的全天候操作控制和管理。 

- **系統管理員代表 (AOBO)** - 使用 [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 時，在合作夥伴租用戶中具有系統管理代理人角色的任何使用者，都將擁有您透過 CSP 計畫所建立 Azure 訂用帳戶的 RBAC 擁有者存取權。

- **Azure Lighthouse**：AOBO 不允許彈性建立與不同客戶一起使用的不同群組，或為群組或使用者啟用不同的角色。 使用 Azure Lighthouse，您可以將不同的群組指派給不同的客戶或角色。 因為使用者會透過 Azure 委派的資源管理來擁有適當的存取層級，所以您可以減少擁有系統管理代理人角色的使用者人數 (因而擁有完整的 AOBO 存取權)。 藉由限制對客戶資源的不必要存取來協助改善安全性。 它也可讓您更有彈性地大規模管理多個客戶。 如需詳細資訊，請參閱 [Azure Lighthouse 與雲端解決方案提供者計畫](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider)。

-  **目錄或來賓使用者或[服務主體](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** ：您可以藉由在客戶目錄中新增使用者，或新增來賓使用者並指派特定 RBAC 角色，委派對 CSP 訂用帳戶的細微存取權。 

Microsoft 建議使用者擁有執行其工作所需的最小權限，作為安全性做法。 請參閱 [Azure Active Directory Privileged Identity Management 資源](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)。 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>將您的合作夥伴識別碼 (MPN 識別碼) 連結至您的認證，以管理客戶的 Azure 資源

下表顯示用來將您的合作夥伴識別碼與各種 RBAC 存取選項產生關聯的方法。

|**類別**   |**案例**   |**MPN 識別碼關聯**|
|-----------------|:------------------------|:------------------|
|AOBO   |CSP 直接合作夥伴或間接提供者會為客戶建立訂用帳戶，讓 CSP 直接合作夥伴或間接提供者成為使用 AOBO 作為訂用帳戶的預設擁有者；CSP 直接合作夥伴或間接提供者會使用 AOBO 為間接經銷商授與訂用帳戶的存取權。|自動 (不需要合作夥伴工作)|
|Azure Lighthouse|合作夥伴會[在 Marketplace 中建立新的受控服務供應項目](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers)。 CSP 訂用帳戶已接受此供應項目，合作夥伴可以取得 CSP 訂用帳戶的存取權。|自動 (不需要合作夥伴工作)|
|Azure Lighthouse|合作夥伴在 Azure 訂用帳戶中部署 [ARM 範本 ](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer)|合作夥伴必須將 MPN 識別碼與合作夥伴租用戶中的使用者或服務主體產生關聯。 如需詳細資訊 - [連結合作夥伴識別碼](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。|
|目錄或來賓使用者|夥伴會在客戶目錄中建立新的使用者或服務主體，並為使用者提供 CSP 訂用帳戶的存取權。 合作夥伴會在客戶目錄中建立新的使用者或服務主體。 合作夥伴會將使用者新增至群組，並且為群組提供 CSP 訂用帳戶的存取權。|合作夥伴必須將 MPN 識別碼與客戶租用戶中的使用者或服務主體產生關聯。 如需詳細資訊 - [連結合作夥伴識別碼](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。|

## <a name="confirm-that-you-have-admin-access"></a>確認您具有系統管理員存取權

您需要系統管理員存取權來管理您的客戶服務，並接收所獲得的信用點數。 如需所獲得信用點數的詳細資訊，請參閱[合作夥伴所獲得的信用點數](partner-earned-credit.md)。 您有兩種方式可確保您知道您具有系統管理員存取權。

- 檢閱每日使用量檔案 - 可以透過檢閱每日使用量檔案中的單價和有效單位價格來判斷，並確認是否已套用折扣。 如果您收到折扣，您是系統管理員。

- 建立 Azure 監視器警示 - 您可以建立 Azure 監視器活動記錄[警示](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)，以便在您的 RBAC 存取權從 CSP 訂用帳戶中移除時收到通知。

### <a name="create-an-azure-monitor-alert"></a>建立 Azure 監視器警示

1. 建立警示。

![azure 警示](images/azure/azurealert1.png)

2. 選取您想要讓警示採取的動作類型。例如，如果您指定要使用電子郵件，您會收到一封電子郵件，通知您是否發生任何角色指派刪除。

![設定警示](images/azure/azureconfigurealert2.png)

### <a name="aobo-removal"></a>AOBO 移除

客戶可以前往 Azure 入口網站上的 **Access 控制**，來管理其訂用帳戶的存取權。 從 [角色指派]  索引標籤中，選取 [移除存取權]  。 如果發生這種情況，您可以：

- 與您的客戶交談，查看是否可以恢復系統管理員存取權。
- 使用透過[角色型存取控制 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview) 提供的存取權。
- 使用透過 [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) 提供的存取權。

角色型存取權與系統管理員存取權不同。 角色會精確地分隔您可以和不可以執行的動作。 系統管理員存取權較廣泛。

若要查看有資格獲得 PEC 的角色，請參閱[合作夥伴所獲得信用點數的角色和權限](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)。




**詳細資訊**

- [撤銷及恢復 Azure CSP 訂用帳戶的系統管理員權限](revoke-reinstate-csp.md)

- [合作夥伴所獲得信用點數 - 概觀](partner-earned-credit.md)

- [受控服務的合作夥伴所獲得信用點數](partner-earned-credit-explanation.md)