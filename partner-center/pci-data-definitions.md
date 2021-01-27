---
title: 深入解析資料定義
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 此檔會列出各種報表及其資料定義，您可以從 [見解下載報表] 頁面下載這些報表。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861388"
---
# <a name="export--data-definitions"></a>匯出–資料定義 

 **適當的角色** 

- 報告檢視人員 
- 高階報告檢視人員 

## <a name="introduction"></a>簡介 

您可以使用 [深入解析] 儀表板上的 [下載報表] 中樞來匯出原始資料集。 

下表列出各種可供您下載的報表，以及其資料定義： 

### <a name="partner-profile-report"></a>**夥伴設定檔報告**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| MPNId | Microsoft 合作夥伴網路 (MPN 的識別碼)  | 
| PartnerName | 夥伴名稱 | 
| PGA_MPNId | 合作夥伴通用帳戶 MPN 的識別碼 | 
| PGA_PartnerName | 合作夥伴通用帳戶名稱 | 
| City | 合作夥伴的城市位置 | 
| Country | 合作夥伴的國家/地區位置 | 
| HierarchyLevel | 指出它是否為全域 MPN 識別碼或位置 MPN 識別碼 | 

### <a name="customer-details-report"></a>**客戶詳細資料包表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerName | 客戶的名稱 | 
| CustomerTenantId | 客戶租使用者的識別碼 | 
| CustomerTpid | 客戶上層父系的識別碼 | 
| CustomerSegment | 客戶區段 | 
| CustomerMarket | 客戶的地理市場 | 
| CustomerStatus | 客戶狀態 (作用中或非使用中)  | 
| Product | MPN： O365、DYNAMICS 365、Enterprise Mobility + Security、Power BI 或 Microsoft Azure 銷售給客戶的產品 | 
| SKU | 產品 SKU | 
| Month | 回報使用量和收益的月份 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理位置 | 
| PartnerAttributionType | 夥伴的屬性類型 | 
| SalesChannel | 銷售頻道 | 
| 空位 | 可用基座 | 
| RevenueUSD | 美元的收益 | 

### <a name="reseller-performance-report"></a>**轉銷商效能報表**

> [!Note]
> 收益和 ACR 資料僅適用于主管報表檢視器的使用者。

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| ResellerMPNid | 轉售商 Microsoft 合作夥伴網路識別碼 | 
| ResellerName | 轉銷商名稱 | 
| ResellerMarket | 市場轉銷商國家/地區 | 
| IndirectProviderMPNId | 間接提供者的識別碼 Microsoft 合作夥伴網路 | 
| IndirectProviderName | 間接提供者名稱 | 
| Month | 回報使用量和收益的月份 | 
| Product | 產品名稱 | 
| SubscriptionID | 訂用帳戶的識別碼 | 
| 空位 | 可用的基座數目 | 
| AssignedSeats | 指派的基座數目 | 
| BilledRevenueUSD | 以美元計費的收入 | 
| CustomerName | 客戶的名稱 | 
| CustomerTPid | 客戶上層父系的識別碼 | 
| CustomerSegment | 客戶區段 | 
| CustomerMarket | 客戶的地理市場 | 
| ResellerStatus | 轉售商狀態 | 

### <a name="subscription-details-report"></a>**訂用帳戶詳細資料包表**

>[!Note]
>收益和 ACR 資料僅適用于主管報表檢視器的使用者。

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| SubscriptionId | 訂用帳戶的 GUID | 
| SubscriptionStartDate | 訂用帳戶的開始日期 | 
| SubscriptionEndDate | 訂用帳戶的結束日期 | 
| SubscriptionState | 訂用帳戶的狀態 (Active 或流失)  | 
| Month | 回報使用量和收益的月份 | 
| IsAutoRenew | 指出訂用帳戶是否 autorenew (是或否)  | 
| CustomerName | 客戶的名稱 | 
| CustomerTenantId | 客戶的 GUID | 
| CustomerTpid | 客戶最上層父系識別碼 | 
| CustomerSegment | 客戶的市場部門 | 
| CustomerMarket | 客戶的地理市場 | 
| Product | 合作夥伴銷售給客戶的產品 | 
| SKU | 產品的 SKU | 
| MPNId | 合作夥伴的 Microsoft 合作夥伴網路識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理位置 | 
| PartnerAttributionType | 訂用帳戶的屬性類型 | 
| SalesChannel | 銷售-直接、CSP (雲端解決方案提供者) 等的通道 | 
| 空位 | 目前的可用基座 | 
| RevenueUSD | 美元的收益 | 
| 註冊識別碼 | 訂用帳戶的註冊識別碼 | 

