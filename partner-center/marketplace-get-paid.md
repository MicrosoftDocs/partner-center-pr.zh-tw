---
title: 合作夥伴中心中取得付費
description: 瞭解如何以 Microsoft 合作夥伴的形式接收收益款項，例如透過商業 marketplace 供應專案、獎勵計畫和雲端解決方案提供者計畫。 包含付款原則、付款保留狀態和付款聲明。
ms.service: marketplace
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: fc1eea0d8a90bb2b5e11dad24a71c9c34fd1a4a0
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492444"
---
# <a name="getting-paid-in-partner-center"></a>合作夥伴中心中取得付費

**適當的角色：**

- 帳戶管理員
- 全域系統管理員

本文提供有關接收您的供應專案、附加元件和廣告收入款項的重要資訊。 其中摘要說明支出原則、取得付費前所需的步驟，以及付款聲明的總覽。

## <a name="payout-policies-and-agreements"></a>支付原則和協定

取得付費需要您遵守合約和付款原則。

- [Microsoft Azure Marketplace 發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)：取得付費之前，您必須接受此發行者合約。 本合約說明您與 Microsoft 之間的關聯性，因為它與商業 marketplace 中的賣方供應專案有關，包括 Microsoft 針對每次銷售所收取的商店費用。
- 付款[原則](payout-policy-details.md)會顯示付款的付款原則，包括付款排程和付款方法。 原則也會說明客戶未付款的流程。
- [稅務詳細資料](tax-details-marketplace.md) 說明在 Microsoft [發行者合約](https://go.microsoft.com/fwlink/p/?LinkID=699560)下，價格選擇和稅務責任的稅務考慮。
- **商店費用** 已正式定義于發行者合約中。 商店費用適用于商業 marketplace 所收集的所有供應專案銷售，包括附加元件。
- 每個月會進行 **付款**， (提供已) 的付款閾值。 我們通常會在該月第15天的指定月份傳送任何款項。 付款通常需要3至10個額外的工作天，才能達到您的付款帳戶。 如需詳細資訊，請參閱[付款閾值、方法和時間範圍](payment-thresholds-methods-timeframes.md)。

## <a name="prerequisite-steps-before-getting-paid"></a>取得付費之前的先決條件步驟

第一次開始付費之前，您必須先設定您的付款帳戶，並完成必要的銀行和稅務表單。 在銀行和稅務表單中，您將提供慣用的付款方法和預繳稅金的稅務形式。 需要銀行和稅務表單才能支付費用。 如需詳細資訊，請參閱 [設定您的支出帳戶和稅務表單](set-up-your-payout-account.md)。

### <a name="payout-hold-status"></a>支出保留狀態

根據預設，我們會以每月為基礎來傳送付款，如上所述。 不過，您可以選擇讓程式保持支出，而且 Microsoft 不會將您的付款發行至您的帳戶。 如果您選擇保留支出，我們會繼續在 [ **支出** ] 頁面中記錄任何收益。 在您解除保留之前，我們不會將任何款項匯到您的帳戶。

若要將您的付款保留，請選取右上方的 **設定** 齒輪圖示，然後選取 [ **帳戶設定**]。 在左側功能表中選取 [付款 **和稅金** ]，然後在 [付款 **和稅務設定檔指派** ] 區段中，找出您想要保留付款的程式。 選取 [ **保留我的付款** ] 核取方塊，以保留此方案的付款。 您可以隨時變更付款保留狀態，但您的決策將會影響下個月的付款。 例如，如果您想要保留四月的支出，請務必在三月底前將支出保留狀態設定為 [開啟]。

一旦您將 [付款保留] 狀態設定為 [ **開啟**]，此程式的所有支出就會保留，直到您清除核取方塊為 [ **關閉**]。 當您這樣做時，您將會在下個月的付款週期中包含 (前提是) 已符合付款閾值。 如果您的支出已保留，但想要在六月產生支出，則在5月底之前清除核取方塊即可 **關閉** 。

>[!Note]
> 您的付款保留狀態會個別套用至每個方案 (Microsoft Store、廣告、Azure Marketplace 等) 。 如果您想要保留所有程式的付款，請個別保存每個方案的款項。

## <a name="payout-statements"></a>支出明細表

付款帳單會顯示您在交易歷程記錄中，從您的供應專案和附加元件銷售的收益。 您也可以查看付款詳細資料，並下載 tsv 或 csv 格式的報表。 若要深入瞭解如何存取付款聲明和交易歷程記錄和付款報告的詳細資料，請參閱付款 [聲明](payout-statement.md) 。 此外，您可以使用 [Partner 支出 API](https://apidocs.microsoft.com/services/partnerpayouts) ，有系統地提取付款報告。

## <a name="next-steps"></a>後續步驟

- [合作夥伴支出 API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支付常見問題](payout-faq.md)
