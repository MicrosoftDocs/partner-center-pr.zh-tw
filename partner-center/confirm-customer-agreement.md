---
title: 確認客戶接受 Microsoft 客戶合約
description: 了解如何確認客戶接受 Microsoft 客戶合約。 雲端解決方案提供者需要此合約來為客戶訂購 Microsoft 產品和服務。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 7d25625eebaf863ed819112439bbf2d6e0f505e1
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000542"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="a5d14-104">確認客戶接受 CSP 合作夥伴方案中的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-104">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="a5d14-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="a5d14-105">**Applies to**</span></span>

- <span data-ttu-id="a5d14-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a5d14-106">Partner Center</span></span>
- <span data-ttu-id="a5d14-107">Microsoft 365 系統管理中心</span><span class="sxs-lookup"><span data-stu-id="a5d14-107">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="a5d14-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="a5d14-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a5d14-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="a5d14-109">Admin agent</span></span>
- <span data-ttu-id="a5d14-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="a5d14-110">Sales agent</span></span>

<span data-ttu-id="a5d14-111">**適當的合作夥伴類型**</span><span class="sxs-lookup"><span data-stu-id="a5d14-111">**Appropriate partner types**</span></span>

- <span data-ttu-id="a5d14-112">間接轉銷商、直接帳單、間接提供者</span><span class="sxs-lookup"><span data-stu-id="a5d14-112">Indirect resellers, Direct bill, Indirect providers</span></span>

<span data-ttu-id="a5d14-113">Microsoft 在 2019 年 10 月 1 日把 **Microsoft 客戶合約**引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-113">On October 1st, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="a5d14-114">若為間接轉銷商，請參閱其他[指引](indirect-reseller-tasks-in-partner-center.md)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-114">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="a5d14-115">為了協助合作夥伴遷移至新的合約，在 2020 年 1 月 31 日前，此兩個合約會並存在 CSP 計畫中。</span><span class="sxs-lookup"><span data-stu-id="a5d14-115">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31st, 2020.</span></span> <span data-ttu-id="a5d14-116">從 2020 年 2 月 1 日開始，Microsoft 客戶合約會取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-116">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="a5d14-117">客戶有兩個選項可以接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-117">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="a5d14-118">**選項 1**：合作夥伴證明客戶接受 - 合作夥伴可以使用合作夥伴中心 API/SDK 或透過合作夥伴中心儀表板來確認客戶接受。</span><span class="sxs-lookup"><span data-stu-id="a5d14-118">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="a5d14-119">**選項 2**：客戶直接接受 - 合作夥伴可以透過 URL 邀請客戶，在 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-119">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="a5d14-120">存取 Microsoft 客戶合約範本</span><span class="sxs-lookup"><span data-stu-id="a5d14-120">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="a5d14-121">您可以從[這裡](https://aka.ms/customeragreement)手動下載最新版本的 Microsoft 客戶合約範本。</span><span class="sxs-lookup"><span data-stu-id="a5d14-121">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="a5d14-122">Microsoft 客戶合約是國家/地區特定。</span><span class="sxs-lookup"><span data-stu-id="a5d14-122">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="a5d14-123">當要求 Microsoft 客戶合約範本時，請務必根據客戶的位置選取正確的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="a5d14-123">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="a5d14-124">選項 1：在合作夥伴中心確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="a5d14-124">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="a5d14-125">合作夥伴可以在合作夥伴中心針對新的和現有的客戶，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-125">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="a5d14-126">轉銷商無法代表其客戶進行證明，而且必須與間接提供者合作，才能完成證明。</span><span class="sxs-lookup"><span data-stu-id="a5d14-126">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="a5d14-127">確認新客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="a5d14-127">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="a5d14-128">當您在合作夥伴中心建立新的客戶租用戶時，請使用下列步驟來確認客戶是否接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-128">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="a5d14-129">您必須是系統管理員代理人或銷售代理人，才能執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="a5d14-129">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="a5d14-130">選取 [客戶]，然後選取 [新客戶]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-130">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="a5d14-131">在 [帳戶資訊] 底下，輸入公司及其主要連絡人的資訊。</span><span class="sxs-lookup"><span data-stu-id="a5d14-131">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="a5d14-132">在 [Microsoft 合約] 底下，選取方塊以證明客戶已接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-132">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="a5d14-133">在 [合約接受日期] 下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="a5d14-133">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="a5d14-134">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="a5d14-134">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="a5d14-135">請確定顯示的主要使用者連絡人資訊正確。</span><span class="sxs-lookup"><span data-stu-id="a5d14-135">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="a5d14-136">如果資訊不正確，請選取 [更新]，然後輸入接受合約人員的正確資訊。</span><span class="sxs-lookup"><span data-stu-id="a5d14-136">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="a5d14-137">選取 [下一個]，繼續建立客戶租用戶。</span><span class="sxs-lookup"><span data-stu-id="a5d14-137">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客戶":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="a5d14-139">確認現有客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="a5d14-139">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="a5d14-140">您必須是系統管理員代理人或銷售代理人，才能執行此動作：</span><span class="sxs-lookup"><span data-stu-id="a5d14-140">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="a5d14-141">選取 [客戶]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-141">Select **Customers**.</span></span> <span data-ttu-id="a5d14-142">尋找並選取客戶。</span><span class="sxs-lookup"><span data-stu-id="a5d14-142">Find and select the customer.</span></span>

