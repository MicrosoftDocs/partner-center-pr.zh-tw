---
title: 確認客戶接受 Microsoft 客戶合約
description: 雲端解決方案提供者 (CSP) 合作夥伴必須先確認客戶接受 Microsoft 客戶合約，才能為客戶訂購 Microsoft 服務。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/05/2020
ms.openlocfilehash: 423cf1aab281ad8e77e03aa386b43360e1b99b3c
ms.sourcegitcommit: 6b03ff400d1350db9696f9b457fcfe710310c5d3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/03/2020
ms.locfileid: "96570564"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a><span data-ttu-id="3e4ff-103">確認客戶接受 CSP 合作夥伴方案中的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-103">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>

<span data-ttu-id="3e4ff-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="3e4ff-104">**Applies to**</span></span>

- <span data-ttu-id="3e4ff-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="3e4ff-105">Partner Center</span></span>
- <span data-ttu-id="3e4ff-106">Microsoft 365 系統管理中心</span><span class="sxs-lookup"><span data-stu-id="3e4ff-106">Microsoft 365 Admin Center</span></span>

<span data-ttu-id="3e4ff-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="3e4ff-107">**Appropriate roles**</span></span>

- <span data-ttu-id="3e4ff-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="3e4ff-108">Admin agent</span></span>
- <span data-ttu-id="3e4ff-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="3e4ff-109">Sales agent</span></span>

<span data-ttu-id="3e4ff-110">Microsoft 在 2019 年 10 月 1 日把 **Microsoft 客戶合約** 引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-110">On October 1, 2019, Microsoft introduced the **Microsoft Customer Agreement** to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="3e4ff-111">若為間接轉銷商，請參閱其他[指引](indirect-reseller-tasks-in-partner-center.md)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-111">Read additional [guidance](indirect-reseller-tasks-in-partner-center.md) for indirect resellers.</span></span> <span data-ttu-id="3e4ff-112">為了協助合作夥伴遷移至新的合約，在 2020 年 1 月 31 日前，此兩個合約會並存在 CSP 計畫中。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-112">To facilitate partners' migration to the new agreement, both agreements coexisted in the CSP program until January 31, 2020.</span></span> <span data-ttu-id="3e4ff-113">從 2020 年 2 月 1 日開始，Microsoft 客戶合約會取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-113">Starting February 1, 2020, the Microsoft Customer Agreement replaced the Microsoft Cloud Agreement.</span></span>

<span data-ttu-id="3e4ff-114">客戶有兩個選項可以接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-114">Customers have two options for accepting the Microsoft Customer Agreement.</span></span> 

