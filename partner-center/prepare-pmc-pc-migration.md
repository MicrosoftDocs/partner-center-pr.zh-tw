---
title: 從 Partner Membership Center 移動
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 從 Partner Membership Center 移至合作夥伴中心之前，請先檢閱有用的資訊和常見問題集。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: a6e188bbd86b066152f90be90d92abb2539f38b3
ms.sourcegitcommit: 3a1c0934ff337fc164bee690e7b9d69d113fdb99
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/03/2020
ms.locfileid: "84328309"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>準備從 Partner Membership Center (PMC) 移至合作夥伴中心

**適當的角色**
- 全域系統管理員
- 使用者系統管理員
- 銷售代理人
- 系統管理代理人

我們正將成員資格管理從 Partner Membership Center (PMC) 移至合作夥伴中心 - 以此單一目的地管理您與 Microsoft 的商務關係。 我們希望您能夠盡可能輕鬆有效地移至合作夥伴中心。 我們已識別出合作夥伴中心與 PMC 不同的層面，而且我們認為您會想要先充分了解並做好準備，再進行移轉。

## <a name="account-and-identity-setup"></a>帳戶和身分識別設定

**什麼是 Azure Active Directory (Azure AD) 公司帳戶？**

Azure 工作帳戶是您公司在 Azure 公用雲端的專用且隔離的虛擬表示，這已在您訂閱 Microsoft 雲端服務 (例如 Azure、Microsoft Intune 或 Office 365) 時建立。

您的公司帳戶會裝載 Azure AD 使用者及其相關資訊 (電子郵件、密碼、設定檔資料、權限等等)。 公司帳戶也包含群組、應用程式，以及其他有關公司與其安全性的資訊。 

