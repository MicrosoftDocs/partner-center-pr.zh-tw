---
title: 遷移 Office 365 E4 訂閱
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 企業版 E4 從 2017 年 4 月 7 日起淘汰。 了解如何將您的客戶訂閱移轉至新版 Office 365。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbd2aceac62a7e726ed81a78305ea23213c94156
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949041"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>將 Office 365 E4 訂閱移轉至新版 Office 365

**適用於**

-  合作夥伴中心

**適當的角色**
-   全域系統管理員
-   使用者系統管理員
-   系統管理代理人
-   銷售代理人

Office 365 企業版 E4 方案已淘汰，自 2017 年 4 月 7 日起生效。 您在這個日期之後無法再購買新的 Office 365 E4 訂閱，而且現有的 E4 訂閱到期時不會自動續約。

當 E4 訂閱結束時，會被取消。 為了確保客戶持續的訂閱，您應該將具有即將到期 E4 訂閱的客戶轉換至支援的 SKU 選項，如下所列。 我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。 

> [!NOTE]  
> Office 365 Enterprise E4 商業和政府 Sku 均已淘汰。
 
在訂閱的詳細資料頁面上，E4 訂閱狀態已從「自動續約於 [日期]」變更為「到期日 [日期]」。 

如果您使用 API（CREST 或合作夥伴中心），您可以評估訂閱的結束日期加上自動續約 = False 屬性，探索即將到期的訂閱。 

E4 訂閱會設定為自動續約 = False 於 2017 年 4 月 7 日。 您可以隨時將客戶移轉至新的方案。 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 企業版 E4 取代方案

您可以選擇維持 E4 相同的功能，或讓您的客戶善加利用 Office 365 和商務用 Skype Online 中較新的功能。 合作夥伴中心的價目表和優惠清單矩陣上可找到定價詳細資料。 Secure Product Enterprise E3 或 Secure Productive Enterprise E5 可分別用來取代下列選項中的 Office 365 企業版 E3 或 Office 365 企業版 E5。

- 選項 1：Office 365 企業版 E5

- 選項 2：Office 365 企業版 E3 + 商務用 Skype 雲端 PBX

- 選項 3：Office 365 企業版 E3 + 商務用 Skype Plus CAL（E4 的價格和功能同位）

- 選項 4：Office 365 企業版 E3


| 功能 | 選項 1 | 選項 2 | 選項 3 | 選項 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| 取得 Office 365 企業版 E4 中包含所有的功能？ | 是 | 是 | 是 | 否 |
| 在 Office 365 中管理電話號碼？ | 是 | 是 | 否 | 否 |
| 在內部部署和 Office 365（混合部署）中管理電話號碼？ | 是 | 是 | 否 | 否 |
| 選項可新增 PSTN 語音通話方案嗎？ | 是 | 是 | 否 | 否 |
| PSTN 會議？ | 是 | 否 | 否 | 否 |
| 共同作業、分析和安全性的進階工具？ | 是 | 否 | 否 | 否 |
| 互動式報告、儀表板，以及資料視覺效果？ | 是 | 否 | 否 | 否 | 
| 使用內建隱私權、透明度及精簡使用者控制項，對資料安全性與合規性的更多控制權？ | 是 | 否 | 否 | 否 | 

## <a name="transition-customers-to-new-product-plans"></a>將客戶轉換到新產品方案

Microsoft 會持續提供新的產品及服務給我們的合作夥伴。 在這些情況下，您可能需要將客戶升級到新服務，或是從最後將會關閉的 SKU 移轉其訂閱。 將客戶從淘汰的 SKU 移轉到較新的 SKU 時需要依照以下步驟執行：

-   購買新訂閱
-   重新指派目前的使用者授權
-   取消舊訂閱

請依照下列步驟，將客戶的 Office 365 企業合作夥伴 E4 訂閱移轉到上述表格中的選項。

### <a name="step-1---purchase-the-new-subscription"></a>步驟 1 - 購買新訂閱

1. 從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，選取您想要移動的客戶，然後選取 [**新增訂閱**]。

2. 選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。

   您的客戶現在應已有舊的和新的訂閱、舊的 Office 365 Enterprise E4 訂閱和新的「目標」訂用帳戶，例如選項 1-Office 365 企業版 E5。

### <a name="step-2---reassign-the-customers-users-licenses"></a>步驟 2 - 重新指派客戶的使用者授權

1. 從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，選取您想要移動的客戶，然後選取 [**使用者和授權**]。 客戶的 [使用者和授權] 頁面隨即開啟。

2. 若要重新指派使用者授權，請選取要重新指派的使用者，然後選取 [**管理授權**]。

3. 在 **\[管理授權\]** 頁面中，清除 **\[Office 365 企業版 E4\] ** 授權核取方塊，然後選取客戶訂閱移動到的新服務方案。

4. 選取 [提交]。 確認頁面會列出新的授權指派。

5. 針對需要重新指派授權的任何其他客戶使用者繼續執行相同步驟。

將使用者授權移至新服務後，您就可以放心地取消最上層 \[客戶\] 的已淘汰訂閱。

### <a name="step-3---cancel-the-old-subscription"></a>步驟 3 - 取消舊訂閱

1. 從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。 選取您想要移動的客戶，然後選取您想要取消的訂閱。

2. 在 [訂閱詳細資料] 頁面中，將訂閱狀態設定為 [已**暫停**]。

3. 選取 [提交]。

舊訂閱已暫停，而新訂閱為使用中。 暫停的訂閱將在 120 天後自動解除佈建。 客戶不會因為舊訂閱而產生額外費用。



 



