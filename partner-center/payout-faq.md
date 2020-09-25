---
title: Microsoft 商業 marketplace 的付款常見問題
description: 取得在商業市場中支出的常見問題解答。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/11/2020
ms.openlocfilehash: eea01f5c3c7f6e249a00e8b95df93274b87fb43d
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335666"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>商業 marketplace 支出的相關常見問題

本文將回答有關在商業市場中支出的常見問題。

## <a name="earnings-incorrect-or-missing"></a>不正確或遺漏的收益

#### <a name="why-are-my-earnings-missing"></a>為什麼我的收益遺失？

- 客戶訂單可能還不符合付款資格。 若為非企業客戶訂單，Microsoft 必須先獲得客戶款項，才能讓發行者賺取成為合格。 若為企業客戶訂單，您的收益將在訂單日期後的1-2 天內提供。 確認 [訂單報表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的訂單狀態。
- 交易歷程記錄報告中不會顯示交易在2019年7月之前的收益。 檢查付款 [下載](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport)中的歷程記錄。
- 檢查付款 [週期的時間範圍](payment-thresholds-methods-timeframes.md) ，並瞭解您的收益應該出現在付款聲明中的時間。

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>為什麼我的收益金額與我預期的不同？

- 如果訂單部分是由您的客戶支付，則您的收益金額會以扣除費用和適當稅金之後的部分支付金額為基礎。
- 檢查依國家/地區的稅金匯款責任。 如果是 Microsoft 負責任的國家/地區，Microsoft 會從發行者的收益中收集並自動稅。 語句中顯示的交易數量是在稅額之後。 請參閱 [稅務詳細資料](tax-details-marketplace.md)。
- SaaS 和 IaaS 供應專案有10% 的折扣機構費用，而不是標準20%，讓收益率為90%。 這項促銷活動將在2021年6月30日前生效。

**進一步閱讀**：商業 [marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)、在商業 marketplace 中 [支付款項](marketplace-get-paid.md)、 [稅務詳細資料](tax-details-marketplace.md)、付款 [聲明](payout-statement.md)、 [商業 marketplace 分析中的訂單儀表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="earnings-reconciliation"></a>收益對帳
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>如何? 在分析中將付款聲明與訂單或使用量報告進行協調？
使用具有分析訂單和使用方式報表的付款交易歷程記錄報表中，會出現 AssetID、訂單和明細專案識別碼。 使用此對應：

- 付款交易歷程記錄。 AssetID = order。分組
- 付款交易歷程記錄。訂單 Id & LineItem = UsageReferenceID [訂單 Id： LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>如何? 知道何時應支付客戶訂單的款項？
- 首先，使用您的 assetID，檢查 [訂單報表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order)中的客戶訂單。
- 在客戶 [報表](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer)中檢查客戶訂用帳戶的客戶頻道。
- 對於企業客戶而言，發行者收益會出現在訂單1-2 天的訂單日期之後。
- 若為非企業客戶，則在收到客戶付款之後的1-2 天內，發行者收益會顯示在該帳單中。

**進一步閱讀**： [ ](payout-statement.md)[商業市場分析中的付款聲明、訂單儀表板](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>支出原則

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>如何? 找出目前的機構費和支出費率？

- 請檢查商業 marketplace 發行者合約。 標準機構費用為20%。 SaaS 共同銷售合格交易有10% 的折扣費用。 檢查是否有任何促銷機構費用的公告。
- 在您的付款帳單中，收益率會指定指定交易的實際付款費率。

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>當我的帳單上出現收益之後，何時可以預期 Microsoft 的付款？
- 當您的收益處于未處理的狀態之後，您就可以檢查到期日，以瞭解您的收益將會處理付款的月份。 備妥付款之後，您的收益狀態將會變更為「已處理」。  Microsoft 會在成熟度月15日發行款項。
- 若為信用卡支付的訂單，Microsoft 會保留30天的款項，直到賺取額度成熟為止。

 **進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [稅務詳細資料](tax-details-marketplace.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)

## <a name="payments-and-adjustments"></a>付款與調整

#### <a name="why-is-my-payment-missing"></a>為什麼我的付款遺失？

- 確定您的支出狀態和稅務設定檔狀態在 [總覽][頁面](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)上顯示為 [*有效*]。
- 您可能不符合付款的最小臨界值。 收益必須至少為 $50 美元才能獲得付款。


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>如何? 將我的帳戶設定為不接受付款嗎？
您可以在付款 [設定檔](https://partner.microsoft.com/dashboard/commercial-marketplace/overview)中保存付款;只要勾選 [ **保留**] 即可。 除非您釋出保留期，否則 Microsoft 將會保留您的款項。

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>為什麼我收到的貨幣與購買貨幣不同？

付款貨幣是以您在 [付款設定檔] 中選取的貨幣為基礎。 購買貨幣是以客戶支付的貨幣為基礎。

#### <a name="how-do-i-reconcile-adjustments"></a>如何? 協調調整？

付款調整是付款更正，以配合補償的調整，例如系統問題。 在付款語句中，ReasonCode 會指定調整的原因。 這些都不是要直接協調到個別交易。

**進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)、 [稅務詳細資料](tax-details-marketplace.md)、 [付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)

## <a name="taxes"></a>稅額

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>我們該如何在付款聲明中找出 Microsoft 或發行者之間的稅金匯款責任？

在 [交易記錄] 下載中，尋找 [稅務模型] 資料行。 這會顯示 MS 管理或 ISV 管理。 請參閱 [稅務詳細資料](tax-details-marketplace.md)中的國家（地區）專屬稅務規則和支出含意。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何? 下載服務費用稅務表單？

移至 [付款 **付款** ] 頁面，然後移至 [付款] 區段 **清單** 。 服務費稅表單的連結會顯示為具有服務費用稅的付款。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何? 下載 PDF 中的預繳稅金表單？

移至 [付款 *付款* ] 頁面，然後移至 [付款] 區段 **清單** 。 付款旁邊會出現預繳稅金表單的連結。

#### <a name="where-do-i-find-year-end-tax-forms"></a>我可以在哪裡找到年份端稅務表單？

移至 [ [設定檔] 頁面](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) ，以查看您的年度最終稅務表單。

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>如何? 尋找交易的預繳稅金？
預繳稅金適用于記載了 W-9 表單的美國發行者。 預繳稅金是以每月付款計算。

**進一步閱讀**： [商業 Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)、付款 [原則詳細資料](payout-policy-details.md)

## <a name="payout-statement-access"></a>付款語句存取權

#### <a name="how-do-i-access-a-payout-statement"></a>如何? 存取付款帳單？

1. 檢查您的角色。 您必須擁有「 *財務參與者* 」或「 *帳戶擁有* 者」角色，才能存取付款聲明。
2. 在右上方導覽中，選取 **付款圖示以** 查看您的付款帳單。 在 **交易歷程記錄**、 **付款**及 **下載**之間進行選擇。

**進一步閱讀**：支付 [角色和許可權](payout-statement.md#roles-and-permissions)、付款 [聲明](payout-statement.md) 

## <a name="payout-statement-report"></a>付款語句報表

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>交易下載中的每個欄位代表什麼意思？

如需屬性及其意義的詳細清單，請參閱付款 [語句](payout-statement.md) 。

#### <a name="what-is-earning-status"></a>什麼是收益狀態？

這會顯示您的收益是未處理、已處理或已傳送。

- 未**處理–收益**是在到期日之前的經過時間。
- 已**處理**–收益已成熟，並準備入每月付款。 每月15日發行付款。
- **已傳送** –付款已根據您的付款設定檔成功發行至您的銀行。

#### <a name="how-do-i-download-service-fee-tax-forms"></a>如何? 下載服務費用稅務表單？

移至 [付款 **付款** ] 頁面，然後移至 [付款] 區段 **清單** 。 服務費稅表單的連結會顯示為具有服務費用稅的付款。

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>如何? 下載 PDF 中的預繳稅金表單？

移至 [付款 **付款** ] 頁面，然後移至 [付款] 區段 **清單** 。 付款旁邊會出現預繳稅金表單的連結。

#### <a name="where-do-i-find-year-end-tax-forms"></a>我可以在哪裡找到年份端稅務表單？

移至 [ [設定檔] 頁面](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) ，以查看您的年度最終稅務表單。

**進一步閱讀**：付款 [語句](payout-statement.md)、 [交易歷程記錄下載](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>歷史對帳單

#### <a name="how-do-i-view-historical-information"></a>如何? 查看歷程記錄資訊？

歷程記錄語句會顯示從2019年10月起的付款資料快照集。 可惜的是，此處的付款資訊不會重新整理。 若要接收最新資訊，請提交最新資料的支援票證。

**進一步閱讀**：付款 [語句](payout-statement.md)、 [交易歷程記錄下載](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>付款匯出 API

#### <a name="how-do-i-download-payout-data"></a>如何? 下載付款資料？

使用 [合作夥伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)。

## <a name="next-steps"></a>後續步驟

- [在商業市集中獲得報酬](marketplace-get-paid.md)
