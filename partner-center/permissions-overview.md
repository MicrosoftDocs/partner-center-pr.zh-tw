---
title: 指派使用者角色和權限 | 合作夥伴中心
ms.topic: article
ms.date: 03/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解哪些角色最適合管理商業交易、轉介、獎勵或您公司 MPN 成員資格的使用者。
author: LauraBrenner
ms.author: labrenne
keywords: 角色, 權限, 系統管理員, 代理人
ms.localizationpriority: high
ms.openlocfilehash: 20930ad547bed2399fd60a5c419d8d5c3be8329e
ms.sourcegitcommit: aa33cbd4b3b2f575afcc71ffbdfdc5b45e372f24
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "80226164"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="93cce-104">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="93cce-104">Assign users roles and permissions</span></span>

<span data-ttu-id="93cce-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-105">**Appropriate roles**</span></span>
-    <span data-ttu-id="93cce-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-106">Global admin</span></span>
-    <span data-ttu-id="93cce-107">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-107">User admin</span></span>
-    <span data-ttu-id="93cce-108">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-108">MPN partner admin</span></span>

<span data-ttu-id="93cce-109">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="93cce-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="93cce-110">下一步：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="93cce-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="93cce-111">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="93cce-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="93cce-112">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="93cce-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="93cce-113">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="93cce-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="93cce-114">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure AD 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="93cce-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="93cce-115">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="93cce-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="93cce-116">Azure Active Directory (AAD) 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="93cce-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="93cce-117">非 AAD 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="93cce-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="93cce-118">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="93cce-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="93cce-119">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-119">**Role**</span></span>|<span data-ttu-id="93cce-120">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="93cce-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="93cce-121">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-121">Global admin</span></span>|<span data-ttu-id="93cce-122">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="93cce-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="93cce-123">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="93cce-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="93cce-124">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="93cce-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="93cce-125">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="93cce-126">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="93cce-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="93cce-127">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-127">User management admin</span></span>   | <span data-ttu-id="93cce-128">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="93cce-129">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="93cce-130">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="93cce-131">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-131">Billing admin</span></span> | <span data-ttu-id="93cce-132">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="93cce-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="93cce-133">預設使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-133">Default user</span></span>|  <span data-ttu-id="93cce-134">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-134">View My profile</span></span>   |
|<span data-ttu-id="93cce-135">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="93cce-135">Admin agent</span></span> | <span data-ttu-id="93cce-136">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="93cce-136">\*    Customer management</span></span>
||<span data-ttu-id="93cce-137">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="93cce-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="93cce-138">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="93cce-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="93cce-139">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="93cce-139">\*    Subscription management</span></span>
||<span data-ttu-id="93cce-140">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="93cce-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="93cce-141">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="93cce-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="93cce-142">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="93cce-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="93cce-143">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="93cce-143">\*    Billing</span></span>
||<span data-ttu-id="93cce-144">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="93cce-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="93cce-145">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="93cce-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="93cce-146">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="93cce-146">Sales agent</span></span> | <span data-ttu-id="93cce-147">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="93cce-147">\*    Customer management</span></span>
||<span data-ttu-id="93cce-148">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="93cce-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="93cce-149">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="93cce-149">\*    Subscription management</span></span>
||<span data-ttu-id="93cce-150">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="93cce-150">\*    View support tickets</span></span>
||<span data-ttu-id="93cce-151">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="93cce-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="93cce-152">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="93cce-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="93cce-153">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="93cce-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="93cce-154">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="93cce-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="93cce-155">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="93cce-155">Helpdesk agent</span></span>| <span data-ttu-id="93cce-156">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="93cce-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="93cce-157">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="93cce-157">\*    Edit customer details</span></span>
||<span data-ttu-id="93cce-158">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="93cce-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="93cce-159">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="93cce-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="93cce-160">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="93cce-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="93cce-161">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="93cce-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="93cce-162">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="93cce-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="93cce-163">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="93cce-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="93cce-164">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-164">**Role**</span></span>   |<span data-ttu-id="93cce-165">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="93cce-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="93cce-166">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-166">Global admin</span></span>| <span data-ttu-id="93cce-167">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="93cce-168">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="93cce-169">來賓使用者 (必須新增至 AAD 租用戶)</span><span class="sxs-lookup"><span data-stu-id="93cce-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="93cce-170">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="93cce-170">**Guest user**</span></span>   | <span data-ttu-id="93cce-171">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="93cce-172">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-172">MPN partner admin</span></span>|
||<span data-ttu-id="93cce-173">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-173">Accounts admin</span></span>|
||<span data-ttu-id="93cce-174">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-174">Incentives admin</span></span>|
||<span data-ttu-id="93cce-175">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-175">Business profile admin</span></span>|
||<span data-ttu-id="93cce-176">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="93cce-177">管理 MPN 成員資格和您的公司 (非 AAD 角色：這些角色會管理公司業務，而不是租用戶)</span><span class="sxs-lookup"><span data-stu-id="93cce-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="93cce-178">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-178">**Role**</span></span> | <span data-ttu-id="93cce-179">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="93cce-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="93cce-180">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-180">MPN partner admin</span></span>|<span data-ttu-id="93cce-181">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="93cce-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="93cce-182">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="93cce-183">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="93cce-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="93cce-184">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="93cce-184">\*    View competencies</span></span>
||<span data-ttu-id="93cce-185">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="93cce-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="93cce-186">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="93cce-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="93cce-187">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="93cce-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="93cce-188">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="93cce-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="93cce-189">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="93cce-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="93cce-190">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="93cce-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="93cce-191">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="93cce-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="93cce-192">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-192">Account admin</span></span>| <span data-ttu-id="93cce-193">新增位置</span><span class="sxs-lookup"><span data-stu-id="93cce-193">Add locations</span></span>
|| <span data-ttu-id="93cce-194">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="93cce-195">\*    將租用戶中使用者的角色指派至非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="93cce-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="93cce-196">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="93cce-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="93cce-197">管理推薦</span><span class="sxs-lookup"><span data-stu-id="93cce-197">Manage referrals</span></span> 