### <a name="azure-usage-report"></a>**Azure 使用量報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| SubscriptionId | 訂用帳戶的 GUID | 
| SubscriptionStartDate | 訂用帳戶開始日期 | 
| SubscriptionEndDate | 訂用帳戶結尾的日期 | 
| SubscriptionState | 訂用帳戶的目前狀態 (開啟、關閉、使用中或在寬限期內)  | 
| Month | 依月份匯總的日期 | 
| ServiceName | Azure 服務的名稱 | 
| MeterCategory | 計量類別的名稱 | 
| UsageUnits | 計費週期期間使用的單位數 | 
| CustomerName | 客戶的名稱 | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶最上層父識別碼 | 
| CustomerSegment | 客戶的區段 | 
| CustomerMarket | 客戶的地理市場 | 
| MPNId | 客戶 Microsoft 合作夥伴網路識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理國家/地區位置 | 
| PartnerAttributionType | 夥伴的屬性類型 | 
| SalesChannel | 銷售的通道 (Direct/CSP、間接/CSP、Direct 等)  | 
| ACR_USD | Azure 耗用的 (ACR) 美元的收入 | 
| 註冊識別碼 | Azure 訂用帳戶的註冊識別碼 | 

### <a name="office-365-license-usage-report"></a>**Office 365 授權使用方式報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶最上層父識別碼 | 
| WorkloadName | 商務用 Skype、小組、Exchange Online | 
| Month | 回報使用量的月份 | 
| PaidAvailableUnits | 付費的可用單位數 | 
| MonthlyActiveUsers | 每月作用中使用者數目 | 
| CustomerName | 客戶的名稱 | 
| CustomerMarket | 客戶市場的地理國家/地區位置 | 
| CustomerSegment | 客戶區段 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理位置 | 
| PartnerAttributionType | 夥伴的屬性類型 | 

### <a name="enterprise-mobility-license-usage-report"></a>**企業行動授權使用量報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶最上層父識別碼 | 
| WorkloadName | Enterprise Mobility + Security (EMS) 工作負載的名稱 | 
| Month | 回報使用量的月份 | 
| PaidAvailableUnits | 付費的可用單位數 | 
| MonthlyActiveUsers | 每月作用中使用者數目 | 
| CustomerName | 客戶的名稱 | 
| CustomerMarket | 客戶市場的地理國家/地區位置 | 
| CustomerSegment | 客戶區段 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理位置 | 
| PartnerAttributionType | 夥伴的屬性類型 | 

### <a name="dynamics-365-license-usage-report"></a>**Dynamics 365 授權使用方式報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| SubscriptionId | 訂用帳戶的 GUID | 
| SubscriptionStartDate | 訂用帳戶的開始日期 | 
| SubscriptionEndDate | 訂用帳戶的結束日期 | 
| SubscriptionStatus | 訂用帳戶的狀態 | 
| Month | 回報使用量的月份 | 
| RevSumDivisionName | Rev sum 除法的名稱 | 
| RevSumCategoryName | Rev sum 類別目錄的名稱 | 
| SKU | 產品的 SKU | 
| SKUId | 產品的 SKU 識別碼 | 
| FreeVsPaidSKU | 指出是免費或付費的 SKU | 
| SalesModel | 用來銷售訂用帳戶的銷售通道 | 
| DetailedSalesModel | 訂用帳戶的詳細銷售模型 | 
| CustomerName | 客戶的名稱 | 
| CustomerTenantId | 客戶租使用者的 GUID | 
| CustomerTpid | 客戶最上層父系識別碼 | 
| CustomerSegment | 客戶的市場部門 | 
| CustomerMarket | 客戶的地理市場 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理國家/地區位置 | 
| PartnerAttachType | 訂用帳戶的屬性類型 | 
| 空位 | 目前的可用基座 | 
| AssignedSeats | 目前指派的基座 | 
| ActiveSeats | 目前作用中基座 | 
| DeploymentOpportunity | 目前的部署機會 | 
| ActiveUsagePercent | 目前作用中的使用百分比 | 

### <a name="power-bi-license-usage-report"></a>**Power BI 授權使用量報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| SubscriptionId | 訂用帳戶的 GUID | 
| SubscriptionStartDate | 訂用帳戶的開始日期 | 
| SubscriptionEndDate | 訂用帳戶的結束日期 | 
| SubscriptionStatus | 訂用帳戶的狀態 (作用中、非使用中或寬限期)  | 
| Month | 依月份匯總的日期 | 
| SKU | 產品的 SKU | 
| SKUId | 產品的 SKU 識別碼 | 
| FreeVsPaidSKU | 免費或付費 SKU 的區別 | 
| SalesModel | 用來銷售訂用帳戶的銷售模型 | 
| DetailedSalesModel | 訂用帳戶的詳細銷售模型 | 
| CustomerName | 客戶的名稱 | 
| CustomerTenantId | 客戶租使用者的 GUID | 
| CustomerTpid | 客戶上層父系的識別碼 | 
| CustomerSegment | 客戶的市場部門 | 
| CustomerMarket | 客戶的地理市場 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerLocation | 合作夥伴的地理國家/地區位置 | 
| PartnerAttachType | 訂用帳戶的屬性類型 | 
| 空位 | 目前的可用基座 | 
| AssignedSeats | 目前指派的基座 | 
| ActiveSeats | 目前作用中基座 | 
| DeploymentOpportunity | 目前的部署機會 | 
| ActiveUsagePercent | 目前作用中的使用百分比 | 

