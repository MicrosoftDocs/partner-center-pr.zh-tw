---
title: 對您的合作夥伴租使用者強制 MFA |合作夥伴中心
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何為您的合作夥伴租使用者強制 MFA，以協助保護您對客戶資源的存取。 包含範例案例。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 雲端解決方案提供者, 雲端解決方案提供者計畫, CSP, 控制台廠商, CPV, 多重要素驗證, MFA, 安全應用程式模型, 安全應用程式模型, 安全性
ms.localizationpriority: medium
ms.openlocfilehash: f0beb695bee9a67f79373ea903158de3fbb66851
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943101"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>對您的合作夥伴租使用者強制多重要素驗證（MFA）

**適用於**

- 雲端解決方案提供者計畫中的所有合作夥伴
  - 直接帳單
  - 間接提供者
  - 間接經銷商
- 所有顧問

這些合作夥伴將需要完成下欄區域的 MFA 驗證：

- [合作夥伴中心儀表板](#partner-center-dashboard)（目標為 H1 CY2020）
- [合作夥伴中心 API](#partner-center-api) （目標為 H1 CY2020）
- [合作夥伴委派管理](#partner-delegated-administration)（自2019年11月18日起）

這項功能的目的是協助合作夥伴保護其對客戶資源的存取，以防止認證洩漏。

## <a name="partner-center-dashboard"></a>合作夥伴中心儀表板
[合作夥伴中心] 儀表板中的某些頁面會受到 MFA 保護，包括：

* [**客戶**] 索引標籤下的所有頁面。
* **支援 > [客戶要求**] 索引標籤下的所有頁面。

如果您嘗試存取這些頁面中的任何一頁，但先前尚未完成 MFA 驗證，則需要執行此動作。

下列使用者類型已獲授權存取這些受 MFA 保護的頁面，因而受到這項功能的影響，包括：

* 管理代理程式
* 銷售代理程式
* 技術服務人員代理程式

若要說明其運作方式，請考慮下列兩個範例。

**範例1：合作夥伴已實行 Azure AD MFA**
1.  Jane 適用于 CSP Contoso。 Contoso 已使用 Azure AD MFA，為 Contoso 合作夥伴租使用者下的所有使用者執行 MFA。
2.  在她的工作站中，Jane 開始新的瀏覽器會話，並導覽至合作夥伴中心儀表板的 [總覽] 頁面（不受 MFA 保護）。 合作夥伴中心會將 Jane 重新導向至 Azure AD 以進行登入。
3.  由於 Contoso 的現有 Azure AD MFA 設定，因此需要 Jane 完成 MFA 驗證。 成功登入和 MFA 驗證後，Jane 會重新導向回到合作夥伴中心儀表板的 [總覽] 頁面。
4.  Jane 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 Jane 在稍早的登入期間已經完成 MFA 驗證，因此 Jane 可以存取受 MFA 保護的頁面，而不需要再次進行 MFA 驗證。

**範例2：合作夥伴已使用身分識別同盟來執行協力廠商 MFA**
1. Trent 適用于 CSP Wingtip。 Wingtip 已使用協力廠商 MFA （透過身分識別同盟與 Azure AD 整合），為其下的所有使用者執行 MFA。
2. Trent 會從他的工作站開始新的瀏覽器會話，並導覽至合作夥伴中心儀表板的 [總覽] 頁面（不受 MFA 保護）。 合作夥伴中心會將 Justin 重新導向至 Azure AD 以進行登入。
3. 由於 Wingtip 已設定身分識別同盟，Azure AD 會將 Trent 重新導向至同盟身分識別提供者，以完成登入和 MFA 驗證。 成功登入和 MFA 驗證之後，Trent 會重新導向回到 Azure AD，然後到合作夥伴中心儀表板的 [總覽] 頁面。
4. Justin 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 Trent 在先前的登入期間已完成 MFA 驗證，Trent 可以存取受 MFA 保護的頁面，而不需要再次進行 MFA 驗證。

**範例3：合作夥伴尚未實作為 MFA**
1. John 適用于 CSP Fabrikam。 Fabrikam 尚未為 Fabrikam 合作夥伴租使用者下的任何使用者實作為 MFA。
2. John 會從工作站開始新的瀏覽器會話，並導覽至合作夥伴中心儀表板的 [總覽] 頁面（這不是受 MFA 保護）。 合作夥伴中心會將 John 重新導向至 Azure AD 以進行登入。
3. 因為 Fabrikam 尚未實行 MFA，所以不需要 John 來完成 MFA 驗證。 成功登入時，John 會重新導向回到合作夥伴中心儀表板的 [總覽] 頁面。
4. John 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 John 尚未完成 MFA 驗證，合作夥伴中心會將 John 重新導向至 Azure AD 以完成 MFA 驗證。 因為這是您第一次需要 John 來完成 MFA，所以 John 也會要求您使用 Microsoft Authenticator 應用程式註冊 MFA。 成功註冊 MFA 後，John 現在可以存取受 MFA 保護的頁面。

## <a name="partner-center-api"></a>合作夥伴中心 API

合作夥伴中心 API 支援僅限應用程式的驗證和應用程式 + 使用者驗證。 使用 [應用程式 + 使用者驗證] 時，合作夥伴中心會需要 MFA 驗證。 更明確地說，當合作夥伴應用程式想要將 API 要求傳送至合作夥伴中心時，它必須在要求的 Authorization 標頭中包含存取權杖。 當合作夥伴中心收到 API 要求，並使用應用程式 + 使用者驗證取得的存取權杖時，合作夥伴中心 API 將會在*驗證方法參考（AMR）* 宣告中檢查*MFA*值是否存在。 您可以使用 JWT 解碼器來驗證存取權杖是否包含預期的驗證方法參考（AMR）值：

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

如果值存在，合作夥伴中心會結束 MFA 驗證完成，並處理 API 要求。 如果值不存在，合作夥伴中心 API 將會拒絕具有下列回應的要求：

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>合作夥伴委派的系統管理

### <a name="using-service-portals"></a>使用服務入口網站

合作夥伴帳戶（包括管理員代理程式和技術服務人員代理程式）可以使用其合作夥伴委派的系統管理員許可權，透過 Microsoft Online Services 入口網站、命令列介面（CLI）和 Api （使用應用程式 + 使用者驗證）來管理客戶資源。

使用合作夥伴委派的系統管理員許可權來管理客戶資源時，若要存取 Microsoft Online Services 入口網站，其中有許多入口網站會要求合作夥伴帳戶以互動方式進行驗證，並將客戶 Azure Active Directory 租使用者設定為驗證內容-需要合作夥伴帳戶才能登入客戶租使用者。

當 Azure Active Directory 收到這類驗證要求時，會要求合作夥伴帳戶完成 MFA 驗證。 有兩種可能的使用者體驗，視合作夥伴帳戶是受控或同盟身分識別而定：

- 如果合作夥伴帳戶是**受控**識別，Azure Active Directory 會直接提示使用者完成 MFA 驗證。 如果合作夥伴帳戶尚未向 Azure Active Directory 註冊 MFA，則會要求使用者先[完成 mfa 註冊](#mfa-registration-experience)。

- 如果夥伴**帳戶是同盟身分識別，** 則此體驗取決於夥伴管理員如何在 Azure Active Directory 中設定同盟。 在 Azure Active Directory 中設定同盟時，合作夥伴系統管理員可以指出是否要 Azure Active Directory 聯盟識別提供者是否支援 MFA。 若是如此，Azure Active Directory 會將使用者重新導向至同盟身分識別提供者，以完成 MFA 驗證。 否則，Azure Active Directory 會直接提示使用者完成 MFA 驗證。 如果合作夥伴帳戶尚未向 Azure Active Directory 註冊 MFA，則會要求使用者先[完成 mfa 註冊](#mfa-registration-experience)。

整體體驗非常類似于終端客戶租使用者為其系統管理員實作為 MFA 的案例。 例如，客戶租使用者已啟用[Azure AD 的基準原則-適用于系統管理員的 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，這需要具有系統管理許可權的所有帳戶，才能使用 MFA 驗證（包括管理員代理程式和技術服務人員代理程式）來登入客戶租使用者。 基於測試目的，合作夥伴可以在客戶租使用者中啟用 [系統[管理員的 MFA] 原則](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，然後嘗試使用合作夥伴委派的系統管理許可權來存取客戶租使用者。

> [!NOTE]
> 並非所有的 Microsoft 線上服務入口網站都需要合作夥伴帳戶，才能在使用合作夥伴委派的系統管理員許可權存取客戶資源時，登入客戶租使用者。 相反地，他們只需要合作夥伴帳戶來登入合作夥伴租使用者。 例如 Exchange 系統管理中心。 經過一段時間，我們預期這些入口網站會要求合作夥伴帳戶在使用合作夥伴委派的系統管理員許可權時，登入客戶租使用者。

### <a name="using-service-apis"></a>使用服務 Api
某些 Microsoft Online Services Api （例如 Azure Resource Manager、Azure AD Graph、Microsoft Graph 等等）支援使用合作夥伴委派系統管理員許可權的合作夥伴，以程式設計方式管理客戶資源。 若要利用這些 Api 來使用合作夥伴委派的系統管理員許可權，合作夥伴應用程式必須在 API 要求授權標頭中包含存取權杖，其中存取權杖的取得方式是讓合作夥伴使用者帳戶向 Azure AD 進行驗證，並使用客戶 Azure AD 設定為驗證內容。 合作夥伴應用程式必須要有合作夥伴使用者帳戶，才能登入客戶租使用者。

當 Azure AD 收到例如驗證要求時，Azure AD 會要求合作夥伴使用者帳戶完成 MFA 驗證。 如果合作夥伴使用者帳戶之前尚未註冊 MFA，則會提示使用者帳戶先完成 MFA 註冊。

使用合作夥伴委派的系統管理員許可權與這些 Api 整合的所有合作夥伴應用程式，都會受到這項功能的影響。 若要確保合作夥伴應用程式可以繼續使用這些 Api，而不會中斷：

- 合作夥伴必須避免搭配 Azure AD 使用非互動式使用者驗證方法來取得存取權杖。 使用非互動式使用者驗證方法（例如[密碼流程](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)）時，Azure AD 將無法提示使用者完成 MFA 驗證。 合作夥伴必須改用互動式使用者驗證方法（例如[OpenID connect 流程](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code)）切換為使用。
- 在互動式使用者驗證方法期間，合作夥伴應使用已啟用 MFA 的合作夥伴使用者帳戶。 或者，當 Azure AD 出現提示時，合作夥伴可以在登入期間完成 MFA 註冊和 MFA 驗證。
- 這非常類似于終端客戶租使用者為其系統管理員實作為 MFA 的案例。 例如，客戶租使用者已啟用[Azure AD 的基準原則-適用于系統管理員的 MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，這需要具有系統管理許可權的所有使用者帳戶，才能使用 MFA 驗證來登入客戶租使用者，包括系統管理員代理程式和技術服務人員代理程式。 基於測試目的，合作夥伴可以在客戶租使用者中啟用 [系統[管理員的 MFA] 原則](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)，然後嘗試使用合作夥伴委派的系統管理許可權，以程式設計方式存取客戶租使用者。

### <a name="mfa-registration-experience"></a>MFA 註冊體驗
在 MFA 驗證期間，如果合作夥伴帳戶之前尚未註冊 MFA，Azure AD 會先提示使用者完成 MFA 註冊：

![MFA 註冊步驟1](images/MfaRegistration1.png)

按一下 **[下一步]** 之後，系統會要求使用者從驗證方法清單中進行選擇（包括電話、SMS 和驗證器應用程式）。

![MFA 註冊步驟2](images/MfaRegistration2.png)

註冊成功後，使用者就必須根據使用者所選擇的驗證來完成 MFA 驗證。



## <a name="request-for-technical-exception"></a>技術例外狀況的要求

如果技術例外狀況遇到 Microsoft Online Services 的技術問題，而且沒有可行的解決方案或因應措施，則合作夥伴可以將其視為不使用 MFA 驗證。 執行此動作之前，請先參閱下列各節：

 - [合作夥伴所報告的常見問題清單](#list-of-common-issues-reported-by-partners)
 - [如何提交技術例外狀況的要求](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>合作夥伴所報告的常見問題清單
在套用技術例外狀況之前，請先參閱其他合作夥伴回報的常見問題清單，以瞭解這些問題是否為技術例外狀況的有效原因。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>問題1：合作夥伴需要更多時間來為其合作夥伴代理程式執行 MFA
夥伴尚未開始，或仍在為需要使用合作夥伴委派的系統管理許可權來管理客戶資源的合作夥伴代理程式，為其建立 MFA 的流程。 合作夥伴需要更多時間來完成 MFA 實施。 這是技術例外狀況的有效原因嗎？

**答**：否。 合作夥伴必須規劃為其使用者執行 MFA，以避免中斷。

> [!NOTE]
> 即使合作夥伴尚未對其夥伴代理程式執行 MFA，合作夥伴代理程式仍然可以使用合作夥伴委派的系統管理許可權來存取 Microsoft Online Services 入口網站，前提是他們可以完成 MFA 註冊和 MFA 驗證在登入客戶租使用者期間出現提示。 完成 MFA 註冊並不會自動啟用 MFA 的使用者。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>問題2：合作夥伴尚未為不是使用委派系統管理員許可權的使用者帳戶執行 MFA
合作夥伴在其合作夥伴租使用者中有一些使用者不需要存取 Microsoft Online Services 入口網站，即可使用合作夥伴委派的系統管理許可權來管理客戶資源。 合作夥伴正進行為這些使用者執行 MFA 的程式，而且需要更多時間才能完成。 這是技術例外狀況的有效原因嗎？

**答**：否。 由於這些使用者帳戶不會使用合作夥伴委派的系統管理許可權來管理客戶資源，因此不需要登入客戶租使用者。 Azure AD 在登入客戶租使用者期間需要進行 MFA 驗證，則不會受到影響。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>問題3：合作夥伴尚未為使用者服務帳戶執行 MFA
合作夥伴在其合作夥伴租使用者中有一些使用者帳戶，而裝置會將其當做服務帳戶使用。 這些通常是低許可權的帳戶，不需要存取合作夥伴中心或 Microsoft 線上服務入口網站，就能使用合作夥伴委派的系統管理許可權來管理客戶資源。 這是技術例外狀況的有效原因嗎？

**答**：否。 由於這些使用者帳戶不會使用合作夥伴委派的系統管理許可權來管理客戶資源，因此不需要登入客戶租使用者。 Azure AD 在登入客戶租使用者期間需要進行 MFA 驗證，則不會受到影響。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>問題4：合作夥伴無法使用 MS 驗證器應用程式來執行 MFA
合作夥伴具有「清理桌面」原則，不允許員工將其個人行動裝置帶入其工作區域。 若沒有存取其個人行動裝置，員工就無法安裝 MS 驗證器應用程式，這是 Azure AD 基準原則唯一支援的 MFA 驗證。 這是技術例外狀況的有效原因嗎？

**答**：否，這不是技術例外狀況的有效原因。 合作夥伴應考慮下列替代方案，讓他們的員工在存取合作夥伴中心時仍然可以完成 MFA 驗證：
- 除了 MS 驗證器應用程式之外，Azure AD 基準原則也可以與協力廠商相容的驗證器應用程式搭配使用，這可能是執行 Microsoft Windows 的 Windows 電腦。
- 合作夥伴也可以註冊 Azure AD Premium 或協力廠商 MFA 解決方案（與 Azure AD 相容），這可提供額外的驗證方法。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>問題5：因為使用舊版驗證通訊協定，所以合作夥伴無法執行 MFA
合作夥伴有一些夥伴代理程式仍在使用舊版驗證通訊協定，而這並不與 MFA 相容。 例如，使用者仍在使用以舊版驗證通訊協定為基礎的 Outlook 2010。 啟用這些夥伴代理程式的 MFA 將會中斷舊版驗證通訊協定的使用。

**答**：否，這不是技術例外狀況的有效原因。 強烈建議您使用傳統驗證通訊協定，因為這些通訊協定無法使用 MFA 驗證來保護，而更容易受到認證危害，所以我們鼓勵您從使用舊版驗證通訊協定。 如果不提供使用舊版驗證通訊協定的選項，合作夥伴應考慮註冊 Azure AD Premium，以支援使用應用程式密碼。 應用程式密碼是一次系統產生的密碼，通常比人類產生的密碼更強。 藉由使用應用程式密碼，合作夥伴可以為其使用者執行 MFA，同時只會回復至舊版驗證通訊協定的應用程式密碼。

> [!NOTE]
> 即使合作夥伴尚未對其夥伴代理程式執行 MFA，合作夥伴代理程式仍然可以使用合作夥伴委派的系統管理許可權來存取 Microsoft Online Services 入口網站，前提是他們可以完成 MFA 註冊和 MFA 驗證在登入客戶租使用者期間出現提示。 完成 MFA 註冊並不會自動啟用 MFA 的使用者。

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>問題6：合作夥伴使用的 Exchange Online PowerShell 不支援 MFA
合作夥伴使用具有合作夥伴委派系統管理許可權的 Exchange Online PowerShell，來代表其客戶管理 Exchange Online 服務。 Exchange Online PowerShell 不支援 MFA。 如果合作夥伴為其使用者執行 MFA，這些使用者將無法再存取 Exchange Online PowerShell。 這是技術例外狀況的有效原因嗎？

**答**：是，這可能會被視為技術例外狀況的有效原因。 [支援夥伴委派系統管理的現有 Exchange Online PowerShell 模組](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)不需要合作夥伴使用者登入客戶租使用者，因此不會受到 AZURE AD 需要 MFA 驗證的影響。 不過，它與 MFA 不相容。 Microsoft Exchange Online 小組正在開發新的 PowerShell 模組，同時支援夥伴委派的系統管理許可權和 MFA。 在提供新的 PowerShell 模組之前，合作夥伴無法為需要使用現有 PowerShell 模組的使用者執行 MFA。 如果這些使用者 Azure AD 因為在跨租使用者登入期間需要進行 MFA 驗證而遇到存取其他 Microsoft Online Services 的困難，合作夥伴可以要求技術例外以隱藏 MFA 驗證。

> [!NOTE]
> 即使合作夥伴無法為需要存取 Exchange Online PowerShell 模組的使用者執行 MFA，這些使用者仍然可以使用提供的合作夥伴委派系統管理許可權來存取 Microsoft 線上服務，以管理客戶資源在登入客戶租使用者期間出現提示時，他們可以完成 MFA 註冊和 MFA 驗證。 完成 MFA 註冊並不會自動啟用 MFA 的使用者，因此不會影響 Exchange Online PowerShell 模組的存取權。

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>問題7：合作夥伴已實行無法辨識的協力廠商 MFA Azure AD
合作夥伴使用協力廠商 MFA 解決方案為其使用者實作為 MFA。 不過，合作夥伴無法正確設定協力廠商 MFA 解決方案，以轉送至 Azure AD 在使用者驗證期間已完成 MFA 驗證。 這是技術例外狀況的有效原因嗎？

**答**：是，這可能會被視為技術例外狀況的有效原因。 提交技術例外狀況的要求之前，請先向協力廠商 MFA 解決方案提供者確認無法將 MFA 解決方案設定為將*authenticationmethodsreferences*宣告（值為*multipleauthn*）傳送到 Azure AD，以指出已在使用者驗證期間完成 mfa 驗證。 提交技術例外狀況的要求時，請提供所使用之協力廠商 MFA 解決方案的詳細資料，並指出整合方法（例如，透過身分識別同盟或使用 Azure AD 自訂控制項）。

### <a name="how-to-submit-a-request-for-technical-exception"></a>如何提交技術例外狀況的要求

若要提交技術例外狀況的要求：

1. 以全域管理員或管理代理程式的身分登入合作夥伴中心。
2. 流覽至 [**支援**] > [**合作夥伴支援要求**]，然後按一下 [**新增要求**]，以建立新的合作夥伴服務要求。
4. 在 [ **MFA 和保護應用程式模型**] 主題底下，select 將**技術例外狀況提交**至問題類型。
6. 提供要求的詳細資料，以提交技術例外狀況的服務要求，然後按一下 [**提交**]。

Microsoft 可能需要最多3個工作天的時間，才能提供對技術例外狀況要求的回應。
