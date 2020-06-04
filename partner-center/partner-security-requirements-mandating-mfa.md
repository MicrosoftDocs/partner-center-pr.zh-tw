---
title: 對合作夥伴租用戶強制使用 MFA
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解對您的合作夥伴租用戶強制使用 MFA 為何有助於保護您對客戶資源的存取。 包含範例案例。
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, 雲端解決方案提供者, 雲端解決方案提供者計畫, CSP, 控制台廠商, CPV, 多重要素驗證, MFA, 安全應用程式模型, 安全應用程式模型, 安全性
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9454e9410e4110fdf3542bde3696d8447d4c90d0
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998304"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>對您的合作夥伴租用戶強制使用多重要素驗證 (MFA)

**適用於**

- 雲端解決方案提供者計畫中的所有合作夥伴
  - 直接帳單
  - 間接提供者
  - 間接轉銷商
- 所有顧問

**受影響的角色**

- 系統管理代理人
- 銷售代理人
- 技術服務代理人
- 計費管理員
- 全域管理員

這項功能的目的是要協助合作夥伴保護其對客戶資源的存取，以防止認證洩漏。
合作夥伴必須針對其合作夥伴租用戶中的所有使用者帳戶 (包括來賓使用者) 強制執行多重要素驗證 (MFA)，這項功能會強制要求這些合作夥伴角色針對下列區域完成 MFA 驗證：

