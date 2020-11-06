---
title: 合作夥伴安全性需求
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 介紹啟用多重要素驗證 (MFA) 和採用安全應用程式模型架構的合作夥伴安全性需求。
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 351d0715645b6e43607279393cdc376d898a7f54
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/31/2020
ms.locfileid: "93132972"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>使用合作夥伴中心或合作夥伴中心 API 的安全性需求

**適用於**

- 雲端解決方案提供者計畫中的所有合作夥伴
- 所有控制台廠商
- 所有顧問

**適當的使用者**

- 所有已啟用的使用者，包括來賓使用者

本文說明參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴的安全性需求，以及驗證選項和其他安全性考量。 隱私權保護和安全性是我們最優先的考量。 我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。 這就是為什麼我們需要生態系統中的每個人都採取行動，並確保具備適當的安全性保護。

## <a name="mandatory-security-requirements"></a>必要的安全性需求

未實作強制安全性需求的合作夥伴將無法在雲端解決方案提供者計畫中進行交易，或利用委派的系統管理員權限來管理客戶租用戶。 此外，未實作安全性需求的合作夥伴，可能會在參與計畫時面臨風險。 與合作夥伴安全性需求相關聯的條款已新增至 Microsoft 合作夥伴合約。 與顧問相關的是，相同的合約需求也將備妥。

為了保護您和您的客戶，我們要求合作夥伴立即採取下列動作：  

1. **為合作夥伴租用戶中的所有使用者帳戶啟用多重要素驗證 (MFA)** 。 您必須在合作夥伴租用戶中的所有使用者帳戶上強制執行 MFA。 使用者帳戶在登入 Microsoft 商業雲端服務，或是透過合作夥伴中心或 API 在雲端解決方案提供者計畫中進行交易時，都必須經過 MFA 的查問。

2. **採用安全應用程式模型架構** 。 所有與合作夥伴中心 API 整合的合作夥伴，都必須針對任何應用程式和使用者驗證模型應用程式採用[安全應用程式模型架構](/partner-center/develop/enable-secure-app-model)。

    > [!IMPORTANT]
    > 我們強烈建議合作夥伴實作安全應用程式模型，以與 Microsoft API (例如 Azure Resource Manager、Microsoft Graph) 進行整合，或利用使用者認證來運用自動化 (例如 PowerShell)，以避免在強制執行 MFA 時發生任何中斷。

這些安全性需求將有助於保護您的基礎結構，並保護您客戶的資料免於潛在的安全性風險 (例如身分盜用或其他詐騙事件)。  

## <a name="implementing-multi-factor-authentication"></a>實作多重要素驗證

若要符合合作夥伴的安全性需求，您必須為合作夥伴租用戶中的每個使用者帳戶實作並強制執行 MFA。 您可以使用下列其中一種方法執行這個動作：

