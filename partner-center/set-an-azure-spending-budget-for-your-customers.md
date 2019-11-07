---
title: 為客戶設定 Azure 消費預算 | 合作夥伴中心
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在合作夥伴中心，您可以為每個客戶設定每月預算，讓他們的 Azure 帳單不會在月底結束時感到驚訝。
ms.assetid: DDE80361-D04E-432C-BC15-D735D2AE954F
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 03901b4b17c744c0c91d732331842f6cb579bf88
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73654063"
---
# <a name="set-an-azure-spending-budget-for-your-customers"></a><span data-ttu-id="c8c52-103">為客戶設定 Azure 消費預算</span><span class="sxs-lookup"><span data-stu-id="c8c52-103">Set an Azure spending budget for your customers</span></span>

<span data-ttu-id="c8c52-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="c8c52-104">**Applies to**</span></span>

-  <span data-ttu-id="c8c52-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="c8c52-105">Partner Center</span></span>
-  <span data-ttu-id="c8c52-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="c8c52-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c8c52-107">為了協助客戶管理其 Azure 費用，您可以設定每月費用預算，讓其 Azure 帳單不會高於預期的費用。</span><span class="sxs-lookup"><span data-stu-id="c8c52-107">To help customers manage their Azure spending, you can set a monthly spending budget so that their Azure bill isn't higher than they anticipated.</span></span> <span data-ttu-id="c8c52-108">設定 Azure 消費預算可讓您將客戶的 Azure 消費與當月份預算做比較。</span><span class="sxs-lookup"><span data-stu-id="c8c52-108">Setting an Azure spending budget allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="c8c52-109">有了這項功能，您就可以：</span><span class="sxs-lookup"><span data-stu-id="c8c52-109">With this feature, you can:</span></span> 

-   <span data-ttu-id="c8c52-110">在客戶的消費金額接近預算限制時收到電子郵件通知</span><span class="sxs-lookup"><span data-stu-id="c8c52-110">Be notified by email if a customer's spending is near the budget limit</span></span>
-   <span data-ttu-id="c8c52-111">每月審查客戶的預估 Azure 成本</span><span class="sxs-lookup"><span data-stu-id="c8c52-111">Review your customers' estimated Azure costs per month</span></span>
-   <span data-ttu-id="c8c52-112">發現設定不當的服務，或看出浮現詐騙跡象的異常用量趨勢</span><span class="sxs-lookup"><span data-stu-id="c8c52-112">Spot a misconfigured service, or unusual usage trends that might suggest fraud</span></span>
-   <span data-ttu-id="c8c52-113">和客戶合作，共同找出根本的問題，並設法管理費用</span><span class="sxs-lookup"><span data-stu-id="c8c52-113">Work with the customer to identify the root issue and manage costs</span></span>
-   <span data-ttu-id="c8c52-114">如果您和您的客戶皆同意，可以將預算調整為較高金額</span><span class="sxs-lookup"><span data-stu-id="c8c52-114">Change the budget to a higher amount if you and your customer are comfortable with it</span></span>

<span data-ttu-id="c8c52-115">Azure 消費資料為估計值，實際帳單金額可能會有差異，這個值不含稅、點數、帳務調整或其他需要支付的費用。</span><span class="sxs-lookup"><span data-stu-id="c8c52-115">The Azure spending data is an estimate, actual billing amounts may vary, and the value does not reflect taxes, credits, adjustments, or other charges that may apply.</span></span> <span data-ttu-id="c8c52-116">消費資料每天重新整理一次。</span><span class="sxs-lookup"><span data-stu-id="c8c52-116">Spending data is refreshed once per day.</span></span> <span data-ttu-id="c8c52-117">除非您在 Azure 入口網站變更客戶的帳戶設定，否則客戶仍將繼續使用 Azure 服務及資源，並支付相關費用。</span><span class="sxs-lookup"><span data-stu-id="c8c52-117">Customers will continue to use—and be charged for—Azure services and resources unless you change their account settings in the Azure portal.</span></span> 

