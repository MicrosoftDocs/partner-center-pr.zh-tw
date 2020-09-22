---
title: 如果您 MPN 程式的唯一系統管理員已離開公司，該怎麼辦？
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何尋找新的 MPN 系統管理員，或從貴公司的全域管理員取得協助。此外，請瞭解如何新增合作夥伴中心全域管理員。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03cd603cf65b1e999cf95fd10d76e6ccc6c403e8
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999332"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>如果您 MPN 程式的唯一系統管理員已離開公司，該怎麼辦？

**適用於**

- 合作夥伴中心

下列文章將逐步引導您瞭解 MPN 系統管理員已離開公司時，該怎麼辦的三個一般案例。

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>案例1： MPN 合作夥伴系統管理員/帳戶管理員已離開公司，但帳戶中仍有全域管理員

在此情況下，公司中的另一個人可以被指派 MPN Partner admin 的角色。指派特定 MPN 夥伴系統管理員/帳戶管理員角色的角色：

1. 使用您的工作帳戶登入合作夥伴中心帳戶 (例如 tom@contoso.com) 。
1. 從全域管理員的 [ **使用者管理** ] 頁面篩選，查看貴公司的全域管理員是誰。 
1. 洽詢其中一個全域管理員，並要求他們將您需要的 MPN 專屬角色指派給您。 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>案例2： MPN 合作夥伴系統管理員/帳戶管理員已離開公司，且帳戶中沒有全域管理員 

如果您移至 [ **使用者管理** ] 頁面並篩選 [全域管理員]，但您發現公司中沒有可協助您取得 MPN 特定角色的全域管理員，請遵循下列步驟：

1. 移至 [portal.azure.com](https://ms.portal.azure.com/)，使用您的工作帳戶登入 (例如 tom@contoso.com) 。 
1. 選取左側功能表導覽列中的 [說明 **+ 支援** ] 選項。
1. 在下一個頁面上，選取下拉式選單中的 [ **新增支援要求** 和 **技術問題** 類型]，插入任何其他詳細資料，然後按 **[下一步：方案]。**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="在 Azure 入口網站中找出系統管理員":::

4. 在下一個頁面中查看建議的解決方案之後，請選取 [ **下一步：詳細資料]** 並完成必要的欄位。
1. 複習並建立支援要求。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>案例3： MPN 合作夥伴系統管理員/帳戶管理員/全域管理員已離開公司，且沒有任何其他使用者可以存取公司的 Azure AD。 這是完全遺失的存取權。

遵循 [系統管理員接管](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) 步驟，以 Azure Active Directory 系統管理員身分接管非受控目錄。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>不確定您的公司是否已經有工作帳戶？

如果不確定您的公司是否有工作帳戶，請依照下列步驟檢查。

1. 登入 Azure 系統 [管理員入口網站](https://ms.portal.azure.com)。
2. 從左側功能表中選取 **Azure Active Directory** ，然後選取 [ **功能變數名稱**]。
如果您已經有工作帳戶，將會列出您的網域名稱。

>[!Note]
>如果您有 Microsoft Azure 或 Office 365 的有效訂用帳戶，則您已經有工作帳戶，且您的登入認證應該與用來存取這些服務的認證相同。