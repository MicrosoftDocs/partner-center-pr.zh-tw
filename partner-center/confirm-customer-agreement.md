---
title: 確認客戶接受 Microsoft 客戶合約
description: 了解如何確認客戶接受 Microsoft 客戶合約。 雲端解決方案提供者 (CSP) 計畫參與者需要此合約來為客戶訂購 Microsoft 產品和服務。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 45a34473ff63875af8bd07962ea836661bc948ee
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92198054"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="4b53e-104">確認客戶接受 CSP 合作夥伴方案中的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-104">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="4b53e-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="4b53e-105">**Applies to**</span></span>

- <span data-ttu-id="4b53e-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="4b53e-106">Partner Center</span></span>
- <span data-ttu-id="4b53e-107">Microsoft 365 系統管理中心</span><span class="sxs-lookup"><span data-stu-id="4b53e-107">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="4b53e-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="4b53e-108">**Appropriate roles**</span></span>

- <span data-ttu-id="4b53e-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="4b53e-109">Admin agent</span></span>
- <span data-ttu-id="4b53e-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="4b53e-110">Sales agent</span></span>

<span data-ttu-id="4b53e-111">Microsoft 在 2019 年 10 月 1 日把 **Microsoft 客戶合約**引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-111">On October 1, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="4b53e-112">若為間接轉銷商，請參閱其他[指引](indirect-reseller-tasks-in-partner-center.md)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-112">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="4b53e-113">為了協助合作夥伴遷移至新的合約，在 2020 年 1 月 31 日前，此兩個合約會並存在 CSP 計畫中。</span><span class="sxs-lookup"><span data-stu-id="4b53e-113">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31, 2020.</span></span> <span data-ttu-id="4b53e-114">從 2020 年 2 月 1 日開始，Microsoft 客戶合約會取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-114">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="4b53e-115">客戶有兩個選項可以接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-115">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="4b53e-116">**選項 1**：合作夥伴證明客戶接受 - 合作夥伴可以使用合作夥伴中心 API/SDK 或透過合作夥伴中心儀表板來確認客戶接受。</span><span class="sxs-lookup"><span data-stu-id="4b53e-116">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="4b53e-117">**選項 2**：客戶直接接受 - 合作夥伴可以透過 URL 邀請客戶，在 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-117">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="4b53e-118">存取 Microsoft 客戶合約範本</span><span class="sxs-lookup"><span data-stu-id="4b53e-118">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="4b53e-119">您可以從[這裡](https://aka.ms/customeragreement)手動下載最新版本的 Microsoft 客戶合約範本。</span><span class="sxs-lookup"><span data-stu-id="4b53e-119">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="4b53e-120">Microsoft 客戶合約是國家/地區特定。</span><span class="sxs-lookup"><span data-stu-id="4b53e-120">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="4b53e-121">當要求 Microsoft 客戶合約範本時，請務必根據客戶的位置選取正確的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="4b53e-121">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="4b53e-122">選項 1：在合作夥伴中心確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="4b53e-122">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="4b53e-123">合作夥伴可以在合作夥伴中心針對新的和現有的客戶，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-123">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="4b53e-124">轉銷商無法代表其客戶進行證明，而且必須與間接提供者合作，才能完成證明。</span><span class="sxs-lookup"><span data-stu-id="4b53e-124">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="4b53e-125">確認新客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="4b53e-125">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="4b53e-126">當您在合作夥伴中心建立新的客戶租用戶時，請使用下列步驟來確認客戶是否接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-126">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="4b53e-127">您必須是系統管理員代理人或銷售代理人，才能執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="4b53e-127">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="4b53e-128">選取 [客戶]，然後選取 [新客戶]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-128">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="4b53e-129">在 [帳戶資訊] 底下，輸入公司及其主要連絡人的資訊。</span><span class="sxs-lookup"><span data-stu-id="4b53e-129">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="4b53e-130">在 [Microsoft 合約] 底下，選取方塊以證明客戶已接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-130">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="4b53e-131">在 [合約接受日期] 下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="4b53e-131">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="4b53e-132">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="4b53e-132">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="4b53e-133">請確定顯示的主要使用者連絡人資訊正確。</span><span class="sxs-lookup"><span data-stu-id="4b53e-133">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="4b53e-134">如果資訊不正確，請選取 [更新]，然後輸入接受合約人員的正確資訊。</span><span class="sxs-lookup"><span data-stu-id="4b53e-134">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="4b53e-135">選取 [下一個]，繼續建立客戶租用戶。</span><span class="sxs-lookup"><span data-stu-id="4b53e-135">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客戶":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="4b53e-137">確認現有客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="4b53e-137">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="4b53e-138">您必須是系統管理員代理人或銷售代理人，才能執行此動作：</span><span class="sxs-lookup"><span data-stu-id="4b53e-138">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="4b53e-139">選取 [客戶]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-139">Select **Customers**.</span></span> <span data-ttu-id="4b53e-140">尋找並選取客戶。</span><span class="sxs-lookup"><span data-stu-id="4b53e-140">Find and select the customer.</span></span>

