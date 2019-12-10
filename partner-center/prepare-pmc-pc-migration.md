---
title: 準備從合作夥伴成員資格中心移至合作夥伴中心 |合作夥伴中心
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 從 PMC 移至合作夥伴中心之前，請先複習有用的資訊和常見問題。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 40ddbd49ad82e1aa5c314da7db366dff6d8a57b4
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943261"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="a899d-103">準備從合作夥伴成員資格中心（PMC）移至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a899d-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="a899d-104">我們正將成員資格管理從合作夥伴成員中心（PMC）移至合作夥伴中心-單一目的地，以管理您與 Microsoft 的商務關係。</span><span class="sxs-lookup"><span data-stu-id="a899d-104">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="a899d-105">我們希望您的移至合作夥伴中心盡可能有效率且更容易。</span><span class="sxs-lookup"><span data-stu-id="a899d-105">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="a899d-106">我們已識別出合作夥伴中心與 PMC 不同的區域，因此我們認為您會想要先瞭解並準備好，然後再進行移動。</span><span class="sxs-lookup"><span data-stu-id="a899d-106">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="a899d-107">帳戶和身分識別設定</span><span class="sxs-lookup"><span data-stu-id="a899d-107">Account and identity setup</span></span>

<span data-ttu-id="a899d-108">**什麼是 Azure Active Directory （Azure AD）工作帳戶？**</span><span class="sxs-lookup"><span data-stu-id="a899d-108">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="a899d-109">Azure 工作帳戶是您公司在 Azure 公用雲端的專用且隔離的虛擬表示，這已在您訂閱 Microsoft 雲端服務 (例如 Azure、Microsoft Intune 或 Office 365) 時建立。</span><span class="sxs-lookup"><span data-stu-id="a899d-109">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="a899d-110">您的工作帳戶會主控您的 Azure AD 使用者及其相關資訊（其電子郵件、密碼、設定檔資料、許可權等）。</span><span class="sxs-lookup"><span data-stu-id="a899d-110">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="a899d-111">工作帳戶也包含群組、應用程式，以及與公司和其安全性有關的其他資訊。</span><span class="sxs-lookup"><span data-stu-id="a899d-111">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="a899d-112">如需詳細資訊，請參閱 。</span><span class="sxs-lookup"><span data-stu-id="a899d-112">For more information see ...</span></span>

