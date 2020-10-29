---
title: 使用多重要素驗證來設定您的使用者
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何使用 MFA 為員工進行設定
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526002"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>使用多重要素驗證來設定您的使用者

**適當的角色**

- 全域系統管理員

較高的隱私權保護和安全性是我們最優先的考量。 我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。 這就是為什麼我們需要生態系統中的每個人都採取行動，並確保具備適當的安全性保護。 為了協助保護合作夥伴和客戶，我們針對參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴推出一組強制性的安全性需求。

合作夥伴都必須針對其合作夥伴租用戶的所有使用者帳戶強制執行多重要素驗證 (MFA)。 

## <a name="add-multi-factor-authentication-for-your-users"></a>為使用者新增多重要素驗證

您必須是公司的全域管理員才能完成這項工作。

若要為使用者啟用 MFA，最簡單的方法是在將使用者新增至 Azure AD 租用戶時進行。

1. 登入 [Azure 入口網站](https://portal.azure.com)，然後移至 [使用者管理]。
1. 選取 [多重要素驗證]。
1. 選取您想要啟用的使用者，然後選取 [啟用]。

這會為這名使用者啟用 MFA。 [已啟用] 表示系統會要求使用者在第一次登入時設定其 MFA 驗證。 之後在登入時，系統就會要求其提供透過電子郵件或簡訊所收到的驗證碼。  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何驗證":::

若要強制使用者使用 MFA，您可以使用上述相同步驟，並選取 [強制執行] 來 **強制執行** 。 請深入了解，閱讀[啟用每一使用者 Azure Multi-Factor Authentication 以保護登入事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)。 

所有使用者都會從 [已停用] **** 開始。 當您以每一使用者 Azure Multi-Factor Authentication 註冊使用者時，其狀態會變更為 [已啟用] **** 。 當已啟用的使用者登入並完成註冊程序時，其狀態會變更為 [強制執行] **** 。 

## <a name="next-steps"></a>後續步驟

- [將角色和權限指派給使用者](permissions-overview.md)



