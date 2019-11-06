---
title: 合作夥伴安全性需求 | 合作夥伴中心
ms.topic: article
ms.date: 10/11/2019
description: 瞭解參與雲端解決方案提供者計畫之顧問和合作夥伴的安全性需求。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, 雲端解決方案提供者, 雲端解決方案提供者計畫, CSP, 控制台廠商, CPV, 多重要素驗證, MFA, 安全應用程式模型, 安全應用程式模型, 安全性
ms.localizationpriority: high
ms.openlocfilehash: 4c7f4e61cc249fb51f58e4a94892a2d937cae4e1
ms.sourcegitcommit: 1fe366f787d97c96510cfd409304e7d48af7c286
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/30/2019
ms.locfileid: "73141978"
---
# <a name="partner-security-requirements"></a>合作夥伴安全性需求

**適用於**

- 雲端解決方案提供者計畫中的所有合作夥伴
  - 直接帳單
  - 間接提供者
  - 間接轉銷商
- 所有控制台廠商
- 所有顧問

較高的隱私權保護和安全性是我們最優先的考量。 我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。 這就是為什麼我們需要生態系統中的每個人都採取行動，並確保其具備適當的安全性保護。 為了協助保護合作夥伴和客戶，我們針對參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴推出一組強制性的安全性需求。

## <a name="overview"></a>概觀

