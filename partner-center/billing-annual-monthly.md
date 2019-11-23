---
title: Monthly and annual billing differences | Partner Center
ms.topic: article
ms.date: 11/21/2019
Description: Differences between monthly and annual billing cycles in Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 4d6b316f55a6d2cd84959d60feed666d657893b8
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389766"
---
# <a name="monthly-and-annual-billing-differences"></a>Monthly and annual billing differences

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

This topic explains the differences between **monthly billing** and **annual billing** in Partner Center, including benefits and use cases. You have the option to pay for certain Cloud Solution Provider (CSP) subscriptions on a monthly or annual basis.

## <a name="applicability"></a>適用性

Most licensed-based subscriptions have the option for either monthly or annual billing option. 用量型訂閱只有每月計費選項。

Both annual and monthly billing are **per subscription**, ***not* per license**.

### <a name="find-subscription-applicability"></a>Find subscription applicability

You can identify the available billing frequencies for each offer by using column J in the offer matrix. You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="applicable-partners"></a>Applicable partners

All partners and partner types can choose monthly or annual billing.

### <a name="applicable-markets"></a>Applicable markets

Monthly and annual billing (for applicable offers) are available in all markets where the CSP program is currently available.

## <a name="change-billing-frequency"></a>Change billing frequency

You can switch between monthly and annual billing at any time. You may want to change your billing frequency if your business needs change.

When you change the billing frequency to annual, the annual term is updated to reflect the date you changed the billing frequency. A new renewal date is also established.

### <a name="monthly-to-annual-billing"></a>Monthly to annual billing

Switching from monthly billing to annual billing may be useful if you have numerous subscriptions that are billed monthly. When you switch to annual billing, you can align the subscriptions to a common billing date.

### <a name="annual-to-monthly-billing"></a>Annual to monthly billing

Switching from annual billing to monthly billing may be useful if you want to adjust your billing dates to those of your individual customers.

## <a name="annual-billing"></a>Annual billing

年度計費具有下列優點：

- 提高付款選項的彈性。
- 更能夠校準向客戶開立發票的方式。
- 減少貨幣變動帶來的影響。
- 降低帳單營運成本。

### <a name="configure-annual-billing"></a>Configure annual billing

If you're planning to switch to annual billing in Partner Center, be sure to consider how your sales motion will be affected. You should inform your team and update your internal processes as necessary. You should also review changes to your invoice and license-based reconciliation file. 