### <a name="teams-meetings-and-calls-report"></a>**小組會議和通話報告**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶上層父系的識別碼 | 
| Month | 回報使用量的月份 | 
| Subworkload |  (會議、電話或電話系統回報使用方式的 Subworkload)  | 
| 會議計數 | 會議數目 | 
| 會議持續時間 | 總會議持續時間（小時） | 

### <a name="teams-monthly-usage-report"></a>**小組每月使用量報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶上層父系的識別碼 | 
| Month | 回報使用量的月份 | 
| Subworkload |  (會議、電話或電話系統回報使用方式的 Subworkload)  | 
| 桌面使用者 | 在桌面上使用小組的使用者數目 | 
| 行動裝置使用者 | 在行動裝置上使用小組的使用者數目 | 
| Web 使用者 | 在 web 上使用小組的使用者數目 | 
| AllUpParticipants | 每月團隊的唯一使用者數目 | 

### <a name="teams-usage-3p-apps-report"></a>**小組使用 3 P apps 報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CustomerTenantId | 客戶的租使用者識別碼 | 
| CustomerTpid | 客戶最上層父識別碼 | 
| Month | 回報使用量的月份 | 
| 3 P 應用程式名稱 | 小組應用程式的名稱 | 
| 使用者計數 | 應用程式的使用者數目 | 


### <a name="training-details-report"></a>**訓練詳細資料包表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| TrainingActivityId | 定型的識別碼 | 
| TrainingTitle | 訓練的標題 | 
| TrainingType | 訓練類型 (認證或測驗)  | 
| IndividualFirstName | 客戶的名字 | 
| IndividualLastName | 客戶的姓氏 | 
| 電子郵件 | 客戶的個人電子郵件識別碼 | 
| CorpEmail | 客戶的 Office 電子郵件識別碼 | 
| TrainingCompletionDate | 定型的完成日期 | 
| Month | 報告資料的月份 | 
| IcMCP | 指出使用者是否為 Microsoft 認證專業人員 (MCP)  | 
| MCPID | 使用者的 MCP 識別碼 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| PartnerCityLocation | 合作夥伴的地理城市位置 | 
| PartnerCountryLocation | 合作夥伴的地理國家/地區位置 | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn 報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| UserName | 使用者名稱 | 
| UserId | 使用者的 GUID | 
| TrainingName | 定型的名稱 | 
| TrainingType | 定型的類型 (模組或學習路徑)  | 
| 產品 | 學習模組適用的產品 | 
| 角色 | 定型的適用角色 | 
| CompletionDate | 定型完成的日期 | 
| MPNId | Microsoft 合作夥伴網路的識別碼 | 
| PartnerName | 夥伴名稱 | 
| Country | 合作夥伴的地理國家/地區位置 | 

### <a name="competency-summary-and-history-report"></a>**專長認證摘要和歷程記錄報告**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CompetencyName | 專長認證的名稱 | 
| CompetencyLevel | 專長認證 (金級或銀級)  | 
| CompetencyStatus | 專長認證的目前狀態 (作用中、非使用中或寬限期)  | 
| CompetencyStartDate | 專長認證的開始日期 | 
| CompetencyEndDate | 專長認證的結束日期 | 