2. <span data-ttu-id="a5d14-143">選取 [帳戶資訊]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-143">Select **Account info**.</span></span>

3. <span data-ttu-id="a5d14-144">在 [Microsoft 客戶合約] 下方，選取 [更新]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-144">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="a5d14-145">輸入接受合約人員的 [名字]、[姓氏]、[電子郵件地址] 和 [電話號碼] (選用)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-145">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="a5d14-146">在 [合約接受日期] 下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="a5d14-146">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="a5d14-147">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="a5d14-147">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="a5d14-148">選取 [儲存] 並繼續作業。</span><span class="sxs-lookup"><span data-stu-id="a5d14-148">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="現有客戶":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="a5d14-150">取得客戶接受的確認</span><span class="sxs-lookup"><span data-stu-id="a5d14-150">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="a5d14-151">您可以使用下列步驟來取得現有客戶已接受 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="a5d14-151">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="a5d14-152">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="a5d14-152">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="a5d14-153">選取 [客戶]，然後尋找並選取您想要查看的客戶。</span><span class="sxs-lookup"><span data-stu-id="a5d14-153">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="a5d14-154">選取 [帳戶資訊]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-154">Select **Account info**.</span></span>

3. <span data-ttu-id="a5d14-155">在 [Microsoft 客戶合約] 底下，檢視此客戶是否已提供確認。</span><span class="sxs-lookup"><span data-stu-id="a5d14-155">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="a5d14-156">使用合作夥伴中心 API/SDK 確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="a5d14-156">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="a5d14-157">您可以使用合作夥伴中心 API/SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-157">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="a5d14-158">如需 API/SDK 的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="a5d14-158">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="a5d14-159">取得 Microsoft 客戶合約的合約中繼資料</span><span class="sxs-lookup"><span data-stu-id="a5d14-159">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="a5d14-160">確認客戶接受 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-160">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="a5d14-161">取得客戶接受 Microsoft 客戶合約的確認</span><span class="sxs-lookup"><span data-stu-id="a5d14-161">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="a5d14-162">取得 Microsoft 客戶合約範本的下載連結</span><span class="sxs-lookup"><span data-stu-id="a5d14-162">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="a5d14-163">選項 2：Microsoft 365 系統管理中心的客戶接受</span><span class="sxs-lookup"><span data-stu-id="a5d14-163">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="a5d14-164">合作夥伴可以透過 URL 邀請新的和現有的客戶，在 Microsoft 365 系統管理中心內檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-164">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="a5d14-165">接下來幾節將示範如何：</span><span class="sxs-lookup"><span data-stu-id="a5d14-165">The next few sections show you how to:</span></span>

