---
title: 建立使用者帳戶和指派角色
description: 每位員工都必須先獲指派角色，然後才能存取合作夥伴中心。 了解如何建立使用者帳戶、指派角色，以及設定權限。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperfq2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 41f7f68c61630daf30595e28bd5de52f5a5787c8
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006772"
---
# <a name="create-user-accounts"></a><span data-ttu-id="0d1bf-104">建立使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="0d1bf-104">Create user accounts</span></span>  

<span data-ttu-id="0d1bf-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="0d1bf-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0d1bf-106">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="0d1bf-106">Account admin</span></span>
- <span data-ttu-id="0d1bf-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="0d1bf-107">Global admin</span></span>
- <span data-ttu-id="0d1bf-108">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="0d1bf-108">User management admin</span></span>

<span data-ttu-id="0d1bf-109">為需要存取合作夥伴中心的員工建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-109">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="0d1bf-110">這些工作必須由使用者管理系統管理員、帳戶系統管理員或全域系統管理員來完成。執行這些工作的使用者也必須獲派 Azure Active Directory (AAD) 的「使用者管理員」或「全域管理員」角色。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-110">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="0d1bf-111">如需 AAD 角色的詳細資訊，請參閱 [Azure Active Directory 中的管理員角色權限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-111">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="0d1bf-112">新增使用者</span><span class="sxs-lookup"><span data-stu-id="0d1bf-112">Add a new user</span></span>

1. <span data-ttu-id="0d1bf-113">從合作夥伴中心右上角的 [設定] 圖示中，選取 [帳戶設定]，接著再選取 [使用者管理]。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-113">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="0d1bf-114">選取 [新增使用者]。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-114">Select **Add user**.</span></span>

3. <span data-ttu-id="0d1bf-115">輸入使用者的全名和唯一電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-115">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="0d1bf-116">選取您要指派給使用者的代理人類型及/或系統管理員類型。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-116">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="0d1bf-117">合作夥伴中心存取權是以角色為基礎，讓您可以指派權限，自訂使用者檢視，只顯示使用者完成特定工作所需的功能。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-117">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="0d1bf-118">若使用者想要角色指派，他們可以移至 [使用者管理] 並篩選全域系統管理員，找到要連絡的全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-118">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="0d1bf-119">選取 [新增] 建立使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-119">Select **Add** to create the user account.</span></span> <span data-ttu-id="0d1bf-120">在下一頁，確認使用者的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-120">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="0d1bf-121">記下此頁面上顯示的新使用者登入資訊。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-121">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="0d1bf-122">請務必將這項資訊複製及傳送給新的使用者，因為稍後您將無法再次存取。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-122">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="0d1bf-123">使用者必須使用其使用者名稱和暫時密碼登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-123">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="0d1bf-124">當使用者第一次登入合作夥伴中心時，系統會提示他們變更密碼。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-124">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="0d1bf-125">指派使用者角色</span><span class="sxs-lookup"><span data-stu-id="0d1bf-125">Assign user roles</span></span>

<span data-ttu-id="0d1bf-126">若要在合作夥伴中心中工作，您必須具有指派的角色。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-126">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="0d1bf-127">目前，這些角色包括 Azure Active Directory 租用戶角色、雲端解決方案提供者 (CSP) 角色，以及非 AAD 公司角色。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-127">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="0d1bf-128">個別公司可能需要所有這些角色。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-128">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="0d1bf-129">個人必須列示在您的租用戶中，才能存取合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-129">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="0d1bf-130">角色指派會提供額外的存取權。</span><span class="sxs-lookup"><span data-stu-id="0d1bf-130">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="0d1bf-131">後續步驟</span><span class="sxs-lookup"><span data-stu-id="0d1bf-131">Next steps</span></span>

- [<span data-ttu-id="0d1bf-132">為需要在合作夥伴中心工作的員工指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="0d1bf-132">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
