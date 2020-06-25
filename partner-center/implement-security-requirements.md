---
title: 實作合作夥伴安全性需求
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何為您的使用者實作必要的安全性需求
author: LauraBrenner
ms.author: labrenne
keywords: 安全性
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133261"
---
# <a name="implement-the-partner-security-requirements"></a>實作合作夥伴安全性需求

**適當的角色**

- 全域系統管理員

確保客戶及合作夥伴的安全性和隱私權是 Microsoft 最為優先的工作。 我們持續看到更多更為複雜的安全性攻擊，這些攻擊主要與身分識別遭到入侵有關。 由於預防性控制項在對抗安全性攻擊的整體防禦策略中扮演重要角色，我們將會開始強制執行一組強制的安全性需求，以協助保護合作夥伴與其客戶。

在本教學課程中，您將深入了解合作夥伴的安全性需求、如何滿足這些需求，以及對合作夥伴目錄中的使用者所造成的影響。

所有參與雲端解決方案提供者方案的合作夥伴、控制台廠商和 Advisor 合作夥伴，都必須針對其合作夥伴租用戶中的每位使用者強制執行多重要素驗證 (MFA)。 這項強制執行的驗證可藉由啟用兩個 [Azure Active Directory 基準原則](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)來完成。 基準原則是一組預先定義的原則，可協助組織抵禦許多常見的攻擊。 這些常見的攻擊可能包括密碼噴灑、重播和網路釣魚。 基準保護原則適用於所有版本的 Azure Active Directory。 Microsoft 將這些基準保護原則提供給所有人使用的原因，是因為以身分識別為基礎的攻擊在過去幾年一直持續攀升。

下列程序描述啟用兩個必要基準原則的程序：

- **要求系統管理員使用 MFA**  啟用 [要求系統管理員使用 MFA] 原則時，將要求系統管理員角色中的使用者使用 Authenticator 應用程式來註冊使用 MFA。 完成 MFA 註冊後，管理員每次登入時都必須執行 MFA。

- **使用者保護**  使用者保護是以風險為基礎的 MFA 基準原則，可保護目錄中的所有使用者。 啟用此原則會要求所有使用者都必須使用驗證器應用程式註冊 MFA。 使用者可以略過 MFA 註冊提示 14 天，在這之後，他們將會遭到封鎖而無法登入，直到他們註冊 MFA 為止。 註冊 MFA 之後，只有在有風險的登入嘗試時，才會提示使用者進行 MFA。 遭盜用的使用者帳戶會遭到封鎖，直到重設其密碼且風險事件已解除為止。

啟用這些原則之後，每個使用者都能夠利用 Azure MFA 來進行驗證，而不需要額外付費。 如果您使用第三方解決方案，則在存取 Microsoft 商業雲端服務時，您必須為每位使用者強制執行 MFA。

>[!NOTE]
>由於會針對合作夥伴目錄中的每個使用者強制執行 MFA，因此會影響任何利用使用者認證的自動化或整合作業。 若要解決這種影響，您必須修改自動化或整合連線到 Microsoft 商業雲端服務的方式。 如果您要連線的服務支援以權杖為基礎的驗證，則建議您實作[安全的應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>步驟一：封鎖任何現有的舊版驗證通訊協定

在您啟用要求系統管理員使用 MFA 和使用者保護原則之前，請確定您的使用者未使用舊版驗證通訊協定。 請參閱[如何：使用條件式存取封鎖 Azure AD 的舊版驗證](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)，以取得詳細資訊。

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>步驟二：要求系統管理員使用 MFA 基準原則

要求管理員使用 MFA 基準原則需要下列目錄角色的 MFA，被視為最具特殊權限的 Azure AD 角色：

- 全域管理員
- SharePoint 管理員
- Exchange 系統管理員
- 條件式存取管理員
- 安全性系統管理員
- 服務台管理員/密碼管理員
- 計費管理員
- 使用者管理員

啟用 [要求系統管理員使用 MFA] 原則時，需要以上九個系統管理員角色，才能使用 Authenticator 應用程式來註冊使用 MFA。 完成 MFA 註冊後，管理員每次登入時都必須執行 MFA。

如果您的組織在指令碼或程式碼中使用這些帳戶，請考慮將它們取代為 [受管理的身分識別](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。

若要啟用此原則並保護您的系統管理員：

1. 以全域管理員、安全性系統管理員或條件式存取系統管理員的身分登入  **Azure 入口網站** 。

2. 瀏覽至 [Azure Active Directory] >  [條件式存取]。

3. 在原則清單中，選取 [基準原則:要求系統管理員使用 MFA]。

4. 將 [啟用原則] 設定為 [立即使用原則]。

5. 選取 [儲存] **** 。

當您啟用此原則之後，系統會在上述系統管理員角色的使用者登入時提示，提供額外的安全性資訊並設定行動應用程式。 完成之後，他們就能夠登入適當的雲端服務。

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>步驟三：啟用使用者保護基準原則

使用者保護基準原則會保護目錄中的所有使用者。 啟用此原則會要求所有使用者都必須在 14 天內註冊 Azure MFA。 註冊之後，只有在有風險的登入嘗試時間，才會提示使用者進行 MFA，合作夥伴租用戶的此種行為未來將會改變。 遭盜用的使用者帳戶會遭到封鎖，直到重設密碼和風險解除為止。

原則 [基準原則：使用者保護] 已預先設定，當您瀏覽至 Azure 入口網站中的 [條件式存取] 刀鋒視窗時，將顯示在頂端。

若要啟用此原則並保護您的使用者：

1. 以全域管理員、安全性系統管理員或條件式存取系統管理員的身分登入  **Azure 入口網站** 。

2. 瀏覽至 [Azure Active Directory] >  [條件式存取]。

3. 在原則清單中，選取 [基準原則:終端使用者保護 (預覽)]。

4. 將 [啟用原則] 設定為 [立即使用原則]。

5. 選取 [儲存] **** 。

當您啟用此原則之後，系統會在所有使用者登入時提示，提供額外的安全性資訊並設定行動應用程式。 完成之後，他們就能夠登入適當的雲端服務。

>[!NOTE]
>在強制執行合作夥伴安全性需求之前，系統只會根據風險提示不受 [要求系統管理員使用 MFA] 基準原則限制的使用者進行 MFA。