---
title: Microsoft 商業 marketplace 的付款常見問題
description: 取得在商業市場中支出的常見問題解答。 包含您的收益為何與預期不同的答案。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: 44bd7f488e3d4e79c45cb2746c7e2a6da449a310
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175291"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>商業 marketplace 支出的相關常見問題

本文將回答有關在商業市場中支出的常見問題。

## <a name="earnings-incorrect-or-missing"></a>不正確或遺漏的收益

#### <a name="why-are-my-earnings-missing"></a>為何會遺漏收益？

- 客戶訂單可能不符合支付資格。 若為非企業客戶的訂單，Microsoft 必須先收到客戶付款，發行者收益才會符合資格。 若為企業客戶的訂單，您會在訂購單日期之後的 1 到 2 天就獲得收益。 確認[訂單報告](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的訂單狀態。
- 2019 年 7 月之前的交易收益可能不會顯示在交易歷史報告中。 請檢查[支付下載](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)中的歷史對帳單。
- 檢查付款 [週期的時間範圍](payment-thresholds-methods-timeframes.md) ，並瞭解您的收益應該出現在付款聲明中的時間。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>為什麼我的收益金額與我預期的不同？

- 如果訂單部分是由您的客戶支付，則您的收益金額會以扣除費用和適當稅金之後的部分支付金額為基礎。
- 檢查依國家/地區的稅金匯款責任。 若為 Microsoft 負擔稅金的國家/地區，Microsoft 會從發行者的收益中收取和扣除稅金。 此對帳單中顯示的交易金額是在稅額之後。 請參閱[稅務詳細資料](tax-details-marketplace.md)。
- SaaS 和 IaaS 供應專案有10% 的折扣機構費用，而不是標準20%，讓收益率為90%。 此促銷活動將持續到 2021 年 6 月 30 日。

**進一步閱讀**：商業 [marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)、在商業 marketplace 中 [支付款項](marketplace-get-paid.md)、 [稅務詳細資料](tax-details-marketplace.md)、付款 [聲明](payout-statement.md)、 [商業 marketplace 分析中的訂單儀表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>收益對帳
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>如何核對支付明細和分析中的訂單或使用量報表？
使用具有分析訂單和使用方式報表的付款交易歷程記錄報表中，會出現 AssetID、訂單和明細專案識別碼。 使用此對應：

- Payout Transaction History.AssetID = order.OrderID
- Payout Transaction History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>如何知道何時會收到客戶訂單的付款？
- 首先，使用您的 assetID，檢查 [訂單報表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的客戶訂單。
- 在客戶 [報表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)中檢查客戶訂用帳戶的客戶頻道。
- 對於企業客戶而言，發行者收益會出現在訂單1-2 天的訂單日期之後。
- 若為非企業客戶，則在收到客戶付款之後的1-2 天內，發行者收益會顯示在該帳單中。

**進一步閱讀**： [ ](payout-statement.md)[商業市場分析中的付款聲明、訂單儀表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>支付原則

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>如何找出目前的代理商費用和支付費率？

- 請查看商業市集發行者合約。 標準代理商費用為 20%。 SaaS Co-Sell 合格交易的折扣費為10%。 請查看公告內的任何促銷代理商費用。
- 在您的付款帳單中，收益率會指定指定交易的實際付款費率。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>當我的對帳單上出現收益後，我應該會在何時收到 Microsoft 的付款？
- 當您的收益處於未處理狀態時，您可以檢查收益將會進行付款處理的當月到期日。 備妥付款之後，您的收益狀態將會變更為「已處理」。  Microsoft 會在到期當月的 15 日發出付款。
- 若為信用卡支付的訂單，Microsoft 會保留30天的款項，直到賺取額度成熟為止。

 **進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [稅務詳細資料](tax-details-marketplace.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>付款與調整

#### <a name="why-is-my-payment-missing"></a>為何我的付款會遺漏？

- 確定您的支出狀態和稅務設定檔狀態在 [總覽][頁面](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)上顯示為 [*有效*]。
- 您可能未達到付款的最低閾值。 收益必須至少有 50 美元才會收到付款。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>如何? 將我的帳戶設定為不接受付款嗎？
您可以在付款 [設定檔](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)中保存付款;只要勾選 [ **保留**] 即可。 除非您釋出保留期，否則 Microsoft 將會保留您的款項。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>為何收到的貨幣與購買貨幣不同？

支付貨幣是以您在 [支付設定檔] 中選取的貨幣為基礎的。 購買貨幣則是以客戶所支付的貨幣為基礎的。

#### <a name="how-do-i-reconcile-adjustments"></a>如何協調調整？

付款調整是為了配合補償調整 (例如系統問題) 所進行的付款更正。 在支付對帳單中，ReasonCode 會指定調整的原因。 調整並非是要直接協調個別交易。

**進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [稅務詳細資料](tax-details-marketplace.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>稅額

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>我們如何在支付對帳單中識別 Microsoft 或發行者之間的稅務匯款責任？

在 [交易歷史下載] 中，尋找 [稅務模型] 資料行。 這會顯示 [MS 管理的] 或 [ISV 管理的]。 請參閱[稅務詳細資料](tax-details-marketplace.md)中的國家/地區特定稅務規則和支付含意。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何下載服務費用稅務表單？

移至 [支付付款] 頁面，然後移至 [付款清單] 區段。 具有服務費用稅務的付款會出現服務費用稅務表單的連結。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何下載 PDF 格式的預繳稅額表單？

移至 [支付付款] 頁面，然後移至 [付款清單] 區段。 付款旁會出現預繳稅額表單的連結。

#### <a name="where-do-i-find-year-end-tax-forms"></a>哪裡可以找到年終稅務表單？

移至 [[設定檔] 頁面](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)，即可檢視您的年終稅務表單。

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>如何找出交易的預繳稅額？
預繳稅額適用於提出 W-9 表單的美國發行者。 預繳稅額會根據每月的付款來計算。

**進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)

## <a name="payout-statement-access"></a>付款語句存取權

#### <a name="how-do-i-access-a-payout-statement"></a>如何存取支付對帳單？

1. 請檢查您的角色。 您必須擁有*財務參與者*或*帳戶擁有者*角色才能存取支付對帳單。
2. 在右上方導覽中，選取 **付款圖示以** 查看您的付款帳單。 在 **交易歷程記錄**、 **付款**及 **下載**之間進行選擇。

**進一步閱讀**：支付 [角色和許可權](payout-statement.md#roles-and-permissions)、付款 [聲明](payout-statement.md) 

## <a name="payout-statement-report"></a>付款語句報表

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>交易下載中的每個欄位代表什麼？

如需屬性及其意義的詳細清單，請參閱付款 [語句](payout-statement.md) 。

#### <a name="what-is-earning-status"></a>什麼是收益狀態？

這會顯示您的收益是未處理、已處理或已傳送。

- 未**處理–收益**是在到期日之前的經過時間。
- 已**處理**–收益已成熟，並準備入每月付款。 每月15日發行付款。
- **已傳送** –付款已根據您的付款設定檔成功發行至您的銀行。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何下載服務費用稅務表單？

移至 [支付付款] 頁面，然後移至 [付款清單] 區段。 具有服務費用稅務的付款會出現服務費用稅務表單的連結。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何? 下載 PDF 中的預繳稅金表單？

移至 [支付付款] 頁面，然後移至 [付款清單] 區段。 付款旁會出現預繳稅額表單的連結。

#### <a name="where-do-i-find-year-end-tax-forms"></a>哪裡可以找到年終稅務表單？

移至 [[設定檔] 頁面](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage)，即可檢視您的年終稅務表單。

**進一步閱讀**：付款 [語句](payout-statement.md)、 [交易歷程記錄下載](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>歷史對帳單

#### <a name="how-do-i-view-historical-information"></a>如何? 查看歷程記錄資訊？

歷史對帳單會顯示從 2019 年 10 月起的支付資料快照集。 可惜的是，此處的付款資訊不會重新整理。 若要接收最新資訊，請提交最新資料的支援票證。

**進一步閱讀**：付款 [語句](payout-statement.md)、 [交易歷程記錄下載](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>付款匯出 API

#### <a name="how-do-i-download-payout-data"></a>如何下載支付資料？

使用 [合作夥伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)。

## <a name="next-steps"></a>後續步驟

- [在商業市集中獲得報酬](marketplace-get-paid.md)
