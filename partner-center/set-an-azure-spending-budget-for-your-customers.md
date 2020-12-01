---
title: 為客戶設定 Azure 費用預算
ms.topic: how-to
ms.date: 06/03/2020
description: 瞭解如何為您的客戶設定或移除每月 Azure 費用預算，以及查看 Azure 費用資料並設定預算相關的通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438989"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="01d90-103">在合作夥伴中心中設定、檢查或移除客戶的每月 Azure 費用預算</span><span class="sxs-lookup"><span data-stu-id="01d90-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="01d90-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="01d90-104">Applies to:</span></span>

- <span data-ttu-id="01d90-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="01d90-105">Partner Center</span></span>
- <span data-ttu-id="01d90-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="01d90-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="01d90-107">您可以在合作夥伴中心中 [為您的客戶設定每月的 Azure 支出預算](#set-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="01d90-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="01d90-108">這可協助您的客戶管理其 Azure 費用。</span><span class="sxs-lookup"><span data-stu-id="01d90-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="01d90-109">此選項可讓您比較客戶的 Azure 費用與該月的預算。</span><span class="sxs-lookup"><span data-stu-id="01d90-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="01d90-110">它也可協助您的客戶為其 Azure 費用編制預算，讓其每月帳單不會高於預期。</span><span class="sxs-lookup"><span data-stu-id="01d90-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="01d90-111">這項功能不適用於沙箱或在生產環境中測試 (提示) 帳戶。</span><span class="sxs-lookup"><span data-stu-id="01d90-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="01d90-112">[為客戶 (的) 設定 Azure 費用預算](#set-azure-spending-budget)之後，您也可以透過下列方式來檢查客戶的使用方式。</span><span class="sxs-lookup"><span data-stu-id="01d90-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="01d90-113">這些選項可協助您找出設定錯誤的服務或可能會建議詐騙的不尋常趨勢。</span><span class="sxs-lookup"><span data-stu-id="01d90-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="01d90-114">然後，您可以與客戶 (的) ，以找出根本原因和管理成本。</span><span class="sxs-lookup"><span data-stu-id="01d90-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="01d90-115">如有必要，您也可以 [將客戶的預算變更](#set-azure-spending-budget) 為較高的金額。</span><span class="sxs-lookup"><span data-stu-id="01d90-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="01d90-116">檢查目前的 Azure 費用</span><span class="sxs-lookup"><span data-stu-id="01d90-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="01d90-117">當客戶的支出接近預算限制時，開啟電子郵件通知</span><span class="sxs-lookup"><span data-stu-id="01d90-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="01d90-118">依使用量的訂用帳戶來查看依服務區分的成本</span><span class="sxs-lookup"><span data-stu-id="01d90-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="01d90-119">您也可以隨時移除客戶 () 的 [Azure 消費預算](#remove-azure-spending-budget) 。</span><span class="sxs-lookup"><span data-stu-id="01d90-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="01d90-120">Azure 費用資料</span><span class="sxs-lookup"><span data-stu-id="01d90-120">Azure spending data</span></span>

<span data-ttu-id="01d90-121">Azure 費用資料是 *估計值* ，而 *實際計費金額可能會有所不同*。</span><span class="sxs-lookup"><span data-stu-id="01d90-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="01d90-122">資料的值 *不會反映* 可能適用的稅金、信用額度、調整或其他費用。</span><span class="sxs-lookup"><span data-stu-id="01d90-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="01d90-123">消費資料每天重新整理 *一次*。</span><span class="sxs-lookup"><span data-stu-id="01d90-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="01d90-124">除非您在 Azure 入口網站中變更其帳戶設定，否則您的客戶可以繼續使用 (並向) 的 Azure 服務和資源收費。</span><span class="sxs-lookup"><span data-stu-id="01d90-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="01d90-125">設定 Azure 費用預算</span><span class="sxs-lookup"><span data-stu-id="01d90-125">Set Azure spending budget</span></span>

<span data-ttu-id="01d90-126">您可以在合作夥伴中心中為多個客戶 *設定每月 Azure 消費預算* ：</span><span class="sxs-lookup"><span data-stu-id="01d90-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="01d90-127">登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="01d90-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="01d90-128">在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="01d90-129">在 [ **Azure 費用** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，選取您要設定預算的客戶 () 。</span><span class="sxs-lookup"><span data-stu-id="01d90-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="01d90-130">輸入 **每月預算** 的值。</span><span class="sxs-lookup"><span data-stu-id="01d90-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="01d90-131">選擇 [套用] 以儲存 **您的變更** 。</span><span class="sxs-lookup"><span data-stu-id="01d90-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="01d90-132">您也可以在訂用帳戶設定中 *設定個別客戶的預算* ：</span><span class="sxs-lookup"><span data-stu-id="01d90-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="01d90-133">登入合作夥伴中心儀表板。</span><span class="sxs-lookup"><span data-stu-id="01d90-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="01d90-134">在 [ **CSP**] 下的左側功能表中，選擇 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="01d90-135">在 [ **客戶** ] 頁面上，選取客戶的 **公司名稱**。</span><span class="sxs-lookup"><span data-stu-id="01d90-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="01d90-136">在 [客戶的訂用帳戶 **] 頁面的** [ **基於使用方式的訂** 用帳戶] 下，選擇 [ **變更預算**]</span><span class="sxs-lookup"><span data-stu-id="01d90-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="01d90-137">輸入預算的值。</span><span class="sxs-lookup"><span data-stu-id="01d90-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="01d90-138">選擇 [套用] 以儲存 **您的變更** 。</span><span class="sxs-lookup"><span data-stu-id="01d90-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="01d90-139">移除 Azure 費用預算</span><span class="sxs-lookup"><span data-stu-id="01d90-139">Remove Azure spending budget</span></span>

<span data-ttu-id="01d90-140">您可以在合作夥伴中心中移除客戶 () 的 *每月 Azure 費用預算* ：</span><span class="sxs-lookup"><span data-stu-id="01d90-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="01d90-141">登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="01d90-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="01d90-142">在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="01d90-143">在 [ **Azure 費用** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，選取您要移除其預算的客戶 (s) 。</span><span class="sxs-lookup"><span data-stu-id="01d90-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="01d90-144">選擇 [ **移除預算**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="01d90-145">檢查目前的 Azure 費用</span><span class="sxs-lookup"><span data-stu-id="01d90-145">Check current Azure spending</span></span>

<span data-ttu-id="01d90-146">您可以隨時 *追蹤客戶目前的 Azure 費用和每月預算* ：</span><span class="sxs-lookup"><span data-stu-id="01d90-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="01d90-147">登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="01d90-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="01d90-148">在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="01d90-149">在 [ **Azure 消費** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，您可以看到客戶的每月預算、目前的費用預估，以及使用的預算百分比。</span><span class="sxs-lookup"><span data-stu-id="01d90-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="01d90-150">預算限制的通知</span><span class="sxs-lookup"><span data-stu-id="01d90-150">Notifications for budget limits</span></span>

<span data-ttu-id="01d90-151">當客戶的每月費用接近預算限制時，您可以 *開啟電子郵件通知* 。</span><span class="sxs-lookup"><span data-stu-id="01d90-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="01d90-152">當您開啟此選項時，當客戶使用80% 或更多的每月預算時，系統會通知您。</span><span class="sxs-lookup"><span data-stu-id="01d90-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="01d90-153">此選項可協助您隨時留意 Azure 帳單。</span><span class="sxs-lookup"><span data-stu-id="01d90-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="01d90-154">若要設定電子郵件通知：</span><span class="sxs-lookup"><span data-stu-id="01d90-154">To configure email notifications:</span></span>

1. <span data-ttu-id="01d90-155">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="01d90-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="01d90-156">移至 [設定]  。</span><span class="sxs-lookup"><span data-stu-id="01d90-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="01d90-157">選取 [ **我的喜好** 設定]。</span><span class="sxs-lookup"><span data-stu-id="01d90-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="01d90-158">如果沒有，請設定慣用的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="01d90-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="01d90-159">設定通知的慣用語言。</span><span class="sxs-lookup"><span data-stu-id="01d90-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="01d90-160">[**通知喜好** 設定] 區段底下的 [選取 **CSP** ] 索引標籤</span><span class="sxs-lookup"><span data-stu-id="01d90-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="01d90-161">檢查 **Azure 消費** 通知的電子郵件選項，並 **儲存**。</span><span class="sxs-lookup"><span data-stu-id="01d90-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="01d90-162">依服務的詳細成本</span><span class="sxs-lookup"><span data-stu-id="01d90-162">Itemized costs by service</span></span>

<span data-ttu-id="01d90-163">您可以 *針對以使用量為基礎的訂用帳戶，查看服務的詳細成本 (和預估使用量)*：</span><span class="sxs-lookup"><span data-stu-id="01d90-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="01d90-164">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="01d90-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="01d90-165">在 [ **CSP**] 下的左側功能表中，選擇 [ **客戶**]。</span><span class="sxs-lookup"><span data-stu-id="01d90-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="01d90-166">在 [ **客戶** ] 頁面上，選取客戶的 **公司名稱**。</span><span class="sxs-lookup"><span data-stu-id="01d90-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="01d90-167">在 [客戶的訂用帳戶 **] 頁面的** [ **基於使用方式的訂閱**] 下，選取 **訂** 用帳戶的名稱。</span><span class="sxs-lookup"><span data-stu-id="01d90-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="01d90-168">在訂用帳戶的頁面上，您可以依服務查看 **詳細的成本** ，以及當月的 **預估使用量** 。</span><span class="sxs-lookup"><span data-stu-id="01d90-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