您的公司電子郵件是 Azure Active Directory 租用戶的一部分。 若要在合作夥伴中心擁有帳戶，您必須要有 AAD 租用戶。 如需 Azure Active Directory 的詳細資訊，請參閱[在 Azure AD 中建立目錄](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。

在合作夥伴中心，您將使用您的公司電子郵件登入帳戶，而不是使用個人電子郵件。
- 您的公司帳戶：john@contoso.com
- 您的個人帳戶：John@outlook.com

**如果您有與 Microsoft (例如 Office 365) 搭配使用的 AAD 租用戶，同時也有用於雲端解決方案提供者業務的租用戶，應使用哪個帳戶登入合作夥伴中心？**

您可以使用雲端解決方案提供者帳戶或 MPN 公司電子郵件帳戶登入合作夥伴中心。 如果您選擇使用雲端解決方案提供者公司電子郵件登入，儀表板上的左側導覽將會顯示 MPN 和雲端解決方案提供者計畫資訊。 如果您使用 MPN Azure AD 租用戶的公司電子郵件登入，則只會看到 MPN 計畫資訊。 

**如果您不想將現有的 Office 365 Azure AD 租用戶用於合作夥伴中心，您可以在從 PMC 移轉之前，先建立新的租用戶。**

您不想使用現有的 Azure AD 租用戶來設定合作夥伴中心帳戶，可能有許多原因。 開始移轉至合作夥伴中心之前，請先移至 [Azure 入口網站](https://ms.portal.azure.com/#home)建立新的 Azure AD 租用戶。 請依照[在 Azure Active Directory 中建立新的租用戶](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)中的指引操作。 使用新的 AAD 租用戶來設定您的合作夥伴中心帳戶。 您必須是全域管理員，才能建立租用戶。 


**合作夥伴中心的使用者角色 (包括來賓使用者角色)**

合作夥伴中心具有不同類型的角色，視所需執行的工作類型而定。 有些角色屬於 Azure AD 角色，例如全域管理員。 有些角色則專屬於計畫 (例如雲端服務提供者計畫) 或獎勵，此外也有專屬於 MPN 的角色。 若要了解所有的合作夥伴中心角色，請參閱[指派使用者角色和權限](permissions-overview.md)。

**我的使用者角色從 PMC 移至合作夥伴中心後，將會如何？**

除了 MPN 全域管理員或執行移轉的主要計畫連絡人以外，PMC 中的所有使用者都將失去其管理員角色。 完成移轉的人員將必須在合作夥伴中心指派角色。 合作夥伴中心的角色與 PMC 中的角色並不相同。 請參閱 [指派使用者角色和權限] (permissions-overview.md) 和[從 PMC 移至合作夥伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)，以深入了解合作夥伴中心的使用者角色。


**我的公司設定檔與商務設定檔之間有何差異？**

公司設定檔是公司的相關資訊，包括地址、位置、主要連絡人、銀行和稅務詳細資料。

商務設定檔則是您向客戶介紹自己的方式，這是一個行銷頁面，可顯示您的標誌、企業焦點的詳細資料、您的專業能力等等。

**帳戶合併對我的帳戶有何意義？**

如果您使用相同的 Azure AD 租用戶將多個 MPN 帳戶移轉至合作夥伴中心，系統會自動加以辨識，並要求您合併帳戶。 即使您有多個網域與相同的 Azure AD 租用戶相關聯，仍是如此。 

您仍可決定使用個別的 AAD 租用戶來移轉至合作夥伴中心，但請注意，這會導致您的專長認證受到單獨評估，並產生額外的購買成本。 如需帳戶彙總的詳細資訊，請參閱[合併您的公司帳戶](consolidate-accounts.md)

**如果我有多個 AAD 租用戶和單一 MPN 帳戶，是否可在合作夥伴中心將其連結嗎？**

是，在合作夥伴中心，您可以將多個 Azure AD 租用戶連結至單一合作夥伴中心帳戶。
如需帳戶彙總的詳細資訊，請參閱[合併您的公司帳戶](consolidate-accounts.md)

**將多個 Azure AD 租用戶新增至單一合作夥伴中心帳戶時是否有任何限制？**

如果 Azure AD 租用戶已與現有的合作夥伴中心帳戶相關聯，則無法使用多租用戶功能將其與新的合作夥伴中心帳戶產生關聯。 另一方面也須考量，一個 Azure AD 租用戶只能與一個合作夥伴中心帳戶相關聯，但一個合作夥伴中心帳戶可以有多個相關聯的租用戶。

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Microsoft 合作夥伴網路 (MPN) 成員資格移轉 

**從 PMC 到合作夥伴中心的移轉可由誰執行？**

此移轉可由公司的 MPN 全域管理員或主要計畫連絡人 (這兩個角色通常由同一人擔任) 起始和執行。

**完成移轉的人員是否會在合作夥伴中心的法定公司設定檔中成為主要連絡人？**

不一定，但主要連絡人必須是有權簽署合約的人。

**Microsoft 可為我移轉 MPN 成員資格嗎？**

不可以。 Microsoft 無法協助您將成員資格帳戶移至合作夥伴中心。 您必須使用公司帳戶 (登入認證) 登入 PMC，然後開始進行移轉程序，以移動您的帳戶。 完成移動帳戶的步驟之後，您即可開始管理成員資格，並將使用者角色和權限指派給小組，使其能夠存取權益以及協助管理成員資格。 Microsoft 會自動移轉目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含 Partner University 存取權在內的 MCP 關聯。

Microsoft 會自動移轉目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含 Partner University 存取權在內的 MCP 關聯。

**續約原則將有何變更？**

 在合作夥伴中心，續約時間範圍為您的週年日起算的 30 天以內。

**移至合作夥伴中心之後，我們的專長認證會維持原狀嗎？**

是的，移至合作夥伴中心後，專長認證將不受影響。 如果您發現有不一致的情況，請連絡[支援部門](https://partner.microsoft.com/support)。


 **移動之後，我的權益 (包括雲端權益、技術支援、軟體權益、Visual Studio) 是否會有變更？**

 您的合格權益不會變更。 如果您發現有不一致的情況，請連絡[支援部門](https://partner.microsoft.com/support)。

 **我們具有 Visual Studio 權益配置的 Microsoft 帳戶是否仍將有效？**


 是。 將會接受並保留配置給 MSA 的 Visual Studio 權益。 在合作夥伴中心中續訂之後，也會保留它們。 不過，如果您在移轉至合作夥伴中心後移除 MSA 配置，便無法將其重新新增至合作夥伴中心。

在合作夥伴中心，合作夥伴可以新增公司帳戶及來賓使用者帳戶，其為來自合作夥伴為 Azure AD 租用戶中 MPN 系統管理員之相同租用戶的 MSA。 如果合作夥伴是多個 Azure AD 租用戶中的全域系統管理員，且這些租用戶都是與相同的合作夥伴中心帳戶相關聯，則該合作夥伴便可以將所有這些租用戶上的使用者加入 Visual Studio 權益和 Azure 以使用量為基礎的配置。

雖然 MPN 系統管理員或全域系統管理員可以將 Visual Studio 以使用量為基礎的訂用帳戶指派給來賓使用者，來賓使用者並無法使用其 MSA 登入合作夥伴中心。 不過，來賓使用者可以登入 Azure 和 Visual Studio 以驗證並使用指派給他的權益。


 **我們應如何管理 MCP 關聯和 Partner University 存取權？**

 從 PMC 移動後，MCP 關聯不會有任何變更。 不過，在移至合作夥伴中心後新增的任何新員工，將必須於合作夥伴中心建立關聯。 現有使用者的所有 Partner University 權限將會保留，但任何新員工都應前往[訓練中心](https://partner.microsoft.com/training)了解如何取得 Partner University 的存取權。

 **移至合作夥伴中心後要如何檢視 MCP 資訊？**

在儀表板上的左側導覽中，選取 [專長認證]。 在 [專長認證] 頁面中，您可以下載技能報告。 技能報告會列出您的哪些使用者已取得與合作夥伴中心的專長認證和計畫有關的技能。 如果您的使用者已獲得技能，但這些技能與您所需的專長認證無關，這些使用者就不會列在報告中。


 **合作夥伴中心是否會使用客戶參考？**

 否，要達到合作夥伴中心的專長認證需求，並不需要客戶參考。

 **記錄可查夥伴關聯是否會移至合作夥伴中心？**

 是，記錄可查夥伴不會變更。 請深入了解[將您的合作夥伴識別碼連結至客戶](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。

**移至合作夥伴中心是否會影響到獎勵？**

否，如果您在移動帳戶時並未合併位置，獎勵將不受影響。 如果您的公司在 PMC 中有多個帳戶，且您在移至合作夥伴中心時決定將其合併為通用帳戶，您將不會失去獎勵，但獎勵給付可能會有延遲。 如果您未移動所有與獎勵計畫相關的 PMC 帳戶，就可能不會再獲得與這些帳戶繫結的獎勵。


**合作夥伴中心有哪些獎勵角色？** 

合作夥伴中心的獎勵角色以位置為基礎，且包含獎勵管理員和獎勵使用者。 若要深入了解這些角色可執行哪些工作，請參閱[指派使用者角色和權限](permissions-overview.md)。

**是否可在全域和位置層級指派獎勵管理員？**

 是。 您可以將一個獎勵管理員指派為所有位置的獎勵管理員，或是讓每個位置各有其本身的獎勵管理員。

 **是否可在全域或位置層級給付獎勵？**

 獎勵只會在位置層級給付。

**關於推薦，我們可以建立多少個商務設定檔？**

您的公司可視需要建立數量不限的商務設定檔，以完整展現公司的興趣。 在每個商務設定檔中，您最多可以列出五個位置，每個國家/地區一個位置。 每個商務設定檔分別可接收其對應位置的推薦。

**如何指派推薦，預期會有哪些變更？例如，如果我在某個市場有一個全球性公司，而在其他市場有一些位置，則應如何指派推薦？**

系統會根據客戶定義的搜尋參數來指派推薦。 不論您是有一個還是多個位置，在客戶指定了所需的位置後，如果您有符合其他參數的業務，則會將推薦指派至該位置。








