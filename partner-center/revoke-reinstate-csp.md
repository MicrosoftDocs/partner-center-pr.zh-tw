---
title: 恢復 Azure CSP 的管理員權限
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何協助客戶恢復合作夥伴的管理員權限，讓合作夥伴能夠協助管理客戶的 Azure CSP 訂用帳戶。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 362ae4a472b78417a4921b734a77f6259aaaa1f3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949259"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="4d787-103">恢復客戶的 Azure CSP 訂用帳戶管理員權限</span><span class="sxs-lookup"><span data-stu-id="4d787-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="4d787-104">**相關角色**</span><span class="sxs-lookup"><span data-stu-id="4d787-104">**Applicable roles**</span></span>

- <span data-ttu-id="4d787-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="4d787-105">Global admin</span></span>
- <span data-ttu-id="4d787-106">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="4d787-106">Admin agent</span></span>

<span data-ttu-id="4d787-107">身為 CSP 合作夥伴，您的客戶通常會預期您代為管理其 Azure 使用量及其系統。</span><span class="sxs-lookup"><span data-stu-id="4d787-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="4d787-108">您必須有管理員權限才能這樣做。</span><span class="sxs-lookup"><span data-stu-id="4d787-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="4d787-109">當您與客戶建立轉銷商關係時，部分許可權會授與這些權限。</span><span class="sxs-lookup"><span data-stu-id="4d787-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="4d787-110">其他權限則由您的客戶授與您。</span><span class="sxs-lookup"><span data-stu-id="4d787-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="4d787-111">CSP 中的 Azure 系統管理員許可權</span><span class="sxs-lookup"><span data-stu-id="4d787-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="4d787-112">CSP 中的 Azure 系統管理員許可權有兩種層級。</span><span class="sxs-lookup"><span data-stu-id="4d787-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="4d787-113">**租用戶層級系統管理員許可權** (**委派的系統管理員許可權**) - CSP 合作夥伴會在與客戶建立 CSP 轉銷商關係時取得這些許可權。</span><span class="sxs-lookup"><span data-stu-id="4d787-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="4d787-114">這可讓 CSP 合作夥伴存取其客戶的租用戶，讓他們能夠執行系統管理功能，例如新增/管理使用者、重設密碼，以及管理使用者授權。</span><span class="sxs-lookup"><span data-stu-id="4d787-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="4d787-115">**訂用帳戶層級系統管理員許可權** - CSP 合作夥伴在為其客戶建立 Azure CSP 訂用帳戶時會取得這些許可權。</span><span class="sxs-lookup"><span data-stu-id="4d787-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="4d787-116">擁有這些權限讓 CSP 合作夥伴可完整存取這些訂用帳戶，使他們能夠佈建及管理 Azure 資源。</span><span class="sxs-lookup"><span data-stu-id="4d787-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="4d787-117">恢復 CSP 合作夥伴的系統管理員許可權</span><span class="sxs-lookup"><span data-stu-id="4d787-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="4d787-118">若要重新取得委派的系統管理員許可權，您必須與您的客戶合作。</span><span class="sxs-lookup"><span data-stu-id="4d787-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="4d787-119">登入合作夥伴中心儀表板，然後從 [合作夥伴中心] 功能表中，選取 [客戶]。</span><span class="sxs-lookup"><span data-stu-id="4d787-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="4d787-120">選取您要合作的客戶，然後**要求轉銷商關係。**</span><span class="sxs-lookup"><span data-stu-id="4d787-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="4d787-121">這會產生連結，可連結到具有租用戶系統管理員權限的客戶。</span><span class="sxs-lookup"><span data-stu-id="4d787-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="4d787-122">該使用者必須選取連結，並核准轉銷商關係要求。</span><span class="sxs-lookup"><span data-stu-id="4d787-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="轉銷商關係":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="4d787-124">新增系統管理員代理程式群組，作為 Azure CSP 訂用帳戶的擁有者</span><span class="sxs-lookup"><span data-stu-id="4d787-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="4d787-125">您的客戶必須將您的系統管理員代理程式群組新增為 Azure CSP 訂用帳戶的擁有者。</span><span class="sxs-lookup"><span data-stu-id="4d787-125">Your customer will need to add your admin agent group as the owner of the Azure CSP subscription.</span></span>

1. <span data-ttu-id="4d787-126">請使用 PowerShell 主控台或 PowerShell 整合式腳本環境 (ISE)。</span><span class="sxs-lookup"><span data-stu-id="4d787-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="4d787-127">請確定已安裝 AzureRM 和 AzureAD 模組。</span><span class="sxs-lookup"><span data-stu-id="4d787-127">Ensure that AzureRM and AzureAD modules are installed.</span></span>

2. <span data-ttu-id="4d787-128">連線到您的 Azure AD 租用戶。</span><span class="sxs-lookup"><span data-stu-id="4d787-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="4d787-129">取得系統管理員代理程式群組的 ObjectId。</span><span class="sxs-lookup"><span data-stu-id="4d787-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```

   :::image type="content" source="images/azure/revoke5.png" alt-text="系統管理代理人群組":::

   <span data-ttu-id="4d787-131">下列步驟是由您客戶公司中的使用者所執行，這些使用者具有 Azure CSP 訂用帳戶擁有者存取權。</span><span class="sxs-lookup"><span data-stu-id="4d787-131">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="4d787-132">具有 Azure CSP 訂用帳戶擁有者存取權的使用者，會使用自己的認證登入 Azure Resource Manager。</span><span class="sxs-lookup"><span data-stu-id="4d787-132">The user with owner access to the Azure CSP subscription,signs in to Azure Resource Manager using her credentials.</span></span>

   ```powershell
   Login-AzureRMAccount
   ```

5. <span data-ttu-id="4d787-133">然後，她可以新增您的系統管理員代理程式群組，作為 CSP Azure 訂用帳戶的擁有者。</span><span class="sxs-lookup"><span data-stu-id="4d787-133">She can then add your admin agent group as owner to the CSP Azure subscription.</span></span>

    ```powershell
    New-AzureRMRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

   :::image type="content" source="images/azure/revoke6.png" alt-text="系統管理代理人擁有者":::

## <a name="next-steps"></a><span data-ttu-id="4d787-135">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="4d787-135">Next steps</span></span>

[<span data-ttu-id="4d787-136">管理 Azure 方案下的訂用帳戶和資源</span><span class="sxs-lookup"><span data-stu-id="4d787-136">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