> [!NOTE]  
> <span data-ttu-id="c8c52-118">這項功能無法在沙箱中使用，或在生產（TIP）帳戶中測試。</span><span class="sxs-lookup"><span data-stu-id="c8c52-118">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="c8c52-119">**開啟電子郵件通知**</span><span class="sxs-lookup"><span data-stu-id="c8c52-119">**Turn on email notifications**</span></span>
1.  <span data-ttu-id="c8c52-120">從 [合作夥伴中心] 功能表中，選取 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="c8c52-120">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c8c52-121">將 **\[取得電子郵件\]** 選項切換為要在客戶的使用達預算的 80% 以上時收到通知。</span><span class="sxs-lookup"><span data-stu-id="c8c52-121">Toggle on the **Get emails** option to be notified when customers use 80% or more of their budget.</span></span> <span data-ttu-id="c8c52-122">這樣能協助您留意 Azure 帳單。</span><span class="sxs-lookup"><span data-stu-id="c8c52-122">This will help you keep an eye on your Azure bill.</span></span> <span data-ttu-id="c8c52-123">您可以將預設的電子郵件地址變更為個人或其他電子郵件以接收通知。</span><span class="sxs-lookup"><span data-stu-id="c8c52-123">You can change the default email address to a personal or any other email to receive notifications.</span></span>

<span data-ttu-id="c8c52-124">**設定預算**</span><span class="sxs-lookup"><span data-stu-id="c8c52-124">**Set a budget**</span></span>
1.  <span data-ttu-id="c8c52-125">從 [合作夥伴中心] 功能表中，選取 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="c8c52-125">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c8c52-126">選取您想要為其設定預算的客戶。</span><span class="sxs-lookup"><span data-stu-id="c8c52-126">Select the customer(s) you want to set a budget for.</span></span> 
3. <span data-ttu-id="c8c52-127">在 **\[每月預算\]** 方塊中輸入一個值並選取 **\[套用\]** 。</span><span class="sxs-lookup"><span data-stu-id="c8c52-127">Enter a value in the **Monthly budget** box and then select **Apply**.</span></span>
4.  <span data-ttu-id="c8c52-128">若要檢查目前的消費，請返回此頁面。</span><span class="sxs-lookup"><span data-stu-id="c8c52-128">To check current spending, return to this page.</span></span>
5.  <span data-ttu-id="c8c52-129">也可以從客戶管理頁面的 **\[用量型訂閱\]** 設定個別的預算。</span><span class="sxs-lookup"><span data-stu-id="c8c52-129">Individual budgets can also be set under **Usage-based subscriptions** on a customer management page.</span></span>

<span data-ttu-id="c8c52-130">**移除預算**</span><span class="sxs-lookup"><span data-stu-id="c8c52-130">**Remove a budget**</span></span>
1.  <span data-ttu-id="c8c52-131">從 [合作夥伴中心] 功能表中，選取 [ **Azure 費用**]。</span><span class="sxs-lookup"><span data-stu-id="c8c52-131">From the Partner Center menu, select **Azure spending**.</span></span>
2.  <span data-ttu-id="c8c52-132">從清單中選取客戶。</span><span class="sxs-lookup"><span data-stu-id="c8c52-132">Select customers from the list.</span></span>
3.  <span data-ttu-id="c8c52-133">選取 **\[移除預算\]** 。</span><span class="sxs-lookup"><span data-stu-id="c8c52-133">Select **Remove budget**.</span></span>

<span data-ttu-id="c8c52-134">**查看詳細成本**</span><span class="sxs-lookup"><span data-stu-id="c8c52-134">**See itemized costs**</span></span>
1.  <span data-ttu-id="c8c52-135">從 [合作夥伴中心] 功能表中，選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="c8c52-135">From the Partner Center menu, select **Customers**.</span></span>
2.  <span data-ttu-id="c8c52-136">從客戶清單中選取客戶。</span><span class="sxs-lookup"><span data-stu-id="c8c52-136">From the customer list, select a customer.</span></span>
3.  <span data-ttu-id="c8c52-137">在其客戶管理頁面中，於 **\[用量型訂閱\]** 下選擇一項訂閱。</span><span class="sxs-lookup"><span data-stu-id="c8c52-137">On their customer management page, under **Usage-based subscriptions**, choose a subscription.</span></span> <span data-ttu-id="c8c52-138">檢視其目前的預估用量及依服務分項的支出清單。</span><span class="sxs-lookup"><span data-stu-id="c8c52-138">View its current estimated usage and a list of itemized costs by service.</span></span>


 

 