<span data-ttu-id="3e4ff-115">**選項 1**：合作夥伴證明客戶接受 - 合作夥伴可以使用合作夥伴中心 API/SDK 或透過合作夥伴中心儀表板來確認客戶接受。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-115">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="3e4ff-116">**選項 2**：客戶直接接受 - 合作夥伴可以透過 URL 邀請客戶，在 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-116">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="3e4ff-117">存取 Microsoft 客戶合約範本</span><span class="sxs-lookup"><span data-stu-id="3e4ff-117">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="3e4ff-118">您可以從[這裡](https://aka.ms/customeragreement)手動下載最新版本的 Microsoft 客戶合約範本。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-118">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="3e4ff-119">Microsoft 客戶合約是國家/地區特定。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-119">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="3e4ff-120">當要求 Microsoft 客戶合約範本時，請務必根據客戶的位置選取正確的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-120">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="3e4ff-121">選項 1：在合作夥伴中心確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="3e4ff-121">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="3e4ff-122">合作夥伴可以在合作夥伴中心針對新的和現有的客戶，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-122">Partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="3e4ff-123">轉銷商無法代表其客戶進行證明，而且必須與間接提供者合作，才能完成證明。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-123">Resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="3e4ff-124">確認新客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="3e4ff-124">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="3e4ff-125">當您在合作夥伴中心建立新的客戶租用戶時，請使用下列步驟來確認客戶是否接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-125">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="3e4ff-126">您必須是系統管理員代理人或銷售代理人，才能執行這些步驟。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-126">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="3e4ff-127">選取 [客戶]，然後選取 [新客戶]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-127">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="3e4ff-128">在 [帳戶資訊] 底下，輸入公司及其主要連絡人的資訊。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-128">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="3e4ff-129">在 [Microsoft 合約] 底下，選取方塊以證明客戶已接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-129">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="3e4ff-130">在 [合約接受日期]  下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-130">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3e4ff-131">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-131">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="3e4ff-132">請確定顯示的主要使用者連絡人資訊正確。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-132">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="3e4ff-133">如果資訊不正確，請選取 [更新]，然後輸入接受合約人員的正確資訊。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-133">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="3e4ff-134">選取 [下一個]，繼續建立客戶租用戶。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-134">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="新客戶":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="3e4ff-136">確認現有客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="3e4ff-136">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="3e4ff-137">您必須是系統管理員代理人或銷售代理人，才能執行此動作：</span><span class="sxs-lookup"><span data-stu-id="3e4ff-137">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="3e4ff-138">選取 [客戶]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-138">Select **Customers**.</span></span> <span data-ttu-id="3e4ff-139">尋找並選取客戶。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-139">Find and select the customer.</span></span>

2. <span data-ttu-id="3e4ff-140">選取 [帳戶資訊]  。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-140">Select **Account info**.</span></span>

3. <span data-ttu-id="3e4ff-141">在 [Microsoft 客戶合約] 下方，選取 [更新]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-141">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="3e4ff-142">輸入接受合約人員的 [名字]、[姓氏]、[電子郵件地址] 和 [電話號碼] (選用)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-142">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="3e4ff-143">在 [合約接受日期]  下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-143">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="3e4ff-144">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-144">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="3e4ff-145">選取 [儲存] 並繼續作業。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-145">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="現有客戶":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="3e4ff-147">取得客戶接受的確認</span><span class="sxs-lookup"><span data-stu-id="3e4ff-147">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="3e4ff-148">您可以使用下列步驟來取得現有客戶已接受 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-148">You can retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement using the following steps.</span></span> <span data-ttu-id="3e4ff-149">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-149">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="3e4ff-150">選取 [客戶]，然後尋找並選取您想要查看的客戶。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-150">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="3e4ff-151">選取 [帳戶資訊]  。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-151">Select **Account info**.</span></span>

3. <span data-ttu-id="3e4ff-152">在 [Microsoft 客戶合約] 底下，檢視此客戶是否已提供確認。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-152">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="3e4ff-153">使用合作夥伴中心 API/SDK 確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="3e4ff-153">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="3e4ff-154">您可以使用合作夥伴中心 API/SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-154">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="3e4ff-155">如需 API/SDK 的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="3e4ff-155">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="3e4ff-156">取得 Microsoft 客戶合約的合約中繼資料</span><span class="sxs-lookup"><span data-stu-id="3e4ff-156">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="3e4ff-157">確認客戶接受 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-157">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="3e4ff-158">取得客戶接受 Microsoft 客戶合約的確認</span><span class="sxs-lookup"><span data-stu-id="3e4ff-158">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="3e4ff-159">取得 Microsoft 客戶合約範本的下載連結</span><span class="sxs-lookup"><span data-stu-id="3e4ff-159">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="3e4ff-160">選項 2：Microsoft 365 系統管理中心的客戶接受</span><span class="sxs-lookup"><span data-stu-id="3e4ff-160">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="3e4ff-161">合作夥伴可以透過 URL 邀請新的和現有的客戶，在 Microsoft 365 系統管理中心內檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-161">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="3e4ff-162">接下來幾節將示範如何：</span><span class="sxs-lookup"><span data-stu-id="3e4ff-162">The next few sections show you how to:</span></span>

- <span data-ttu-id="3e4ff-163">建立全新的客戶，並邀請客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-163">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="3e4ff-164">邀請新客戶檢閱及接受轉銷商關係和合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-164">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="3e4ff-165">邀請現有的客戶檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-165">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="3e4ff-166">您可以使用[合作夥伴中心 API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement)，取得客戶直接接受 Microsoft 客戶合約的狀態。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-166">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="3e4ff-167">建立全新的客戶，並邀請客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-167">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="3e4ff-168">使用下列步驟在合作夥伴中心建立新的客戶，然後邀請他們在 Microsoft 365 系統管理中心內檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-168">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="3e4ff-169">從合作夥伴中心的 [客戶] 索引標籤中，選取 [新增客戶]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-169">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="3e4ff-170">在 [帳戶資訊] 底下的所有必要欄位中，輸入新客戶的相關資訊，包括客戶的公司名稱和主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-170">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="3e4ff-171">在 [客戶合約] 中，選取第一個選項 [要求客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-171">Under **Customer Agreement**, select the first option, **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="3e4ff-172">完成頁面上其他任何必要欄位。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-172">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="3e4ff-173">選取 **[下一步：檢閱]** ，然後繼續建立客戶租用戶的步驟。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-173">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="3e4ff-174">新客戶在接受 Microsoft 客戶合約之前，無法進行新的購買。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-174">New customers cannot make a new purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="建立新客戶":::

5. <span data-ttu-id="3e4ff-176">當您到達新客戶工作流程中的 [確認] 畫面時，請儲存客戶認證。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-176">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="3e4ff-177">您稍後必須將這些認證提供給您的客戶。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-177">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="3e4ff-178">在合作夥伴中心外，建立並傳送電子郵件，邀請客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-178">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="3e4ff-179">請務必在電子郵件中包含下列項目：</span><span class="sxs-lookup"><span data-stu-id="3e4ff-179">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="3e4ff-180">此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的連結 (需要登入)</span><span class="sxs-lookup"><span data-stu-id="3e4ff-180">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="3e4ff-181">您在步驟 5 中儲存的客戶認證。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-181">The customer's credentials you saved in Step 5.</span></span>

7. <span data-ttu-id="3e4ff-182">客戶接著會收到來自合作夥伴的電子郵件邀請，然後選取 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-182">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="3e4ff-183">客戶使用先前所收到來自合作夥伴的客戶認證，來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-183">The customer signs into Microsoft 365 Admin Center using the customer credentials previously received from the partner.</span></span>

9. <span data-ttu-id="3e4ff-184">客戶接著勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-184">The customer then checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="3e4ff-185">邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-185">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="3e4ff-186">使用下列步驟來邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-186">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="3e4ff-187">從合作夥伴中心的 [客戶] 索引標籤中，選取 [要求建立轉銷商關係] 連結。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-187">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="3e4ff-188">系統會產生自動電子郵件範本，包括文字和參數化 URL，以將客戶引導至 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-188">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="3e4ff-189">您可以自訂自動產生的電子郵件範本，然後選取 [複製到剪貼簿] 或 [在電子郵件中開啟]。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-189">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="3e4ff-190">使用此電子郵件範本來邀請客戶接受 **轉銷商關係** 要求和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-190">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="3e4ff-191">(注意：在電子郵件邀請中，請確定合作夥伴也包含自動提供的 URL，以及最近建立的客戶認證)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-191">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="建立關係":::

5. <span data-ttu-id="3e4ff-193">客戶透過電子郵件接收邀請，然後按一下參數化 URL。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-193">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="3e4ff-194">客戶使用合作夥伴在電子郵件內提供的認證來登入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-194">Customer uses credentials provided by partner within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="3e4ff-195">客戶勾選方塊以接受 **轉銷商關係** 和 **Microsoft 客戶合約**。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-195">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="3e4ff-196">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-196">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="3e4ff-197">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="接受合約":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="3e4ff-199">邀請現有的客戶檢閱及接受合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-199">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="3e4ff-200">使用下列步驟來邀請現有的客戶檢閱及接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-200">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="3e4ff-201">建立具有內嵌 URL 的客戶電子郵件，邀請您的客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-201">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="3e4ff-202">您的客戶透過電子郵件收到邀請，然後按一下 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-202">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="3e4ff-203">客戶將其認證輸入 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-203">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="3e4ff-204">您的客戶勾選方塊來接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-204">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="3e4ff-205">在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-205">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="3e4ff-206">他們可以選取合作夥伴來查看詳細資料。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-206">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="客戶":::

>[!NOTE]
><span data-ttu-id="3e4ff-208">在某些情況下，客戶可能無法直接接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-208">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="3e4ff-209">若要深入了解這些情況，請參閱[您需要代表客戶進行證明的兩個案例](attest-acceptance-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-209">To learn more about these situations, see [Two scenarios where you need to attest on behalf of your customer](attest-acceptance-customer-agreement.md).</span></span>

### <a name="historical-timeline-details"></a><span data-ttu-id="3e4ff-210">歷程記錄時間軸詳細資料</span><span class="sxs-lookup"><span data-stu-id="3e4ff-210">Historical timeline details</span></span>

| <span data-ttu-id="3e4ff-211">日期</span><span class="sxs-lookup"><span data-stu-id="3e4ff-211">Date</span></span> | <span data-ttu-id="3e4ff-212">里程碑</span><span class="sxs-lookup"><span data-stu-id="3e4ff-212">Milestone</span></span> | <span data-ttu-id="3e4ff-213">詳細資料</span><span class="sxs-lookup"><span data-stu-id="3e4ff-213">Details</span></span> |
|------------|------------|--------------------------------|
|<span data-ttu-id="3e4ff-214">2019 年 8 月 1 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-214">August 01, 2019</span></span>| <span data-ttu-id="3e4ff-215">沙箱中提供 UX 預覽</span><span class="sxs-lookup"><span data-stu-id="3e4ff-215">UX preview available in sandbox</span></span>| <span data-ttu-id="3e4ff-216">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心儀表板，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-216">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard in the CSP sandbox environment.</span></span> <span data-ttu-id="3e4ff-217">具有 CSP 沙箱環境存取權的合作夥伴可預覽使用者體驗變更。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-217">Partners with access to the CSP sandbox environment preview the user experience changes.</span></span> <span data-ttu-id="3e4ff-218">沒有沙箱存取權的合作夥伴可以深入了解本主題中的變更。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-218">Partners without sandbox access can learn about the changes in this topic.</span></span>|
|<span data-ttu-id="3e4ff-219">2019 年 9 月 3 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-219">September 03, 2019</span></span>|<span data-ttu-id="3e4ff-220">沙箱中提供 API 預覽。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-220">API preview is available in sandbox.</span></span>|<span data-ttu-id="3e4ff-221">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 API 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-221">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center API in CSP sandbox environment.</span></span> <span data-ttu-id="3e4ff-222">API 合作夥伴可以使用此機會預覽 API 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-222">API partners can use this opportunity to preview the API changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="3e4ff-223">2019 年 9 月 20 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-223">September 20, 2019</span></span>|<span data-ttu-id="3e4ff-224">沙箱中提供 .NET SDK 預覽。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-224">.NET SDK preview is available in sandbox.</span></span>|<span data-ttu-id="3e4ff-225">合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 .NET SDK 來確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-225">Partner can confirm customer acceptance of the Microsoft Customer Agreement using Partner Center .NET SDK in CSP sandbox environment.</span></span> <span data-ttu-id="3e4ff-226">API 合作夥伴可以使用此機會預覽 .NET SDK 變更，並開始處理 API 整合以支援新的合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-226">API partners can use this opportunity to preview the .NET SDK changes and start working on API integration to support the new agreement.</span></span>|
|<span data-ttu-id="3e4ff-227">2019 年 10 月 1 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-227">October 01, 2019</span></span>|<span data-ttu-id="3e4ff-228">可在生產環境中使用的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-228">Microsoft Customer Agreement available in production</span></span>|<span data-ttu-id="3e4ff-229">Microsoft 會將 Microsoft 客戶合約引進 CSP 計畫，以取代 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-229">Microsoft introduces the Microsoft Customer Agreement to the CSP program to replace the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="3e4ff-230">合作夥伴可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-230">Partners can confirm customer acceptance of the Microsoft Customer Agreement using the Partner Center dashboard and API in production.</span></span> <span data-ttu-id="3e4ff-231">CSP 合作夥伴計畫中仍支援 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-231">The Microsoft Cloud Agreement remains supported within the CSP partner program.</span></span> <span data-ttu-id="3e4ff-232">不過，建議合作夥伴開始遷移至 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-232">However, partners are advised to start migrating to the Microsoft Customer Agreement.</span></span> <span data-ttu-id="3e4ff-233">現有訂用帳戶的新購買和授權計數變更，將需要 Microsoft 客戶合約或 Microsoft Cloud 合約的合作夥伴確認。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-233">New purchases and license count changes to existing subscriptions will require partner confirmation of either the Microsoft Customer Agreement or the Microsoft Cloud Agreement.</span></span> <span data-ttu-id="3e4ff-234">某些新供應項目 (例如新的 Azure 方案) 將需要確認 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-234">Certain new offers (for example, the new Azure plan) will require confirmation of the Microsoft Customer Agreement.</span></span>|
|<span data-ttu-id="3e4ff-235">2020 年 1 月 31 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-235">January 31, 2020</span></span>|<span data-ttu-id="3e4ff-236">已從生產環境中移除 Microsoft Cloud 合約</span><span class="sxs-lookup"><span data-stu-id="3e4ff-236">Microsoft Cloud Agreement removed from production</span></span>|<span data-ttu-id="3e4ff-237">CSP 合作夥伴計畫中不再接受 Microsoft Cloud 合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-237">The Microsoft Cloud Agreement is no longer accepted within the CSP partner program.</span></span> <span data-ttu-id="3e4ff-238">現有訂用帳戶的新購買和授權計數變更，將需要合作夥伴提供 Microsoft 客戶合約的確認。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-238">New purchases and license count changes to existing subscriptions will require the partner to provide confirmation of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="3e4ff-239">這項需求適用於新客戶及先前可能已接受 Microsoft Cloud 合約的現有客戶。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-239">This requirement applies to new customers and existing customers who may have previously accepted the Microsoft Cloud Agreement.</span></span>|
|<span data-ttu-id="3e4ff-240">2020 年 2 月 3 日</span><span class="sxs-lookup"><span data-stu-id="3e4ff-240">February 3, 2020</span></span>|<span data-ttu-id="3e4ff-241">合作夥伴現在可以選擇透過 URL 來邀請客戶，在已驗證的 Microsoft 365 系統管理中心檢閱及接受合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-241">Partner now has the option to invite the customer via a URL to review and accept the agreement in authenticated Microsoft 365 Admin Center.</span></span> | <span data-ttu-id="3e4ff-242">客戶可以在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-242">Customer can accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="3e4ff-243">客戶在 Microsoft 365 系統管理中心直接接受合約即會確認條款核准。</span><span class="sxs-lookup"><span data-stu-id="3e4ff-243">Customer's direct acceptance of the agreement in Microsoft 365 Admin Center confirms approval of terms.</span></span> 