---
title: 以授權為基礎的對帳檔案 |合作夥伴中心
ms.topic: article
ms.date: 01/08/2020
description: 瞭解合作夥伴中心內以授權為基礎的對帳檔案。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 7b7e3140ddcbdbaa5ff75203928b890abc2db852
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757181"
---
# <a name="license-based-reconciliation-files"></a>授權型對帳檔案

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**
-   全域系統管理員
-   使用者系統管理員
-   帳單管理
-   系統管理代理人

若要根據客戶的訂單來協調您的變更，請將對帳檔案中的**Syndication_Partner_Subscription_Number**與合作夥伴中心的訂用帳戶**識別碼**進行比較。

## <a name="fields-in-license-based-reconciliation-files"></a>以授權為基礎的對帳檔案中的欄位

| 欄位 | 說明 | 範例值 |
| ------ | ----------- | ------------ |
| PartnerId | 特定計費實體的唯一識別碼（GUID 格式）。 不需要進行調整。 在所有資料列中都是如此。 | *8ddd03642-測試-測試-測試-46b58d356b4e* |
| CustomerId | 客戶的唯一 Microsoft 識別碼（GUID 格式）。 | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | 客戶的組織名稱（如合作夥伴中心所報告）。 *將發票與系統資訊協調的非常重要欄位。* | *測試客戶 A* |
| MpnId | CSP 合作夥伴的 MPN 識別碼。 請參閱[如何依合作夥伴進行](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)加入。 | *4390934* |
| ResellerMpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 目前的活動無法使用。 |
| OrderId | 訂單在 Microsoft 帳單平台中的唯一識別碼。 在聯繫支援人員時，識別訂單可能會很有用。 不用於對帳。 | *566890604832738111* |
| SubscriptionId | 訂閱在 Microsoft 帳單平台中的唯一識別碼。 在聯絡支援人員時，識別訂用帳戶可能會很有用。 不用於對帳。 *此值與合作夥伴管理主控台上的**訂**用帳戶識別碼不同。請改為參閱**SyndicationPartnerSubscriptionNumber** 。* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | 訂閱的唯一識別碼。 針對相同的方案，客戶可以有多個訂用帳戶。 此資料行對對帳檔案分析很重要。 此欄位會對應至合作夥伴管理主控台中的訂用帳戶**識別碼**。 | *fb977ab5-測試-測試-測試-24c8d9591708* |
| OfferId | 唯一的供應專案識別碼。 標準供應專案識別碼，如價格清單中所定義。 *此值不符合價格清單中的**供應專案識別碼**。請改為參閱**DurableOfferID** 。* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | 唯一的長期供應專案識別碼，如價格清單中所定義。 *這個值會符合價格清單中的**供應專案識別碼**。* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 客戶購買的服務優惠名稱，如價目表中所定義。 | *Microsoft Office 365 （方案 E3）* |
| SubscriptionStartDate | 訂用帳戶開始日期。 時間一律是一天的開始時間 (0:00)。 此欄位會設定為提交訂單後的日期。 與**subscription.subscriptionenddate**搭配使用，以判斷客戶是否仍在訂用帳戶的第一年內，或訂用帳戶已于以下年度續訂。 | *2/1/2019 0:00* |
| SubscriptionEndDate | 訂閱結束日期。 時間一律是一天的開始時間 (0:00)。 *12 個月加上開始日期後的**x**天*，以符合合作夥伴的帳單日期或*從續約日期算起12個月*。 續約時，價格會更新至目前的價目表。 自動續約之前，可能需要與客戶連絡。 | *2/1/2019 0:00* |
| ChargeStartDate | 開始計算費用的日期。 時間一律是一天的開始時間 (0:00)。 當客戶變更基座號碼時，用來計算每日費用（*pro rata*費用）。 | *2/1/2019 0:00* |
| ChargeEndDate | 結束計算費用的日期。 時間一律是一天的結束時間 (23:59)。 當客戶變更基座號碼時，用來計算每日費用（*pro rata*費用）。 | *2/28/2019 23:59* |
| ChargeType | 費用或調整的[類型](recon-file-charge-types.md)。 | 請參閱[費用類型](recon-file-charge-types.md)。 |
| UnitPrice | 每一基座價格，即購買時價目表中所公佈的價格。 請確定這符合您的計費系統中儲存的資訊。 | *6.82* |
| 數量 | 基座數目。 請確定這符合您的計費系統中儲存的資訊。 | *2* |
| 金額 | 數量總價。 用來檢查金額計算是否符合您為客戶計算此值的方式。 | *13.32* |
| TotalOtherDiscount | 套用至這些費用的折扣金額。 專長認證或地圖所附的產品授權，或符合獎勵資格的新訂用帳戶，也會在本專欄中包含折扣金額。 | *2.32* |
| 小計 | 稅前總計。 檢查您的小計是否符合您的預期總計（以折扣為例）。 | *11* |
| 稅 | 稅金金額費用。 根據您市場的稅務規則和特定情況。 | *0* |
| TotalForCustomer | 稅後總計。 檢查發票中是否向您收取稅金。 | *11* |
| Currency | 貨幣類型。 每一帳單實體都只有一種貨幣。 檢查它是否符合您的第一個發票。 在任何主要的計費平臺更新之後再次檢查。 | *EUR* |
| DomainName | 客戶的功能變數名稱。 在下一個帳單週期之前，此欄位會是空白的。 *請勿使用此欄位作為客戶的唯一識別碼。客戶/合作夥伴可以透過 Office 365 入口網站更新虛名或預設網域。* | *example.onmicrosoft.com* |
| SubscriptionName | 訂閱暱稱。 如果未指定昵稱，合作夥伴中心會使用**OfferName**。 | *PROJECT ONLINE* |
| SubscriptionDescription | 客戶購買的服務優惠名稱，如價目表中所定義。 （這是與**OfferName**相同的欄位）。 | *PROJECT ONLINE PREMIUM （不含 PROJECT CLIENT）* |
| BillingCycleType | 一次性計費頻率。| *每月* |
