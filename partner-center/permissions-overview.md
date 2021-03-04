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
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: 964c0e6be3003c2b3c9da8828d6e896e2fff82f9
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756459"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="d1c87-103">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="d1c87-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="d1c87-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d1c87-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-105">Global admin</span></span>
- <span data-ttu-id="d1c87-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-106">User admin</span></span>
- <span data-ttu-id="d1c87-107">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-107">MPN partner admin</span></span>

<span data-ttu-id="d1c87-108">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="d1c87-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="d1c87-109">後續步驟：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="d1c87-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="d1c87-110">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="d1c87-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="d1c87-111">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="d1c87-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="d1c87-112">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="d1c87-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="d1c87-113">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure Active Directory 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="d1c87-113">For example, if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure Active Directory tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="d1c87-114">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="d1c87-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="d1c87-115">Azure Active Directory 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="d1c87-115">Azure Active Directory tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="d1c87-116">非 Azure Active Directory 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="d1c87-116">Non-Azure-Active-Directory roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="d1c87-117">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="d1c87-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="d1c87-118">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-118">**Role**</span></span>|<span data-ttu-id="d1c87-119">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="d1c87-119">**What they can do**</span></span>|<span data-ttu-id="d1c87-120">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-120">**Learn more**</span></span>|
|----------------------------------|---|:---------------------------------|
|<span data-ttu-id="d1c87-121">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-121">Global admin</span></span>|<span data-ttu-id="d1c87-122">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="d1c87-122">\*    Can access all Microsoft account/services with full privileges</span></span>|[<span data-ttu-id="d1c87-123">管理您的合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="d1c87-123">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
|      |<span data-ttu-id="d1c87-124">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-124">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-125">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-125">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="d1c87-126">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="d1c87-126">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="d1c87-127">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-127">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="d1c87-128">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="d1c87-128">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="d1c87-129">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-129">User management admin</span></span>   | <span data-ttu-id="d1c87-130">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-130">\*    View, create, and manage users</span></span>|[<span data-ttu-id="d1c87-131">在合作夥伴中心管理您的 Microsoft 合作夥伴網路會員資格權益和優惠</span><span class="sxs-lookup"><span data-stu-id="d1c87-131">Manage your Microsoft Partner Network membership benefits and offers in Partner Center</span></span>](manage-your-partner-network-benefits.md)
||<span data-ttu-id="d1c87-132">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-132">\*    View all partner profiles</span></span>
||<span data-ttu-id="d1c87-133">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-133">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-134">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-134">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="d1c87-135">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-135">Billing admin</span></span> | <span data-ttu-id="d1c87-136">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="d1c87-136">- View, create, and manage billing, invoices, and recon files</span></span>|[<span data-ttu-id="d1c87-137">讀取您的帳單</span><span class="sxs-lookup"><span data-stu-id="d1c87-137">Read your bill</span></span>](billing.md)
||<span data-ttu-id="d1c87-138">\*    檢視定價</span><span class="sxs-lookup"><span data-stu-id="d1c87-138">\*    View pricing</span></span>
||<span data-ttu-id="d1c87-139">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-139">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-140">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-140">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="d1c87-141">預設使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-141">Default user</span></span>|  <span data-ttu-id="d1c87-142">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-142">View My profile</span></span>   |[<span data-ttu-id="d1c87-143">重設密碼</span><span class="sxs-lookup"><span data-stu-id="d1c87-143">Reset your password</span></span>](reset-my-pasword.md)
|<span data-ttu-id="d1c87-144">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="d1c87-144">Admin agent</span></span> | <span data-ttu-id="d1c87-145">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-145">\*    Customer management</span></span>|[<span data-ttu-id="d1c87-146">與您的客戶連線</span><span class="sxs-lookup"><span data-stu-id="d1c87-146">Connect with your customers</span></span>](connect-with-your-customers.md)
||<span data-ttu-id="d1c87-147">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="d1c87-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="d1c87-148">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="d1c87-148">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="d1c87-149">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-149">\*    Subscription management</span></span>
||<span data-ttu-id="d1c87-150">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="d1c87-150">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="d1c87-151">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="d1c87-151">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="d1c87-152">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="d1c87-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="d1c87-153">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="d1c87-153">\*    Billing</span></span>
||<span data-ttu-id="d1c87-154">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-154">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="d1c87-155">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="d1c87-155">\*    Register a value added reseller</span></span>
||<span data-ttu-id="d1c87-156">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-156">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-157">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-157">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="d1c87-158">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="d1c87-158">Sales agent</span></span> | <span data-ttu-id="d1c87-159">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-159">\*    Customer management</span></span>|[<span data-ttu-id="d1c87-160">為您的客戶提供計費支援，並協助回答其計費問題</span><span class="sxs-lookup"><span data-stu-id="d1c87-160">Provide billing support for your customers and help answer their billing questions</span></span>](provide-billing-support.md)
||<span data-ttu-id="d1c87-161">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="d1c87-161">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="d1c87-162">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-162">\*    Subscription management</span></span>
||<span data-ttu-id="d1c87-163">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-163">\*    View support tickets</span></span>
||<span data-ttu-id="d1c87-164">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="d1c87-164">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="d1c87-165">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="d1c87-165">\*    View pricing and offers</span></span>
||<span data-ttu-id="d1c87-166">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="d1c87-166">\*    Manage customer leads</span></span>
||<span data-ttu-id="d1c87-167">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="d1c87-167">\*    View the customer agreement</span></span>
||<span data-ttu-id="d1c87-168">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="d1c87-168">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="d1c87-169">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-169">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-170">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-170">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="d1c87-171">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="d1c87-171">Helpdesk agent</span></span>| <span data-ttu-id="d1c87-172">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="d1c87-172">\*    Search for and view a customer</span></span>|[<span data-ttu-id="d1c87-173">將問題呈報給 Microsoft，並了解哪些問題更適合呈報給 Microsoft</span><span class="sxs-lookup"><span data-stu-id="d1c87-173">Escalate problems to Microsoft and learn which issues are more-suited to Microsoft escalation</span></span>](escalate-problems-to-microsoft.md)
||<span data-ttu-id="d1c87-174">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="d1c87-174">\*    Edit customer details</span></span>
||<span data-ttu-id="d1c87-175">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="d1c87-175">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="d1c87-176">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="d1c87-176">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="d1c87-177">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="d1c87-177">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="d1c87-178">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-178">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-179">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-179">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a><span data-ttu-id="d1c87-180">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="d1c87-180">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="d1c87-181">(CSP 角色和非 Azure AD 角色)</span><span class="sxs-lookup"><span data-stu-id="d1c87-181">(CSP role and non-Azure AD role)</span></span>

