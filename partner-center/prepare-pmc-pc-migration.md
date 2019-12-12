---
title: 準備從合作夥伴成員資格中心移至合作夥伴中心 |合作夥伴中心
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 從 PMC 移至合作夥伴中心之前，請先複習有用的資訊和常見問題。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8d0e540282b3e683233c188f9258683809af510e
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004857"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>準備從合作夥伴成員資格中心（PMC）移至合作夥伴中心

**Roles adecuados**
-   全域系統管理員
-   Administrador de usuarios
-   Agente de ventas
-   Agente de administración

我們正將成員資格管理從合作夥伴成員中心（PMC）移至合作夥伴中心-單一目的地，以管理您與 Microsoft 的商務關係。 我們希望您的移至合作夥伴中心盡可能有效率且更容易。 我們已識別出合作夥伴中心與 PMC 不同的區域，因此我們認為您會想要先瞭解並準備好，然後再進行移動。

## <a name="account-and-identity-setup"></a>帳戶和身分識別設定

**什麼是 Azure Active Directory （Azure AD）工作帳戶？**

Una cuenta profesional de Azure es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, que se crea automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.

您的工作帳戶會主控您的 Azure AD 使用者及其相關資訊（其電子郵件、密碼、設定檔資料、許可權等）。 工作帳戶也包含群組、應用程式，以及與公司和其安全性有關的其他資訊。 如需詳細資訊，請參閱 。

在合作夥伴中心，您將使用您的公司電子郵件，登入您的帳戶，而不是您的個人電子郵件。
- 您的公司帳戶： john@contoso.com
- 您的個人帳戶： John@outlook.com

