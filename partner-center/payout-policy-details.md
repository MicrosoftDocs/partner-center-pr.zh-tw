---
title: 支出排程和原則詳細資料-Azure marketplace
description: 深入瞭解與商業 marketplace 付款原則相關的詳細資料，包括排程和 recoupment。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 11/06/2020
ms.openlocfilehash: cbd849001d128db1912a9bb61ef4c5217a5932ce
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947659"
---
# <a name="payout-schedules-and-policy-details"></a>支出排程和原則詳細資料

本文討論 Microsoft 的付款流程、付款排程、要在哪裡尋找付款狀態，以及客戶未付款的流程。

## <a name="payment-schedules"></a>付款排程

下列各節說明 **Enterprise 合約** 和 **信用卡/發票** 交易的支出流程。

### <a name="enterprise-agreement-transactions"></a>Enterprise 合約交易

當客戶從 Microsoft AppSource 購買產品，Azure Marketplace 或使用其現有的 Microsoft Enterprise 合約進行交易時，我們會在下一期的客戶發票30天內發出支出。 客戶使用信用卡的交易在付款前有30天的保留期。

付款通常會在 Microsoft 向客戶收取款項之前發生。 如果客戶無法支付 Microsoft 的費用，但我們已發出款項，請參閱以下 [客戶的非付款流程](#process-for-customer-non-payment) 。

| 事件 | 描述 | 報表可見度 | 計時 |
| --- | --- | --- | --- |
| 交易的使用量或月份 | 客戶使用或購買服務。 | [使用量](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [訂單](/azure/marketplace/partner-center-portal/orders-dashboard) 儀表板 | **第1個月** |
| 採購單已建立 | 判斷總使用量和交易總計 | [使用量](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [訂單](/azure/marketplace/partner-center-portal/orders-dashboard) 儀表板 | **第2個月** |
| 已建立 ISV 付款收益 | 判斷機關費和支出收益 | 在付款[語句](payout-statement.md)的交易歷程記錄中標示為未處理 | **第3個月 (第一周)** |
| 準備付款 | 每月付款已備妥收益 | 在付款[聲明](payout-statement.md)的交易歷程記錄中標示為即將推出 | **第3個月 (第一周)** |
| **付款日期** | **付款會傳送給發行者** | **標示為在交易歷程記錄和付款 [聲明](payout-statement.md)的付款區段中傳送** | **第3個月 (不晚于 15)** |
| 客戶付款的發票 | Microsoft 會從客戶收集款項 | 沒有變更 | **第4到12個月** |
|

\* 付款日期是太平洋標準時間 (PST) 。

### <a name="customers-who-pay-using-credit-card-or-invoice"></a>使用信用卡或發票付款的客戶

所有使用信用卡或每月發票的購買都有30天的保留期，以確保從客戶收集資金。

| 事件 | 描述 | 報表可見度 | 計時 |
| --- | --- | --- | --- |
| 交易的使用量或月份 | 客戶使用或購買服務。 | [使用量](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [訂單](/azure/marketplace/partner-center-portal/orders-dashboard) 儀表板 | **第1個月** |
| 客戶付款的發票 | 決定總使用量、總交易值和客戶支付發票 | [使用量](/azure/marketplace/partner-center-portal/usage-dashboard) 或 [訂單](/azure/marketplace/partner-center-portal/orders-dashboard) 儀表板 | **第2個月** |
| 已建立 ISV 付款收益 | 判斷機關費和支出收益 | 在付款[語句](payout-statement.md)的交易歷程記錄中標示為未處理 | **第2個月** |
| 30天的保留期 | 確定資金的集合、可能的退款和退款要求 | 在付款[語句](payout-statement.md)的交易歷程記錄中標示為未處理 | **第3個月** |
| 準備付款 | 每月付款已備妥收益 | 在付款[聲明](payout-statement.md)的交易歷程記錄中標示為即將推出 | **第4個月 (第一周)** |
| **付款日期** | **付款會傳送給發行者** | **標示為在交易歷程記錄和付款 [聲明](payout-statement.md)的付款區段中傳送** | **第4個月 (不晚于 15)** |
|

\* 付款日期是太平洋標準時間 (PST) 。

## <a name="process-for-customer-non-payment"></a>客戶未付款的流程

在罕見的情況下，Microsoft 無法向客戶收取其商業 marketplace 購買的款項。 當客戶無法根據其計費排程支付 Microsoft 的費用時，就會開始進行收集程式。 此程式需要大約四個月的時間，並牽涉到從 Microsoft 持續進行通訊。 如果未在此程式結束時收到付款，Microsoft 會將資金寫成 uncollectable。

根據此處所示的付款流程，Microsoft 可能已將資金支付給發行者， (您) 最終 uncollectable。 因此，我們有協調這些金額的流程。 為確保您的 (已收到) 付款的相關警告，當客戶在收款流程中時，您將會收到通知，而且可能會將購買專案寫出。

Microsoft 會使用下列其中一種方法 recoup 任何已支付給您的支出： (1) Microsoft 可以從未來的支出減去未付款的金額;例如，如果支出中的 $1000 被視為 uncollectable 並寫出，您的未來支出將會在 $1000 復原之前被取消，或 (2) Microsoft 可能會要求退款或發票發行者提供任何未回收金額。

以下是範例排程：

| 事件 | 大約日期 * | 合作夥伴可見度 |
| --- | --- | --- |
| 付款日期範例 | 10/15/2020 | 在付款儀表板中標示為在交易歷程記錄和付款區段中 **傳送** |
| <font color="red">如果客戶未支付 Microsoft 費用</font> | 12/2/2020 –12/5/2020 | 沒有變更，與上述相同 |
| 客戶第一次收到付款電子郵件 | 12/6/2020 | None |
| 客戶會收到不斷增加緊急的一般電子郵件 | 12/7/2020 –1/31/2021 | None |
| 發行者可能會通知寫出 | 1/7/2021 | 傳送給發行者的電子郵件通知，其客戶尚未傳送款項。 包含交易識別碼和金額。 |
| 客戶接收終止通知 | 2/1/2021 | None |
| 集合處理常式結束/資金已寫出 | 2/15/2021 | 傳送給發行者的電子郵件通知，已將資金寫掉。 包含交易識別碼和金額。 |
| 扣除支出 | 3/1/2021 | 發行者會在合作夥伴中心付款聲明中看到負面交易 |
| 支付支出 | 3/15/2021 | 未來的支出會顯示在合作夥伴中心的付款聲明中。 在餘額不再為負數之前，發行者將不會收到付款。  |
|||

\* 付款日期是太平洋標準時間 (PST) 。

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>要達到付款帳戶的付款天數

我們通常會在該月第15天的指定月份傳送任何款項，但需要額外的時間才能支付您的帳戶。 天數取決於我們用於帳戶的付款方法，如下所述。

> [!NOTE]
> 如下所示的天數是近似值;任何付款都可能需要較長或較短的時間才能到達您的帳戶。

| 付款方法     | 進入支付帳戶所需的天數     |
|--------------------|--------------------------------------------|
| PayPal             | 1 個工作天                             |
| ACH/SEPA           | 2-3 個工作天                          |
| 電匯      | 7-10 個工作天                         |
|

## <a name="next-steps"></a>後續步驟

- [稅賦詳細資訊](tax-details-marketplace.md)
