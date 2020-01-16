---
title: 每日評分的使用量對帳檔案 |合作夥伴中心
ms.topic: article
ms.date: 01/14/2020
description: 瞭解如何在合作夥伴中心讀取每日分級的使用量對帳檔案。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a9c7f328cf1a10b4a23aeb775524d5931bdbb703
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021722"
---
# <a name="daily-rated-usage-reconciliation-files"></a>每日評分的使用量對帳檔案

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**

- 系統管理代理人
- 帳單管理
- 銷售代理人
- 技術服務代理人

本主題說明如何閱讀每日分級的使用量對帳檔案。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>每日分級使用量對帳檔案中的欄位

| 欄位 | 說明 |
| ------ | ----------- |
| PartnerId | GUID 格式的合作夥伴識別碼。 |
| PartnerName | 合作夥伴名稱。 |
| CustomerId | 客戶的唯一 Microsoft 識別碼（GUID 格式）。 |
| CustomerName | 合作夥伴中心中回報的客戶組織名稱。 *此資料行非常重要，因為它會將發票與您的系統資訊進行協調。* |
| CustomerDomainName | 客戶的功能變數名稱。 |
| CustomerCountry | 客戶所在的國家/地區。 |
| MpnId | CSP 合作夥伴的 MPN 識別碼。 |
| Tier2MpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 |
| InvoiceNumber | 交易的指定位置顯示的發票號碼。 |
| ProductId | 產品的識別碼。 |
| SkuId | 特定 SKU 的識別碼。 |
| AvailabilityId | 特定 SKU 可用性的識別碼。 這會顯示 SKU 是否可在指定的國家/地區、貨幣、產業區段等中購買。 |
| SkuName | 特定 SKU 的標題。 |
| ProductName | 產品的名稱。 |
| PublisherName | 發行者的名稱。 |
| PublisherId | GUID 格式的發行者識別碼。 |
| SubscriptionDescription | 客戶購買的服務優惠名稱，如價目表中所定義。 （這是與**OfferName**相同的欄位）。 |
| SubscriptionId | 訂閱在 Microsoft 帳單平台中的唯一識別碼。 不用於對帳。 *此識別碼與合作夥伴系統管理員主控台上的訂用帳戶**ID**不同。* |
| ChargeStartDate | 計費週期的開始日期（除了向先前的計費週期中呈現先前不收費潛在使用量資料的日期以外）。 時間一律是一天的開始時間 (0:00)。 |
| ChargeEndDate | 計費週期的結束日期（除了向先前的 biling 迴圈呈現先前不收費潛在使用量資料的日期以外）。 時間一律是一天的結束時間 (23:59)。 |
| UsageDate | 服務使用量的日期。 |
| MeterType | 計量的類型。 |
| MeterCategory | 使用的最上層服務。 |
| MeterId | 所使用之計量的識別碼。 |
| MeterSubCategory | 可能會影響費率的 Azure 服務類型。 |
| MeterName | 所耗用計量的測量單位。 |
| MeterRegion | 此欄可識別適用及填入此項目之服務地區內的資料中心的位置。 |
| 單位 | 資源**名稱**的單位。 |
| ResourceLocation | 正在執行計量的資料中心。 |
| ConsumedService | 您所使用的 Azure 平台服務。 |
| ResourceGroup | 代表保存 Azure 解決方案相關資源的容器。 |
| ResourceURI | 所使用資源的 URI。 |
| ChargeType | 費用或調整的類型。  |
| UnitPrice | 每個授權的價格，如購買時的價格清單中所發佈。 請確定此價格符合您的計費系統中儲存的資訊。 |
| 數量 | 授權數目。 請確定此價格符合您的計費系統中儲存的資訊。 |
| Unittype.pixel 表示 | 計量計費的單位類型。  |
| BillingPreTaxTotal | 稅金前的帳單總金額。 |
| BillingCurrency | 客戶地理區域中的貨幣。 |
| PricingPreTaxTotal | 新增稅額前的價格。 |
| PricingCurrency | 價格清單中的貨幣。 |
| ServiceInfo1 | 在指定一天布建和使用的服務匯流排連接數目。 |
| ServiceInfo2 | 舊版欄位，可捕捉選擇性的服務特定中繼資料。 |
| 標記 | 代表使用者所設定之 Azure 資源的邏輯組織。 |
| AdditionalInfo | 其他資料行中未涵蓋的任何其他資訊。 |
| EffectiveUnitPrice | 每個單位的實際值，包括任何折扣、取得的點數等。 |
| PCToBCExchangeRate | 定價貨幣對計費貨幣的匯率。 |
| PCToBCExchangeRateDate | 決定計費貨幣的定價貨幣的日期。 |
| EntitlementId | 代表 Azure 訂用帳戶識別碼。 |
| EntitlementDescription | 代表 Azure 訂用帳戶識別碼的名稱。 |
| PartnerEarnedCreditPercentage | 顯示行專案的 PartnerEarnedCredit。 獲得的點數會是0或15% |
