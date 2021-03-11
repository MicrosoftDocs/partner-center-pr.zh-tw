---
title: 查看您的獎勵和計畫詳細資料
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 使用這些頁面來查看和管理獎勵方案狀態
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4c4b3a9a71027f5fb02bc29566c20c214e3df371
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022803"
---
# <a name="view-your-incentives-program-details"></a>查看您的獎勵計畫詳細資料

**適當的角色**

- 獎勵系統管理員
- 獎勵使用者
- 全域系統管理員
- MPN 合作夥伴系統管理員

本文說明 [ **我的獎勵總覽** ] 頁面，其中顯示您的獎勵計畫的整體狀態，以及每個位置的每個程式的狀態。 它也會提供不同的註冊狀態。

>[!NOTE]
>如需合作夥伴中心獎勵與獎勵功能的詳細資訊，請參閱 [合作夥伴投資和獎勵](https://partner.microsoft.com/membership/partner-incentives) (登入所需的) 。

## <a name="access-the-incentives-overview-page"></a>存取獎勵總覽頁面

1. 登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。
1. 選取 [ **獎勵**]，然後從功能表中選取 **[總覽** ]。
1. 在頁面頂端查看收益和付款摘要，並在下表中取得進一步的詳細資料。 您也可以排序、分組和展開隨附的資料表：

   - 若要依資料行排序，請選取資料行名稱。
   - 若要依程式分組，請選取資料表上方的 [ **依程式** ] 索引標籤。
   - 若要依位置分組，請選取資料表上方的 [ **依位置** ] 索引標籤。
   - 若要查看特定群組內註冊的更多詳細資料，請選取指定資料列結尾的燕號符號。 這個箭號會展開您的觀點。
1. 如果需要進一步動作以註冊計劃，此資訊將會出現在 **狀態** 欄中。 在此情況下，請選取＞形箭號，以了解您需要採取的後續步驟。

## <a name="enrollment-status"></a>註冊狀態

下表說明 [ **狀態** ] 資料行中顯示的不同註冊狀態。

| **狀態**         | **出現時間** |
|:------------------------------------|:------------------|
| 必要的動作  | 合作夥伴已接受邀請以註冊獎勵方案，但可能需要更新銀行或稅務資訊。 請參閱任何後續步驟的 **必要動作** 資料行，或在合作夥伴中心更新您的銀行或稅務資訊的連結。 |
| 已停用  | 獎勵系統不再提供特定的獎勵方案。 |
| 已註冊  | 所有稅務和銀行資訊都已經過驗證。 合作夥伴不需要進一步的註冊動作。 |
| 正在註冊  | 使用者不是獎勵系統管理員，而且註冊是在 **所需的動作** 或 **驗證註冊** 狀態中。|
| 非使用中/不合格 | 這次的獎勵計畫可能尚未開放註冊，或合作夥伴不符合目前的註冊或重新註冊資格。 <br><br> 如果狀態為不 **合格**，則表示夥伴不符合計畫目前的資格需求;選取註冊狀態底下的 [ **查看資格需求** ] 連結，將會顯示符合資格的需求，以及符合的需求。 <br><br> 您也可能會看到虛擬組織 (VORG) 或合作夥伴通用帳戶 (PGA) 註冊的 **非** 使用中狀態，但在獎勵計畫中不再有效。  |
| 已邀請  | 已將新的獎勵方案註冊邀請傳送給合作夥伴，但合作夥伴尚未開始註冊程式。 連續的 [ **必要動作** ] 資料行會顯示後續步驟和任何相關連結。  |
| 正在驗證註冊  | 合作夥伴已完成或更新了新的或現有註冊的銀行與稅務資訊，並正在等候 Microsoft 驗證此資訊。 在驗證過程中， **驗證註冊** 最多可能會出現48小時。  |

## <a name="see-your-payment-information"></a>查看您的付款資訊

選取畫面右上角的付款圖示來存取這些不同的摘要：

- 交易記錄
- 付款
- 匯出資料

:::image type="content" source="images/payouts/payout-overview.png" alt-text="說明合作夥伴中心入口網站右上角的支出圖示":::

這項資訊包括您在獎勵計劃中註冊後的獎勵總收益和付款。 此頁面也包含收益和付款 (依位置或計劃)，以及建議您採取的所有進一步動作，以便在特定位置註冊計劃。 

您也可以使用 [合作夥伴付款 API](https://apidocs.microsoft.com/services/partnerpayouts) 來連接並直接取得付款交易與付款資料。 若要深入瞭解，請參閱付款 [聲明](payout-statement.md) 。

## <a name="next-steps"></a>下一步

- [支付明細表](payout-statement.md)
