---
title: 2020 年 11 月公告
description: Microsoft 合作夥伴中心的 2020 年 11 月公告，包括新功能、促銷、供應項目、市場，或現有供應項目的變更。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691294"
---
# <a name="november-2020-announcements"></a>2020 年 11 月公告

本頁詳述 Microsoft 合作夥伴中心 2020 年 11 月的公告。

2020 公告：[4 月](2020-april.md) | [5 月](2020-may.md) | [6 月](2020-june.md) | [7 月](2020-july.md) | [8 月](2020-august.md) | [9 月](2020-september.md) | [10 月](2020-October.md) | 11 月

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>合作夥伴計費貨幣的 EU/EFTA 變更 (適用於新商業供應項目)。  

### <a name="categories"></a>類別
- 日期 2020-11-17
- 功能

### <a name="impacted-audience"></a>影響對象  

EU/EFTA 地區中透過雲端解決方案提供者計畫進行交易的合作夥伴 

### <a name="summary"></a>總結 

在歐盟 (EU)/歐洲自由貿易聯盟 (EFTA) 地區中，雲端解決方案提供者計畫中所有新的商業供應項目都將使用合作夥伴計費位置，而不是客戶計費位置。 這表示 Microsoft 將依據合作夥伴所在位置的貨幣 (而非其客戶所在位置的貨幣) 對合作夥伴計費。 此作業會分兩個階段完成： 

- **階段 1：在 CSP 中購買新商業供應項目的新客戶**

從 2021 年 1 月開始，有新客戶購買了新商業供應項目的合作夥伴，將會以合作夥伴所在位置的貨幣對這些購買計費。 有現有的客戶在 CSP 中購買了新商業供應項目的合作夥伴，在此階段將繼續以客戶計費位置的貨幣計費。 

 

- **階段 2：在 2021 年 1 月前在 CSP 中購買新商業供應項目的現有客戶** 

在階段 1 之後的日曆年度 2021 年期間，Microsoft 將會針對有現有客戶 (在 2021 年 1 月之前購買新的商業供應項目) 的合作夥伴，將新商業供應項目的計費從客戶所在位置的貨幣轉換為合作夥伴所在位置的貨幣。 在實作這項變更之前，合作夥伴會先收到通知。  

>[注意] 這項變更只會影響合作夥伴的計費貨幣，而不會影響 CSP 中新商業供應項目的定價。 

這項變更涵蓋的新商業供應項目包括：雲端解決方案提供者計畫中屬於 Azure 方案、Azure 保留、伺服器訂閱、永久軟體和 Microsoft 商業市集購買的 Azure 訂閱。

### <a name="partner-benefits"></a>合作夥伴權益  

- 這項更新可降低 EU/EFTA 地區的多幣別發票所產生的複雜性和額外負荷，以提供新的商業體驗。  

- 合作夥伴將收到採用單一貨幣的合併發票，而不會再收到個別客戶所在地貨幣的發票。 

- 獎勵給付將採用與合作夥伴的發票貨幣相同的貨幣。

- 合作夥伴會發現多幣別發票所導致的計費複雜性不復存在，而能夠省下現行與對帳有關的時間和資源。 

- 對於尚未採用新商業供應項目的合作夥伴，這項變更與先前的合作夥伴計費模型保持一致，讓合作夥伴能更輕鬆地轉換至 CSP 的新商業體驗。 

### <a name="resources"></a>資源 

請在 Microsoft 合作夥伴網站上的 [作業資源庫] (https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ ) 中參閱本主題的相關資訊。  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>合作夥伴呼叫合作夥伴中心 API 的 API 節流

### <a name="categories"></a>類別

- 日期 2020-11-17
- 功能

### <a name="summary"></a>摘要

Microsoft 即將為呼叫合作夥伴中心 API 的合作夥伴導入 API 節流，以在給定的時間範圍內提供更一致的效能。

### <a name="impacted-audience"></a>影響對象

透過雲端解決方案提供者計畫進行交易的合作夥伴

### <a name="details"></a>詳細資料

Microsoft 即將在 2021 年第 1 季實作 API 節流，讓呼叫合作夥伴中心 API 的合作夥伴在一段時間範圍內能獲得更一致的效能。 節流會限制在特定時間範圍內對服務的要求數目，以避免過度使用資源。 超過節流閾值時，合作夥伴中心將會在一段時間內限制來自該用戶端的任何後續要求。  

