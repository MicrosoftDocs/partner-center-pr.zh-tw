---
title: 角色、合作夥伴取得點數的許可權
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解合作夥伴的角色和許可權，以取得合作夥伴獲得的點數 (PEC) 。 這些角色不同于合作夥伴中心中的角色。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011738"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>符合可獲得合作夥伴所獲得點數的角色和許可權

下列角色會對應到可判斷合作夥伴是否符合合作夥伴所獲得點數資格的許可權層級。

>[!Important]
>這些角色和許可權與使用者在合作夥伴中心中所需的角色和許可權不同。

|**角色**   |**說明**   |**PEC 合格**   |
|-----------------|:------------------|:--------------|
|擁有者  |您可以管理所有專案，包括對資源的存取。|Yes|
|參與者 |除了授與資源的存取權之外，您還可以管理所有專案。|Yes|
|讀取者|您可以查看所有內容，但不會進行任何變更|No|
|ACRDelete|acr 刪除|Yes|
|ACRImageSigner|ACR 影像簽署者|Yes|
|ACRPull|acr 提取|Yes|
|AcrPush|acr 推送|Yes|
|AcrQuarantineReader|ACR 隔離資料讀取者|No|
|AcrQuarantineWriter| ACR 隔離資料寫入者|Yes|
|API 管理服務參與者|可管理服務與 API|Yes|
|API 管理服務操作員角色|可管理服務，但無法管理 API|Yes|
|API 管理服務讀取者角色|具有服務與 API 的唯讀存取權|No|
|Application Insights 元件參與者|管理 Application Insights 元件|Yes|
|Application Insights 快照集偵錯工具|給予使用者權限，以便檢視及下載使用 Application Insights 快照偵錯工具所收集的偵錯快照。 請注意，擁有者或參與者角色未包含這些權限。|Yes|
自動化作業運算子 | 使用「自動化 Runbook」來建立及管理作業。 | Yes | 
自動化運算子 | 「自動化運算子」能夠啟動、停止、暫止及繼續作業 | Yes | 
自動化 Runbook 運算子 | 讀取 Runbook 屬性 - 以便能夠建立 Runbook 的作業。 | Yes | 
Avere 參與者 | 可以建立和管理 Avere vFXT 叢集。 | Yes | 
Avere 操作員 | 供 Avere vFXT 叢集用來管理叢集 | Yes | 
Azure 事件中樞資料擁有者 | 允許完整存取 Azure 事件中樞資源。 | Yes | 
Azure 事件中樞資料接收者 | 允許接收 Azure 事件中樞資源。 | Yes | 
Azure 事件中樞資料傳送者 | 允許傳送 Azure 事件中樞資源。 | Yes | 
Azure Kubernetes Service 叢集管理員角色 | 列出叢集管理員認證動作。 | Yes | 
Azure Kubernetes Service 叢集使用者角色 | 列出叢集使用者認證動作。 | Yes | 
Azure 地圖服務資料讀者 (預覽) | 授權從 Azure 地圖服務帳戶讀取地圖相關資料。 | No | 
Azure 服務匯流排資料擁有者 | 允許完整存取 Azure 服務匯流排資源。 | Yes | 
Azure 服務匯流排資料接收者 | 允許接收 Azure 服務匯流排資源。 | Yes | 
Azure 服務匯流排資料傳送者 | 允許傳送 Azure 服務匯流排資源。 | Yes | 
Azure Stack 註冊擁有者 | 可讓您管理 Azure Stack 註冊。 | Yes | 
備份參與者 | 可讓您管理備份服務，但無法建立保存庫及授與存取權給其他人 | Yes | 
備份操作員 | 可讓您管理備份服務，但無法移除備份、建立保存庫及為其他人提供存取權 | Yes | 
備份讀取者 | 可以檢視備份服務，但無法進行變更 | No | 
帳單讀取器 | 允許對計費資料進行讀取存取 | No | 
BizTalk 參與者 | 可讓您管理 BizTalk 服務，但無法存取它們。 | Yes | 
區塊鏈成員節點存取 (預覽) | 允許存取區塊鏈成員節點 | Yes | 
藍圖參與者 | 可以管理藍圖定義，但不能加以指派。 | Yes | 
藍圖操作員 | 可以指派現有已發佈的藍圖，但無法建立新的藍圖。 注意：這只適用于使用使用者指派的受控識別來完成指派。 | Yes | 
CDN 端點參與者 | 可管理 CDN 端點，但無法對其他使用者授與存取權。 | Yes | 
CDN 端點讀者 | 可檢視 CDN 端點，但無法進行變更。 | No | 
CDN 設定檔參與者 | 可管理 CDN 設定檔及其端點，但無法對其他使用者授與存取權。 | Yes | 
CDN 設定檔讀者 | 可檢視 CDN 設定檔及其端點，但無法進行變更。 | No | 
傳統網路參與者 | 可讓您管理傳統網路，但無法存取它們。 | Yes | 
傳統儲存體帳戶參與者 | 可讓您管理傳統儲存體帳戶，但無法存取它們。 | Yes | 
傳統儲存體帳戶金鑰操作員服務角色 | 「傳統儲存體帳戶金鑰操作員」可以列出及重新產生「傳統儲存體帳戶」的金鑰 | Yes | 
傳統虛擬機器參與者 | 可讓您管理傳統虛擬機器 (不含虛擬機器所連線的虛擬網路或儲存體帳戶)，但無法存取它們。 | Yes | 
認知服務參與者 | 可讓您建立、讀取、更新、刪除及管理認知服務的金鑰。 | Yes | 
認知服務資料讀者 (預覽) | 可讓您讀取認知服務資料。 | No | 
認知服務使用者 | 可讓您讀取和列出認知服務的金鑰。 | No | 
Cosmos DB 帳戶讀者角色 | 可以讀取 Azure Cosmos DB 帳戶資料。 請參閱 DocumentDB 帳戶參與者以管理 Azure Cosmos DB 帳戶。 | No | 
Cosmos DB 操作員 | 可讓您管理 Azure Cosmos DB 帳戶，但無法存取其中的資料。 防止存取帳戶金鑰和連接字串。 | Yes | 
CosmosBackupOperator | 可為帳戶的 Cosmos DB 資料庫或容器提交還原要求 | Yes | 
成本管理參與者 | 可檢視成本和管理成本組態 (例如預算、匯出) | Yes | 
成本管理讀者 | 可檢視成本資料和組態 (例如預算、匯出) | No | 
資料箱參與者 | 可讓您管理資料箱服務下的所有項目，為他人賦予存取權除外。 | Yes | 
資料箱讀者 | 可讓您管理資料箱服務，建立訂單或編輯訂單詳細資料和為他人賦予存取權除外。 | No | 
Data Factory 參與者 | 建立和管理 Data Factory，以及其中的子資源。 | Yes | 
Data Lake Analytics 開發人員 | 可讓您提交、監視及管理您自己的作業，但無法建立或刪除 Data Lake Analytics 帳戶。 | Yes | 
資料清除者 | 可清除分析資料 | Yes | 
DevTest Labs 使用者 | 可讓您連線、啟動、重新啟及關閉您 Azure DevTest Labs 中的虛擬機器。 | Yes | 
DNS 區域參與者 | 可讓您管理 Azure DNS 中的 DNS 區域與記錄集，但無法讓您控制誰可存取它們。 | Yes | 
DocumentDB 帳戶參與者 | 可以管理 Azure Cosmos DB 帳戶。 Azure Cosmos DB 先前稱為 DocumentDB。 | Yes | 
EventGrid EventSubscription 參與者 | 可讓您管理 EventGrid 事件訂用帳戶作業。 | Yes | 
EventGrid EventSubscription 讀者 | 可讓您讀取 EventGrid 事件訂用帳戶。 | No | 
HDInsight 叢集操作員 | 可讓您讀取和修改 HDInsight 叢集設定。 | Yes | 
HDInsight 網域服務參與者 | 可讀取、建立、修改和刪除 HDInsight 企業安全性套件所需的網域服務相關作業 | Yes | 
Intelligent Systems 帳戶參與者 | 可讓您管理「智慧型系統」帳戶，但無法存取它們。 | Yes | 
Key Vault 參與者 | 可讓您管理金鑰保存庫，但無法存取它們。 | Yes | 
實驗室建立者 | 可讓您在「Azure 實驗室帳戶」下建立、管理、刪除您的受控實驗室。 | Yes | 
Log Analytics 參與者 | 「Log Analytics 參與者」角色可以讀取所有監視資料和編輯監視設定。 編輯監視設定包括將 VM 延伸模組新增至 VM、讀取儲存體帳戶金鑰以便能夠設定從「Azure 儲存體」收集記錄、建立及設定「自動化」帳戶、新增解決方案，以及設定所有 Azure 資源上的 Azure 診斷。 | Yes | 
Log Analytics 讀者 | 「Log Analytics 讀者」可以檢視和搜尋所有監視資料，以及檢視監視設定，包括檢視所有 Azure 資源上的 Azure 診斷設定。 | No | 
邏輯應用程式參與者 | 可讓您管理邏輯應用程式，但無法變更對邏輯應用程式的存取。 | Yes | 
邏輯應用程式操作員 | 可讓您讀取、啟用及停用邏輯應用程式，但無法編輯或更新邏輯應用程式。 | Yes | 
受控應用程式操作員角色 | 可讓您讀取受控應用程式資源及對其執行動作 | Yes | 
受控應用程式讀者 | 可讓您讀取受控應用程式中的資源及要求 JIT 存取權。 | No | 
受控身分識別參與者 | 建立、讀取、更新及刪除使用者指派的身分識別 | Yes | 
受控身分識別操作員 | 讀取及指派使用者指派的身分識別 | Yes | 
管理群組參與者 | 管理群組參與者角色 | Yes | 
管理群組讀者 | 管理群組讀者角色 | No | 
監視參與者 | 可以讀取所有監視資料並編輯監視設定。 請參閱開始使用 Azure 監視器的角色、權限和安全性。 | Yes | 
監視計量發行者 | 針對 Azure 資源啟用發佈計量 | Yes | 
監視讀取器 | 可以讀取所有監視資料 (計量、記錄等等)。 請參閱開始使用 Azure 監視器的角色、權限和安全性。 | No | 
網路參與者 | 可讓您管理網路，但無法存取它們。 | Yes | 
New Relic APM 帳戶參與者 | 可讓您管理 New Relic Application Performance Management 帳戶及應用程式，但無法存取它們。 | Yes | 
讀取者及資料存取 | 可讓您檢視所有內容，但無法讓您刪除或建立儲存體帳戶或內含的資源。 也可透過存取儲存體帳戶金鑰，對儲存體帳戶中內含的所有資料進行讀取/寫入存取。 | Yes | 
Redis 快取參與者 | 可讓您管理 Redis 快取，但無法存取它們。 | Yes | 
資源原則參與者 (預覽) | (預覽) 從 EA 回填的使用者，有權建立/修改資源原則、建立支援票證及讀取資源/階層。 | Yes | 
排程器工作集合參與者 | 可讓您管理「排程器」工作集合，但無法存取它們。 | Yes | 
搜尋服務參與者 | 可讓您管理「搜尋」服務，但無法存取它們。 | Yes | 
安全性系統管理員 | 僅限資訊安全中心：可檢視安全性原則、檢視安全性狀態、編輯安全性原則、檢視警示和建議、關閉警示和建議 | Yes | 
安全性管理員 (舊版) | 此為舊版角色。 請改用安全性系統管理員 | Yes | 
安全性讀取者 | 僅限資訊安全中心：可檢視建議和警示、檢視安全性原則、檢視安全性狀態，但無法進行變更 | No | 
Site Recovery 參與者 | 可讓您管理 Site Recovery 服務，但無法建立保存庫和指派角色 | Yes | 
Site Recovery 操作員 | 可讓您容錯移轉及容錯回復，但無法執行其他 Site Recovery 管理作業 | Yes | 
Site Recovery 讀取者 | 可讓您檢視 Site Recovery 狀態，但無法執行其他管理作業 | No | 
空間錨點帳戶參與者 | 可讓您管理帳戶中的空間錨點，但無法刪除 | Yes | 
空間錨點帳戶擁有者 | 可讓您管理帳戶中的空間錨點，包含刪除 | Yes | 
空間錨點帳戶讀者 | 可讓您尋找和讀取帳戶中空間錨點的屬性 | No | 
SQL DB 參與者 | 可讓您管理 SQL 資料庫，但無法存取它們。 此外，您也無法管理其安全性相關原則或其父 SQL 伺服器。 | Yes | 
SQL 受控執行個體參與者 | 可讓您管理 SQL 受控實例和必要的網路設定，但無法將存取權授與其他人。 | Yes | 
SQL 安全性管理員 | 可讓您管理 SQL 伺服器及資料庫的安全性相關原則，但無法存取它們。 | Yes | 
SQL Server 參與者 | 可讓您管理 SQL 伺服器及資料庫，但無法存取它們，也無法存取其安全性相關原則。 | Yes | 
儲存體帳戶參與者 | 允許管理儲存體帳戶。 支援存取帳戶金鑰，以透過共用金鑰授權來存取資料。 | Yes | 
儲存體帳戶金鑰操作員服務角色 | 允許列出及重新產生儲存體帳戶存取金鑰。 | Yes | 
儲存體 Blob 資料參與者 | 讀取、寫入和刪除 Azure 儲存體的容器和 blob。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | Yes | 
儲存體 Blob 資料擁有者 | 支援完整存取 Azure 儲存體 blob 容器和資料，包括指派 POSIX 存取控制。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | Yes | 
儲存體 Blob 資料讀者 | 讀取和列出 Azure 儲存體的容器和 blob。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | No | 
儲存體 Blob 委派者 | 取得使用者委派金鑰，以針對使用 Azure AD 認證所簽署的容器或 blob，建立共用存取簽章。 如需詳細資訊，請參閱建立使用者委派 SAS。 | Yes | 
儲存體檔案資料 SMB 共用參與者 | 允許透過 SMB 進行 Azure 儲存體檔案共用的讀取、寫入和刪除存取 | Yes | 
儲存體檔案資料 SMB 共用提升權限的參與者 | 允許透過 SMB 在 Azure 儲存體檔案共用中讀取、寫入、刪除及修改 NTFS 許可權存取 | Yes | 
儲存體檔案資料 SMB 共用讀者 | 允許透過 SMB 讀取存取 Azure 檔案共用 | No | 
儲存體佇列資料參與者 | 讀取、寫入及刪除 Azure 儲存體的佇列和佇列訊息。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | Yes | 
儲存體佇列資料訊息處理者 | 從 Azure 儲存體佇列中瞄核、擷取和刪除訊息。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | Yes | 
儲存體佇列資料訊息傳送者 | 將訊息新增至 Azure 儲存體佇列。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | Yes | 
儲存體佇列資料讀者 | 讀取和列出 Azure 儲存體的佇列和佇列訊息。 若要了解特定資料作業所需的動作，請參閱呼叫 blob 和佇列資料作業的權限。 | No | 
支援要求參與者 | 可讓您建立及管理支援要求 | Yes | 
流量管理員參與者 | 可讓您管理「流量管理員」設定檔，但無法控制誰可以存取它們。 | Yes | 
使用者存取系統管理員 | 可讓您管理 Azure 資源的使用者存取。 | Yes | 
虛擬機器系統管理員登入 | 在入口網站中檢視虛擬機器並以系統管理員身分登入 | Yes | 
虛擬機器參與者 | 可讓您管理虛擬機器 (不含虛擬機器所連接的虛擬網路或儲存體帳戶)，但無法存取它們。 | Yes | 
虛擬機器使用者登入 | 在入口網站中檢視虛擬機器並以一般使用者身分登入。 | Yes | 
Web 方案參與者 | 可讓您管理網站的 Web 方案，但無法存取它們。 | Yes | 
網站參與者 | 可讓您管理網站 (不會) web 方案，但無法存取它們 | 是 |
