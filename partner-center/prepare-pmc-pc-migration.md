---
title: 準備從 Partner Membership Center 移至合作夥伴中心 | 合作夥伴中心
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 從 PMC 移至合作夥伴中心之前，請先檢閱有用的資訊和常見問題集。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 06167a667152ddaf65702547783df93726f6cadc
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2020
ms.locfileid: "78340097"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="47a28-103">準備從 Partner Membership Center (PMC) 移至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="47a28-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="47a28-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="47a28-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="47a28-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="47a28-105">Global admin</span></span>
-    <span data-ttu-id="47a28-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="47a28-106">User admin</span></span>
-    <span data-ttu-id="47a28-107">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="47a28-107">Sales agent</span></span>
-    <span data-ttu-id="47a28-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="47a28-108">Admin agent</span></span>

<span data-ttu-id="47a28-109">我們正將成員資格管理從 Partner Membership Center (PMC) 移至合作夥伴中心 - 以此單一目的地管理您與 Microsoft 的商務關係。</span><span class="sxs-lookup"><span data-stu-id="47a28-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="47a28-110">我們希望您能夠盡可能輕鬆有效地移至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="47a28-111">我們已識別出合作夥伴中心與 PMC 不同的層面，而且我們認為您會想要先充分了解並做好準備，再進行移轉。</span><span class="sxs-lookup"><span data-stu-id="47a28-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="47a28-112">帳戶和身分識別設定</span><span class="sxs-lookup"><span data-stu-id="47a28-112">Account and identity setup</span></span>