<span data-ttu-id="a899d-113">在合作夥伴中心，您將使用您的公司電子郵件，登入您的帳戶，而不是您的個人電子郵件。</span><span class="sxs-lookup"><span data-stu-id="a899d-113">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="a899d-114">您的公司帳戶： john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="a899d-114">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="a899d-115">您的個人帳戶： John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="a899d-115">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="a899d-116">您的公司電子郵件是 Azure active directory 租使用者的一部分。</span><span class="sxs-lookup"><span data-stu-id="a899d-116">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="a899d-117">若要在合作夥伴中心擁有帳戶，您需要有 AAD 租使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-117">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="a899d-118">如需 Azure Active Directory 的詳細資訊，請參閱[在 Azure AD 中建立目錄](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="a899d-118">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="a899d-119">**當您從 PMC 移至合作夥伴中心時，如果您有與 Microsoft 的 AAD 租使用者（例如 Office 365），而且您的 CSP 業務也有租使用者，您應該使用哪一個帳戶登入合作夥伴中心？**</span><span class="sxs-lookup"><span data-stu-id="a899d-119">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="a899d-120">您可以使用 CSP 帳戶或 MPN work 電子郵件帳戶登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a899d-120">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="a899d-121">如果您選擇使用 CSP 工作電子郵件登入，儀表板上的左側導覽會顯示 MPN 和 CSP 計畫資訊。</span><span class="sxs-lookup"><span data-stu-id="a899d-121">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="a899d-122">如果您使用 MPN Azure AD 租使用者的公司電子郵件登入，只會看到您的 MPN 程式資訊。</span><span class="sxs-lookup"><span data-stu-id="a899d-122">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="a899d-123">MPN 和 CSP 之間的使用者角色不同，因此，如果您在 MPN 和 CSP business 兩者都使用相同的帳戶，請務必據以指派使用者角色。</span><span class="sxs-lookup"><span data-stu-id="a899d-123">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="a899d-124">如需使用者角色的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a899d-124">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="a899d-125">**如果您不想要將現有的 Office 365 Azure AD 租使用者用於合作夥伴中心，您可以在從 PMC 遷移之前，先建立新的租使用者。**</span><span class="sxs-lookup"><span data-stu-id="a899d-125">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="a899d-126">您不想使用現有的 Azure AD 租使用者來設定您的合作夥伴中心帳戶，可能有許多原因。</span><span class="sxs-lookup"><span data-stu-id="a899d-126">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="a899d-127">開始遷移至合作夥伴中心之前，請移至[Azure 入口網站](https://ms.portal.azure.com/#home)建立新的 Azure AD 租使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-127">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="a899d-128">遵循在 Azure Active Directory 中[建立新的租](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)使用者中的指引。</span><span class="sxs-lookup"><span data-stu-id="a899d-128">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="a899d-129">一旦您建立新的租使用者，請在從 PMC 移至合作夥伴中心時，使用此 AAD 租使用者來設定您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="a899d-129">Once you have created the new tenant, use this AAD tenant to set up your Partner Center account when you move from PMC to Partner Center.</span></span> <span data-ttu-id="a899d-130">您必須是全域管理員，才能建立租使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-130">You must be a global admin to create the tenant.</span></span> <span data-ttu-id="a899d-131">使用這個新目錄來遷移至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a899d-131">Use this new directory to migrate to Partner Center.</span></span>


<span data-ttu-id="a899d-132">**AAD 全域管理員角色與 PMC MPN 全域管理員角色之間有何差異？**</span><span class="sxs-lookup"><span data-stu-id="a899d-132">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="a899d-133">這些是兩個完全不同的角色，具有不同的許可權。</span><span class="sxs-lookup"><span data-stu-id="a899d-133">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="a899d-134">合作夥伴中心內的 AAD 租使用者全域管理員會管理租使用者-新增或移除使用者、提供及管理密碼、角色和許可權，並可存取其在合作夥伴中心內的所有公司程式。</span><span class="sxs-lookup"><span data-stu-id="a899d-134">The AAD tenant global admin in Partner Center administers the tenant - adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company's programs in Partner Center.</span></span> 

<span data-ttu-id="a899d-135">PMC 中的 MPN 全域管理員角色可以執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="a899d-135">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="a899d-136">查看和編輯所有與公司相關聯的資料，以及公司的所有位置</span><span class="sxs-lookup"><span data-stu-id="a899d-136">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="a899d-137">在全域或本機層級新增系統管理員。</span><span class="sxs-lookup"><span data-stu-id="a899d-137">Add administrators at the global or local level.</span></span>  <span data-ttu-id="a899d-138">此外，全域管理員可以將任何位置的任何人員指派給全域管理員存取權，不論其相關聯的位置為何，都能授與全域存取權。</span><span class="sxs-lookup"><span data-stu-id="a899d-138">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="a899d-139">執行任何面向合作夥伴的 UI 功能，包括：</span><span class="sxs-lookup"><span data-stu-id="a899d-139">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="a899d-140">新增/移除使用者</span><span class="sxs-lookup"><span data-stu-id="a899d-140">Add/remove users</span></span>

 - <span data-ttu-id="a899d-141">指派/移除角色</span><span class="sxs-lookup"><span data-stu-id="a899d-141">Assign/remove roles</span></span> 

 - <span data-ttu-id="a899d-142">新增/移除/更新位置</span><span class="sxs-lookup"><span data-stu-id="a899d-142">Add/remove/update locations</span></span> 

 - <span data-ttu-id="a899d-143">購買專長認證/maps</span><span class="sxs-lookup"><span data-stu-id="a899d-143">Purchase competency/maps</span></span> 

