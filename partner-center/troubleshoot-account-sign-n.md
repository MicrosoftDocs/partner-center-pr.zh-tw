---
title: 針對設定合作夥伴中心帳戶或 MPN 續約問題進行疑難排解
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 針對在合作夥伴中心中註冊的問題進行疑難排解
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 403899b73dda09dded582c94cabe4219ef56c568
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000612"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>針對帳戶設定或 MPN 續約問題進行疑難排解

**適用於**

- 合作夥伴中心
 
**適當的角色**

- 全域系統管理員
- MPN 合作夥伴系統管理員 
 
以下是一些針對設定合作夥伴中心帳戶時所發生的常見問題進行疑難排解的建議。

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>如果您要從 Partner Membership Center 進行遷移，而且無法編輯任何公司資訊欄位，會發生什麼事

如果您的公司已經有合作夥伴中心的 (說 CSP 帳戶) –您將會看到一個唯讀畫面，它會顯示您的公司存在於合作夥伴中心中的所有相關資訊。

您無法變更此畫面上的詳細資料。 這是設計的，而不是錯誤。

選取 [ **接受** ] 並 **繼續** 進行。


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>如果 IT 部門已關閉合作夥伴中心的 **註冊**。


您會看到此訊息，是因為已停用病毒使用者，或在 Azure AD 租使用者上停用了病毒註冊。 您 Azure AD 帳戶的全域管理員可以執行下列 PowerShell 命令來啟用所需的功能：

**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

如需詳細資訊，請參閱 [自助式註冊](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>忘記密碼

如果您忘了密碼，請選取登入頁面上的 [ **無法存取您的帳戶？** ] 連結來重設您的密碼，或要求您的全域管理員為您指派新的認證。

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>在 [告訴我們您公司的相關資訊] 畫面上，您會收到「發生錯誤」錯誤

如果您不小心在公司電話號碼中使用特殊字元、空格或國家/地區代碼，則通常會出現此錯誤訊息。 [電話號碼] 欄位中輸入的值最多隻能包含10個字元。


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>您的信用卡購買收到錯誤訊息，指出「您的訂單已遭到拒絕。 請驗證您的資訊」


請一律使用與信用卡相對應的位址，而不是您的法律實體。 此外，請確定郵遞區號正確，並對應至您所使用的位址。

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>您想要從離線付款切換至線上付款條件 

您將需要使用慣用的付款條件來取消原始訂單和重新購買。

若要取消訂單：

1. 選取儀表板中的 [ **成員資格** 供應專案] 索引標籤。

2. 選取 [**取消訂單**]

3. 確認視窗會出現，您必須確認才能取消最初訂單。

## <a name="next-steps"></a>後續步驟

- [管理您的合作夥伴中心帳戶](partner-center-account-setup.md)
- [如何讀取帳單和偵察檔案](read-your-bill.md)