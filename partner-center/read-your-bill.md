---
title: 如何讀取帳單 & 偵察檔
ms.topic: article
ms.date: 06/05/2020
description: 深入瞭解您的發票 & 對帳檔案。 您的帳單會顯示該月期間內的方案、產品和客戶合作夥伴中心費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215810"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a><span data-ttu-id="0e074-104">瞭解您的帳單和對帳檔案-瞭解如何在合作夥伴中心中尋找</span><span class="sxs-lookup"><span data-stu-id="0e074-104">Understand your bill and reconciliation file - learn how to find them in Partner Center</span></span>


<span data-ttu-id="0e074-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="0e074-105">**Appropriate roles**</span></span>

- <span data-ttu-id="0e074-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="0e074-106">Global admin</span></span>
- <span data-ttu-id="0e074-107">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="0e074-107">Billing admin</span></span>
- <span data-ttu-id="0e074-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="0e074-108">Admin agent</span></span>


<span data-ttu-id="0e074-109">您的 **發票** 是 **所有合作夥伴中心費用的摘要** ， (整個方案、所有產品和所有客戶) 。</span><span class="sxs-lookup"><span data-stu-id="0e074-109">Your **invoice** is a **summary of all your Partner Center charges** (across the program, all products, and all customers).</span></span> 

## <a name="invoice-types"></a><span data-ttu-id="0e074-110">發票類型</span><span class="sxs-lookup"><span data-stu-id="0e074-110">Invoice types</span></span>

<span data-ttu-id="0e074-111">Microsoft 會針對任何以授權為基礎的費用發出一張發票 (例如，Office 365) 和以使用量為基礎的費用 (例如 Azure) ，以及針對一次性費用的個別發票 (例如 Azure RI、Marketplace 或 Azure 方案) 。</span><span class="sxs-lookup"><span data-stu-id="0e074-111">Microsoft will issue one invoice for any license-based charges (such as Office 365) and usage-based charges (such as Azure) and a separate invoice for one-time charges (such as Azure RI, Marketplace, or Azure plan).</span></span>

<span data-ttu-id="0e074-112">例如，</span><span class="sxs-lookup"><span data-stu-id="0e074-112">For example,</span></span>  

<span data-ttu-id="0e074-113">**案例 1 [單一貨幣]**：合作夥伴已購買145P 供應專案和 O365 授權</span><span class="sxs-lookup"><span data-stu-id="0e074-113">**Scenario 1 [Single Currency]**: Partner has purchases for 145P offer and O365 licenses,</span></span>  

- <span data-ttu-id="0e074-114">合作夥伴會取得一個發票 PDF 和2個對帳檔案，其中涵蓋 O365 和 Azure (145p) 的費用。</span><span class="sxs-lookup"><span data-stu-id="0e074-114">Partner will get one invoice PDF and 2 reconciliation files covering the charges for both O365 and Azure (145p).</span></span>  

<span data-ttu-id="0e074-115">**案例 2 [單一貨幣]**：合作夥伴已購買 azure RI、Marketplace 及/或 azure 方案，以及145p 購買。</span><span class="sxs-lookup"><span data-stu-id="0e074-115">**Scenario 2 [Single Currency]**: Partner has purchases for Azure RI, Marketplace and/or Azure plan along with 145p purchases.</span></span>

- <span data-ttu-id="0e074-116">合作夥伴會取得一個發票 PDF，以及涵蓋 Azure (145p) 費用的對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="0e074-116">Partner will get one invoice PDF and a reconciliation file covering the charges for Azure (145p).</span></span> 

- <span data-ttu-id="0e074-117">合作夥伴會收到另一個發票 PDF 和一個對帳檔案，其中涵蓋其 Azure RI、Marketplace、Azure 方案的費用。</span><span class="sxs-lookup"><span data-stu-id="0e074-117">Partner will receive another invoice PDF and a reconciliation file covering their charges for Azure RI, Marketplace, Azure plan.</span></span> 

<span data-ttu-id="0e074-118">**案例 3 [多貨幣]**：合作夥伴已在丹麥幣和 azure 方案中購買 azure RI 以及歐元的145p 購買。</span><span class="sxs-lookup"><span data-stu-id="0e074-118">**Scenario 3 [Multi-Currency]**: Partner has purchases for Azure RI in DKK and Azure plan in EUR along with 145p purchases in EUR.</span></span>

