---
title: 合作夥伴中心中的商用 marketplace 付款聲明
description: 瞭解付款聲明與摘要，以及如何查看和匯出商業 marketplace 的付款資料
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335676"
---
# <a name="payout-statements"></a>付款語句

付款 **聲明** 提供透過商業市場銷售的優惠支出總覽。 它會顯示您的收益的交易歷程記錄、預估您下一個付款，並顯示付款趨勢。 您也可以下載交易歷程記錄和付款語句。 本文說明如何存取您的付款帳單，以及您在合作夥伴中心中可存取的不同付款頁面和下載。

## <a name="roles-and-permissions"></a>角色和權限

若要存取付款帳單，您必須獲派「 **帳戶擁有** 者」或「 **財務參與者** 」角色。

| 報告/頁面 | 帳戶擁有者 | Manager | 開發人員 | 商務參與者 | 財務參與者 | 行銷人員 |
| --- | --- | --- | --- | --- | --- | --- |
| 擷取報告 (包括近即時資料) | 可檢視 | 可檢視 | 無存取權 | 無存取權 | 可檢視 | 無存取權 |
| 意見反應報告/回應 | 可檢視並傳送意見反應 | 可檢視並傳送意見反應 | 可檢視並傳送意見反應 | 無存取權 | 無存取權 | 可檢視並傳送意見反應 |
| 健康狀態報告 (包括近乎即時的資料) | 可檢視 | 可檢視 | 可檢視 | 可檢視 | 無存取權 | 無存取權 |
| 使用量報告 | 可檢視 | 可檢視 | 可檢視 | 可檢視 | 無存取權 | 無存取權 |
| 支付帳戶 | 可更新 | 無存取權 | 無存取權 | 無存取權 | 可更新 | 無存取權 |
| 稅金設定檔 | 可更新 | 無存取權 | 無存取權 | 無存取權 | 可更新 | 無存取權 |
| 支付摘要 | 可檢視 | 無存取權 | 無存取權 | 無存取權 | 可檢視 | 無存取權 |
|

## <a name="access-your-payout-statement"></a>存取您的支出聲明