### <a name="competency-performance-report"></a>**專長認證效能報告**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| CompetencyName | 專長認證的名稱 | 
| CompetencyAttainmentOptionName | 專長認證達到選項的名稱 | 
| Month | 報告計量的月份 | 
| MetricName | 與專長認證相關的度量名稱 | 
| MetricMonthlyContribution | 度量的每月貢獻 | 
| TTMAggregate | 過去12個月的匯總度量 | 
| AnniversaryYearAggregate | 目前周年年度的匯總度量 | 
| GoldThreshold | 符合金級專長認證的效能需求 | 
| SilverThreshold | 符合銀級專長認證的效能需求 | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**雲端上升-Microsoft 365 傾向報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| MPN 識別碼 | Microsoft 合作夥伴網路識別碼 | 
| [合作夥伴名稱] | 夥伴名稱 | 
| 客戶識別碼 | 客戶的識別碼 | 
| DUNS 號碼 | Dun & Bradstreet (D&B) 會計給傾向的客戶數目 | 
| 帳戶名稱 | 帳戶的名稱 | 
| 網域 | 帳戶的網域 | 
| 組織大小 | 組織的大小 | 
| 產業 | 公司所屬的產業 | 
| Vertical | 由 Microsoft、D&B 和其他產業標準所識別的傾向評分之客戶的垂直 | 
| 區域 | 位置的地理區域 | 
| 子公司 | 針對傾向評分的客戶子公司 | 
| Sales Territory | 傾向評分之客戶的銷售領域 | 
| City | 組織的地理城市位置 | 
| 州 | 組織的地理狀態位置 | 
| 郵遞區號 | 組織的郵遞區號 | 
| Country | 組織的地理國家/地區位置 | 
| 區段 | 市場區段 | 
| 子區段 | 市場子細分 | 
| SMC 類型摘要 | SMC 型別 | 
| 最上層非受控-計算基礎 | 熱門未受管理的客戶-計算 | 
| 最上層非受控-使用者基底 | 熱門未受管理的客戶-使用者 | 
| IsNonProfit | 指出組織是否為非收益 (是或否)  | 
| 啟用遠端工作-目標 Exchange Online | 具有有效 Exchange Online 訂用帳戶的客戶，加入 Microsoft 365 | 
| 使用雲端升高傾向-+ 10 授權啟用 (目前版本) 的遠端工作內部部署 | 具有目前內部部署 Office 或 Windows 用戶端的客戶。 也就是說，用戶端版本晚于生命週期結束 (EOL) 版本。 客戶有10個以上的授權。 具有傾向分數的客戶。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 使用雲端升高傾向 (目前的版本) 啟用內部部署的遠端工作-<10 授權 | 具有目前內部部署 Office 或 Windows 用戶端的客戶 (也就是版本晚于 EOL) 。 客戶的授權少於10個。 具有傾向分數的客戶。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 啟用遠端工作-內部部署 (目前的版本) 沒有雲端升高傾向-+ 10 授權 | 具有目前內部部署 Office 或 Windows 用戶端的客戶 (也就是版本晚于 EOL) 。 客戶有10個以上的授權。 客戶沒有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 啟用遠端工作-內部部署取得 (目前版本) 沒有雲端升高傾向-<10 授權 | 具有目前內部部署 Office 或 Windows 用戶端的客戶 (也就是版本晚于 EOL) 。 客戶的授權少於10個。 客戶沒有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 使用雲端升高傾向-+ 10 授權啟用內部部署內部部署 (EOL 版本)  | 具有 EOL 內部部署 Office 或 Windows 用戶端的客戶 (也就是 EOL 版或更早的) 。 客戶有10個以上的授權。 客戶有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 透過雲端升高傾向啟用 (EOL 版本) 的遠端工作內部部署取得 <10 授權 | 具有 EOL 內部部署 Office 或 Windows 用戶端的客戶 (也就是 EOL 版或更早的) 。 客戶的授權少於10個。 客戶有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 啟用遠端工作-內部取得 (EOL 版本) 沒有雲端升高傾向-+ 10 授權 | 具有目前內部部署 Office 或 Windows 用戶端的客戶 (也就是 EOL 版或更早的) 。 客戶有10個以上的授權。 客戶沒有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 啟用遠端工作-內部部署取得 (EOL 版本) 沒有雲端升高傾向-<10 授權 | 具有目前內部部署 Office 或 Windows 用戶端的客戶 (也就是 EOL 版或更早的) 。 客戶的授權少於10個。 客戶沒有傾向分數。 夥伴應以轉換為 Microsoft 365 的目標。 | 
| 針對 Microsoft 365 (Act NowithEvaluate) 啟用遠端工作-高傾向的潛在客戶 | 具有高傾向 Microsoft 365 的潛在客戶客戶 | 
| 啟用遠端工作-與 Microsoft 365 競爭 (縮放)  | 具有縮放和 Microsoft 365 的客戶，以轉換為小組的目標 | 
| 啟用遠端工作-在不 Microsoft 365 的情況下競爭 (縮放)  | 具有縮放的客戶、轉換為小組的目標 | 
| 降低以 Microsoft 365 E5 為目標的成本與管理 Microsoft 365 E3 | 具有 Microsoft 365 E3 的現有客戶，Microsoft 365 E5 的目標 | 
| 降低以 Microsoft 365 商務版 Premium 為目標的基本和企業標準客戶的成本與管理 Microsoft 365 商務版 | 現有 Microsoft 365 商務版基本和企業標準客戶、Microsoft 365 商務版 Premium 的目標 | 
| 轉換組織生產力-Surface 傾向 | 客戶顯示 Surface 的傾向 | 
| M365Cluster | 識別客戶要購買 Microsoft 365 的傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在立即行動並評估客戶為目標之後仍有容量時，才會培養並教育客戶。 | 
| M365Fit | 定義 firmographics 的內部和外部資料點。 「調整評分」會將 lookalike 模型用於我們最適合的小型或中型企業 (Smb) 來比較客戶，並查看是否適合 Microsoft 雲端產品。 每季更新評分。 | 
| M365Intent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| SurfaceCluster | 藉由將符合和意圖建議合併到叢集中，來識別客戶的購買面傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在立即行動並評估客戶為目標之後仍有容量時，才會培養並教育客戶。 | 
| SurfaceFit | 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用 lookalike 模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最佳選擇。 每季更新評分。 | 
| SurfaceIntent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| O365Cluster | 識別客戶購買 Office 365 的傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在立即行動並評估客戶為目標之後仍有容量時，才會培養並教育客戶。 | 
| O365Fit | 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用 lookalike 模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最佳選擇。 每季更新評分。 | 
| O365Intent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| M365UpsellCustomer | 指出客戶是否顯示 Microsoft 365 的追加銷售傾向 | 
| 有 Google | 指出客戶是否顯示擁有 Google 產品的競爭信號 | 
| 具有 AWS | 指出客戶是否顯示擁有 Amazon Web Services (AWS) 產品的競爭信號 | 
| 具有 EA | 識別更新是否為 (EA) 或 EA 訂用帳戶的 enterprise 合約 | 
| 已開啟 | 識別續約為開放或開價值的合約 | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**雲端上升-Dynamics 365 傾向報告**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| MPN 識別碼 | Microsoft 合作夥伴網路識別碼 | 
| [合作夥伴名稱] | 夥伴名稱 | 
| 客戶識別碼 | 客戶識別碼 | 
| DUNS 號碼 | Bradstreet 為傾向評分之客戶的 Dun & 號碼 | 
| 帳戶名稱 | 帳戶的名稱 | 
| 網域 | 帳戶的網域 | 
| 組織大小 | 組織的大小 | 
| 產業 | 公司所屬的產業 | 
| Vertical | 由 Microsoft、D&B 和其他產業標準所識別的傾向評分之客戶的垂直
| 區域 | 位置的地理區域 | 
| 子公司 | 針對傾向評分的客戶子公司 | 
| Sales Territory | 傾向評分之客戶的銷售領域 | 
| City | 地理城市位置 | 
| 州 | 地理狀態位置 | 
| 郵遞區號 | 組織的郵遞區號 | 
| Country | 地理國家/地區位置 | 
| 區段 | 市場區段 | 
| 子區段 | 市場子細分 | 
| SMC 類型摘要 | 客戶的分類：熱門未受管理的使用者群是具有300位以上員工的客戶、最常見的非受控計算基底是客戶，在三年的 Azure 中有 USD10、000、中型企業是有25位員工或更高的客戶，而小型企業是員工人數少於25位的客戶。 | 
| 最上層非受控-計算基礎 | 熱門未受管理的客戶-計算 | 
| 最上層非受控-使用者基底 | 熱門未受管理的客戶-使用者 | 
| IsNonProfit | 指出組織是否為非收益 (是或否)  | 
| 啟用數位銷售-Microsoft 365 基座大小 >= 25 基座 (SalesPro 傾向模型)  | 沒有 Dynamics 365 的客戶。 基座大小： 25 +。 合作夥伴應以 Dynamics 365 SalesPro 的交叉銷售為目標。 | 
| 啟用數位銷售-Dynamics 365 SalesPro 傾向 (立即行動或評估)  | 沒有 Dynamics 365 的高傾向客戶。 合作夥伴應以 Dynamics 365 SalesPro 為目標。 | 
| 管理金融風險 & 詐騙-Dynamics 內部部署安裝 Navision (Business Central 傾向模型)  | 具有內部部署 Navision 的現有客戶。 合作夥伴應以 Dynamics 365 Business Central 為目標。 | 
| 管理金融風險 & 詐騙-Dynamics 內部部署安裝基礎-Dynamics AX (Dynamics 365 財務 + Operations 傾向模型)  | 具有內部部署 AX 的現有客戶。 合作夥伴應以 Dynamics 365 財務 + 作業為目標。 | 
| 管理金融風險 & 詐騙-Dynamics 內部部署安裝基礎-絕佳 Plains (Business Central 傾向模型)  | 具有內部部署絕佳 Plains 的現有客戶。 合作夥伴應以 Dynamics 365 Business Central 為目標。 | 
| 管理金融風險 & 詐騙-Dynamics 內部部署安裝基礎-索羅門群島 (Business Central 傾向模型)  | 具有內部部署索羅門群島的現有客戶。 合作夥伴應以 Dynamics 365 Business Central 為目標。 | 
| 管理財務風險 & 詐騙-Dynamics 內部部署安裝基礎-其他 (Business Central 傾向模型)  | 先前未列出其他內部部署解決方案的現有客戶。 合作夥伴應以 Dynamics 365 Business Central 為目標。 | 
| 打造 Agile 商務程式-Dynamics 內部部署安裝 base-AX/GP/SL/NAV/Other (Dynamics 365 傾向 model)  | 打造 Agile 商務程式-Dynamics 內部部署安裝 base-AX/GP/SL/NAV/Other (Dynamics 365 傾向 model)  | 
| 打造 Agile 商務程式-Dynamics Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model)  | 打造 agile 商務程式-Dynamics Mendix/OutSystems/Salesforce (Dynamics 365 傾向 model)  | 
| 打造 Agile 商務程式-Dynamics 365 財務 + Operations 安裝基礎 | 現有的 Dynamics 365 財務 + 營運客戶。 目標 Power Apps 的夥伴。 | 
| 打造 Agile 商務程式-Dynamics 365 Business Central install base | 現有的 Dynamics 365 Business Central 客戶。 目標 Power Apps 的夥伴。 | 
| 打造 Agile 商務程式-Dynamics 365 Customer Engagement 安裝基礎 | 現有的 Dynamics 365 Customer Engagement 客戶。 目標 Power Apps 的夥伴。 | 
| 打造具復原性的供應鏈-Windows，並以非 Oracle 或 SAP ERP 的 Dynamics 365 供應鏈管理來啟動第一部 Dynamics 365 工作負載 (企業資源規劃) 客戶 | Dynamics 365 供應鏈管理的目標客戶 | 
| 打造具復原性的供應鏈-跨銷售 Dynamics 365 供應鏈管理及/或零售或商務至現有的 Dynamics 365 Customer Engagement 客戶 | 現有的 Dynamics 365 Customer Engagement 客戶會以跨銷售 Dynamics 365 供應鏈管理為目標。 | 
| 打造具恢復功能的供應鏈-跨銷售 Dynamics 365 供應鏈管理及/或零售或商務至 Dynamics 365 Customer Engagement 和 Oracle 或 SAP | 現有的 Dynamics 365 Customer Engagement 客戶（具有 Oracle 或 SAP）以 Dynamics 365 供應鏈管理為目標 | 
| D365BCCluster | 識別客戶的傾向，以購買 Dynamics 365 Business Central。 顯示傾向 for Business Central 的客戶將會處於「中」和「小型」類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365BCFit | 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用 lookalike 模型來比較客戶，並查看它們是否適合 Microsoft 雲端產品。 每季更新評分。 | 
| D365BCIntent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| D365FOCluster | 識別客戶用來購買 Dynamics 365 財務和營運的傾向。 顯示財務 + 營運傾向的客戶，將會位於最上層的非受控類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365FOFit | 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用 lookalike 模型來比較客戶，並查看它們是否適合 Microsoft 雲端產品。 每季更新評分。 | 
| D365FOIntent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| D365CECluster | 識別客戶的傾向，以購買 Dynamics 365 Customer Engagement。 顯示傾向 for Customer Engagement 的客戶將會處於「中」和「小型」類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365CEFit | 指出適用于 Dynamics 365 Customer Engagement | 
| D365CEIntent | 指出 Dynamics 365 Customer Engagement 的意圖 | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | 識別客戶是否有 Dynamics 內部部署 AX 或 CRM 的開放續約 | 
| M365UpsellCustomer | 指出客戶是否顯示 Microsoft 365 的追加銷售傾向 | 
| 有 Google | 指出客戶是否顯示擁有 Google 產品的競爭信號 | 
| 具有 AWS | 指出客戶是否顯示擁有 AWS 產品的競爭信號 | 
| 具有 EA | 識別更新是否為 EA 或 EA 訂用帳戶 | 
| 已開啟 | 識別續約為開放或開價值的合約 | 

