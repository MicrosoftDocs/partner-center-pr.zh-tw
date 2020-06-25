---
title: 從 PMC 遷移到合作夥伴中心
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何將您的公司從 Partner Membership Center (PMC) 遷移至合作夥伴中心。
author: LauraBrenner
ms.author: labrenne
keywords: PMC, 移轉, 移至合作夥伴中心
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 773466a1c7bfb8a091be11f8e825dae6cc90b765
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679085"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>從 PMC 移轉至合作夥伴中心的指南

**適當的角色**

- 全域系統管理員

Microsoft 合作夥伴網站 (網域為 Partner.microsoft.com) 是合作夥伴的統一數位體驗。 從合作夥伴網站中，您將能夠探索您的商機並參與引導式體驗，以協助您的公司利用 Microsoft 建置並銷售您的應用程式與服務。 使用可跨合作夥伴網站提供的儀表板連結，Microsoft 合作夥伴網路的會員可以登入合作夥伴中心，您可以在其中管理與 Microsoft 的關係、註冊方案，以及註冊供應項目。

Partner Membership Center (PMC) 即將解除任務。 您的公司已受邀將您的 Microsoft 合作夥伴網路會員資格管理轉移至合作夥伴中心。 本指南將為您從 PMC 移至合作夥伴中心時所預期的情況做好準備。

>[!NOTE]
>即使您的公司有多個帳戶或位置，移至合作夥伴中心一開始會先將某個 (您的第一個) 帳戶移至合作夥伴中心。

## <a name="get-started"></a>開始使用

移動開始於 PMC。 您的全域系統管理員會收到開始移動的邀請。

### <a name="prepare-in-pmc"></a>在 PMC 中準備

- 驗證公司詳細資料
- 驗證主要方案連絡人
- 驗證商務位置
- 更新您核准的使用者

### <a name="when-youre-ready"></a>當您就緒時

選取您邀請上的 [開始]。 您將會進入合作夥伴中心的登入頁面。

:::image type="content" source="images/migration/getstarted.jpg" alt-text="開始使用":::

## <a name="start-with-your-work-email"></a>從您的工作電子郵件開始

如果您的公司沒有工作電子郵件和 AAD 租用戶，我們可以協助您在合作夥伴中心登入過程中設定一個。 當您嘗試使用不是工作電子郵件的電子郵件帳戶 (例如您的個人帳戶) 登入時，系統會引導您提供公司相關資訊，讓我們可以設定 AAD 租用戶和工作電子郵件。 這些公司詳細資料將用來在合作夥伴中心完成您的帳戶，因此請確定它們是正確的。

>[!NOTE]
>如果您是位於中國的合作夥伴，並同時在 Microsoft 合作夥伴網路和雲端解決方案提供者 (CSP) 方案中註冊，您的每個帳戶將會有個別租用戶。 您搭配雲端解決方案提供者方案的帳戶是在國家雲端進行管理，而您的 Microsoft 合作夥伴網路帳戶則是在全球雲端進行管理。 無法連結這兩個帳戶。

:::image type="content" source="images/migration/newtellusabout.png" alt-text="向我們描述您的公司":::

一旦驗證或更新了資訊後，請選取 [接受並繼續]。
此頁面上的條款與貴公司已在 PMC 簽署的合約**完全相同**。  
這個步驟會起始 Azure AD 租用戶的建立，並為您提供工作帳戶。

選取 [接受並繼續] 也會執行下列動作：

- 將您的帳戶連同其所有位置移轉至合作夥伴中心

- 移轉您可能已在 PMC 中購買的任何專長認證或 MAP

- 移轉您已在 PMC 中擁有的任何行銷資源、供應項目及方案 (MAP、銀級、金級)

## <a name="invite-employees-to-join-you"></a>邀請員工加入您

當建立新的 Azure AD 租用戶時，您可以邀請員工登入合作夥伴中心。

:::image type="content" source="images/migration/invite.png" alt-text="邀請員工":::

如果您已使用現有的 AAD 租用戶登入，您的員工將會與您一起移動。 在此情況下，請為您的員工指派可決定他們在合作夥伴中心做什麼的角色。 

>[!NOTE] 
>合作夥伴中心的角色與 PMC 中的角色不同。 如需詳細資訊，請參閱[從 PMC 移至合作夥伴中心](move-pmc-pc-map.md)。

## <a name="verify-your-domain-and-become-a-global-admin"></a>驗證您的網域並成為全域系統管理員  

如果您的 AAD 租用戶是新的，則不會有任何人獲指派為全域系統管理員的角色。若要成為全域系統管理員，您必須驗證您的網域擁有權。 您可能需要網域系統管理員來協助您處理此工作。

雖然您可以使用已購買的供應項目，但在您完成指派全域管理員的步驟之前，將無法購買任何新的供應項目。

:::image type="content" source="images/migration/takecontrol.png" alt-text="掌握控制權":::

當您選取開始時，您會看到下列畫面：

:::image type="content" source="images/migration/verifytxt.png" alt-text="驗證網域擁有權":::

您的網域註冊將已填入資料。 只有網域擁有者可以更新 DNS 檔案，因此藉由將文字檔案複製並新增至您的 DNS 記錄，我們可以驗證您是否為擁有者。 將需要幾分鐘的時間才會進行更新。 您將需要登出合作夥伴中心，然後重新登入。 您的角色已變更為全域系統管理員。

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>熟悉您的儀表板和合作夥伴中心

導覽您的儀表板。 您可以在這裡管理您的會員資格、新增參考用的商務設定檔、註冊雲端解決方案提供者方案，以及透過選取 [儀表板] 隨時查看與您商務相關的通知和供應項目。 您也可以管理獎勵、在市集購買、註冊上市服務等。  

:::image type="content" source="images/migration/fre.png" alt-text="進行導覽":::

## <a name="next-steps"></a>接下來的步驟

- [建立使用者帳戶](create-user-accounts-and-set-permissions.md)

- [指派使用者角色和權限](permissions-overview.md)

- [管理您的成員資格計畫](renew-mpn-offers.md)

- [建立公司的商務設定檔](create-a-marketing-profile.md)

- [透過推薦與客戶保持聯繫](responding-to-referrals.md)

- [將多家公司從 PMC 移轉至合作夥伴中心的指南](move-multiple-companies.md)
