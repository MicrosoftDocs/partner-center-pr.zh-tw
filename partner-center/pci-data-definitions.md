---
title: 見解資料定義
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 此檔提供各種報表的清單，以及每份報表的資料定義，可從 [見解下載報表] 頁面下載。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501744"
---
# <a name="export--data-definitions"></a>匯出–資料定義 

 **適當的角色** 

- 報告檢視人員 
- 高階報告檢視人員 

## <a name="introduction"></a>簡介 

深入解析儀表板中的 [下載報表] 中樞可讓您匯出原始資料集。  

您可以連同資料定義一起下載各種報表，如下所示： 

**夥伴設定檔**：設定檔報表的各種欄位資料定義如下： 


| **資料行名稱** | **資料描述** |
|---------|:---------|
|MPNId|Microsoft 合作夥伴網路識別碼|
|PartnerName|夥伴名稱 |
|PGA_MPNId|合作夥伴通用帳戶 MPN 識別碼|
|PGA_PartnerName|合作夥伴通用帳戶名稱|
|City|合作夥伴的城市位置 |
|國家/地區|合作夥伴的國家/地區位置 |
|HierarchyLevel|指出它是全域 MPN 識別碼或位置 MPN 識別碼|

**客戶詳細** 資料：客戶詳細資料包表的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerName|客戶的名稱 |
|CustomerTenantId|客戶租用戶識別碼 |
|CustomerTpid|客戶最上層父系識別碼 |
|CustomerSegment|客戶區段 |
|CustomerMarket|客戶的地理市場  |
|CustomerStatus|客戶狀態 (Active/Inactive)  |
|產品|MPN 銷售給客戶的產品。 這項程式將是 O365、D365、企業行動力、Power BI Microsoft Azure 的其中一個。|
|SKU|   產品 SKU|
|Month| 回報使用量和收益的月份|
|MPNId| Microsoft 合作夥伴網路識別碼|
|PartnerName|   夥伴名稱|
|PartnerLocation|   合作夥伴的地理位置|
|PartnerAttributionType|    夥伴的屬性類型|
|SalesChannel|  銷售通路|
|空位|    可用基座| 
|RevenueUSD|    以美元為單位的收益|

**轉銷商效能**：轉售商效能報告各欄位的資料定義為：

> [!Note]
> 收益和 ACR 資料僅適用于執行報表檢視器的使用者。