登入 [合作夥伴中心](https://partner.microsoft.com/dashboard/home) ，然後選取畫面右上角的付款圖示來存取這些不同的摘要：

- 交易記錄
- 付款
- 匯出資料

:::image type="content" source="images/payouts/payout-overview.png" alt-text="說明合作夥伴中心入口網站右上角的支出圖示":::

您也可以使用 [合作夥伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts) 來連接並直接取得付款交易與付款資料。


## <a name="transaction-history"></a>交易記錄

[ **交易記錄** ] 頁面會顯示您的收益摘要、估計的下一個付款，以及過去36個月的收益和付款趨勢。 您也可以從這個區段下載交易詳細資料。

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="交易總覽。":::

- 今年所**傳送的收益**–已支付的總收益與總收益，並將在未來的月份支付。
- **預估的付款月份** –未來幾個月內預期的總收益。
- **收益與付款趨勢** -過去36個月的每月收益和付款金額。
- **下載** –下載 .csv 或 tsv 格式的交易詳細資料。

使用頁面右上角的日期範圍選取範圍來篩選頁面的輸出，以顯示過去3、6、12或36個月。 或者，選取最多36個月的自訂日期範圍。 預設的日期範圍為12個月。

:::image type="content" source="images/payouts/search-filter.png" alt-text="位於頁面右上方的搜尋篩選準則。":::

### <a name="transaction-history-summary"></a>交易歷程記錄摘要

這會顯示收益詳細資料，包括從產品銷售收入日期、狀態和預估付款月份獲得的收益。

:::image type="content" source="images/payouts/transaction-history.png" alt-text="交易歷程記錄。":::

- **取得日期** –購買日期。
- **收益類型** –賺取的類型，例如銷售、退款或共同作業。
- **總金額** –淨收益金額。 在商業市場中，這表示扣除標準 marketplace 費用之後。
- **狀態** –有三個選項：
    - **即將推出** –收益在擱置的冷卻期間內。
    - 已**處理**–已針對下一個付款準備收益。
    - 已**傳送**–已支付收益。
- **預估的付款月份** –應支付收益的月份。

一旦交易符合付款資格，就會顯示交易。 若要瞭解您可能遺失或未預期的收益，請參閱 [商業 marketplace 支出](payout-faq.md#why-are-my-earnings-missing)的常見問題解答。

### <a name="transaction-history-download"></a>交易歷程記錄下載

若要查看更多關於收益的詳細資料，請選取頁面頂端的 [ **下載** ]。 下表說明報表中的每個資料行。

| 資料行名稱 | 說明 | 獎勵計畫/市場的適用性 |
| --- | --- | --- |
| agreementEndDate | 合約結束日期 | 獎勵 - 僅限部分計劃 |
| agreementNumber | 合約編號 | 獎勵 - 僅限部分計劃 |
| agreementStartDate | 合約開始日期 | 獎勵 - 僅限部分計劃 |
| calculationDate | 在系統中計算收益的日期 | 全部 |
| claimId | 宣告的唯一識別碼 | 獎勵 - 僅限部分計劃 |
| customerCountry | 客戶國家/地區 | marketplaces |
| customerEmail |  |  |
| customerName | 一律為空白 | 獎勵方案只 (例外狀況： OEM) 和市場 |
| customerTenantId |  |  |
| distributorId | 散發者識別碼 | 獎勵 - 僅限部分計劃 |
| distributorName | 散發者名稱 | 獎勵 - 僅限部分計劃 |
| earningAmount | 以原始交易貨幣為單位的收益金額 | 全部 |
| earningAmountInLastPaymentCurrency | 上次付款貨幣的收益金額 (如果之前沒有付款，欄位將會是空白) |  |
| earningAmountUSD | 以美金為單位的收益金額 | 全部 |
| earningDate | 收益的日期 | 全部 |
| earningExchangeRate | 用來顯示對應美金金額的匯率 | 全部 |
| earningId | 每一項收益的唯一識別碼 | 全部 |
| earningRate | 在交易量上套用以產生收益的獎勵率 | 全部 |
| earningType | 指出其是費用、退款、合作，還是銷售等 | 全部 |
| exchangeRateDate | 用來計算 EarningAmount (以美金為單位) 的匯率日期 | 全部 |
| externalReferenceId | 計劃的唯一識別碼 | 直接付費方案 (獎勵和市場)  |
| externalReferenceIdLabel | 唯一識別碼標籤 | 直接付費方案 (獎勵和市場)  |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | 發票號碼 (適用于僅限企業)  | 獎勵和市場-僅限一些方案 |
| lastPaymentCurrency | 上次付款貨幣 (如果之前沒有付款，欄位將會是空白) |  |
| lever | 指出收益的商務規則 | 全部 |
| LicensingProgramName | 授權方案的名稱 |  |
| LineItemId | 客戶發票中的個別明細項目 |  |
| localProviderSeller | 記錄的本地提供者/賣方 |  |
| 成熟度月份 | 預估的付款月份 | 全部 |
| OrderId | 與客戶的發票相關  | marketplaces |
| parentProductId | 唯一的父產品識別碼。 如果該交易沒有父產品，則父產品識別碼 = 產品識別碼。 | marketplaces |
| parentProductName | 父產品的名稱。 如果該交易沒有父產品，則父產品名稱 = 產品名稱。 | marketplaces |
| participantId | 根據該計劃獲取收益的合作夥伴主要身分識別 | 全部 |
| participantIdType | 適用于市場獎勵計畫和賣方的程式識別碼 | 全部 |
| participantName | 收益合作夥伴的名稱 | 全部 |
| partnerCountryCode | 收益合作夥伴的位置/國家/地區 | 全部 |
| partNumber | 一律為空白 | 一些獎勵計畫和市場 |
| paymentId | 付款的唯一識別碼。 這個數字通常會顯示在銀行對帳單中 | 僅限 SAP 付款 |
| paymentStatus | 付款狀態 | 全部 |
| paymentStatusDescription | 付款狀態的易記描述 | 全部 |
| productId | 唯一產品識別碼 | marketplaces |
| productName | 連結至交易的產品名稱 | 全部 |
| productType | 產品的類型 (例如應用程式、附加元件或遊戲) | marketplaces |
| Program Code | 要與方案名稱對應的字串 |  |
| programName | 獎勵/Microsoft Store 計劃名稱 | 全部 |
| purchaseOrderCoverageEndDate | 一律為空白 | 獎勵計劃 - CRI |
| purchaseOrderCoverageStartDate | 一律為空白 | 獎勵計劃 - CRI |
| purchaseOrderType | 一律為空白 | 獎勵計劃 - CRI |
| purchaseTypeCode | 一律為空白 | 獎勵計劃 - CRI |
| quantity | 根據計劃而有所不同。 指出交易計劃的計費數量 | 全部 |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | 轉銷商識別碼 | 獎勵 - 僅限部分計劃 |
| resellerName | 轉銷商名稱 |  |
| SkuId | 發佈期間定義的 SKU 識別碼。 供應項目可有多個 SKU，但一個 SKU 只能與單一供應項目建立關聯。 獎勵 - 僅限部分計劃 |  |
| storeFee | Microsoft 所保留的金額，作為在 Microsoft Store 中提供應用程式或附加元件的費用 | marketplaces |
| subscriptionEndDate | 訂閱結束日期 | 獎勵 - 僅限部分計劃 |
| subscriptionId | 與客戶建立關聯的訂閱識別碼 | 獎勵 - 僅限部分計劃 |
| subscriptionStartDate | 訂閱開始日期 | 獎勵 - 僅限部分計劃 |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | 負責繳交稅金 (營業稅、使用稅或加值稅/貨物及服務稅) 的合作對象 | marketplaces |
| taxRemitted | 已繳交稅金的金額 (營業稅、使用稅或加值稅/貨物及服務稅) | marketplaces |
| taxState | 客戶的州/省 |  |
| taxZipCode | 客戶的郵遞區號 |  |
| tpan | 指出協力廠商廣告網路 | 僅限市場廣告 |
| transactionAmount | 原始交易貨幣 (據以產生收益) 的交易金額 | 全部 |
| transactionAmountUSD | 以美金為單位的交易金額 | 全部 |
| transactionCountryCode | 交易發生的國家/地區代碼 |  |
| transactionCurrency | 進行原始客戶交易時所使用的貨幣 (不是合作夥伴位置的貨幣) | 全部 |
| transactionDate | 交易的日期。 對於將許多交易貢獻給一項收益的計劃相當實用 | 全部 |
| transactionExchangeRate | 用來顯示對應交易美金金額的匯率日期 | 全部 |
| transactionId | 交易的唯一識別碼 | 全部 |
| transactionPaymentMethod | 用於交易的客戶付款方式 (例如卡片、行動裝置電信業者代扣或 PayPal) | marketplaces |
| transactionType | 交易的類型 (例如購買、退貨、沖銷或退款) | marketplaces |
| workload | 工作負載 | 獎勵 - 僅限部分計劃 |
|

## <a name="payments"></a>付款

[ **付款** ] 頁面會詳述您已向 Microsoft 取得的金錢。 它也會顯示您將支付的時間和數量。

>[!Note]
> 若要符合支付資格，收益必須達到美金 $50 元的[付款門檻](payment-thresholds-methods-timeframes.md)。 如需詳細資訊，請參閱 [Microsoft 發行者合約](https://go.microsoft.com/fwlink/?LinkID=699560)。

:::image type="content" source="images/payouts/payments-overview.png" alt-text="付款總覽畫面。":::

- 今年**總支付的總**金額（以美元為單位，以美元為單位），適用于您所有的方案。
- 下一期的**預估款項**–您 (的下一次付款，即使有其他人即將) ，也會以美元為單位。
- **上次付款** –金額 (美元) 、方案名稱，以及最新款項的方案。
- **依來源的付款** -過去12個月內每個方案 (的付款金額（以美元) ）。

### <a name="payments-list"></a>付款清單

付款表的清單會顯示付費和暫止 **的** 付款。 您可以下載 PDF 格式的服務費用稅務資訊，並查看指定付款的收益詳細資料。

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="匯出交易歷程記錄":::

- **付費** -所有付款都已成功傳送。 在下拉式功能表中選擇年份，以篩選出該年度所發行的付款。
- **待決** –即將進行的付款。
- **服務費稅 (PDF 表單) ** –適用于支付服務費用的款項。 服務費用含稅會以 **其他稅金**顯示。
- **View** –將付款中包含的收益清單重新導向至交易歷程記錄。

若要瞭解您可能遺失或未預期的收益，請參閱 [商業 marketplace 支出](payout-faq.md#why-are-my-earnings-missing)的常見問題解答。

### <a name="payment-status"></a>付款狀態

下表說明不同的收益狀態。

| 收益狀態 | 原因 | 需要合作夥伴動作嗎？ |
| --- | --- | --- |
| 尚未處理 | 收益符合付款資格。 它會維持在此狀態中，如獎勵計畫的《節目表》中所定義。 | 否 |
| 即將付款 | 付款訂單會在付款處理之前產生等待內部審核。 | 否 |
| 稅務發票正在暫止 | 您的稅務發票未完成或無效。 | 您需要更新稅務發票才能接收付款 |
| 檢閱期間遭到拒絕 | 評論期間的付款已遭到拒絕。 | 請連絡 Microsoft 支援服務以取得詳細資料 |
| Failed | 付款因 Microsoft 系統錯誤而失敗。 | 如需詳細資訊，請洽詢 Microsoft 支援服務 |
| 正在進行 | 付款正在進行中。 | 否 |
| 付款不正確 | 付款 recouping 正在進行中。 | 否 |
| 已傳送 | 付款已傳送至您的銀行。 | 否 |
| 正在重新處理 | 付款發生 Microsoft 系統錯誤，正在重新處理。 | 否 |
| Reversed | 您的銀行已反轉付款，並將在下一個付款週期再次傳送。 | 否 |
| 稅務發票遭拒 | 稅務發票在檢閱期間遭到拒絕。 所有暫止的付款都將會暫停，直到稅務發票檢閱完成。 | 如需詳細資訊，請洽詢 Microsoft 支援服務 |
| 正在檢閱稅務發票 | 正在檢閱稅務發票。 付款將會在稅務發票獲得核准後發出。 | 否 |
| 已拒絕 | 您的銀行拒絕付款。 | 請連絡銀行以了解詳細資料。 |
|

### <a name="payments-download"></a>付款下載

若要查看您付款的詳細資料，請選取頁面頂端的 [ **下載** ]。 下表說明報表中的每個資料行。

| 資料行名稱 | 描述 |
| --- | --- |
| participantID | 根據該計劃獲取收益的合作夥伴主要身分識別 |
| participantIDType | 適用于商店程式的獎勵計畫和賣方識別碼的程式識別碼 |
| participantName | 收益合作夥伴的名稱 |
| programName | 獎勵/商店計畫名稱 |
| 收益 | 該計劃/participantID 的付款貨幣收益金額 |
| earnedUSD | 方案/participantID 的收益金額，單位為美金 |
| withheldTax | 方案/participantID 的付款貨幣收益金額中扣除的稅務金額 |
| salesTax | 方案/participantID (僅適用于獎勵方案的總銷售稅額（僅適用于獎勵方案）)  |
| serviceFeeTax | 方案/participantID 付款貨幣中的 serviceFeeTax 總金額 (僅適用於 Microsoft Store 計劃和 Azure Marketplace) |
| totalPayment | 方案/participantID 以當地貨幣計算的總付款，排除扣除的稅額並包含營業稅 (若適用的話) |
| currencyCode | 付款貨幣代碼 |
| paymentMethod | 用來向合作夥伴進行支付的方法，例如電子銀行轉帳、折讓單 |
| paymentID | 付款的唯一識別碼。 這個數字通常可在銀行對帳單上看到 (僅適用於 SAP 付款)。 |
| paymentStatus | 付款狀態 |
| paymentStatusDescription | 付款狀態的易記描述 |
| paymentDate | 從 Microsoft 傳送付款時的日期 |
|

## <a name="export-data"></a>匯出資料

[ **匯出資料** ] 頁面不會自行重新整理。 您可能需要手動重新整理頁面，才能看到最新的資料。 從三個索引標籤中選取，以匯出 **交易歷程記錄**、 **付款**、 **交易摘要**或歷程記錄 **語句**。

您的篩選可能會導致 **沒有資料可用** 錯誤。 如果您將預設的時間週期保留在三個月，然後從該期間以外的收益中選取付款識別碼，就會發生這種情況。 如果發生這種情況，請展開您的時間週期，然後再試一次。

以下是範例付款匯出：

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="匯出付款報告。":::

### <a name="historical-statements"></a>歷史對帳單

「 **匯出資料** 」摘要也提供歷程記錄語句的存取權。

> [!NOTE]
> 歷程記錄語句是快照集，且不會重新整理。 如有需要，請聯絡 [支援](https://partner.microsoft.com/support/v2/?stage=1) 人員並要求最新資料。

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="匯出歷程記錄語句。":::

- 從2019年7月1日之前的交易記錄會分開處理，並使用來自稍後歷程記錄報表的不同欄位。
- 舊版交易歷程記錄有一個稱為「保留」的資料行，它會對應到新式歷程記錄中的「收益」資料行，差別在於它會排除狀態等於「付款已傳送」的所有收益。
- 3M、6M 或 12M 等篩選不會套用到歷史對帳單區段。

### <a name="historical-statement-downloads"></a>歷程記錄語句下載

下表說明歷程記錄語句中的每個資料行。

| 欄位名稱 | 描述 |
| --- | --- |
| 收益來源 | 根據交易發生位置 (例如 Microsoft Store 或廣告) 決定的收入來源 |
| 訂單識別碼 | 唯一的訂單識別碼。 此識別碼可供透過購買交易的個別非購買交易 (例如退貨或退款) 來識別購買交易。 這兩者都會具備相同的訂單識別碼。 此外，如果有多個付款條件用於單一購買的分割費用，則可讓您連結購買交易。 |
| Transaction ID | 唯一的交易識別碼。 |
| 交易日期時間 | 發生交易的日期和時間 (UTC)。 |
| 父產品識別碼 | 唯一的父產品識別碼。 如果該交易沒有父產品，則父產品識別碼 = 產品識別碼。 |
| Product ID | 唯一的產品識別碼。 |
| 父產品名稱 | 父產品的名稱。 如果該交易沒有父產品，則父產品名稱 = 產品名稱。 |
| 產品名稱 | 產品的名稱 |
| 產品類型 | 產品的類型 (例如應用程式、附加元件或遊戲) |
| 數量 | 當收入來源是商務用 Microsoft Store 時，Quantity 代表購買的授權數。 針對其他所有的收入來源，Quantity 一律為 1。 即使單一交易因為使用了兩種不同付款方式而分成兩個明細項目，每個明細項目仍會顯示 Quantity 為 1。 |
| 交易類型 | 交易的類型 (例如購買、退貨、沖銷或退款) |
| 付款方式 | 用於交易的客戶付款方式 (例如卡片、行動裝置電信業者代扣或 PayPal) |
| 國家/地區 | 發生交易的國家/地區 |
| 本地提供者/賣方 | 記錄的本地提供者/賣方 |
| 交易貨幣 | 交易的貨幣 |
| 交易金額 | 交易的金額 |
| 已繳交稅金 | 已繳交稅金的金額 (營業稅、使用稅或加值稅/貨物及服務稅) |
| 淨收入 | 扣除已繳交稅金的交易金額 |
| Microsoft Store 費用 | Microsoft 所保留的淨收入百分比，作為在 Microsoft Store 中提供應用程式或附加元件的費用 |
| 應用程式收入 | 扣除 Microsoft Store 費用後的淨收入 |
| 已預繳稅金 | 預繳的所得稅金額 (不包含在**已保留** CSV 檔案中) |
| 付款 | 扣除任何適用已預繳所得稅之後的應用程式收入 (以交易貨幣顯示) 不包含在**已保留** CSV 檔案中。 |
| FX 率 | 用來將交易貨幣轉換成付款貨幣的外幣匯率 |
| 付款貨幣 | 用來進行付款的貨幣 |
| 已轉換付款 | 使用 FX 率轉換成付款貨幣的付款金額 |
| 稅務匯款模型 | 負責繳交稅金 (營業稅、使用稅或加值稅/貨物及服務稅) 的合作對象 |
| 資格日期時間 | 交易收入符合支出資格的日期和時間 (UTC)。 建立支出時，其會包含資格日期時間在支出建立日期之前的交易收入 (僅包含在**已保留** CSV 檔案 中)。 |
| Charges | 顯示彙總在交易金額資料行中所有費用詳細資料的明細 (僅會針對 Azure Marketplace 包含，不會包含在**已保留** CSV 檔案中)。 |
|||

## <a name="next-steps"></a>後續步驟

- [合作夥伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支出原則詳細資料](payout-policy-details.md)
- 如需帳務支援，請連絡商業市集[發佈者支援](https://partner.microsoft.com/support/v2/?stage=1)。