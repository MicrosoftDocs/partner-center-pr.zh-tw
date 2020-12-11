---
title: 2020 年 12 月公告
description: Microsoft 合作夥伴中心的 2020 年 12 月公告，包括新功能、促銷、供應項目、市場，或現有供應項目的變更。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 12/02/2020
ms.openlocfilehash: 1341e60fd9914f421fd59335a8f037f3d915b72f
ms.sourcegitcommit: bc44a6e0c5ef048cda6e882fdb543c13c5b64912
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/08/2020
ms.locfileid: "96869294"
---
# <a name="december-2020-announcements"></a>2020 年 12 月公告

本頁詳述 Microsoft 合作夥伴中心 2020 年 11 月的公告。

2020 公告：[4 月](2020-april.md) | [5 月](2020-may.md) | [6 月](2020-june.md) | [7 月](2020-july.md) | [8 月](2020-august.md) | [9 月](2020-september.md) | [10 月](2020-October.md) | [11 月](2020-november.md) | 12 月

______________

## <a name="sdk-release-on-net-standard-v1163"></a><a name="4"></a>.NET Standard (v1.16.3) 上的 SDK 版本

### <a name="categories"></a>類別

- 日期：2020-12-8
- 功能

### <a name="impacted-audience"></a>影響對象

使用合作夥伴中心 .NET SDK 且參與 CSP 計畫的 Direct Bill 合作夥伴和 Indirect Provider。

### <a name="details"></a>詳細資料

