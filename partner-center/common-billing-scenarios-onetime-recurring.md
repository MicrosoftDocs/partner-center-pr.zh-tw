---
title: Common billing scenarios for one-time and select recurring purchases | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for one-time and select recurring purchases (such as purchasing subscriptions, adding more subscriptions, adding and removing seats).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389636"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>One-time and select recurring purchase billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Purchase a subscription and add a seat on the same day

在案例 1，您在 6 月 11 日以 $4 美元的單價購買一個訂用帳戶。 同一天稍晚，您以相同的價格購買另一個相同的訂用帳戶。

對帳檔案會包含下列內容：

- 6 月 10 日 – 7 月 9 日服務期間的 $4 美元帳單。
- 6 月 11 日 - 7 月 11 日服務期間的 $-4.00 美元依比例計算的重新計費。 這是您擁有 1 個授權的期間。 計算 = (每月價格/服務期間總天數) x 依比例計算的服務期間天數 x 授權數目 = (4/30) x 30 x 1 = 4.00。
- 6 月 10 日 - 7 月 9 日服務期間的 $8.00 美元依比例計算的重新計費。 這是您擁有 2 個授權的期間。 計算 = (4/30) x 30 x 2 = 8.00。

|**購買日期**   |**收費開始** |**收費結束**  |**單價**  |**數量**  |**金額** |**收費類型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |新的         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Purchase a subscription and add more subscriptions later

在案例 2，您在 6 月 11 日以單價 $4 美元購買一個訂用帳戶，而在 6 月 12 日您以相同價格針對相同產品購買另一個訂用帳戶。

對帳檔案會包含下列內容：

- 6 月 10 日 – 7 月 9 日服務期間的 $4 美元帳單。
- 6 月 11 日 - 7 月 12 日服務期間的 $-3.87 美元依比例計算的重新計費。 這是您擁有 1 個授權的期間。 計算 = (每月價格/服務期間總天數) x 依比例計算的服務期間天數 x 授權數目 = (4/30) x 29 x 1 = 3.87。
- 6 月 12 日 - 7 月 9 日服務期間的 $7.74 美元依比例計算的重新計費。 這是您擁有 2 個授權的期間。 計算 = (4/30) x 29 x 2 = 7.74。

|**購買日期**   |**收費開始** |**收費結束**  |**單價**  |**數量**  |**金額** |**收費類型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (您有一份授權)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |新的         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3.87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7.74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Purchase a subscription and remove a seat on the same day

在案例 3，您在 6 月 11 日以 $4 美元的單價針對相同產品購買兩個訂用帳戶。 同一天稍晚，您移除其中一個基座。  

對帳檔案會包含下列內容：

- 6 月 10 日 – 7 月 9 日服務期間的 $8 美元帳單 (兩份授權)。
- 6 月 11 日 - 7 月 11 日服務期間的 $-8.00 美元依比例計算的重新計費。 這是您擁有 2 個授權的期間。 計算 = (每月價格/服務期間總天數) x 依比例計算的服務期間天數 x 授權數目 = (4/30) x 30 x 2 = 8.00。
- 6 月 11 日 - 7 月 9 日服務期間的 $4.00 美元依比例計算的重新計費。 這是您擁有 1 個授權的期間。 計算 = (4/30) x 30 x 1 = 4.00。

|**購買日期**   |**收費開始** |**收費結束**  |**單價**  |**數量**  |**金額** |**收費類型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |新的         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Purchase a subscription and remove seats later

在案例 4，您在 6 月 11 日以單價 $4 美元購買 2 個訂用帳戶，並在 6 月 12 日移除其中一個基座。

對帳檔案會包含下列內容：

- 6 月 10 日 – 7 月 9 日服務期間的 $8 美元帳單。
- 6 月 11 日 - 7 月 12 日服務期間的 $-7.74 美元依比例計算的重新計費。 這是您擁有 2 個授權的期間。 計算 = (每月價格/服務期間總天數) x 依比例計算的服務期間天數 x 授權數目 = (4/30) x 29 x 2 = 7.74。
- 6 月 12 日 - 7 月 9 日服務期間的 $3.87 美元依比例計算的重新計費。 這是您擁有 1 個授權的期間。 計算 = (4/30) x 29 x 1 = 3.87。

|**購買日期**   |**收費開始** |**收費結束**  |**單價**  |**數量**  |**金額** |**收費類型** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (您有 2 份授權)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |新的       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7.74       |removeQuantity           |
|6/12/2019 (您有 1 份授權)    | 6/10/2019    |7/09/2019   |$4    |1      |$3.87    |removeQuantity |