### <a name="cloud-ascent---azure-propensity-report"></a>**雲端上升-Azure 傾向報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| MPN 識別碼 | Microsoft 合作夥伴網路識別碼 | 
| [合作夥伴名稱] | 夥伴名稱 | 
| 客戶識別碼 | 客戶識別碼 | 
| DUNS 號碼 | Bradstreet 為傾向評分之客戶的 Dun & 號碼 | 
| 帳戶名稱 | 帳戶的名稱 | 
| 網域 | 帳戶的網域 | 
| 組織大小 | 組織的大小 | 
| 產業 | 產業 | 
| Vertical | 由 Microsoft、D&B 和其他產業標準所識別的傾向評分之客戶的垂直 | 
| 區域 | 位置的地理區域 | 
| 子公司 | 針對傾向評分的客戶子公司 | 
| Sales Territory | 傾向評分之客戶的銷售領域 | 
| City | 地理城市位置 | 
| 州 | 地理狀態位置 | 
| 郵遞區號 | 組織的郵遞區號 | 
| Country | 地理國家/地區位置 | 
| 區段 | 市場區段 | 
| 子區段 | 市場子細分 | 
| SMC 類型摘要 | SMC 型別 | 
| 最上層非受控-計算基礎 | 熱門未受管理的客戶-計算 | 
| 最上層非受控-使用者基底 | 熱門未受管理的客戶-使用者 | 
| IsNonProfit | 指出組織是否為非收益 (是或否)  | 
| 遷移-EOL Windows Server-EOL Windows Server IB 與雲端升高傾向-5 個以上的授權 | 具有 EOL 內部部署 Windows Server 的客戶 (也就是 EOL 版或更早的) 。 客戶有5個或更多的授權。 具有傾向分數的客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL Windows Server-EOL Windows Server IB 與雲端升高傾向-<5 授權 | 具有 EOL 內部部署 Windows Server 的客戶 (也就是 EOL 版或更早的) 。 客戶的授權少於5個。 具有傾向分數的客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL Windows Server-EOL Windows Server IB 未進行雲端升高傾向-5 個以上的授權 | 具有 EOL 內部部署 Windows Server 的客戶 (也就是 EOL 版或更早的) 。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 在不具雲端升高的情況下，遷移-EOL Windows Server-EOL Windows Server IB 傾向-<5 授權 | 具有 EOL 內部部署 Windows Server 的客戶 (也就是 EOL 版或更早的) 。 具有少於5個授權。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL SQL-EOL SQL Server IB 與雲端升高傾向-5 個以上的授權 | 具有 EOL 內部部署 SQL Server 的客戶 (也就是 EOL 版或更早的) 。 客戶有5個以上的授權。 客戶有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL SQL-EOL SQL Server IB 與雲端升高傾向-<5 授權 | 具有 EOL 內部部署 SQL Server 的客戶 (也就是 EOL 版或更早的) 。 具有少於5個授權。 具有傾向分數的客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL SQL-EOL SQL Server IB 未進行雲端升高傾向-5 個以上的授權 | 具有 EOL 內部部署 SQL Server 的客戶 (也就是 EOL 版或更早的) 。 客戶有5個或更多的授權。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-EOL SQL-EOL SQL Server IB 沒有雲端升高傾向-<5 授權 | 具有 EOL 內部部署 SQL Server 的客戶 (也就是 EOL 版或更早的) 。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移內部部署 Windows Server-目前 Windows Server IB 與雲端升高傾向-5 + 授權 | 客戶目前的內部部署 Windows Server (也就是版本晚于 EOL) 。 客戶有5個以上的授權。 客戶有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移內部部署 Windows Server-目前的 Windows Server IB 與雲端升高傾向-<5 授權 | 客戶目前的內部部署 Windows Server (也就是版本晚于 EOL) 。 客戶的授權少於5個。 客戶的 Azure 傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移內部部署 Windows Server-目前沒有雲端升高的 Windows Server IB 傾向-5 個以上的授權 | 客戶目前的內部部署 Windows Server (也就是版本晚于 EOL) 。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移內部部署 Windows Server-目前沒有雲端升高的 Windows Server IB 傾向-<5 授權 | 客戶目前的內部部署 Windows Server (也就是版本晚于 EOL) 。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移至 Azure SQL 或 SQL 虛擬機器 (Vm) 目前 SQL Server IB 與雲端升高傾向-5 + 授權 | 具有目前內部部署 SQL Server 的客戶 (也就是) EOL 以後的版本。 客戶有5個以上的授權。 客戶有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移至 Azure SQL 或 SQL Vm-目前 SQL Server IB 與雲端升高傾向-<5 個授權 | 具有目前內部部署 SQL Server 的客戶 (也就是) EOL 以後的版本。 客戶的授權少於5個。 客戶有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移至 Azure SQL 或 SQL Vm-目前的 SQL Server IB （沒有雲端升高傾向）-5 個以上的授權 | 具有目前內部部署 SQL Server 的客戶 (也就是) EOL 以後的版本。 客戶有5個以上的授權。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-遷移至 Azure SQL 或 SQL Vm-目前的 SQL Server IB （沒有雲端升高傾向）-<5 個授權 | 具有目前內部部署 SQL Server 的客戶 (也就是) EOL 以後的版本。 客戶的授權少於5個。 客戶沒有傾向分數。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-OSS-遷移至開放原始碼 Shakespeare (OSS) DB | 具有下列任一項競爭產品的現有客戶：于 postgresql、MySQL、適用于 mariadb。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-OSS-Azure 上的 Linux | 使用 Linux 的現有客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-SAP-Azure 上的 SAP | 具有 SAP 的現有客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-Windows 虛擬桌面-遠端桌面服務 IB | 識別使用中 Windows 遠端桌面服務的客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-Windows 虛擬桌面-跨銷售現代化工作至 Azure/WVD | 識別有 Microsoft 365 且沒有 Azure 的客戶。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-VMware IB | 產品的現有客戶： VMware。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 遷移-Citrix IB | 具有產品的現有客戶： Citrix 系統。 合作夥伴應以此客戶為目標，以遷移至 Azure。 | 
| 創新-分析-使用 high Azure 傾向進行 Power BI IB | 具有和使用中 Power BI 訂用帳戶的客戶，包括： Power BI 獨立 Pro、Power BI-Azure 套件、Power BI Office 套件、Power BI 套件 Microsoft 365 | 
| DevOps 與 GitHub-Visual Studio/MSDN IB | 識別具有 active Visual Studio 版本的客戶 | 
| Windows Server Standard 版本 | 顯示客戶購買的 Windows Server Standard 版本 | 
| Windows Server Standard 授權 | 顯示客戶的 Windows Server Standard 購買授權類型 | 
| Windows Server 資料中心版本 | 顯示客戶購買的 Windows 資料中心版本 | 
| Windows Server 資料中心授權 | 顯示客戶購買的 Windows 資料中心授權類型 | 
| AzureFit | 定義 firmographics 的內部和外部資料點。 [符合評分] 會使用 lookalike 模型來比較客戶，並查看它們是否適合 Microsoft 雲端產品。 每季更新評分。 | 
| AzureIntent | 社交媒體和客戶的線上行為定義意圖的相關信號。 意圖評分會依大小重迭，以定義群集。 意圖評分會每月更新。 | 
| AzureCluster | 藉由將符合和意圖建議合併到叢集中，來識別客戶購買 Azure 的傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| WindowsServerDataCenter_HasOpenRenewal | 識別客戶是否有 Windows Server Datacenter 的 open 續約 | 
| WindowsServerStandard_HasOpenRenewal | 識別客戶是否有 Windows Server Standard 的 open 續約 | 
| AzureUpsellCustomer | 識別客戶是否顯示 Azure 的追加銷售傾向 | 
| 有 Google | 指出客戶是否顯示擁有 Google 產品的競爭信號 | 
| 具有 AWS | 指出客戶是否顯示擁有 AWS 產品的競爭信號 | 
| 具有 EA | 識別更新是否為 EA 或 EA 訂用帳戶 | 
| 已開啟 | 識別續約為開放或開價值的合約 | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**雲端上升-合約續約傾向報表**

