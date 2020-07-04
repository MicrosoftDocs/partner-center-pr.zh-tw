---
title: 遷移部分商務用 Skype 訂閱
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何及何時將過期的商務用 Skype Online 方案1訂閱遷移至新的 Office 365 版本。
author: BrentSerbus
ms.author: brserbus
keywords: 商務用 Skype 方案, 淘汰 Skype, Office 365
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4202e146a470e2231ac33df9878be91e19fcddf3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949611"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>將商務用 Skype Online 方案 1 訂閱移轉至較新的 Office 365 版本

**適用於**

- 合作夥伴中心

商務用 Skype Online 方案1將于2018年8月1日起淘汰。 該日期之後，客戶將再也無法購買新的商務用 Skype 方案 1 訂閱，而現有訂閱在到期後不會自動續約，也不會提供續約選項。 在訂閱的詳細資料頁面上，商務用 Skype Online 方案 1 訂閱狀態已從「自動續約於 [日期]」變更為「到期日 [日期]」。  

為了確保客戶持續的訂閱，您應該將具有即將到期之商務用 Skype Online 方案 1 訂閱的客戶轉換至支援的 SKU 選項，如下所列。 我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。 

>[!NOTE]
>商務用 Skype Online 方案 1 商業和政府 SKU 都將淘汰。

如果您使用 API (CREST 或合作夥伴中心)，請評估訂閱的結束日期加上自動續約 = False 屬性，尋找即將到期的訂閱。 商務用 Skype Online 方案 1 訂閱將於 2018 年 9 月 1 日設定為自動續約 = False。 您可以隨時將客戶移轉至新的方案。 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>商務用 Skype Online 方案 1 取代方案

透過新方案，您的客戶可以運用 Office 365 中的較新特色和功能。 合作夥伴中心的價目表和優惠清單矩陣上可找到定價詳細資料。 

- 選項 1：Office 365 企業版 F1
- 選項 2：Microsoft 365 企業版 F1
- 選項 3：其他 Office 365 方案

|**功能**    |**選項 1**   |**選項 2**   |**選項3**   |
|:-----------------|:-----------------|:-------------|:------------|
|取得商務用 Skype Online 方案 1 包含的所有功能|是   |是   |是   |
|IM 和顯示狀態 |是   |是   |是   |
|透過 IP 的對等音訊和視訊|是   |是   |是   
|以驗證使用者身分加入會議| 是   |是   |是   |

## <a name="transition-customers-to-new-product-plans"></a>將客戶轉換到新產品方案

Microsoft 會持續提供新的產品及服務給我們的合作夥伴。 在這些情況下，您可能需要將客戶升級到新服務，或是從最後將會關閉的 SKU 移轉其訂閱。 將客戶從淘汰的 SKU 移轉到較新的 SKU 時需要依照以下步驟執行：

- 購買新訂閱
- 重新指派目前的使用者授權
- 取消舊訂閱

### <a name="migrate-your-customers-to-new-plans"></a>將您的客戶移轉至新方案

1. 若要購買新的訂用帳戶，請從 [**合作夥伴中心] 功能表**選取 [**客戶**]，選取您想要移動的客戶，然後選取 [**新增訂閱**]。

2. 選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。 

您的客戶現在應該已有舊的和新的訂用帳戶、舊的商務用 Skype Online 方案1訂用帳戶，以及新的「目標」訂用帳戶，例如選項 1-Office 365 Enterprise F1。

3. 若要重新指派客戶的使用者授權，請在 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，選取您要移動的客戶，然後選取 [**使用者和授權**]。 客戶的 [使用者和授權] 頁面隨即開啟。

4. 若要重新指派使用者授權，請選取要重新指派的使用者，然後選取 **\[管理授權\]**。

5. 在 **\[管理授權\]** 頁面中，清除 \[商務用 Skype Online 方案 1 授權\] 核取方塊，然後選取客戶要移動到的訂閱新服務方案。

6. 選取 [提交]。 確認頁面會列出新的授權指派。 為其他需要指派授權的使用者，繼續進行這個相同程序。

將使用者授權移至新服務後，您就可以放心地取消客戶層級的已淘汰訂閱。

7. 從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。 選取您要取消其訂閱的客戶。

8. 在訂閱詳細資料頁面中，將訂閱設定為 **\[已暫停\]**。

9. 選取 [**提交]。**

舊訂閱已暫停，而新訂閱為使用中。 暫停的訂閱將在 120 天後自動解除佈建。 客戶不會因為舊訂閱而產生額外費用。

