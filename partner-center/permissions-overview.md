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
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434317"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="30e94-103">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="30e94-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="30e94-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-104">**Appropriate roles**</span></span>

- <span data-ttu-id="30e94-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-105">Global admin</span></span>
- <span data-ttu-id="30e94-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-106">User admin</span></span>
- <span data-ttu-id="30e94-107">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-107">MPN partner admin</span></span>

<span data-ttu-id="30e94-108">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="30e94-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="30e94-109">後續步驟：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="30e94-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="30e94-110">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="30e94-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="30e94-111">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="30e94-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="30e94-112">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="30e94-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="30e94-113">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure AD 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="30e94-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="30e94-114">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="30e94-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="30e94-115">Azure Active Directory (AAD) 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="30e94-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="30e94-116">非 AAD 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="30e94-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="30e94-117">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="30e94-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="30e94-118">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-118">**Role**</span></span>|<span data-ttu-id="30e94-119">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="30e94-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="30e94-120">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-120">Global admin</span></span>|<span data-ttu-id="30e94-121">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="30e94-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="30e94-122">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="30e94-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="30e94-123">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="30e94-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="30e94-124">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="30e94-125">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="30e94-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="30e94-126">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-126">User management admin</span></span>   | <span data-ttu-id="30e94-127">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="30e94-128">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="30e94-129">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="30e94-130">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-130">Billing admin</span></span> | <span data-ttu-id="30e94-131">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="30e94-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="30e94-132">預設使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-132">Default user</span></span>|  <span data-ttu-id="30e94-133">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-133">View My profile</span></span>   |
|<span data-ttu-id="30e94-134">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="30e94-134">Admin agent</span></span> | <span data-ttu-id="30e94-135">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="30e94-135">\*    Customer management</span></span>
||<span data-ttu-id="30e94-136">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="30e94-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="30e94-137">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="30e94-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="30e94-138">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="30e94-138">\*    Subscription management</span></span>
||<span data-ttu-id="30e94-139">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="30e94-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="30e94-140">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="30e94-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="30e94-141">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="30e94-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="30e94-142">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="30e94-142">\*    Billing</span></span>
||<span data-ttu-id="30e94-143">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="30e94-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="30e94-144">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="30e94-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="30e94-145">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="30e94-145">Sales agent</span></span> | <span data-ttu-id="30e94-146">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="30e94-146">\*    Customer management</span></span>
||<span data-ttu-id="30e94-147">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="30e94-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="30e94-148">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="30e94-148">\*    Subscription management</span></span>
||<span data-ttu-id="30e94-149">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="30e94-149">\*    View support tickets</span></span>
||<span data-ttu-id="30e94-150">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="30e94-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="30e94-151">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="30e94-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="30e94-152">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="30e94-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="30e94-153">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="30e94-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="30e94-154">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="30e94-154">Helpdesk agent</span></span>| <span data-ttu-id="30e94-155">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="30e94-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="30e94-156">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="30e94-156">\*    Edit customer details</span></span>
||<span data-ttu-id="30e94-157">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="30e94-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="30e94-158">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="30e94-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="30e94-159">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="30e94-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="30e94-160">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="30e94-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="30e94-161">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="30e94-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="30e94-162">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="30e94-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="30e94-163">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-163">**Role**</span></span>   |<span data-ttu-id="30e94-164">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="30e94-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="30e94-165">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-165">Global admin</span></span>| <span data-ttu-id="30e94-166">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="30e94-167">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="30e94-168">來賓使用者 (必須新增至 AAD 租用戶)</span><span class="sxs-lookup"><span data-stu-id="30e94-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="30e94-169">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="30e94-169">**Guest user**</span></span>   | <span data-ttu-id="30e94-170">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="30e94-171">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-171">MPN partner admin</span></span>|
||<span data-ttu-id="30e94-172">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-172">Accounts admin</span></span>|
||<span data-ttu-id="30e94-173">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-173">Incentives admin</span></span>|
||<span data-ttu-id="30e94-174">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-174">Business profile admin</span></span>|
||<span data-ttu-id="30e94-175">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="30e94-176">管理 MPN 成員資格和您的公司 (非 AAD 角色：這些角色會管理公司業務，而不是租用戶)</span><span class="sxs-lookup"><span data-stu-id="30e94-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="30e94-177">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-177">**Role**</span></span> | <span data-ttu-id="30e94-178">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="30e94-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="30e94-179">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-179">MPN partner admin</span></span>|<span data-ttu-id="30e94-180">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="30e94-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="30e94-181">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="30e94-182">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="30e94-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="30e94-183">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="30e94-183">\*    View competencies</span></span>
||<span data-ttu-id="30e94-184">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="30e94-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="30e94-185">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="30e94-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="30e94-186">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="30e94-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="30e94-187">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="30e94-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="30e94-188">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="30e94-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="30e94-189">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="30e94-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="30e94-190">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="30e94-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="30e94-191">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-191">Account admin</span></span>| <span data-ttu-id="30e94-192">新增位置</span><span class="sxs-lookup"><span data-stu-id="30e94-192">Add locations</span></span>
|| <span data-ttu-id="30e94-193">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="30e94-194">\*    將租用戶中使用者的角色指派至非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="30e94-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="30e94-195">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="30e94-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="30e94-196">管理推薦</span><span class="sxs-lookup"><span data-stu-id="30e94-196">Manage referrals</span></span> 

|<span data-ttu-id="30e94-197">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-197">**Role**</span></span>|<span data-ttu-id="30e94-198">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="30e94-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="30e94-199">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-199">Referrals admin</span></span>       |<span data-ttu-id="30e94-200">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="30e94-201">\*    接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="30e94-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="30e94-202">\*    檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="30e94-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="30e94-203">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="30e94-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="30e94-204">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-204">Business profile admin</span></span>   |<span data-ttu-id="30e94-205">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="30e94-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="30e94-206">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="30e94-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="30e94-207">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="30e94-207">Manage incentives</span></span> 

|<span data-ttu-id="30e94-208">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-208">**Role**</span></span> | <span data-ttu-id="30e94-209">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="30e94-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="30e94-210">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="30e94-210">Incentives admin</span></span>|<span data-ttu-id="30e94-211">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="30e94-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="30e94-212">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="30e94-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="30e94-213">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="30e94-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="30e94-214">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="30e94-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="30e94-215">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="30e94-215">\*    Access support</span></span>
||<span data-ttu-id="30e94-216">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="30e94-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="30e94-217">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="30e94-217">Incentives user</span></span>|<span data-ttu-id="30e94-218">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="30e94-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="30e94-219">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="30e94-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="30e94-220">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="30e94-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="30e94-221">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="30e94-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="30e94-222">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="30e94-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="30e94-223">**角色**</span><span class="sxs-lookup"><span data-stu-id="30e94-223">**Role**</span></span> | <span data-ttu-id="30e94-224">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="30e94-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="30e94-225">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="30e94-225">Executive report viewer</span></span>|<span data-ttu-id="30e94-226">存取所有報告資料集</span><span class="sxs-lookup"><span data-stu-id="30e94-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="30e94-227">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="30e94-227">Report viewer</span></span>|<span data-ttu-id="30e94-228">存取具有營收、客戶和員工個人資料例外狀況的資料報告</span><span class="sxs-lookup"><span data-stu-id="30e94-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    