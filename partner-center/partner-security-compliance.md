---
title: 合作夥伴安全性需求狀態 | 合作夥伴中心
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入了解在雲端解決方案提供者計畫中，針對顧問、控制台廠商和合作夥伴增加安全性的新強制需求。
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, 雲端解決方案提供者, 雲端解決方案提供者計畫, CSP, 控制台廠商, CPV, 多重要素驗證, MFA, 安全應用程式模型, 安全應用程式模型, 安全性
ms.localizationpriority: high
ms.openlocfilehash: 7e8226009e9f214e420475dbd350f2bcb3984414
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943111"
---
# <a name="partner-security-requirements-status"></a>合作夥伴安全性需求狀態

**適用於**

- 雲端解決方案提供者計畫中的所有合作夥伴
  - 直接帳單
  - 間接提供者
  - 間接轉銷商
- 所有控制台廠商
- 所有顧問

較高的隱私權保護和安全性是我們最優先的考量。 我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。 這就是為什麼我們需要生態系統中的每個人都採取行動，並確保其具備適當的安全性保護。 為了協助保護合作夥伴和客戶，我們針對參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴推出一組強制性的安全性需求。

自 2019 年 8 月 1 日起，所有合作夥伴都必須針對其合作夥伴租用戶的所有使用者 (包括服務帳戶) 強制執行多重要素驗證。 如需新安全性原則的詳細資訊，請參閱[合作夥伴安全性需求](partner-security-requirements.md)。

我們想要確保每個使用者都有每個單一驗證的 MFA 挑戰。 您可以透過下列其中一種方式來完成這項作業：

