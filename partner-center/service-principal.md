---
title: Azure AD 服務主體
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何將服務主體新增至您的 Azure AD 租用戶。 這樣做就等於在合作夥伴中心新增 Azure AD 應用程式 (服務主體)。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2020
ms.locfileid: "87811238"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>在合作夥伴中心新增 Azure AD 應用程式 (服務主體)

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員

在合作夥伴中心的商務 Marketplace 計畫中，您現在可以將 Azure AD 應用程式 (服務主體) 新增為合作夥伴中心帳戶中的使用者。 (先前，您可以在 Cloud Partner 入口網站或 CPP 帳戶中這麼做。 但現在您已移轉至合作夥伴中心，所以 CPP 帳戶為唯讀狀態。)
 
>[!Note] 
>服務主體與 Azure AD 應用程式是同義。

## <a name="add-an-azure-ad-application-service-principal"></a>新增 Azure AD 應用程式 (服務主體)

1. 在合作夥伴中心儀表板，選取 [設定]，然後選取 [開發人員設定]。

2. 選取 [使用者]，然後選取 [新增 Azure AD 應用程式]。

3. 選取現有的 Azure AD 應用程式，或建立新的應用程式。

4. 如果建立新的 Azure AD 應用程式，請包含下列資訊：  

   - **回覆 URL**：使用者用於登入以使用您 Azure AD 應用程式的 URL。

   - **應用程式識別碼 URI**：Azure AD 應用程式的邏輯識別碼，會在向 Azure AD 傳送單一登入要求時顯示。

   - **安全性角色**：**管理員** (與 CPP 中的「擁有者」角色相同) 和**開發人員** (與 CPP 中的「參與者」角色相同) 角色適用於合作夥伴中心內的商務 Marketplace 計畫，而且可與此 Azure AD 應用程式相關聯。  

## <a name="next-steps"></a>接下來的步驟

- [合作夥伴中心的商業市場概觀](csp-commercial-marketplace-overview.md)