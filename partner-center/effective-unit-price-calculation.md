---
title: 有效單位價格計算
ms.topic: how-to
ms.date: 11/10/2020
description: 深入瞭解有效的單位價格和其計算方式。 本文也包含範例計算。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556322"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>適用于 Azure 方案耗用量的有效單位價格計算

## <a name="the-effective-unit-price"></a>有效單位價格

有效單位價格是在計量層級 (計算，而不是資源層級) ，而且會根據計量使用量進行每日調整。

我們會使用下列三個因素來計算有效的單價：

- 在整個計費週期內每天監視的耗用量
- 計量的計費成本
- 分層 (（如果適用）) 

由於我們每天都會監視計費週期的耗用量，因此有效的單位價格將會波動。 在停止耗用量計算並關閉計費期間之後，將可使用指定計費週期的最終價格。 您將會看到在第四或第五個小數位數之後的耗用量變更。

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>瞭解您的計量是否使用分層定價

如果您不知道您的計量是否使用分層定價，請使用下列程式來找出。 

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。
2. 選取 [ **銷售**]、選取 [ **定價和** 供應專案]，然後選取 [ **Azure 方案定價**]。
3. 依識別碼找出您的計量，然後下載您的定價資料。 

## <a name="sample-calculation"></a>範例計算

下表提供如何在開啟期間計算有效單位價格的範例。

在資料表中，下列值適用： 

- **高** = 資源/小時的單位價格 = 0.868

- **BCU** = 計量的計費耗用量單位

- **BC** = 計量 = BCU * UP * 0.85 的計費成本。 這會反映 15% PEC 折扣的調整。 接著，我們會使用函式的下限，將值限制在小數點後面的兩位數，以收費最小金額。 

- **有效單位價格** = BCU/BC

>[!NOTE]
>注意：此範例中的計量表沒有定價層。

| Date | BCU (計費耗用量單位)  | BC (計費成本)  | 有效單位價格 |
| ------ | ----------- | ----------- | ----------- |  
| 3-8 月 | 29 | 21.39 | 0.737586206896552 |
| 10-8 月 | 210.950039 | 155.63 | 0.737757626107858 |
| 25-8 月 | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>後續步驟

- [帳單與稅金](billing.md)