<span data-ttu-id="d1c87-182">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="d1c87-182">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="d1c87-183">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-183">**Role**</span></span>   |<span data-ttu-id="d1c87-184">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-184">**What you can do**</span></span>|<span data-ttu-id="d1c87-185">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-185">**Learn more**</span></span>|
|------------------------------|:----------------------------|----|
|<span data-ttu-id="d1c87-186">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-186">Global admin</span></span>| <span data-ttu-id="d1c87-187">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-187">View and manage your CPV profile</span></span>|[<span data-ttu-id="d1c87-188">註冊為控制台廠商，以協助整合 CSP 合作夥伴系統與合作夥伴中心 API</span><span class="sxs-lookup"><span data-stu-id="d1c87-188">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>](enroll-as-cpv.md)
||<span data-ttu-id="d1c87-189">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-189">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a><span data-ttu-id="d1c87-190">來賓使用者 (必須新增至 Azure Active Directory 租用戶)</span><span class="sxs-lookup"><span data-stu-id="d1c87-190">Guest user (must be added to the Azure Active Directory tenant)</span></span>

|<span data-ttu-id="d1c87-191">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="d1c87-191">**Guest user**</span></span>   | <span data-ttu-id="d1c87-192">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-192">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="d1c87-193">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-193">MPN partner admin</span></span>|
||<span data-ttu-id="d1c87-194">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-194">Business profile admin</span></span>|
||<span data-ttu-id="d1c87-195">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-195">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company"></a><span data-ttu-id="d1c87-196">管理 MPN 成員資格和您的公司</span><span class="sxs-lookup"><span data-stu-id="d1c87-196">Manage MPN membership and your company</span></span> 

