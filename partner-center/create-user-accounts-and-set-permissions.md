---
title: 建立使用者帳戶和指派角色
description: 每位員工都必須先獲指派角色，然後才能存取合作夥伴中心。 了解如何建立使用者帳戶、指派角色，以及設定權限。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 角色, 權限, 新增使用者, 指派角色, 系統管理員, 代理人,
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 8d738e9231959e7d156a053fa1ac28ccfc219547
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394199"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="bf458-105">建立使用者帳戶以及指派角色和權限</span><span class="sxs-lookup"><span data-stu-id="bf458-105">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="bf458-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="bf458-106">**Appropriate roles**</span></span>

- <span data-ttu-id="bf458-107">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-107">Account admin</span></span>
- <span data-ttu-id="bf458-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-108">Global admin</span></span>
- <span data-ttu-id="bf458-109">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-109">User management admin</span></span>

<span data-ttu-id="bf458-110">為需要存取合作夥伴中心的員工建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="bf458-110">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="bf458-111">這些工作必須由使用者管理系統管理員、帳戶系統管理員或全域系統管理員來完成。執行這些工作的使用者也必須獲派 Azure Active Directory (AAD) 的「使用者管理員」或「全域管理員」角色。</span><span class="sxs-lookup"><span data-stu-id="bf458-111">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="bf458-112">如需 AAD 角色的詳細資訊，請參閱 [Azure Active Directory 中的管理員角色權限](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="bf458-112">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="bf458-113">新增使用者</span><span class="sxs-lookup"><span data-stu-id="bf458-113">Add a new user</span></span>

1. <span data-ttu-id="bf458-114">從合作夥伴中心右上角的 [設定] 圖示中，選取 [使用者管理]。</span><span class="sxs-lookup"><span data-stu-id="bf458-114">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="bf458-115">選取 [新增使用者]。</span><span class="sxs-lookup"><span data-stu-id="bf458-115">Select **Add user**.</span></span>

3. <span data-ttu-id="bf458-116">輸入使用者的全名和唯一電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="bf458-116">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="bf458-117">選取您要指派給使用者的代理人類型及/或系統管理員類型。</span><span class="sxs-lookup"><span data-stu-id="bf458-117">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="bf458-118">合作夥伴中心存取權是以角色為基礎，讓您可以指派權限，自訂使用者檢視，只顯示使用者完成特定工作所需的功能。</span><span class="sxs-lookup"><span data-stu-id="bf458-118">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="bf458-119">若使用者想要角色指派，他們可以移至 [使用者管理] 並篩選全域系統管理員，找到要連絡的全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="bf458-119">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="bf458-120">選取 [新增] 建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="bf458-120">Select **Add** to create the user account.</span></span> <span data-ttu-id="bf458-121">在下一頁，確認使用者的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="bf458-121">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="bf458-122">記下此頁面上顯示的新使用者登入資訊。</span><span class="sxs-lookup"><span data-stu-id="bf458-122">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="bf458-123">請務必將這項資訊複製及傳送給新的使用者，因為稍後您將無法再次存取。</span><span class="sxs-lookup"><span data-stu-id="bf458-123">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="bf458-124">使用者必須使用其使用者名稱和暫時密碼登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="bf458-124">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="bf458-125">當使用者第一次登入合作夥伴中心時，系統會提示他們變更密碼。</span><span class="sxs-lookup"><span data-stu-id="bf458-125">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="bf458-126">尋找您的全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-126">Find your global admin</span></span>

<span data-ttu-id="bf458-127">有時候使用者可能需要變更其角色，或者新的使用者可能想要特定的角色指派。</span><span class="sxs-lookup"><span data-stu-id="bf458-127">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="bf458-128">若要尋找可進行角色變更或將角色指派給新使用者的全域系統管理員，請從合作夥伴中心右上角的 [設定] 圖示中選取 [使用者管理]，然後篩選全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="bf458-128">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="bf458-129">新的全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-129">New global admin</span></span>

<span data-ttu-id="bf458-130">如果您的全域系統管理員離開組織，而需要其他人擔任此角色，則可以將票證提交給 Azure 或 Office 365 小組。</span><span class="sxs-lookup"><span data-stu-id="bf458-130">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="bf458-131">如需執行這項操作的相關資訊，請選取下列其中一個選項。</span><span class="sxs-lookup"><span data-stu-id="bf458-131">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="bf458-132">新的 Azure 全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-132">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="bf458-133">新的 Office 365 全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-133">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="bf458-134">指派使用者角色</span><span class="sxs-lookup"><span data-stu-id="bf458-134">Assign user roles</span></span>

<span data-ttu-id="bf458-135">若要在合作夥伴中心中工作，您必須具有指派的角色。</span><span class="sxs-lookup"><span data-stu-id="bf458-135">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="bf458-136">目前，這些角色包括 Azure Active Directory 租用戶角色、雲端解決方案提供者 (CSP) 角色，以及非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="bf458-136">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="bf458-137">個別公司可能需要所有這些角色。</span><span class="sxs-lookup"><span data-stu-id="bf458-137">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="bf458-138">個人必須列示在您的租用戶中，才能存取合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="bf458-138">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="bf458-139">角色指派會提供額外的存取權。</span><span class="sxs-lookup"><span data-stu-id="bf458-139">Role assignments provide additional access.</span></span>


<span data-ttu-id="bf458-140">**AAD 租用戶角色包括**：</span><span class="sxs-lookup"><span data-stu-id="bf458-140">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="bf458-141">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-141">Global admin</span></span>
- <span data-ttu-id="bf458-142">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-142">User admin</span></span>

<span data-ttu-id="bf458-143">**CSP 角色包括**：</span><span class="sxs-lookup"><span data-stu-id="bf458-143">**CSP roles include**:</span></span>
- <span data-ttu-id="bf458-144">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="bf458-144">Admin agent</span></span>
- <span data-ttu-id="bf458-145">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-145">Billing admin</span></span>
- <span data-ttu-id="bf458-146">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="bf458-146">Sales agent</span></span>
- <span data-ttu-id="bf458-147">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="bf458-147">Helpdesk agent</span></span>

<span data-ttu-id="bf458-148">**管理 MPN 會員資格和公司 (非 AAD) 的角色**</span><span class="sxs-lookup"><span data-stu-id="bf458-148">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="bf458-149">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-149">MPN partner admin</span></span>
- <span data-ttu-id="bf458-150">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-150">Account admin</span></span>
- <span data-ttu-id="bf458-151">推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-151">Referral admin</span></span>
- <span data-ttu-id="bf458-152">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-152">Business profile admin</span></span>
- <span data-ttu-id="bf458-153">獎勵系統管理員和使用者</span><span class="sxs-lookup"><span data-stu-id="bf458-153">Incentives admin and user</span></span>

<span data-ttu-id="bf458-154">**控制台廠商是 CSP 和非 AAD 角色**。</span><span class="sxs-lookup"><span data-stu-id="bf458-154">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="bf458-155">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bf458-155">Global admin</span></span>

<span data-ttu-id="bf458-156">**來賓使用者**必須是 AAD 租用戶的一部分，而且可以具有任何非 AAD 角色。</span><span class="sxs-lookup"><span data-stu-id="bf458-156">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="bf458-157">如需角色的特定資訊以及每個角色可以執行哪些任務的相關資訊，請參閱[指派使用者權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="bf458-157">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="bf458-158">關聯使用者在合作夥伴中心的 Microsoft Learn 帳戶</span><span class="sxs-lookup"><span data-stu-id="bf458-158">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="bf458-159">為了能夠看到您的使用者對專長認證所採取的訓練和學習路徑，他們必須將其 MCP 識別碼關聯至其合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="bf458-159">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="bf458-160">身為全域系統管理員，當您新增使用者時，請務必提醒他們將其 MCP 識別碼關聯至其帳戶。</span><span class="sxs-lookup"><span data-stu-id="bf458-160">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="bf458-161">如何將您的 MCP 識別碼關聯至您的合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="bf458-161">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="bf458-162">從合作夥伴中心儀表板，選取儀表板右上角的 [您的帳戶] 圖示，然後選取 [我的設定檔]。</span><span class="sxs-lookup"><span data-stu-id="bf458-162">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="bf458-163">在 [您的學習] 之下，您將能夠關聯 Microsoft Learning 帳戶，也可以將您的 Microsoft 帳戶連線到 Partner University。</span><span class="sxs-lookup"><span data-stu-id="bf458-163">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>
