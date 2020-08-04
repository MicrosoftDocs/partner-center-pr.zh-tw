---
title: 管理客戶帳戶中的使用者
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何為客戶建立使用者帳戶、新增或移除使用者授權、重設使用者密碼、刪除使用者帳戶，或將其還原。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527674"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a>合作夥伴中心內客戶帳戶的使用者管理工作

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員
- 使用者管理系統管理員
- 系統管理代理人
- 銷售代理人
- 技術服務代理人

您可以在客戶的帳戶中建立及刪除新的使用者。 您也可以還原在刪除後的30天內，您先前刪除的一個或多個使用者帳戶。 使用者先前的訂閱指派同樣會還原 (假設他們之前的配置可用)

當您為客戶購買新的訂用帳戶時，客戶應該會提供一份清單，列出所有需要帳戶的使用者、其使用者權限，以及每個使用者所需的服務。  

您可以使用 [與 Excel 相容的 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)來匯入名稱，一次[指派訂閱給多個使用者](bulk-license-provisioning-for-multiple-users.md)。

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>為客戶建立使用者帳戶

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 在客戶功能表中，選取 [使用者與授權]****。

4. 針對您新增的每個使用者，選取 **\[新增訂閱\]**，然後填入相關資訊 (包括權限和授權)。 [儲存] 變更。

5. 請務必記錄使用者名稱和暫時密碼，以傳送給使用者。

6. 如果您要以是一次加入一個的方式新增多個使用者，請使用 **\[新增其他使用者\]**。

7. 您也可以透過[匯入 Excel 相容 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)，一次新增多個使用者。 您可以等到新增一整組使用者之後，再從確認畫面以電子郵件傳送或直接列印這些名稱和密碼。

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>新增或移除客戶的使用者授權

下列步驟適用于新增或移除 Microsoft 產品的使用者授權。 若要在商業 marketplace 中新增或移除以授權為基礎的 SaaS 訂用帳戶的使用者授權，請參閱[新增或移除 SaaS 訂閱的授權](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 在客戶功能表中，選取 [使用者與授權]****。

4. 從清單中選擇一或多位使用者。 例如，如果客戶剛購買新的授權，而您想要將它們指派給尚未擁有的人員，您可以使用 [**篩選使用者依據**] 選項來尋找正確的群組。

5. 選取 [**管理授權**]。 進行變更，然後 [**儲存**]。

> [!NOTE]
> 針對[Azure Marketplace 產品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)，授權指派和啟用是透過發行產品的獨立軟體廠商（ISV）來管理。

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>為客戶重設使用者的密碼

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3.  在客戶功能表中，選取 [使用者與授權]****。 從清單中選擇使用者。

4.  在畫面底部，選取 [**重設密碼**]。 

5.  將新的暫時密碼傳送給使用者。

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>為客戶刪除使用者帳戶

1.  從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。 從清單中選擇客戶。

2.  在客戶功能表中，選取 [使用者與授權]****。 從清單中選擇使用者。

3.  在畫面底部，選取 [刪除使用者帳戶]****。

如果您需要還原此帳戶，您可以在 \[客戶\] 之 **\[使用者和授權\]** 清單的 **\[刪除的使用者\]** 索引標籤中找到該帳戶。 您有 30 天的期限可以還原刪除的使用者。

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>還原刪除的使用者帳戶

1.  從 [**合作夥伴中心**] 功能表選取 [**客戶**]，然後從清單中選擇客戶。

2.  選取 [**使用者和授權**]。

3.  選取 **\[刪除的使用者 ( )\]** 索引標籤，其中應該會顯示 **(1)**，如果有多個可還原的已刪除使用者，則顯示更大的數字。

4.  選取一或多個 [已刪除的使用者] 核取方塊，然後選取 [**還原**]。

    所有選取的使用者帳戶都會重新出現在 [**使用者和授權**] 頁面中。

## <a name="related-topics"></a>相關主題


[指派或撤銷多個使用者的授權](bulk-license-provisioning-for-multiple-users.md)

[為客戶帳戶建立多位使用者](adding-multiple-users-to-a-customer-account.md)