| 資料行名稱 | 資料說明 | 
| :--------- | :--------- | 
| MPN 識別碼 | Microsoft 合作夥伴網路識別碼 | 
| [合作夥伴名稱] | 夥伴名稱 | 
| 客戶識別碼 | 客戶識別碼 | 
| DUNS 號碼 | Bradstreet 為傾向評分之客戶的 Dun & 號碼 | 
| 帳戶名稱 | 帳戶的名稱 | 
| 網域 | 帳戶的網域 | 
| 組織大小 | 組織的大小 | 
| 產業 | 產業 | 
| Vertical | 由 Microsoft、D&B 和其他產業標準所識別的傾向評分之客戶的垂直 | 
| 區域 | 位置的地理區域 | 
| 子公司 | 針對傾向評分的客戶子公司 | 
| Sales Territory | 傾向評分之客戶的銷售領域 | 
| City | 地理城市位置 | 
| 州 | 地理狀態位置 | 
| 郵遞區號 | 組織的郵遞區號 | 
| Country | 地理國家/地區位置 | 
| 區段 | 市場區段 | 
| 子區段 | 市場子細分 | 
| SMC 類型摘要 | SMC 型別 | 
| 最上層非受控-計算基礎 | 熱門未受管理的客戶-計算 | 
| 最上層非受控-使用者基底 | 熱門未受管理的客戶-使用者 | 
| IsNonProfit | 指出組織是否為非收益 (是或否)  | 
| 有 Google | 指出客戶是否顯示擁有 AWS 產品的競爭信號 | 
| 具有 AWS | 指出客戶是否顯示擁有 AWS 產品的競爭信號 | 
| Azure 叢集 | 識別客戶購買 Azure 的傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365 財務 + 營運叢集 | 識別客戶用來購買 Dynamics 365 財務和營運的傾向。 顯示財務 + 營運傾向的客戶，將會位於最上層的非受控類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365 CE 叢集 | 識別客戶的傾向，以購買 Dynamics 365 Customer Engagement。 顯示傾向 for Customer Engagement 的客戶將會處於「中」和「小型」類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| D365 BC 叢集 | 識別客戶的傾向，以購買 Dynamics 365 Business Central。 顯示傾向 for Business Central 的客戶將會處於「中」和「小型」類別中。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| Microsoft 365 叢集 | 識別客戶要購買 Microsoft 365 的傾向。 目標立即行動和評估叢集，因為它們會產生更高的產量。 只有在您將目標設為 [立即行動] 並評估客戶之後，才會以培養為目標，並教育客戶。 | 
| 授權方案 | 識別續約的授權方案類型 | 
| 協議識別碼 | 合約的識別碼 | 
| [合約結束日期] | 合約的結束日期 | 
| 到期類型 | 到期的類型 | 
| 收入即將過期 | 與過期訂用帳戶相關聯的收益 | 
| 具有 EA | 識別更新是否為 EA 或 EA 訂用帳戶 | 
| 已開啟 | 識別續約為開放或開價值的合約 | 
| Azure 追加銷售客戶 | 識別客戶是否顯示 Azure 的追加銷售傾向 | 
| Microsoft 365 向上銷售客戶 | 指出客戶是否顯示 Microsoft 365 的追加銷售傾向 | 
| RevSumDivisionName | 識別要更新的產品 | 

## <a name="next-steps"></a>後續步驟

如需詳細資訊，請參閱 [下載報表](pci-download-reports.md)。
