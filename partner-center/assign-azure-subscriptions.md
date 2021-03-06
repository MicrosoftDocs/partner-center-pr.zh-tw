---
title: 將 Azure 訂用帳戶指派給客戶
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心中將 Azure 訂用帳戶指派給您的客戶，以及如何讓客戶管理自己的訂用帳戶。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8cac2a6edc9199befeae940ed271c3236440c260
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "96473946"
---
# <a name="assigning-azure-subscriptions-to-customers-in-partner-center"></a>在合作夥伴中心指派 Azure 訂用帳戶給您的客戶

**適當的角色**

- 全域系統管理員
- 銷售代理人

## <a name="assign-azure-subscriptions-to-your-customers"></a>將 Azure 訂用帳戶指派給您的客戶

1. 從 **合作夥伴中心**] 功能表中選取 [**客戶**]，並找出您想要管理的客戶。

2. 選取該列結尾的向下鍵以展開客戶記錄，然後選取 **\[Microsoft Azure 管理入口網站\]**。 系統會將您導向至可管理客戶訂用帳戶的 [Azure 入口網站](https://portal.azure.com/) 。

3. 從 Azure 入口網站選取 [ **訂閱**]。

4. 選取您想要指派的訂閱，然後選取 **\[存取控制\]**。

5. 選取 **\[新增\]** 將使用者新增至訂閱。 

6. 將使用者新增至訂閱後，您可以指派角色給使用者，以及使用者可以存取的特定帳戶。

## <a name="enable-customers-to-manage-their-azure-subscriptions"></a>讓客戶能夠管理他們的 Azure 訂閱

建立客戶的 Microsoft Azure 訂閱之後，您可以允許他們管理訂閱。 若要這樣做，您必須登入客戶的 Microsoft Azure 管理入口網站。 

1. 若要開啟客戶的 Azure 入口網站，請在客戶清單中展開客戶的清單，或選取客戶的名稱，然後選取 [ **Microsoft Azure 管理入口網站**]。

   > [!NOTE]  
   > 如果系統提示您登入 Azure 入口網站，您可能沒有委派的系統管理許可權。 選取 **\[要求建立關係\]** 以邀請客戶將您列名為他們的「記錄可查夥伴」。 客戶接受您的邀請後，系統就會自動將委派的管理員權限授與您。

2. 在 Azure 入口網站中，開啟客戶的訂用帳戶清單，然後選取客戶的 Azure 訂用帳戶。

3. 將角色指派給任何客戶的使用者，讓他們可以建立和管理其訂用帳戶下的資源。

## <a name="next-steps"></a>後續步驟

- [CSP 合作夥伴如何將訂用帳戶銷售給客戶](customer-subscriptions.md)

- [如何取得管理客戶服務或訂用帳戶的許可權](customers-revoke-admin-privileges.md)
