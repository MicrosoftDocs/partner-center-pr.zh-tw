---
title: 從 PMC 遷移至合作夥伴中心的指南 |合作夥伴中心
ms.topic: article
ms.date: 04/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 當您將公司從 PMC 遷移至合作夥伴中心時的須知事項
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 移轉, 移至合作夥伴中心
ms.localizationpriority: medium
ms.openlocfilehash: a39c4114758004ff4291bc577182fd8ba469149b
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653092"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>從 PMC 遷移至合作夥伴中心的指南

Partner.microsoft.com 的 Microsoft 合作夥伴網站是合作夥伴的統一數位體驗。 從合作夥伴網站中，您將能夠探索您的機會並參與引導式體驗，以協助您的公司與 Microsoft 建立及銷售您的應用程式與服務。 使用可跨合作夥伴網站取得的 [儀表板] 連結，Microsoft 合作夥伴網路的成員可以登入合作夥伴中心，您可以在其中管理與 Microsoft 的關係、註冊方案，並註冊供應專案。 

合作夥伴會員中心（PMC）即將解除委任。 您的公司已受邀將您的 Microsoft 合作夥伴網路成員資格管理轉換至合作夥伴中心。 本指南將協助您進行從 PMC 移至合作夥伴中心時所預期的情況。

>[!Note]
>即使您的公司有多個帳戶或位置，移至合作夥伴中心一開始會先將一個（您的第一個）帳戶移至合作夥伴中心。

## <a name="get-started"></a>入門

移動開始于 PMC。 您的全域管理員會收到開始移動的邀請。 

**在 PMC 中準備**
- 確認您的公司詳細資料 
- 驗證主要計畫連絡人 
- 驗證商務位置
- 更新已核准的使用者

**當您準備好時**

選取您邀請上的 [**開始**使用]。 您將會進入合作夥伴中心的登入頁面。

![入門](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>開始使用您的工作電子郵件

如果您的公司沒有工作電子郵件和 AAD 租使用者，我們可以協助您在合作夥伴中心登入程式期間設定一個。 當您嘗試使用不是工作電子郵件（例如您的個人帳戶）的電子郵件帳戶登入時，系統會將您導向您的公司相關資訊，讓我們可以設定 AAD 租使用者和工作電子郵件。
這些公司詳細資料將用來在合作夥伴中心完成您的帳戶，因此請確定它們是正確的。

>[!Note]
>如果您是中國的合作夥伴，並同時在 Microsoft 合作夥伴網路和雲端解決方案提供者（CSP）方案中註冊，您將會有每個帳戶的個別租使用者。 使用雲端解決方案提供者方案的帳戶是在國家雲端進行管理，而您的 Microsoft 合作夥伴網路帳戶則是在全球雲端進行管理。 無法連結這兩個帳戶。

![告訴我們您的公司](images/migration/newtellusabout.png)

驗證或更新資訊之後，請選取 [**接受並繼續**]。
此頁面上的條款及條件與您公司已登入 PMC 的合約**完全相同**。  
這會起始 Azure AD 租使用者的建立，並為您提供工作帳戶。

選取 [**接受並繼續**] 也會執行下列動作：

•將您的帳戶連同其所有位置一起遷移至合作夥伴中心

•遷移您可能已在 PMC 中購買的任何專長認證或對應

•遷移您在 PMC 中擁有的擁有權益（地圖、銀級、金級）

## <a name="invite-employees-to-join-you"></a>邀請員工加入您

當您建立新的 Azure AD 租使用者時，您可以邀請您的員工登入合作夥伴中心。

![邀請員工](images/migration/invite.png)


如果您已使用現有的 AAD 租使用者登入，您的員工將會與您一起移動。 在此情況下，請指派您的員工角色來決定他們可以在合作夥伴中心執行的工作。 注意：合作夥伴中心的角色與 PMC 中的角色不同。 如需詳細資訊，請參閱[從 PMC 移至合作夥伴中心](move-pmc-pc-map.md)。

## <a name="verify-your-domain-and-become-a-global-admin"></a>驗證您的網域，並成為全域管理員  

如果您的 AAD 租使用者是新的，則不會有任何人指派為全域管理員的角色。若要成為全域管理員，您必須驗證您的網域擁有權。 您可能需要網域系統管理員來協助您進行此工作。 請注意，雖然您可以使用已購買的供應專案，但在您完成取得全域管理員的步驟之前，將無法購買任何新的供應專案。 

![Take 控制項](images/migration/takecontrol.png)

當您選取 [開始使用] 時，您會看到下列畫面：

![確認網域擁有權](images/migration/verifytxt.png)

您的網域註冊機構將已為您填入。 只有網域擁有者可以更新 DNS 檔案，因此藉由將文本檔案複製並新增至您的 DNS 記錄，我們可以驗證您是否為擁有者。 需要幾分鐘的時間才會進行更新。 您將需要登出合作夥伴中心，然後重新登入。 您的角色已變更為全域管理員。 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>熟悉您的儀表板和合作夥伴中心

流覽您的儀表板。 您可以在這裡管理您的成員資格、新增參考的商務設定檔、註冊雲端解決方案提供者方案，並選取 [**儀表板**] 隨時查看與您的商務相關的通知和供應專案。 您也可以管理獎勵、在 marketplace 購買、註冊進入市場服務等。  

![進行導覽](images/migration/fre.png)

## <a name="next-steps"></a>後續步驟

- [建立使用者帳戶](create-user-accounts-and-set-permissions.md)
- [指派使用者角色和權限](permissions-overview.md)
- [管理您的成員資格計畫](renew-mpn-offers.md)
- [建立公司的商務設定檔](create-a-marketing-profile.md)
- [透過推薦與客戶保持聯繫](responding-to-referrals.md)

## <a name="see-also"></a>請參閱

- [將多家公司從 PMC 遷移至合作夥伴中心的指南](move-multiple-companies.md)