### <a name="partner-benefits"></a>合作夥伴權益 

合作夥伴中心依設計可處理大量要求，但若有幾個合作夥伴提出了極大量的要求，節流將有助於為所有合作夥伴維持理想的效能和可靠性。 這樣可以盡可能縮短停機時間。 藉由減少大量要求，我們得以確保所有合作夥伴都享有一致的效能。 


### <a name="apis-to-be-throttled"></a>要節流的 API

|**運算**|**合作夥伴中心文件**|
|-------------------------|----------------------------------|
|{baseURL}/v1/customers/{customer_id}/subscriptions|[取得客戶的所有訂用帳戶](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[依照識別碼取得訂用帳戶](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/customers/{customer_id}/orders||[取得客戶的所有訂單](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}|[依識別碼取得供應項目](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/customers/{customer_id}/orders/{order_id}/provisioningstatus|[取得訂用帳戶的佈建狀態](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}|[管理訂單和管理訂用帳戶](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/addons|[取得訂用帳戶的附加元件清單](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/azureEntitlements|[取得訂用帳戶的 Azure 權利清單](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/customers/{customer_id}/subscriptions/{subscription_id}/registrationstatus|[取得訂用帳戶的註冊狀態](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/customers/{customer-tenant-id}/transfers|[取得客戶的所有轉移](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{upgrade-id}/status|[取得產品升級狀態](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/customers/{customer-id}/subscriptions/{subscription-id}/conversions|[取得試用版轉換方案的清單](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

此公告旨在讓合作夥伴及早了解即將進行的變更，進而做好準備。 我們強烈建議合作夥伴熟悉這些 API，並考慮使用活動記錄 API 以提高效率並避免節流。 如需這項功能的詳細資訊，請參閱 [API 節流指導方針](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance)中的詳細資訊。 

### <a name="next-steps"></a>後續步驟

請參閱 [API 節流指導方針](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance)，並執行必要的步驟。 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>因 MCA 要求重複而產生的 409 錯誤

### <a name="categories"></a>類別

- 日期 2020-11-16
- 功能

### <a name="context"></a>Context

- 今年二月，我們要求合作夥伴簽署了 Microsoft 客戶合約 (MCuA)。 這是從 Microsoft Cloud 合約 (MCA) 進行的移轉。 
- 在此變更中，我們要求合作夥伴依照[這裡](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)的說明納入合約類型參數。

### <a name="what-happened-next"></a>後續情形：

- 並非所有的合作夥伴都已在其實作中納入參數要求。 Microsoft 將 MCA 退回給這類合作夥伴。
- 其後，合作夥伴會將簽署要求重新傳送給客戶，然後將 MCA 重新傳送給 Microsoft。 
- 重複的要求會影響 Microsoft 為合作夥伴提供服務的能力。
- 2020 年 9 月，我們透過 Yammer 在多個論壇向合作夥伴傳送了通知，要求合作夥伴修正參數。 Microsoft 無法再接受重複的要求，這類要求將會引發 409 錯誤。

>[注意] 這不是合作夥伴的新合約/API 變更。

- 在 10 月，我們與提出最多重複要求的合作夥伴展開密切合作，以修正問題。
- 目前，我們會提醒合作夥伴，並且對前 10 大違規者傳送個人電子郵件，要求他們檢閱自己的要求並與我們聯繫，以便協助他們測試並解決問題。
- 我們已在 2020 年 11 月 10 日停止接受重複要求，且未更正參數的合作夥伴將會收到 409 錯誤。
- 從那時起，我們撤回了不接受重複要求的變更。 
- 但自 2021 年 1 月 14 日起，我們將再恢復為不再接受重複要求。 這可讓合作夥伴有更多時間進行其調整。 我們已收到某個合作夥伴提供的通知，他們計畫在11/16 部署更新，屆時我們將與他們密切合作。
- 我們要求合作夥伴與我們聯繫，以將其租用戶新增至具有變更的正式發行前小眾測試版，而協助他們進行測試，並確定其解決方案更新可正常運作。



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>可用的測試：教育版客戶驗證程序的合作夥伴中心 API 更新和使用者介面 (UI) 增強功能

### <a name="categories"></a>類別

- 日期 2020-11-10
- 功能 | 提高效率和規模

### <a name="impacted-audience"></a>影響對象

透過雲端解決方案提供者 (CSP) 計畫銷售學術供應項目的合作夥伴。

### <a name="summary"></a>總結

教育版客戶驗證程序的合作夥伴中心 API 更新和 UI 增強功能現在可以執行測試了。

### <a name="details"></a>詳細資料

Microsoft 的營運以信任為原則。 我們承諾針對在 CSP 計畫中從事學術供應項目交易時所需的客戶驗證，提供符合規範且安全的方法，是我們一貫努力的目標。 作為承諾的一部分，我們將會在本會計年度的第二季 (FY21 Q2) 引進合作夥伴中心 API 和 UI 增強功能。 這些增強功能可讓您更清楚地了解客戶驗證程序，並讓您能夠輸入更精確的資料，以提升客戶驗證的成功機率。

**合作夥伴中心的增強功能**

- 新的 GET 和 POST 資格 API 可支援精確的資料輸入，並改善 Microsoft 的教育客戶驗證程序。

- UI 增強功能可支援精確的資料輸入，並改善 Microsoft 的教育客戶驗證程序。

**測試**

若要深入了解想要成功進行客戶驗證所需的 API 和資料輸入，合作夥伴能夠從 2020 年 10 月開始測試這些增強功能。 我們將在近期提供關於確切時間和如何參與的詳細資料。 現有的合作夥伴中心 API 將在 FY21 Q2 結束前淘汰。 屆時，您就必須轉換使用新的合作夥伴中心 API。

   - 測試已可供使用 合作夥伴測試日期為 2020 年 10 月 2 日到 2020 年 12 月 2 日。 想要參與的合作夥伴應下載合作夥伴中心教育客戶測試指南，以了解整備方式、註冊方式，以及測試階段中預期的情況。

**圖書館和博物館客戶**

除了這些增強功能外，我們也迫不及待地宣佈，在 FY21 Q2，我們將為圖書館和博物館客戶啟用學術定價供應項目，以擴展可作為 CSP 供應項目銷售對象的教育客戶。

Microsoft 保留對任何客戶或建議客戶審查其教育使用者資格的權利。 如需完整詳細資料，請參閱[學術合格教育使用者需求](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)。

## <a name="next-steps"></a>後續步驟

請檢閱新的合作夥伴中心 UI 和 API 變更，以及[合作夥伴中心教育客戶驗證程序增強功能內容集合](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)中的測試指南

• 註冊參與測試。 (如需詳細資訊，請參閱[測試指南](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf))。 

• 確定您的組織已熟悉[學術合格教育使用者需求](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)。 

• 與組織中的適當小組以及轉銷商分享這項資訊，協助他們為這些變更做好準備。



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>在作業整備資源庫上擴展商業授權合作夥伴內容

### <a name="categories"></a>類別

- 日期：2020-11-5
- 功能

### <a name="summary"></a>摘要

從 2020 年 11 月 5 日開始，合作夥伴大學的商業授權合作夥伴內容也會在作業整備資源庫中提供。

### <a name="impacted-audience"></a>影響對象

商業合作夥伴

### <a name="details"></a>詳細資料

從 2020 年 11 月 5 日開始，合作夥伴大學的商業授權合作夥伴內容也會在作業整備資源庫中提供。 這會將作業整備資源庫上已存在的營運和商業授權合作夥伴啟動內容，與合作夥伴大學的持續性商業授權合作夥伴內容合併在一起。 因此，這能為合作夥伴提供更順暢的整備體驗。 下列集合已新增至作業整備資源庫：

- [Microsoft Azure - 供應項目和授權](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [商業授權 - CSP 焦點呼叫](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [商業授權 - 授權更新呼叫](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>接下來的步驟

請與貴組織所有相關連絡人分享這項資訊。

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5"></a>Microsoft Teams 會議室進階 SKU 啟動

### <a name="categories"></a>類別

- 日期：2020-11-3
- 供應項目/市場

### <a name="summary"></a>摘要

透過雲端解決方案提供者 (CSP) 計畫所提供、適用於 Microsoft Teams 的 Microsoft Teams 會議室進階 SKU 現已正式推出。

### <a name="impacted-audience"></a>影響對象

透過雲端解決方案提供者 (CSP) 方案交易的所有合作夥伴

### <a name="details"></a>詳細資料

適用於 Microsoft Teams 會議室的新 Microsoft Teams 會議室進階 SKU 現在已可供透過您以每月每裝置 50 美元購買 CSP 的客戶使用。 Microsoft Teams 會議室進階 SKU 是 Microsoft Teams 會議室標準 SKU (先前稱為「會議室」授權) 的替代方案。 此 SKU 包含標準供應項目中的一切權益，例如 Microsoft Teams、商務用 Skype Online 和 Intune 管理所需的授權。 此供應項目也可實現電話系統，這是公用交換電話網路 (PSTN) 整合和音訊會議 (如果有的話) 的所需項目。 

透過進階供應項目，客戶可以存取新發行的 Microsoft Teams 會議室受控服務，在此服務中，會由專家代表客戶處理會議室的管理和作業。 這個雲端式 IT 管理和監視服務可讓 Microsoft Teams 會議室裝置及其週邊設備保持在安全且最新的狀態。 其也會受到主動監視和管理，從而維護已專為提供絕佳會議室體驗而最佳化的環境。

#### <a name="released-at-launch"></a>推出時的釋出內容

   |****|**Microsoft Teams 會議室標準版每月每裝置 15 美元**|**Microsoft Teams 會議室進階版每月每裝置 50 美元**|
   |-------------------|:------|:------|
   |商務用 Skype|是| |
   |Microsoft Teams|是|是|
   |電話系統|是|是|
   |音訊會議|是|是|
   |Microsoft Intune|是|是|
   | |Microsoft Teams 會議室標準版每月每裝置 15 美元|Microsoft Teams 會議室進階版每月每裝置 50 美元|
   |Microsoft Teams 會議室受控服務| |是|
   |全球可用性|是|在經過挑選的市場中|

#### <a name="microsoft-teams-rooms-managed-services"></a>Microsoft Teams 會議室受控服務

- 主動式管理：全天候管理您的會議室系統，包括修補、設定管理等。
•   即時監視和根本原因分析：在需要時，使用由 Microsoft 與客戶協調所驅動的協調事件管理回應來進行監視和偵測。 行動應用程式可讓您隨時隨地掌握警示。
- 受控更新：應用程式、Windows KB 和韌體更新的管理與傳遞。
- 安全性威脅防護：透過 Microsoft Defender 進階威脅防護的安全性威脅防護。
- 客戶支援：透過我們專門的服務營運中心提供全天候票證支援，以提供非自動化案例的協助事件補救。 細微的角色型存取控制。
- 見解與建議：針對會議室健全狀況、詳細目錄、使用情形、線上會議和事件趨勢的客戶和報告彙總見解。

#### <a name="offer-details"></a>供應項目詳細資料

   |**供應項目名稱**|**優惠識別碼**|**材質識別碼**|
   |-------------------|:------|:------|
   |Teams 會議室進階版|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Teams 會議室進階版 (USA 和 CAN)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Teams 會議室進階版 (教職員用)|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>後續步驟

- 熟悉新的供應項目和其地理可用性，請造訪[常見問題集 (FAQ)]()。
- 熟悉新的供應項目和其地理可用性。 
- 在 [Microsoft Teams 會議室](https://rooms.microsoft.com/)深入了解 Microsoft 會議室和相關供應項目。
- 使用 [Teams 合作夥伴指南](https://aka.ms/teamscallingmeetingsguide)來發展 Teams 會議室實務，並建立共同銷售就緒的供應項目。
- 若要深入了解產品解決方案和服務，請檢閱 [Microsoft Teams 會議室常見問題集](https://aka.ms/PartnerMTRFAQ)。 
- 請與您組織中所有的適當連絡人分享這項資訊，以了解追加銷售和交叉銷售商機。

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>適用於政府社群雲端 (GCC) 的新 Microsoft Teams 進階通訊 SKU 即將推出

### <a name="categories"></a>類別

- 日期：2020-11-2
- 供應項目/市場

### <a name="summary"></a>摘要

適用於 Microsoft Teams 的進階通訊附加元件 SKU 即將於 2020 年 12 月 1 日推出。

### <a name="impacted-audience"></a>影響對象

透過雲端解決方案提供者 (CSP) 方案交易的所有合作夥伴

### <a name="details"></a>詳細資料

您現在可以用每個使用者每個月 12 美元的價格，取得 GCC 中的 Microsoft Teams 適用的進階通訊附加元件。 附加元件 SKU 可以在包含 Microsoft Teams 的任何其他 Microsoft 365 套件上購買。 進階通訊提供了一組用於大型會議、通訊原則和整合的新功能，以及適用於 IT 管理的進階工具。 

#### <a name="offer-details"></a>供應項目詳細資料

   |**供應項目名稱**|**優惠識別碼**|**材質識別碼**|
   |-------------------|:------|:------|
   |適用於 GCC 的進階通訊|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>常見問題集 

**什麼是進階通訊？** 這是新的 Microsoft Teams 附加元件，可讓客戶進一步強化其溝通經驗。 客戶可以在其訂閱的任何 Microsoft 365 SKU 上購買。

**需要多少成本？** 商用 ERP 是每位使用者每個月 12 美元。

**哪些客戶可以購買此附加元件？** GCC 客戶可以購買附加元件。

**如何購買？** 附加元件可透過 Enterprise 合約、Enterprise 合約訂用帳戶、教育解決方案註冊、CSP 或 Web Direct 來購買。

**可以在何處銷售？** 該元件可在美國市場銷售。

**有哪些必要條件？** 包含 Microsoft Teams 的任何 Microsoft 365 或 Office 365 套件，都可以有此附加元件。

### <a name="next-steps"></a>後續步驟

請與您組織中相關連絡人分享這項資訊，以了解追加銷售和交叉銷售商機。 請參閱 [Teams 合作夥伴指南](https://aka.ms/teamscallingmeetingsguide)的資源區段。

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365：最近推出和即將推出的新供應項目與產品

### <a name="categories"></a>類別

- 日期：2020-11-2
- 供應項目/市場

### <a name="impacted-audience"></a>影響對象

直接提供者、間接提供者和間接經銷商

### <a name="details"></a>詳細資料

#### <a name="new-offers"></a>新供應項目

Microsoft 將在 2020 年 11 月 1 日發行 Dynamics 365 Project Operations 供應項目，並移除適用於商業客戶的 Dynamics 365 Project Service Automation (PSA)。 此通訊提供與本次推出和新的獨立軟體廠商 (ISV) 內嵌供應項目的雙重使用權限對應有關的其他資訊。

#### <a name="project-operations-isv-embed-offers"></a>Project Operations ISV 內嵌供應項目

Microsoft 在 2020 年 11 月 1 日另外發行了三個 36 個月的 ISV 內嵌供應項目，適用於雲端解決方案提供者 (CSP) 客戶的 Dynamics 365 for Project Operations。 如需 SKU 詳細資料，請參閱 [Dynamics CSP Offers-November 2020 Excel 文件](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls)中的 [Project Operations] 索引標籤。

#### <a name="project-operations-dual-use-rights-mapping"></a>Project Operations 雙重使用權限對應

您可以在下表中找到 Project Operations 供應項目的 Dynamics 365 雙重使用權限內部部署對應的資訊：

   |**D365 Operations 供應項目**|**D365 內部部署雙重使用權限對應**|
   |-------------------|:------|
   |D365 Operations 供應項目|D365 內部部署雙重使用權限對應|
   |D365 Project Operations|D365 for Operations，使用 Dyn365 Project Operations SKU (109108477) 的內部部署 (XA 伺服器)|
   |D365 Project Operations Attach|D365 for Operations，使用 Dyn365 Project Operations SKU (109108477) 的內部部署 (XA 伺服器)|
   |D365 Finance 和 Project Operations|D365 for Operations，使用 Dyn365 Project Operations SKU (109108477) 的內部部署 (XA 伺服器)|
   |D365 Finance Attach 和 Project Operations|D365 for Operations，使用 Dyn365 Project Operations SKU (109108477) 的內部部署 (XA 伺服器)|
   |D365 Unified Operations – Activity 和 Project Operations|D365 for Operations，使用 Dyn365 Project Operations SKU (109108477) 的內部部署 (XA 伺服器)|

#### <a name="previously-announced"></a>先前公告

Microsoft 在 2020 年 11 月 1 日發行了下列全新和更新的 Dynamics 365 和 Power Platform 供應項目，以及適用於 CSP 的產品：

- Dynamics 365 Customer Voice USL 

如需供應項目識別碼詳細資料，請參閱 [Dynamics CSP Offers-November 2020 Excel 文件](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls)中的 [Project Operations] 索引標籤。

您可以在 Microsoft Dynamics 365 Customer Voice 首頁找到更多資源。

### <a name="next-steps"></a>後續步驟

請與組織內的相關人員分享這項資訊。

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>適用於非營利組織的 Microsoft 365 商務語音介紹

### <a name="categories"></a>類別

- 日期：2020-11-2
- 供應項目/市場

### <a name="summary"></a>摘要

Microsoft 在 2020 年 11 月 1 日針對適用於非營利組織的 Microsoft 365 商務語音引進了新的 SKU。

### <a name="impacted-audience"></a>影響對象

直接提供者、間接提供者和間接經銷商

### <a name="details"></a>詳細資料

Microsoft 在 2020 年 11 月 1 日針對商務語音引進了新的 SKU。 完整套件在加拿大、英國及美國提供。 商務語音 (不含通話方案) 將會在所有其他市場中提供。 

Microsoft 365 商務語音是一種雲端式電話系統，適用於納入 Office 365 的中小型企業。 將商務語音新增至客戶的 Office 365 訂用帳戶，即可透過單一應用程式 Microsoft Teams 中的通話、聊天和會議功能，來提供多合一的溝通與共同作業解決方案。

如需定價詳細資料，請參閱價目表。

您可以將 Microsoft 365 商務語音新增至下列最多有 300 位使用者的訂用帳戶：

- Office 365：商務基本版、商務進階版、A1、E1、A3 和 E3
- Microsoft 365：商務版、A3 和 E3


### <a name="next-steps"></a>後續步驟

- 請熟悉預覽價目表中的資訊，並與組織內的所有適當連絡人分享這項資訊。 
- 檢閱雲端解決方案提供者計畫更新資源庫中的所有準備資料：[適用於中小型企業的 Microsoft 365 商務語音簡介](https://partner.microsoft.com/resources/collection/m365-voice-smb#/)。 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>現已推出適用於 Microsoft 365 商務語音的雲端解決方案提供者 (CSP) 促銷

### <a name="categories"></a>類別

- 日期：2020-11-2
- 供應項目/市場

### <a name="summary"></a>摘要

新用戶和續約用戶訂閱包含通話方案的 Microsoft 365 商務語音及不含通話方案的 Microsoft 365 商務語音，均須享有折扣定價。

### <a name="impacted-audience"></a>影響對象

透過 CSP 計畫進行交易的所有合作夥伴

### <a name="details"></a>詳細資料

從 2020 年 11 月 1 日到 2021 年 4 月 30 日止，新用戶和續約用戶訂閱包含通話方案的 Microsoft 365 商務語音及不含通話方案的 Microsoft 365 商務語音，均須享有折扣定價。 包含通話方案的 Microsoft 365 商務語音享有 12 個月 25% 的折扣，而不含通話方案的 Microsoft 365 商務語音則享有 12個月 33% 的折扣。 

#### <a name="offer-details"></a>供應項目詳細資料

   |**供應項目名稱**|**優惠識別碼**|**材質識別碼**|
   |-------------------|:------|:------|
   |Microsoft 365 商務語音採用促銷|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Microsoft 365 商務語音採用促銷|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Microsoft 365 商務語音 (美國) 採用促銷|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Microsoft 365 商務語音 (不含通話方案) 採用促銷|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Microsoft 365 商務語音 (不含通話方案) 採用促銷|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Microsoft 365 商務語音 (不含通話方案) 採用促銷|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |適用於美國的 Microsoft 365 商務語音 (不含通話方案) 採用促銷|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

這些促銷所影響的客戶如下：

- 全新客戶租用戶
- 現有客戶租用戶，但其在 CSP、Web Direct 或任何其他 Microsoft 商業頻道的任何商務語音或音訊會議授權上，沒有作用中或最近 (過去 30 天內) 取消的訂用帳戶

#### <a name="additional-resources"></a>其他資源

- 請瀏覽 [Microsoft 365 商務語音合作夥伴頁面](https://www.microsoft.com/microsoft-365/partners/businessvoice)，以深入了解商務語音。 
- 若要深入了解這項促銷，請參閱相關的[合作夥伴常見問題集](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo)。

### <a name="next-steps"></a>後續步驟

- 請熟悉這些會議及通話促銷機會，並與您組織中的所有適當連絡人分享這項資訊。
- 將這些促銷併入您的 Microsoft 365 銷售動作中。
- 向客戶說明將商務語音新增至 Teams 的價值。 

________________