| **資料行名稱** | **資料描述** |
|---------|:---------|
|ResellerMpnid|轉售商 Microsoft 合作夥伴網路識別碼| 
|ResellerName|轉銷商名稱|
|ResellerMarket|市場轉銷商國家/地區| 
|IndirectProviderMPNId|間接提供者 Microsoft 合作夥伴網路識別碼|
|IndirectProviderName|間接提供者名稱|
|Month|回報使用量和收益的月份|
|產品|產品名稱|
|SubscriptionID|訂用帳戶識別碼|
|空位|可用的基座數目|
|AssignedSeats|指派的基座數目|
|BilledRevenueUSD|$) 的 (計費收益|
|CustomerName|客戶的名稱| 
|CustomerTPid|客戶最上層父系識別碼| 
|CustomerSegment|客戶區段 |
|CustomerMarket|客戶的地理市場 |
|ResellerStatus|轉售商狀態| 

訂用帳戶 **詳細** 資料：訂用帳戶詳細資料包表的各種欄位資料定義如下：

>[!Note]
>收益和 ACR 資料僅適用于主管報表檢視器的使用者

| **資料行名稱** | **資料描述** |
|---------|:---------|
|SubscriptionId|    訂用帳戶的 GUID|
|SubscriptionStartDate| 訂用帳戶的開始日期|
|SubscriptionEndDate|   訂用帳戶的結束日期|
|SubscriptionState| 訂用帳戶的狀態 (Active 或流失) |
|Month| 回報使用量和收益的月份|
|IsAutoRenew|   指出訂用帳戶是自動續訂，還是不 (Y/N) |
|CustomerName|  客戶名稱| 
|CustomerTenantId|  客戶 GUID|
|CustomerTpid|  客戶最上層父系識別碼| 
|CustomerSegment|   客戶的市場部門| 
|CustomerMarket|    客戶的地理市場|
|產品|   合作夥伴銷售給客戶的產品| 
|SKU|   產品的 Sku |
|MPNId| 合作夥伴的 Microsoft 合作夥伴網路識別碼 |
|PartnerName|   夥伴名稱 |
|PartnerLocation|   合作夥伴的地理位置 |
|PartnerAttributionType|    訂用帳戶的屬性類型|
|SalesChannel|  銷售 (Direct/CSP 等的通道 )  |
|空位|    目前的可用基座|
|RevenueUSD|    以美元為單位的收益|
|註冊識別碼| 訂用帳戶的註冊識別碼|

**Azure 使用量**： azure 使用量報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|SubscriptionId|    訂用帳戶的 GUID|
|SubscriptionStartDate| 訂用帳戶的開始日期。|
|SubscriptionEndDate|   訂用帳戶結束的日期。|
|SubscriptionState| 訂用帳戶的目前狀態 (Open/Closed/主動/InGrace 期間) |
|Month| 依月份匯總的日期 |
|ServiceName|   Azure 服務的名稱|
|MeterCategory| 計量類別的名稱|
|UsageUnits|    計費週期期間使用的單位數 |
|CustomerName|  客戶的名稱 |
|CustomerTenantId|  客戶的租使用者識別碼 |
|CustomerTpid|  客戶最上層父識別碼 |
|CustomerSegment|   客戶的區段 |
|CustomerMarket|    客戶的地理市場 |
|MPNId  |客戶 Microsoft 合作夥伴網路識別碼 |
|PartnerName|   夥伴名稱 |
|PartnerLocation    |合作夥伴的地理國家/地區位置 |
|PartnerAttributionType |夥伴的屬性類型|
|SalesChannel|  銷售的 Channel (直接/CSP 間接/CSP 直接存取等 )  |
|ACR_USD|   Azure 耗用的收入（美元）|
|註冊識別碼| Azure 訂用帳戶的註冊識別碼|

**Office 365-授權使用方式**： Office 365 授權使用量報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerTenantId|  客戶的租使用者識別碼| 
|CustomerTpid|  客戶最上層父識別碼 |
|WorkloadName|  Sfb、小組、EXO |
|Month| 回報使用量的月份|
|PaidAvailableUnits|    付費的可用單位數|
|MonthlyActiveUsers|    每月作用中使用者數目|
|CustomerName|  客戶的名稱|
|CustomerMarket|    客戶市場的地理位置 |
|CustomerSegment|   客戶區段 |
|MPNId| Microsoft 合作夥伴網路識別碼|
|PartnerName|   夥伴名稱|
|PartnerLocation|   合作夥伴的地理位置|
|PartnerAttributionType|    夥伴的屬性類型|

**企業行動力–授權使用** 方式： EMS 的各種欄位的資料定義–授權使用量報表：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerTenantId|  客戶的租使用者識別碼| 
|CustomerTpid|  客戶最上層父識別碼 |
|WorkloadName|  EMS 工作負載的名稱 |
|Month| 回報使用量的月份|
|PaidAvailableUnits|    付費的可用單位數|
|MonthlyActiveUsers|    每月作用中使用者數目|
|CustomerName|  客戶的名稱|
|CustomerMarket|客戶市場的地理位置 |
|CustomerSegment|   客戶區段 |
|MPNId| Microsoft 合作夥伴網路識別碼|
|PartnerName|   夥伴名稱|
|PartnerLocation|   合作夥伴的地理位置|
|PartnerAttributionType|    夥伴的屬性類型|

**Dynamics 365 –授權使用** 方式： dynamics 365 的各種欄位的資料定義–授權使用量報表：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|SubscriptionId|訂用帳戶的 GUID|
|SubscriptionStartDate| 訂用帳戶的開始日期|
|SubscriptionEndDate|   訂用帳戶的結束日期|
|SubscriptionStatus|    訂用帳戶的狀態 |
|Month| 回報使用量的月份|
|RevSumDivisionName|    Rev sum 除法的名稱|
|RevSumCategoryName|    Rev sum 類別目錄的名稱|
|SKU|   產品的 Sku |
|SKUId| 產品的 Sku 識別碼 |
|FreeVsPaidSKU| 指出它是免費或付費的 SKU |
|SalesModel|    用來銷售訂用帳戶的銷售通道|
|DetailedSalesModel|    訂用帳戶的詳細銷售模型|
|CustomerName|  客戶名稱 |
|CustomerTenantId|  客戶租使用者 GUID |
|CustomerTpid|  客戶最上層父系識別碼 |
|CustomerSegment|   客戶的市場部門 |
|CustomerMarket|    客戶的地理市場 |
|MPNId| Microsoft 合作夥伴網路識別碼 |
|PartnerName|   夥伴名稱 |
|PartnerLocation|   合作夥伴的地理國家/地區位置 |
|PartnerAttachType| 訂用帳戶的屬性類型|
|空位|    目前的可用基座|
|AssignedSeats| 目前指派的基座 |
|ActiveSeats|   目前作用中基座 |
|DeploymentOpportunity| 目前的部署機會|
|ActiveUsagePercent|    目前作用中的使用量百分比|
 
**Power BI 授權使用** 方式： Power BI 的各種欄位的資料定義–授權使用方式報表：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|SubscriptionId|    訂用帳戶的 GUID|
|SubscriptionStartDate| 訂用帳戶的開始日期|
|SubscriptionEndDate|   訂用帳戶的結束日期|
|SubscriptionStatus|    訂用帳戶的狀態 (作用中或 In-Active 或在寬限期內) |
|Month| 依月份匯總的日期 |
|SKU|   產品的 Sku |
|SKUId| 產品的 Sku 識別碼 |
|FreeVsPaidSKU| 免費或付費 Sku 的區別 |
|SalesModel|    用來銷售訂用帳戶的銷售模型|
|DetailedSalesModel|    訂用帳戶的詳細銷售模型|
|CustomerName|  客戶名稱 |
|CustomerTenantId|  客戶租使用者 GUID |
|CustomerTpid|  客戶最上層父系識別碼| 
|CustomerSegment|   客戶的市場部門 |
|CustomerMarket|    客戶的地理市場 |
|MPNId| Microsoft 合作夥伴網路識別碼 |
|PartnerName|   夥伴名稱 |
|PartnerLocation|   合作夥伴的地理國家/地區位置 |
|PartnerAttachType| 訂用帳戶的屬性類型|
|空位|    目前的可用基座|
|AssignedSeats| 目前指派的基座|
|ActiveSeats|   目前作用中基座|
|DeploymentOpportunity| 目前的部署機會|
|ActiveUsagePercent|    目前作用中的使用量百分比|

**小組使用方式–會議和通話**：各種欄位的資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerTenantId|  客戶的租使用者識別碼 |
|CustomerTpid|  客戶最上層父識別碼 |
|Month| 回報使用量的月份|
|Subworkload|    (會議、電話、電話系統報告使用量的子工作負載) |
|會議計數| 會議數目|
|會議持續時間|  總會議持續時間（小時）|

**小組-每月使用量詳細** 資料：各種欄位的資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerTenantId|  客戶的租使用者識別碼 |
|CustomerTpid|  客戶最上層父識別碼 |
|Month| 回報使用量的月份|
|Subworkload|    (會議、電話、電話系統報告使用量的子工作負載) |
|桌面使用者| 在桌面上使用小組的使用者數目|
|行動裝置使用者|  在行動裝置上使用小組的使用者數目|
|Web 使用者| 在 Web 上使用小組的使用者數目|
|AllUpParticipants| 每月小組的不同使用者數目|

**小組使用方式– 3 p apps**：各種欄位的資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CustomerTenantId|  客戶的租使用者識別碼| 
|CustomerTpid|  客戶最上層父識別碼 |
|Month| 回報使用量的月份|
|3 P 應用程式名稱|   小組應用程式的名稱|
|使用者計數|    應用程式的使用者數目|


**定型詳細** 資料：訓練詳細資料包表的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|TrainingActivityId|    定型的識別碼 |
|TrainingTitle| 訓練的標題 |
|TrainingType|   (認證/測驗) 的訓練類型|
|IndividualFirstName|   客戶的名字| 
|IndividualLastName|    客戶的姓氏| 
|電子郵件| 客戶的個人電子郵件識別碼|
|CorpEmail| 客戶的 Office 電子郵件識別碼|
|TrainingCompletionDate|    定型的完成日期 |
|Month| 報告資料的月份|
|IcMCP| 指出使用者是否為 Microsoft 認證專業人員|
|MCPID| 使用者的 MCP 識別碼|
|MPNId| Microsoft 合作夥伴網路識別碼 |
|PartnerName|   夥伴名稱 |
|PartnerCityLocation|   合作夥伴的地理城市位置 |
|PartnerCountryLocation|    合作夥伴的地理國家/地區位置 |

**Microsoft Learn**： Microsoft Learn 報表之各種欄位的資料定義為：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|使用者名稱|使用者名稱| 
|UserId|使用者 GUID |
|TrainingName|定型的名稱 |
|TrainingType|定型類型 (模組/Learning 路徑) |
|產品|學習模組適用的產品|
|角色|定型的適用角色 |
|CompletionDate|定型完成的日期 |
|MPNId|Microsoft 合作夥伴網路識別碼 |
|PartnerName|夥伴名稱 |
|國家/地區|合作夥伴的地理國家/地區位置 |

專長 **認證摘要和歷程記錄**：專長認證摘要和歷程記錄報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CompetencyName|專長認證的名稱 |
|CompetencyLevel|專長認證 (金級/Silver) |
|CompetencyStatus|專長認證 (主動式/非使用中/處於寬限期) 的目前狀態|
|CompetencyStartDate|指定專長認證的開始日期| 
|CompetencyEndDate|指定專長認證的結束日期 |

專長 **認證效能**：專長認證效能報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|CompetencyName|    專長認證的名稱 |
|CompetencyAttainmentOptionName|    專長認證達到選項的名稱|
|Month| 報告計量的月份|
|MetricName|    與專長認證相關的度量名稱|
|MetricMonthlyContribution| 度量的每月貢獻|
|TTMAggregate|  過去12個月的匯總度量|
|AnniversaryYearAggregate|  目前周年年度的匯總度量|
|GoldThreshold| 符合金級專長認證的效能需求|
|SilverThreshold|   符合銀級專長認證的效能需求|

**雲端上升-M365 傾向**：雲端上升-M365 傾向報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|MPN 識別碼|    Microsoft 合作夥伴網路識別碼|
|[合作夥伴名稱]|  夥伴名稱|
|客戶識別碼|   客戶識別碼 |
|DUNS 號碼|   Dun & Bradstreet 為傾向評分的客戶數目|
|帳戶名稱|  帳戶的名稱 |
|網域|    帳戶的網域|
|組織大小|  組織的大小|
|產業|  產業  |
|Vertical|  由 Microsoft 和其他產業標準 (D&B 所識別的客戶的垂直傾向) |
|區域|  位置的地理區域|
|子公司|    客戶的子公司正在進行傾向評分|
|Sales Territory|   客戶的銷售領域正在進行傾向評分|
|City|  地理城市位置 |
|州| 地理狀態位置|
|郵遞區號|   郵遞區號|
|國家/地區|   地理國家/地區位置 |
|區段|   市場區段 |
|子區段|   市場子區段 |
|SMC 類型摘要|  SMC 型別 |
|最上層非受控-計算基礎|  熱門未受管理的客戶-計算|
|最上層非受控-使用者基底| 熱門未受管理的客戶-使用者|
|IsNonProfit|   非收益或收益 (是/否) |
|啟用遠端工作-目標 Exchange Online|   具有有效 exchange online 訂用帳戶的客戶，加入至 M365|
|使用 CLAS 傾向-+ 10 授權啟用 (目前版本) 的遠端內部部署取得|具有目前內部部署辦公室或 Win 用戶端的客戶 (也就是在 EOS 產品) 之後的版本。 客戶有10個以上的授權。 具有傾向分數的客戶。 夥伴應以轉換為 M365 的目標。|
|使用 CLAS 傾向來啟用 (目前版本) 的遠端內部部署取得 <10 授權|具有目前內部部署辦公室或 Win 用戶端的客戶 (也就是在 EOS 產品) 之後的版本。 客戶的授權少於10個。 具有傾向分數的客戶。 夥伴應以轉換為 M365 的目標。|
|啟用 (目前版本) 的遠端內部部署取得，而不使用 CLAS 傾向-+ 10 授權| 具有目前內部部署辦公室或 Win 用戶端的客戶 (也就是在 EOS 產品) 之後的版本。 客戶有10個以上的授權。 客戶沒有傾向分數。 夥伴應以轉換為 M365 的目標。|
|啟用 (目前版本) 的遠端內部部署取得，而不使用 CLAS 傾向-<10 授權| 具有目前內部部署辦公室或 Win 用戶端的客戶 (也就是在 EOS 產品) 之後的版本。 客戶的授權少於10個。 客戶沒有傾向分數。 夥伴應以轉換為 M365 的目標。|
|使用 CLAS 傾向-+ 10 授權啟用 (EOS) 的遠端內部部署收購|具有 EOS 內部內部部署辦公室或 Win 用戶端的客戶 (也就是在和包含 EOS 產品之前的版本。 客戶有10個以上的授權。 客戶有傾向分數。 夥伴應以轉換為 M365 的目標。|
|使用 CLAS 傾向來啟用 (EOS) 的遠端內部部署收購-<10 授權|具有 EOS 內部內部部署辦公室或 Win 用戶端的客戶 (也就是在和包含 EOS 產品之前的版本。 客戶的授權少於10個。 客戶有傾向分數。 夥伴應以轉換為 M365 的目標。|
|啟用 (EOS) 的遠端內部部署取得（不含 CLAS 傾向）-+ 10 授權| 具有目前內部內部部署辦公室或贏得客戶 (的客戶，也就是) 之前的版本，以及包含 EOS 產品的版本。 客戶有10個以上的授權。 客戶沒有傾向分數。 夥伴應以轉換為 M365 的目標。|
|在沒有 CLAS 傾向的情況下，啟用 (EOS) 的遠端內部部署收購-<10 授權| 具有目前內部內部部署辦公室或贏得客戶 (的客戶，也就是) 之前的版本，以及包含 EOS 產品的版本。 客戶的授權少於10個。 客戶沒有傾向分數。 夥伴應以轉換為 M365 的目標。|
|啟用遠端工作-M365 的高傾向潛在客戶 (立即行動/評估) | 具有 high 傾向 for M365 的潛在客戶客戶。|
|啟用遠端工作-使用 M365 進行 (縮放) 競爭| 具有縮放和 M365 的客戶，以轉換為小組的目標|
|啟用遠端工作-在沒有 M365 的情況下競爭 (縮放) |  具有縮放的客戶，以轉換為目標的團隊|
|降低 M365 E5 目標的成本和管理 M365 E3| 具有 M365 E3 的現有客戶，適用于 M365 E5 的目標|
|降低以 M365 BP 為目標的 M365 BB 和 BS 客戶的成本和管理|    現有的 M365 BB 和 BS 客戶，將這些客戶的目標設為 M365 BP|
|轉換組織生產力-Surface 傾向|    客戶顯示 Surface 的傾向。|
|M365Cluster|識別客戶要購買 M365 的傾向。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|M365Fit|   定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|M365Intent|    社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|SurfaceCluster|    這會藉由將符合和意圖建議合併到叢集中，來識別客戶的購買面傾向。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|SurfaceFit|    定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|SurfaceIntent| 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|O365Cluster|   這會識別客戶的傾向以購買 O365。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|O365Fit|   定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|O365Intent|    社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|M365UpsellCustomer|    這會識別客戶是否顯示 M365 的追加銷售傾向|
|有 Google|    此旗標會識別客戶是否顯示擁有 Google 產品的競爭信號|
|具有 AWS|   此旗標會識別客戶是否顯示擁有 AWS 產品的競爭信號|
|具有 EA|    這會識別更新是否為 (EA) 或 EA 訂用帳戶的 enterprise 合約|
|已開啟|  這會識別更新是開啟或開啟值的合約|

**雲端上升-D365 傾向**：雲端上升-D365 傾向報告的各種欄位資料定義如下：

| **資料行名稱** | **資料描述** |
|---------|:---------|
|MPN 識別碼|    Microsoft 合作夥伴網路識別碼|
|[合作夥伴名稱]|  夥伴名稱|
|客戶識別碼|   客戶識別碼 |
|DUNS 號碼|   Dun & Bradstreet 為傾向評分的客戶數目|
|帳戶名稱|  帳戶的名稱 |
|網域|    帳戶的網域|
|組織大小|  組織的大小|
|產業|  產業  |
|Vertical|  由 Microsoft 和其他產業標準 (D&B 所識別的客戶的垂直傾向) 
|區域|  位置的地理區域|
|子公司|    客戶的子公司正在進行傾向評分|
|Sales Territory|   Sales Territory|
|City|  地理城市位置 |
|州| 地理狀態位置|
|郵遞區號|   郵遞區號|
|國家/地區|   地理國家/地區位置 |
|區段|   市場區段 |
|子區段|   市場子區段 |
|SMC 類型摘要|  客戶的分類：熱門未受管理的使用者群是具有300位以上員工的客戶、最上層未受管理的計算基底是在 Azure 3 年期內有 $ 10k 的客戶、中型企業是有25位員工或更高的客戶|
|最上層非受控-計算基礎   |熱門未受管理的客戶-計算|
|最上層非受控-使用者基底| 熱門未受管理的客戶-使用者|
|IsNonProfit|   非收益或收益 (是/否) |
|啟用數位銷售-M365-基座大小 >= 25 基座 (SalesPro 傾向模型) |   不具 D365 的客戶。 基座大小： 25 +。 合作夥伴應以 D365 Salespro 的交叉銷售為目標|
|啟用數位銷售-D365 SalesPro 傾向 (立即行動/評估)  |沒有 D365 的高傾向客戶。  合作夥伴應以 D365 SalesPro 為目標。|
|管理金融風險 & 詐騙-Dynamics 內部內部部署安裝 Navision (BC 傾向模型) |具有內部部署 Navision 的現有客戶。  合作夥伴應針對 D365 BC 設定目標|
|管理金融風險 & 詐騙-Dynamics 內部內部部署安裝基礎-AX (F&O 傾向模型)     |具有內部部署 AX 的現有客戶。  夥伴應以 D365 F&O 為目標|
|管理金融風險 & 詐騙-Dynamics 內部內部部署安裝基礎-絕佳 Plains (BC 傾向模型) |  具有內部部署絕佳 Plains 的現有客戶。  合作夥伴應針對 D365 BC 設定目標|
|管理金融風險 & 詐騙-Dynamics 內部內部部署安裝基礎-索羅門群島 (BC 傾向模型) |具有內部部署索羅門群島的現有客戶。  合作夥伴應針對 D365 BC 設定目標|
|管理金融風險 & 詐騙-Dynamics 內部內部部署安裝基礎-其他 (BC 傾向模型)  |先前未列出其他內部部署解決方案的現有客戶。  合作夥伴應針對 D365 BC 設定目標|
|打造 Agile 商務程式-Dynamics 內部內部部署安裝 Base-AX/GP/SL/NAV/Other (D365 傾向模型) |   打造 Agile 商務程式-Dynamics 內部內部部署安裝 Base-AX/GP/SL/NAV/Other (D365 傾向模型) |
|打造 Agile 商務程式-Dynamics Mendix/Outsystems/Salesforce (D365 傾向 Model) | 打造 Agile 商務程式-Dynamics Mendix/Outsystems/Salesforce (D365 傾向 Model) |
|打造 Agile 商務程式-D365 F&O Install Base |現有的 D365 F&O 客戶。  目標 Power Apps 的夥伴。|
|打造 Agile 商務程式-D365 BC Install Base| 現有的 D365 BC 客戶。 目標 Power Apps 的夥伴。|
|打造 Agile 商務程式-D365 CE 安裝基底| 現有的 D365 CE 客戶。 目標 Power Apps 的夥伴。|
|打造具復原性的供應鏈-贏得並以非 Oracle/SAP ERP 客戶的 D365 供應鏈的形式啟用第一個 D365 工作負載|  D365 供應鏈的目標客戶。|
|打造具彈性的供應鏈-跨銷售 D365 供應鏈及/或零售/商務至現有的 D365 CE 客戶 |現有的 D365 CE 客戶，適用于跨銷售 D365 供應鏈的目標|
|建立具恢復功能的供應鏈-交叉銷售 D365 Sup。 D365 CE 及 (Oracle 或 SAP) 的連鎖及/或零售/商務| 具有 Oracle 或 SAP 的現有 D365 CE 客戶可針對 D365 供應鏈設定目標|
|D365BCCluster| 這會識別客戶的傾向，以購買 D365 Business Central。  顯示傾向 for BC 的客戶將會處於「中」和「小型」類別中。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365BCFit| 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|D365BCIntent|  社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|D365FOCluster| 這會識別客戶用來購買 D365 財務和作業的傾向。  針對 F&O 顯示傾向的客戶將會在最上層的非受控類別中。 叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365FOFit| 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|D365FOIntent|  社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|D365CECluster| 這會識別客戶的傾向，以購買 D365 Customer Engagement。  顯示傾向 for CE 的客戶將會處於「中」和「小型」類別中。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365CEFit| 適用于 D365 CE|
|D365CEIntent|  D365 CE 的意圖|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  這會識別客戶是否有 Dynamics 內部內部部署 AX 或 CRM 的 open 續訂。|
|M365UpsellCustomer|    這會識別客戶是否顯示 M365 的追加銷售傾向|
|有 Google|    此旗標會識別客戶是否顯示擁有 Google 產品的競爭信號|
|具有 AWS|   此旗標會識別客戶是否顯示擁有 AWS 產品的競爭信號|
|具有 EA |這會識別更新是否為 (EA) 或 EA 訂用帳戶的 enterprise 合約|
|已開啟|  這會識別更新是開啟或開啟值的合約|

**Cloud Ascent-Azure 傾向**： Cloud Ascent-Azure 傾向報告的各種欄位資料定義如下：

|**資料行名稱** |**資料描述** |
|---------|:---------|
|MPN 識別碼|    Microsoft 合作夥伴網路識別碼|
|[合作夥伴名稱]|  夥伴名稱|
|客戶識別碼|   客戶識別碼 |
|DUNS 號碼|   Dun & Bradstreet 為傾向評分的客戶數目|
|帳戶名稱|  帳戶的名稱 |
|網域|    帳戶的網域|
|組織大小|  組織的大小|
|產業|  產業  |
|Vertical|  由 Microsoft 和其他產業標準 (D&B 所識別的客戶的垂直傾向) |
|區域|  位置的地理區域|
|子公司|    客戶的子公司正在進行傾向評分|
|Sales Territory|   Sales Territory|
|City|  地理城市位置 |
|州| 地理狀態位置|
|郵遞區號|   郵遞區號|
|國家/地區|   地理國家/地區位置 |
|區段|   市場區段 |
|子區段|   市場子區段 |
|SMC 類型摘要|  SMC 型別 |
|最上層非受控-計算基礎|  熱門未受管理的客戶-計算|
|最上層非受控-使用者基底| 熱門未受管理的客戶-使用者|
|IsNonProfit|   非收益或收益 (是/否) |
|遷移-EOS Win Server-EOS Windows Server IB 與 CLAS 傾向-5 + 授權|   具有 EOS 內部內部部署 Win Server 的客戶 (也就是在) 之前的版本，以及包含 EOS 產品的版本。 客戶有5個或更多的授權。 具有傾向分數的客戶。  合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS Win Server-EOS Windows Server IB 與 CLAS 傾向-<5 授權|   具有 EOS (終止服務的客戶) 內部內部部署 Win Server (也就是在) 之前的版本，以及包含 EOS 產品。 客戶的授權少於5個。 具有傾向分數的客戶。  合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS Win Server-不含 CLAS 傾向的 Windows Server IB-5 + 授權 |具有 EOS 內部內部部署 Win Server 的客戶 (也就是在) 之前的版本，以及包含 EOS 產品的版本。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS Win Server-無 CLAS 傾向的 Windows Server IB-<5 授權|    具有 EOS 內部內部部署 Win Server 的客戶 (也就是在) 之前的版本，以及包含 EOS 產品的版本。 具有少於5個授權。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|使用 CLAS 傾向-5 + 授權遷移-EOS SQL-EOS SQL Server IB|  具有 EOS 內部內部部署 SQL Server 的客戶 (也就是，在) 之前的版本，包括的 EOS 產品。 客戶有5個以上的授權。 客戶有傾向分數。  合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS SQL-EOS SQL Server IB with CLAS 傾向-<5 授權|  具有 EOS 內部內部部署 SQL Server 的客戶 (也就是，在) 之前的版本，包括的 EOS 產品。 具有少於5個授權。 具有傾向分數的客戶。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS SQL-EOS SQL Server IB 而不 CLAS 傾向-5 + 授權|   具有 EOS 內部內部部署 SQL Server 的客戶 (也就是，在) 之前的版本，包括的 EOS 產品。 客戶有5個或更多的授權。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-EOS SQL-EOS SQL Server IB 但不 CLAS 傾向-<5 授權|   具有 EOS 內部內部部署 SQL Server 的客戶 (也就是，在) 之前的版本，包括的 EOS 產品。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移內部內部部署 Win Server-目前的 Windows Server IB 與 CLAS 傾向-5 個以上的授權|   具有目前內部內部部署 Win Server (也就是在 EOS 產品) 之後版本的客戶。 客戶有5個以上的授權。 客戶有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移內部內部部署 Win Server-目前的 Windows Server IB 與 CLAS 傾向-<5 授權|   具有目前內部內部部署 Win Server (也就是在 EOS 產品) 之後版本的客戶。 客戶的授權少於5個。 客戶的 Azure 傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移內部內部部署 Win Server-目前的 Windows Server IB （未 CLAS 傾向）-5 個以上的授權|    具有目前內部內部部署 Win Server (也就是在 EOS 產品) 之後版本的客戶。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移內部內部部署 Win Server-目前的 Windows Server IB （不含 CLAS 傾向）-<5 授權 |具有目前內部內部部署 Win Server (也就是在 EOS 產品) 之後版本的客戶。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移至 Azure SQL 或 SQL Vm-目前的 SQL Server IB 與 CLAS 傾向-5 個以上的授權|  目前內部部署 SQL Server 的客戶 (也就是在 EOS 產品) 之後的版本。 客戶有5個以上的授權。 客戶有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移至 Azure SQL 或 SQL Vm-目前 SQL Server IB 與 CLAS 傾向-<5 授權|  目前內部部署 SQL Server 的客戶 (也就是在 EOS 產品) 之後的版本。 客戶的授權少於5個。 客戶有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移至 Azure SQL 或 SQL Vm-目前的 SQL Server IB （沒有 CLAS 傾向）-5 個以上的授權|   目前內部部署 SQL Server 的客戶 (也就是在 EOS 產品) 之後的版本。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-遷移至 Azure SQL 或 SQL Vm-目前的 SQL Server IB 而不 CLAS 傾向-<5 授權|   目前內部部署 SQL Server 的客戶 (也就是在 EOS 產品) 之後的版本。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-OSS-遷移至 OSS DB| 具有下列任一項競爭產品的現有客戶：于 postgresql、MySQL、適用于 mariadb。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-OSS-Azure 上的 Linux |具有產品的現有客戶： Linux。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-SAP-Azure 上的 SAP|  具有產品的現有客戶： SAP。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-WVD-RDS IB |識別使用中 Windows 遠端桌面服務的客戶。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-WVD-跨銷售現代化工作至 Azure/WVD|   識別具有 M365 的客戶，但沒有 Azure。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-VMware IB|   產品的現有客戶： VMware。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|遷移-Citrix IB|   具有產品的現有客戶： Citrix 系統。 合作夥伴應以這些客戶為目標，以遷移至 Azure。|
|創新-分析-Power BI IB （含高 Azure 傾向）|   具有和使用中 Power BI 訂用帳戶的客戶，包括： Power BI 獨立 Pro、Power BI-Azure 套件、Power BI Office 套件、Power BI 套件-M365|
|啟用-DevOps 與 GitHub-VisualStudio/MSDN IB|    使用活躍的 visual studio 識別的客戶|
|Win Server Standard 版本|   這會顯示客戶購買的 Windows Server Standard 版本|
|Win Server Standard 授權|   這會顯示客戶的 Windows Server Standard 購買授權類型|
|Win Server 資料中心版本|    這會顯示客戶購買的 Windows 資料中心版本|
|Win Server 資料中心授權| 這會顯示客戶購買的 Windows 資料中心授權類型|
|AzureFit|  定義 firmographics 的內部和外部資料點。 [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。 每季更新評分。|
|AzureIntent|   社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會重迭在適合定義叢集的最上層。 意圖評分會每月更新。|
|AzureCluster|  這會藉由將符合和意圖建議合併到叢集中，來識別客戶購買 Azure 的傾向。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|WindowsServerDataCenter_HasOpenRenewal|    這會識別客戶是否有 windows server 資料中心的開啟續約|
|WindowsServerStandard_HasOpenRenewal|  這會識別客戶是否有 windows server standard 的 open 續約|
|AzureUpsellCustomer|   這會識別客戶是否顯示 Azure 的追加銷售傾向|
|有 Google|    此旗標會識別客戶是否顯示擁有 Google 產品的競爭信號|
|具有 AWS|   此旗標會識別客戶是否顯示擁有 AWS 產品的競爭信號|
|具有 EA |這會識別更新是否為 (EA) 或 EA 訂用帳戶的 enterprise 合約|
|已開啟|  這會識別更新是開啟或開啟值的合約|

**雲端 Ascent-Agreement 續約傾向**：雲端高階合約續約傾向報告的各種欄位資料定義如下：

|**資料行名稱** |**資料描述** |
|---------|:---------|
|MPN 識別碼|    Microsoft 合作夥伴網路識別碼|
|[合作夥伴名稱]|  夥伴名稱|
|客戶識別碼|   客戶識別碼 |
|DUNS 號碼|   Dun & Bradstreet 為傾向評分的客戶數目|
|帳戶名稱|  帳戶的名稱 |
|網域|    帳戶的網域|
|組織大小|  組織的大小|
|產業|  產業  |
|Vertical|  由 Microsoft 和其他產業標準 (D&B 所識別的客戶的垂直傾向) |
|區域|  位置的地理區域|
|子公司|    客戶的子公司正在進行傾向評分|
|Sales Territory|   Sales Territory|
|City|  地理城市位置 |
|州| 地理狀態位置|
|郵遞區號|   郵遞區號|
|國家/地區|   地理國家/地區位置 |
|區段|   市場區段 |
|子區段|   市場子區段 |
|SMC 類型摘要|  SMC 型別 |
|最上層非受控-計算基礎|  熱門未受管理的客戶-計算|
|最上層非受控-使用者基底| 熱門未受管理的客戶-使用者|
|IsNonProfit|非收益或收益 (是/否) |
|有 Google|此旗標會識別客戶是否顯示擁有 AWS 產品的競爭信號|
|具有 AWS|此旗標會識別客戶是否顯示擁有 AWS 產品的競爭信號|
|Azure 叢集|這會識別客戶購買 Azure 的傾向。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365 F&O Cluster|  這會識別客戶用來購買 D365 財務和作業的傾向。  針對 F&O 顯示傾向的客戶將會在最上層的非受控類別中。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365 CE 叢集|   這會識別客戶的傾向，以購買 D365 Customer Engagement。  顯示傾向 for CE 的客戶將會處於「中」和「小型」類別中。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|D365 BC 叢集|   這會識別客戶的傾向，以購買 D365 Business Central。  顯示傾向 for BC 的客戶將會處於「中」和「小型」類別中。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|M365 叢集|  這會識別客戶要購買 M365 的傾向。  叢集立即行動和評估應以其為目標，因為它們會產生更高的產量。  培養並教育客戶只有在目標為 [立即行動] 和 [評估客戶] 之後仍有容量時，才應將其設為目標。|
|授權方案|   這會識別續約的授權方案類型|
|協議識別碼|  合約識別碼|
|[合約結束日期]|    [合約結束日期] |
|到期類型|   到期的類型|
|收入即將過期|  與過期訂用帳戶相關聯的收益|
|具有 EA|    這會識別更新是否為 (EA) 或 EA 訂用帳戶的 enterprise 合約|
|已開啟|  這會識別更新是開啟或開啟值的合約|
|Azure 追加銷售客戶| 這會識別客戶是否顯示 Azure 的追加銷售傾向|
|M365 向上銷售客戶|  這會識別客戶是否顯示 M365 的追加銷售傾向|
|RevSumDivisionName|    這會識別要更新的產品|

## <a name="next-steps"></a>後續步驟

針對報表，請參閱 [下載報表](pci-download-reports.md)。
