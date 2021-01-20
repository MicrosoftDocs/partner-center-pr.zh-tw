---
title: 使用多重要素驗證來設定您的使用者
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何使用 MFA 為員工進行設定
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182370"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>使用多重要素驗證來設定您的使用者

**適當的角色**

- 全域系統管理員

較高的隱私權保護和安全性是我們最優先的考量。 我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。 這就是為什麼我們需要生態系統中的每個人都採取行動，並確保具備適當的安全性保護。 我們強烈建議所有合作夥伴在其合作夥伴租用戶中為其使用者啟用多重要素驗證 (MFA)。 

## <a name="add-multi-factor-authentication-for-your-users"></a>為使用者新增多重要素驗證

您必須是公司的全域管理員才能完成這項工作。

若要為使用者啟用 MFA，最簡單的方法是在將使用者新增至 Azure AD 租用戶時進行。

1. 登入 [Azure 入口網站](https://portal.azure.com)，然後移至 [使用者管理]。
1. 選取 [多重要素驗證]。
1. 選取您想要啟用的使用者，然後選取 [啟用]。

這會為這名使用者啟用 MFA。 [已啟用] 表示系統會要求使用者在第一次登入時設定其 MFA 驗證。 之後在登入時，系統就會要求其提供透過電子郵件或簡訊 (視其設定而定) 所收到的驗證碼。  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何驗證":::

>[!NOTE]
>您可以使用上述相同步驟，並選取 [強制執行] 來 **強制** 使用者使用 MFA。 若要深入了解，請閱讀[啟用每一使用者 Azure Multi-Factor Authentication 以保護登入事件](/azure/active-directory/authentication/howto-mfa-userstates)。 

所有使用者都會從 [已停用] **** 開始。 當您以每一使用者 Azure Multi-Factor Authentication 註冊使用者時，其狀態會變更為 [已啟用] **** 。 當已啟用的使用者登入並完成註冊程序時，其狀態會變更為 [強制執行] **** 。 

## <a name="next-steps"></a>後續步驟

- [將角色和權限指派給使用者](permissions-overview.md)