- <span data-ttu-id="0e074-119">合作夥伴會收到一個發票 PDF 和一個對帳檔案，其中涵蓋丹麥幣中 Azure RI 的費用。</span><span class="sxs-lookup"><span data-stu-id="0e074-119">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure RI in DKK.</span></span> 

- <span data-ttu-id="0e074-120">合作夥伴會收到一個發票 PDF，以及一個涵蓋 Azure 方案費用的對帳檔案（以歐元計算）。</span><span class="sxs-lookup"><span data-stu-id="0e074-120">Partner will receive one invoice PDF and a reconciliation file covering the charges for Azure plan in EUR.</span></span> 

- <span data-ttu-id="0e074-121">合作夥伴會收到另一個發票 PDF 和一個對帳檔案，其中涵蓋其145p 優惠的歐元 (或合作夥伴的帳單貨幣) 費用。</span><span class="sxs-lookup"><span data-stu-id="0e074-121">Partner will receive another invoice PDF and a reconciliation file covering their charges for 145p offer in EUR (or partner billing currency).</span></span> 

## <a name="find-your-bill"></a><span data-ttu-id="0e074-122">尋找帳單</span><span class="sxs-lookup"><span data-stu-id="0e074-122">Find your bill</span></span> 

<span data-ttu-id="0e074-123">您可以在 [儀表板] 的 [帳單] 頁面中找到合作夥伴中心的發票。</span><span class="sxs-lookup"><span data-stu-id="0e074-123">You can find your invoice on the Billing page of the dashboard in Partner Center.</span></span> <span data-ttu-id="0e074-124">您也可以在此頁面上找到您的帳單歷程記錄、支出趨勢和對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="0e074-124">You can also find your billing history, spending trends, and reconciliation files on this page.</span></span> 

1. <span data-ttu-id="0e074-125">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。</span><span class="sxs-lookup"><span data-stu-id="0e074-125">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span> 

2. <span data-ttu-id="0e074-126">在左側功能表中，選取 [ **計費**]。</span><span class="sxs-lookup"><span data-stu-id="0e074-126">In the left-hand menu, select **Billing**.</span></span> 

3. <span data-ttu-id="0e074-127">在 [帳單] 頁面上，選取您要下載的發票。</span><span class="sxs-lookup"><span data-stu-id="0e074-127">On the Billing page, select the invoice you want to download.</span></span> 

<span data-ttu-id="0e074-128">您可以在頁面頂端的 [帳戶餘額] 下的 [上次發票日期] 中找到最新發票的連結。</span><span class="sxs-lookup"><span data-stu-id="0e074-128">You can find a link to your latest invoice at the top of the page under Account balance as of last invoice date.</span></span> 

<span data-ttu-id="0e074-129">您可以在 [帳單記錄] 區段中找到先前的發票。</span><span class="sxs-lookup"><span data-stu-id="0e074-129">You can find previous invoices in the Billing history section.</span></span> <span data-ttu-id="0e074-130">選擇適當的年份，然後選取適當計費週期旁的下拉式箭號。</span><span class="sxs-lookup"><span data-stu-id="0e074-130">Choose the appropriate year, then select the drop-down arrow next to the appropriate Billing period.</span></span> <span data-ttu-id="0e074-131">選取發票 ( .pdf) 旁的連結，以下載該期間的發票。</span><span class="sxs-lookup"><span data-stu-id="0e074-131">Select the link next to Invoices (.pdf) to download that period's invoice.</span></span> 

## <a name="understanding-invoice-pdf"></a><span data-ttu-id="0e074-132">瞭解發票 PDF</span><span class="sxs-lookup"><span data-stu-id="0e074-132">Understanding invoice PDF</span></span> 

<span data-ttu-id="0e074-133">**使用量和以授權為基礎的費用發票**：適用于 Office 365 和 Azure 等服務費用的發票將于您所選計費日期的兩 (2) 天內提供 [UTC]。</span><span class="sxs-lookup"><span data-stu-id="0e074-133">**Invoices for Usage and license-based charges**: Invoices for charges for services such as Office 365 and Azure will be available within two (2) days of your selected billing date [UTC].</span></span>  

<span data-ttu-id="0e074-134">**Onetime 和週期性費用的發票**：服務的費用發票（例如 azure RI、azure 方案、Marketplace）將于每月的每月8日之後提供。</span><span class="sxs-lookup"><span data-stu-id="0e074-134">**Invoices for onetime and recurring charges**: Invoices for charges for services such as Azure RI, Azure plan, Marketplace will be available not later than 8th of every month.</span></span>  

