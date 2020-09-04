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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040764"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="53c3e-103">為需要在合作夥伴中心工作的公司使用者指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="53c3e-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="53c3e-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="53c3e-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-105">Global admin</span></span>
- <span data-ttu-id="53c3e-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-106">User admin</span></span>
- <span data-ttu-id="53c3e-107">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-107">MPN partner admin</span></span>

<span data-ttu-id="53c3e-108">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="53c3e-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="53c3e-109">後續步驟：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="53c3e-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="53c3e-110">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="53c3e-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="53c3e-111">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="53c3e-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="53c3e-112">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="53c3e-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="53c3e-113">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure AD 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="53c3e-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="53c3e-114">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="53c3e-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="53c3e-115">Azure Active Directory (AAD) 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="53c3e-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="53c3e-116">非 AAD 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="53c3e-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="53c3e-117">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="53c3e-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="53c3e-118">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-118">**Role**</span></span>|<span data-ttu-id="53c3e-119">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="53c3e-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="53c3e-120">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-120">Global admin</span></span>|<span data-ttu-id="53c3e-121">\*    具有存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="53c3e-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="53c3e-122">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-123">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="53c3e-124">\*    檢視合約、價格清單和供應項目</span><span class="sxs-lookup"><span data-stu-id="53c3e-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="53c3e-125">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="53c3e-126">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="53c3e-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="53c3e-127">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-127">User management admin</span></span>   | <span data-ttu-id="53c3e-128">\*    檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="53c3e-129">\*    檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="53c3e-130">\*    檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="53c3e-131">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-132">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="53c3e-133">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-133">Billing admin</span></span> | <span data-ttu-id="53c3e-134">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="53c3e-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="53c3e-135">\*    檢視定價</span><span class="sxs-lookup"><span data-stu-id="53c3e-135">\*    View pricing</span></span>
||<span data-ttu-id="53c3e-136">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-137">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="53c3e-138">預設使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-138">Default user</span></span>|  <span data-ttu-id="53c3e-139">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-139">View My profile</span></span>   |
|<span data-ttu-id="53c3e-140">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="53c3e-140">Admin agent</span></span> | <span data-ttu-id="53c3e-141">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="53c3e-141">\*    Customer management</span></span>
||<span data-ttu-id="53c3e-142">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="53c3e-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="53c3e-143">\*    建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="53c3e-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="53c3e-144">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="53c3e-144">\*    Subscription management</span></span>
||<span data-ttu-id="53c3e-145">\*    客戶的服務健康情況與服務要求</span><span class="sxs-lookup"><span data-stu-id="53c3e-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="53c3e-146">\*    要求委派系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="53c3e-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="53c3e-147">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="53c3e-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="53c3e-148">\*    帳單</span><span class="sxs-lookup"><span data-stu-id="53c3e-148">\*    Billing</span></span>
||<span data-ttu-id="53c3e-149">\*    代表客戶進行管理</span><span class="sxs-lookup"><span data-stu-id="53c3e-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="53c3e-150">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="53c3e-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="53c3e-151">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-152">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="53c3e-153">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="53c3e-153">Sales agent</span></span> | <span data-ttu-id="53c3e-154">\*    客戶管理</span><span class="sxs-lookup"><span data-stu-id="53c3e-154">\*    Customer management</span></span>
||<span data-ttu-id="53c3e-155">\*    將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="53c3e-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="53c3e-156">\*    訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="53c3e-156">\*    Subscription management</span></span>
||<span data-ttu-id="53c3e-157">\*    檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-157">\*    View support tickets</span></span>
||<span data-ttu-id="53c3e-158">\*    要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="53c3e-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="53c3e-159">\*    檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="53c3e-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="53c3e-160">\*    管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="53c3e-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="53c3e-161">\*    檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="53c3e-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="53c3e-162">\*    註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="53c3e-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="53c3e-163">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-164">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="53c3e-165">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="53c3e-165">Helpdesk agent</span></span>| <span data-ttu-id="53c3e-166">\*    搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="53c3e-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="53c3e-167">\*    編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="53c3e-167">\*    Edit customer details</span></span>
||<span data-ttu-id="53c3e-168">\*    協助解決客戶的帳單或訂用帳戶管理問題</span><span class="sxs-lookup"><span data-stu-id="53c3e-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="53c3e-169">\*    代表客戶要求支援</span><span class="sxs-lookup"><span data-stu-id="53c3e-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="53c3e-170">\*    代表客戶管理訂用帳戶和帳單問題</span><span class="sxs-lookup"><span data-stu-id="53c3e-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="53c3e-171">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-172">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="53c3e-173">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="53c3e-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="53c3e-174">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="53c3e-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="53c3e-175">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="53c3e-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="53c3e-176">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-176">**Role**</span></span>   |<span data-ttu-id="53c3e-177">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="53c3e-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="53c3e-178">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-178">Global admin</span></span>| <span data-ttu-id="53c3e-179">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="53c3e-180">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="53c3e-181">來賓使用者 (必須新增至 AAD 租用戶)</span><span class="sxs-lookup"><span data-stu-id="53c3e-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="53c3e-182">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="53c3e-182">**Guest user**</span></span>   | <span data-ttu-id="53c3e-183">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="53c3e-184">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-184">MPN partner admin</span></span>|
||<span data-ttu-id="53c3e-185">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-185">Accounts admin</span></span>|
||<span data-ttu-id="53c3e-186">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-186">Incentives admin</span></span>|
||<span data-ttu-id="53c3e-187">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-187">Business profile admin</span></span>|
||<span data-ttu-id="53c3e-188">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="53c3e-189">管理 MPN 成員資格和您的公司 (非 AAD 角色：這些角色會管理公司業務，而不是租用戶)</span><span class="sxs-lookup"><span data-stu-id="53c3e-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="53c3e-190">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-190">**Role**</span></span> | <span data-ttu-id="53c3e-191">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="53c3e-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="53c3e-192">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-192">MPN partner admin</span></span>|<span data-ttu-id="53c3e-193">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="53c3e-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="53c3e-194">\*    檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="53c3e-195">\*    檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="53c3e-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="53c3e-196">\*    檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="53c3e-196">\*    View competencies</span></span>
||<span data-ttu-id="53c3e-197">\*    檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="53c3e-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="53c3e-198">\*    檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="53c3e-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="53c3e-199">\*    檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="53c3e-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="53c3e-200">\*    檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="53c3e-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="53c3e-201">\*    可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="53c3e-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="53c3e-202">\*    檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="53c3e-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="53c3e-203">\*    檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="53c3e-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="53c3e-204">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-205">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="53c3e-206">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-206">Account admin</span></span>| <span data-ttu-id="53c3e-207">新增位置</span><span class="sxs-lookup"><span data-stu-id="53c3e-207">Add locations</span></span>
|| <span data-ttu-id="53c3e-208">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="53c3e-209">\*    將租用戶中使用者的角色指派至非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="53c3e-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="53c3e-210">\*    在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="53c3e-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="53c3e-211">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-212">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="53c3e-213">管理推薦</span><span class="sxs-lookup"><span data-stu-id="53c3e-213">Manage referrals</span></span> 