-  <span data-ttu-id="a899d-144">觀看權益</span><span class="sxs-lookup"><span data-stu-id="a899d-144">View benefits</span></span>

<span data-ttu-id="a899d-145">當 MPN 全域管理員移到合作夥伴中心時，角色稱為 MPN 夥伴管理員，其許可權和工作與合作夥伴中心全域管理員不同。如需合作夥伴中心角色和許可權的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a899d-145">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="a899d-146">**在合作夥伴中心包含來賓使用者角色的使用者角色**</span><span class="sxs-lookup"><span data-stu-id="a899d-146">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="a899d-147">合作夥伴中心具有不同類型的角色，視所需執行的工作類型而定。</span><span class="sxs-lookup"><span data-stu-id="a899d-147">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="a899d-148">有一些角色（例如全域管理員） Azure AD 角色。</span><span class="sxs-lookup"><span data-stu-id="a899d-148">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="a899d-149">某些角色專屬於雲端服務提供者方案或獎勵等方案，而且有 MPN 特有的角色。</span><span class="sxs-lookup"><span data-stu-id="a899d-149">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="a899d-150">若要瞭解合作夥伴中心的角色為何，請參閱[指派使用者角色和許可權](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a899d-150">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="a899d-151">**當我的使用者角色從 PMC 移到合作夥伴中心時，會發生什麼事？**</span><span class="sxs-lookup"><span data-stu-id="a899d-151">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="a899d-152">除了進行遷移的 MPN 全域管理員或主要程式連絡人以外，PMC 中的所有使用者都會失去其系統管理員角色。</span><span class="sxs-lookup"><span data-stu-id="a899d-152">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="a899d-153">完成遷移的個人將需要在合作夥伴中心指派角色。</span><span class="sxs-lookup"><span data-stu-id="a899d-153">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="a899d-154">合作夥伴中心的角色與 PMC 中的角色不同。</span><span class="sxs-lookup"><span data-stu-id="a899d-154">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="a899d-155">閱讀 [指派使用者角色和許可權] （許可權-overview.md，並[從 PMC 移至合作夥伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)，以取得合作夥伴中心的使用者角色的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="a899d-155">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="a899d-156">**我的公司設定檔與我的商務設定檔之間有何差異？**</span><span class="sxs-lookup"><span data-stu-id="a899d-156">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="a899d-157">您的公司設定檔是貴公司的相關資訊，其中包含位址、位置、主要連絡人、銀行和稅務詳細資料。</span><span class="sxs-lookup"><span data-stu-id="a899d-157">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="a899d-158">您的商務設定檔是您向客戶呈現自己的方式，而這是一個行銷頁面，可顯示您的標誌、企業焦點的詳細資料、您的專業知識等等。</span><span class="sxs-lookup"><span data-stu-id="a899d-158">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="a899d-159">**帳戶匯總對我的帳戶的意義為何？**</span><span class="sxs-lookup"><span data-stu-id="a899d-159">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="a899d-160">如果您使用相同的 Azure AD 租使用者，將多個 MPN 帳戶遷移到合作夥伴中心，系統會自動辨識並要求您合併您的帳戶。</span><span class="sxs-lookup"><span data-stu-id="a899d-160">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="a899d-161">即使您有多個與相同 Azure AD 租使用者相關聯的網域，也是如此。</span><span class="sxs-lookup"><span data-stu-id="a899d-161">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="a899d-162">您仍然可以使用個別的 AAD 租使用者決定遷移至合作夥伴中心，但請注意，這會導致您的專長認證和額外購買成本的隔離評估。</span><span class="sxs-lookup"><span data-stu-id="a899d-162">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="a899d-163">**如果我有多個 AAD 租使用者和單一 MPN 帳戶，可以在合作夥伴中心連結它們嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-163">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="a899d-164">是，在合作夥伴中心，您可以將多個 Azure AD 租使用者連結至單一合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="a899d-164">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="a899d-165">請按一下這裡以進一步了解。</span><span class="sxs-lookup"><span data-stu-id="a899d-165">Learn more here.</span></span> 

