---
title: 將其他租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在您的合作夥伴中心帳戶中新增、合併或管理多個 Azure AD 租使用者。 深入瞭解您可能會想要進行的一些原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105542"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在您的合作夥伴中心帳戶中新增和管理多個租使用者


**適當的角色**

- 全域系統管理員

這項功能可讓您管理貴公司的多個租用戶，並將其合併到您的合作夥伴中心帳戶。 您可能需要在合作夥伴中心帳戶中管理多個 Azure AD 租使用者的原因有很多。 例如：

- 您的公司可能會購買另一家公司，而您希望新公司中的員工能夠使用合作夥伴中心。 不過，您希望兩個公司保持獨立。 在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶 (PGA) 產生關聯。 此關聯可讓兩個公司的使用者在合作夥伴中心中工作。

- 如果您有一個以上的租使用者來執行您的商務 (例如 contoso.com、contoso.uk、contoso.in) 您可以使用多租使用者將它們系結到相同的電腦帳戶。

- 合併和收購需要您使用多個租使用者 (例如，如果 Contoso 取得 Fabrikam，您就必須能夠同時使用 Constoso.com 和 Fabrikam.com 各自的租使用者) 。

- 來自任何租使用者的使用者都必須能夠：
    1.  存取合作夥伴中心用於訓練、數位下載、MCP 關聯
    2.  指派合作夥伴中心角色，例如 MPN Admin、獎勵系統管理員等等。


## <a name="add-another-azure-ad-tenant-to-your-account"></a>將另一個 Azure AD 租使用者新增至您的帳戶

1. 以全域管理員身分登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)。
1. 從 [**設定**]**圖示選取 [****帳戶設定**]，然後選取 [租使用者]。
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="建立租使用者的關聯"::: 

3. 選取 [ **建立其他 AD 租** 使用者的關聯]，並指出您要關聯的租使用者。

1. 以全域管理員身分登入您想要關聯的租使用者，並確認該關聯。 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="確認租使用者的關聯"::: 

5. 確認之後，您會看到所有的 **設定** 通知。  選取 [ **返回租使用者管理** ]，您會看到列出新加入的租使用者。 
 

>[!NOTE]
>如果租使用者已經與另一個合作夥伴中心帳戶建立關聯，您就無法將它與帳戶產生關聯。


## <a name="remove-a-tenant-from-your-account"></a>從您的帳戶移除租使用者
 
1. 以全域管理員身分登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)。

1. 從 [ **設定** ] 圖示選取 [ **帳戶設定** -> 租使用者]，然後按一下 [ **夥伴** ] 索引標籤。
 
3. 針對您想要中斷關聯的租使用者，按一下 [ **移除** ]。

4. 中斷關聯租使用者表示該租使用者上的使用者將無法再存取合作夥伴中心帳戶，而這可能會影響您的能力。 

除了主要租使用者和您目前登入的租使用者之外，所有相關聯的租使用者都會啟用 [ **移除** ] 按鈕。

:::image type="content" source="images/disassociate.png" alt-text="具有 [移除] 按鈕的租使用者":::
 

## <a name="next-steps"></a>後續步驟

- [新增使用者](create-user-accounts-and-set-permissions.md)






