---
title: 將 Kaizala Pro 訂閱遷移至 Microsoft 365
description: 瞭解如何將 Kaizala Pro 訂閱遷移至 Microsoft 365 或 Office 365 版本。 如需轉換客戶的詳細資料，請閱讀這篇文章。
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175174"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>將 Kaizala Pro 獨立訂閱遷移至 Microsoft 365 或 Office 365 版本

從2020年7月1日起，Microsoft 即將結束 Kaizala Pro 獨立服務的銷售。 客戶將無法再于此日期之後購買新的 Kaizala Pro 訂用帳戶，而且現有的 Kaizala Pro 訂閱將不會在到期時自動更新。

為確保客戶的持續性，您應該將即將到期的 Kaizala Pro 獨立訂用帳戶轉換為支援的 SKU 選項，如下所示。 建議您將客戶移至訂用帳戶年度結束日期之前的新訂用帳戶，以避免客戶發生任何服務中斷。

如果您使用 API (CREST 或合作夥伴中心) ，您可以評估訂用帳戶的結束日期，並將 [自動更新] 屬性設定為 [false]，以探索即將到期的訂閱： `auto renew = False` 。

E4 訂閱將于 `auto renew=False` 2020 年7月1日設定為。 您可以隨時將客戶移轉至新的方案。

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro 獨立取代方案

透過新的方案，您的客戶可以利用 Microsoft 365 中的較新特性和功能。 合作夥伴中心的價目表和優惠清單矩陣上可找到定價詳細資料。

- [**商務 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)，包括：  
   - Microsoft 365 商務基本版
   - Microsoft 365 商務標準版
   - Microsoft 365 商務進階版
    
- [**適用于 Frontline 的 Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)，包括：
   - Microsoft 365 F3 (先前的 Microsoft 365 F1) 與 Office 365 F3
    
- [**適用于 Enterprise 的 Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)，包括： 
   - Office 365 E1
   - Microsoft 365 E3 與 Office 365 E3
   - Microsoft 365 E5 與 Office 365 E5

- [**Microsoft 365 教育**](https://www.microsoft.com/education/buy-license/microsoft365)版，包括： 
    - Microsoft 365 A1 和 Office 365 A1
    - Microsoft 365 A3 和 Office 365 A3
    - Microsoft 365 A5 和 Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>將客戶轉換到新產品方案

Microsoft 會持續提供新的產品及服務給我們的合作夥伴。 在這些情況下，您可能需要將客戶升級到新服務，或是從最後將會關閉的 SKU 移轉其訂閱。 將客戶從淘汰的 SKU 移轉到較新的 SKU 時需要依照以下步驟執行：

A. 購買新訂閱

B. 重新指派目前的使用者授權

C. 取消舊訂閱


## <a name="migrate-your-customers-to-new-plans"></a>將您的客戶移轉至新方案

### <a name="a-purchase-the-new-subscription"></a>A. 購買新訂閱

1. 若要購買新的訂用帳戶，請選取 [ **合作夥伴中心** ] 功能表中的 [ **客戶**]，選取您要移動的客戶，然後選取 [ **新增訂閱**]。

2. 選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。

您的客戶現在應該會有舊的和新的訂用帳戶，也就是舊的 Kaizala Pro 獨立訂用帳戶和新的「目標」訂用帳戶，例如選項 1-Office 365 Enterprise F1。

### <a name="b-reassign-current-user-licenses"></a>B. 重新指派目前的使用者授權

1. 若要重新指派客戶的使用者授權，請從 [ **合作夥伴中心** ] 功能表選取 [ **客戶**]，選取您要移動的客戶，然後選取 [ **使用者和授權**]。 [客戶的使用者和授權] 頁面隨即開啟。

2. 若要重新指派使用者授權，請選取要重新指派的使用者，然後選取 [ **管理授權**]。

3. 在 [ **管理授權** ] 頁面上，清除 [Kaizala Pro 獨立授權] 核取方塊，然後為客戶移至的訂用帳戶選取新的服務方案。

4.  選取 [提交]  。 確認頁面會列出新的授權指派。 為其他需要指派授權的使用者，繼續進行這個相同程序。

### <a name="c-cancel-old-subscription"></a>C. 取消舊訂閱

將使用者授權移至新服務後，您就可以放心地取消客戶層級的已淘汰訂閱。

1.  從 [ **合作夥伴中心** ] 功能表選取 [ **客戶**]。 選取您要取消其訂閱的客戶。

2.  在訂閱詳細資料頁面中，將訂閱設定為 **\[已暫停\]**。

3.  選取 [提交]  。

舊訂閱已暫停，而新訂閱為使用中。 暫停的訂閱將在 120 天後自動解除佈建。 客戶不會因為舊訂閱而產生額外費用。
