---
title: 偵察 CSP 單次購買的檔案欄位
ms.topic: conceptual
ms.date: 11/10/2020
description: 在合作夥伴中心中，瞭解 CSP 單次採購對帳檔案中的所有專案，包括範例值。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 29574dad6c3dd5eedbcf93dd555509cb04144ef5
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182574"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP 一次性採購對帳檔案欄位

## <a name="using-the-recon-file"></a>使用偵察檔案
下表提供適用于 CSP 一次性購買的對帳檔案中欄位的描述和範例值。

如需對等檔的詳細資訊，請參閱 [使用對帳](use-the-reconciliation-files.md)檔案。

| Column | 描述 | 範例值 |
| ------ | ----------- | ------------ |
| PartnerId | 特定帳單實體之 GUID 格式的唯一識別碼。 不需要進行對帳。 在所有資料列中都是如此。 | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | GUID 格式的客戶唯一的 Microsoft 識別碼。 | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | 如合作夥伴中心報告的客戶組織名稱。 此資料行對於使用您的系統資訊來協調發票而言很重要。 | *強尼現代化的 DE2* |
| CustomerDomainName | 客戶的功能變數名稱。 | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 您的客戶所在的國家/地區。 查看您所在地區的 [國家/地區完整清單](./regional-authorization-overview.md) 。  | *德* |
| InvoiceNumber | 與對等檔相關聯的發票號碼。  | *G002297372* |
| MpnId | MPN CSP 合作夥伴的識別碼。 如需詳細資訊，請參閱 [如何依合作夥伴進行](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)詳細資料。 | *6034453* |
| ResellerMpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 | *6048879* |
| OrderId | Microsoft 計費平台中訂單的唯一識別碼。 在聯繫支援時識別訂單可能很有用。 未用於對帳。 | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 訂單的放置日期。 | *10/3/2020* |
| ProductId | 產品的唯一識別碼。 | *DZH318Z0BNZ5* |
| SkuId | SKU 的唯一識別碼。 | *006G* |
| AvailabilityId | 可用性唯一識別碼。 | *DZH318Z08B80* |
| SkuName | SKU 名稱。 | *資料表-LRS* |
| ProductName | 產品名稱。 | *資料表* |
| ChargeType | 費用或調整的 [類型](./recon-file-charge-types.md) 。 | *新增* |
| UnitPrice | 每一授權的價格（依購買時的價格清單發佈）。 請確定此專案符合您的計費系統中儲存的資訊。 | *0.045* |
| 數量 | 授權數目。 請確定此專案符合您的計費系統中儲存的資訊。 | *1* |
| 小計 | 稅前總計。 小計應等於可計費的數量乘以有效的單位價格。 | *0* |
| TaxTotal | 稅額費用。 根據您市場的稅務規則和特定情況。 | *0* |
| 總計 | 總金額等於小計加總稅額。 | *0* |
| 貨幣 | 您的帳單會在客戶的貨幣內容中產生。 這表示如果您是與不同可計費貨幣的客戶進行交易的合作夥伴，則會收到每個客戶貨幣類型的發票。  | *歐元* |
| PriceAdjustmentDescription | 單位價格的調整原因。 這些是主要原因，但不限於決定有效的單位價格。 | *[15.0% 合作夥伴為受管理的服務提供點數]* |
| PublisherName | 產品的發行者。  | *Microsoft* |
| PublisherId | 合作夥伴中心用來識別發行者的唯一識別碼。 | *那* |
| SubscriptionDescription | 客戶購買的服務優惠名稱，如價目表中所定義。 此資料行是與 OfferName 相同的欄位。 | *Azure 方案* |
| SubscriptionId | Microsoft 計費平台中訂用帳戶的唯一識別碼。 未用於對帳。 請注意，此識別碼與夥伴管理主控台上的訂用帳戶識別碼不同。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | 合作夥伴中心支付訂用帳戶費用的日期。 如果訂用帳戶是以年度計費期限和每月計費方案購買，則在第一個對帳檔案中，這是購買訂閱的日期。 從下一個對帳檔案開始，它會遞增30天。 | *9/1/2020* |
| ChargeEndDate | 訂用帳戶計費週期的結束日期。 如果訂用帳戶是以年度計費期限和每月計費方案購買，則在第一個對帳檔案中，這是購買訂閱之後的30天。 從下一個對帳檔案開始，它會遞增30天。 | *9/30/2020* |
| TermAndBillingCycle | 在購買時繼續訂用帳戶的持續時間。 | *每月儲存 (GB 的資料)* |
| EffectiveUnitPrice | 計算計費週期成本的按比例單位價格。 折扣、計費天數的調整，以及其他因素決定有效的單價。 如需詳細資訊，請參閱 [有效的單位價格計算](./effective-unit-price-calculation.md)。  | *0.03825* |
| Unittype.pixel 表示 | 計量計費的單位類型。 | *1 GB/月* |
| 替代識別碼 | 參考之訂單明細專案的替代識別碼。 | *6dc5c039750a* |
| BillableQuantity | 要計費的總數量。  | *0.005001* |
| BillingFrequency | 購買時選取的計費方案。 | *那*  |
| PricingCurrency | 價格清單中的貨幣。 | *美元* |
| PCToBCExchangeRate | 將定價貨幣套用至帳單貨幣的匯率。 | *0.846202666* |
| PCToBCExchangeRateDate | 判斷帳單貨幣的定價貨幣的日期。 | *9/30/2020* |
| MeterDescription | 計量描述。  | *資料表-LRS 儲存 (GB/月) 的資料* |
| ReservationOrderId | 保留訂單識別碼。 | *E21A6344E398FFC1C4D7...* |

## <a name="next-steps"></a>後續步驟

- [帳單與稅金](billing.md)