<span data-ttu-id="d1c87-197">這些角色不是 Azure Active Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="d1c87-197">These roles are not Azure Active Directory roles.</span></span> <span data-ttu-id="d1c87-198">這些角色會管理公司業務，而不是租用戶。</span><span class="sxs-lookup"><span data-stu-id="d1c87-198">These roles manage the company business rather than the tenant.</span></span>

|<span data-ttu-id="d1c87-199">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-199">**Role**</span></span> | <span data-ttu-id="d1c87-200">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-200">**What you can do**</span></span>|<span data-ttu-id="d1c87-201">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-201">**Learn more**</span></span>|
|----------------------------|:----------------------------|-----|
|<span data-ttu-id="d1c87-202">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-202">MPN partner admin</span></span>|<span data-ttu-id="d1c87-203">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="d1c87-203">\*    View, create, and manage partner service requests</span></span>|[<span data-ttu-id="d1c87-204">購買或續約 Microsoft 行動套件優惠，或者銀級或金級專長認證</span><span class="sxs-lookup"><span data-stu-id="d1c87-204">Buy or renew a Microsoft Action Pack subscription or silver and gold competencies</span></span>](mpn-get-action-pack.md)
||<span data-ttu-id="d1c87-205">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-205">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="d1c87-206">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="d1c87-206">\*    View user details and their skills data</span></span>
||<span data-ttu-id="d1c87-207">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="d1c87-207">\*    View competencies</span></span>
||<span data-ttu-id="d1c87-208">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="d1c87-208">\*    View and manage benefits</span></span>
||<span data-ttu-id="d1c87-209">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="d1c87-209">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="d1c87-210">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="d1c87-210">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="d1c87-211">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="d1c87-211">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="d1c87-212">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="d1c87-212">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="d1c87-213">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="d1c87-213">\*    View customer data analytics</span></span>
||<span data-ttu-id="d1c87-214">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="d1c87-214">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="d1c87-215">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-215">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-216">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-216">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="d1c87-217">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-217">Account admin</span></span>| <span data-ttu-id="d1c87-218">新增位置</span><span class="sxs-lookup"><span data-stu-id="d1c87-218">Add locations</span></span>|[<span data-ttu-id="d1c87-219">管理位置</span><span class="sxs-lookup"><span data-stu-id="d1c87-219">Manage locations</span></span>](manage-locations.md)
|| <span data-ttu-id="d1c87-220">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-220">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="d1c87-221">\*    將租用戶中使用者的角色指派至非 Azure Active Directory 角色</span><span class="sxs-lookup"><span data-stu-id="d1c87-221">\*    Assign roles for users in tenant to non-Azure-Active-Directory roles</span></span> 
||<span data-ttu-id="d1c87-222">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="d1c87-222">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="d1c87-223">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-223">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-224">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-224">\*    View partner support tickets you create</span></span>

## <a name="manage-referrals"></a><span data-ttu-id="d1c87-225">管理推薦</span><span class="sxs-lookup"><span data-stu-id="d1c87-225">Manage referrals</span></span>

