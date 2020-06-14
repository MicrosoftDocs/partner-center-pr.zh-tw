---
title: 一次性和週期性的對帳檔案
ms.topic: article
ms.date: 05/26/2020
description: 瞭解合作夥伴中心一次性和週期性對帳檔案中每個欄位或資料行的意義。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84bed4fac8984b3fc8757b8185da514c5d8212d6
ms.sourcegitcommit: 0154eabccdc92d1fbe73734f5514f317b9e9fee0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/12/2020
ms.locfileid: "84749192"
---
# <a name="one-time-and-recurring-reconciliation-files-in-partner-center"></a>合作夥伴中心的一次性和週期性對帳檔案

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**

- 全域系統管理員
- 使用者系統管理員
- 帳單系統管理員
- 系統管理代理人
- 銷售代理人

本主題說明如何在合作夥伴中心讀取一次性和週期性的對帳檔案。

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>一次性和週期性對帳檔案中的欄位

| 資料行 | 描述 |
| ------ | ----------- |
| PartnerId | 特定計費實體的唯一 Azure Active Directory （Azure AD）租使用者識別碼（GUID 格式）。 不需要進行調整。 在所有資料列中都是如此。 |
| CustomerId | GUID 格式的唯一 Azure AD 租使用者識別碼。 識別客戶。 |
| CustomerName | 客戶的組織名稱（如合作夥伴中心所報告）。 |
| CustomerDomainName | 客戶的功能變數名稱。 在下一個帳單週期之前，此欄位會是空白的。 *請勿使用此欄位作為客戶的唯一識別碼。客戶/合作夥伴可以透過 Office 365 入口網站更新虛名或預設網域。* |
| CustomerCountry | 客戶所在的國家/地區。 |
| InvoiceNumber | 出現指定交易的發票號碼。 |
| MpnId | CSP 合作夥伴的 MPN 識別碼。 |
| OrderId | Microsoft 商務平臺中訂單的唯一識別碼。 不用於對帳。 |
| OrderDate | 下訂單的日期。 |
| ProductId | 產品的識別碼。 |
| SkuId | 特定 SKU （庫存單位）的識別碼。 |
| AvailabilityId | 特定 SKU 可用性的識別碼。 這會顯示 SKU 是否可在指定的國家/地區、貨幣、產業區段等中購買。 |
| SkuName | 特定 SKU 的標題。 |
| ProductName | 產品的名稱。 |
| ChargeType | 費用或調整的類型。 |
| UnitPrice | 購買時價格清單中所發佈的單價。 *請確定這符合您的計費系統中儲存的資訊。* |
| 數量 | 單位數目。 *請確定這符合您的計費系統中儲存的資訊。* |
| SubTotal | 稅前總計。 檢查您的小計是否符合您的預期總計（以折扣為例）。 |
| TaxTotal | 稅金金額費用。 根據您市場的稅務規則和特定情況。 |
| 總計 | 稅後總計。 檢查發票中是否向您收取稅金。 |
| 貨幣 | 貨幣類型。 每個計費實體都只有一個貨幣。 請確定這符合您的第一張發票，並在任何主要計費平臺更新之後再次檢查。 |
| PriceAdjustmentDescription | 任何適用折扣的說明。 |
| PublisherName | 產品發行者的名稱。
| PublisherId | 特定發行者的唯一識別碼。 |
| SubscriptionDescription | 訂用帳戶的易記名稱。 |
| SubscriptionId | Microsoft commerce 平臺中訂用帳戶的唯一識別碼。 不用於對帳。 *此識別碼與合作夥伴系統管理員主控台上的訂用帳戶**ID**不同。* |
| ChargeStartDate | 開始計算費用的日期。 此時間一律為第一天的開始時間，即 0:00。 |
| ChargeEndDate | 結束計算費用的日期。 時間一律是一天的結束時間 (23:59)。 |
| TermAndBillingcycle | 購買的詞彙長度和計費週期（例如， *1 年、每月*）。 |
| EffectiveUnitPrice | 進行調整後的單位價格。 |
| Unittype.pixel 表示 | 所購買的單位類型。 |
| 替代識別碼 | **訂單**識別碼的替代識別碼。 |
| BillableQuantity | 代表已購買或耗用的單位總數。 |
| BillingFrequency | 描述明細專案是每月或一次性計費頻率。 *這目前僅支援 Azure RI，每月支援的值為。如果 RI 以一次性計費頻率購買，偵察檔案中的這個欄位將會顯示為空白。* |
| PricingCurrency | 資源或供應專案的標價。 |
| PCToBCExchangeRate | 定價貨幣對計費貨幣的匯率。 |
| PCToBCExchangeRateDate | 決定計費貨幣的定價貨幣的日期。 |
| MeterDescription | 耗用量明細專案的計量描述。 |
