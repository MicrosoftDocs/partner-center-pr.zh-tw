---
title: 常見帳單案例 | 合作夥伴中心
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn what you will see on your bill after you add new subscriptions, adjust the number of licenses in a subscription, or cancel a subscription.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: d8afffa1dd11e386b03548c8f10e5490e6db5894
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253400"
---
# <a name="common-billing-scenarios"></a>一般帳單案例

**適用於**

-   Cloud Solution Provider program billing

這個主題將說明在您新增新訂閱、調整訂閱的授權數目，或取消訂閱後帳單上應該會看見的項目。 用量型和授權型訂閱受到的影響會有不同。

## <a name="in-this-section"></a>本節內容

-   [Usage-based billing](#usagebased)

-   [License-based billing](#licensebased)

## <a href="" id="usagebased"></a>Usage-based billing

用量型訂閱會在訂閱週年日，於每個月期後付款。 For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period December 15 - January 14. You will be charged again on February 15 for the service period January 15 - February 14, etc. The charges that are generated on the subscription anniversary day will appear on the following invoice and reconciliation file.

You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice. This is not an error; it simply means that the service was timestamped after the services occurred. Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill. 

Usage-based subscriptions may be suspended at any time. 

Azure 雲端解決方案提供者價目表每月發行一次，可在合作夥伴中心的 \[銷售\] -> \[定價與方案\] 頁面中找到。 請注意，價格可能每天變動，並會反映在價目表的 \[變更歷程記錄\] 索引標籤中。

使用量費用是以每日價格為準。 如果價格在服務期間變更，您會看到每一個依比例計算的服務期間和適用價格的計費明細。

## <a href="" id="licensebased"></a>License-based billing

**帳單：** 授權型訂閱會在訂閱週年日，事先收取整個期間的費用。

**週年日：** 週年日是您購買訂閱的月份日期。 例如，如果您在 1 月 15 日購買訂閱，週年日將是每個月 15 日。

**期間：** 所有授權型訂閱都擁有 12 個月付費期間，從購買日期起算。

**取消：** 在第 1 個月暫停的訂閱將可收到 100% 的退款。 在第 2-12 個月暫停的訂閱則會收到依比例計算的退款。

**續約：** 所有授權型訂閱都在付費期間開始的 12 個月後自動續約。

## <a href="" id="licensebasedmonthly"></a>Monthly billing scenarios

**Scenario 1: New subscription**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00    

2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |循環費用   |4.00       |1        |4.00    

**Scenario 2: Change license quantity**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00    

您在 2 月 1 日將授權數量從一個增加為兩個。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |2/12/2018    |循環執行個體 (依比例計算)   |-4.00       |1        |-4.00    
|1/13/2018         |1/31/2018    | 循環執行個體 (依比例計算)   |2.45       |1        |2.45    
|2/1/2018         |2/12/2018    | 循環執行個體 (依比例計算)   |1.55       |2        |3.10    
|2/13/2018         |3/12/2018    | 循環執行個體 (依比例計算)   |4.00       |2        |8.00    

**Unit Price Formulas:**

The monthly price is 4.00 and there are 31 days in the service period 1/13/2018 - 2/12/2018. 等於每天價格 0.129 (4/31)。

There are 19 days in the proration period 1/13/2018 - 1/31/2018.

按比例計算單價 = 2.451 = 19 x 0.129

There are 12 days in the proration period 2/1/2018 - 2/12/2018.

按比例計算單價 = 1.54 = 12 x 0.129

**Scenario 3: Suspend before 30 days**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取每月計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |2/12/2018    |循環費用   |4.00       |1        |4.00    

On February 1 you suspend a subscription. 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|2/12/2018|取消費用|-4.00|1|-4.00

**Scenario 4: Suspend after 30 days**

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

**Unit Price Formulas:**

The monthly price is 4.00 and there are 28 days in the service period 2/13/2018 - 3/12/2018. 等於每天價格 0.143 (4/28)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

There are 12 days in the cancellation period 3/1/2018 - 3/12/2018. 

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).

## <a name="annual-billing-scenarios"></a>年度計費案例

**Scenario 1: New subscription**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

**Scenario 2: Add license after subscription anniversary date but before billing date**

您在 2017 年 2 月 11 日購買新訂閱，包含一份費率為 $211.20 美元/年的授權。 您的訂閱週年日已設定為每個月的 11 日。 Microsoft 帳單系統會建立下列帳務明細︰ 

-   $211.20 charge for period 2/11/17 - 2/10/18. 

您於 2017 年 2 月 12 日購買第二份授權。 您的帳單日期為 2017 日 2 月 14 日。 產生了發票和對帳檔案。 對帳檔案將會包含下列帳務明細︰ 

|收費開始日期  |收費結束日期  |收費類型  |單價 |數量 | 金額 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |購買時按比例計算費用 |211.20 |1 | 211.20 |

在您的週年日 2017 年 3 月 11 日，Microsoft 帳單系統針對您於 2017 年 2 月 12 日增加的授權建立下列帳務明細： 
-   -$211.20 credit for period 2/11/17 - 2/10/18. 
-   $0.58 prorated charge per license for 1 license for period 2/11/17 - 2/11/17. 
-   $15.62 prorated charge per license for 2 licenses for period 2/12/17 - 3/10/2017. 
-   $195.00 prorated charge per license for 2 licenses for period 3/11/2017 - 2/10/2018. 

您於 2017 年 2 月 11 日購買一份授權。 您於 2017 年 2 月 12 日新增一份授權。 您的帳單日期為 2017 日 2 月 14 日。 您的訂閱於 2018 日 2 月 11 日續約。

您的下一個帳單日期為 2017 年 3 月 14 日，系統產生了發票與對帳檔案。 對帳檔案將會包含下列帳務明細︰ 

|收費開始日期  |收費結束日期  |收費類型  |單價 |數量 | 金額 |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2017/2/11 |2018/2/10 |循環執行個體 (依比例計算) |-211.20 |1 |-211.20 |
|2017/2/11 |2017/2/11 |循環執行個體 (依比例計算) |0.58 |1 |0.58 |
|2017/2/12 |2017/3/10 |循環執行個體 (依比例計算) |15.62 |2 |31.25 |
|2017/3/11 |2018/2/10 |循環執行個體 (依比例計算) |195.00 |2 |390.00 |

訂閱將於 2018 年 2 月 11 日續約 12 個月。


**Scenario 3: Change license quantity**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日將授權數量從一個增加為兩個。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
1/13/2018|1/12/2019|循環執行個體 (依比例計算)|-48.00|1|-48.00
1/13/2018|1/31/2018|循環執行個體 (依比例計算)|2.47|1|2.47
2/1/2018|1/12/2019|循環執行個體 (依比例計算)|44.98|2|89.96

**Unit Price Formulas:**

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

There are 19 days in service period 1/13/2018 - 1/31/2018. 

因此，單價 = 2.47 (19x0.13x1)

There are 346 days in service period 2/1/2018 - 1/12/2019. 

因此，單價 = 44.98 (346x0.13x2)

**Scenario 4: Suspend before 30 days**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日暫停訂閱。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|取消費用|-48.00|1|-48.00

**Scenario 5: Suspend after 30 days**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

2 月 15 日的授權型對帳檔案不會包含此訂閱的任何帳務明細：
您在 3 月 1 日暫停訂閱。 3 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|取消費用|-41.34|1|-41.34

**Unit Price Formulas:**

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

There are 318 days in service period 3/1/2018 - 1/12/2019. 

因此，單價 = 41.34 (318x0.13x1)。 因為這是貸記金額，所以單價是 -41.34。

**Scenario 6: Suspend and reactivate**

您的帳單日期是每個月 15 日。 您在 1 月 13 日購買新訂閱，包含每個月 $4 的授權，並選取年度計費。 1 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|購買時按比例計算之費用|48.00|1|48.00

您在 2 月 1 日暫停訂閱。 2 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|取消費用|-48.00|1|-48.00

您在 3 月 1 日重新啟用訂閱。 3 月 15 日的授權型對帳檔案將包含下列帳務明細：

|收費開始日期 |收費結束日期 |收費類型 |單價 |數量 |金額 |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|購買時按比例計算之費用|41.34|1|41.34

**Unit Price Formulas:**

年度價格是 48.00，相當於每日價格 0.13 (48.00/365)。

單價 = 服務期間天數 x 每天價格 x 授權天數。

There are 318 days in service period 3/1/2018 - 1/12/2019. 

因此，單價 = 41.34 (318x0.13x1)。
