---
title: 為客戶設定 Azure 消費預算 | 合作夥伴中心
ms.topic: article
ms.date: 11/21/2019
description: 瞭解如何為您的客戶設定或移除每月的 Azure 費用預算，同時也可查看 Azure 費用資料並設定預算相關通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e33a15110666bb3b4a3c76c198cde7a59d81411f
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/05/2020
ms.locfileid: "82797886"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="91e70-103">為客戶設定 Azure 消費預算</span><span class="sxs-lookup"><span data-stu-id="91e70-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="91e70-104">適用於：</span><span class="sxs-lookup"><span data-stu-id="91e70-104">Applies to:</span></span>

- <span data-ttu-id="91e70-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="91e70-105">Partner Center</span></span>
- <span data-ttu-id="91e70-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="91e70-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="91e70-107">您可以在合作夥伴中心[為您的客戶設定每月的 Azure 費用預算](#set-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="91e70-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="91e70-108">這可協助您的客戶管理其 Azure 費用。</span><span class="sxs-lookup"><span data-stu-id="91e70-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="91e70-109">此選項可讓您將客戶的 Azure 費用與當月的預算進行比較。</span><span class="sxs-lookup"><span data-stu-id="91e70-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="91e70-110">它也可協助您的客戶預算其 Azure 費用，讓其每月帳單不會高於預期。</span><span class="sxs-lookup"><span data-stu-id="91e70-110">It also helps your customers budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>


> [!NOTE]  
> <span data-ttu-id="91e70-111">這項功能無法在沙箱中使用，或在生產（TIP）帳戶中測試。</span><span class="sxs-lookup"><span data-stu-id="91e70-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="91e70-112">[為客戶設定 Azure 消費預算](#set-azure-spending-budget)之後，您也可以透過下列方式來審查客戶的使用量。</span><span class="sxs-lookup"><span data-stu-id="91e70-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="91e70-113">這些選項可協助您找出設定錯誤的服務或可能會建議詐騙的異常趨勢。</span><span class="sxs-lookup"><span data-stu-id="91e70-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="91e70-114">接著，您可以與您的客戶合作，找出根本原因並管理成本。</span><span class="sxs-lookup"><span data-stu-id="91e70-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="91e70-115">如有必要，您也可以[將客戶的預算變更](#set-azure-spending-budget)為較高的金額。</span><span class="sxs-lookup"><span data-stu-id="91e70-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="91e70-116">檢查目前的 Azure 費用</span><span class="sxs-lookup"><span data-stu-id="91e70-116">Check current Azure spending</span></span>](#check-current-azure-spending)
- [<span data-ttu-id="91e70-117">當客戶的支出接近預算限制時，開啟電子郵件通知</span><span class="sxs-lookup"><span data-stu-id="91e70-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)
- [<span data-ttu-id="91e70-118">依據依使用量的訂用帳戶，查看服務的明細成本</span><span class="sxs-lookup"><span data-stu-id="91e70-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="91e70-119">您也可以隨時[移除客戶的 Azure 消費預算](#remove-azure-spending-budget)。</span><span class="sxs-lookup"><span data-stu-id="91e70-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="91e70-120">Azure 費用資料</span><span class="sxs-lookup"><span data-stu-id="91e70-120">Azure spending data</span></span>

<span data-ttu-id="91e70-121">Azure 消費資料是*估計值*，而*實際的計費金額可能會有所不同*。</span><span class="sxs-lookup"><span data-stu-id="91e70-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="91e70-122">資料的值*不會反映*可能適用的稅金、信用額度、調整或其他費用。</span><span class="sxs-lookup"><span data-stu-id="91e70-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="91e70-123">消費資料每天會重新整理*一次*。</span><span class="sxs-lookup"><span data-stu-id="91e70-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="91e70-124">除非您變更 Azure 入口網站中的帳戶設定，否則您的客戶可以繼續使用（並收取） Azure 服務和資源。</span><span class="sxs-lookup"><span data-stu-id="91e70-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="91e70-125">設定 Azure 消費預算</span><span class="sxs-lookup"><span data-stu-id="91e70-125">Set Azure spending budget</span></span>

<span data-ttu-id="91e70-126">您可以為合作夥伴中心內的多個客戶*設定每月 Azure 費用預算*：</span><span class="sxs-lookup"><span data-stu-id="91e70-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="91e70-127">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="91e70-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="91e70-128">在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="91e70-129">在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用**帳戶的客戶] 底下，選取您想要設定預算的客戶。</span><span class="sxs-lookup"><span data-stu-id="91e70-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>
4. <span data-ttu-id="91e70-130">輸入 [**每月預算**] 的值。</span><span class="sxs-lookup"><span data-stu-id="91e70-130">Enter a value for **Monthly budget**.</span></span>
5. <span data-ttu-id="91e70-131">選擇 **[** 套用] 以儲存變更。</span><span class="sxs-lookup"><span data-stu-id="91e70-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="91e70-132">您也可以在其訂用帳戶設定中*為個別客戶設定預算*：</span><span class="sxs-lookup"><span data-stu-id="91e70-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="91e70-133">登入合作夥伴中心儀表板。</span><span class="sxs-lookup"><span data-stu-id="91e70-133">Sign in to the Partner Center dashboard.</span></span>
2. <span data-ttu-id="91e70-134">在左側功能表中，選擇 [ **CSP**] 底下的 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="91e70-135">在 [**客戶**] 頁面上，選取客戶的**公司名稱**。</span><span class="sxs-lookup"><span data-stu-id="91e70-135">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="91e70-136">在 [客戶的訂用帳戶 **] 頁面的**[**使用量型訂閱**] 底下，選擇 [**變更預算**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>
5. <span data-ttu-id="91e70-137">輸入預算的值。</span><span class="sxs-lookup"><span data-stu-id="91e70-137">Enter a value for the budget.</span></span>
6. <span data-ttu-id="91e70-138">選擇 **[** 套用] 以儲存變更。</span><span class="sxs-lookup"><span data-stu-id="91e70-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="91e70-139">移除 Azure 費用預算</span><span class="sxs-lookup"><span data-stu-id="91e70-139">Remove Azure spending budget</span></span>

<span data-ttu-id="91e70-140">您可以在合作夥伴中心移除客戶的*每月 Azure 費用預算*：</span><span class="sxs-lookup"><span data-stu-id="91e70-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="91e70-141">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="91e70-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="91e70-142">在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="91e70-143">在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用帳戶的客戶**] 底下，選取您想要移除其預算的客戶。</span><span class="sxs-lookup"><span data-stu-id="91e70-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>
4. <span data-ttu-id="91e70-144">選擇 [**移除預算**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="91e70-145">檢查目前的 Azure 費用</span><span class="sxs-lookup"><span data-stu-id="91e70-145">Check current Azure spending</span></span>

<span data-ttu-id="91e70-146">您可以隨時*追蹤客戶目前的 Azure 支出和每月預算*：</span><span class="sxs-lookup"><span data-stu-id="91e70-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="91e70-147">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="91e70-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="91e70-148">在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="91e70-149">在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用帳戶的客戶**] 底下，您可以看到客戶的每月預算、目前的支出預估和所用預算百分比的總覽。</span><span class="sxs-lookup"><span data-stu-id="91e70-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="91e70-150">預算限制的通知</span><span class="sxs-lookup"><span data-stu-id="91e70-150">Notifications for budget limits</span></span>

<span data-ttu-id="91e70-151">當客戶的每月費用接近其預算限制時，您可以*開啟電子郵件通知*。</span><span class="sxs-lookup"><span data-stu-id="91e70-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="91e70-152">當您開啟此選項時，當客戶使用80% 或以上的每月預算時，系統會通知您。</span><span class="sxs-lookup"><span data-stu-id="91e70-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="91e70-153">此選項可協助您隨時留意 Azure 帳單。</span><span class="sxs-lookup"><span data-stu-id="91e70-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="91e70-154">若要設定電子郵件通知：</span><span class="sxs-lookup"><span data-stu-id="91e70-154">To configure email notifications:</span></span>

1. <span data-ttu-id="91e70-155">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="91e70-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="91e70-156">在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-156">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>
3. <span data-ttu-id="91e70-157">在 [ **Azure 消費**] 頁面的 [**電子郵件通知**] 下，將 [**取得電子郵件**] 設定切換為 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-157">On the **Azure spending** page, under **Email notifications**, toggle the **Get emails** setting to **On**.</span></span>
4. <span data-ttu-id="91e70-158">選擇 [**變更電子郵件地址**] 以查看通知的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="91e70-158">Choose **Change email address** to see the email address for notifications.</span></span>
5. <span data-ttu-id="91e70-159">如果電子郵件地址*不正確*，請輸入正確的電子郵件地址，然後選擇 [**更新**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-159">If the email address *isn't correct*, enter the correct email address and choose **Update**.</span></span> <span data-ttu-id="91e70-160">如果電子郵件地址*正確無誤*，請選擇 [**取消**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-160">If the email address *is correct*, choose **Cancel**.</span></span>

## <a name="itemized-costs-by-service"></a><span data-ttu-id="91e70-161">依服務的明細成本</span><span class="sxs-lookup"><span data-stu-id="91e70-161">Itemized costs by service</span></span>

<span data-ttu-id="91e70-162">您可以*針對使用量型訂用帳戶，根據服務來查看明細成本（和預估使用量）*：</span><span class="sxs-lookup"><span data-stu-id="91e70-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="91e70-163">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="91e70-163">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="91e70-164">在左側功能表中，選擇 [ **CSP**] 底下的 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="91e70-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>
3. <span data-ttu-id="91e70-165">在 [**客戶**] 頁面上，選取客戶的**公司名稱**。</span><span class="sxs-lookup"><span data-stu-id="91e70-165">On the **Customers** page, select the customer's **Company name**.</span></span>
4. <span data-ttu-id="91e70-166">在 [客戶的**訂閱**] 頁面的 [**使用量型訂閱**] 底下，選取**訂**用帳戶的名稱。</span><span class="sxs-lookup"><span data-stu-id="91e70-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>
5. <span data-ttu-id="91e70-167">在訂用帳戶的頁面上，您可以查看服務的**明細成本**，以及當月的**預估使用量**。</span><span class="sxs-lookup"><span data-stu-id="91e70-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
