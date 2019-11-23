---
title: 為客戶提供 Microsoft 產品試用 | 合作夥伴中心
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 您的客戶可以試用 Microsoft 訂閱產品 30 天。 You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384835"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>為客戶提供 Microsoft 產品試用

適用於：

- 合作夥伴中心

提供 30 天免費試用，讓客戶接觸全新 Microsoft 產品是個不錯的方式。 就像在許多其他線上服務一樣，您可以註冊類別目錄中的試用版。 所有合作夥伴可以都參與。

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. 例如：針對 Office 365 商務進階版取得一個免費試用版本，以及針對 Office 365 E3 取得另一個免費試用版本。 However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

下列產品提供免費試用版本：

- Office 365 商務進階版
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 for Financials
- Microsoft 365 商務版

我們提供這些產品的免費試用，是因為它們是最全方位也最熱門的商務用供應項目。 未來可能會增加其他免費試用供應項目。

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. 在類別目錄的 **\[帳單週期\]** 中，按一下 **\[試用優惠\]** 。 這樣就只允許免費試用出現，並停用其他非免費的優惠。 試用項目將會顯示在類別目錄的 **\[試用\]** 索引標籤中。
3. 選取您想要提供的免費試用，然後選取 **\[提交\]** 。 所有試用都是 30 天，此期間不會向您收費。 您也可以隨時在試用期間將其轉換為付費訂閱。

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. 移至客戶訂閱頁面，並選取免費試用。
2. 選取 **\[將試用版轉換成付費訂閱\]** 。
3. 輸入您想要的授權數量與帳單週期，然後選取 **\[套用\]** 。
4. 付費訂閱會從轉換日期開始計費，並將在轉換日期起算 12 個月後自動續約訂閱。 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [將試用版訂閱轉換成付費](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [取得試用版轉換方案的清單](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. 我們建議您頻繁監視這些日期，以便可以針對接近決策點的客戶採取適當的行動。

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>帳單

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. 如果將免費試用轉換為年度計費的付費方案，訂閱續約日期將是轉換日期起算的 12 個月後。 如果將免費試用轉換為每月計費的付費方案，訂閱續約日期將是轉換日期之後帳單日期起算的 12 個月後。

### <a name="invoices"></a>發票

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>獎勵

Free trials do not have an impact on incentives.

## <a name="support"></a>支援

For support on free trials, submit a service request through Partner Center.
