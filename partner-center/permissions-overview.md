---
title: 指派使用者角色和權限 | 合作夥伴中心
ms.topic: article
ms.date: 10/10/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 需要在合作夥伴中心裡工作的每位員工，都必須有指派的角色。
author: LauraBrenner
ms.author: labrenne
keywords: 角色, 權限, 系統管理員, 代理人
ms.localizationpriority: high
ms.openlocfilehash: aa2eb2561332f730abedd2416813189abe6dc02d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652425"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="88ea2-104">指派使用者角色和權限</span><span class="sxs-lookup"><span data-stu-id="88ea2-104">Assign users roles and permissions</span></span>


<span data-ttu-id="88ea2-105">您已設定您的合作夥伴設定檔，包括合法的名稱和地址、支援詳細資料、免稅證明、銀行資訊，以及貴公司的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="88ea2-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="88ea2-106">下一步：讓您的使用者以密碼和角色進行設定，讓他們可以開始在合作夥伴中心與您合作。</span><span class="sxs-lookup"><span data-stu-id="88ea2-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="88ea2-107">設定您的員工以在合作夥伴中心工作</span><span class="sxs-lookup"><span data-stu-id="88ea2-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="88ea2-108">您可以依據您給予使用者的角色和權限，來決定他們對合作夥伴中心所擁有的存取類型。</span><span class="sxs-lookup"><span data-stu-id="88ea2-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="88ea2-109">角色與您的企業所牽涉的計畫相關。</span><span class="sxs-lookup"><span data-stu-id="88ea2-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="88ea2-110">例如，如果您的企業是雲端解決方案提供者 (CSP) 企業，您不僅要使用標準的 Azure AD 租用戶管理角色 (例如全域管理員)，還需要 CSP 計畫專屬的角色。</span><span class="sxs-lookup"><span data-stu-id="88ea2-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="88ea2-111">每個計畫都有其特有的角色。</span><span class="sxs-lookup"><span data-stu-id="88ea2-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="88ea2-112">Azure Active Directory (AAD) 租用戶角色包含全域管理員、使用者管理員和 CSP 角色。</span><span class="sxs-lookup"><span data-stu-id="88ea2-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="88ea2-113">非 AAD 角色是指不管理租用戶的角色，包括 MPN 管理員、商務設定檔管理員、推薦管理員、獎勵管理員和獎勵使用者。</span><span class="sxs-lookup"><span data-stu-id="88ea2-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="88ea2-114">在合作夥伴中心管理商業交易 (Azure AD 和 CSP 角色)</span><span class="sxs-lookup"><span data-stu-id="88ea2-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="88ea2-115">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-115">**Role**</span></span>|<span data-ttu-id="88ea2-116">**可以執行的動作**</span><span class="sxs-lookup"><span data-stu-id="88ea2-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="88ea2-117">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-117">Global admin</span></span>|<span data-ttu-id="88ea2-118">• 具有能存取所有 Microsoft 帳戶/服務的完整權限</span><span class="sxs-lookup"><span data-stu-id="88ea2-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="88ea2-119">• 建立合作夥伴中心的支援票證</span><span class="sxs-lookup"><span data-stu-id="88ea2-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="88ea2-120">• 檢視合約、價格清單和優惠</span><span class="sxs-lookup"><span data-stu-id="88ea2-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="88ea2-121">• 檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="88ea2-122">檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="88ea2-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="88ea2-123">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-123">User management admin</span></span>   | <span data-ttu-id="88ea2-124">• 檢視、建立和管理使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="88ea2-125">• 檢視所有合作夥伴設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-125">• View all partner profiles</span></span>
||<span data-ttu-id="88ea2-126">• 檢視、建立和管理合作夥伴使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="88ea2-127">帳單管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-127">Billing admin</span></span> | <span data-ttu-id="88ea2-128">- 檢視、建立和管理帳單、發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="88ea2-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="88ea2-129">預設使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-129">Default user</span></span>|  <span data-ttu-id="88ea2-130">檢視我的設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-130">View My profile</span></span>   |
|<span data-ttu-id="88ea2-131">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="88ea2-131">Admin agent</span></span> | <span data-ttu-id="88ea2-132">• 客戶管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-132">•    Customer management</span></span>
||<span data-ttu-id="88ea2-133">• 將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="88ea2-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="88ea2-134">• 建立設定檔並將其套用至裝置</span><span class="sxs-lookup"><span data-stu-id="88ea2-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="88ea2-135">• 訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-135">• Subscription management</span></span>
||<span data-ttu-id="88ea2-136">• 客戶的服務健康狀況和服務要求</span><span class="sxs-lookup"><span data-stu-id="88ea2-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="88ea2-137">• 要求委派的系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="88ea2-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="88ea2-138">• 檢視定價和供應項目</span><span class="sxs-lookup"><span data-stu-id="88ea2-138">• View pricing and offers</span></span>
||<span data-ttu-id="88ea2-139">• 計費</span><span class="sxs-lookup"><span data-stu-id="88ea2-139">• Billing</span></span>
||<span data-ttu-id="88ea2-140">• 代表客戶管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="88ea2-141">• 註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="88ea2-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="88ea2-142">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="88ea2-142">Sales agent</span></span> | <span data-ttu-id="88ea2-143">• 客戶管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-143">•    Customer management</span></span>
||<span data-ttu-id="88ea2-144">• 將裝置清單新增至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="88ea2-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="88ea2-145">• 訂用帳戶管理</span><span class="sxs-lookup"><span data-stu-id="88ea2-145">• Subscription management</span></span>
||<span data-ttu-id="88ea2-146">• 檢視支援票證</span><span class="sxs-lookup"><span data-stu-id="88ea2-146">• View support tickets</span></span>
||<span data-ttu-id="88ea2-147">• 要求與客戶建立關係</span><span class="sxs-lookup"><span data-stu-id="88ea2-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="88ea2-148">• 管理潛在客戶</span><span class="sxs-lookup"><span data-stu-id="88ea2-148">• Manage customer leads</span></span>
||<span data-ttu-id="88ea2-149">• 檢視客戶合約</span><span class="sxs-lookup"><span data-stu-id="88ea2-149">• View the customer agreement</span></span>
||<span data-ttu-id="88ea2-150">• 註冊加值型經銷商</span><span class="sxs-lookup"><span data-stu-id="88ea2-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="88ea2-151">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="88ea2-151">Helpdesk agent</span></span>| <span data-ttu-id="88ea2-152">• 搜尋並檢視客戶</span><span class="sxs-lookup"><span data-stu-id="88ea2-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="88ea2-153">• 編輯客戶詳細資料</span><span class="sxs-lookup"><span data-stu-id="88ea2-153">• Edit customer details</span></span>
||<span data-ttu-id="88ea2-154">• 協助解決客戶的帳單及訂閱管理問題</span><span class="sxs-lookup"><span data-stu-id="88ea2-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="88ea2-155">• 代表客戶要求支援 (注意：您必須是系統管理員代理人，才能針對 Office 365 訂閱完成此工作)</span><span class="sxs-lookup"><span data-stu-id="88ea2-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="88ea2-156">•代表客戶管理訂閱和計費問題 (注意：您必須是系統管理員代理人，才能針對 Office 365 訂閱完成此工作)</span><span class="sxs-lookup"><span data-stu-id="88ea2-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="88ea2-157">控制台廠商 (CPV)。</span><span class="sxs-lookup"><span data-stu-id="88ea2-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="88ea2-158">(CSP 角色和非 AAD 角色)</span><span class="sxs-lookup"><span data-stu-id="88ea2-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="88ea2-159">CPV 開發可供雲端解決方案提供者 (CSP) 合作夥伴使用的應用程式，讓他們能夠整合其系統與合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="88ea2-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="88ea2-160">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-160">**Role**</span></span>   |<span data-ttu-id="88ea2-161">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="88ea2-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="88ea2-162">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-162">Global admin</span></span>| <span data-ttu-id="88ea2-163">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="88ea2-164">檢視及管理您需要存取 CPV 功能的任何使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="88ea2-165">來賓使用者 (必須新增至 AAD 租用戶)</span><span class="sxs-lookup"><span data-stu-id="88ea2-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="88ea2-166">**來賓使用者**</span><span class="sxs-lookup"><span data-stu-id="88ea2-166">**Guest user**</span></span>   | <span data-ttu-id="88ea2-167">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="88ea2-168">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-168">MPN partner admin</span></span>|
||<span data-ttu-id="88ea2-169">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-169">Accounts admin</span></span>|
||<span data-ttu-id="88ea2-170">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-170">Incentives admin</span></span>|
||<span data-ttu-id="88ea2-171">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-171">Business profile admin</span></span>|
||<span data-ttu-id="88ea2-172">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="88ea2-173">管理 MPN 成員資格和您的公司 (非 AAD 角色：這些角色會管理公司業務，而不是租用戶)</span><span class="sxs-lookup"><span data-stu-id="88ea2-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="88ea2-174">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-174">**Role**</span></span> | <span data-ttu-id="88ea2-175">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="88ea2-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="88ea2-176">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-176">MPN partner admin</span></span>|<span data-ttu-id="88ea2-177">• 檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="88ea2-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="88ea2-178">• 檢視法律、公司、商務和 MPN 設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="88ea2-179">• 檢視使用者詳細資料及其技能資料</span><span class="sxs-lookup"><span data-stu-id="88ea2-179">• View user details and their skills data</span></span>
||<span data-ttu-id="88ea2-180">• 檢視專長認證</span><span class="sxs-lookup"><span data-stu-id="88ea2-180">• View competencies</span></span>
||<span data-ttu-id="88ea2-181">• 檢視及管理權益</span><span class="sxs-lookup"><span data-stu-id="88ea2-181">• View and manage benefits</span></span>
||<span data-ttu-id="88ea2-182">• 檢視及購買 MPN 供應項目</span><span class="sxs-lookup"><span data-stu-id="88ea2-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="88ea2-183">• 檢視 MPN 供應項目訂購記錄和發票</span><span class="sxs-lookup"><span data-stu-id="88ea2-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="88ea2-184">• 檢視合作夥伴貢獻指標資料</span><span class="sxs-lookup"><span data-stu-id="88ea2-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="88ea2-185">• 可以使用「憑券驗證」工具工作</span><span class="sxs-lookup"><span data-stu-id="88ea2-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="88ea2-186">- 檢視客戶資料分析</span><span class="sxs-lookup"><span data-stu-id="88ea2-186">- View customer data analytics</span></span>
|| <span data-ttu-id="88ea2-187">檢視公司內的其他使用者角色，但無法指派角色</span><span class="sxs-lookup"><span data-stu-id="88ea2-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="88ea2-188">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-188">Account admin</span></span>| <span data-ttu-id="88ea2-189">新增位置</span><span class="sxs-lookup"><span data-stu-id="88ea2-189">Add locations</span></span>
|| <span data-ttu-id="88ea2-190">管理與您身為系統管理員的帳戶相關的設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="88ea2-191">• 將租用戶中使用者的角色指派給非 AAD 角色</span><span class="sxs-lookup"><span data-stu-id="88ea2-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="88ea2-192">• 在計畫中註冊位置</span><span class="sxs-lookup"><span data-stu-id="88ea2-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="88ea2-193">管理推薦</span><span class="sxs-lookup"><span data-stu-id="88ea2-193">Manage referrals</span></span> 

