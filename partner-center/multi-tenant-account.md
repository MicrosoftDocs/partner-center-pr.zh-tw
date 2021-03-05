---
title: 將租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心帳戶中新增、合併或管理多個 Azure AD 租使用者，並瞭解您可能會想要這麼做的原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124800"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>在您的合作夥伴中心帳戶中新增和管理多個租使用者


**適當的角色**

- 全域系統管理員
- 帳戶管理員

本文討論如何為您的公司將多個 Azure Active Directory (Azure AD) 租使用者，然後在您的合作夥伴中心帳戶中新增及管理這些租使用者。 有許多原因需要這麼做。 例如：

- 假設您的公司 Contoso 已獲得另一家 Fabrikam。 您希望兩個公司保持獨立，但您希望新的員工能夠使用合作夥伴中心。 在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶 (PGA) 相關聯。 此關聯可讓兩個公司的使用者在合作夥伴中心內工作。

- 如果您使用多個租使用者執行業務 (例如， *contoso.com*、 *contoso.uk* 和 *contoso.in*) ，您可以使用多租使用者將這些租使用者群組在相同的電腦帳戶中。

- 如果合併和收購指導方針要求您使用兩個公司的租使用者，您可以同時使用 *constoso.com* 和 *fabrikam.com* 租使用者。

- 任何租使用者的使用者都必須能夠：
    * 存取合作夥伴中心以取得訓練、數位下載或 Microsoft 認證專業人員 (MCP) 關聯。
    * 指派合作夥伴中心角色，例如 Microsoft Partner Network (MPN) 系統管理員或獎勵系統管理員。

## <a name="add-an-azure-ad-tenant-to-your-account"></a>將 Azure AD 租使用者新增至您的帳戶

1. 以全域管理員身分登入 [Microsoft 合作夥伴中心](https://partner.microsoft.com/dashboard)。

1. 選取右上方的 [**設定**]，選取 [**帳戶設定**]，然後選取 [租使用者 **]。**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="[Azure AD 設定檔] 窗格上 [關聯] 按鈕的螢幕擷取畫面。"::: 

1. 選取 [ **關聯**]，然後指定您要關聯的租使用者。

1. 在提示字元中，以全域管理員身分登入您想要關聯的租使用者，然後選取 [ **確認**]。 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[確認新的 Azure AD 關聯] 窗格上 [確認] 按鈕的螢幕擷取畫面。"::: 

   確認關聯之後，就會顯示 **所有設定** 的訊息。 若要查看新增的租使用者，請選取 [ **返回租使用者管理**]。 
 
>[!NOTE]
>如果租使用者已與另一個合作夥伴中心帳戶相關聯，您就無法將該租使用者與帳戶產生關聯。


## <a name="remove-a-tenant-from-your-account"></a>從您的帳戶移除租使用者
 
1. 以全域管理員身分登入 [Microsoft 合作夥伴中心](https://partner.microsoft.com/dashboard)。

1. 選取右上方的 [ **設定** ] 圖示，然後選取 [ **帳戶設定**]。

1. 在左窗格中 **，選取 [** 租使用者]。 在 [ **管理 AZURE AD** 租使用者] 底下，選取 [ **夥伴** ] 索引標籤。
 
1. 選取您要移除其關聯的租使用者旁的 [ **移除** ]。

   :::image type="content" source="images/disassociate.png" alt-text="目前租使用者關聯及其 [移除] 連結的螢幕擷取畫面。":::

   如先前的螢幕擷取畫面所示，除了主要租使用者和您目前登入的租使用者之外，所有相關聯的租使用者都會啟用 [ **移除** ] 連結。 

   > [!NOTE]   
   > 當您移除租使用者時，該租使用者上的使用者將無法再存取合作夥伴中心帳戶，因此移除可能會影響您的專長認證。 

## <a name="next-steps"></a>接下來的步驟

- [建立使用者帳戶](create-user-accounts-and-set-permissions.md)






