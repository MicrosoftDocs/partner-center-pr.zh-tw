---
title: 建立使用者帳戶和指派角色
description: 每位員工都必須先獲指派角色，然後才能存取合作夥伴中心。 了解如何建立使用者帳戶、指派角色，以及設定權限。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: c8fad4432f9aabba69877d80038ec9e2665c639d
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492529"
---
# <a name="create-user-accounts"></a>建立使用者帳戶  

**適當的角色**

- 帳戶管理員
- 全域系統管理員
- 使用者管理系統管理員

為需要存取合作夥伴中心的員工建立使用者帳戶。 這些工作必須由使用者管理系統管理員、帳戶系統管理員或全域系統管理員來完成。執行這些工作的使用者也必須獲派 Azure Active Directory (AAD) 的「使用者管理員」或「全域管理員」角色。 如需 AAD 角色的詳細資訊，請參閱 [Azure Active Directory 中的管理員角色權限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。

## <a name="add-a-new-user"></a>新增使用者

1. 從合作夥伴中心右上角的 [設定] 圖示中，選取 [帳戶設定]，接著再選取 [使用者管理]。

2. 選取 [新增使用者]。

3. 輸入使用者的全名和唯一電子郵件地址。

4. 選取您要指派給使用者的代理人類型及/或系統管理員類型。 合作夥伴中心存取權是以角色為基礎，讓您可以指派權限，自訂使用者檢視，只顯示使用者完成特定工作所需的功能。  若使用者想要角色指派，他們可以移至 [使用者管理] 並篩選全域系統管理員，找到要連絡的全域系統管理員。

5. 選取 [新增] 建立使用者帳戶。 在下一頁，確認使用者的詳細資料。

> [!IMPORTANT]  
> 記下此頁面上顯示的新使用者登入資訊。 請務必將這項資訊複製及傳送給新的使用者，因為稍後您將無法再次存取。 

使用者必須使用其使用者名稱和暫時密碼登入合作夥伴中心。 當使用者第一次登入合作夥伴中心時，系統會提示他們變更密碼。

## <a name="assign-user-roles"></a>指派使用者角色

若要在合作夥伴中心中工作，您必須具有指派的角色。  目前，這些角色包括 Azure Active Directory 租用戶角色、雲端解決方案提供者 (CSP) 角色，以及非 AAD 公司角色。 個別公司可能需要所有這些角色。

>[!Important]
>個人必須列示在您的租用戶中，才能存取合作夥伴中心。 角色指派會提供額外的存取權。

## <a name="next-steps"></a>後續步驟

- [為需要在合作夥伴中心工作的員工指派使用者角色和權限](permissions-overview.md)
