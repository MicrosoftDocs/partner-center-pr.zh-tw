---
title: 將其他租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 透過您的合作夥伴中心帳戶管理多個租使用者
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389507"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在合作夥伴中心帳戶中新增和管理多個租使用者

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員

您可能需要在合作夥伴中心帳戶中管理多個 Azure AD 租使用者的原因有很多。 例如，您的公司可能購買另一家公司，而您希望新公司的員工能夠使用合作夥伴中心。 不過，您想要讓兩個公司保持獨立。 在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶（PNG）產生關聯。 此關聯可讓兩家公司的使用者在合作夥伴中心內工作。

## <a name="add-another-azure-ad-tenant-to-your-account"></a>將另一個 Azure AD 租使用者新增至您的帳戶

1. 身為全域管理員，請登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。
1. 從 [**設定**]**圖示選取 [****帳戶設定**]，然後選取 [租使用者]。
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="建立租使用者的關聯"::: 

3. 選取 [**關聯另一個 AD 租**使用者]，並指定您想要建立關聯的租使用者。

1. 身為全域管理員，請登入您想要建立關聯的租使用者，並確認該關聯。 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="確認關聯租使用者"::: 

5. 確認之後，您會看到**所有設定**通知。  選取 [**回到租使用者管理**]，您就會看到已列出新加入的租使用者。
 
## <a name="next-steps"></a>後續步驟

- [新增使用者](create-user-accounts-and-set-permissions.md)
