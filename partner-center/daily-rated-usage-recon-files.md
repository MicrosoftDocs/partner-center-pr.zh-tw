---
title: 每日分級的使用量對帳檔案
ms.topic: article
ms.date: 06/12/2020
description: 瞭解如何在合作夥伴中心中讀取每日分級的使用量對帳檔案。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bff2c66e7efd05631de7d7643a780cbe5f726103
ms.sourcegitcommit: 3670c6e7f22e4f56545886052b68b9d5b6b3092c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/01/2020
ms.locfileid: "89281310"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>瞭解如何在合作夥伴中心中讀取每日分級的使用量對帳檔案

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 銷售代理人
- 技術服務代理人

本文說明如何讀取每日分級的使用量對帳檔案。

>[!NOTE]
>每日分級的使用量通常需要24小時才會出現在合作夥伴中心中，或透過 API 存取。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>每日分級的使用量對帳檔案中的欄位

| 資料行 | 描述 |
| ------ | ----------- |
| PartnerId | GUID 格式的合作夥伴識別碼。 |
| PartnerName | 合作夥伴名稱。 |
| CustomerId | GUID 格式的客戶唯一的 Microsoft 識別碼。 |
| CustomerName | 如合作夥伴中心報告的客戶組織名稱。 *此資料行對於使用您的系統資訊來協調發票而言很重要。* |
| CustomerDomainName | 客戶的功能變數名稱。 |
| CustomerCountry | 客戶所在的國家/地區。 |
| MpnId | MPN CSP 合作夥伴的識別碼。 |
| Tier2MpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 |
| InvoiceNumber | 出現指定交易的發票號碼。 |
| ProductId | 產品的識別碼。 |
| SkuId | 特定 SKU 的識別碼。 |
| AvailabilityId | 特定 SKU 可用性的識別碼。 此資料行會顯示 SKU 是否可在指定的國家/地區、貨幣、產業區段等中進行購買。 |
| SkuName | 特定 SKU 的標題。 |
| ProductName | 產品的名稱。 |
| PublisherName | 發行者的名稱。 |
| PublisherId | GUID 格式之發行者的識別碼。 |
| SubscriptionDescription | 客戶購買的服務優惠名稱，如價目表中所定義。  (這個資料行是 **OfferName**) 的相同欄位。 |
| SubscriptionId | Microsoft 計費平台中訂用帳戶的唯一識別碼。 未用於對帳。 *此識別碼與夥伴管理主控台上的 **訂** 用帳戶識別碼不同。* |
| ChargeStartDate |  (計費週期的開始日期，但在呈現先前的計費週期中，不收費潛在使用量資料的日期) 。 此時間一律為第一天的開始時間，即 0:00。 |
| ChargeEndDate | 計費週期的結束日期 (，但在呈現先前的計費週期中不收費潛在使用量資料的日期) 。 時間一律是一天的結束時間 (23:59)。 |
| UsageDate | 服務使用量的日期。 |
| MeterType | 計量類型。 |
| MeterCategory | 使用量的最上層服務。 |
| 計量識別碼 | 所要使用之計量的識別碼。 |
| MeterSubCategory | 可能會影響費率的 Azure 服務類型。 |
| MeterName | 所耗用計量的測量單位。 |
| MeterRegion | 此資料行會識別 MeterRegion 適用和擴展之服務區域內的資料中心位置。 |
| 單位 | 資源 **名稱**的單位。 |
| ResourceLocation | 正在執行計量的資料中心。 |
| ConsumedService | 您所使用的 Azure 平台服務。 |
| ResourceGroup | 表示保存 Azure 解決方案相關資源的容器。 |
| ResourceURI | 所使用資源的 URI。 |
| ChargeType | 費用或調整的類型。  |
| UnitPrice | 每一授權的價格（依購買時的價格清單發佈）。 請確定此價格符合您的計費系統中儲存的資訊（在對帳期間）。 |
| 數量 | 授權數目。 請確定此價格符合您的計費系統中儲存的資訊（在對帳期間）。 |
| Unittype.pixel 表示 | 計量計費單位的單位類型。  |
| BillingPreTaxTotal | 稅金前的帳單總金額。<br/> _**BillingPreTaxTotal** = FLOOR ( # A1 [ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ] ) ，2) _ |
| BillingCurrency | 客戶地理區域中的貨幣。 |
| PricingPreTaxTotal | 在稅金新增之前的定價。 |
| PricingCurrency | 價格清單中的貨幣。 |
| ServiceInfo1 | 在指定的一天布建和使用的服務匯流排連接數目。 |
| ServiceInfo2 | 舊版欄位，可捕獲選擇性的服務特定中繼資料。 |
| 標籤 | 代表使用者所設定之 Azure 資源的邏輯組織。 |
| AdditionalInfo | 任何未涵蓋於其他資料行中的其他資訊。 |
| EffectiveUnitPrice | 依單位計費的實際值，包括任何折扣、獲得的點數等等。 |
| PCToBCExchangeRate | 定價貨幣適用于計費貨幣的匯率。 |
| PCToBCExchangeRateDate | 判斷帳單貨幣的定價貨幣的日期。 |
| EntitlementId | 代表 Azure 訂用帳戶識別碼。 |
| EntitlementDescription | 代表 Azure 訂用帳戶識別碼的名稱。 |
| PartnerEarnedCreditPercentage | 顯示明細專案的 PartnerEarnedCredit。 獲得的點數將會是0或15% |

>[!NOTE]
>每日評等使用量通常需要24小時才會出現在合作夥伴中心中，或透過 API 來存取。