|<span data-ttu-id="93cce-198">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-198">**Role**</span></span>|<span data-ttu-id="93cce-199">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="93cce-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="93cce-200">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-200">Referrals admin</span></span>       |<span data-ttu-id="93cce-201">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="93cce-202">\*    接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="93cce-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="93cce-203">\*    檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="93cce-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="93cce-204">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="93cce-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="93cce-205">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-205">Business profile admin</span></span>   |<span data-ttu-id="93cce-206">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="93cce-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="93cce-207">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="93cce-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="93cce-208">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="93cce-208">Manage incentives</span></span> 

|<span data-ttu-id="93cce-209">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-209">**Role**</span></span> | <span data-ttu-id="93cce-210">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="93cce-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="93cce-211">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="93cce-211">Incentives admin</span></span>|<span data-ttu-id="93cce-212">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="93cce-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="93cce-213">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="93cce-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="93cce-214">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="93cce-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="93cce-215">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="93cce-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="93cce-216">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="93cce-216">\*    Access support</span></span>
||<span data-ttu-id="93cce-217">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="93cce-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="93cce-218">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="93cce-218">Incentives user</span></span>|<span data-ttu-id="93cce-219">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="93cce-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="93cce-220">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="93cce-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="93cce-221">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="93cce-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="93cce-222">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="93cce-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="93cce-223">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="93cce-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="93cce-224">**角色**</span><span class="sxs-lookup"><span data-stu-id="93cce-224">**Role**</span></span> | <span data-ttu-id="93cce-225">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="93cce-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="93cce-226">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="93cce-226">Executive report viewer</span></span>|<span data-ttu-id="93cce-227">存取所有報告資料集</span><span class="sxs-lookup"><span data-stu-id="93cce-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="93cce-228">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="93cce-228">Report viewer</span></span>|<span data-ttu-id="93cce-229">存取具有營收、客戶和員工個人資料例外狀況的資料報告</span><span class="sxs-lookup"><span data-stu-id="93cce-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












