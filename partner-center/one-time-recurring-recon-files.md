---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389676"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Column | 說明 |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. 在所有資料列中都是如此。 |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| [客戶名稱] | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. 在下一個帳單週期之前，此欄位會是空白的。 *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | 客戶所在的國家/地區。 |
| 發票號碼 | 交易的指定位置顯示的發票號碼。 |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| 訂單識別碼 | Unique identifier for an order in the Microsoft commerce platform. Not used for reconciliation. |
| 訂單日期 | 下訂單的日期。 |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 特定 SKU 的標題。 |
| [產品名稱] | 產品的名稱。 |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | Friendly name of a subscription. |
| [訂閱識別碼] | Unique identifier for a subscription in the Microsoft commerce platform. Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | 開始計算費用的日期。 時間一律是一天的開始時間 (0:00)。 |
| ChargeEndDate | 結束計算費用的日期。 時間一律是一天的結束時間 (23:59)。 |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| 收費類型 | 費用或調整的類型。 |
| 單價 | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | The unit price after adjustments have been made. |
| 數量 | Number of units. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | The type of unit being purchased. |
| DiscountDetails | An explanation of any applicable discount. |
| Sub Total | 稅前總計。 Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| 總計 | 稅後總計。 檢查發票中是否向您收取稅金。 |
| Currency | 貨幣類型。 每一帳單實體都只有一種貨幣。 Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
