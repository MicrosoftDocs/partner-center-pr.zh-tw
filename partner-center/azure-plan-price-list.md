---
title: CSP 合作夥伴的 Azure 方案價目表
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 方案合作夥伴如何使用合作夥伴中心查看 Azure 方案下訂用帳戶的價目表。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: acf8a26960df0bebd97b8684c5a51173a86af416
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84452605"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>適用於 Azure 的 CSP 中新商務體驗的價目表

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員
- 技術服務代理人
- 銷售代理人
- 使用者管理系統管理員

CSP 中新 Azure 商務體驗的價目表會張貼在合作夥伴中心。 價目表會以即時精確的檔案動態傳遞，而且價格只會以美元顯示。 不過，計費是以適用於客戶貨幣位置的支援貨幣來完成。 如需有關客戶貨幣位置計費的詳細資訊，請參閱 [Azure 方案 - 計費](azure-plan-billing.md)。

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>請參閱 Azure 方案定價下的訂用帳戶定價

1. 從左側的 [合作夥伴中心] 功能表中，選取 [銷售]，然後選取 [市集]。

2. 在 Azure 方案定價底下，選取您想要定價的國家/地區。

3. 在 [匯出類型] 旁邊，選取 [Azure 方案使用定價]、[Azure 方案保留定價] 或 [FX 費率]。 注意：[FX 費率] 不是國家/地區特有。

4. 在 [日期定價] 旁，選取您想要的日期，例如 [目前]。

   :::image type="content" source="images/azure/pricingnew.png" alt-text="國家/地區特有":::

注意：您可以匯出兩個不同的價目表 - Azure 方案定價和市集協力廠商定價。

## <a name="azure-price-list-specifics"></a>Azure 價目表詳細資訊

- 您可以從 [合作夥伴中心] 的 [市集] 頁面的 [銷售] 底下，取得 Azure 方案定價。

- 匯出適用於 Azure 方案使用服務、Azure Reservations 和 FX 費率。

- 匯出的選項包括：

  - **今天的定價**：這包括從當月 1 日到當月目前日期的所有計量和定價。 這包括新的價格、已變更的價格或已移除的價格。 所有價格都有有效的開始和結束日期，以說明其為新增或移除。

  - **上個月的定價**：每個資源類型的下載都會依月份。 對於定價檔案，這會包含在該月份期間可用的所有計量。 如果在當月中間出現新的計量，我會顯示為具有有效日期 (反映其可用性) 的計量。 已停止的價格也類似，會顯示有效的結束日期，說明何時無法再使用。

  - **FX 費率**：FX 費率將於每月 1 日之前 (下午 6 點 PST) 提供下載。 例如，如果您想要 11 月的費率，請在 10 月 31 日下載費率。 您也可以使用上個月的 FX 費率。

- 價目表中的價格是直接價格。 某些合作夥伴可能符合合作夥伴所獲得信用點數的資格。 如需合作夥伴所獲得信用點數如何計算的相關資訊，請參閱[合作夥伴所獲得信用點數如何計算及付費](partner-earned-credit-explanation.md)。

- **合格的服務**：合作夥伴所獲得信用點數適用於 **Azure 方案使用定價**中所列的服務，合作夥伴可以從 [Azure 方案定價](https://partner.microsoft.com/commerce/sales)頁面匯出。 請注意，有一些例外狀況，包括 (但不限於) Azure 方案使用價目表和 Azure 方案保留的 [標記] 資料行中，識別為 [協力廠商] 的協力廠商產品。

## <a name="price-list-data"></a>價目表資料

|**欄位**   |**描述**   |
|--------------------------|:---------------------------|
|ProductTitle  |產品的標題或名稱|
|ProductID   |產品識別碼|
|SKuId|SKU 的識別碼|
|SkuTitle|SKU 的標題或名稱|
|發行者|第一方一律是 Microsoft|
|SkuDescription|SKU 的描述|
|UnitOfMeasure|收取費用或計費的單位|
|TermDuration|針對期間型的產品，期間的長度，適用於保留|
|Market|定價的市場|
|貨幣|定價的貨幣|
|UnitPrice|每一單位價格|
|PricingTierRangeMin|針對分層定價，適用的最低價格|
|PricingTierRangeMax|針對分層定價，適用的最高價格|
|EffectiveStartDate|定價的開始日期|
|EffectiveEndDate|定價的結束日期|
|MeterIds|產品 SKU 的計量識別碼|
|MeterType|計量類型|
|標記|項目的屬性，對於 Azure 方案定價，這會是 Azure 或 Azure 和 Reservations (特別適用於保留)|

Azure 方案的價目表可以從 [Azure 方案定價和 Marketplace 頁面](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)匯出

## <a name="pricing-api-for-azure-plan"></a>Azure 方案的定價 API

您可以使用[定價 API](https://docs.microsoft.com/partner/develop/pricing)，透過程式設計來擷取 Azure 方案的取用和保留定價。 您也可以擷取外幣匯率。

定價 API 所在的端點與其他合作夥伴中心的 API 不同。 定價資訊包含 Azure 方案資源的計量定價 (以美元為單位) 以及適用於 Azure 方案訂用帳戶的保留定價。

此 API 也可讓合作夥伴擷取每月匯率，原因則是 Azure 方案僅以美元定價。 您可以使用 API 來擷取當月或先前月份的定價和外幣匯率。

>[!NOTE]
> 定價 API 是用於 Azure 方案定價的專屬 API。 針對 Azure 資源或部署至非 Azure 方案訂用帳戶的保留，則仍請使用合作夥伴中心 [定價與供應項目] 頁面中所公佈的現有 RateCard API 和價目表。 Azure 方案定價 API 不支援軟體、市集或基座型定價，例如 Microsoft 365 或 Dynamics 365。

如需 Azure 方案定價和外幣匯率 API 的詳細資訊，請參閱完整的[定價 API 文件](https://docs.microsoft.com/partner/develop/pricing)。
