---
title: 建立使用者帳戶和指派角色
description: 每位員工都必須先獲指派角色，然後才能存取合作夥伴中心。 了解如何建立使用者帳戶、指派角色，以及設定權限。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: cfd681a56bfaebcc1fd6c77de3e5a0c6deb4a46f
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527734"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a><span data-ttu-id="3d6c1-104">建立使用者帳戶以及指派角色和權限</span><span class="sxs-lookup"><span data-stu-id="3d6c1-104">Create user accounts and assign roles and permissions</span></span>

<span data-ttu-id="3d6c1-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="3d6c1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="3d6c1-106">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-106">Account admin</span></span>
- <span data-ttu-id="3d6c1-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-107">Global admin</span></span>
- <span data-ttu-id="3d6c1-108">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-108">User management admin</span></span>

<span data-ttu-id="3d6c1-109">為需要存取合作夥伴中心的員工建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="3d6c1-110">這些工作必須由使用者管理系統管理員、帳戶系統管理員或全域系統管理員來完成。執行這些工作的使用者也必須獲派 Azure Active Directory (AAD) 的「使用者管理員」或「全域管理員」角色。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="3d6c1-111">如需 AAD 角色的詳細資訊，請參閱 [Azure Active Directory 中的管理員角色權限](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>


## <a name="add-a-new-user"></a><span data-ttu-id="3d6c1-112">新增使用者</span><span class="sxs-lookup"><span data-stu-id="3d6c1-112">Add a new user</span></span>

1. <span data-ttu-id="3d6c1-113">從合作夥伴中心右上角的 [設定] 圖示中，選取 [使用者管理]。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-113">From the **Settings** icon at the top right of the Partner Center, select **User management**.</span></span>

2. <span data-ttu-id="3d6c1-114">選取 [新增使用者]。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-114">Select **Add user**.</span></span>

3. <span data-ttu-id="3d6c1-115">輸入使用者的全名和唯一電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="3d6c1-116">選取您要指派給使用者的代理人類型及/或系統管理員類型。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="3d6c1-117">合作夥伴中心存取權是以角色為基礎，讓您可以指派權限，自訂使用者檢視，只顯示使用者完成特定工作所需的功能。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="3d6c1-118">若使用者想要角色指派，他們可以移至 [使用者管理] 並篩選全域系統管理員，找到要連絡的全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="3d6c1-119">選取 [新增] 建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="3d6c1-120">在下一頁，確認使用者的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="3d6c1-121">記下此頁面上顯示的新使用者登入資訊。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="3d6c1-122">請務必將這項資訊複製及傳送給新的使用者，因為稍後您將無法再次存取。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 


<span data-ttu-id="3d6c1-123">使用者必須使用其使用者名稱和暫時密碼登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="3d6c1-124">當使用者第一次登入合作夥伴中心時，系統會提示他們變更密碼。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span> 


### <a name="find-your-global-admin"></a><span data-ttu-id="3d6c1-125">尋找您的全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-125">Find your global admin</span></span>

<span data-ttu-id="3d6c1-126">有時候使用者可能需要變更其角色，或者新的使用者可能想要特定的角色指派。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-126">Sometimes a user might need to have their role changed or a new user may want a specific role assignment.</span></span>  
<span data-ttu-id="3d6c1-127">若要尋找可進行角色變更或將角色指派給新使用者的全域系統管理員，請從合作夥伴中心右上角的 [設定] 圖示中選取 [使用者管理]，然後篩選全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-127">To find a global admin who can make role changes or assign roles to a new user, from the **Settings icon** at the top right of the Partner Center, select **User management** and filter on global admin.</span></span> 


### <a name="new-global-admin"></a><span data-ttu-id="3d6c1-128">新的全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-128">New global admin</span></span>

<span data-ttu-id="3d6c1-129">如果您的全域系統管理員離開組織，而需要其他人擔任此角色，則可以將票證提交給 Azure 或 Office 365 小組。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-129">If your global admin leaves the organization and someone else needs to fill this role, you can submit a ticket to either the Azure or Office 365 team.</span></span> <span data-ttu-id="3d6c1-130">如需執行這項操作的相關資訊，請選取下列其中一個選項。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-130">For information on how to do this, select one of the options below.</span></span>

[<span data-ttu-id="3d6c1-131">新的 Azure 全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-131">New global admin for Azure</span></span>](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[<span data-ttu-id="3d6c1-132">新的 Office 365 全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-132">New global admin for Office 365</span></span>](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a><span data-ttu-id="3d6c1-133">指派使用者角色</span><span class="sxs-lookup"><span data-stu-id="3d6c1-133">Assign user roles</span></span>

<span data-ttu-id="3d6c1-134">若要在合作夥伴中心中工作，您必須具有指派的角色。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-134">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="3d6c1-135">目前，這些角色包括 Azure Active Directory 租用戶角色、雲端解決方案提供者 (CSP) 角色，以及非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-135">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="3d6c1-136">個別公司可能需要所有這些角色。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-136">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="3d6c1-137">個人必須列示在您的租用戶中，才能存取合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-137">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="3d6c1-138">角色指派會提供額外的存取權。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-138">Role assignments provide additional access.</span></span>


<span data-ttu-id="3d6c1-139">**AAD 租用戶角色包括**：</span><span class="sxs-lookup"><span data-stu-id="3d6c1-139">**AAD tenant roles include**:</span></span>
- <span data-ttu-id="3d6c1-140">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-140">Global admin</span></span>
- <span data-ttu-id="3d6c1-141">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-141">User admin</span></span>

<span data-ttu-id="3d6c1-142">**CSP 角色包括**：</span><span class="sxs-lookup"><span data-stu-id="3d6c1-142">**CSP roles include**:</span></span>
- <span data-ttu-id="3d6c1-143">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="3d6c1-143">Admin agent</span></span>
- <span data-ttu-id="3d6c1-144">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-144">Billing admin</span></span>
- <span data-ttu-id="3d6c1-145">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="3d6c1-145">Sales agent</span></span>
- <span data-ttu-id="3d6c1-146">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="3d6c1-146">Helpdesk agent</span></span>

<span data-ttu-id="3d6c1-147">**管理 MPN 會員資格和公司 (非 AAD) 的角色**</span><span class="sxs-lookup"><span data-stu-id="3d6c1-147">**Roles that manage the MPN membership and the company (Non-AAD)**</span></span>
- <span data-ttu-id="3d6c1-148">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-148">MPN partner admin</span></span>
- <span data-ttu-id="3d6c1-149">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-149">Account admin</span></span>
- <span data-ttu-id="3d6c1-150">推薦系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-150">Referral admin</span></span>
- <span data-ttu-id="3d6c1-151">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-151">Business profile admin</span></span>
- <span data-ttu-id="3d6c1-152">獎勵系統管理員和使用者</span><span class="sxs-lookup"><span data-stu-id="3d6c1-152">Incentives admin and user</span></span>

<span data-ttu-id="3d6c1-153">**控制台廠商是 CSP 和非 AAD 角色**。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-153">**Control Panel Vendor is a CSP and non-AAD role**.</span></span>
- <span data-ttu-id="3d6c1-154">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="3d6c1-154">Global admin</span></span>

<span data-ttu-id="3d6c1-155">**來賓使用者**必須是 AAD 租用戶的一部分，而且可以具有任何非 AAD 角色。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-155">**Guest user** must be part of the AAD tenant and can have any non-AAD role.</span></span>

<span data-ttu-id="3d6c1-156">如需角色的特定資訊以及每個角色可以執行哪些任務的相關資訊，請參閱[指派使用者權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-156">For specific information on the roles and what each role can do, see [Assign user permissions](permissions-overview.md).</span></span>

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a><span data-ttu-id="3d6c1-157">關聯使用者在合作夥伴中心的 Microsoft Learn 帳戶</span><span class="sxs-lookup"><span data-stu-id="3d6c1-157">Associate a user's Microsoft Learn account in Partner Center</span></span>

<span data-ttu-id="3d6c1-158">為了能夠看到您的使用者對專長認證所採取的訓練和學習路徑，他們必須將其 MCP 識別碼關聯至其合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-158">In order to be able to see the training and learning paths your users are taking towards competencies, they need to associate their MCP ID to their Partner Center account.</span></span> <span data-ttu-id="3d6c1-159">身為全域系統管理員，當您新增使用者時，請務必提醒他們將其 MCP 識別碼關聯至其帳戶。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-159">As the global admin, when you add new users, be sure to remind them to associate their MCP ID to their account.</span></span> 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a><span data-ttu-id="3d6c1-160">如何將您的 MCP 識別碼關聯至您的合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="3d6c1-160">How to associate your MCP ID to your Partner Center account</span></span>

1. <span data-ttu-id="3d6c1-161">從合作夥伴中心儀表板，選取儀表板右上角的 [您的帳戶] 圖示，然後選取 [我的設定檔]。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-161">From the Partner Center dashboard, select the **Your account** icon in the right corner of the dashboard, and then select **My profile**.</span></span>

2. <span data-ttu-id="3d6c1-162">在 [您的學習] 之下，您將能夠關聯 Microsoft Learning 帳戶，也可以將您的 Microsoft 帳戶連線到 Partner University。</span><span class="sxs-lookup"><span data-stu-id="3d6c1-162">Under **Your learning** you will be able to associate your Microsoft Learning account and also connect your Microsoft account to Partner University.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3d6c1-163">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="3d6c1-163">Next steps</span></span>

- [<span data-ttu-id="3d6c1-164">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="3d6c1-164">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>](permissions-overview.md)