---
title: 將角色和權限指派給使用者
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最適合在合作夥伴中心管理商業交易、推薦、獎勵或 MPN 會員資格的貴公司使用者。
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839183"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="7a7bf-103">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="7a7bf-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="7a7bf-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7a7bf-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-105">Global admin</span></span>
- <span data-ttu-id="7a7bf-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-106">User admin</span></span>
- <span data-ttu-id="7a7bf-107">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-107">MPN partner admin</span></span>

<span data-ttu-id="7a7bf-108">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7a7bf-109">後續步驟：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7a7bf-110">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="7a7bf-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7a7bf-111">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7a7bf-112">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7a7bf-113">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure AD 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7a7bf-114">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7a7bf-115">Azure Active Directory (AAD) 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7a7bf-116">非 AAD 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7a7bf-117">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="7a7bf-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7a7bf-118">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-118">**Role**</span></span>|<span data-ttu-id="7a7bf-119">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7a7bf-120">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-120">Global admin</span></span>|<span data-ttu-id="7a7bf-121">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="7a7bf-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7a7bf-122">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="7a7bf-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7a7bf-123">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="7a7bf-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7a7bf-124">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7a7bf-125">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="7a7bf-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7a7bf-126">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-126">User management admin</span></span>   | <span data-ttu-id="7a7bf-127">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="7a7bf-128">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="7a7bf-129">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7a7bf-130">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-130">Billing admin</span></span> | <span data-ttu-id="7a7bf-131">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="7a7bf-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="7a7bf-132">\*    檢視定價</span><span class="sxs-lookup"><span data-stu-id="7a7bf-132">\*    View pricing</span></span>
|<span data-ttu-id="7a7bf-133">預設使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-133">Default user</span></span>|  <span data-ttu-id="7a7bf-134">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-134">View My profile</span></span>   |
|<span data-ttu-id="7a7bf-135">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="7a7bf-135">Admin agent</span></span> | <span data-ttu-id="7a7bf-136">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="7a7bf-136">\*    Customer management</span></span>
||<span data-ttu-id="7a7bf-137">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="7a7bf-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7a7bf-138">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="7a7bf-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="7a7bf-139">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="7a7bf-139">\*    Subscription management</span></span>
||<span data-ttu-id="7a7bf-140">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="7a7bf-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="7a7bf-141">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="7a7bf-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="7a7bf-142">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="7a7bf-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="7a7bf-143">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="7a7bf-143">\*    Billing</span></span>
||<span data-ttu-id="7a7bf-144">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="7a7bf-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="7a7bf-145">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="7a7bf-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="7a7bf-146">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="7a7bf-146">Sales agent</span></span> | <span data-ttu-id="7a7bf-147">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="7a7bf-147">\*    Customer management</span></span>
||<span data-ttu-id="7a7bf-148">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="7a7bf-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="7a7bf-149">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="7a7bf-149">\*    Subscription management</span></span>
||<span data-ttu-id="7a7bf-150">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="7a7bf-150">\*    View support tickets</span></span>
||<span data-ttu-id="7a7bf-151">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="7a7bf-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="7a7bf-152">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="7a7bf-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="7a7bf-153">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="7a7bf-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="7a7bf-154">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="7a7bf-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="7a7bf-155">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="7a7bf-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="7a7bf-156">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="7a7bf-156">Helpdesk agent</span></span>| <span data-ttu-id="7a7bf-157">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="7a7bf-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="7a7bf-158">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="7a7bf-158">\*    Edit customer details</span></span>
||<span data-ttu-id="7a7bf-159">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="7a7bf-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7a7bf-160">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="7a7bf-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="7a7bf-161">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="7a7bf-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7a7bf-162">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7a7bf-163">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="7a7bf-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7a7bf-164">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="7a7bf-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7a7bf-165">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-165">**Role**</span></span>   |<span data-ttu-id="7a7bf-166">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7a7bf-167">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-167">Global admin</span></span>| <span data-ttu-id="7a7bf-168">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7a7bf-169">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7a7bf-170">來賓使用者 (必須新增至 AAD 租用戶)</span><span class="sxs-lookup"><span data-stu-id="7a7bf-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7a7bf-171">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-171">**Guest user**</span></span>   | <span data-ttu-id="7a7bf-172">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7a7bf-173">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-173">MPN partner admin</span></span>|
||<span data-ttu-id="7a7bf-174">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-174">Accounts admin</span></span>|
||<span data-ttu-id="7a7bf-175">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-175">Incentives admin</span></span>|
||<span data-ttu-id="7a7bf-176">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-176">Business profile admin</span></span>|
||<span data-ttu-id="7a7bf-177">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7a7bf-178">管理 MPN 成員資格和您的公司 (非 AAD 角色：這些角色會管理公司業務，而不是租用戶)</span><span class="sxs-lookup"><span data-stu-id="7a7bf-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7a7bf-179">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-179">**Role**</span></span> | <span data-ttu-id="7a7bf-180">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7a7bf-181">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-181">MPN partner admin</span></span>|<span data-ttu-id="7a7bf-182">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="7a7bf-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7a7bf-183">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7a7bf-184">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="7a7bf-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="7a7bf-185">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="7a7bf-185">\*    View competencies</span></span>
||<span data-ttu-id="7a7bf-186">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="7a7bf-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="7a7bf-187">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="7a7bf-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="7a7bf-188">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="7a7bf-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7a7bf-189">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="7a7bf-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="7a7bf-190">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="7a7bf-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7a7bf-191">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="7a7bf-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="7a7bf-192">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="7a7bf-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7a7bf-193">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-193">Account admin</span></span>| <span data-ttu-id="7a7bf-194">新增位置</span><span class="sxs-lookup"><span data-stu-id="7a7bf-194">Add locations</span></span>
|| <span data-ttu-id="7a7bf-195">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7a7bf-196">\*    將租用戶中使用者的角色指派至非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="7a7bf-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7a7bf-197">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="7a7bf-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7a7bf-198">管理推薦</span><span class="sxs-lookup"><span data-stu-id="7a7bf-198">Manage referrals</span></span> 

