---
title: 尋找桌面人數和費用等級
ms.topic: how-to
ms.date: 02/18/2021
description: 瞭解如何使用 Channel 獎勵平臺 (晶片) 找出合約的桌面計數和費用層級資訊。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756113"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>找出合約的桌面計數和費用等級

**適當的角色**

- 主要連絡人或計畫管理員

您可以登入 [explore.ms](https://www.explore.ms/) 以審查合約，或下載檔案，以提供桌面人數和費用等級的合約詳細資料。

## <a name="to-locate-the-information"></a>找出資訊

### <a name="method-1--explorems"></a>方法1– Explore.ms

1. 在 Internet Explorer 中開啟 [explore.ms](https://www.explore.ms/) 。 

>[!Note]
>您無法在 Google Chrome 或 Microsoft Edge 中執行此功能。

2. 使用您的公司/學校帳戶或 live ID 登入。  

3. 在 [ **報表** ] 欄位中，選取 [ **協定**]。

4. 在產生的頁面上，于 [ **搜尋** ] 欄位中輸入合約編號，然後選取 [ **選取/訂購資料行**]。

5. 在快顯視窗中，從 [可用的資料行] 清單中選取 [ **合約桌面計數** ]，然後選取向右箭號以加入資料行。 選取 [確定]。

6. 選取 [ **搜尋]。**

7. 在產生的畫面中，流覽結果以尋找 [ **合約桌面計數** ] 資料行。 

8. 根據下方的費率表格，使用桌面計數來決定費用等級。  

| 費用等級 | 桌面計數 |
| ------ | :-----------: |
|  A | 0-2399    |
|  B | 2400–5999    |
|  C | 6000–14999    |
|  D | 15000 +   |

>[!NOTE]
>企業獎勵層級是以桌面或使用者計數為基礎， (以) 的商業和公共部門 (PS) 註冊的較高者為准。 針對沒有自然相關聯的桌面或使用者計數的註冊，Microsoft 會根據隨附 EA 的桌面計數或使用者計數來套用桌面計數。 <br><br>如果沒有隨附的 EA，費用層級會以註冊的定價層級為基礎。 您也可以在 [www.explore.ms](https://www.explore.ms/)上查看交易的定價層級。 <br><br>如果現有的 EA/EAS 上有多個集區和/或定價層級，Microsoft 將會在最高指派的定價/集區層級上支付獎勵，層級 A 最低，而層級 D 最高。

#### <a name="pool-and-pricing-levels"></a>集區和定價層級

使用上面所述的步驟在 explore.ms 中搜尋合約號碼之後，請選取合約編號。 這會將您帶到 [合約詳細資料] 頁面，這會顯示 **合約摘要** 和 **供應** 專案。 [供應專案] 區段包含定價層級。

## <a name="method-2---chip"></a>方法 2-晶片

1. 登入晶片並選取 LSP 獎勵。

2. 從 [**合作夥伴付款摘要**] 頁面上，選取您要查看的報表月份，然後從 [**匯出至 Excel**] 下的下拉式清單中選取 [**計算詳細資料**]：

:::image type="content" source="images/chip/chiplocate.png" alt-text="找出程式詳細資料":::

3. 匯出將會開始，您可以開啟檔案，或儲存/另存新檔至目的地。

4. 當報表開啟時，流覽至位於左下角的 [ **DetailReport-FlatFile** ] 索引標籤：

:::image type="content" source="images/chip/flatfile.png" alt-text="一般檔案下載":::

您現在可以在 [資料行 J] 中搜尋您要尋找的合約編號，然後您會在 [資料行 R] 中找到指派的桌面計數，標示為 [Agreement_DesktopCount]。 您也可以在「AI 標示的階層」資料行中確認此合約的費用等級。

## <a name="next-steps"></a>下一步

- [針對晶片存取問題進行疑難排解](chip-access-trouble.md)