您的公司電子郵件是 Azure active directory 租使用者的一部分。 若要在合作夥伴中心擁有帳戶，您需要有 AAD 租使用者。 如需 Azure Active Directory 的詳細資訊，請參閱[在 Azure AD 中建立目錄](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。

**當您從 PMC 移至合作夥伴中心時，如果您有與 Microsoft 的 AAD 租使用者（例如 Office 365），而且您的 CSP 業務也有租使用者，您應該使用哪一個帳戶登入合作夥伴中心？**

您可以使用 CSP 帳戶或 MPN work 電子郵件帳戶登入合作夥伴中心。 如果您選擇使用 CSP 工作電子郵件登入，儀表板上的左側導覽會顯示 MPN 和 CSP 計畫資訊。 如果您使用 MPN Azure AD 租使用者的公司電子郵件登入，只會看到您的 MPN 程式資訊。 MPN 和 CSP 之間的使用者角色不同，因此，如果您在 MPN 和 CSP business 兩者都使用相同的帳戶，請務必據以指派使用者角色。 如需使用者角色的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。

**如果您不想要將現有的 Office 365 Azure AD 租使用者用於合作夥伴中心，您可以在從 PMC 遷移之前，先建立新的租使用者。**

您不想使用現有的 Azure AD 租使用者來設定您的合作夥伴中心帳戶，可能有許多原因。 開始遷移至合作夥伴中心之前，請移至[Azure 入口網站](https://ms.portal.azure.com/#home)建立新的 Azure AD 租使用者。 遵循在 Azure Active Directory 中[建立新的租](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)使用者中的指引。 一旦您建立新的租使用者，請在從 PMC 移至合作夥伴中心時，使用此 AAD 租使用者來設定您的合作夥伴中心帳戶。 您必須是全域管理員，才能建立租使用者。 使用這個新目錄來遷移至合作夥伴中心。


**AAD 全域管理員角色與 PMC MPN 全域管理員角色之間有何差異？**

這些是兩個完全不同的角色，具有不同的許可權。 合作夥伴中心內的 AAD 租使用者全域管理員會管理租使用者-新增或移除使用者、提供及管理密碼、角色和許可權，並可存取其在合作夥伴中心內的所有公司程式。 

PMC 中的 MPN 全域管理員角色可以執行下列動作：

- 查看和編輯所有與公司相關聯的資料，以及公司的所有位置

-  在全域或本機層級新增系統管理員。  此外，全域管理員可以將任何位置的任何人員指派給全域管理員存取權，不論其相關聯的位置為何，都能授與全域存取權。
-  執行任何面向合作夥伴的 UI 功能，包括： 

-  新增/移除使用者

 - 指派/移除角色 

 - 新增/移除/更新位置 

 - 購買專長認證/maps 

-  觀看權益

當 MPN 全域管理員移到合作夥伴中心時，角色稱為 MPN 夥伴管理員，其許可權和工作與合作夥伴中心全域管理員不同。如需合作夥伴中心角色和許可權的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。

**在合作夥伴中心包含來賓使用者角色的使用者角色**

合作夥伴中心具有不同類型的角色，視所需執行的工作類型而定。 有一些角色（例如全域管理員） Azure AD 角色。 某些角色專屬於雲端服務提供者方案或獎勵等方案，而且有 MPN 特有的角色。 若要瞭解合作夥伴中心的角色為何，請參閱[指派使用者角色和許可權](permissions-overview.md)。



**當我的使用者角色從 PMC 移到合作夥伴中心時，會發生什麼事？**

除了進行遷移的 MPN 全域管理員或主要程式連絡人以外，PMC 中的所有使用者都會失去其系統管理員角色。 完成遷移的個人將需要在合作夥伴中心指派角色。 合作夥伴中心的角色與 PMC 中的角色不同。 閱讀 [指派使用者角色和許可權] （許可權-overview.md，並[從 PMC 移至合作夥伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)，以取得合作夥伴中心的使用者角色的詳細資訊。


**我的公司設定檔與我的商務設定檔之間有何差異？**

您的公司設定檔是貴公司的相關資訊，其中包含位址、位置、主要連絡人、銀行和稅務詳細資料。

您的商務設定檔是您向客戶呈現自己的方式，而這是一個行銷頁面，可顯示您的標誌、企業焦點的詳細資料、您的專業知識等等。

**帳戶匯總對我的帳戶的意義為何？**

如果您使用相同的 Azure AD 租使用者，將多個 MPN 帳戶遷移到合作夥伴中心，系統會自動辨識並要求您合併您的帳戶。 即使您有多個與相同 Azure AD 租使用者相關聯的網域，也是如此。 

您仍然可以使用個別的 AAD 租使用者決定遷移至合作夥伴中心，但請注意，這會導致您的專長認證和額外購買成本的隔離評估。 

**如果我有多個 AAD 租使用者和單一 MPN 帳戶，可以在合作夥伴中心連結它們嗎？**

是，在合作夥伴中心，您可以將多個 Azure AD 租使用者連結至單一合作夥伴中心帳戶。
請按一下這裡以進一步了解。 

**將多個 Azure AD 租使用者新增至單一合作夥伴中心帳戶是否有任何限制？**

如果 Azure AD 租使用者已與現有的合作夥伴中心帳戶相關聯，則無法使用多租使用者功能將它與新的合作夥伴中心帳戶產生關聯。 另一個要考慮的方法是，Azure AD 租使用者只能與一個合作夥伴中心帳戶相關聯，但合作夥伴中心帳戶可以有多個相關聯的租使用者。

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft 合作夥伴網路（MPN）成員資格遷移 

**誰可以執行從 PMC 移至合作夥伴中心？**

您的公司 MPN 全域管理員或主要程式連絡人（這兩個角色通常由同一人持有）可以起始和執行移動。

**完成遷移的人員是否會成為合作夥伴中心內公司法律設定檔的主要連絡人？**

但不一定，主要連絡人必須是有權簽署合約的人。

**Microsoft 可以為我遷移我的 MPN 成員資格嗎？**

不。 Microsoft 無法協助您將您的成員資格帳戶移至合作夥伴中心。 您必須使用您的工作帳戶（登入認證）登入 PMC，以開始進行遷移程式，以移動您的帳戶。 完成移動帳戶的步驟之後，您就可以開始管理您的成員資格，並將使用者角色和許可權指派給您的小組，讓他們可以存取權益並協助管理成員資格。 Microsoft 會自動遷移目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含合作夥伴大學存取權的 MCP 關聯。

Microsoft 會自動遷移目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含合作夥伴大學存取權的 MCP 關聯。

**更新原則會如何變更？**

 在 [合作夥伴中心] 中，[更新] 視窗會從您的週年日起到以下30天。

**我們的專長認證會在移至合作夥伴中心後保持不變嗎？**

是的，compentencies 不會受到 [移至合作夥伴中心] 的影響。 如果您注意到不一致的情況，請聯絡[支援](https://partner.microsoft.com/support)人員。


 **移動後，我的權益（包括雲端權益、技術支援、軟體權益、Visual Studio）是否有變更？**

 您的合格權益不會變更。 如果您注意到不一致的情況，請聯絡[支援](https://partner.microsoft.com/support)人員。

 **我們的 Microsoft 帳戶將會接受 Visual Studio 權益嗎？**


 可以。 Los beneficios de Visual Studio asignados a MSA se respetarán y conservarán. También se conservarán después de la renovación en el Centro de partners. 不過，如果您在合作夥伴中心遷移之後移除 MSA 配置，就無法將其新增回合作夥伴中心。

En el Centro de partners, un partner puede agregar cuentas profesionales y cuentas de usuario invitado que son MSA del mismo inquilino donde el partner es administrador de MPN en el inquilino de Azure AD. Si el partner es un administrador global en varios inquilinos de Azure AD y todos estos inquilinos están asociados a la misma cuenta del Centro de partners, se permite que el partner agregue usuarios de todos estos inquilinos a los beneficios de Visual Studio y asignaciones basadas en el uso de Azure.

Aunque a los usuarios invitados se les pueden asignar suscripciones basadas en el uso de Visual Studio mediante el administrador de MPN o el administrador global, los usuarios invitados no pueden iniciar sesión en el Centro de partners mediante su MSA. Sin embargo, los usuarios invitados pueden iniciar sesión en Azure y Visual Studio para validar y usar sus beneficios asignados.


 **我們應該如何管理 MCP 關聯和合作夥伴大學的存取權？**

 從 PMC 移動的 MCP 關聯不會有任何變更。 不過，移至合作夥伴中心後的任何新員工都必須在合作夥伴中心內建立關聯。 現有使用者的所有合作夥伴大學許可權將會保留，但任何新員工都應前往[訓練中心](https://partner.microsoft.com/training)，以取得如何取得合作夥伴大學的相關資訊。

 **當我移到合作夥伴中心後，如何? 看到 MCP 資訊？**

從 [儀表板] 的左側導覽中選取 [**職稱**]。 在 [專長認證 **] 頁面上**，您可以下載技能報告。 技能報告將會列出已取得合作夥伴中心之專長和計畫相關技能的使用者。 如果您的使用者已獲得技能，但那些技能與您正在努力的專長無關，則不會列在報表中。


 **合作夥伴中心是否使用客戶參考？**

 否，您不需要客戶參考以符合合作夥伴中心的專長認證需求。

 **記錄關聯的夥伴會移到合作夥伴中心嗎？**

 是，不會變更記錄的夥伴。 深入瞭解如何將[您的合作夥伴識別碼連結至您的客戶](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。

**因為移至合作夥伴中心，是否會影響獎勵？**

否，如果您已移動帳戶而未合併位置，則不會影響獎勵。 如果您的公司在 PMC 中有多個帳戶，而當您移至合作夥伴中心時，您決定將合併到通用帳戶，則不會有任何獎勵，但激勵支出可能會有延遲。 如果您未移動所有與獎勵計畫相關的 PMC 帳戶，您可能會停止獲得與這些帳戶系結的獎勵。


**合作夥伴中心的獎勵使用者角色為何？** 

合作夥伴中心的獎勵角色是以位置為基礎，並包含獎勵系統管理員和獎勵使用者。 如需這些角色可執行之動作的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。

**可以在全域和位置層級指派給使用者嗎？**

 可以。 您可以將獎勵系統管理員指派為所有位置的獎勵管理員，或每個位置都有自己的獎勵系統管理員。

 **可以在全域或位置層級支付獎勵嗎？**

 獎勵只會在位置層級付費。

**關於參考，我們可以建立多少個商務設定檔？**

您的公司可以建立所需數量的商務設定檔，以完全代表貴公司的興趣。 在每個商務設定檔中，您最多可以列出五個位置，每個國家/地區一個位置。 每個商務設定檔都可以接收其每個位置的參考。

**如何指派參照，我可以預期的變更為何？例如，如果我在某個市場上有一個全球性的公司，而在其他市場上有個地點，則會如何指派參考？**

系統會根據客戶所定義的搜尋參數來指派參照。 因此，不論您是否有一個位置或多個地點，如果客戶指定了所需的位置，而且您有符合其他參數的業務，則參照會移至該位置。