<span data-ttu-id="47a28-113">**什麼是 Azure Active Directory (Azure AD) 公司帳戶？**</span><span class="sxs-lookup"><span data-stu-id="47a28-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="47a28-114">Azure 工作帳戶是您公司在 Azure 公用雲端的專用且隔離的虛擬表示，這已在您訂閱 Microsoft 雲端服務 (例如 Azure、Microsoft Intune 或 Office 365) 時建立。</span><span class="sxs-lookup"><span data-stu-id="47a28-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="47a28-115">您的公司帳戶會裝載 Azure AD 使用者及其相關資訊 (電子郵件、密碼、設定檔資料、權限等等)。</span><span class="sxs-lookup"><span data-stu-id="47a28-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="47a28-116">公司帳戶也包含群組、應用程式，以及其他有關公司與其安全性的資訊。</span><span class="sxs-lookup"><span data-stu-id="47a28-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="47a28-117">在合作夥伴中心，您將使用您的公司電子郵件登入帳戶，而不是使用個人電子郵件。</span><span class="sxs-lookup"><span data-stu-id="47a28-117">In Partner Center, you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="47a28-118">您的公司帳戶：john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="47a28-118">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="47a28-119">您的個人帳戶：John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="47a28-119">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="47a28-120">您的公司電子郵件是 Azure Active Directory 租用戶的一部分。</span><span class="sxs-lookup"><span data-stu-id="47a28-120">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="47a28-121">若要在合作夥伴中心擁有帳戶，您必須要有 AAD 租用戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-121">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="47a28-122">如需 Azure Active Directory 的詳細資訊，請參閱[在 Azure AD 中建立目錄](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)。</span><span class="sxs-lookup"><span data-stu-id="47a28-122">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="47a28-123">**如果您有與 Microsoft (例如 Office 365) 搭配使用的 AAD 租用戶，同時也有用於雲端解決方案提供者業務的租用戶，當您從 PMC 移至合作夥伴中心時，應使用哪個帳戶登入合作夥伴中心？**</span><span class="sxs-lookup"><span data-stu-id="47a28-123">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="47a28-124">您可以使用雲端解決方案提供者帳戶或 MPN 公司電子郵件帳戶登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-124">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="47a28-125">如果您選擇使用雲端解決方案提供者公司電子郵件登入，儀表板上的左側導覽將會顯示 MPN 和雲端解決方案提供者計畫資訊。</span><span class="sxs-lookup"><span data-stu-id="47a28-125">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="47a28-126">如果您使用 MPN Azure AD 租用戶的公司電子郵件登入，則只會看到 MPN 計畫資訊。</span><span class="sxs-lookup"><span data-stu-id="47a28-126">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="47a28-127">MPN 和雲端解決方案提供者的使用者角色並不相同，因此，如果您對 MPN 和雲端解決方案提供者業務使用相同的帳戶，請務必據以指派使用者角色。</span><span class="sxs-lookup"><span data-stu-id="47a28-127">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="47a28-128">如需使用者角色的相關資訊，請參閱[指派使用者角色和權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="47a28-128">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="47a28-129">**如果您不想將現有的 Office 365 Azure AD 租用戶用於合作夥伴中心，您可以在從 PMC 移轉之前，先建立新的租用戶。**</span><span class="sxs-lookup"><span data-stu-id="47a28-129">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="47a28-130">您不想使用現有的 Azure AD 租用戶來設定合作夥伴中心帳戶，可能有許多原因。</span><span class="sxs-lookup"><span data-stu-id="47a28-130">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="47a28-131">開始移轉至合作夥伴中心之前，請先移至 [Azure 入口網站](https://ms.portal.azure.com/#home)建立新的 Azure AD 租用戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-131">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="47a28-132">請依照[在 Azure Active Directory 中建立新的租用戶](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)中的指引操作。</span><span class="sxs-lookup"><span data-stu-id="47a28-132">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="47a28-133">建立新的租用戶後，當您從 PMC 移至合作夥伴中心時，請使用此 AAD 租用戶來設定您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-133">Once you have created the new tenant, use this AAD tenant to set up your Partner Center account when you move from PMC to Partner Center.</span></span> <span data-ttu-id="47a28-134">您必須是全域管理員，才能建立租用戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-134">You must be a global admin to create the tenant.</span></span> <span data-ttu-id="47a28-135">請使用這個新的目錄移轉至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-135">Use this new directory to migrate to Partner Center.</span></span>


<span data-ttu-id="47a28-136">**AAD 全域管理員角色與 PMC MPN 全域管理員角色有何差異？**</span><span class="sxs-lookup"><span data-stu-id="47a28-136">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="47a28-137">這是兩個不同的角色，具有不同的權限。</span><span class="sxs-lookup"><span data-stu-id="47a28-137">These are two different roles with different permissions.</span></span> <span data-ttu-id="47a28-138">合作夥伴中心的 AAD 租用戶全域管理員可管理租用戶 - 新增或移除使用者、提供及管理密碼、角色和權限，並且可存取其公司在合作夥伴中心內的所有計畫。</span><span class="sxs-lookup"><span data-stu-id="47a28-138">The AAD tenant global admin in Partner Center administers the tenant - adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company's programs in Partner Center.</span></span> 

<span data-ttu-id="47a28-139">PMC 中的 MPN 全域管理員角色可執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="47a28-139">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="47a28-140">檢視和編輯所有與公司相關聯的資料，以及公司的所有位置</span><span class="sxs-lookup"><span data-stu-id="47a28-140">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="47a28-141">在全域或本機層級新增管理員。</span><span class="sxs-lookup"><span data-stu-id="47a28-141">Add administrators at the global or local level.</span></span>  <span data-ttu-id="47a28-142">此外，全域管理員可為任何位置的任何人員指派全域管理員存取權，而為他們授與全域存取權，不論其關聯的位置為何。</span><span class="sxs-lookup"><span data-stu-id="47a28-142">Also, Global admins can assign any person at any location Global Administrator Access, which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="47a28-143">執行任何合作夥伴對應 UI 功能，包括：</span><span class="sxs-lookup"><span data-stu-id="47a28-143">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="47a28-144">新增/移除使用者</span><span class="sxs-lookup"><span data-stu-id="47a28-144">Add/remove users</span></span>

 - <span data-ttu-id="47a28-145">指派/移除角色</span><span class="sxs-lookup"><span data-stu-id="47a28-145">Assign/remove roles</span></span> 

 - <span data-ttu-id="47a28-146">新增/移除/更新位置</span><span class="sxs-lookup"><span data-stu-id="47a28-146">Add/remove/update locations</span></span> 

 - <span data-ttu-id="47a28-147">購買專長認證/MAPS</span><span class="sxs-lookup"><span data-stu-id="47a28-147">Purchase competency/maps</span></span> 

-  <span data-ttu-id="47a28-148">檢視權益</span><span class="sxs-lookup"><span data-stu-id="47a28-148">View benefits</span></span>

<span data-ttu-id="47a28-149">當 MPN 全域管理員移至合作夥伴中心時，我們將此角色稱為 MPN 合作夥伴管理員，其權限和工作皆與合作夥伴中心全域管理員不同。若要深入了解合作夥伴中心的角色和權限，請參閱[指派使用者角色和權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="47a28-149">When the MPN global admin moves to Partner Center the role is called the MPN partner admin, which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="47a28-150">**合作夥伴中心的使用者角色 (包括來賓使用者角色)**</span><span class="sxs-lookup"><span data-stu-id="47a28-150">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="47a28-151">合作夥伴中心具有不同類型的角色，視所需執行的工作類型而定。</span><span class="sxs-lookup"><span data-stu-id="47a28-151">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="47a28-152">有些角色屬於 Azure AD 角色，例如全域管理員。</span><span class="sxs-lookup"><span data-stu-id="47a28-152">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="47a28-153">有些角色則專屬於計畫 (例如雲端服務提供者計畫) 或獎勵，此外也有專屬於 MPN 的角色。</span><span class="sxs-lookup"><span data-stu-id="47a28-153">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="47a28-154">若要了解所有的合作夥伴中心角色，請參閱[指派使用者角色和權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="47a28-154">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="47a28-155">**我的使用者角色從 PMC 移至合作夥伴中心後，將會如何？**</span><span class="sxs-lookup"><span data-stu-id="47a28-155">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="47a28-156">除了 MPN 全域管理員或執行移轉的主要計畫連絡人以外，PMC 中的所有使用者都將失去其管理員角色。</span><span class="sxs-lookup"><span data-stu-id="47a28-156">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="47a28-157">完成移轉的人員將必須在合作夥伴中心指派角色。</span><span class="sxs-lookup"><span data-stu-id="47a28-157">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="47a28-158">合作夥伴中心的角色與 PMC 中的角色並不相同。</span><span class="sxs-lookup"><span data-stu-id="47a28-158">The roles in Partner Center differ from the roles in PMC.</span></span> <span data-ttu-id="47a28-159">請參閱 [指派使用者角色和權限] (permissions-overview.md) 和[從 PMC 移至合作夥伴中心](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)，以深入了解合作夥伴中心的使用者角色。</span><span class="sxs-lookup"><span data-stu-id="47a28-159">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="47a28-160">**我的公司設定檔與商務設定檔之間有何差異？**</span><span class="sxs-lookup"><span data-stu-id="47a28-160">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="47a28-161">公司設定檔是公司的相關資訊，包括地址、位置、主要連絡人、銀行和稅務詳細資料。</span><span class="sxs-lookup"><span data-stu-id="47a28-161">Your company profile is the information about your company that includes address, locations, primary contact, bank, and tax details.</span></span>

<span data-ttu-id="47a28-162">商務設定檔則是您向客戶介紹自己的方式，這是一個行銷頁面，可顯示您的標誌、企業焦點的詳細資料、您的專業能力等等。</span><span class="sxs-lookup"><span data-stu-id="47a28-162">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="47a28-163">**帳戶合併對我的帳戶有何意義？**</span><span class="sxs-lookup"><span data-stu-id="47a28-163">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="47a28-164">如果您使用相同的 Azure AD 租用戶將多個 MPN 帳戶移轉至合作夥伴中心，系統會自動加以辨識，並要求您合併帳戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-164">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="47a28-165">即使您有多個網域與相同的 Azure AD 租用戶相關聯，仍是如此。</span><span class="sxs-lookup"><span data-stu-id="47a28-165">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="47a28-166">您仍可決定使用個別的 AAD 租用戶來移轉至合作夥伴中心，但請注意，這會導致您的專長認證受到單獨評估，並產生額外的購買成本。</span><span class="sxs-lookup"><span data-stu-id="47a28-166">You could still decide to migrate to Partner Center using separate AAD tenants, but note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="47a28-167">**如果我有多個 AAD 租用戶和單一 MPN 帳戶，是否可在合作夥伴中心將其連結嗎？**</span><span class="sxs-lookup"><span data-stu-id="47a28-167">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="47a28-168">是，在合作夥伴中心，您可以將多個 Azure AD 租用戶連結至單一合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-168">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="47a28-169">請於此處深入了解。</span><span class="sxs-lookup"><span data-stu-id="47a28-169">Learn more here.</span></span> 

<span data-ttu-id="47a28-170">**將多個 Azure AD 租用戶新增至單一合作夥伴中心帳戶時是否有任何限制？**</span><span class="sxs-lookup"><span data-stu-id="47a28-170">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="47a28-171">如果 Azure AD 租用戶已與現有的合作夥伴中心帳戶相關聯，則無法使用多租用戶功能將其與新的合作夥伴中心帳戶產生關聯。</span><span class="sxs-lookup"><span data-stu-id="47a28-171">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="47a28-172">另一方面也須考量，一個 Azure AD 租用戶只能與一個合作夥伴中心帳戶相關聯，但一個合作夥伴中心帳戶可以有多個相關聯的租用戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-172">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="47a28-173">Microsoft 合作夥伴網路 (MPN) 成員資格移轉</span><span class="sxs-lookup"><span data-stu-id="47a28-173">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="47a28-174">**從 PMC 到合作夥伴中心的移轉可由誰執行？**</span><span class="sxs-lookup"><span data-stu-id="47a28-174">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="47a28-175">此移轉可由公司的 MPN 全域管理員或主要計畫連絡人 (這兩個角色通常由同一人擔任) 起始和執行。</span><span class="sxs-lookup"><span data-stu-id="47a28-175">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="47a28-176">**完成移轉的人員是否會在合作夥伴中心的法定公司設定檔中成為主要連絡人？**</span><span class="sxs-lookup"><span data-stu-id="47a28-176">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="47a28-177">不一定，但主要連絡人必須是有權簽署合約的人。</span><span class="sxs-lookup"><span data-stu-id="47a28-177">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="47a28-178">**Microsoft 可為我移轉 MPN 成員資格嗎？**</span><span class="sxs-lookup"><span data-stu-id="47a28-178">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="47a28-179">不可以。</span><span class="sxs-lookup"><span data-stu-id="47a28-179">No.</span></span> <span data-ttu-id="47a28-180">Microsoft 無法協助您將成員資格帳戶移至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-180">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="47a28-181">您必須使用公司帳戶 (登入認證) 登入 PMC，然後開始進行移轉程序，以移動您的帳戶。</span><span class="sxs-lookup"><span data-stu-id="47a28-181">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="47a28-182">完成移動帳戶的步驟之後，您即可開始管理成員資格，並將使用者角色和權限指派給小組，使其能夠存取權益以及協助管理成員資格。</span><span class="sxs-lookup"><span data-stu-id="47a28-182">After you've completed the steps to move your account, you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="47a28-183">Microsoft 會自動移轉目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含 Partner University 存取權在內的 MCP 關聯。</span><span class="sxs-lookup"><span data-stu-id="47a28-183">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="47a28-184">Microsoft 會自動移轉目前的專長認證、權益、位置資訊、獎勵的銀行/稅務資訊，以及包含 Partner University 存取權在內的 MCP 關聯。</span><span class="sxs-lookup"><span data-stu-id="47a28-184">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="47a28-185">**續約原則將有何變更？**</span><span class="sxs-lookup"><span data-stu-id="47a28-185">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="47a28-186">在合作夥伴中心，續約時間範圍為您的週年日起算的 30 天以內。</span><span class="sxs-lookup"><span data-stu-id="47a28-186">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="47a28-187">**移至合作夥伴中心之後，我們的專長認證會維持原狀嗎？**</span><span class="sxs-lookup"><span data-stu-id="47a28-187">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="47a28-188">是的，移至合作夥伴中心後，專長認證將不受影響。</span><span class="sxs-lookup"><span data-stu-id="47a28-188">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="47a28-189">如果您發現有不一致的情況，請連絡[支援部門](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="47a28-189">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="47a28-190">**移動之後，我的權益 (包括雲端權益、技術支援、軟體權益、Visual Studio) 是否會有變更？**</span><span class="sxs-lookup"><span data-stu-id="47a28-190">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="47a28-191">您的合格權益不會變更。</span><span class="sxs-lookup"><span data-stu-id="47a28-191">Your eligible benefits will not change.</span></span> <span data-ttu-id="47a28-192">如果您發現有不一致的情況，請連絡[支援部門](https://partner.microsoft.com/support)。</span><span class="sxs-lookup"><span data-stu-id="47a28-192">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="47a28-193">**我們具有 Visual Studio 權益配置的 Microsoft 帳戶是否仍將有效？**</span><span class="sxs-lookup"><span data-stu-id="47a28-193">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="47a28-194">是。</span><span class="sxs-lookup"><span data-stu-id="47a28-194">Yes.</span></span> <span data-ttu-id="47a28-195">將會接受並保留配置給 MSA 的 Visual Studio 權益。</span><span class="sxs-lookup"><span data-stu-id="47a28-195">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="47a28-196">在合作夥伴中心中續訂之後，也會保留它們。</span><span class="sxs-lookup"><span data-stu-id="47a28-196">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="47a28-197">不過，如果您在移轉至合作夥伴中心後移除 MSA 配置，便無法將其重新新增至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-197">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="47a28-198">在合作夥伴中心，合作夥伴可以新增公司帳戶及來賓使用者帳戶，其為來自合作夥伴為 Azure AD 租用戶中 MPN 系統管理員之相同租用戶的 MSA。</span><span class="sxs-lookup"><span data-stu-id="47a28-198">In Partner Center, a partner can add work accounts and guest user accounts, which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="47a28-199">如果合作夥伴是多個 Azure AD 租用戶中的全域系統管理員，且這些租用戶都是與相同的合作夥伴中心帳戶相關聯，則該合作夥伴便可以將所有這些租用戶上的使用者加入 Visual Studio 權益和 Azure 以使用量為基礎的配置。</span><span class="sxs-lookup"><span data-stu-id="47a28-199">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="47a28-200">雖然 MPN 系統管理員或全域系統管理員可以將 Visual Studio 以使用量為基礎的訂用帳戶指派給來賓使用者，來賓使用者並無法使用其 MSA 登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="47a28-200">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="47a28-201">不過，來賓使用者可以登入 Azure 和 Visual Studio 以驗證並使用指派給他的權益。</span><span class="sxs-lookup"><span data-stu-id="47a28-201">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="47a28-202">**我們應如何管理 MCP 關聯和 Partner University 存取權？**</span><span class="sxs-lookup"><span data-stu-id="47a28-202">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="47a28-203">從 PMC 移動後，MCP 關聯不會有任何變更。</span><span class="sxs-lookup"><span data-stu-id="47a28-203">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="47a28-204">不過，在移至合作夥伴中心後新增的任何新員工，將必須於合作夥伴中心建立關聯。</span><span class="sxs-lookup"><span data-stu-id="47a28-204">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="47a28-205">現有使用者的所有 Partner University 權限將會保留，但任何新員工都應前往[訓練中心](https://partner.microsoft.com/training)了解如何取得 Partner University 的存取權。</span><span class="sxs-lookup"><span data-stu-id="47a28-205">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="47a28-206">**移至合作夥伴中心後要如何檢視 MCP 資訊？**</span><span class="sxs-lookup"><span data-stu-id="47a28-206">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="47a28-207">在儀表板上的左側導覽中，選取 [專長認證]  。</span><span class="sxs-lookup"><span data-stu-id="47a28-207">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="47a28-208">在 [專長認證]  頁面中，您可以下載技能報告。</span><span class="sxs-lookup"><span data-stu-id="47a28-208">From the **Competencies** page, you are able to download the skills report.</span></span> <span data-ttu-id="47a28-209">技能報告會列出您的哪些使用者已取得與合作夥伴中心的專長認證和計畫有關的技能。</span><span class="sxs-lookup"><span data-stu-id="47a28-209">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="47a28-210">如果您的使用者已獲得技能，但這些技能與您所需的專長認證無關，這些使用者就不會列在報告中。</span><span class="sxs-lookup"><span data-stu-id="47a28-210">If your users have gained skills but those skills are not relevant to the competencies you're working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="47a28-211">**合作夥伴中心是否會使用客戶參考？**</span><span class="sxs-lookup"><span data-stu-id="47a28-211">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="47a28-212">否，要達到合作夥伴中心的專長認證需求，並不需要客戶參考。</span><span class="sxs-lookup"><span data-stu-id="47a28-212">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="47a28-213">**記錄可查夥伴關聯是否會移至合作夥伴中心？**</span><span class="sxs-lookup"><span data-stu-id="47a28-213">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="47a28-214">是，記錄可查夥伴不會變更。</span><span class="sxs-lookup"><span data-stu-id="47a28-214">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="47a28-215">請深入了解[將您的合作夥伴識別碼連結至客戶](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="47a28-215">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="47a28-216">**移至合作夥伴中心是否會影響到獎勵？**</span><span class="sxs-lookup"><span data-stu-id="47a28-216">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="47a28-217">否，如果您在移動帳戶時並未合併位置，獎勵將不受影響。</span><span class="sxs-lookup"><span data-stu-id="47a28-217">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="47a28-218">如果您的公司在 PMC 中有多個帳戶，且您在移至合作夥伴中心時決定將其合併為通用帳戶，您將不會失去獎勵，但獎勵給付可能會有延遲。</span><span class="sxs-lookup"><span data-stu-id="47a28-218">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="47a28-219">如果您未移動所有與獎勵計畫相關的 PMC 帳戶，就可能不會再獲得與這些帳戶繫結的獎勵。</span><span class="sxs-lookup"><span data-stu-id="47a28-219">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="47a28-220">**合作夥伴中心有哪些獎勵使用者角色？**</span><span class="sxs-lookup"><span data-stu-id="47a28-220">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="47a28-221">合作夥伴中心的獎勵角色以位置為基礎，且包含獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="47a28-221">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="47a28-222">若要深入了解這些角色可執行哪些工作，請參閱[指派使用者角色和權限](permissions-overview.md)。</span><span class="sxs-lookup"><span data-stu-id="47a28-222">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="47a28-223">**是否可在全域和位置層級指派獎勵使用者？**</span><span class="sxs-lookup"><span data-stu-id="47a28-223">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="47a28-224">是。</span><span class="sxs-lookup"><span data-stu-id="47a28-224">Yes.</span></span> <span data-ttu-id="47a28-225">您可以將一個獎勵管理員指派為所有位置的獎勵管理員，或是讓每個位置各有其本身的獎勵管理員。</span><span class="sxs-lookup"><span data-stu-id="47a28-225">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="47a28-226">**是否可在全域或位置層級給付獎勵？**</span><span class="sxs-lookup"><span data-stu-id="47a28-226">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="47a28-227">獎勵只會在位置層級給付。</span><span class="sxs-lookup"><span data-stu-id="47a28-227">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="47a28-228">**關於推薦，我們可以建立多少個商務設定檔？**</span><span class="sxs-lookup"><span data-stu-id="47a28-228">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="47a28-229">您的公司可視需要建立數量不限的商務設定檔，以完整展現公司的興趣。</span><span class="sxs-lookup"><span data-stu-id="47a28-229">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="47a28-230">在每個商務設定檔中，您最多可以列出五個位置，每個國家/地區一個位置。</span><span class="sxs-lookup"><span data-stu-id="47a28-230">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="47a28-231">每個商務設定檔分別可接收其對應位置的推薦。</span><span class="sxs-lookup"><span data-stu-id="47a28-231">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="47a28-232">**如何指派推薦，預期會有哪些變更？例如，如果我在某個市場有一個全球性公司，而在其他市場有一些位置，則應如何指派推薦？**</span><span class="sxs-lookup"><span data-stu-id="47a28-232">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="47a28-233">系統會根據客戶定義的搜尋參數來指派推薦。</span><span class="sxs-lookup"><span data-stu-id="47a28-233">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="47a28-234">因此，不論您是有一個還是多個位置，在客戶指定了所需的位置後，如果您有符合其他參數的業務，則會將推薦指派至該位置。</span><span class="sxs-lookup"><span data-stu-id="47a28-234">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








