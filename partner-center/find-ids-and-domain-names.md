---
title: 尋找租使用者識別碼、功能變數名稱、使用者物件識別碼
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在 Azure 入口網站中尋找識別碼-組織的 Azure AD 租使用者識別碼、功能變數名稱或特定的使用者物件識別碼。 某些工作需要此資訊。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/17/2020
ms.locfileid: "90740387"
---
# <a name="locate-important-ids-for-a-user"></a>找出使用者的重要識別碼

本文說明如何使用 [Azure 入口網站](https://portal.azure.com/) 來尋找使用者的下列資訊：

- 使用者組織或公司的 Microsoft Azure Active Directory (Azure AD) 租使用者識別碼

- 與 Azure AD 租使用者相關聯之組織或公司的主功能變數名稱稱

- 使用者物件識別碼

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>尋找 Microsoft Azure AD 租使用者識別碼和主功能變數名稱稱

請遵循下列步驟，找出 Azure 入口網站內 Azure AD 的租使用者識別碼或主功能變數名稱稱。

> [!NOTE]
> 租使用者識別碼可能會在不同的應用程式或資源中被稱為不同的名稱。 例如，租使用者識別碼可以稱為「目錄識別碼」、「Azure Active Directory (Azure AD) 租使用者、Microsoft ID 或某些報表（甚至是 *tenantguid*）。

1. 登入 [Azure 入口網站](https://portal.azure.com/)。

2. 從功能表中選取 [Azure Active Directory]。

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="顯示 Azure 入口網站從功能表選取 Azure Active Directory 選項。":::

3. Azure Active Directory **總覽** ] 頁面隨即出現。 若要尋找 Azure AD 租使用者識別碼或主功能變數名稱稱，請尋找 [ **租使用者識別碼** ] 欄位和 [ **主網域** ] 欄位。 這些欄位會出現在 [租使用者資訊] 區段中。

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="顯示具有兩個醒目提示欄位、租使用者識別碼和主功能變數名稱稱的 [總覽] 頁面。":::

4. 您可以使用一些其他方式，在 Azure 入口網站中尋找租使用者識別碼。 從功能表中選取 [Azure Active Directory]。 然後，找出功能表上的 [ **管理** ] 區段，然後選取 [ **屬性**]。

   [屬性] 頁面也會顯示使用者相關聯的租使用者識別碼。

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="顯示具有反白顯示 [租使用者識別碼] 欄位的屬性頁面。":::

## <a name="find-the-user-object-id"></a>尋找使用者物件識別碼

找不到功能變數名稱和租使用者識別碼，可能不一定就足夠了。 您可能也需要找出指派給使用者的特定物件識別碼。 依照下列步驟，在 Azure 入口網站中尋找使用者的物件識別碼：

1. 登入 [Azure 入口網站](https://portal.azure.com/)。

2. 從功能表中選取 [Azure Active Directory]。

3. 找出功能表上的 [ **管理** ] 區段，然後選取 [ **使用者**]。

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="顯示 Azure Active Directory 功能表，並醒目提示 [使用者] 選項。":::

4. 在 [使用者] 頁面的 [搜尋] 方塊中，輸入使用者的名稱。

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="顯示具有搜尋方塊的使用者頁面，以搜尋特定使用者。":::

5. 選取使用者在清單中顯示的名稱。  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="顯示使用者頁面，其中顯示搜尋使用者的資料列。":::

6. 在使用者的設定檔頁面面上找出身分識別區段。 [物件識別碼] 欄位會出現在這裡，並顯示使用者的唯一物件識別碼。

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="顯示 [使用者設定檔] 頁面上的 [身分識別] 區段和一個醒目提示的物件識別碼欄位。":::

## <a name="next-steps"></a>後續步驟

- [深入瞭解 Azure Active Directory 中的使用者設定檔](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [瞭解合作夥伴可如何在合作夥伴中心中查看或匯出客戶詳細資料](see-your-customer-list.md)