- 實作 [Azure Active Directory (Azure AD) 安全性預設值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。 請參閱 [下一節](#security-defaults) 中的詳細資訊。

- 為每個使用者帳戶購買 Azure Active Directory Premium。 如需詳細資訊，請參閱[規劃 Azure Multi-Factor Authentication 部署](/azure/active-directory/authentication/howto-mfa-getstarted)。

- 使用第三方解決方案，為合作夥伴租用戶中的每個使用者帳戶強制執行 MFA。 若要確保解決方案會提供預期的解決方案，請參閱[如何強制執行安全性需求](#how-the-requirements-are-enforced)。

> [!NOTE]
> 雖然在合約上，主權雲端 (美國政府和德國) 不需要多重要素驗證，但強烈建議您採用這些安全性需求。

### <a name="security-defaults"></a>安全性預設值

合作夥伴可選擇用來實作 MFA 需求的選項之一，是在 Azure AD 中啟用安全性預設值。 安全性預設值提供基本層級的安全性，且無需額外費用。 啟用安全性預設值之前，請先檢閱如何使用 Azure AD 為您的組織啟用 MFA，以及下列主要考量。

- 已採用基準原則的合作夥伴必須採取動作，才能轉換成安全性預設值。

- 安全性預設值可取代預覽基準原則的一般可用性。 當合作夥伴啟用安全性預設值之後，他們將無法再啟用基準原則。

- 使用安全性預設值時，將會一次啟用所有原則。

- 使用[條件式存取](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)的合作夥伴將[無法使用安全性預設值](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)。

- 我們目前不會封鎖舊版驗證。 不過，由於與身分盜用相關的大部分事件都來自使用舊版驗證的登入嘗試，因此我們鼓勵合作夥伴捨棄這些較舊的通訊協定。

- Azure AD Connect 同步帳戶已從安全性預設值中排除。

如需詳細資訊，請參閱[組織的 Azure Multi-Factor Authentication 概觀](/azure/active-directory/authentication/concept-mfa-get-started)和[何謂安全性預設值？](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。

> [!NOTE]
> Azure AD 安全性預設值是從簡化的基準保護原則演化而來的。 如果您已啟用基準保護原則，則強烈建議您啟用[安全性預設值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)。

## <a name="implementation-considerations"></a>實作考量

這些需求適用於您夥伴租用戶中的所有使用者帳戶，因此您必須考量若干事項，以確保能夠順利部署。 例如，識別 Azure AD 中無法執行 MFA 的使用者帳戶，以及您的組織中不支援新式驗證的應用程式和裝置。

在執行任何動作之前，建議您先完成下列驗證。 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>您是否具有不支援使用新式驗證的應用程式或裝置？

當您強制執行 MFA 舊版驗證時，將會封鎖使用 IMAP、POP3、SMTP 等通訊協定，因為這些通訊協定不支援 MFA。 若要解決此限制，請使用[應用程式密碼](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)功能來確保應用程式或裝置仍會進行驗證。 請檢閱[使用應用程式密碼的考量事項](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)，以確認是否可在您的環境中加以使用。

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>您是否有 Office 365 使用者具有與合作夥伴租用戶相關聯的授權？

在實作任何解決方案之前，建議您先確認合作夥伴租用戶中的使用者所使用的 Microsoft Office 版本。 您的使用者可能會遇到 Outlook 之類應用程式的連線問題。 強制執行 MFA 之前，請務必確定您使用的是 Outlook 2013 SP1 或更新版本，且您的組織已啟用新式驗證。 如需詳細資訊，請參閱[在 Exchange Online 中啟用新式驗證](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)。 

若要為執行 Windows 且已安裝 Microsoft Office 2013 的裝置啟用新式驗證，您將需要建立兩個登錄機碼。 請參閱[為 Windows 裝置上的 Office 2013 啟用新式驗證](/office365/admin/security-and-compliance/enable-modern-authentication)。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>是否有原則防止任何使用者在工作時使用其行動裝置？

請務必找出會防止員工在工作時使用行動裝置的任何公司原則，因為它會影響您所實作的 MFA 解決方案。 部分解決方案，例如透過 [Azure AD 安全性預設值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)所實作的解決方案，只會允許使用驗證器應用程式進行驗證。 如果您的組織有防止使用行動裝置的原則，則應該考量下列其中一個選項：

- 部署可在安全系統上執行的以時間為基礎的一次性基礎密碼 (TOTP) 應用程式。

- 實作第三方解決方案，在可提供最適當驗證選項的合作夥伴租用戶中，為每個使用者帳戶強制執行 MFA。

- 為受影響的使用者購買 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 授權。

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>您有會利用使用者認證進行驗證的哪些自動化或整合？

由於我們為合作夥伴目錄中的每個使用者 (包括服務帳戶) 強制執行 MFA，因此，利用使用者認證進行驗證的任何自動化或整合都會受到影響。 因此，請務必找出在這些情況下所使用的帳戶。 請參閱下列範例應用程式或服務的清單以供考慮：

- 用來代表您的客戶佈建資源的控制台

- 與用於發票 (與雲端解決方案提供者計畫相關) 的任何平台整合並支援您的客戶

- 使用 Az、AzureRM、Azure AD、MS Online 等模組的 PowerShell 指令碼

以上清單並不完整。 因此，在利用使用者認證來進行驗證的環境中，請務必執行任何應用程式或服務的完整評估。 若要與 MFA 的需求抗衡，您應該盡可能在[安全應用程式模型架構](/partner-center/develop/enable-secure-app-model)中實作指導方針。

## <a name="accessing-your-environment"></a>存取您的環境

若要進一步了解未經過 MFA 查問而進行驗證的內容或對象，建議您檢閱登入活動。 您可以透過 Azure Active Directory Premium 來運用登入報告。 如需此主題的詳細資訊，請參閱 [Azure Active Directory 入口網站中的登入活動報告](/azure/active-directory/reports-monitoring/concept-sign-ins)。 如果您沒有 Azure Active Directory Premium，或是想要找出方法來透過 PowerShell 取得此登入活動，則必須從[合作夥伴中心 PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) 模組中，運用 [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) Cmdlet。

## <a name="how-the-requirements-are-enforced"></a>強制執行需求的方式

合作夥伴安全性需求會由 Azure AD 強制執行，然後由合作夥伴中心強制執行，方法是藉由檢查 MFA 宣告是否存在來識別已執行 MFA 驗證。 自 2019 年 11 月 18 日起，Microsoft 就已針對合作夥伴租用戶啟用額外的安全性保護措施 (先前稱為「技術強制」)。

啟用時，將會要求合作夥伴租用戶中的使用者在執行任何系統管理員代表 (AOBO) 作業、存取合作夥伴中心入口網站或呼叫合作夥伴中心 API 時完成 MFA 驗證。 如需詳細資訊，請參閱[對您的合作夥伴租用戶強制使用多重要素驗證 (MFA)](partner-security-requirements-mandating-mfa.md)。 

未符合需求的合作夥伴應該儘快實作這些措施，以避免任何業務中斷。 如果您是使用 Azure Multi-Factor Authentication 或 Azure AD 安全性預設值，則不需要採取任何其他動作。

如果您使用第三方 MFA 解決方案，則系統可能不會發出 MFA 宣告。 如果遺漏此宣告，則 Azure AD 將無法判斷驗證要求是否經過 MFA 的查問。 如需如何驗證解決方案發出預期宣告的詳細資訊，請閱讀[測試合作夥伴安全性需求](/powershell/partnercenter/test-partner-security-requirements)。 

> [!IMPORTANT]
> 如果協力廠商解決方案未發出預期的宣告，則您必須與開發解決方案的廠商合作，以判斷應該採取哪些動作。

## <a name="resources-and-samples"></a>資源和範例

如需支援和範例程式碼，請參閱下列資源：

- [合作夥伴中心安全性指導群組社群](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)：合作夥伴中心安全性指導群組社群是線上社群，您可以在其中瞭解近期活動，並詢問您可能會遇到的任何問題。
- [合作夥伴中心 .NET 範例](https://github.com/microsoft/partner-center-dotnet-samples)：此 GitHub 存放庫包含使用 .NET 開發的範例，將示範如何實作安全應用程式模型架構。
- [合作夥伴中心 Java 範例](https://github.com/microsoft/partner-center-java-samples)：此 GitHub 存放庫包含使用 Java 開發的範例，將示範如何實作安全應用程式模型架構。
- [合作夥伴中心 PowerShell - Multi-Factor Authentication](/powershell/partnercenter/multi-factor-auth)：此多重要素驗證文章提供如何使用 PowerShell 來實作安全應用程式模型架構的詳細資料。

## <a name="next-steps"></a>後續步驟

- [對您的合作夥伴租用戶強制使用多重要素驗證 (MFA)](partner-security-requirements-mandating-mfa.md)