You will also need to [update your APIs for annual billing](#required-api-changes).

#### <a name="required-api-changes"></a>Required API changes

為了運用年度計費，API 必須進行一些變更。

- [Order.BillingCycle property](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Create an order](https://docs.microsoft.com/partner-center/develop/create-an-order)

For more information about Partner Center APIs, see all [Partner Center developer resources and documentation](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Placing orders

The billing frequency type, including the annual billing option, is assigned to the **Offer** as an attribute. There is not a unique offer specifically for orders with annual billing. 不過，您可使用客戶更容易記得的名稱將方案重新命名，作為區別之用。

### <a name="select-annual-billing"></a>Select annual billing

When you add a new subscription, you will be prompted to choose the billing frequency. 您可以在此時選擇年度計費選項。 When you select annual billing,all available offers will be displayed.

### <a name="billing-time"></a>Billing time

您會在下一個帳單日期收到帳單。 For example, if your billing date is the 1st of the month and you purchase an annually billed subscription on October 29, 2019, you will be billed on November 1, 2019. Assuming that you make no license changes, you will be billed again on November 1, 2020. If you make a license change you will receive a credit and rebill on your next billing date.

### <a name="annual-renewals"></a>Annual renewals

Your subscription renewal date will be twelve months after the service start date. 服務期間從建立訂閱的日期起算。  For example, a subscription created on January 10, 2019, will be renewed on January 10, 2020.

您會在訂閱續約日期之後的下一個帳單日期收到帳單。 例如，如果您在 2018 年 1 月 15 日購買年度計費訂閱，而您的帳單日期是 1 月 20 日，則您的訂閱將在 2019 年 1 月 15 日續約。 接著您會在 2019 年 1 月 20 日收到續約的帳單。

### <a name="split-subscription-billing-frequency"></a>Split subscription billing frequency

It isn't possible to split a **single subscription** so that one part is billed monthly and the other part is billed annually. The entire subscription must have the same billing frequency (either monthly or annual billing).

For customers with **multiple subscriptions** of the same offer, it may be possible to have different billing frequencies per subscription. 某些供應項目會限制每一個客戶只能同時擁有一個訂閱。 若供應項目並沒有進行限制，則客戶就可以以不同的帳單週期，針對同一項供應項目購買多個訂閱。 您可以在方案組合的 I 欄中找到所有供應項目的限制。 You can find the offer matrix in the **See offers and pricing** section on Partner Center.

### <a name="free-subscription-period"></a>Free subscription period

Subscriptions with annual billing frequency do not receive a free period. The twelve-month paid term begins on the purchase date. 這和採用每月帳單週期的訂閱不同，每月週期在購買日期到下一個帳單日期之間有免費期間。

### <a name="adding-and-removing-licenses"></a>Adding and removing licenses

您隨時可以變更訂閱的授權數量。 新增額外的授權並不會影響帳單週期。

您可以隨時新增或移除授權。  You will receive a credit and prorated rebill on your next billing date after you change the number of licenses.

If your existing subscription has annual billing, it's not possible to add licenses with monthly billing to that subscription. 您使用年度計費購買訂閱後，任何新增的基座都將遵循相同的帳單週期。 如果您隨後需要購買每月訂閱的授權，您將需要購買新的訂閱。

### <a name="add-on-offers"></a>Add-on offers

附加元件訂閱會自動採用父供應項目訂閱所採用的帳單週期。 Annual billing is available for add-on offers. 

### <a name="cancelling-subscriptions"></a>Cancelling subscriptions

所有帳單週期的取消原則都相同。

For annual billing, if the subscription is cancelled in the first 30 days of the twelve-month paid term you will receive a 100 percent credit on your next billing date. If the subscription is cancelled after 30 days of the twelve-month paid term you will receive a prorated credit on your next billing date.

### <a name="moving-subscriptions-between-partners"></a>Moving subscriptions between partners

Customers can't move subscriptions between from one partner to another. 這項規定同時適用於每月與年度計費的訂閱。

新的合作夥伴必須代表客戶購買新的訂閱 It's not possible to move subscriptions between partners.

### <a name="reactivating-subscriptions"></a>Reactivating subscriptions

You can reactivate a subscription for up to 90 days after the suspension date. 您會在接下來的帳單日期收到依比例計算的費用。 訂閱續約日期保持不變。

## <a name="pricing"></a>定價

### <a name="offer-pricing"></a>Offer pricing

The offer price at time of purchase is guaranteed for the full billed subscription term (one month for monthly billing, twelve months for annual billing). 訂閱續約時，會根據續約當日的價目表重設價格。 The new price is guaranteed for the next subscription term.

If an offer price decreases during the billing period, the amount you are billed for doesn't change. The price is set for the full billing period at the time of purchase. This applies to both monthly and annual billing.

### <a name="cancellation-credits"></a>Cancellation credits

Credit for a cancelled license or subscription is calculated as follows:

**Cancellation credit** = ((**monthly price***12)/365) \* **days remaining in the twelve-month term** \* number of licenses cancelled.

## <a name="reconciliation-file"></a>Reconciliation file

### <a name="find-subscriptions-billing-frequency"></a>Find subscription's billing frequency

Review your license-based reconciliation file for information on whether your subscription is billed monthly or annually. This information is in column **AA**.

To find out whether you can change a monthly subscription to annual billing, see [Find subscription applicability](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Reconciliation file changes for annual billing

When you purchase or renew a subscription with annual billing, your license-based reconciliation file will change as follows.

A new row on the license-based reconciliation file on the first billing date following the purchase or a new subscription.

若訂閱沒有發生任何變更，則對帳檔案上訂閱期限的第二個月到第十二個月上不會有任何列。 If a change is made to the subscription during the twelve-month term, a credit and prorated rebill will appear on the next reconciliation file after the change is made.

The next change to the reconciliation file will appear when the subscription is renewed. 這將會出現在續約之後的第一個帳單日期。

### <a name="usage-file-changes-for-annual-billing"></a>Usage file changes for annual billing

The following annually billed subscription changes appear in column P of your usage file.

- **Prorate Fees When Purchase**: the initial purchase of an annual subscription.
- **Cycle Instance Prorate**: license changes that result in credit and rebilling.
- **Cancel Fee**: the [cancellation of an annual subscription](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancellation of annual subscription

When an annually billed subscription is cancelled, the reconciliation file will contain one line item for a cancellation credit.

If the cancellation occurs in the first 30 days of the twelve-month term, the subscription will be credited at 100 percent. 若在 30 天之後才進行取消，收到的訂閱退款將會依比例計算。

### <a name="adding-licenses-to-annual-subscription"></a>Adding licenses to annual subscription

When you add licenses to a subscription, the reconciliation file will contain a credit and prorated rebill. This applies to monthly and annually billed subscriptions.

### <a name="price-lists-for-annual-billing"></a>Price lists for annual billing

Partner Center price lists show the monthly prices. There is no annual price listed. 將每月價格乘以 12，即可計算得到年度價格。

### <a name="offer-matrix"></a>Offer matrix

Offer IDs in the offer matrix are the same for all billing frequencies. There are no unique IDs for offers that can be billed annually.

## <a name="incentives"></a>獎勵

### <a name="incentives-calculation"></a>Incentives calculation

Incentives are calculated based on **billed revenue**, ***not* adjusted revenue**. 實獲的獎勵付款會根據我們在雲端解決方案提供者獎勵指南中的原則提供。

When an annually billed subscription is sold, that subscription's revenue is recognized for the calculation of incentives based on billed revenue.

### <a name="payout"></a>支付

Currently, all incentive payments are made twice a year. 這些付款將在半年度結束之後的 45 天支付。

### <a name="rates"></a>費率

Partners earn incentives on all eligible transactions, regardless of how a subscription is billed. Incentive earnings are calculated based on the global incentive rate (which is applied to the billed revenue for the period), the local accelerator (for all geographies in which there are local accelerators), and any global campaigns (where applicable).

### <a name="contacts"></a>連絡人

For questions about incentives, contact the appropriate regional incentives support team:

| 地區 | Email address |
| ------ | ------------- |
| 北美洲 | <ocina@microsoft.com> |
|Latin America & Brazil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excluding Japan) | <ociapgc@microsoft.com> |
| 日本 | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspension

If you suspend an subscription (in Partner Center or through the APIs) within 30 days of purchase, you will receive a 100% credit, regardless of billing frequency.

For annual billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to December 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to December 31st.
3. The reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to December 31st.

For monthly billing:

1. The partner buys the subscription on January 1st. A charge billing line is created for the service period January 1st to January 31st.
2. The partner suspends the subscription on January 25th. A credit billing line is created for the service period January 1st to January 31st.
3. The partner reactivates the subscription on January 29th. A charge billing line is created for the service period January 29th to January 31st.
