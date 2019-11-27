---
title: 一次性和週期性的對帳檔案 |合作夥伴中心
ms.topic: article
ms.date: 11/21/2019
description: 瞭解合作夥伴中心內的一次性和週期性對帳檔案。
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
# <a name="one-time-and-recurring-reconciliation-files"></a>一次性和週期性的對帳檔案

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

本主題說明如何在合作夥伴中心讀取一次性和週期性的對帳檔案。

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>一次性和週期性對帳檔案中的欄位

| 欄 | 描述 |
| ------ | ----------- |
| PartnerId | 特定計費實體的唯一 Azure Active Directory （Azure AD）租使用者識別碼（GUID 格式）。 不需要進行調整。 在所有資料列中都是如此。 |
| 客戶識別碼 | GUID 格式的唯一 Azure AD 租使用者識別碼。 識別客戶。 |
| [客戶名稱] | 客戶的組織名稱（如合作夥伴中心所報告）。 |
| CustomerDomainName | 客戶的功能變數名稱。 在下一個帳單週期之前，此欄位會是空白的。 *請勿使用此欄位作為客戶的唯一識別碼。客戶/合作夥伴可以透過 Office 365 入口網站更新虛名或預設網域。* |
| 客戶國家/地區 | 客戶所在的國家/地區。 |
| 發票號碼 | 交易的指定位置顯示的發票號碼。 |
| MpnId | CSP 合作夥伴的 MPN 識別碼。 |
| 轉售商 MpnId | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 |
| 訂單識別碼 | Microsoft 商務平臺中訂單的唯一識別碼。 不用於對帳。 |
| 訂單日期 | 下訂單的日期。 |
| ProductId | 產品的識別碼。 |
| SkuId | 特定 SKU （庫存單位）的識別碼。 |
| AvailabilityId | 特定 SKU 可用性的識別碼。 這會顯示 SKU 是否可在指定的國家/地區、貨幣、產業區段等中購買。 |
| SKU 名稱 | 特定 SKU 的標題。 |
| [產品名稱] | 產品的名稱。 |
| PublisherName | 產品發行者的名稱。
| PublisherID | 特定發行者的唯一識別碼。 |
| 訂用帳戶描述 | 訂用帳戶的易記名稱。 |
| [訂閱識別碼] | Microsoft commerce 平臺中訂用帳戶的唯一識別碼。 不用於對帳。 *此識別碼與合作夥伴系統管理員主控台上的訂用帳戶**ID**不同。* |
| ChargeStartDate | 開始計算費用的日期。 時間一律是一天的開始時間 (0:00)。 |
| ChargeEndDate | 結束計算費用的日期。 時間一律是一天的結束時間 (23:59)。 |
| 詞彙和 Billingcycle | 購買的詞彙長度和計費週期（例如， *1 年、每月*）。 |
| 收費類型 | 費用或調整的類型。 |
| 單價 | 購買時價格清單中所發佈的單價。 *請確定這符合您的計費系統中儲存的資訊。* |
| 有效單位價格 | 進行調整後的單位價格。 |
| 數量 | 單位數。 *請確定這符合您的計費系統中儲存的資訊。* |
| 單位類型 | 所購買的單位類型。 |
| DiscountDetails | 任何適用折扣的說明。 |
| 子總計 | 稅前總計。 檢查您的小計是否符合您的預期總計（以折扣為例）。 |
| 稅金總計 | 稅金金額費用。 根據您市場的稅務規則和特定情況。 |
| 總計 | 稅後總計。 檢查發票中是否向您收取稅金。 |
| Currency | 貨幣類型。 每一帳單實體都只有一種貨幣。 請確定這符合您的第一張發票，並在任何主要計費平臺更新之後再次檢查。 |
| 替代識別碼 | **訂單**識別碼的替代識別碼。 |