|<span data-ttu-id="53c3e-214">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-214">**Role**</span></span>|<span data-ttu-id="53c3e-215">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="53c3e-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="53c3e-216">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-216">Referrals admin</span></span>       |<span data-ttu-id="53c3e-217">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="53c3e-218">\*    接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="53c3e-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="53c3e-219">\*    檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="53c3e-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="53c3e-220">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="53c3e-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="53c3e-221">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-221">Business profile admin</span></span>   |<span data-ttu-id="53c3e-222">\*    檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="53c3e-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="53c3e-223">\*    檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="53c3e-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="53c3e-224">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-225">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="53c3e-226">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="53c3e-226">Manage incentives</span></span> 

|<span data-ttu-id="53c3e-227">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-227">**Role**</span></span> | <span data-ttu-id="53c3e-228">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="53c3e-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="53c3e-229">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="53c3e-229">Incentives admin</span></span>|<span data-ttu-id="53c3e-230">\*    起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="53c3e-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="53c3e-231">\*    可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="53c3e-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="53c3e-232">\*    可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="53c3e-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="53c3e-233">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="53c3e-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="53c3e-234">\*    存取支援</span><span class="sxs-lookup"><span data-stu-id="53c3e-234">\*    Access support</span></span>
||<span data-ttu-id="53c3e-235">\*    對獎勵付款提出爭議</span><span class="sxs-lookup"><span data-stu-id="53c3e-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="53c3e-236">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="53c3e-236">Incentives user</span></span>|<span data-ttu-id="53c3e-237">\*    可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="53c3e-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="53c3e-238">\*    可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="53c3e-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="53c3e-239">\*    檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="53c3e-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="53c3e-240">\*    建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="53c3e-241">\*    檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="53c3e-242">檢視合作夥伴中心深入解析資料</span><span class="sxs-lookup"><span data-stu-id="53c3e-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="53c3e-243">**角色**</span><span class="sxs-lookup"><span data-stu-id="53c3e-243">**Role**</span></span> | <span data-ttu-id="53c3e-244">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="53c3e-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="53c3e-245">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="53c3e-245">Executive report viewer</span></span>|<span data-ttu-id="53c3e-246">存取所有報告資料集、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="53c3e-247">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="53c3e-247">Report viewer</span></span>|<span data-ttu-id="53c3e-248">存取具有營收、客戶和員工個人資料例外狀況的資料報告、建立合作夥伴支援票證、檢視您所建立的合作夥伴支援票證</span><span class="sxs-lookup"><span data-stu-id="53c3e-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