<span data-ttu-id="a899d-166">**將多個 Azure AD 租使用者新增至單一合作夥伴中心帳戶是否有任何限制？**</span><span class="sxs-lookup"><span data-stu-id="a899d-166">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="a899d-167">如果 Azure AD 租使用者已與現有的合作夥伴中心帳戶相關聯，則無法使用多租使用者功能將它與新的合作夥伴中心帳戶產生關聯。</span><span class="sxs-lookup"><span data-stu-id="a899d-167">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="a899d-168">另一個要考慮的方法是，Azure AD 租使用者只能與一個合作夥伴中心帳戶相關聯，但合作夥伴中心帳戶可以有多個相關聯的租使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-168">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="a899d-169">Microsoft 合作夥伴網路（MPN）成員資格遷移</span><span class="sxs-lookup"><span data-stu-id="a899d-169">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="a899d-170">**誰可以執行從 PMC 移至合作夥伴中心？**</span><span class="sxs-lookup"><span data-stu-id="a899d-170">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="a899d-171">您的公司 MPN 全域管理員或主要程式連絡人（這兩個角色通常由同一人持有）可以起始和執行移動。</span><span class="sxs-lookup"><span data-stu-id="a899d-171">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="a899d-172">**完成遷移的人員是否會成為合作夥伴中心內公司法律設定檔的主要連絡人？**</span><span class="sxs-lookup"><span data-stu-id="a899d-172">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="a899d-173">但不一定，主要連絡人必須是有權簽署合約的人。</span><span class="sxs-lookup"><span data-stu-id="a899d-173">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="a899d-174">**Microsoft 可以為我遷移我的 MPN 成員資格嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-174">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="a899d-175">不。</span><span class="sxs-lookup"><span data-stu-id="a899d-175">No.</span></span> <span data-ttu-id="a899d-176">Microsoft 無法協助您將您的成員資格帳戶移至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a899d-176">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="a899d-177">您必須使用您的工作帳戶（登入認證）登入 PMC，以開始進行遷移程式，以移動您的帳戶。</span><span class="sxs-lookup"><span data-stu-id="a899d-177">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="a899d-178">完成移動帳戶的步驟之後，您就可以開始管理您的成員資格，並將使用者角色和許可權指派給您的小組，讓他們可以存取權益並協助管理成員資格。</span><span class="sxs-lookup"><span data-stu-id="a899d-178">After you've completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="a899d-179">Microsoft 會自動遷移目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含合作夥伴大學存取權的 MCP 關聯。</span><span class="sxs-lookup"><span data-stu-id="a899d-179">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="a899d-180">Microsoft 會自動遷移目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含合作夥伴大學存取權的 MCP 關聯。</span><span class="sxs-lookup"><span data-stu-id="a899d-180">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="a899d-181">**更新原則會如何變更？**</span><span class="sxs-lookup"><span data-stu-id="a899d-181">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="a899d-182">在 [合作夥伴中心] 中，[更新] 視窗會從您的週年日起到以下30天。</span><span class="sxs-lookup"><span data-stu-id="a899d-182">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="a899d-183">**我們的專長認證會在移至合作夥伴中心後保持不變嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-183">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="a899d-184">是的，compentencies 不會受到 [移至合作夥伴中心] 的影響。</span><span class="sxs-lookup"><span data-stu-id="a899d-184">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="a899d-185">如果您注意到不一致的情況，請聯絡[支援](https://partner.microsoft.com/support)人員。</span><span class="sxs-lookup"><span data-stu-id="a899d-185">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="a899d-186">**移動後，我的權益（包括雲端權益、技術支援、軟體權益、Visual Studio）是否有變更？**</span><span class="sxs-lookup"><span data-stu-id="a899d-186">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="a899d-187">您的合格權益不會變更。</span><span class="sxs-lookup"><span data-stu-id="a899d-187">Your eligible benefits will not change.</span></span> <span data-ttu-id="a899d-188">如果您注意到不一致的情況，請聯絡[支援](https://partner.microsoft.com/support)人員。</span><span class="sxs-lookup"><span data-stu-id="a899d-188">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="a899d-189">**我們的 Microsoft 帳戶將會接受 Visual Studio 權益嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-189">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="a899d-190">可以。</span><span class="sxs-lookup"><span data-stu-id="a899d-190">Yes.</span></span> <span data-ttu-id="a899d-191">將會接受並保留配置給 MSA 的 Visual Studio 權益。</span><span class="sxs-lookup"><span data-stu-id="a899d-191">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="a899d-192">在合作夥伴中心中續訂之後，也會保留它們。</span><span class="sxs-lookup"><span data-stu-id="a899d-192">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="a899d-193">不過，如果您在合作夥伴中心遷移之後移除 MSA 配置，就無法將其新增回合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a899d-193">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="a899d-194">在合作夥伴中心中，合作夥伴可以加入公司帳戶及來賓使用者帳戶，其為來自合作夥伴為 Azure AD 租用戶中 MPN 系統管理員之相同租用戶的 MSA。</span><span class="sxs-lookup"><span data-stu-id="a899d-194">In Partner Center, a partner can add work accounts and guest user accounts which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="a899d-195">如果合作夥伴是多個 Azure AD 租用戶中的全域系統管理員，且這些租用戶都是與相同的合作夥伴中心帳戶相關聯，則該合作夥伴便可以將所有這些租用戶上的使用者加入 Visual Studio 權益和 Azure 以使用量為基礎的配置。</span><span class="sxs-lookup"><span data-stu-id="a899d-195">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="a899d-196">雖然 MPN 系統管理員或全域系統管理員可以將 Visual Studio 以使用量為基礎的訂用帳戶指派給來賓使用者，來賓使用者並無法使用其 MSA 登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="a899d-196">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="a899d-197">不過，來賓使用者可以登入 Azure 和 Visual Studio 以驗證並使用指派給他的權益。</span><span class="sxs-lookup"><span data-stu-id="a899d-197">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="a899d-198">**我們應該如何管理 MCP 關聯和合作夥伴大學的存取權？**</span><span class="sxs-lookup"><span data-stu-id="a899d-198">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="a899d-199">從 PMC 移動的 MCP 關聯不會有任何變更。</span><span class="sxs-lookup"><span data-stu-id="a899d-199">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="a899d-200">不過，移至合作夥伴中心後的任何新員工都必須在合作夥伴中心內建立關聯。</span><span class="sxs-lookup"><span data-stu-id="a899d-200">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="a899d-201">現有使用者的所有合作夥伴大學許可權將會保留，但任何新員工都應前往[訓練中心](https://partner.microsoft.com/training)，以取得如何取得合作夥伴大學的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="a899d-201">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="a899d-202">**當我移到合作夥伴中心後，如何? 看到 MCP 資訊？**</span><span class="sxs-lookup"><span data-stu-id="a899d-202">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="a899d-203">從 [儀表板] 的左側導覽中選取 [**職稱**]。</span><span class="sxs-lookup"><span data-stu-id="a899d-203">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="a899d-204">在 [專長認證 **] 頁面上**，您可以下載技能報告。</span><span class="sxs-lookup"><span data-stu-id="a899d-204">From the **Competencies** page you are able to download the skills report.</span></span> <span data-ttu-id="a899d-205">技能報告將會列出已取得合作夥伴中心之專長和計畫相關技能的使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-205">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="a899d-206">如果您的使用者已獲得技能，但那些技能與您正在努力的專長無關，則不會列在報表中。</span><span class="sxs-lookup"><span data-stu-id="a899d-206">If your users have gained skills but those skills are not relevant to the competencies which you are working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="a899d-207">**合作夥伴中心是否使用客戶參考？**</span><span class="sxs-lookup"><span data-stu-id="a899d-207">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="a899d-208">否，您不需要客戶參考以符合合作夥伴中心的專長認證需求。</span><span class="sxs-lookup"><span data-stu-id="a899d-208">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="a899d-209">**記錄關聯的夥伴會移到合作夥伴中心嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-209">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="a899d-210">是，不會變更記錄的夥伴。</span><span class="sxs-lookup"><span data-stu-id="a899d-210">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="a899d-211">深入瞭解如何將[您的合作夥伴識別碼連結至您的客戶](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="a899d-211">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="a899d-212">**因為移至合作夥伴中心，是否會影響獎勵？**</span><span class="sxs-lookup"><span data-stu-id="a899d-212">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="a899d-213">否，如果您已移動帳戶而未合併位置，則不會影響獎勵。</span><span class="sxs-lookup"><span data-stu-id="a899d-213">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="a899d-214">如果您的公司在 PMC 中有多個帳戶，而當您移至合作夥伴中心時，您決定將合併到通用帳戶，則不會有任何獎勵，但激勵支出可能會有延遲。</span><span class="sxs-lookup"><span data-stu-id="a899d-214">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="a899d-215">如果您未移動所有與獎勵計畫相關的 PMC 帳戶，您可能會停止獲得與這些帳戶系結的獎勵。</span><span class="sxs-lookup"><span data-stu-id="a899d-215">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="a899d-216">**合作夥伴中心的獎勵使用者角色為何？**</span><span class="sxs-lookup"><span data-stu-id="a899d-216">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="a899d-217">合作夥伴中心的獎勵角色是以位置為基礎，並包含獎勵系統管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="a899d-217">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="a899d-218">如需這些角色可執行之動作的詳細資訊，請參閱[指派使用者角色和許可權](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="a899d-218">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="a899d-219">**可以在全域和位置層級指派給使用者嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-219">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="a899d-220">可以。</span><span class="sxs-lookup"><span data-stu-id="a899d-220">Yes.</span></span> <span data-ttu-id="a899d-221">您可以將獎勵系統管理員指派為所有位置的獎勵管理員，或每個位置都有自己的獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="a899d-221">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="a899d-222">**可以在全域或位置層級支付獎勵嗎？**</span><span class="sxs-lookup"><span data-stu-id="a899d-222">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="a899d-223">獎勵只會在位置層級付費。</span><span class="sxs-lookup"><span data-stu-id="a899d-223">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="a899d-224">**關於參考，我們可以建立多少個商務設定檔？**</span><span class="sxs-lookup"><span data-stu-id="a899d-224">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="a899d-225">您的公司可以建立所需數量的商務設定檔，以完全代表貴公司的興趣。</span><span class="sxs-lookup"><span data-stu-id="a899d-225">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="a899d-226">在每個商務設定檔中，您最多可以列出五個位置，每個國家/地區一個位置。</span><span class="sxs-lookup"><span data-stu-id="a899d-226">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="a899d-227">每個商務設定檔都可以接收其每個位置的參考。</span><span class="sxs-lookup"><span data-stu-id="a899d-227">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="a899d-228">**如何指派參照，我可以預期的變更為何？例如，如果我在某個市場上有一個全球性的公司，而在其他市場上有個地點，則會如何指派參考？**</span><span class="sxs-lookup"><span data-stu-id="a899d-228">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="a899d-229">系統會根據客戶所定義的搜尋參數來指派參照。</span><span class="sxs-lookup"><span data-stu-id="a899d-229">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="a899d-230">因此，不論您是否有一個位置或多個地點，如果客戶指定了所需的位置，而且您有符合其他參數的業務，則參照會移至該位置。</span><span class="sxs-lookup"><span data-stu-id="a899d-230">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








