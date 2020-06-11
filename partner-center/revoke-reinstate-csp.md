---
title: 恢復 Azure CSP 的管理員權限
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何協助客戶恢復合作夥伴的管理員權限，讓合作夥伴能夠協助管理客戶的 Azure CSP 訂用帳戶。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3bb1f5daf1582c4ca4a67c2813d598567db17f13
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467248"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>恢復客戶的 Azure CSP 訂用帳戶管理員權限  

**相關角色**

- 全域系統管理員
- 系統管理代理人

身為 CSP 合作夥伴，您的客戶通常會預期您代為管理其 Azure 使用量及其系統。 您必須有管理員權限才能這樣做。 當您與客戶建立轉銷商關係時，部分許可權會授與這些權限。 其他權限則由您的客戶授與您。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 中的 Azure 系統管理員許可權

CSP 中的 Azure 系統管理員許可權有兩種層級。

**租用戶層級系統管理員許可權** (**委派的系統管理員許可權**) - CSP 合作夥伴會在與客戶建立 CSP 轉銷商關係時取得這些許可權。 這可讓 CSP 合作夥伴存取其客戶的租用戶，讓他們能夠執行系統管理功能，例如新增/管理使用者、重設密碼，以及管理使用者授權。

**訂用帳戶層級系統管理員許可權** - CSP 合作夥伴在為其客戶建立 Azure CSP 訂用帳戶時會取得這些許可權。 擁有這些權限讓 CSP 合作夥伴可完整存取這些訂用帳戶，使他們能夠佈建及管理 Azure 資源。

## <a name="reinstate-csp-partners-admin-privileges"></a>恢復 CSP 合作夥伴的系統管理員許可權

若要重新取得委派的系統管理員許可權，您必須與您的客戶合作。

1. 登入合作夥伴中心儀表板，然後從 [合作夥伴中心] 功能表中，選取 [客戶]。

2. 選取您要合作的客戶，然後**要求轉銷商關係。** 這會產生連結，可連結到具有租用戶系統管理員權限的客戶。

3. 該使用者必須選取連結，並核准轉銷商關係要求。

   :::image type="content" source="images/azure/revoke4.png" alt-text="轉銷商關係":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>新增系統管理員代理程式群組，作為 Azure CSP 訂用帳戶的擁有者

您的客戶必須將您的系統管理員代理程式群組新增為 Azure CSP 訂用帳戶的擁有者。

1. 請使用 PowerShell 主控台或 PowerShell 整合式腳本環境 (ISE)。 請確定已安裝 AzureRM 和 AzureAD 模組。

2. 連線到您的 Azure AD 租用戶。

   ```powershell
   Connect-AzureAD
   ```

3. 取得系統管理員代理程式群組的 ObjectId。

   ```powershell
   Get-AzureADGroup
   ```

   :::image type="content" source="images/azure/revoke5.png" alt-text="系統管理代理人群組":::

   下列步驟是由您客戶公司中的使用者所執行，這些使用者具有 Azure CSP 訂用帳戶擁有者存取權。

4. 具有 Azure CSP 訂用帳戶擁有者存取權的使用者，會使用自己的認證登入 Azure Resource Manager。

   ```powershell
   Login-AzureRMAccount
   ```

5. 然後，她可以新增您的系統管理員代理程式群組，作為 CSP Azure 訂用帳戶的擁有者。

    ```powershell
    New-AzureRMRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

   :::image type="content" source="images/azure/revoke6.png" alt-text="系統管理代理人擁有者":::

## <a name="next-steps"></a>接下來的步驟

[管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)