自 2019 年 8 月 1 日起，所有合作夥伴都必須針對其合作夥伴租用戶的所有使用者帳戶強制執行多重要素驗證。 與合作夥伴安全性需求相關聯的條款已新增至[雲端解決方案提供者計畫指南](https://go.microsoft.com/fwlink/p/?LinkId=617100)。 與顧問相關的是，相同的合約需求也將備妥。

> [!NOTE]
> 我們強烈建議所有合作夥伴透過主權雲端 (21Vianet、US Government 和 Germany) 進行交易，並立即採取這些安全性需求。 不過，這些合作夥伴不需要符合 2019 年 8 月 1 日生效的安全性需求。 Microsoft 未來將針對主權雲端的這些安全性需求強制執行，提供額外的詳細資料。

一旦強制執行這些需求，未實作強制安全性需求的合作夥伴，將無法在雲端解決方案提供者計畫中進行交易，或利用委派系統管理員權限來管理客戶租用戶。

## <a name="actions-that-you-need-to-take"></a>您需要採取的動作

若要符合合作夥伴的安全性需求，您必須針對合作夥伴租用戶中的每位使用者帳戶強制執行多重要素驗證。 您可以透過下列其中一種方式來完成這項作業

- 實作 Azure Active Directory 的「[要求系統管理員使用 MFA](/azure/active-directory/conditional-access/howto-baseline-protect-administrators)」和「[使用者保護](/azure/active-directory/conditional-access/howto-baseline-protect-end-users)」基準保護原則功能，而無需額外費用
- 為每個使用者帳戶購買 Azure Active Directory Premium。 如需詳細資訊，請參閱[規劃雲端式 Azure 多重要素驗證部署](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)。
- 使用協力廠商解決方案，對合作夥伴租用戶中的每個使用者帳戶強制執行多重要素驗證。 如需詳細資訊，請參閱[如何強制執行安全性需求](#how-the-requirements-will-be-enforced)，以確保解決方案會提供預期的資訊。

### <a name="consideration"></a>考量

因為這些需求適用於合作夥伴租用戶中的所有使用者，所以要確保順利部署就需要進行幾項考量。 這些考量包括識別 Azure Active Directory 中無法執行多重要素驗證的使用者帳戶，以及組織所使用不支援新式驗證的應用程式和裝置。

執行任何動作之前，建議您先找出下列各項

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>您是否具有不支援使用新式驗證的應用程式或裝置？

強制執行多重要素驗證的舊版驗證時，將會封鎖使用 IMAP、POP3、SMTP 等通訊協定，因為這些通訊協定不支援多重要素驗證。 若要解決此限制，稱為[應用程式密碼](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)的功能可用來確保應用程式或裝置仍然可以進行驗證。 您應該複查[這裡](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)所記載、使用應用程式密碼的考量事項，以判斷是否可以在您的環境中使用它們。

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>您是否有使用者使用與合作夥伴租用戶使用者相關聯的授權所提供的 Office 365？

在實作任何解決方案之前，建議您先判斷合作夥伴租用戶中的使用者所使用的 Microsoft Office 版本為何。 在採取任何動作之前，先複查[規劃 Office 365 部署的多重要素驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)。 您的使用者可能會遇到 Outlook 之類應用程式的連線問題。 強制執行多重要素驗證之前，請務必確定正在使用 Outlook 2013 SP1 或更新版本，且您的組織已啟用新式驗證。 如需詳細資訊，請參閱[在 Exchange Online 中啟用新式驗證](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)。

若要為執行 Windows 且已安裝 Microsoft Office 2013 的任何裝置啟用新式驗證，您將需要建立兩個登錄機碼。 請參閱[為 Windows 裝置上的 Office 2013 啟用新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>是否有原則防止任何使用者在工作時使用其行動裝置？

請務必找出會防止員工在工作時使用行動裝置的任何公司原則，因為該原則會影響您所實作的多重要素驗證解決方案。 部分解決方案，例如透過[基準保護原則](/azure/active-directory/conditional-access/concept-baseline-protection)所實作的解決方案，只會允許使用驗證器應用程式進行驗證。 如果您的組織有防止使用行動裝置的原則，則應該考量下列其中一個選項

- 部署可在安全系統上執行的以時間為基礎的一次性基礎密碼 (TOTP) 應用程式
- 實作協力廠商解決方案，在可提供最適當驗證選項的合作夥伴租用戶中，為每個使用者帳戶強制執行多重要素驗證
- 為受影響的使用者購買 [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) 授權

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>您有會利用使用者認證進行驗證的哪些自動化或整合？

由於需求是對合作夥伴目錄中的每個使用者 (包括服務帳戶) 強制執行 MFA，因此，利用使用者認證進行驗證的任何自動化或整合都會受到影響。 因此，請務必找出在這些情況下所使用的帳戶。 以下是應該考量的應用程式或服務的範例清單

- 用來代表您的客戶佈建資源的控制台
- 與用於發票 (與雲端解決方案提供者計畫相關) 的任何平台整合並支援您的客戶
- 使用 Az、AzureRM、Azure AD、MS Online 等模組的 PowerShell 指令碼

以上清單並不完整。 因此，在利用使用者認證來進行驗證的環境中，請務必執行任何應用程式或服務的完整評估。 若要與多重要素驗證的需求抗衡，您應該盡可能在[安全應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)中實作指導方針。

## <a name="accessing-your-environment"></a>存取您的環境

若要進一步瞭解未經過多重要素驗證查問而進行驗證的內容或對象，建議您參閱登入活動。 您可以透過 Azure Active Directory Premium 來運用登入報告。 如需詳細資訊，請參閱 Azure Active Directory 入口網站中的[登入活動報告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)。 如果您沒有 Azure Active Directory Premium，或是想要透過 PowerShell 取得 Azure Active Directory Premium 的方法，則必須從[合作夥伴中心 PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) 模組中，運用 [PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) Cmdlet。

## <a name="how-the-requirements-will-be-enforced"></a>強制執行需求的方法

合作夥伴安全性需求將會由 Azure Active Directory 強制執行，然後由合作夥伴中心強制執行，方法是藉由檢查 MFA 宣告是否存在來識別已執行多重要素驗證。 如果您正在使用 Azure 多重要素驗證或基準保護原則，則不需要採取任何其他動作。

使用協力廠商的多重要素驗證解決方案時，可能不會發出 MFA 宣告。 如果遺漏此宣告，則 Azure Active Directory 將無法判斷驗證要求是否經過多重要素驗證的查問。 如需如何驗證解決方案發出預期宣告的詳細資訊，請參閱[測試合作夥伴安全性需求](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)。

> [!IMPORTANT]
> 如果協力廠商解決方案未發出預期的宣告，則您必須與開發解決方案的廠商合作，以判斷應該採取哪些動作。

## <a name="resources-and-support"></a>資源與支援

以下是可以找到支援和範例程式碼的資源

- [合作夥伴中心安全性指導群組社群](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) - 這是線上社群，您可以在其中瞭解近期活動，並詢問您可能會遇到的任何問題。
- [合作夥伴中心 .NET 範例](https://github.com/microsoft/partner-center-dotnet-samples) - 此 GitHub 存放庫包含使用 .NET 開發的範例，將示範如何實作安全應用程式模型架構。
- [合作夥伴中心 Java 範例](https://github.com/microsoft/partner-center-java-samples) - 此 GitHub 存放庫包含使用 Java 開發的範例，將示範如何實作安全應用程式模型架構。
- [合作夥伴中心 PowerShell - 多重要素驗證](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - 本文章提供如何使用 PowerShell 來實作安全應用程式模型架構的詳細資料。
