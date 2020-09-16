---
title: 區域 PSTN 服務稅金和費用
description: 身為交易 Microsoft 365 語音產品的 Office 365 合作夥伴，您可能會受到 PSTN 服務的區域性稅金、費用或法規需求所規範。
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594454"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>區域稅、公用交換電話網絡的法規 (PTSN) 服務

**適用於**

- 合作夥伴中心
- Office 365 合作夥伴交易 Microsoft 365 的語音產品

**適當的角色**
-    全域系統管理員
-    使用者系統管理員
-    系統管理代理人

在某些管轄區中 (PSTN) 服務的公用交換電話網絡，可能會受到可能影響合作夥伴訂單和發票的特殊法律需求。 在美國（包括波多黎各），PSTN 服務（包括音訊會議、通話方案和通訊點數）受限於特殊的稅務和法規需求。 在美國和波多黎各中，Microsoft 價格的 PSTN 服務為含稅（含）。  獨特的 PSTN 稅和法規將會影響 Office 365 合作夥伴交易 Microsoft 365 的語音產品。  如果合作夥伴會標示 Microsoft PSTN 服務的價格，他們可能要負責計算和代繳 PSTN 稅金及費用。

## <a name="partner-recommendations"></a>合作夥伴建議

與您的稅務和法律顧問合作，瞭解您的組織對於 PSTN 服務的法規、稅金和費用，以及其他潛在負債的責任。

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>發票簡報和夥伴對帳檔案

美國、波多黎各和加拿大地區的 CSP 發票和 CSP 對帳檔案，包括商務用 Skype PSTN 和 Microsoft 365 語音服務會為 PSTN 和非 PSTN 元件提供個別的明細專案。

此外，CSP 發票會顯示下列註腳：

* 顯示的價格是音訊會議和通話方案服務的費用。  任何適用的交易稅金都會以除美國境內的銷售以外的顯示數量來計費。  在美國，所顯示的價格為含稅，因為它包含通話方案和音訊會議服務的費用，以及我們需要收取的稅金和費用費用。  音訊會議和通話方案服務由獲得授權的 Microsoft 分支機搆提供服務。  如需詳細資料，請參閱 [Microsoft 大量授權](https://go.microsoft.com/fwlink/?LinkId=690247)。

## <a name="reconciliation-file-example"></a>對帳檔案範例

Office 365 Enterprise E5 以兩個具有相同名稱和相同 Id 的明細專案形式出現在對帳檔案，但每個明細專案都有唯一的單位價格 (範例： $28.40 和 $2.00) 。 這會區隔 Office 365 優惠的商務用 Skype PSTN 會議元件，讓您可以正確地套用稅金。

**夥伴對帳範例 #1 (選取資料行) ：**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企業版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |循環費用   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 企業版 E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |循環費用   |2.00   |

**合作夥伴對帳範例 #2**

加拿大提供的 Microsoft 365 商務版 Voice 有額外的 PSTN 的可納稅元件，這些元件會在 CSP 發票上合併 (類似于 Office 365 E5、提供兩條明細專案，一個用於 PSTN 元件，另一個用於非 PSTN 元件) 。  Microsoft 365 商務版 Voice 的 CSP 對帳檔案將會個別顯示所有的 PSTN 可納稅元件， (個別的 PSTN 元件不會合並。CSV 或 API 工具) 。  在對帳檔案中找到之客戶的訂單詳細資料和計費金額總和將符合 CSP 發票。

## <a name="additional-resources"></a>其他資源
如需詳細資訊，請造訪 [適用于合作夥伴的 Microsoft 365](https://www.microsoft.com/microsoft-365/partners/) 網站。

