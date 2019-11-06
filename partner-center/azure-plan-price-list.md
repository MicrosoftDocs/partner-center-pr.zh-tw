---
title: Azure 方案價目表 | 合作夥伴中心
ms.topic: article
ms.date: 11/01/2019
description: 如何查看 Azure 方案下訂用帳戶的價目表
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 53e5327b505de1c1860e44b477aca21b5aef2d2b
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428543"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>適用於 Azure 的 CSP 中新商務體驗的價目表 

CSP 中新 Azure 商務體驗的價目表會張貼在合作夥伴中心。 價目表會以即時精確的檔案動態傳遞，而且價格只會以美元顯示。 不過，計費是以適用於客戶貨幣位置的支援貨幣來完成。 如需有關客戶貨幣位置計費的詳細資訊，請參閱 [Azure 方案 - 計費](azure-plan-billing.md)。

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>請參閱 Azure 方案定價下的訂用帳戶定價

1. 從左側的 [合作夥伴中心] 功能表中，選取 [銷售]  ，然後選取 [市集]  。

2. 在 [匯出類型]  旁，選取 [Azure 方案使用定價]  。

3. 在 [日期定價]  旁，選取您想要的日期，例如 [目前]  。 注意：您也可以選取 [FX 費率]  以匯出目前的 FX 費率。

![Azure 定價 2](images/azure/pricelist2.jpg)

4. 在 [市集]  底下選取產品的 [類型]  和 [類別]  ，或搜尋產品。 以您的搜尋為基礎的可用產品隨即顯示。

![定價](images/azure/Azurepricelist1.jpg)

5. 然後選取 [匯出 Azure 方案價目表]  ，以下載您所選產品的 Azure 方案價格。


![匯出價目表](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Azure 價目表詳細資訊

- 您可以從 [合作夥伴中心] 的 [市集] 頁面的 [銷售]  底下，取得 Azure 方案定價。

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
|市場|定價的市場|
|貨幣|定價的貨幣|
|UnitPrice|每一單位價格|
|PricingTierRangeMin|針對分層定價，適用的最低價格|
|PricingTierRangeMax|針對分層定價，適用的最高價格|
|EffectiveStartDate|定價的開始日期|
|EffectiveEndDate|定價的結束日期|
|MeterIds|產品 SKU 的計量識別碼|
|MeterType|計量類型|
|標記|項目的屬性，對於 Azure 方案定價，這會是 Azure 或 Azure 和 Reservations (特別適用於保留)|

詳細的[價目表資訊](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
