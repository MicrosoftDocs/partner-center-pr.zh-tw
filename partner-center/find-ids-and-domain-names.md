---
title: 尋找租使用者識別碼、功能變數名稱、使用者物件識別碼
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在 Azure 入口網站中尋找識別碼-組織的 Azure AD 租使用者識別碼、功能變數名稱或特定的使用者物件識別碼。 某些工作需要此資訊。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439230"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="5362a-104">找出使用者的重要識別碼</span><span class="sxs-lookup"><span data-stu-id="5362a-104">Locate important IDs for a user</span></span>

<span data-ttu-id="5362a-105">本文說明如何使用 [Azure 入口網站](https://portal.azure.com/) 來尋找使用者的下列資訊：</span><span class="sxs-lookup"><span data-stu-id="5362a-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="5362a-106">使用者組織或公司的 Microsoft Azure Active Directory (Azure AD) 租使用者識別碼</span><span class="sxs-lookup"><span data-stu-id="5362a-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="5362a-107">與 Azure AD 租使用者相關聯之組織或公司的主功能變數名稱稱</span><span class="sxs-lookup"><span data-stu-id="5362a-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="5362a-108">使用者物件識別碼</span><span class="sxs-lookup"><span data-stu-id="5362a-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="5362a-109">尋找 Microsoft Azure AD 租使用者識別碼和主功能變數名稱稱</span><span class="sxs-lookup"><span data-stu-id="5362a-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="5362a-110">請遵循下列步驟，找出 Azure 入口網站內 Azure AD 的租使用者識別碼或主功能變數名稱稱。</span><span class="sxs-lookup"><span data-stu-id="5362a-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="5362a-111"> (如果您想要以程式設計方式尋找租使用者識別碼，請參閱 [使用 PowerShell 或 CLI 尋找租使用者識別碼](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)。 ) </span><span class="sxs-lookup"><span data-stu-id="5362a-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="5362a-112">租使用者識別碼可能會在不同的應用程式或資源中被稱為不同的名稱。</span><span class="sxs-lookup"><span data-stu-id="5362a-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="5362a-113">例如，租使用者識別碼可以稱為「目錄識別碼」、「Azure Active Directory (Azure AD) 租使用者、Microsoft ID 或某些報表（甚至是 *tenantguid*）。</span><span class="sxs-lookup"><span data-stu-id="5362a-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="5362a-114">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="5362a-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5362a-115">從功能表中選取 [Azure Active Directory]。</span><span class="sxs-lookup"><span data-stu-id="5362a-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="顯示 Azure 入口網站從功能表選取 Azure Active Directory 選項。":::

3. <span data-ttu-id="5362a-117">Azure Active Directory **總覽** ] 頁面隨即出現。</span><span class="sxs-lookup"><span data-stu-id="5362a-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="5362a-118">若要尋找 Azure AD 租使用者識別碼或主功能變數名稱稱，請尋找 [ **租使用者識別碼** ] 欄位和 [ **主網域** ] 欄位。</span><span class="sxs-lookup"><span data-stu-id="5362a-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="5362a-119">這些欄位會出現在 [租使用者資訊] 區段中。</span><span class="sxs-lookup"><span data-stu-id="5362a-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="顯示具有兩個醒目提示欄位、租使用者識別碼和主功能變數名稱稱的 [總覽] 頁面。":::

4. <span data-ttu-id="5362a-121">您可以使用一些其他方式，在 Azure 入口網站中尋找租使用者識別碼。</span><span class="sxs-lookup"><span data-stu-id="5362a-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="5362a-122">從功能表中選取 [Azure Active Directory]。</span><span class="sxs-lookup"><span data-stu-id="5362a-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="5362a-123">然後，找出功能表上的 [ **管理** ] 區段，然後選取 [ **屬性**]。</span><span class="sxs-lookup"><span data-stu-id="5362a-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="5362a-124">[屬性] 頁面也會顯示使用者相關聯的租使用者識別碼。</span><span class="sxs-lookup"><span data-stu-id="5362a-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="顯示具有反白顯示 [租使用者識別碼] 欄位的屬性頁面。":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="5362a-126">尋找使用者物件識別碼</span><span class="sxs-lookup"><span data-stu-id="5362a-126">Find the user object ID</span></span>

<span data-ttu-id="5362a-127">找不到功能變數名稱和租使用者識別碼，可能不一定就足夠了。</span><span class="sxs-lookup"><span data-stu-id="5362a-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="5362a-128">您可能也需要找出指派給使用者的特定物件識別碼。</span><span class="sxs-lookup"><span data-stu-id="5362a-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="5362a-129">依照下列步驟，在 Azure 入口網站中尋找使用者的物件識別碼：</span><span class="sxs-lookup"><span data-stu-id="5362a-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="5362a-130">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="5362a-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="5362a-131">從功能表中選取 [Azure Active Directory]。</span><span class="sxs-lookup"><span data-stu-id="5362a-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="5362a-132">找出功能表上的 [ **管理** ] 區段，然後選取 [ **使用者**]。</span><span class="sxs-lookup"><span data-stu-id="5362a-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="顯示 Azure Active Directory 功能表，並醒目提示 [使用者] 選項。":::

4. <span data-ttu-id="5362a-134">在 [使用者] 頁面的 [搜尋] 方塊中，輸入使用者的名稱。</span><span class="sxs-lookup"><span data-stu-id="5362a-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="顯示具有搜尋方塊的使用者頁面，以搜尋特定使用者。":::

5. <span data-ttu-id="5362a-136">選取使用者在清單中顯示的名稱。</span><span class="sxs-lookup"><span data-stu-id="5362a-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="顯示使用者頁面，其中顯示搜尋使用者的資料列。":::

6. <span data-ttu-id="5362a-138">在使用者的設定檔頁面面上找出身分識別區段。</span><span class="sxs-lookup"><span data-stu-id="5362a-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="5362a-139">[物件識別碼] 欄位會出現在這裡，並顯示使用者的唯一物件識別碼。</span><span class="sxs-lookup"><span data-stu-id="5362a-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="顯示 [使用者設定檔] 頁面上的 [身分識別] 區段和一個醒目提示的物件識別碼欄位。":::

## <a name="next-steps"></a><span data-ttu-id="5362a-141">後續步驟</span><span class="sxs-lookup"><span data-stu-id="5362a-141">Next steps</span></span>

- [<span data-ttu-id="5362a-142">使用 PowerShell 或 CLI 以程式設計方式尋找您的租使用者識別碼</span><span class="sxs-lookup"><span data-stu-id="5362a-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="5362a-143">深入瞭解 Azure Active Directory 中的使用者設定檔</span><span class="sxs-lookup"><span data-stu-id="5362a-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="5362a-144">瞭解合作夥伴可如何在合作夥伴中心中查看或匯出客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="5362a-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

