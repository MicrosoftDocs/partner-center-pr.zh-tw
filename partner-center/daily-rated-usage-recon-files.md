---
title: 每日評分的使用量對帳檔案 |合作夥伴中心
ms.topic: article
ms.date: 11/21/2019
description: 瞭解合作夥伴中心內每日評分的使用量調節檔案。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389696"
---
# <a name="daily-rated-usage-reconciliation-files"></a>每日評分的使用量對帳檔案

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

本主題說明如何閱讀每日分級的使用量對帳檔案。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>每日分級使用量對帳檔案中的欄位

| 欄 | 描述 |
| ------ | ----------- |
| PartnerId | GUID 格式的合作夥伴識別碼。 |
| PartnerName | 夥伴名稱。 |
| CustomerId | 客戶的唯一 Microsoft 識別碼（GUID 格式）。 |
| CustomerCompanyName | 合作夥伴中心中回報的客戶組織名稱。 *此資料行非常重要，因為它會將發票與您的系統資訊進行協調。* |
| CustomerDomainName | 客戶的功能變數名稱。 目前的活動無法使用。 |
| 客戶國家/地區 | 客戶所在的國家/地區。 |
| MPNID | CSP 合作夥伴的 MPN 識別碼。 |
| 轉售商 MPNID | 訂用帳戶之記錄轉銷商的 MPN 識別碼。 目前的活動無法使用。 |
| InvoiceNumber | 交易的指定位置顯示的發票號碼。 目前的活動無法使用。 |
| ProductId | 產品的識別碼。 |
| SkuId | 特定 SKU 的識別碼。 |
| AvailabilityId | 特定 SKU 可用性的識別碼。 這會顯示 SKU 是否可在指定的國家/地區、貨幣、產業區段等中購買。 |
| SKU 名稱 | 特定 SKU 的標題。 |
| PublisherName | 發行者的名稱。 |
| PublisherID | GUID 格式的發行者識別碼。 目前的活動無法使用。 |
| 訂用帳戶描述 | 客戶購買的服務優惠名稱，如價目表中所定義。 （這是與**OfferName**相同的欄位）。 |
| [訂閱識別碼] | 訂閱在 Microsoft 帳單平台中的唯一識別碼。 不用於對帳。 *此識別碼與合作夥伴系統管理員主控台上的訂用帳戶**ID**不同。* |
| ChargeStartDate | 計費週期的開始日期（除了向先前的計費週期中呈現先前不收費潛在使用量資料的日期以外）。 時間一律是一天的開始時間 (0:00)。 |
| ChargeEndDate | 計費週期的結束日期（除了向先前的 biling 迴圈呈現先前不收費潛在使用量資料的日期以外）。 時間一律是一天的結束時間 (23:59)。 |
| 使用日期 | 服務使用量的日期。 |
| 計量類型 | 計量的類型。 |
| 計量類別 | 使用的最上層服務。 |
| 計量識別碼 | 所使用之計量的識別碼。 |
| 計量子類別 | 可能會影響費率的 Azure 服務類型。 |
| 計量名稱 | 所耗用計量的測量單位。 |
| 計量區域 | 此欄可識別適用及填入此項目之服務地區內的資料中心的位置。 |
| 單位 | 資源**名稱**的單位。 |
| 已耗用數量 | 報告期間所耗用的服務數量（例如*小時*或*GB*）。 包含先前報告期間的任何未開立帳單使用量。 |
| 資源位置 | > 計量執行所在的資料中心。 |
| 已使用服務 | 您所使用的 Azure 平臺服務。 |
| 資源 URI | 所使用資源的 URI。 |
| 收費類型 | 費用或調整的類型。 目前的活動無法使用。 |
| 單價 | 每個授權的價格，如購買時的價格清單中所發佈。 請確定此價格符合您的計費系統中儲存的資訊。 |
| 數量 | 授權數目。 請確定此價格符合您的計費系統中儲存的資訊。 |
| 單位類型 | 計量計費的單位類型。 目前的活動無法使用。 |
| 計費預付稅 | 稅金前的帳單總金額。 |
| 計費貨幣 | 客戶地理區域中的貨幣。 |
| 定價稅前總計 | 新增稅額前的價格。 |
| 定價貨幣 | 價格清單中的貨幣。 |
| 服務資訊1 | 在指定一天布建和使用的服務匯流排連接數目。 |
| 服務資訊2 | 舊版欄位，可捕捉選擇性的服務特定中繼資料。 |
| 其他資訊 | 其他資料行中未涵蓋的任何其他資訊。 |