- <span data-ttu-id="a5d14-166">建立全新的客戶，並邀請客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-166">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="a5d14-167">邀請新客戶檢閱及接受轉銷商關係和合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-167">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="a5d14-168">邀請現有的客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-168">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="a5d14-169">您可以使用[合作夥伴中心 API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement)，取得客戶直接接受 Microsoft 客戶合約的狀態。</span><span class="sxs-lookup"><span data-stu-id="a5d14-169">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="a5d14-170">建立全新的客戶，並邀請客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-170">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="a5d14-171">使用下列步驟在合作夥伴中心建立新的客戶，然後邀請他們在 Microsoft 365 系統管理中心內檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-171">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="a5d14-172">從合作夥伴中心的 [客戶] 索引標籤中，選取 [新增客戶]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-172">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="a5d14-173">在 [帳戶資訊] 底下的所有必要欄位中，輸入新客戶的相關資訊，包括客戶的公司名稱和主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="a5d14-173">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="a5d14-174">在 [客戶合約] 中，選取第一個選項 [要求客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-174">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="a5d14-175">完成頁面上其他任何必要欄位。</span><span class="sxs-lookup"><span data-stu-id="a5d14-175">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="a5d14-176">選取 **[下一步：檢閱]** ，然後繼續建立客戶租用戶的步驟。</span><span class="sxs-lookup"><span data-stu-id="a5d14-176">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="a5d14-177">新客戶在接受 Microsoft 客戶合約之前，無法進行新的購買。</span><span class="sxs-lookup"><span data-stu-id="a5d14-177">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="建立新客戶":::

5. <span data-ttu-id="a5d14-179">當您到達新客戶工作流程中的 [確認] 畫面時，請儲存客戶認證。</span><span class="sxs-lookup"><span data-stu-id="a5d14-179">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="a5d14-180">您稍後必須將這些認證提供給您的客戶。</span><span class="sxs-lookup"><span data-stu-id="a5d14-180">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="a5d14-181">在合作夥伴中心外，建立並傳送電子郵件，邀請客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-181">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="a5d14-182">請務必在電子郵件中包含下列項目：</span><span class="sxs-lookup"><span data-stu-id="a5d14-182">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="a5d14-183">此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的連結 (需要登入)</span><span class="sxs-lookup"><span data-stu-id="a5d14-183">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="a5d14-184">您在步驟 5 中儲存的客戶認證。</span><span class="sxs-lookup"><span data-stu-id="a5d14-184">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="a5d14-185">客戶接著會收到來自合作夥伴的電子郵件邀請，然後選取 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-185">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="a5d14-186">客戶使用先前所收到來自合作夥伴的客戶認證，來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="a5d14-186">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="a5d14-187">客戶接著勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-187">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="a5d14-188">邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-188">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="a5d14-189">使用下列步驟來邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-189">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="a5d14-190">從合作夥伴中心的 [客戶] 索引標籤中，選取 [要求建立轉銷商關係] 連結。</span><span class="sxs-lookup"><span data-stu-id="a5d14-190">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="a5d14-191">系統會產生自動電子郵件範本，包括文字和參數化 URL，以將客戶引導至 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="a5d14-191">An automatic email template will be generated, including text and a parameterized URL which will direct the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="a5d14-192">您可以自訂自動產生的電子郵件範本，然後選取 [複製到剪貼簿] 或 [在電子郵件中開啟]。</span><span class="sxs-lookup"><span data-stu-id="a5d14-192">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="a5d14-193">使用此電子郵件範本來邀請客戶接受**轉銷商關係**要求和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="a5d14-193">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="a5d14-194">(注意：在電子郵件邀請中，請確定合作夥伴也包含自動提供的 URL，以及最近建立的客戶認證)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-194">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="建立關係":::

5. <span data-ttu-id="a5d14-196">客戶透過電子郵件接收邀請，然後按一下參數化 URL。</span><span class="sxs-lookup"><span data-stu-id="a5d14-196">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="a5d14-197">客戶使用合作夥伴在電子郵件內提供的認證來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="a5d14-197">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="a5d14-198">客戶勾選方塊以接受**轉銷商關係**和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="a5d14-198">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="a5d14-199">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="a5d14-199">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="a5d14-200">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="a5d14-200">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受合約":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="a5d14-202">邀請現有的客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-202">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="a5d14-203">使用下列步驟來邀請現有的客戶檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-203">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="a5d14-204">建立具有內嵌 URL 的客戶電子郵件，邀請您的客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-204">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="a5d14-205">您的客戶透過電子郵件收到邀請，然後按一下 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-205">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="a5d14-206">客戶將其認證輸入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="a5d14-206">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="a5d14-207">您的客戶勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-207">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="a5d14-208">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="a5d14-208">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="a5d14-209">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="a5d14-209">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客戶":::

>[!NOTE]
><span data-ttu-id="a5d14-211">在某些情況下，客戶可能無法直接接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-211">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="a5d14-212">若要深入了解這些情況，請參閱[您需要代表客戶進行證明的兩個案例](attest-acceptance-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="a5d14-212">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="a5d14-213">歷程記錄時間軸詳細資料</span><span class="sxs-lookup"><span data-stu-id="a5d14-213">Historical timeline details</span></span>

| <span data-ttu-id="a5d14-214">日期</span><span class="sxs-lookup"><span data-stu-id="a5d14-214">Date</span></span> | <span data-ttu-id="a5d14-215">里程碑</span><span class="sxs-lookup"><span data-stu-id="a5d14-215">Milestone</span></span> | <span data-ttu-id="a5d14-216">詳細資料</span><span class="sxs-lookup"><span data-stu-id="a5d14-216">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="a5d14-217">2019 年 8 月 1 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-217">August 01, 2019</span></span>|<span data-ttu-id="a5d14-218">沙箱中提供 UX 預覽</span><span class="sxs-lookup"><span data-stu-id="a5d14-218">UX preview available in sandbox</span></span>|<span data-ttu-id="a5d14-219">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心儀表板，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-219">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="a5d14-220">具有 CSP 沙箱環境存取權的合作夥伴可預覽使用者體驗變更。</span><span class="sxs-lookup"><span data-stu-id="a5d14-220">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="a5d14-221">沒有沙箱存取權的合作夥伴可以深入了解本主題中的變更。</span><span class="sxs-lookup"><span data-stu-id="a5d14-221">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="a5d14-222">2019 年 9 月 3 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-222">September 03, 2019</span></span>|<span data-ttu-id="a5d14-223">沙箱中提供 API 預覽。</span><span class="sxs-lookup"><span data-stu-id="a5d14-223">API preview is available in sandbox.</span></span>|<span data-ttu-id="a5d14-224">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 API 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-224">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="a5d14-225">API 合作夥伴可以使用此機會預覽 API 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-225">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="a5d14-226">2019 年 9 月 20 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-226">September 20, 2019</span></span>|<span data-ttu-id="a5d14-227">沙箱中提供 .NET SDK 預覽。</span><span class="sxs-lookup"><span data-stu-id="a5d14-227">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="a5d14-228">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 .NET SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-228">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="a5d14-229">API 合作夥伴可以使用此機會預覽 .NET SDK 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-229">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="a5d14-230">2019 年 10 月 1 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-230">October 01, 2019</span></span>|<span data-ttu-id="a5d14-231">可在生產環境中使用的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-231">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="a5d14-232">Microsoft 會將 Microsoft 客戶合約引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-232">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="a5d14-233">合作夥伴可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-233">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="a5d14-234">CSP 合作夥伴計畫中仍支援 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-234">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="a5d14-235">不過，建議合作夥伴開始遷移至 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-235">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="a5d14-236">現有訂用帳戶的新購買和授權計數變更，將需要 Microsoft 客戶合約或 Microsoft Cloud 合約的合作夥伴確認。</span><span class="sxs-lookup"><span data-stu-id="a5d14-236">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="a5d14-237">某些新供應項目 (例如新的 Azure 方案) 將需要確認 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-237">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="a5d14-238">2020 年 1 月 31 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-238">January 31, 2020</span></span>|<span data-ttu-id="a5d14-239">已從生產環境中移除 Microsoft Cloud 合約</span><span class="sxs-lookup"><span data-stu-id="a5d14-239">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="a5d14-240">CSP 合作夥伴計畫中不再接受 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-240">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="a5d14-241">現有訂用帳戶的新購買和授權計數變更，將需要合作夥伴提供 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="a5d14-241">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="a5d14-242">這項需求適用於新客戶及先前可能已接受 Microsoft Cloud 合約的現有客戶。</span><span class="sxs-lookup"><span data-stu-id="a5d14-242">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="a5d14-243">2020 年 2 月 3 日</span><span class="sxs-lookup"><span data-stu-id="a5d14-243">February 3, 2020</span></span>|<span data-ttu-id="a5d14-244">合作夥伴現在可以選擇透過 URL 來邀請客戶，在已驗證的 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-244">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="a5d14-245">客戶可以在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="a5d14-245">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="a5d14-246">客戶在 Microsoft 365 系統管理中心直接接受合約即會確認條款核准。</span><span class="sxs-lookup"><span data-stu-id="a5d14-246">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 