- 實作 Azure AD Premium 以確保對每個使用者強制執行 MFA
- 實作 [Azure AD 安全性預設值](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- 實作第三方解決方案，以確保對每個使用者強制執行 MFA

## <a name="partner-security-requirements-status"></a>合作夥伴安全性需求狀態

這份報告藉由提供一種方法來查看您可能會落後的地方，協助您確認安全性需求狀態。 追蹤會定期更新。

>[!NOTE]
>只有在合作夥伴中心才支援合作夥伴安全性需求狀態報告。 不適用於 Microsoft Cloud for US Government 或 Microsoft Cloud Germany。 我們強烈建議所有合作夥伴透過主權雲端 (21Vianet、US Government 和 Germany) 進行交易，並立即採取這些新的安全性需求。 不過，這些合作夥伴不需要符合 2019 年 8 月 1 日生效的新安全性需求。 Microsoft 未來將針對主權雲端的這些安全性需求強制執行，提供額外的詳細資料。

每次您的員工登入合作夥伴中心，或透過 API、透過合作夥伴中心取得或傳送資料時，其安全性狀態會受到挑戰和追蹤。 也包含在安全性狀態追蹤中的，是您的應用程式和任何控制台廠商應用程式。 顯示的是過去 7 天的狀態。

## <a name="multi-factor-authentication-mfa-report"></a>多重要素驗證 ("MFA") 報告

合作夥伴中心 MFA 報告藉由提供兩個以合作夥伴中心活動為基礎的計量，提供合作夥伴 MFA 實作的深入解析：

**使用者完成的 MFA 驗證**

此計量與合作夥伴中心儀表板中的活動有關。 它會測量已完成 MFA 驗證的使用者所做的作業百分比。 例如：

- Contoso 是 CSP 合作夥伴，有兩位管理員代理人：Jane 和 John。
- 在第一天，Jane 登入合作夥伴中心儀表板而未進行 MFA 驗證，並進行 3 個作業。
- 在第二天，John 登入合作夥伴中心儀表板而未進行 MFA 驗證，並進行 5 個作業。
- 在第三天，Jane 以 MFA 驗證登入合作夥伴中心儀表板，並進行 2 個作業。
- 這兩位代理人在剩餘的 4 天內都沒有執行任何作業。
- 在 7 天時間範圍內的 10 個作業中，2 個是由具有 MFA 驗證的使用者所進行。 因此，計量會顯示 20%。

**應用程式 + 使用者驗證**

此計量與使用應用程式 + 使用者驗證所建立的合作夥伴中心 API 要求有關。 它會測量使用具有 MFA 宣告的存取權杖所建立 API 要求的百分比。 例如：

- Fabrikam 是 CSP 合作夥伴，而且有一個 CSP 應用程式使用混合的應用程式 + 使用者驗證和僅使用應用程式驗證方法。
- 在第一天，應用程式提出 3 個 API 要求，由透過應用程式 + 使用者驗證方法取得的存取權杖所支援，未進行 MFA 驗證。
- 在第二天，應用程式提出 5 個 API 要求，而這些要求是由使用僅使用應用程式驗證取得的存取權杖所支援。
- 在第三天，應用程式提出 2 個 API 要求，由使用應用程式 + 使用者驗證方法搭配 MFA 驗證取得的存取權杖所支援。
- 這兩位代理人在剩餘的 4 天內都沒有執行任何作業。
- 第二天的 5 個 API 要求是由透過僅使用應用程式驗證取得的存取權杖所支援，因為它不會使用使用者認證，所以會在計量中省略。 剩餘的 5 個作業中，有 2 個是由透過 MFA 驗證取得的存取權杖所支援。 因此，計量會顯示 40%。

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>如果 MFA 報告下的計量不是 100%，我該怎麼做

如果合作夥伴已實作 MFA，則合作夥伴中心 MFA 報告底下的計量有可能不是 100%。 若要了解原因，以下是一些要考慮的因素。

> [!NOTE]
> 您需要與組織中的某人合作，該名人員熟悉您合作夥伴租用戶的身分識別管理和 MFA 實作。

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>您是否已為您的合作夥伴租用戶實作 MFA？

如果不是，您必須先為您的合作夥伴租用戶實作 MFA。 如需如何實作 MFA 的詳細資訊，請參閱[合作夥伴安全性需求](partner-security-requirements.md)文章。

### <a name="have-you-only-recently-completed-mfa-implementation"></a>您是否只在最近完成 MFA 實作？

計量會每日計算，並將過去 7 天內執行的作業列入計算。 如果您只在最近完成合作夥伴租用戶的 MFA 實作，計量可能不是 100%。

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>某些使用者帳戶是否已從 MFA 實作中排除？

了解您目前的 MFA 實作是否涵蓋所有使用者帳戶，或只涵蓋部分。 某些 MFA 解決方案是原則式，可支援使用者排除，而其他解決方案則可能需要您針對每個使用者明確啟用 MFA。 確認您未從目前的 MFA 實作中排除任何使用者。 遭到排除的使用者帳戶若登入合作夥伴中心以執行任何 CSP 相關活動，會造成計量不是 100%。

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>是否只有在符合特定條件時才需要 MFA？

了解目前的實作是否只在特定條件下才強制執行 MFA。 某些 MFA 解決方案提供彈性，只在符合特定條件時才強制執行 MFA。 例如，使用者從未知的裝置或不明的位置進行存取。 已啟用 MFA 但是在存取合作夥伴中心時不需要完成 MFA 驗證的使用者，可能會導致計量不是 100%。

>[!NOTE]
>對於已使用 Azure AD 安全性預設值來實作 MFA 的合作夥伴，請務必注意，若沒有系統管理員使用者帳戶，則會根據風險強制執行多重要素驗證。 使用者只有在進行有風險的登入嘗試 (例如，使用者從其他位置登入) 時，才會收到要進行 MFA 的提示。 此外，使用者最多有 14 天的時間來註冊 MFA。 未完成 MFA 註冊的使用者在 14 天的期間內，不會經過 MFA 驗證的查問。 因此，使用 Azure AD 安全性預設值來實作 MFA 的合作夥伴，計量可能不會是 100%。

### <a name="are-you-using-3rd-party-mfa-solution"></a>您是否使用第三方 MFA 解決方案？

如果您使用第三方 MFA 解決方案，請識別您要將它與 Azure AD 整合的方式。 一般來說有兩種方法，包括同盟和自訂控制項：

* **身分識別同盟**  - 當 Azure AD 收到驗證要求時，Azure AD 會將使用者重新導向至同盟識別提供者進行驗證。 驗證成功之後，同盟識別提供者會連同 SAML 權杖，將使用者重新導向回 Azure AD。 為了讓 Azure AD 在向同盟識別提供者進行驗證時，辨識使用者已完成 MFA 驗證，SAML 權杖必須包含authenticationmethodsreferences  宣告 (具有 multipleauthn  值)。 檢查同盟識別提供者是否支援發出這類宣告。 若是如此，請檢查同盟識別提供者是否已設定為執行此動作。 如果宣告遺失，Azure AD (進而是合作夥伴中心) 將不會知道使用者已完成 MFA 驗證，而這會造成計量不是 100%。

* **自訂控制項** - Azure AD 自訂控制項不能用來識別使用者是否已透過協力廠商 MFA 解決方案完成 MFA 驗證。 因此，透過自訂控制項完成 MFA 驗證的任何使用者，一律會對 Azure AD (接著是合作夥伴中心) 顯示未完成 MFA 驗證。 可能的話，建議您在與 Azure AD 整合時，切換為使用身分識別同盟，而不是自訂控制項。

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>識別哪些使用者已登入合作夥伴中心但未進行 MFA

識別哪些使用者已登入合作夥伴中心但未進行 MFA 驗證，並根據您目前的 MFA 實作進行驗證，可能很有幫助。 您可以使用 [Azure AD 登入報告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)知道使用者是否已完成 MFA 驗證。 Azure AD 登入報告目前僅適用於已訂閱 Azure AD Premium 的合作夥伴，或包含 Azure AD Premium (例如 EMS) 的任何 O365 SKU。

**詳細資訊**

- [合作夥伴中心安全性指引群組社群](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [合作夥伴中心安全性需求](partner-security-requirements.md)
- [合作夥伴中心安全性需求常見問題](partner-security-requirements-faq.md)
