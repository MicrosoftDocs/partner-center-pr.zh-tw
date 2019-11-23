---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389616"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00 |

2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |循環費用   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Change license quantity

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00    |

您在 2 月 1 日將授權數量從一個增加為兩個。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |循環執行個體 (依比例計算)   |-4.00       |1        |-4.00   |
|1/13/2018         |1/31/2018    | 循環執行個體 (依比例計算)   |2.45       |1        |2.45    |
|2/1/2018         |2/12/2018    | 循環執行個體 (依比例計算)   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | 循環執行個體 (依比例計算)   |4.00       |2        |8.00    |

每月價格是 4.00，服務期間 1/13/2018 – 2/12/2018 共有 31 天。 等於每天價格 0.129 (4/31)。

1/13/2018 – 1/31/2018 期間按比例計算有 19 天。

按比例計算單價 = 2.451 = 19 x 0.129

2/1/2018 – 2/12/2018 期間按比例計算有 12 天。

按比例計算單價 = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00    |

On February 1 you suspend a subscription. 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|取消費用|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|循環費用|4.00|1|4.00

2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|循環費用|4.00|1|4.00

您在 3 月 1 日暫停訂閱。 3 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|取消費用|-1.72|1|-1.72

每月價格是 4.00，服務期間 2/13/2018 – 3/12/2018 共有 28 天。 等於每天價格 0.143 (4/28)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

3/1/2018 – 3/12/2018 的取消期間有 12 天。

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).