2. <span data-ttu-id="4b53e-141">選取 [帳戶資訊]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-141">Select **Account info**.</span></span>

3. <span data-ttu-id="4b53e-142">在 [Microsoft 客戶合約] 下方，選取 [更新]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-142">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="4b53e-143">輸入接受合約人員的 [名字]、[姓氏]、[電子郵件地址] 和 [電話號碼] (選用)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-143">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="4b53e-144">在 [合約接受日期] 下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="4b53e-144">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="4b53e-145">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="4b53e-145">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="4b53e-146">選取 [儲存] 並繼續作業。</span><span class="sxs-lookup"><span data-stu-id="4b53e-146">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="新客戶":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="4b53e-148">取得客戶接受的確認</span><span class="sxs-lookup"><span data-stu-id="4b53e-148">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="4b53e-149">您可以使用下列步驟來取得現有客戶已接受 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="4b53e-149">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="4b53e-150">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="4b53e-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="4b53e-151">選取 [客戶]，然後尋找並選取您想要查看的客戶。</span><span class="sxs-lookup"><span data-stu-id="4b53e-151">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="4b53e-152">選取 [帳戶資訊]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-152">Select **Account info**.</span></span>

3. <span data-ttu-id="4b53e-153">在 [Microsoft 客戶合約] 底下，檢視此客戶是否已提供確認。</span><span class="sxs-lookup"><span data-stu-id="4b53e-153">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="4b53e-154">使用合作夥伴中心 API/SDK 確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="4b53e-154">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="4b53e-155">您可以使用合作夥伴中心 API/SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-155">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="4b53e-156">如需 API/SDK 的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="4b53e-156">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="4b53e-157">取得 Microsoft 客戶合約的合約中繼資料</span><span class="sxs-lookup"><span data-stu-id="4b53e-157">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="4b53e-158">確認客戶接受 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-158">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="4b53e-159">取得客戶接受 Microsoft 客戶合約的確認</span><span class="sxs-lookup"><span data-stu-id="4b53e-159">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="4b53e-160">取得 Microsoft 客戶合約範本的下載連結</span><span class="sxs-lookup"><span data-stu-id="4b53e-160">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="4b53e-161">選項 2：Microsoft 365 系統管理中心的客戶接受</span><span class="sxs-lookup"><span data-stu-id="4b53e-161">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="4b53e-162">合作夥伴可以透過 URL 邀請新的和現有的客戶，在 Microsoft 365 系統管理中心內檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-162">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="4b53e-163">接下來幾節將示範如何：</span><span class="sxs-lookup"><span data-stu-id="4b53e-163">The next few sections show you how to:</span></span>

