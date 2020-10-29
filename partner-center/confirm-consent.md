---
title: 確認客戶接受 Microsoft 客戶合約
description: 了解如何確認客戶接受 Microsoft 客戶合約。 這可能需要為客戶訂購 Microsoft 產品和服務。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333912"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="1fe34-104">用來確認客戶是否已接受 Microsoft 客戶合約的更新後方法</span><span class="sxs-lookup"><span data-stu-id="1fe34-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="1fe34-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="1fe34-105">**Applies to**</span></span>

-  <span data-ttu-id="1fe34-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="1fe34-106">Partner Center</span></span>

<span data-ttu-id="1fe34-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="1fe34-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1fe34-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="1fe34-108">Admin agent</span></span>
- <span data-ttu-id="1fe34-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="1fe34-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="1fe34-110">目前只有 Microsoft 公用雲端中的合作夥伴中心支援合約資源。</span><span class="sxs-lookup"><span data-stu-id="1fe34-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="1fe34-111">合約資源不適用於：</span><span class="sxs-lookup"><span data-stu-id="1fe34-111">It is not applicable to:</span></span>
> * <span data-ttu-id="1fe34-112">由 21Vianet 營運的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="1fe34-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="1fe34-113">Microsoft Cloud 德國合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="1fe34-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="1fe34-114">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="1fe34-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="1fe34-115">自 2020 年 1 月 31 日起，所有客戶 (包括現有和新的客戶) 都必須簽署新的 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="1fe34-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="1fe34-116">如需詳細資訊，請閱讀[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)。</span><span class="sxs-lookup"><span data-stu-id="1fe34-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="1fe34-117">身為合作夥伴，您必須先讓您的客戶接受 Microsoft 客戶合約，才能為該客戶訂購 Microsoft 產品和服務。</span><span class="sxs-lookup"><span data-stu-id="1fe34-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="1fe34-118">為了更妥善協助合作夥伴符合合規需求，Microsoft 會要求合作夥伴提供接受合約者的下列相關詳細資料，以確認接受：</span><span class="sxs-lookup"><span data-stu-id="1fe34-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="1fe34-119">名字</span><span class="sxs-lookup"><span data-stu-id="1fe34-119">First name</span></span>

- <span data-ttu-id="1fe34-120">姓氏</span><span class="sxs-lookup"><span data-stu-id="1fe34-120">Last name</span></span>

- <span data-ttu-id="1fe34-121">電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="1fe34-121">Email address</span></span>

- <span data-ttu-id="1fe34-122">電話號碼 (選用)</span><span class="sxs-lookup"><span data-stu-id="1fe34-122">Phone number (optional)</span></span>

- <span data-ttu-id="1fe34-123">接受日期</span><span class="sxs-lookup"><span data-stu-id="1fe34-123">Date of acceptance</span></span>

<span data-ttu-id="1fe34-124">直接帳單合作夥伴和間接提供者透過合作夥伴中心或合作夥伴中心 API 交易時，必須確認客戶已接受 Microsoft 客戶合約。</span><span class="sxs-lookup"><span data-stu-id="1fe34-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="1fe34-125">確認是「強制性」  的。</span><span class="sxs-lookup"><span data-stu-id="1fe34-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="1fe34-126">如未提供客戶確認：</span><span class="sxs-lookup"><span data-stu-id="1fe34-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="1fe34-127">您將無法為此客戶建立新訂單。</span><span class="sxs-lookup"><span data-stu-id="1fe34-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="1fe34-128">您將無法變更此客戶現有授權型訂閱的授權數目。</span><span class="sxs-lookup"><span data-stu-id="1fe34-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="1fe34-129">確認客戶接受可以透過合作夥伴中心或合作夥伴中心 API 來完成。</span><span class="sxs-lookup"><span data-stu-id="1fe34-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="1fe34-130">若要透過合作夥伴中心 API 執行這項操作，請參閱下列主題：</span><span class="sxs-lookup"><span data-stu-id="1fe34-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="1fe34-131">取得客戶同意的確認</span><span class="sxs-lookup"><span data-stu-id="1fe34-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="1fe34-132">取得合約中繼資料</span><span class="sxs-lookup"><span data-stu-id="1fe34-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="1fe34-133">確認客戶同意</span><span class="sxs-lookup"><span data-stu-id="1fe34-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="1fe34-134">這同時適用于生產和沙箱環境。</span><span class="sxs-lookup"><span data-stu-id="1fe34-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="1fe34-135">確認新客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="1fe34-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="1fe34-136">當您在合作夥伴中心建立新的客戶租用戶，請使用下列程序來確認客戶接受。</span><span class="sxs-lookup"><span data-stu-id="1fe34-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="1fe34-137">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="1fe34-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1fe34-138">選取 [客戶]  ，選取 [新客戶]  ，然後選取 [帳戶資訊]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="1fe34-139">輸入[公司]  和 [主要連絡人]  資訊。</span><span class="sxs-lookup"><span data-stu-id="1fe34-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="公司資訊":::