<span data-ttu-id="0e074-135">以下是發票 PDF 檔上的一些索引鍵欄位–</span><span class="sxs-lookup"><span data-stu-id="0e074-135">Below are some of the key fields on the Invoice PDF document –</span></span>

<span data-ttu-id="0e074-136">**發票號碼**：針對個別計費期間所產生發票檔的唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="0e074-136">**Invoice number**: Unique identifier for the invoice document generated for the respective billing period.</span></span> 

<span data-ttu-id="0e074-137">**計費週期**：這是您使用使用方式和授權型服務的期間。</span><span class="sxs-lookup"><span data-stu-id="0e074-137">**Billing period**: This is the period during which you have usages and license-based services.</span></span> 

<span data-ttu-id="0e074-138">**發票日期**：每個月產生發票的計費日期或週年日。</span><span class="sxs-lookup"><span data-stu-id="0e074-138">**Invoice date**: The billing date or anniversary date on which your invoice is generated each month.</span></span> 

<span data-ttu-id="0e074-139">**付款到期日**：必須收到付款的日期。</span><span class="sxs-lookup"><span data-stu-id="0e074-139">**Payment due date**: The date by which your payment must be received.</span></span> 

<span data-ttu-id="0e074-140">**費用**：依計費期計費的帳單貨幣所應付的金額。</span><span class="sxs-lookup"><span data-stu-id="0e074-140">**Charges**: The amount due in your billing currency for the respective billing period.</span></span> 

<span data-ttu-id="0e074-141">**信用額度**：點數 (例如 SLA) 或對訂用帳戶所做的調整 (例如，授權增加或減少) 。</span><span class="sxs-lookup"><span data-stu-id="0e074-141">**Credits**: Credits (such as SLA) or adjustments for changes made to subscriptions (for example, license increases or decreases).</span></span> 

<span data-ttu-id="0e074-142">**付款指示**：如何根據您的區域支付發票的說明。</span><span class="sxs-lookup"><span data-stu-id="0e074-142">**Payment instructions**: Description of how to pay your invoice, based on your region.</span></span> <span data-ttu-id="0e074-143">付款時，務必要包含您的發票號碼。</span><span class="sxs-lookup"><span data-stu-id="0e074-143">Always be sure to include your invoice number when making a payment.</span></span> 

<span data-ttu-id="0e074-144">如需發票檔案中所有欄位的詳細描述 (包含一次性費用) 的欄位，請參閱 [發票檔案欄位](invoice-file.md)。</span><span class="sxs-lookup"><span data-stu-id="0e074-144">For a detailed description of all the fields in your invoice file (including fields for one-time charges), see [Invoice file fields](invoice-file.md).</span></span> 

## <a name="understand-reconciliation-files"></a><span data-ttu-id="0e074-145">瞭解對帳檔案</span><span class="sxs-lookup"><span data-stu-id="0e074-145">Understand reconciliation files</span></span>

 <span data-ttu-id="0e074-146">針對您的費用提供深入探討/詳述詳細資料的對帳檔案，可隨發票 PDF 下載。</span><span class="sxs-lookup"><span data-stu-id="0e074-146">Reconciliation files, which provides a drill down/itemized details of your charges, are available to download along with the Invoice PDF.</span></span> <span data-ttu-id="0e074-147">對帳檔案包含客戶識別碼和訂用帳戶識別碼，您可以用來建立客戶的發票。</span><span class="sxs-lookup"><span data-stu-id="0e074-147">The reconciliation files include customer identifiers and subscription identifiers that you can use to create customer invoices.</span></span> <span data-ttu-id="0e074-148">請參閱  [如何使用對帳](use-the-reconciliation-files.md) 檔案，以取得更多有關偵察檔案的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="0e074-148">Please refer to  [How to use the reconciliation files](use-the-reconciliation-files.md) to get more details on the recon files.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0e074-149">後續步驟</span><span class="sxs-lookup"><span data-stu-id="0e074-149">Next steps</span></span>

- [<span data-ttu-id="0e074-150">如何使用對帳檔案</span><span class="sxs-lookup"><span data-stu-id="0e074-150">How to use the reconciliation files</span></span>](use-the-reconciliation-files.md)