|<span data-ttu-id="d1c87-226">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-226">**Role**</span></span> | <span data-ttu-id="d1c87-227">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-227">**What you can do**</span></span>|<span data-ttu-id="d1c87-228">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-228">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="d1c87-229">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-229">Referrals admin</span></span>|<span data-ttu-id="d1c87-230">在合作夥伴中心的 [推薦] 索引標籤底下建立及管理所有項目</span><span class="sxs-lookup"><span data-stu-id="d1c87-230">Create and manage everything under Referrals tab in Partner Center</span></span>|[<span data-ttu-id="d1c87-231">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="d1c87-231">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="d1c87-232">可以檢視和編輯所有共同銷售商機和潛在客戶</span><span class="sxs-lookup"><span data-stu-id="d1c87-232">Can view and edit all the co-sell opportunities and leads</span></span>
||    <span data-ttu-id="d1c87-233">可以為交易指派小組成員</span><span class="sxs-lookup"><span data-stu-id="d1c87-233">Can assign team members for a deal</span></span>
||    <span data-ttu-id="d1c87-234">可以檢視和編輯商務設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-234">Can view and edit business profiles</span></span>
||    <span data-ttu-id="d1c87-235">可以檢視和註冊已標示為成交且符合交易註冊資格的交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-235">Can view and register deals for opportunities that are marked as won and eligible for deal registration</span></span>
||    <span data-ttu-id="d1c87-236">可以建立和檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-236">Can create and view support tickets</span></span>
|<span data-ttu-id="d1c87-237">推薦使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-237">Referrals user</span></span>|<span data-ttu-id="d1c87-238">只有當共同銷售商機屬於小組一部分時，才能加以建立和管理</span><span class="sxs-lookup"><span data-stu-id="d1c87-238">Create and manage co-sell opportunities only if they are a part of the team</span></span> |[<span data-ttu-id="d1c87-239">管理共同銷售商機</span><span class="sxs-lookup"><span data-stu-id="d1c87-239">Manage Co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
||    <span data-ttu-id="d1c87-240">可以針對為其指派角色時所在的位置建立共同銷售商機。</span><span class="sxs-lookup"><span data-stu-id="d1c87-240">Can create co-sell opportunities for the locations where they are assigned the role.</span></span>
||    <span data-ttu-id="d1c87-241">可以在其屬於小組成員時，檢視和註冊已標示為成交且符合交易註冊資格的交易。</span><span class="sxs-lookup"><span data-stu-id="d1c87-241">Can view and register deals for opportunities that are marked as won and eligible for deal registration if they are team member.</span></span>
||    <span data-ttu-id="d1c87-242">可以建立和檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-242">Can create and view support tickets</span></span>
|<span data-ttu-id="d1c87-243">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-243">Business profile admin</span></span>|<span data-ttu-id="d1c87-244">建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-244">Create and manage business profiles</span></span> | [<span data-ttu-id="d1c87-245">管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="d1c87-245">Manage business profiles</span></span>](create-a-marketing-profile.md)
||    <span data-ttu-id="d1c87-246">可以建立和檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-246">Can create and view support tickets</span></span>

<span data-ttu-id="d1c87-247">除了新的推薦使用者角色外，我們還引進了交易的位置範圍。</span><span class="sxs-lookup"><span data-stu-id="d1c87-247">Along with the new referrals user role, we are also introducing the location scope for deals.</span></span> <span data-ttu-id="d1c87-248">下表說明以位置為基礎的交易存取。</span><span class="sxs-lookup"><span data-stu-id="d1c87-248">The table below explains the deals-access based on the location.</span></span>

|<span data-ttu-id="d1c87-249">**範圍**</span><span class="sxs-lookup"><span data-stu-id="d1c87-249">**Scope**</span></span> | <span data-ttu-id="d1c87-250">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-250">**What you can do**</span></span> |
|------------------------------|:-------------------------|
|<span data-ttu-id="d1c87-251">整個公司</span><span class="sxs-lookup"><span data-stu-id="d1c87-251">Entire company</span></span> | <span data-ttu-id="d1c87-252">管理員和使用者都有權在其公司內的任何位置建立交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-252">Both admins and users have access to create deals for any location in their company</span></span>|
|| <span data-ttu-id="d1c87-253">推薦管理員有權檢視和編輯所有交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-253">Referral admin has access to view and edit all the deals</span></span> |
|| <span data-ttu-id="d1c87-254">只有在屬於小組成員時，推薦使用者才有權檢視和編輯所有交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-254">Referral users have access to view and edit all the deals only if they are a part of the team</span></span> |
|<span data-ttu-id="d1c87-255">一或多個位置</span><span class="sxs-lookup"><span data-stu-id="d1c87-255">One or more locations</span></span> | <span data-ttu-id="d1c87-256">管理員和使用者都有權在其公司內為指派的位置建立交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-256">Both admins and users have access to create deals for the assigned location in their company</span></span>|
|| <span data-ttu-id="d1c87-257">推薦管理員有權檢視和編輯所有屬於已指派位置的交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-257">Referral admin has access to view and edit all the deals belonging to the assigned locations</span></span>|
|| <span data-ttu-id="d1c87-258">如果屬於小組成員，則推薦使用者有權檢視和編輯所有屬於已指派位置的交易</span><span class="sxs-lookup"><span data-stu-id="d1c87-258">Referral users have access to view and edit all the deals belonging to the assigned locations if they are part of the team</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="d1c87-259">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="d1c87-259">Manage incentives</span></span>

|<span data-ttu-id="d1c87-260">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-260">**Role**</span></span> | <span data-ttu-id="d1c87-261">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-261">**What you can do**</span></span>|<span data-ttu-id="d1c87-262">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-262">**Learn more**</span></span>
|------------------------------|:-------------------------|---|
|<span data-ttu-id="d1c87-263">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="d1c87-263">Incentives admin</span></span>|<span data-ttu-id="d1c87-264">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="d1c87-264">\*    Initiates and manages incentives</span></span> |[<span data-ttu-id="d1c87-265">使用這些資源協助您開始使用獎勵</span><span class="sxs-lookup"><span data-stu-id="d1c87-265">Use these resources to help you get started with incentives</span></span>](incentives-get-started-intro.md)
||<span data-ttu-id="d1c87-266">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="d1c87-266">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="d1c87-267">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="d1c87-267">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="d1c87-268">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="d1c87-268">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="d1c87-269">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="d1c87-269">\*    Access support</span></span>
||<span data-ttu-id="d1c87-270">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="d1c87-270">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="d1c87-271">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="d1c87-271">Incentives user</span></span>|<span data-ttu-id="d1c87-272">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="d1c87-272">\*    Can view incentives programs</span></span>
||<span data-ttu-id="d1c87-273">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="d1c87-273">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="d1c87-274">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="d1c87-274">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="d1c87-275">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-275">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="d1c87-276">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-276">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="d1c87-277">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="d1c87-277">View Partner Center Insights data</span></span>

|<span data-ttu-id="d1c87-278">**角色**</span><span class="sxs-lookup"><span data-stu-id="d1c87-278">**Role**</span></span> | <span data-ttu-id="d1c87-279">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="d1c87-279">**What you can do**</span></span>|<span data-ttu-id="d1c87-280">**深入了解**</span><span class="sxs-lookup"><span data-stu-id="d1c87-280">**Learn more**</span></span>|
|------------------------------|:-------------------------|---|
|<span data-ttu-id="d1c87-281">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="d1c87-281">Executive report viewer</span></span>|<span data-ttu-id="d1c87-282">存取所有報告資料集、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-282">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|[<span data-ttu-id="d1c87-283">概述合作夥伴中心深入解析中可用的儀表板報告</span><span class="sxs-lookup"><span data-stu-id="d1c87-283">Overview dashboard reports available in Partner Center Insights</span></span>](pci-overview-report.md)
|<span data-ttu-id="d1c87-284">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="d1c87-284">Report viewer</span></span>|<span data-ttu-id="d1c87-285">存取具有營收、客戶和員工個人資料例外狀況的資料報告、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="d1c87-285">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|

## <a name="next-steps"></a><span data-ttu-id="d1c87-286">後續步驟</span><span class="sxs-lookup"><span data-stu-id="d1c87-286">Next steps</span></span>

- [<span data-ttu-id="d1c87-287">建立使用者帳戶以及指派角色和權限</span><span class="sxs-lookup"><span data-stu-id="d1c87-287">Create user accounts and assign roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)
- [<span data-ttu-id="d1c87-288">在註冊新的合作夥伴中心方案時確認帳戶資訊</span><span class="sxs-lookup"><span data-stu-id="d1c87-288">Verify your account information when you enroll in a new Partner Center program</span></span>](verification-responses.md)
