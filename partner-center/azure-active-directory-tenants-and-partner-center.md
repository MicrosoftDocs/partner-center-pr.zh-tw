---
title: 工作帳戶與合作夥伴中心
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解若要建立合作夥伴中心帳戶，就必須有工作帳戶。 檢查您是否已經有工作帳戶。
author: LauraBrenner
ms.author: labrenne
Keywords: 工作帳戶, 電子郵件, 租用戶, Azure 租用戶, 建立帳戶, 網域名稱
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: e34eecb482df140a1a225d0d28460ef957701d59
ms.sourcegitcommit: af3ecd7f35e5bb3b87f5f683335c76e287f2a9b8
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/13/2020
ms.locfileid: "83369265"
---
# <a name="your-company-work-account-and-partner-center"></a>您的公司工作帳戶與合作夥伴中心  

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員
- 使用者管理系統管理員

## <a name="why-you-need-a-work-account"></a>您必須有工作帳戶的原因

Microsoft 會要求您將公司的工作帳戶連結到新的合作夥伴中心帳戶。 此連結可讓您的帳戶使用者利用其工作帳戶使用者名稱和密碼來登入合作夥伴中心。

## <a name="the-work-account-email-address"></a>工作帳戶電子郵件地址

您的工作帳戶或工作電子郵件是貴公司提供給您的電子郵件地址。 工作帳戶電子郵件的格式通常為 `you@yourcompany.com`。 個人電子郵件地址 (例如 Hotmail、Gmail 或 Yahoo 等等) 不是工作電子郵件，因此無法用於您的合作夥伴中心帳戶。

如果您有多個有效的工作電子郵件地址，請使用與貴公司總部而不是地區部門相關聯的工作電子郵件地址，例如，使用您的 `contoso.com` 電子郵件，而不是 `contoso.uk` 地址。

> [!NOTE]  
> 決定使用現有的工作帳戶之前，請先考慮帳戶中有多少使用者需要使用合作夥伴中心。 如果帳戶中有不需要使用合作夥伴中心的使用者，請考慮只為那些需要使用合作夥伴中心的使用者建立新帳戶。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>不確定您的公司是否已經有工作帳戶？

如果不確定您的公司是否有工作帳戶，請依照下列步驟檢查。 如果您有使用中的 Microsoft Azure 或 Office 365 訂用帳戶，就已經擁有工作帳戶。

1. 登入 [Azure 入口網站](https://portal.azure.com)

2. 從功能表選取 [Azure Active Directory]，然後選取 [網域名稱]。

3. 如果您已經有工作帳戶，將會列出您的網域名稱。

如果貴公司還沒有工作帳戶，您可以在註冊過程中建立一個帳戶。

下圖提供數個一般案例的步驟：

- 判斷您是否有工作帳戶
- 判斷如何登入您的工作帳戶
- 判斷您是否需要建立新的工作帳戶

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="您有工作帳戶嗎？還是您需要建立一個工作帳戶？":::

如需關於在 Azure AD 中新增網域的詳細資訊，請參閱[在 Azure AD 中新增網域或建立網域關聯](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>關於 Microsoft Azure

Microsoft Azure 是一個公用雲端平台，公司可以用來在 Microsoft 管理的資料中心全球網路上建置、部署和管理應用程式。 公司會利用 Azure，透過虛擬功能或服務 (而不是實體機器) 來建置虛擬 IT 基礎結構。

當您購買 Azure 訂用帳戶時，基本上就是在租借 Azure 公用雲端的專用安全空間，這跟您租用辦公大樓的場地來經營公司的實體業務沒有太大區別。 相對於辦公大樓的擁有者，您的公司就是租用戶。

Azure 工作帳戶是您公司在 Azure 公用雲端的專用且隔離的虛擬表示，這已在您訂閱 Microsoft 雲端服務 (例如 Azure、Microsoft Intune 或 Office 365) 時建立。

您的工作帳戶會裝載 Azure AD 的使用者和他們的相關資訊 (密碼、設定檔資料、權限等等)。 公司帳戶也包含群組、應用程式，以及其他有關公司與其安全性的資訊。
