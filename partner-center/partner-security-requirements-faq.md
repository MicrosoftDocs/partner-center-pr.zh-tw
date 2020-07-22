---
title: 合作夥伴安全性需求常見問題集
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 關於合作夥伴安全性需求的常見問題 - 是什麼、合作夥伴應如何實行這些問題，以及如何知道您是否符合這些需求。
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d2656ad80cc66742ee432f3eaecb284da798b1c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434117"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>關於合作夥伴安全性需求的常見問題集

**適當的使用者**

- 所有已啟用的使用者，包括來賓使用者

此文章包含[合作夥伴安全性需求](partner-security-requirements.md)的常見問題集。

## <a name="partner-security-requirements"></a>合作夥伴安全性需求

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>合作夥伴有何安全性需求，及其為何應實作這些需求？

更好且持續的安全性和隱私權保護是我們最優先的考量，而且我們一直在協助合作夥伴保護其客戶和租用戶。 我們持續看到更為複雜且更加頻繁發生的安全性攻擊，這些攻擊主要都與身分識別入侵事件有關。 由於預防性控制在整體防禦策略中扮演了對抗安全性攻擊的重要角色，因此我們已於 2019 年引進[強制的安全性需求](partner-security-requirements.md)。 參與「雲端解決方案提供者 (CSP)」計畫、「控制台廠商」和「顧問」的所有合作夥伴，都應該實作這些需求才能繼續符合規範。

### <a name="what-are-the-key-timelines-and-milestones"></a>有哪些關鍵時程表和里程碑？

與這些安全性需求相關聯的條款會隨附至 2019 年的 Microsoft 合作夥伴合約。 您必須盡快實作這些安全性需求，才能符合參與 CSP 計畫的規範。

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>如果未實作這些合作夥伴安全性需求，會發生什麼情況？

Microsoft 合作夥伴合約會要求您對使用者帳戶強制執行多重要素驗證，並採用安全應用程式模型來與合作夥伴中心 API 互動。 

未遵守這些安全性作法的合作夥伴可能會失去在 CSP 計畫中進行交易，或使用委派系統管理員權限來管理客戶租用戶的能力。

### <a name="does-this-apply-to-all-geographies"></a>這是否適用於所有地理位置？

是。這適用於所有地理位置。 我們強烈建議所有合作夥伴透過主權雲端 (21Vianet、US Government 和 Germany) 進行交易，並立即採取這些新的安全性需求。 不過，這些合作夥伴不需要符合 8 月 1 日生效的新安全性需求。 Microsoft 未來將針對主權雲端的這些安全性需求強制執行，提供額外的詳細資料。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>是否可以要求特別排除某個帳戶？

否。您無法針對強制執行 MFA 的需求排除任何使用者帳戶。 基於合作夥伴所擁有的高度權限，Microsoft 合作夥伴合約會要求針對您合作夥伴租用戶中的每個使用者帳戶強制執行多重要素驗證。

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>如何知道我是否符合合作夥伴的安全性需求？

您必須完成下列步驟

