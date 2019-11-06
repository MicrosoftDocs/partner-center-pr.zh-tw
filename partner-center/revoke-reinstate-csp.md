---
title: 恢復 Azure CSP 訂用帳戶的系統管理員權限 | 合作夥伴中心
ms.topic: article
ms.date: 10/15/2019
description: 本檔案說明如何協助客戶恢復合作夥伴的系統管理員許可權
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 51f19724751b296789a1d5367d9892b21cab4f09
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/01/2019
ms.locfileid: "73433744"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>恢復 Azure CSP 訂用帳戶的系統管理員權限  

**相關角色**

- 全域系統管理員
- 系統管理代理人

身為 CSP 合作夥伴，您的客戶通常會預期您代為管理其 Azure 使用量及其系統。 若要這麼做，您必須擁有系統管理員許可權。 當您與客戶建立轉銷商關係時，部分許可權會授與這些權限。 其他權限則由您的客戶授與您。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP 中的 Azure 系統管理員許可權 

CSP 中的 Azure 系統管理員許可權有兩種層級。 

**租用戶層級系統管理員許可權** (**委派的系統管理員許可權**) – CSP 合作夥伴會在與客戶建立 CSP 轉銷商關係時取得這些許可權。 這可讓 CSP 合作夥伴存取其客戶的租用戶，讓他們能夠執行系統管理功能，例如新增/管理使用者、重設密碼，以及管理使用者授權。 

**訂用帳戶層級系統管理員許可權** – CSP 合作夥伴在為其客戶建立 Azure CSP 訂用帳戶時會取得這些許可權。 這可讓 CSP 合作夥伴完成這些訂用帳戶的存取權，讓他們能夠佈建及管理 Azure 資源。 


## <a name="reinstate-csp-partners-admin-privileges"></a>恢復 CSP 合作夥伴的系統管理員許可權

若要重新取得委派的系統管理員許可權，您必須與您的客戶合作。
 
 1. 登入合作夥伴中心儀表板，然後從 [合作夥伴中心] 功能表中，選取 [客戶]  。

 2. 選取您要合作的客戶，然後**要求轉銷商關係。** 這會產生連結，可連結到具有租用戶系統管理員權限的客戶。

 3. 該使用者必須選取連結，並核准轉銷商關係要求。
 
![轉銷商關係](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>新增系統管理員代理程式群組，作為 Azure CSP 訂用帳戶的擁有者

 您的客戶必須將您的系統管理員代理程式群組新增為 Azure CSP 訂用帳戶的擁有者。

1. 請使用 PowerShell 主控台或 PowerShell 整合式腳本環境 (ISE)。 請確定已安裝 AzureRM 和 AzureAD 模組。 

2.  連線到您的 Azure AD 租用戶。
PowerShell Cmdlet：Connect-AzureAD

3.  取得系統管理員代理程式群組的 ObjectId。
PowerShell Cmdlet：Get-AzureADGroup`1nn

![系統管理員代理程式群組](images/azure/revoke5.png)

下列步驟是由您客戶公司中的使用者所執行，這些使用者具有 Azure CSP 訂用帳戶擁有者存取權。

4. 具有 Azure CSP 訂用帳戶擁有者存取權的使用者，會使用自己的認證登入 Azure Resource Manager。

    PowerShell Cmdlet：Login-AzureRMAccount

5.  然後，她可以新增您的系統管理員代理程式群組，作為 CSP Azure 訂用帳戶的擁有者。

    PowerShell Cmdlet：New-AzureRMRoleAssignment -ObjectId <您在步驟 3 中取得的物件識別碼> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![系統管理員代理程式群組](images/azure/revoke6.png)    

**詳細資訊**

[管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)