自 2020 年 12 月 8 日起，合作夥伴可以開始下載 [MicrosoftPartnerCenter.NETSDK (NuGet 資源庫 | Microsoft.Store.PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3) 版本，以及更新的公用合作夥伴中心 SDK [GitHub 範例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)。 此版本包含下列各項的更新：
 
**SelfServePolicies - 新增功能**

- [GetSelfServePolicies](/partner-center/develop/get-a-self-serve-policy-by-id.md)
- [GetListOfSelfServicePolicies](/partner-center/develop/get-a-list-of-self-serve-policies.md)
- [CreateSelfServePolicies](/partner-center/develop/create-a-self-serve-policy.md)
- [UpdateSelfServePolicies](/partner-center/develop/update-a-self-serve-policy.md)
- [DeleteSelfServePolicies](/partner-center/develop/delete-a-self-serve-policy.md)
 
**客戶公司設定檔**

- 新增 [OrganizationRegistrationNumber](/partner-center/develop/create-a-customer.md)
 
**CustomerBillingProfile.DefaultAddress**

- 新增 MiddleName
 
### <a name="next-steps"></a>後續步驟

- 下載最新版本 [MicrosoftPartnerCenter.NETSDK (NuGet 資源庫 | Microsoft.Store.PartnerCenter 1.16.3)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.16.3)
- 下載並檢閱 [GitHub 範例](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

______________

## <a name="december-2020-license-based-price-list-release-notes"></a><a name="3"></a>2020 年 12 月授權型價目表版本資訊

### <a name="categories"></a>類別

- 日期：2020-12-8
- 供應項目/市場

### <a name="summary"></a>摘要 

2020 年 12 月授權型價目表和供應項目清單矩陣有一些問題。

### <a name="impacted-audience"></a>影響對象 

透過雲端解決方案提供者 (CSP) 方案交易的所有合作夥伴

### <a name="details"></a>詳細資料

2020 年 12 月授權型價目表和供應項目清單矩陣檔案包含一些異常。 這些問題僅與授權型定價檔案相關，應該會在 2021 年 1 月更新中修正。

#### <a name="incorrect-offers-in-the-license-based-price-list"></a>授權型價目表中有不正確的供應項目

12 月授權型價目表包含下列不應在價目表中的供應項目。 這些供應項目先前已錯誤地包含在價目表中，且不應發佈。 沒有供應項目可供使用的排程。 未來如果將其新增回去，則會在未來的預覽價目表中列為「新增」。

   |**供應項目名稱**|**優惠識別碼**|
   |-------------------|:------|
   |Dynamics 365 人力資源 (非營利組織定價)|1596fa61-7da1-4263-98f8-b27dfa4cfbb5|
   |Dynamics 365 人力資源附加至合格的 Dynamics 365 基礎供應項目 (非營利組織定價)|8bf0b826-e05b-45aa-9cd1-9a9f742f7731|
   |Dynamics 365 人力資源附加至合格的 Dynamics 365 基礎供應項目 (非營利組織定價) (合格供應項目)|f906435d-9dc9-42ba-bea6-2a2b08ca60db|
   |Dynamics 365 人力資源沙箱 (非營利組織定價)|079ec5ba-d726-4384-95af-62d135c210d2|
   |Dynamics 365 人力資源自助 (非營利組織定價)|931acecc-34c3-4f83-913e-c7fdbfd7e2a1|
   |Dynamics 365 作業 - 訂單行 (非營利組織定價)|7dd6b78a-3d53-47f8-8a64-bd84609a9a70|
   
#### <a name="incorrect-offers-in-the-offer-list-matrix"></a>供應項目清單矩陣中的供應項目不正確
   
下列供應項目錯誤地在供應項目清單矩陣中。 這些供應項目無法使用，尚未提供可供使用的目標日期。 合作夥伴應該忽略這些項目。

   |**供應項目名稱**|**優惠識別碼**|
   |-------------------|:------|
   |Dynamics 365 作業 - 資料庫容量 (非營利組織定價)|1d3f4d81-89b9-419e-a880-31b2c50b8d66|
   |Dynamics 365 作業 - 檔案容量 (非營利組織定價)|dc173a86-285b-444c-881e-3ece531f67da|

#### <a name="powerapps-offer"></a>Powerapps 供應項目

此供應項目已包含在供應項目清單矩陣中，但是未包含在 12 月價目表中。 供應項目可供使用，您可以在上個月的價目表 11 月檔案中找到定價。 此供應項目應新增回到 1 月價目表。

   |**供應項目名稱**|**優惠識別碼**|
   |-------------------|:------|
   |每個應用程式的 Power Apps 方案|5e1087b6-246b-4503-b88a-b60bdf0b3840|

### <a name="next-steps"></a>後續步驟

請經常檢查版本資訊，因為發現到的其他問題將會附加至此公告。

### <a name="last-updated"></a>上次更新

2020 年 12 月 8 日

______________

## <a name="an-update-of-the-us-microsoft-365-business-voice-with-calling-plan-offer-is-coming-soon"></a><a name="2"></a>美國 Microsoft 365 商務語音與通話方案供應專案即將更新

### <a name="categories"></a>類別

- 日期：2020-12-3
- 供應項目/市場

### <a name="summary"></a>摘要 

在 2021 年 1 月 1 日，Microsoft 會開始將美國合作夥伴和客戶轉換到新的 Microsoft 365 商務語音與通話方案供應項目。 不需要合作夥伴執行任何動作。

### <a name="impacted-audience"></a>影響對象 

透過雲端解決方案提供者 (CSP) 方案交易的所有合作夥伴

### <a name="details"></a>詳細資料

Microsoft 將以新的供應項目來取代現有的美國商務語音與通話方案供應項目，以支援電信產品的內部需求。 新的供應項目會有相同的功能集和定價。 供應項目變更為 Microsoft 內部，且不應該影響 CSP 合作夥伴行銷、銷售或支援商務語音與通話方案供應項目的方式。 此變更只會套用到此供應項目。

針對新銷售，您將會在 2021 年 1 月 1 日開始使用新的供應項目。 舊的供應項目將會取代為價目表上的新供應項目。

現有的客戶會在其更新日期自動轉換為新的供應項目。 合作夥伴和更新的客戶不需要採取任何動作。


**新供應項目詳細資料
 
   |**供應項目名稱**|**優惠識別碼**|**材質識別碼**|
   |-------------------|:------|:------|
   |Microsoft 365 商務語音 (美國)|86713ec1-ad33-42cf-a1ce-8397d4d875fe|PZW-00023|
   
**舊供應項目詳細資料

   |**供應項目名稱**|**優惠識別碼**|**材質識別碼**|
   |-------------------|:------|:------|
   |Microsoft 365 商務語音 (美國)|9f9f2c7b-c961-402b-9421-8e3c9207eeb3|PZW-00009|

### <a name="next-steps"></a>後續步驟

請參閱價目表，並與貴組織中所有相關連絡人分享這項資訊。

______________

## <a name="now-live-partner-center-api-updates-and-user-interface-enhancements-for-the-education-customer-validation-process"></a><a name="1"></a>即時實況：教育版客戶驗證程序的合作夥伴中心 API 更新和使用者介面增強功能

### <a name="categories"></a>類別

- 日期：2020-12-3
- 功能

### <a name="impacted-audience"></a>影響對象 

透過雲端解決方案提供者計畫銷售學術供應項目的合作夥伴

### <a name="summary"></a>摘要 

Microsoft 的營運以信任為原則。 針對在雲端解決方案提供者計畫中從事學術供應項目交易時所需的客戶驗證，提供符合規範且安全的方法，是我們一貫努力的目標。 為履行此承諾，我們將會導入合作夥伴中心 API 和使用者介面增強功能，讓客戶審查程序更加清楚明瞭，且能夠輸入更精確的資料，以提升客戶審查的成功率。 

**合作夥伴中心的增強功能** 

- 新的 GET 和 POST 資格 API 可支援精確的資料輸入，並改善 Microsoft 的教育客戶驗證程序。 

- 使用者介面增強功能可支援精確的資料輸入，並改善 Microsoft 的教育客戶驗證程序。 

**取代現有的 GET 和 PUT 限定性條件 API** 

現有的 GET 和 PUT 限定性條件 API 將會在 **2021 年 2 月底前** 淘汰。 屆時，您必須轉換成新的 GET 和 POST 合作夥伴中心 API，才能夠購買教育版供應項目。  

**測試** 

若要深入了解想要成功進行客戶驗證所需的 API 和資料輸入，合作夥伴可以開始測試這些增強功能。 想要參與測試的合作夥伴應下載[合作夥伴中心教育客戶測試指南](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf)，以了解整備、註冊方式的方向，以及測試階段中預期情況的相關資訊。

**圖書館和博物館客戶** 

除了上述增強功能以外，我們也迫不及待地宣佈，我們將為圖書館和博物館客戶啟用學術定價供應項目，以擴展您可以銷售 CSP 供應項目的教育客戶。 

Microsoft 保留對任何客戶或建議客戶審查其教育使用者資格的權利。 如需完整詳細資料，請參閱[學術合格教育使用者需求](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)。 

### <a name="next-stepsadditional-resources"></a>後續步驟/其他資源

- 在作業整備資源中檢閱新的合作夥伴中心使用者介面、API 變更和指南：[合作夥伴中心教育客戶驗證](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)程序增強功能 

- 請確定您的組織已熟悉[學術合格教育使用者需求](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7)。 

- 請與組織中的適當小組以及轉銷商分享這項資訊，協助他們為這些變更做好準備。 

### <a name="change-log"></a>變更記錄 

_ 2020 年 8 月 31 日：原始發行 

- 2020 年 9 月 25 日：已新增測試視窗更新 

- 2020 年 10 月 4 日：註冊以進行測試的提醒 

- 2020 年 11 月 10 日：註冊以進行測試的提醒 

- 2020 年 12 月 3 日：API 即時更新 