|<span data-ttu-id="88ea2-194">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-194">**Role**</span></span>|<span data-ttu-id="88ea2-195">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="88ea2-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="88ea2-196">推薦管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-196">Referrals admin</span></span>       |<span data-ttu-id="88ea2-197">• 檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="88ea2-198">• 接收及管理推薦</span><span class="sxs-lookup"><span data-stu-id="88ea2-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="88ea2-199">• 檢視、建立和管理共同銷售推薦</span><span class="sxs-lookup"><span data-stu-id="88ea2-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="88ea2-200">• 檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="88ea2-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="88ea2-201">商務設定檔管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-201">Business profile admin</span></span>   |<span data-ttu-id="88ea2-202">• 檢視、建立和管理商務設定檔</span><span class="sxs-lookup"><span data-stu-id="88ea2-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="88ea2-203">• 檢視、建立和管理合作夥伴服務要求</span><span class="sxs-lookup"><span data-stu-id="88ea2-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="88ea2-204">管理獎勵</span><span class="sxs-lookup"><span data-stu-id="88ea2-204">Manage incentives</span></span> 

|<span data-ttu-id="88ea2-205">**角色**</span><span class="sxs-lookup"><span data-stu-id="88ea2-205">**Role**</span></span> | <span data-ttu-id="88ea2-206">**可以執行的作業**</span><span class="sxs-lookup"><span data-stu-id="88ea2-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="88ea2-207">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="88ea2-207">Incentives admin</span></span>|<span data-ttu-id="88ea2-208">• 起始及管理獎勵</span><span class="sxs-lookup"><span data-stu-id="88ea2-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="88ea2-209">• 可以檢視和編輯獎勵計畫的各個層面</span><span class="sxs-lookup"><span data-stu-id="88ea2-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="88ea2-210">• 可以檢視和編輯銀行及稅務詳細資料</span><span class="sxs-lookup"><span data-stu-id="88ea2-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="88ea2-211">• 檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="88ea2-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="88ea2-212">• 存取支援</span><span class="sxs-lookup"><span data-stu-id="88ea2-212">• Access support</span></span>
||<span data-ttu-id="88ea2-213">• 爭議獎勵付款</span><span class="sxs-lookup"><span data-stu-id="88ea2-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="88ea2-214">獎勵使用者</span><span class="sxs-lookup"><span data-stu-id="88ea2-214">Incentives user</span></span>|<span data-ttu-id="88ea2-215">• 可以檢視獎勵計畫</span><span class="sxs-lookup"><span data-stu-id="88ea2-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="88ea2-216">• 可以檢視和起始獎勵宣告</span><span class="sxs-lookup"><span data-stu-id="88ea2-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="88ea2-217">• 檢視回贈和合作收益</span><span class="sxs-lookup"><span data-stu-id="88ea2-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="88ea2-218">• 存取支援</span><span class="sxs-lookup"><span data-stu-id="88ea2-218">• Access support</span></span>