|<span data-ttu-id="7a7bf-199">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-199">**Role**</span></span>|<span data-ttu-id="7a7bf-200">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7a7bf-201">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-201">Referrals admin</span></span>       |<span data-ttu-id="7a7bf-202">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="7a7bf-203">\*    接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="7a7bf-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="7a7bf-204">\*    檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="7a7bf-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7a7bf-205">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="7a7bf-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7a7bf-206">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-206">Business profile admin</span></span>   |<span data-ttu-id="7a7bf-207">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="7a7bf-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="7a7bf-208">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="7a7bf-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7a7bf-209">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="7a7bf-209">Manage incentives</span></span> 

|<span data-ttu-id="7a7bf-210">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-210">**Role**</span></span> | <span data-ttu-id="7a7bf-211">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7a7bf-212">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-212">Incentives admin</span></span>|<span data-ttu-id="7a7bf-213">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="7a7bf-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="7a7bf-214">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="7a7bf-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7a7bf-215">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="7a7bf-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7a7bf-216">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="7a7bf-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7a7bf-217">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="7a7bf-217">\*    Access support</span></span>
||<span data-ttu-id="7a7bf-218">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="7a7bf-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="7a7bf-219">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="7a7bf-219">Incentives user</span></span>|<span data-ttu-id="7a7bf-220">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="7a7bf-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="7a7bf-221">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="7a7bf-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7a7bf-222">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="7a7bf-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="7a7bf-223">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="7a7bf-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="7a7bf-224">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="7a7bf-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="7a7bf-225">**角色**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-225">**Role**</span></span> | <span data-ttu-id="7a7bf-226">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="7a7bf-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7a7bf-227">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-227">Executive report viewer</span></span>|<span data-ttu-id="7a7bf-228">存取所有報告資料集</span><span class="sxs-lookup"><span data-stu-id="7a7bf-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="7a7bf-229">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="7a7bf-229">Report viewer</span></span>|<span data-ttu-id="7a7bf-230">存取具有營收、客戶和員工個人資料例外狀況的資料報告</span><span class="sxs-lookup"><span data-stu-id="7a7bf-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
