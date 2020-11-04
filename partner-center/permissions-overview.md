---
title: 將角色和權限指派給使用者
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最適合在合作夥伴中心管理商業交易、推薦、獎勵或 MPN 會員資格的貴公司使用者。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperfq1
ms.openlocfilehash: 6707ede563d07b6b96d2133bd75f8fbd53531875
ms.sourcegitcommit: 98f5eebe7d08ba214ed5a078f1ac770439e41eb7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/31/2020
ms.locfileid: "93133026"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="a8b23-103">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="a8b23-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="a8b23-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a8b23-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-105">Global admin</span></span>
- <span data-ttu-id="a8b23-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-106">User admin</span></span>
- <span data-ttu-id="a8b23-107">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-107">MPN partner admin</span></span>

<span data-ttu-id="a8b23-108">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="a8b23-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="a8b23-109">後續步驟：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="a8b23-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="a8b23-110">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="a8b23-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="a8b23-111">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="a8b23-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="a8b23-112">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="a8b23-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="a8b23-113">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure Active Directory 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="a8b23-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="a8b23-114">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="a8b23-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="a8b23-115">Azure Active Directory 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="a8b23-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="a8b23-116">非 Azure Active Directory 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="a8b23-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="a8b23-117">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="a8b23-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="a8b23-118">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-118">**Role**</span></span>|<span data-ttu-id="a8b23-119">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="a8b23-119">**What they can do**</span></span>|<span data-ttu-id="a8b23-120">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="a8b23-121">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-121">Global admin</span></span>|<span data-ttu-id="a8b23-122">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="a8b23-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="a8b23-123">管理您的合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="a8b23-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="a8b23-124">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-125">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="a8b23-126">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="a8b23-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="a8b23-127">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="a8b23-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="a8b23-128">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="a8b23-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="a8b23-129">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-129">User management admin</span></span>   | <span data-ttu-id="a8b23-130">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="a8b23-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="a8b23-131">在合作夥伴中心管理您的 Microsoft 合作夥伴網路會員資格權益和優惠</span><span class="sxs-lookup"><span data-stu-id="a8b23-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="a8b23-132">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="a8b23-133">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-134">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a8b23-135">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-135">Billing admin</span></span> | <span data-ttu-id="a8b23-136">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="a8b23-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="a8b23-137">讀取您的帳單</span><span class="sxs-lookup"><span data-stu-id="a8b23-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="a8b23-138">\*    檢視定價</span><span class="sxs-lookup"><span data-stu-id="a8b23-138">\*    View pricing</span></span>
||<span data-ttu-id="a8b23-139">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-140">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a8b23-141">預設使用者</span><span class="sxs-lookup"><span data-stu-id="a8b23-141">Default user</span></span>|  <span data-ttu-id="a8b23-142">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-142">View My profile</span></span>   |[<span data-ttu-id="a8b23-143">重設密碼</span><span class="sxs-lookup"><span data-stu-id="a8b23-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="a8b23-144">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="a8b23-144">Admin agent</span></span> | <span data-ttu-id="a8b23-145">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="a8b23-145">\*    Customer management</span></span>|[<span data-ttu-id="a8b23-146">與您的客戶連線</span><span class="sxs-lookup"><span data-stu-id="a8b23-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="a8b23-147">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a8b23-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a8b23-148">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="a8b23-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="a8b23-149">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="a8b23-149">\*    Subscription management</span></span>
||<span data-ttu-id="a8b23-150">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="a8b23-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="a8b23-151">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="a8b23-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="a8b23-152">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="a8b23-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="a8b23-153">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="a8b23-153">\*    Billing</span></span>
||<span data-ttu-id="a8b23-154">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="a8b23-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="a8b23-155">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="a8b23-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="a8b23-156">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-157">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a8b23-158">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="a8b23-158">Sales agent</span></span> | <span data-ttu-id="a8b23-159">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="a8b23-159">\*    Customer management</span></span>|[<span data-ttu-id="a8b23-160">為您的客戶提供計費支援，並協助回答其計費問題</span><span class="sxs-lookup"><span data-stu-id="a8b23-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="a8b23-161">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a8b23-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="a8b23-162">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="a8b23-162">\*    Subscription management</span></span>
||<span data-ttu-id="a8b23-163">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-163">\*    View support tickets</span></span>
||<span data-ttu-id="a8b23-164">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="a8b23-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="a8b23-165">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="a8b23-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="a8b23-166">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="a8b23-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="a8b23-167">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="a8b23-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="a8b23-168">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="a8b23-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="a8b23-169">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-170">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="a8b23-171">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="a8b23-171">Helpdesk agent</span></span>| <span data-ttu-id="a8b23-172">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="a8b23-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="a8b23-173">將問題呈報給 Microsoft，並了解哪些問題更適合呈報給 Microsoft</span><span class="sxs-lookup"><span data-stu-id="a8b23-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="a8b23-174">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="a8b23-174">\*    Edit customer details</span></span>
||<span data-ttu-id="a8b23-175">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="a8b23-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="a8b23-176">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="a8b23-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="a8b23-177">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="a8b23-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="a8b23-178">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-179">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="a8b23-180">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="a8b23-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="a8b23-181">(CSP 角色和非 Azure AD 角色)</span><span class="sxs-lookup"><span data-stu-id="a8b23-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="a8b23-182">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="a8b23-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="a8b23-183">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-183">**Role**</span></span>   |<span data-ttu-id="a8b23-184">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="a8b23-184">**What you can do**</span></span>|<span data-ttu-id="a8b23-185">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="a8b23-186">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-186">Global admin</span></span>| <span data-ttu-id="a8b23-187">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="a8b23-188">註冊為控制台廠商，以協助整合 CSP 合作夥伴系統與合作夥伴中心 API</span><span class="sxs-lookup"><span data-stu-id="a8b23-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="a8b23-189">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="a8b23-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="a8b23-190">來賓使用者 (必須新增至 Azure Active Directory 租用戶)</span><span class="sxs-lookup"><span data-stu-id="a8b23-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="a8b23-191">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="a8b23-191">**Guest user**</span></span>   | <span data-ttu-id="a8b23-192">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="a8b23-193">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-193">MPN partner admin</span></span>|
||<span data-ttu-id="a8b23-194">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-194">Business profile admin</span></span>|
||<span data-ttu-id="a8b23-195">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="a8b23-196">管理 MPN 成員資格和您的公司</span><span class="sxs-lookup"><span data-stu-id="a8b23-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="a8b23-197">這些角色不是 Azure Active Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="a8b23-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="a8b23-198">這些角色會管理公司業務，而不是租用戶。</span><span class="sxs-lookup"><span data-stu-id="a8b23-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="a8b23-199">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-199">**Role**</span></span> | <span data-ttu-id="a8b23-200">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="a8b23-200">**What you can do**</span></span>|<span data-ttu-id="a8b23-201">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="a8b23-202">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-202">MPN partner admin</span></span>|<span data-ttu-id="a8b23-203">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="a8b23-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="a8b23-204">購買或續約 Microsoft 行動套件優惠，或者銀級或金級專長認證</span><span class="sxs-lookup"><span data-stu-id="a8b23-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="a8b23-205">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="a8b23-206">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="a8b23-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="a8b23-207">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="a8b23-207">\*    View competencies</span></span>
||<span data-ttu-id="a8b23-208">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="a8b23-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="a8b23-209">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="a8b23-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="a8b23-210">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="a8b23-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="a8b23-211">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="a8b23-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="a8b23-212">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="a8b23-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="a8b23-213">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="a8b23-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="a8b23-214">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="a8b23-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="a8b23-215">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-216">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="a8b23-217">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-217">Account admin</span></span>| <span data-ttu-id="a8b23-218">新增位置</span><span class="sxs-lookup"><span data-stu-id="a8b23-218">Add locations</span></span>|[<span data-ttu-id="a8b23-219">管理位置</span><span class="sxs-lookup"><span data-stu-id="a8b23-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="a8b23-220">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="a8b23-221">\*    將租用戶中使用者的角色指派至非 Azure Active Directory 角色</span><span class="sxs-lookup"><span data-stu-id="a8b23-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="a8b23-222">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="a8b23-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="a8b23-223">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-224">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-224">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="a8b23-225">管理推薦</span><span class="sxs-lookup"><span data-stu-id="a8b23-225">Manage referrals</span></span> 

|<span data-ttu-id="a8b23-226">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-226">**Role**</span></span>|<span data-ttu-id="a8b23-227">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="a8b23-227">**What you can do**</span></span>|<span data-ttu-id="a8b23-228">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-228">**Learn more**</span></span>|
|-----------------------------|:------------------------|---|
|<span data-ttu-id="a8b23-229">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-229">Referrals admin</span></span>       |<span data-ttu-id="a8b23-230">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-230">\*    View, create, and manage business profiles</span></span>|[<span data-ttu-id="a8b23-231">管理不同的潛在客戶，例如客戶查詢、適合行銷的潛在客戶，以及適合銷售的潛在客戶</span><span class="sxs-lookup"><span data-stu-id="a8b23-231">Manage different leads like customer inquiries, marketing-qualified leads, and sales-qualified leads</span></span>](manage-leads.md)
||<span data-ttu-id="a8b23-232">\*    接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="a8b23-232">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="a8b23-233">\*    檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="a8b23-233">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="a8b23-234">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="a8b23-234">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="a8b23-235">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-235">Business profile admin</span></span>   |<span data-ttu-id="a8b23-236">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-236">\* View, create, and manage business profile</span></span> |[<span data-ttu-id="a8b23-237">建立商務設定檔</span><span class="sxs-lookup"><span data-stu-id="a8b23-237">Create a business profile</span></span>](create-a-marketing-profile.md)
||<span data-ttu-id="a8b23-238">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="a8b23-238">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="a8b23-239">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-239">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-240">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-240">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="a8b23-241">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="a8b23-241">Manage incentives</span></span> 

|<span data-ttu-id="a8b23-242">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-242">**Role**</span></span> | <span data-ttu-id="a8b23-243">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="a8b23-243">**What you can do**</span></span>|<span data-ttu-id="a8b23-244">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-244">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="a8b23-245">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="a8b23-245">Incentives admin</span></span>|<span data-ttu-id="a8b23-246">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="a8b23-246">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="a8b23-247">使用這些資源協助您開始使用獎勵</span><span class="sxs-lookup"><span data-stu-id="a8b23-247">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="a8b23-248">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="a8b23-248">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="a8b23-249">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="a8b23-249">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="a8b23-250">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="a8b23-250">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a8b23-251">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="a8b23-251">\*    Access support</span></span>
||<span data-ttu-id="a8b23-252">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="a8b23-252">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="a8b23-253">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="a8b23-253">Incentives user</span></span>|<span data-ttu-id="a8b23-254">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="a8b23-254">\*    Can view incentives programs</span></span>
||<span data-ttu-id="a8b23-255">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="a8b23-255">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="a8b23-256">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="a8b23-256">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="a8b23-257">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-257">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="a8b23-258">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-258">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="a8b23-259">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="a8b23-259">View Partner Center Insights data</span></span>

|<span data-ttu-id="a8b23-260">**角色**</span><span class="sxs-lookup"><span data-stu-id="a8b23-260">**Role**</span></span> | <span data-ttu-id="a8b23-261">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="a8b23-261">**What you can do**</span></span>|<span data-ttu-id="a8b23-262">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="a8b23-262">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="a8b23-263">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="a8b23-263">Executive report viewer</span></span>|<span data-ttu-id="a8b23-264">存取所有報告資料集、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-264">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="a8b23-265">概述合作夥伴中心深入解析中可用的儀表板報告</span><span class="sxs-lookup"><span data-stu-id="a8b23-265">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="a8b23-266">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="a8b23-266">Report viewer</span></span>|<span data-ttu-id="a8b23-267">存取具有營收、客戶和員工個人資料例外狀況的資料報告、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="a8b23-267">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="a8b23-268">後續步驟</span><span class="sxs-lookup"><span data-stu-id="a8b23-268">Next steps</span></span>

- [<span data-ttu-id="a8b23-269">建立使用者帳戶以及指派角色和權限</span><span class="sxs-lookup"><span data-stu-id="a8b23-269">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="a8b23-270">在註冊新的合作夥伴中心方案時確認帳戶資訊</span><span class="sxs-lookup"><span data-stu-id="a8b23-270">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