- [合作夥伴中心儀表板](#partner-center-dashboard) (從 2020 年 5 月 1 日開始)
- [合作夥伴中心 API](#partner-center-api) (從 2020 年 5 月 1 日開始)
- [合作夥伴委派的管理](#partner-delegated-administration)

更好且持續的安全性和隱私權保護是我們最優先的考量，而且我們一直在協助合作夥伴保護其客戶和租用戶。 參與「雲端解決方案提供者 (CSP)」計畫、「控制台廠商 (CPV)」和「顧問」的所有合作夥伴，都應該實作[合作夥伴安全性需求](partner-security-requirements.md)才能繼續符合規範。

Microsoft 已開始為合作夥伴租用戶啟用額外的安全性保護。 此一啟用保護的舉措可協助合作夥伴保護其租用戶和客戶，方法是強制使用多重要素驗證 (MFA) 驗證，以防止未經授權的存取。

我們已成功對所有合作夥伴租用戶完成合作夥伴「委派的管理」功能的啟用。 為了進一步協助保護合作夥伴和客戶，自 2020 年 5 月 1 日起，我們將開始在 CSP 中啟用合作夥伴中心交易，協助合作夥伴保護其企業及保護客戶免於遭遇身分識別竊取相關事件。

本文件可為合作夥伴提供有關如何啟用安全性保護的詳細體驗和指導方針。

## <a name="partner-center-dashboard"></a>合作夥伴中心儀表板

合作夥伴中心儀表板中的特定頁面會受到 MFA 保護，包括：

* [客戶] 索引標籤底下的所有頁面，例如可透過下列 URL 來存取的所有頁面： https://partner.microsoft.com/commerce/*
* [支援 > 客戶要求] 索引標籤底下的所有頁面，例如在 https://partner.microsoft.com/dashboard/support/csp/customers/* 底下存取的頁面
* 帳單頁面

如果您未先完成 MFA 驗證即嘗試存取其中任何頁面，您必須執行該驗證。

> [!NOTE]
> 合作夥伴中心上的其他頁面 (例如 [概觀] 頁面、[服務健康情況狀態] 檢查頁面) 將不會受 MFA 保護。

下列使用者類型有權存取這些受 MFA 保護的頁面，因而會受到這項功能的影響


| 受 MFA 保護的頁面       | 系統管理代理人      |  銷售代理人     |   技術服務代理人     | 全域管理員      |  計費管理員     | 
|---    |---    |---    |---    |---    |---    |
| [客戶] 索引標籤下的所有頁面      |   x    |    x   |  x     |       |       |
| [支援 > 客戶要求] 索引標籤底下的所有頁面     | x      |       |    x   |       |       |
| 帳單頁面     |   x    |       |       |    x   |   x    |

**範例**

為了說明驗證的運作方式，請考量以下兩個範例。

**範例 1：合作夥伴已實作 Azure AD MFA**
1.    Jane 任職於 CSP Contoso。 針對使用 Azure Active Directory (Azure AD) MFA 的 Contoso 合作夥伴租用戶，Contoso 為其下的所有使用者實作了 MFA。
2.    Jane 啟動了新的瀏覽器工作階段，並導覽至合作夥伴中心儀表板的 [概觀] 頁面 (未受 MFA 保護)。 合作夥伴中心將 Jane 重新導向至 Azure AD 以進行登入。
3.    基於 Contoso 所設定的現有 Azure AD MFA，Jane 必須完成 MFA 驗證。 成功登入並通過 MFA 驗證後，Jane 重新導向回合作夥伴中心儀表板的 [概觀] 頁面。
4.    Jane 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 Jane 在稍早的登入期間已完成 MFA 驗證，因此 Jane 可存取受 MFA 保護的頁面，而無須再次進行 MFA 驗證。

**範例 2：合作夥伴使用身分識別同盟實作了第三方 MFA**
1. Trent 任職於雲端解決方案提供者 Wingtip。 Wingtip 使用第三方 MFA (透過身分識別同盟與 Azure AD 整合)，為 Wingtip 合作夥伴租用戶下的所有使用者實作了 MFA。
2. Trent 啟動了新的瀏覽器工作階段，並導覽至合作夥伴中心儀表板的 [概觀] 頁面 (未受 MFA 保護)。 合作夥伴中心將 Trent 重新導向至 Azure AD 以進行登入。
3. Wingtip 已設定身分識別同盟，因此 Azure AD 將 Trent 重新導向至同盟身分識別提供者，以完成登入和 MFA 驗證。 成功登入並通過 MFA 驗證後，Trent 重新導向至 Azure AD，然後回到合作夥伴中心儀表板的 [概觀] 頁面。
4. Trent 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 Trent 在稍早的登入期間已完成 MFA 驗證，因此 Trent 可存取受 MFA 保護的頁面，而無須再次進行 MFA 驗證。

**範例 3：合作夥伴未實作 MFA**
1. John 任職於 CSP Fabrikam。 Fabrikam 並未針對 Fabrikam 合作夥伴租用戶下的任何使用者實作 MFA。
2. John 啟動了新的瀏覽器工作階段，並導覽至合作夥伴中心儀表板的 [概觀] 頁面 (未受 MFA 保護)。 合作夥伴中心將 John 重新導向至 Azure AD 以進行登入。
3. Fabrikam 並未實作 MFA，因此 John 不需要完成 MFA 驗證。 成功登入後，John 重新導向回合作夥伴中心儀表板的 [概觀] 頁面。
4. John 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 John 未完成 MFA 驗證，因此合作夥伴中心將 John 重新導向至 Azure AD，以完成 MFA 驗證。 這是系統第一次要求 John 完成 MFA，因此 John 也必須[註冊 MFA](#mfa-registration-experience)。 成功註冊 MFA 後，John 此時即可存取受 MFA 保護的頁面。
5. 改天，在 Fabrikam 為任何使用者實作 MFA 之前，John 啟動新的瀏覽器工作階段，並瀏覽至合作夥伴中心儀表板的 [概觀] 頁面 (不受 MFA 保護)。 合作夥伴中心將 John 重新導向至 Azure AD 以在沒有 MFA 提示的情況下登入。 
6. John 嘗試存取合作夥伴中心內受 MFA 保護的其中一個頁面。 由於 John 未完成 MFA 驗證，因此合作夥伴中心將 John 重新導向至 Azure AD，以完成 MFA 驗證。 因為 John 已註冊 MFA，所以這次只會要求他完成 MFA 驗證。

> [!NOTE]
>動作：公司系統管理員應立即透過合作夥伴中心所建議的任何[選項](partner-security-requirements.md#actions-that-you-need-to-take)來實作 MFA。

## <a name="partner-center-api"></a>合作夥伴中心 API

合作夥伴中心 API 支援僅限應用程式的驗證，以及「應用程式 + 使用者」驗證。 

使用「應用程式 + 使用者」驗證時，合作夥伴中心會要求進行 MFA 驗證。 更明確地說，合作夥伴應用程式需要將 API 要求傳送至合作夥伴中心時，必須在要求的授權標頭中包含存取權杖。 

> [!NOTE]
>[安全應用程式模型](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)是一種安全、可擴縮的架構，可在您呼叫合作夥伴中心 API 時，透過 Microsoft Azure MFA 架構來驗證 CSP 合作夥伴和 CPV，請先實作此模型再於租用戶上啟用 MFA。 

當合作夥伴中心收到 API 要求和使用「應用程式 + 使用者」驗證取得的存取權杖時，合作夥伴中心 API 會檢查*驗證方法參考 (AMR)* 宣告中是否有 *MFA* 值存在。 您可以使用 JWT 解碼器來驗證存取權杖是否包含預期的驗證方法參考 (AMR) 值：

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
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

如果該值存在，合作夥伴中心即會判定 MFA 驗證已完成，並處理 API 要求。 如果該值不存在，合作夥伴中心 API 將會以下列回應拒絕要求：

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

如果使用「僅限應用程式」驗證，支援「僅限應用程式」驗證的 API 將會持續運作，而不會要求 MFA。

## <a name="partner-delegated-administration"></a>合作夥伴委派的管理

### <a name="using-service-portals"></a>使用服務入口網站

合作夥伴帳戶 (包含系統管理代理人和技術服務代理人) 可使用其「合作夥伴委派的管理」權限，透過 Microsoft Online Services 入口網站、命令列介面 (CLI) 和 API (使用「應用程式 + 使用者驗證」) 來管理客戶資源。

使用「合作夥伴委派的管理員」權限 (Admin-On-Behalf-Of) 存取 Microsoft Online Services 入口網站以管理客戶資源時，其中有許多入口網站會要求合作夥伴帳戶以互動方式進行驗證 (將客戶 Azure Active Directory 租用戶設定為驗證內容) - 合作夥伴帳戶必須登入客戶租用戶。

Azure Active Directory 在收到這類驗證要求時，會要求合作夥伴帳戶完成 MFA 驗證。 可能的使用者體驗有兩種，這取決於合作夥伴帳戶是受控識別還是同盟身分識別：

- 如果合作夥伴帳戶是**受控**識別，Azure Active Directory 將會直接提示使用者完成 MFA 驗證。 如果合作夥伴帳戶尚未向 Azure Active Directory 註冊 MFA，則會要求使用者先[完成 MFA 註冊](#mfa-registration-experience)。

- 如果合作夥伴帳戶是**同盟**身分識別，則此體驗將取決於合作夥伴管理員在 Azure Active Directory 中設定同盟的方式。 在 Azure Active Directory 中設定同盟時，合作夥伴管理員可向 Azure Active Directory 指出同盟身分識別提供者是否支援 MFA。 若支援，Azure Active Directory 會將使用者重新導向至同盟身分識別提供者，以完成 MFA 驗證。 若不支援，則 Azure Active Directory 會直接提示使用者完成 MFA 驗證。 如果合作夥伴帳戶尚未向 Azure Active Directory 註冊 MFA，則會要求使用者先[完成 MFA 註冊](#mfa-registration-experience)。

其整體的體驗類似於客戶租用戶已為其管理員實作了 MFA 的案例。 例如，客戶租用戶會啟用 [Azure AD 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，此時，所有具有系統管理權限的帳戶都必須使用 MFA 驗證登入客戶租用戶，包括系統管理代理人和技術服務代理人。 基於測試目的，合作夥伴可以在客戶租用戶中啟用 [Azure AD 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然後嘗試使用「合作夥伴委派的管理」權限來存取客戶租用戶。

> [!NOTE]
> 合作夥伴帳戶使用「合作夥伴委派的管理」權限存取客戶資源時，並非所有的 Microsoft Online Service 入口網站都會要求這些帳戶登入客戶租用戶。 這些入口網站只會要求合作夥伴帳戶登入合作夥伴租用戶。 Exchange 系統管理中心是其中一例。 一段時間後，我們預期這些入口網站會要求合作夥伴帳戶在使用「合作夥伴委派的管理」權限時登入客戶租用戶。

### <a name="using-service-apis"></a>使用服務 API
某些 Microsoft Online Services API (例如 Azure Resource Manager、Azure AD Graph、Microsoft Graph 等等) 支援合作夥伴使用「合作夥伴委派的管理」權限以程式設計方式管理客戶資源。 若要透過這些 API 來使用「合作夥伴委派的管理」權限，合作夥伴應用程式必須在 API 要求授權標頭中包含存取權杖；其存取權杖的取得方式是讓合作夥伴使用者帳戶向 Azure AD 進行驗證 (將客戶 Azure AD 設定為驗證內容)。 使用合作夥伴應用程式時，合作夥伴使用者帳戶必須登入客戶租用戶。

Azure AD 在收到這類驗證要求時，會要求合作夥伴帳戶完成 MFA 驗證。 如果合作夥伴使用者帳戶尚未註冊 MFA，則會提示使用者帳戶先完成 MFA 註冊。

所有使用「合作夥伴委派的管理」權限與這些 API 整合的合作夥伴應用程式，都會受到這項功能的影響。 若要確保合作夥伴應用程式可繼續使用這些 API 而不會中斷：

- 合作夥伴必須避免向 Azure AD 使用非互動式使用者驗證方法來取得存取權杖。 使用非互動式使用者驗證方法 (例如[密碼流程](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)) 時，Azure AD 將無法提示使用者完成 MFA 驗證。 合作夥伴必須改為使用互動式使用者驗證方法，例如 [OpenID Connect 流程](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code)。
- 採用互動式使用者驗證方法時，合作夥伴應使用已啟用 MFA 的合作夥伴使用者帳戶。 或者，當 Azure AD 顯示提示時，合作夥伴可在登入期間完成 MFA 註冊和 MFA 驗證。
- 其體驗類似於客戶租用戶已為其管理員實作了 MFA 的案例。 例如，客戶租用戶會啟用 [Azure AD 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，此時，所有具有系統管理權限的使用者帳戶都必須使用 MFA 驗證登入客戶租用戶，包括系統管理代理人和技術服務代理人。 基於測試目的，合作夥伴可以在客戶租用戶中啟用 [Azure AD 安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，然後嘗試使用「合作夥伴委派的管理」權限以程式設計方式存取客戶租用戶。

### <a name="mfa-registration-experience"></a>MFA 註冊體驗
在 MFA 驗證期間，如果合作夥伴帳戶尚未註冊 MFA，Azure AD 會提示使用者先完成 MFA 註冊：

![MFA 註冊步驟 1](images/MfaRegistration1.png)

在按 [下一步] 之後，系統會要求使用者從驗證方法清單中進行選擇。

![MFA 註冊步驟 2](images/MfaRegistration2.png)

註冊成功後，使用者必須根據自己選擇的驗證來完成 MFA 驗證。



## <a name="request-for-technical-exception"></a>技術例外狀況的要求

合作夥伴若遇到 Microsoft Online Services 的技術問題，而且沒有可行的解決方案或因應措施，他們可以提出技術例外狀況的要求，以抑制 MFA 驗證。 執行此動作之前，請先檢閱下列各節：

 - [合作夥伴回報的常見問題清單](#list-of-common-issues-reported-by-partners)
 - [如何提交技術例外狀況的要求](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>合作夥伴回報的常見問題清單
在提出技術例外狀況的要求之前，請先檢閱其他合作夥伴回報的常見問題清單，以了解這些問題是否為技術例外狀況的合理原因。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>問題 1：合作夥伴需要更多時間來為其合作夥伴代理人實作 MFA
合作夥伴尚未開始為其需要使用「合作夥伴委派的管理」權限存取 Microsoft Online Services 入口網站以管理客戶資源的合作夥伴代理人實作 MFA，或是仍在進行中。 合作夥伴需要更多時間來完成 MFA 實作。 此問題是否為技術例外狀況的合理原因？

**答**：不可以。 合作夥伴必須擬定為其使用者實作 MFA 的計畫，以避免作業中斷。

> [!NOTE]
> 即使合作夥伴尚未對其合作夥伴代理人執行 MFA，合作夥伴代理人仍可使用「合作夥伴委派的管理」權限存取 Microsoft Online Services 入口網站，只要他們在登入客戶租用戶期間能夠按照提示完成 MFA 註冊和 MFA 驗證即可。 完成 MFA 註冊並不會自動為使用者啟用 MFA。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>問題 2：合作夥伴尚未對未使用「委派的管理」權限的使用者帳戶實作 MFA
合作夥伴在其合作夥伴租用戶中有一些使用者不需要使用「合作夥伴委派的管理」權限存取 Microsoft Online Services 入口網站以管理客戶資源。 合作夥伴正進行為這些使用者實作 MFA 的程序，而需要更多時間才能完成。 此問題是否為技術例外狀況的合理原因？

**答**：不可以。 由於這些使用者帳戶不會使用「合作夥伴委派的管理」權限來管理客戶資源，因此不需要登入客戶租用戶。 在登入客戶租用戶期間，需要 MFA 驗證的 Azure AD 將不會影響到這些帳戶。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>問題 3：合作夥伴尚未對使用者服務帳戶實作 MFA
合作夥伴在其合作夥伴租用戶中有一些使用者帳戶，裝置將其當做服務帳戶使用。 這是低權限的帳戶，不需要使用「合作夥伴委派的管理」權限存取合作夥伴中心或 Microsoft Online Services 入口網站以管理客戶資源。 此問題是否為技術例外狀況的合理原因？

**答**：不可以。 由於這些使用者帳戶不會使用「合作夥伴委派的管理」權限來管理客戶資源，因此不需要登入客戶租用戶。 在登入客戶租用戶期間，需要 MFA 驗證的 Azure AD 將不會影響到這些帳戶。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>問題 4：合作夥伴無法使用 MS 驗證器應用程式來實作 MFA
合作夥伴採行「簡潔桌面」原則，不允許員工將其個人行動裝置帶入工作區域中。 無法存取個人行動裝置，員工就無法安裝 MS 驗證器應用程式，但這是 Azure AD 安全性預設值唯一支援的 MFA 驗證。 此問題是否為技術例外狀況的合理原因？

**答**：否，這不是技術例外狀況的合理原因。 合作夥伴應考慮使用下列替代方案，讓其員工仍可藉由存取合作夥伴中心來完成 MFA 驗證：
- 合作夥伴也可以註冊 Azure AD Premium，或是可提供額外驗證方法的第三方 MFA 解決方案 (與 Azure AD 相容)。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>問題 5：合作夥伴因使用了舊版驗證通訊協定而無法實作 MFA
合作夥伴有一些合作夥伴代理人仍在使用與 MFA 不相容的舊版驗證通訊協定。 例如，有些使用者仍在使用以舊版驗證通訊協定為基礎的 Outlook 2010。 為這些合作夥伴代理人啟用 MFA，將會中斷舊版驗證通訊協定的使用。

**答**：否，這不是技術例外狀況的合理原因。 基於潛在的安全問題，強烈建議合作夥伴不要再使用舊版驗證通訊協定，因為這些通訊協定無法受到 MFA 驗證的保護，且認證洩漏的風險會高出許多。 如果無法不繼續使用舊版驗證通訊協定，合作夥伴應考慮註冊支援使用應用程式密碼的 Azure AD Premium。 應用程式密碼是系統產生的一次性密碼，通常比人類產生的密碼更嚴密。 使用應用程式密碼時，合作夥伴可為其使用者實作 MFA，且舊版驗證通訊協定只會回復至應用程式密碼。

閱讀有關[基本驗證和 Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) 的文章，以了解關於支援 Outlook 舊版驗證的最新計畫，並遵循 [Exchange 小組部落格](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange)來獲取即將推出的新聞。 

> [!NOTE]
> 即使合作夥伴尚未對其合作夥伴代理人執行 MFA，合作夥伴代理人仍可使用「合作夥伴委派的管理」權限存取 Microsoft Online Services 入口網站，只要他們在登入客戶租用戶期間能夠按照提示完成 MFA 註冊和 MFA 驗證即可。 完成 MFA 註冊並不會自動為使用者啟用 MFA。

#### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>問題 6：合作夥伴實作了 Azure AD 無法辨識的第三方 MFA
合作夥伴使用第三方 MFA 解決方案為其使用者實作了 MFA。 不過，合作夥伴無法正確設定第三方 MFA 解決方案，以轉送至已在使用者驗證期間完成 MFA 驗證的 Azure AD。 這是技術例外狀況的合理原因嗎？

**答**：是的，此問題可能會被視為技術例外狀況的合理原因。 在提交技術例外狀況的要求之前，請先向第三方 MFA 解決方案提供者確認無法設定 MFA 解決方案，使其將 *authenticationmethodsreferences* 宣告 (使用 *multipleauthn* 值) 傳送至 Azure AD，以指出已在使用者驗證期間完成 MFA 驗證。 在提交技術例外狀況的要求時，您必須提供所使用第三方 MFA 解決方案的詳細資料，並指出整合方法 (例如透過身分識別同盟或使用 Azure AD 自訂控制)，並在技術例外狀況要求中提供下列資訊來作為支援文件：
* 第三方 MFA 設定。 
* [測試合作夥伴安全性需求](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)的結果，此測試必須由已啟用第三方 MFA 的帳戶來執行。
* 您所使用或打算使用的第三方 MFA 解決方案採購單。


### <a name="how-to-submit-a-request-for-technical-exception"></a>如何提交技術例外狀況的要求

若要提交技術例外狀況的要求：

1. 以全域管理員或系統管理代理人的身分登入合作夥伴中心。
2. 若要建立新的合作夥伴服務要求，請導覽至 [支援] > [合作夥伴支援要求]，然後按一下 [新增要求]。
3. 在搜尋方塊中搜尋 **MFA - 例外狀況要求**；或者，從 [類別] 選取 [CSP]，然後從 [主題] 選取 [帳戶、上架、存取]，然後從 [子主題] 選取 [MFA - 例外狀況要求]，然後選取 [下一步]。
4. 提供提交技術例外狀況的服務要求所需的詳細資料，然後按一下 [提交]。

Microsoft 最多可能需要三個工作天，才能對技術例外狀況的要求提供回應。