- 您必須符合[合作夥伴安全性需求](https://docs.microsoft.com/partner-center/partner-security-requirements)中所述的所有需求
- 您必須確保合作夥伴租用戶中的所有使用者帳戶都已強制執行多重要素驗證。

為了協助識別您可採取動作的主要區域，我們會提供可透過合作夥伴中心取得的[安全性需求狀態](https://partner.microsoft.com/pcv/security/compliance)報告。

如需狀態報告的詳細資訊，請參閱[合作夥伴安全性需求狀態](https://docs.microsoft.com/partner-center/partner-security-compliance)。

## <a name="required-actions"></a>必要動作

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>我需要採取哪些關鍵動作來符合需求？

雲端解決方案提供者計畫 (直接帳單、間接提供者及間接轉銷商)、顧問及控制台廠商中的所有合作夥伴都必須符合需求。

1. **為所有使用者強制執行 MFA**

    雲端解決方案提供者計畫、顧問及控制台廠商中的所有合作夥伴都必須針對其合作夥伴租用戶中的所有使用者強制執行 MFA。

    其他考量：

    - 間接提供者必須與間接轉銷商合作以上線至合作夥伴中心 (如果他們尚未這麼做)，並鼓勵其轉銷商符合需求。
    - 合作夥伴租用戶中的所有使用者可以透過 Azure AD 安全性預設值免費使用 Azure MFA，但必須搭配驗證器應用程式的唯一驗證方法，此方法支援時間型單次密碼 (TOTP)。
    - 如果需要其他方法 (例如通話或文字簡訊)，[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU 能提供額外的驗證方法。
    - 合作夥伴也可以在存取 Microsoft 商業雲端服務時，針對每個帳戶運用第三方 MFA 解決方案。

2. **採用安全應用程式模型架構**

    已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。 如果未這麼做，則可能會因部署 MFA 而導致中斷。 下列資源能提供採用此模型之方法的相關概觀和指引。

    - [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
    - [合作夥伴中心：安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/) \(英文\)
    - [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/) \(英文\)
    - [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
    - [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) \(英文\)

    如果您使用的是控制台，則請向廠商洽詢有關採用安全應用程式模型架構的事宜。

    控制台廠商必須以控制台廠商的身分針對合作夥伴中心進行[上線](https://docs.microsoft.com/partner-center/enroll-as-cpv)，並立即開始實作此需求。 請參閱[合作夥伴中心：安全應用程式模型架構](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制台廠商必須接受並管理雲端解決方案提供者合作夥伴的同意 (而非認證)，並清除所有現有雲端解決方案提供者合作夥伴的認證。

## <a name="multi-factor-authentication"></a>多重要素驗證

### <a name="what-is-multi-factor-authentication-mfa"></a>什麼是 Multi-Factor Authentication (MFA)？

MFA 是一種安全性機制，可以透過一個以上的必要安全性和驗證程序來驗證個人。 它是透過要求進行下列兩種或更多驗證方法來運作：

- 您知道的資訊 (通常是密碼)
- 您擁有的事物 (不易複製的受信任裝置，例如電話)
- 代表您身分的事物 (生物識別技術)

### <a name="what-is-the-cost-of-enabling-mfa"></a>啟用 MFA 的成本為何？

Microsoft 透過實作 Azure AD 安全性預設值免費提供 MFA。 透過此 MFA 版本提供的唯一驗證選項是驗證器應用程式。 如果需要撥打電話或 SMS 訊息，便必須購買 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) 授權。 或者，您可以運用第三方解決方案來為合作夥伴租用戶中的每個使用者提供 MFA；在此情況下，您必須負責確保 MFA 解決方案已強制執行，且您已符合規範。

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>如果我已經有 MFA 解決方案，需要採取哪些動作？

透過這些安全性需求，合作夥伴租用戶中的使用者在存取 Microsoft 商業雲端服務時，必須使用 MFA 進行驗證。 您可以使用第三方解決方案來滿足這些需求。 Microsoft 已不再針對獨立身分識別提供者提供驗證測試，以確認與 Azure Active Directory 之間的相容性。 若要測試您產品的互通性，請參閱這些[指導方針](https://www.microsoft.com/download/details.aspx?id=56843)。

> [!IMPORTANT]
> 如果您使用第三方解決方案，請務必確認解決方案是否發出包含 MFA 值的驗證方法參考 (AMR) 宣告。 請參閱[測試合作夥伴安全性需求](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)，以取得驗證第三方解決方案如何發出預期宣告的詳細資訊。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>我使用多個合作夥伴租用戶來進行交易。 我是否需要對它們全部實作 MFA？

是。您必須針對與雲端解決方案提供者計畫或顧問計畫相關聯的每個 Azure Active Directory 租用戶強制執行 MFA。 若要購買 Azure Active Directory Premium 授權，則必須為每個 Azure Active Directory 租用戶中的使用者購買授權。

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>我合作夥伴租用戶中的每個使用者帳戶是否都必須強制執行 MFA？

是，每個使用者都必須強制執行 MFA。 不過，如果您是使用 Azure AD 安全性預設值，則不需要採取任何其他動作，因為該功能會針對所有使用者帳戶強制執行 MFA。 啟用安全性預設值是一種免費且簡單的方法，可確保您的使用者帳戶符合 MFA 規範，而不會在強制執行 MFA 時受到影響。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>我是 Microsoft 的直接帳單合作夥伴。 我需要做些什麼？

直接帳單雲端解決方案提供者合作夥伴必須針對其合作夥伴租用戶中的每個使用者強制執行 MFA。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>我是間接轉銷商，且僅透過經銷商進行交易。 我仍然需要這麼做嗎？

所有間接轉銷商都必須針對其合作夥伴租用戶中的每個使用者強制執行 MFA。 這是間接轉銷商必須執行的動作。

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>我沒有使用合作夥伴中心 API。 我是否仍然需要實作 MFA？

是。此安全性需求適用於所有使用者，包括合作夥伴租用戶中的合作夥伴系統管理使用者及使用者。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>哪些協力廠商提供與 Azure Active Directory 相容的 MFA 解決方案？

檢閱 MFA 廠商及解決方案時，合作夥伴必須確保他們所選擇的解決方案能與 Azure Active Directory 相容。

Microsoft 已不再針對獨立身分識別提供者提供驗證測試，以確認與 Azure Active Directory 之間的相容性。 如果您想要測試您產品的互通性，請參閱這些[指導方針](https://www.microsoft.com/download/details.aspx?id=56843) \(英文\)。

如需詳細資訊，請參閱 [Azure AD 同盟相容性清單](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility) \(部分機器翻譯\)。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>我要如何在我們的整合沙箱中測試 MFA？

應該啟用 Azure AD 安全性預設值功能，或者您也可以運用利用同盟的協力廠商解決方案。

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>啟用 MFA 是否會影響我與客戶租用戶之間的互動方式？

不可以。 履行這些安全性需求將不會影響您管理客戶的方式。 您執行委派系統管理作業的能力將不會中斷。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>我的客戶是否需要遵守合作夥伴安全性需求？

否。您不需要針對您客戶 Azure AD 租用戶中的每個使用者強制執行 MFA。 不過，建議您與每個客戶合作，以判斷保護其使用者的最佳方式。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>是否可以將任何使用者排除於此需求之外？

否。您合作夥伴租用戶中的每個使用者 (包括服務帳戶) 都必須使用 MFA 進行驗證。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>合作夥伴安全性需求是否適用於整合沙箱？

是。合作夥伴安全性需求適用於整合沙箱。 這代表您必須為整合沙箱租用戶中的使用者實作適當的 MFA 解決方案。 建議您實作 Azure AD 安全性預設值來提供 MFA。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>我如何設定緊急存取 (緊急開關) 帳戶？

一般認為的最佳做法，是建立一或兩個緊急存取帳戶，以因應不小心被封鎖在自己的 Azure AD 租用戶之外的情況。 基於合作夥伴安全性需求，每個使用者都必須使用 MFA 進行驗證。 這代表您必須修改緊急存取帳戶的定義。 它可以是運用協力廠商解決方案來進行 MFA 的帳戶。

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>如果我使用的是第三方解決方案，是否需要 Active Directory 同盟服務 (ADFS)？

否。如果您使用的是第三方解決方案，則不需要 Active Directory 同盟服務 (ADFS)。 建議您與解決方案的廠商合作，以判斷其解決方案的需求為何。

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>是否需要啟用 Azure AD 安全性預設值？

否，不需要啟用 Azure AD 安全性預設值。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>是否可以使用條件式存取來符合 MFA 需求？

是。您可以使用條件式存取來針對合作夥伴租用戶中的每個使用者 (包括服務帳戶) 強制執行 MFA。 不過，基於合作夥伴所擁有的高度權限，我們必須確保每個使用者的每個驗證都有 MFA 挑戰。 這代表您將無法運用條件式存取能避開 MFA 需求的功能。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>合作夥伴安全性需求是否會影響到 Azure AD Connect 所使用的服務帳戶？

否。合作夥伴安全性需求並不會影響到 Azure AD Connect 所使用的服務帳戶。 如果您因強制執行 MFA 而遇到與 Azure AD Connect 相關的問題，請向 Microsoft 支援服務開啟技術性支援要求。

## <a name="secure-application-model"></a>安全應用程式模型

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>誰應該採用安全應用程式模型來符合需求？

Microsoft 正在引進一個能運用 Multi-Factor Authentication 的安全可擴充架構，來驗證雲端解決方案提供者 (CSP) 合作夥伴和控制台廠商 (CPV)。 如需詳細資訊，請參閱[安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。

### <a name="what-is-the-secure-application-model"></a>什麼是安全應用程式模型？

Microsoft 正在引進一個能運用 Multi-Factor Authentication 的安全可擴充架構，來驗證雲端解決方案提供者 (CSP) 合作夥伴和控制台廠商 (CPV)。 如需詳細資訊，請參閱[安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。  

### <a name="how-do-i-implement-the-secure-application-model"></a>我要如何實作安全應用程式模型？

已使用任何 API (例如 Azure Resource Manager、Microsoft Graph、合作夥伴中心 API 等) 開發自訂整合，或是使用 PowerShell 等工具實作自訂自動化的所有合作夥伴，都必須採用[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\) 來與 Microsoft 雲端服務整合。 如果未這麼做，則可能會因部署 MFA 而導致中斷。 下列資源能提供採用此模型之方法的相關概觀和指引。

- [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
- [合作夥伴中心：安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/) \(英文\)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/) \(英文\)
- [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
- [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) \(英文\)

如果您使用的是控制台，則必須洽詢廠商有關採用安全應用程式模型架構的事宜。

控制台廠商必須以控制台廠商的身分針對合作夥伴中心進行[上線](https://docs.microsoft.com/partner-center/enroll-as-cpv)，並立即開始實作此需求。 請參閱[合作夥伴中心：安全應用程式模型架構](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。 控制台廠商必須接受並管理雲端解決方案提供者合作夥伴的同意 (而非認證)，並清除所有現有雲端解決方案提供者合作夥伴的認證。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>安全應用程式模型是否僅需針對合作夥伴中心 API/SDK 實作？

藉由針對所有使用者帳戶強制執行多重要素驗證，任何想要以非互動方式執行的自動化或整合都會受到影響。 儘管合作夥伴安全性需求需要您針對合作夥伴中心 API 啟用安全應用程式模型，但您可以利用它來解決自動化和整合進行第二個要素驗證的需求。 

>[!Note] 
>存取的資源必須支援以存取權杖為基礎的驗證。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>我正在使用 PowerShell 之類的自動化工具。 我要如何實作安全應用程式模型？

如果您的自動化是要以非互動方式執行，且仰賴使用使用者認證進行驗證，則您必須實作安全應用程式模型。 請參閱[安全應用程式模型 | 合作夥伴中心 PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) \(英文\) 以取得如何實作此架構的指引。  

>[!Note] 
>並非所有自動化工具都會提供使用存取權杖進行驗證的能力。 如果您需要協助以了解應該進行哪些變更，請在[合作夥伴中心安全性指引](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) \(英文\) 群組上張貼訊息。 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>應用程式系統管理員在執行同意程序時，應該提供哪些使用者認證？

建議您使用已指派最低權限的服務帳戶。 就合作夥伴中心 API 而言，這表示您應該使用已指派給「銷售代理人」或「系統管理代理人」角色的帳戶。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>應用程式系統管理員在執行同意程序時，為何不應該提供全域系統管理使用者認證？

使用最低權限的身分識別是最佳做法，因為那可降低風險。 不建議使用具有全域系統管理權限之帳戶的原因，是因為那會提供比起所需範圍還要多的權限。

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>我是雲端解決方案提供者合作夥伴。 我要如何知道自己的控制台廠商 (CPV) 是否正在實作該解決方案？

針對使用控制台廠商 (CPV) 解決方案來在雲端解決方案提供者 (CSP) 計畫中進行交易的合作夥伴，您必須負責洽詢自己的 CPV。

### <a name="who-is-a-control-panel-vendor-cpv"></a>誰是控制台廠商 (CPV)？

控制台廠商是開發應用程式以供雲端解決方案提供者合作夥伴用來與合作夥伴中心 API 整合的獨立軟體廠商。 控制台廠商不是能直接存取合作夥伴中心儀表板或 API 的雲端解決方案提供者合作夥伴。 如需詳細描述，請參閱[合作夥伴中心：安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>我是 CPV。 我要如何註冊？

若要註冊為控制台廠商 (CPV)，請遵循[這裡](https://docs.microsoft.com/partner-center/enroll-as-cpv)所提供的指導方針。

CPV 必須連絡 [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com)，以接收註冊連結並提供與該 CPV 具有商務關係或了解其業務的 Microsoft 員工贊助者。 例如合作夥伴開發經理 (PDM)。

在您註冊至合作夥伴中心並註冊您的應用程式之後，您將能存取合作夥伴中心 API。 如果您是新的 CPV，您將能透過合作夥伴中心通知接收到您的沙箱資訊。 在您完成 Microsoft CPV 的註冊，並接受 CPV 合約之後，您便可以：

1. 管理多租用戶應用程式 (將應用程式加入 Azure 入口網站、在合作夥伴中心中將應用程式註冊及解除註冊)。 
     >[!Note] 
     >CPV 必須在合作夥伴中心註冊其應用程式，以取得合作夥伴中心 API 的授權。 單純將應用程式加入 Azure 入口網站，並無法授權 CPV 應用程式使用合作夥伴中心 API。
2. 檢視及管理您的 CPV 設定檔。
3. 檢視及管理您需要存取 CPV 功能的使用者。 CPV 唯一可以擁有的角色是全域管理員角色。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>我正在使用合作夥伴中心 SDK。 該 SDK 是否會自動採用安全應用程式模型？

否。您必須遵循[安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)中所提供的指導方針。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>我是否可以搭配未啟用 MFA 的帳戶針對安全應用程式模型產生重新整理權杖？

是。可以使用未強制執行 MFA 的帳戶產生重新整理權杖。 不過您不應該這麼做，因為基於 MFA 需求的因素，使用未啟用 MFA 的帳戶產生的所有權杖都會無法存取資源。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>在啟用 MFA 的情況下，我的應用程式要如何取得存取權杖？

您必須遵循[安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)，其中會提供如何在遵守新安全性需求的情況下執行此操作的詳細資料。 您可以在[這裡](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) \(英文\) 找到 .NET 範例程式碼，並在[這裡](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) \(英文\) 找到 Java 範例程式碼。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>身為 CPV，我要如何在我們的 CPV 租用戶，或是 CSP 合作夥伴的租用戶中建立 Azure AD 應用程式？

CPV 必須在與其註冊為 CPV 時所關聯的租用戶中建立 Azure Active Directory 應用程式。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>我是使用僅限應用程式驗證的 CSP。 我是否需要進行任何變更？

僅限應用程式驗證並不會受到影響，因為使用者認證不會用來要求存取權杖。 如果會共用使用者認證，控制台廠商 (CPV) 必須採用[安全應用程式模型架構](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)，並清除其所擁有的任何現有合作夥伴認證。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>身為 CPV，我是否可以運用僅限應用程式驗證樣式來取得存取權杖？

否。控制台廠商合作夥伴並無法運用僅限應用程式驗證樣式來代表合作夥伴要求存取權杖。 他們應該實作安全應用程式模型，這能運用應用程式 + 使用者驗證樣式。

## <a name="technical-enforcement"></a>技術強制執行

### <a name="what-is-the-activation-of-security-safeguards"></a>什麼是安全性保護的啟用？

參與「雲端解決方案提供者 (CSP)」計畫、「控制台廠商 (CPV)」和「顧問」的所有合作夥伴，都應該實作強制的安全性需求才能繼續符合規範。

為了提供額外的保護，Microsoft 已開始啟用安全性保護，藉由強制使用多重要素驗證 (MFA) 驗證來防止未經授權的存取，而協助合作夥伴保護其租用戶和客戶。  

我們已成功對所有合作夥伴租用戶完成 admin-on-behalf-of (AOBO) 功能的啟用。 為了進一步協助保護合作夥伴和客戶，以 Q2 CY2020 為目標，我們將開始在 CSP 中啟用合作夥伴中心交易，協助合作夥伴保護其企業和客戶免於遭遇身分識別竊取相關事件。

如需詳細資訊，請造訪[對您的合作夥伴租用戶強制使用多重要素驗證 (MFA)](partner-security-requirements-mandating-mfa.md) 頁面。

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>我正在使用第三方 MFA 解決方案，但是被封鎖，我該怎麼做？

為了驗證存取資源的帳戶是否受到多重要素驗證的挑戰，我們會檢查[驗證方法參考](https://tools.ietf.org/html/rfc8176)宣告，以查看是否已列出 MFA。 有些第三方解決方案不會發出此宣告，或不包含 MFA 值。 如果遺漏宣告，或未列出 MFA 值，則無法判斷驗證的帳戶是否已挑戰多重要素驗證。 您必須與第三方解決方案的廠商合作，以判斷需要採取哪些動作，解決方案才會發出驗證方法參考宣告。

如果您不確定您的第三方解決方案是否發出預期宣告，請參閱[測試合作夥伴安全性需求](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0)。

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA 阻止我使用 AOBO 來支援我的客戶，我該怎麼做？

合作夥伴安全性需求的技術強制會檢查已驗證的帳戶是否已挑戰多重要素驗證。 如果帳戶尚未進行，則系統會將您重新導向至登入頁面，然後再次提示您進行驗證。 如需更詳細的體驗與指導方針，請參閱這份[對您的合作夥伴租用戶強制使用多重要素驗證 (MFA)](partner-security-requirements-mandating-mfa.md#partner-delegated-administration) 文件。 如果您的網域未加入同盟，則在成功驗證之後，系統會提示您設定多重要素驗證。 完成後，您就可以使用 AOBO 來管理您的客戶。 如果您的網域已加入同盟，則您必須確保帳戶會受到多重要素驗證的挑戰。

## <a name="security-defaults-transition"></a>安全性預設值轉換

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>如何從基準原則轉換到安全性預設值或其他 MFA 解決方案？

Azure Active Directory (Azure AD) [「基準」原則將會遭到移除，並取代](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults)為「安全性預設值」，這是一組更完整的保護原則，適合您和您的客戶使用。 [安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)可協助您的組織防範身分識別竊取的相關安全性攻擊。

如果您尚未從基準原則轉換為安全性預設值原則或[其他 MFA 實作選項](partner-security-requirements.md#actions-that-you-need-to-take)，則因為基準原則將會淘汰，您的多重要素驗證 (MFA) 實作會遭到移除。 系統會要求合作夥伴租用戶中執行受 MFA 保護作業的使用者完成 MFA 驗證。 請於[這裡](partner-security-requirements-mandating-mfa.md)檢閱更詳細的指導方針。
若要持續符合規範並將中斷的情況降至最低，請採取下列其中一個動作：

- 轉換成安全性預設值
    - 安全性預設值原則是合作夥伴可選擇來實作 MFA 的其中一個選項。 其提供基本層級的安全性，而且不需額外費用即可啟用。
    - 了解如何使用 Azure AD 為組織啟用 MFA，並檢閱[安全性預設值重要考量](partner-security-requirements.md#security-defaults)。
    - 請啟用符合您商務需求的安全性預設值原則。
- 轉換為條件式存取
    - 如果安全性預設值原則不符合您的需求，請啟用條件式存取。 如需詳細資訊，請檢閱 Azure AD 條件式存取文件。

## <a name="key-resources"></a>主要資源

### <a name="how-to-get-started"></a>如何開始使用

- [合作夥伴安全性需求：逐步指南](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 將您的問題和意見反應移至此[合作夥伴中心安全性指引群組](https://aka.ms/MPCSecurityGuidance) \(英文\)。
- 參與近期的合作夥伴辦公時間和網路研討會。 請查看[這裡的詳細排程和資源](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) \(英文\)。

### <a name="resources-for-adopting-secure-application-model"></a>採用安全應用程式模型的資源

- [安全應用程式模型概觀](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) \(英文\)
- [合作夥伴中心：安全應用程式模型指南](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 .NET 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/) \(英文\)
- [雲端解決方案提供者計畫中的合作夥伴：用於啟用安全應用程式模型的 Java 範例程式碼](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/) \(英文\)
- [合作夥伴中心驗證文件](https://docs.microsoft.com/partner-center/develop/partner-center-authentication) \(英文\)
- [合作夥伴中心 PowerShell Multi-Factor Authentication (MFA) 文件](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) \(英文\)

## <a name="support"></a>支援

### <a name="where-can-i-get-support"></a>我可以在哪裡取得支援？

如需符合安全性需求的支援資源，如果您具有進階合作夥伴支援 (ASfP)，請連絡您的服務帳戶經理；如果您具有頂級合作夥伴支援合約 (PSfP)，請連絡您的服務帳戶經理及技術帳戶經理。

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>我如何取得技術資訊和支援以協助採用安全應用程式模型架構？

您可透過 MPN 權益使用適用於 Azure Active Directory 的技術產品支援選項。 能存取有效 ASfP 或 PSfP 訂用帳戶的合作夥伴可以與其相關聯的帳戶經理 (SAM/TAM) 合作，以了解最適合他們的選項。

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>當我失去合作夥伴中心的存取權時，如何聯絡支援人員？

前往 [Microsoft 合作夥伴支援](https://partner.microsoft.com/support)，然後選擇 [顯示所有支援選項]。 您會看到可用來聯絡 Microsoft 合作夥伴支援的選項。 其中包括致電支援人員的電話號碼，以及與支援人員交談的選項。 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>我可以在哪裡找到技術性常見問題的詳細資訊？

關於技術性常見問題的相關資訊可在[這裡](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)找到。