- <span data-ttu-id="4b53e-164">建立全新的客戶，並邀請客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-164">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="4b53e-165">邀請新客戶檢閱及接受轉銷商關係和合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-165">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="4b53e-166">邀請現有的客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-166">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="4b53e-167">您可以使用[合作夥伴中心 API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement)，取得客戶直接接受 Microsoft 客戶合約的狀態。</span><span class="sxs-lookup"><span data-stu-id="4b53e-167">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="4b53e-168">建立全新的客戶，並邀請客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-168">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="4b53e-169">使用下列步驟在合作夥伴中心建立新的客戶，然後邀請他們在 Microsoft 365 系統管理中心內檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-169">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="4b53e-170">從合作夥伴中心的 [客戶] 索引標籤中，選取 [新增客戶]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-170">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="4b53e-171">在 [帳戶資訊] 底下的所有必要欄位中，輸入新客戶的相關資訊，包括客戶的公司名稱和主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="4b53e-171">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="4b53e-172">在 [客戶合約] 中，選取第一個選項 [要求客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-172">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="4b53e-173">完成頁面上其他任何必要欄位。</span><span class="sxs-lookup"><span data-stu-id="4b53e-173">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="4b53e-174">選取 **[下一步：檢閱]** ，然後繼續建立客戶租用戶的步驟。</span><span class="sxs-lookup"><span data-stu-id="4b53e-174">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="4b53e-175">新客戶在接受 Microsoft 客戶合約之前，無法進行新的購買。</span><span class="sxs-lookup"><span data-stu-id="4b53e-175">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="新客戶":::

5. <span data-ttu-id="4b53e-177">當您到達新客戶工作流程中的 [確認] 畫面時，請儲存客戶認證。</span><span class="sxs-lookup"><span data-stu-id="4b53e-177">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="4b53e-178">您稍後必須將這些認證提供給您的客戶。</span><span class="sxs-lookup"><span data-stu-id="4b53e-178">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="4b53e-179">在合作夥伴中心外，建立並傳送電子郵件，邀請客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-179">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="4b53e-180">請務必在電子郵件中包含下列項目：</span><span class="sxs-lookup"><span data-stu-id="4b53e-180">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="4b53e-181">此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的連結 (需要登入)</span><span class="sxs-lookup"><span data-stu-id="4b53e-181">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="4b53e-182">您在步驟 5 中儲存的客戶認證。</span><span class="sxs-lookup"><span data-stu-id="4b53e-182">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="4b53e-183">客戶接著會收到來自合作夥伴的電子郵件邀請，然後選取 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-183">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="4b53e-184">客戶使用先前所收到來自合作夥伴的客戶認證，來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="4b53e-184">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="4b53e-185">客戶接著勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-185">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="4b53e-186">邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-186">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="4b53e-187">使用下列步驟來邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-187">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="4b53e-188">從合作夥伴中心的 [客戶] 索引標籤中，選取 [要求建立轉銷商關係] 連結。</span><span class="sxs-lookup"><span data-stu-id="4b53e-188">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="4b53e-189">系統會產生自動電子郵件範本，包括文字和參數化 URL，以將客戶引導至 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="4b53e-189">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="4b53e-190">您可以自訂自動產生的電子郵件範本，然後選取 [複製到剪貼簿] 或 [在電子郵件中開啟]。</span><span class="sxs-lookup"><span data-stu-id="4b53e-190">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="4b53e-191">使用此電子郵件範本來邀請客戶接受**轉銷商關係**要求和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="4b53e-191">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="4b53e-192">(注意：在電子郵件邀請中，請確定合作夥伴也包含自動提供的 URL，以及最近建立的客戶認證)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-192">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="新客戶":::

5. <span data-ttu-id="4b53e-194">客戶透過電子郵件接收邀請，然後按一下參數化 URL。</span><span class="sxs-lookup"><span data-stu-id="4b53e-194">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="4b53e-195">客戶使用合作夥伴在電子郵件內提供的認證來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="4b53e-195">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="4b53e-196">客戶勾選方塊以接受**轉銷商關係**和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="4b53e-196">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="4b53e-197">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="4b53e-197">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="4b53e-198">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4b53e-198">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="新客戶":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="4b53e-200">邀請現有的客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-200">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="4b53e-201">使用下列步驟來邀請現有的客戶檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-201">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="4b53e-202">建立具有內嵌 URL 的客戶電子郵件，邀請您的客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-202">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="4b53e-203">您的客戶透過電子郵件收到邀請，然後按一下 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-203">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="4b53e-204">客戶將其認證輸入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="4b53e-204">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="4b53e-205">您的客戶勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-205">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="4b53e-206">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="4b53e-206">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="4b53e-207">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4b53e-207">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="新客戶":::

>[!NOTE]
><span data-ttu-id="4b53e-209">在某些情況下，客戶可能無法直接接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-209">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="4b53e-210">若要深入了解這些情況，請參閱[您需要代表客戶進行證明的兩個案例](attest-acceptance-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="4b53e-210">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="4b53e-211">歷程記錄時間軸詳細資料</span><span class="sxs-lookup"><span data-stu-id="4b53e-211">Historical timeline details</span></span>

| <span data-ttu-id="4b53e-212">日期</span><span class="sxs-lookup"><span data-stu-id="4b53e-212">Date</span></span> | <span data-ttu-id="4b53e-213">里程碑</span><span class="sxs-lookup"><span data-stu-id="4b53e-213">Milestone</span></span> | <span data-ttu-id="4b53e-214">詳細資料</span><span class="sxs-lookup"><span data-stu-id="4b53e-214">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="4b53e-215">2019 年 8 月 1 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-215">August 01, 2019</span></span>| <span data-ttu-id="4b53e-216">沙箱中提供 UX 預覽</span><span class="sxs-lookup"><span data-stu-id="4b53e-216">UX preview available in sandbox</span></span>| <span data-ttu-id="4b53e-217">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心儀表板，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-217">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="4b53e-218">具有 CSP 沙箱環境存取權的合作夥伴可預覽使用者體驗變更。</span><span class="sxs-lookup"><span data-stu-id="4b53e-218">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="4b53e-219">沒有沙箱存取權的合作夥伴可以深入了解本主題中的變更。</span><span class="sxs-lookup"><span data-stu-id="4b53e-219">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="4b53e-220">2019 年 9 月 3 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-220">September 03, 2019</span></span>|<span data-ttu-id="4b53e-221">沙箱中提供 API 預覽。</span><span class="sxs-lookup"><span data-stu-id="4b53e-221">API preview is available in sandbox.</span></span>|<span data-ttu-id="4b53e-222">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 API 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-222">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="4b53e-223">API 合作夥伴可以使用此機會預覽 API 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-223">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="4b53e-224">2019 年 9 月 20 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-224">September 20, 2019</span></span>|<span data-ttu-id="4b53e-225">沙箱中提供 .NET SDK 預覽。</span><span class="sxs-lookup"><span data-stu-id="4b53e-225">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="4b53e-226">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 .NET SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-226">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="4b53e-227">API 合作夥伴可以使用此機會預覽 .NET SDK 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-227">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="4b53e-228">2019 年 10 月 1 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-228">October 01, 2019</span></span>|<span data-ttu-id="4b53e-229">可在生產環境中使用的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-229">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="4b53e-230">Microsoft 會將 Microsoft 客戶合約引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-230">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="4b53e-231">合作夥伴可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-231">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="4b53e-232">CSP 合作夥伴計畫中仍支援 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-232">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="4b53e-233">不過，建議合作夥伴開始遷移至 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-233">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="4b53e-234">現有訂用帳戶的新購買和授權計數變更，將需要 Microsoft 客戶合約或 Microsoft Cloud 合約的合作夥伴確認。</span><span class="sxs-lookup"><span data-stu-id="4b53e-234">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="4b53e-235">某些新供應項目 (例如新的 Azure 方案) 將需要確認 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-235">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="4b53e-236">2020 年 1 月 31 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-236">January 31, 2020</span></span>|<span data-ttu-id="4b53e-237">已從生產環境中移除 Microsoft Cloud 合約</span><span class="sxs-lookup"><span data-stu-id="4b53e-237">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="4b53e-238">CSP 合作夥伴計畫中不再接受 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-238">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="4b53e-239">現有訂用帳戶的新購買和授權計數變更，將需要合作夥伴提供 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="4b53e-239">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="4b53e-240">這項需求適用於新客戶及先前可能已接受 Microsoft Cloud 合約的現有客戶。</span><span class="sxs-lookup"><span data-stu-id="4b53e-240">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="4b53e-241">2020 年 2 月 3 日</span><span class="sxs-lookup"><span data-stu-id="4b53e-241">February 3, 2020</span></span>|<span data-ttu-id="4b53e-242">合作夥伴現在可以選擇透過 URL 來邀請客戶，在已驗證的 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-242">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="4b53e-243">客戶可以在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="4b53e-243">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="4b53e-244">客戶在 Microsoft 365 系統管理中心直接接受合約即會確認條款核准。</span><span class="sxs-lookup"><span data-stu-id="4b53e-244">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 