3. <span data-ttu-id="1fe34-141">在 [Microsoft 客戶合約]  底下，選取 [客戶已接受最新的 Microsoft 客戶合約]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="1fe34-142">在 [合約接受日期]  下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1fe34-143">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="1fe34-144">輸入提供接受的使用者詳細資料。</span><span class="sxs-lookup"><span data-stu-id="1fe34-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="新增接受日期":::

   <span data-ttu-id="1fe34-146">根據預設，會顯示主要連絡人的使用者資訊。</span><span class="sxs-lookup"><span data-stu-id="1fe34-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="1fe34-147">如果此資訊不正確，請選取 [更新]  ，然後輸入接受合約之人員的 [名字]  、[姓氏]  、[電子郵件地址]  、\*[電話號碼]  (選用)。</span><span class="sxs-lookup"><span data-stu-id="1fe34-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="1fe34-148">選取 [下一步]  以繼續建立客戶租用戶的其餘步驟。</span><span class="sxs-lookup"><span data-stu-id="1fe34-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1fe34-149">確認現有客戶的客戶接受</span><span class="sxs-lookup"><span data-stu-id="1fe34-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="1fe34-150">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="1fe34-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1fe34-151">選取 [客戶]，然後尋找並選取您想要查看的客戶。</span><span class="sxs-lookup"><span data-stu-id="1fe34-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1fe34-152">選取 [帳戶資訊]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-152">Select **Account info** .</span></span>

3. <span data-ttu-id="1fe34-153">在 [Microsoft 客戶合約]  下方，選取 [更新]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="更新":::

4. <span data-ttu-id="1fe34-155">輸入接受合約之使用者的[名字]  、[姓氏]  、[電子郵件地址]  、[電話號碼]  (選用)。</span><span class="sxs-lookup"><span data-stu-id="1fe34-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="1fe34-156">在 [合約接受日期]  下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1fe34-157">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="1fe34-158">選取 [儲存並繼續]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="1fe34-159">為現有客戶建立新訂單時確認客戶接受</span><span class="sxs-lookup"><span data-stu-id="1fe34-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="1fe34-160">如果您嘗試為以前沒有確認過的現有客戶建立新訂單，您會收到完成確認的提示。</span><span class="sxs-lookup"><span data-stu-id="1fe34-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="1fe34-161">使用下列程序來執行此動作。</span><span class="sxs-lookup"><span data-stu-id="1fe34-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="1fe34-162">輸入接受合約之使用者的[名字]  、[姓氏]  、[電子郵件地址]  、[電話號碼]  (選用)。</span><span class="sxs-lookup"><span data-stu-id="1fe34-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="1fe34-163">在 [合約接受日期]  下方，輸入適當的日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1fe34-164">您不能將此日期設定為未來日期。</span><span class="sxs-lookup"><span data-stu-id="1fe34-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="1fe34-165">選取 [儲存並繼續]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1fe34-166">擷取現有客戶的客戶接受確認</span><span class="sxs-lookup"><span data-stu-id="1fe34-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="1fe34-167">您可以使用下列程序，擷取您先前提供過的現有客戶的客戶接受確認。</span><span class="sxs-lookup"><span data-stu-id="1fe34-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="1fe34-168">您必須是系統管理員代理人或銷售代理人，才能執行此動作。</span><span class="sxs-lookup"><span data-stu-id="1fe34-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1fe34-169">選取 [客戶]，然後尋找並選取您想要查看的客戶。</span><span class="sxs-lookup"><span data-stu-id="1fe34-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1fe34-170">選取 [帳戶資訊]  。</span><span class="sxs-lookup"><span data-stu-id="1fe34-170">Select **Account info** .</span></span>

3. <span data-ttu-id="1fe34-171">在[Microsoft 客戶合約]  下方，您會看到是否已為這個客戶提供確認。</span><span class="sxs-lookup"><span data-stu-id="1fe34-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1fe34-172">後續步驟</span><span class="sxs-lookup"><span data-stu-id="1fe34-172">Next steps</span></span>

- [<span data-ttu-id="1fe34-173">確認客戶接受 CSP 合作夥伴方案中的 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="1fe34-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="1fe34-174">代表客戶證明接受 Microsoft 客戶合約</span><span class="sxs-lookup"><span data-stu-id="1fe34-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)