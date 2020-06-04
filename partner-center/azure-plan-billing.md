---
title: Azure 方案計費 - 發票和對帳檔案
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何存取及了解與 Azure 方案計費相關的發票和對帳檔案結構。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: fa1d1298f0fd3650bdaa4e6fc6b602844ac199c4
ms.sourcegitcommit: 83f9c114910282dc87b3ec22d59a8b24b1d6b368
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/01/2020
ms.locfileid: "84262872"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="bc48d-103">CSP 中的新商務體驗 - Azure 計費</span><span class="sxs-lookup"><span data-stu-id="bc48d-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="bc48d-104">**適當的角色：**</span><span class="sxs-lookup"><span data-stu-id="bc48d-104">**Appropriate roles:**</span></span>

- <span data-ttu-id="bc48d-105">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="bc48d-105">Admin agent</span></span>
- <span data-ttu-id="bc48d-106">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="bc48d-106">Billing admin</span></span>
- <span data-ttu-id="bc48d-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bc48d-107">Global admin</span></span>

<span data-ttu-id="bc48d-108">Azure 方案下的計費，是藉由使用一致的單一計費日期和以行事曆月份為基礎的計費期間，簡化的計費體驗。</span><span class="sxs-lookup"><span data-stu-id="bc48d-108">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="bc48d-109">計費基本資訊摘要</span><span class="sxs-lookup"><span data-stu-id="bc48d-109">Summary of billing essentials</span></span>

- <span data-ttu-id="bc48d-110">**發票日期**：發票和對帳檔案在合作夥伴中心儀表板/API 中將於 8 日 (午夜 UTC) 提供。</span><span class="sxs-lookup"><span data-stu-id="bc48d-110">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="bc48d-111">**發票計費期間**：發票計費期間會對應到行事曆月份，例如，10/1-10/31、11/1-11/30。</span><span class="sxs-lookup"><span data-stu-id="bc48d-111">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="bc48d-112">**收費服務期間**：收費將會與行事曆月份一致。</span><span class="sxs-lookup"><span data-stu-id="bc48d-112">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="bc48d-113">例如，如果計費合作夥伴在 10/15 透過 Azure 方案新增 Azure 服務，而客戶在 10/15 開始使用 Azure 服務，則計費合作夥伴會在 11/8 收到 10/15 - 10/31 服務期間客戶使用的發票/對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="bc48d-113">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="bc48d-114">下一個月份的發票會在 12/8 產生，其中包含 11/1- 11/31 服務期間的所有費用。</span><span class="sxs-lookup"><span data-stu-id="bc48d-114">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="bc48d-115">**發票付款期限**：淨 60 天。</span><span class="sxs-lookup"><span data-stu-id="bc48d-115">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="bc48d-116">**發票貨幣**：合作夥伴會繼續以客戶國家/地區的指派貨幣來計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-116">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="bc48d-117">例如，如果計費合作夥伴是在愛爾蘭，而客戶是在英國、挪威和德國，則計費合作夥伴將會收到 GBP、NOK 和 EUR 發票/對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="bc48d-117">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="bc48d-118">**合作夥伴獎勵**：從發票月份結束起算 45 天支付。</span><span class="sxs-lookup"><span data-stu-id="bc48d-118">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="bc48d-119">存取您的發票和對帳檔案</span><span class="sxs-lookup"><span data-stu-id="bc48d-119">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="bc48d-120">貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。</span><span class="sxs-lookup"><span data-stu-id="bc48d-120">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> 

<span data-ttu-id="bc48d-121">**若要存取發票和對帳檔案**</span><span class="sxs-lookup"><span data-stu-id="bc48d-121">**To access the invoice and reconciliation file**</span></span>

1. <span data-ttu-id="bc48d-122">登入合作夥伴中心[儀表板](https://partner.microsoft.com/en-us/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-122">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/).</span></span>

2. <span data-ttu-id="bc48d-123">從 [合作夥伴中心] 功能表中，選取 [計費]。</span><span class="sxs-lookup"><span data-stu-id="bc48d-123">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="bc48d-124">選取 [週期性] 和 [一次性] 的索引標籤，以及您感興趣的貨幣。</span><span class="sxs-lookup"><span data-stu-id="bc48d-124">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

![計費](images/azure/billing3.png)

4. <span data-ttu-id="bc48d-126">選取 [發票] 或 [對帳檔案]。</span><span class="sxs-lookup"><span data-stu-id="bc48d-126">Select **Invoice** or **Reconciliation file**.</span></span>  

<span data-ttu-id="bc48d-127">若要檢視歷程記錄發票和對帳檔案，請展開下方的計費歷程記錄資料列。</span><span class="sxs-lookup"><span data-stu-id="bc48d-127">To view historical invoices and recon files expand the Billing history row below.</span></span>


## <a name="understanding-usage-data"></a><span data-ttu-id="bc48d-128">瞭解使用量資料</span><span class="sxs-lookup"><span data-stu-id="bc48d-128">Understanding usage data</span></span> 

1. <span data-ttu-id="bc48d-129">Azure 方案是使用量的根或最上層容器。</span><span class="sxs-lookup"><span data-stu-id="bc48d-129">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="bc48d-130">所有使用量都會繫結回單一 Azure 方案。</span><span class="sxs-lookup"><span data-stu-id="bc48d-130">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="bc48d-131">在方案中，將會有一或多個 Azure 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="bc48d-131">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="bc48d-132">這些是用於資源管理和部署的容器。</span><span class="sxs-lookup"><span data-stu-id="bc48d-132">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="bc48d-133">在訂用帳戶內，資源群組會新增至群組資源。</span><span class="sxs-lookup"><span data-stu-id="bc48d-133">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="bc48d-134">每個資源都會部署到一個資源群組。</span><span class="sxs-lookup"><span data-stu-id="bc48d-134">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="bc48d-135">資源的範例包括虛擬機器和儲存體帳戶。</span><span class="sxs-lookup"><span data-stu-id="bc48d-135">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="bc48d-136">資源發出計量：計量是資源耗用量的度量，一個資源可能會發出多個計量的使用量。</span><span class="sxs-lookup"><span data-stu-id="bc48d-136">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="bc48d-137">計量是以 ProductID、SKUID 和 AvailabilityID 識別。</span><span class="sxs-lookup"><span data-stu-id="bc48d-137">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="bc48d-138">訂用帳戶資源群組和計量的階層</span><span class="sxs-lookup"><span data-stu-id="bc48d-138">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="bc48d-139">**Azure 帳戶 (租用戶)**</span><span class="sxs-lookup"><span data-stu-id="bc48d-139">**Azure account (tenant)**</span></span>

- <span data-ttu-id="bc48d-140">訂用帳戶 A</span><span class="sxs-lookup"><span data-stu-id="bc48d-140">Subscription A</span></span>
    - <span data-ttu-id="bc48d-141">資源群組 1</span><span class="sxs-lookup"><span data-stu-id="bc48d-141">ResourceGroup 1</span></span>
        - <span data-ttu-id="bc48d-142">虛擬機器 (資源)</span><span class="sxs-lookup"><span data-stu-id="bc48d-142">Virtual machine (resource)</span></span>
            - <span data-ttu-id="bc48d-143">計算計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-143">Compute meter</span></span>
        - <span data-ttu-id="bc48d-144">虛擬網路 (資源)</span><span class="sxs-lookup"><span data-stu-id="bc48d-144">Virtual network (resource)</span></span>
            - <span data-ttu-id="bc48d-145">沒有計費計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-145">No billing meter</span></span>

    - <span data-ttu-id="bc48d-146">資源群組 2</span><span class="sxs-lookup"><span data-stu-id="bc48d-146">ResourceGroup 2</span></span>
        - <span data-ttu-id="bc48d-147">虛擬機器 (資源)</span><span class="sxs-lookup"><span data-stu-id="bc48d-147">Virtual machine (resource)</span></span>
            - <span data-ttu-id="bc48d-148">電腦計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-148">Computer meter</span></span>
        - <span data-ttu-id="bc48d-149">進階 SSD 受控磁碟 (資源)</span><span class="sxs-lookup"><span data-stu-id="bc48d-149">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="bc48d-150">儲存體容量計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-150">Storage capacity meter</span></span>
            - <span data-ttu-id="bc48d-151">儲存體作業計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-151">Storage operations meter</span></span>

- <span data-ttu-id="bc48d-152">訂用帳戶 B - 資源群組 1 - Azure SQL (資源) - DTU 計量 - VPN 閘道 (資源) - VPN 閘道計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-152">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="bc48d-153">資源群組 2</span><span class="sxs-lookup"><span data-stu-id="bc48d-153">ResourceGroup 2</span></span>
        - <span data-ttu-id="bc48d-154">虛擬網路介面 (資源)</span><span class="sxs-lookup"><span data-stu-id="bc48d-154">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="bc48d-155">沒有計費計量</span><span class="sxs-lookup"><span data-stu-id="bc48d-155">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="bc48d-156">讀取發票</span><span class="sxs-lookup"><span data-stu-id="bc48d-156">Read the invoice</span></span>

1. <span data-ttu-id="bc48d-157">發票在每個月的第八天之後才可取得。</span><span class="sxs-lookup"><span data-stu-id="bc48d-157">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="bc48d-158">合作夥伴有 60 天的時間匯款。</span><span class="sxs-lookup"><span data-stu-id="bc48d-158">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="bc48d-159">計費期間會涵蓋指定的行事曆月份，例如，10/1-10/31。</span><span class="sxs-lookup"><span data-stu-id="bc48d-159">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="bc48d-160">費用是調整淨額 (金額是「受控服務的合作夥伴所獲得信用點數」淨額)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-160">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="bc48d-161">如需其他計費詳細資料，請參閱發票對帳檔案和每日評等使用量檔案。</span><span class="sxs-lookup"><span data-stu-id="bc48d-161">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

![發票](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="bc48d-163">讀取發票對帳檔案</span><span class="sxs-lookup"><span data-stu-id="bc48d-163">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="bc48d-164">在對帳檔案中，每個 Azure 方案和計量組合最多可以有兩個計費行。</span><span class="sxs-lookup"><span data-stu-id="bc48d-164">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="bc48d-165">如果計量符合整個行事曆月份任何類型折扣或信用點數的資格 (例如階層折扣或受控服務的合作夥伴所獲得信用點數)，則對帳檔案只會包含一個計費行。</span><span class="sxs-lookup"><span data-stu-id="bc48d-165">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="bc48d-166">**PriceAdjusmentDescription** 資料行會參考折扣或獲得的信用點數。</span><span class="sxs-lookup"><span data-stu-id="bc48d-166">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="bc48d-167">如果沒有符合折扣或合作夥伴所獲得信用點數的特定計量資源，則對帳檔案只會包含一個計費行，而有效單價會是零售價格 (這就是單價)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-167">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="bc48d-168">如果計量或任何發出該計量的資源符合部分月份**受控服務的合作夥伴所獲得信用點數**的資格，則對帳檔案會包含兩個計費行。</span><span class="sxs-lookup"><span data-stu-id="bc48d-168">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="bc48d-169">一行代表計量合格的天數，而第二行則代表計量不合格的天數。</span><span class="sxs-lookup"><span data-stu-id="bc48d-169">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span> 

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="bc48d-170">讀取每日使用量檔案</span><span class="sxs-lookup"><span data-stu-id="bc48d-170">Read the daily usage file</span></span>

- <span data-ttu-id="bc48d-171">Azure 方案下的訂用帳戶計量會進行分級，並以每天為基礎進行累計。</span><span class="sxs-lookup"><span data-stu-id="bc48d-171">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span> 

- <span data-ttu-id="bc48d-172">**受控服務的合作夥伴所獲得信用點數**是以每天為基礎進行判斷和套用。</span><span class="sxs-lookup"><span data-stu-id="bc48d-172">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="bc48d-173">每個訂用帳戶計量都會有一個資料列，用於月份中每天的使用量。</span><span class="sxs-lookup"><span data-stu-id="bc48d-173">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="bc48d-174">在下列範例中：</span><span class="sxs-lookup"><span data-stu-id="bc48d-174">In the example below:</span></span>

  - <span data-ttu-id="bc48d-175">7/1 - 7/3 的計量符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-175">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="bc48d-176">7/4 - 7/7 的計量不符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-176">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="bc48d-177">7/8 - 7/31 的計量符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-177">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="bc48d-179">以客戶貨幣表示的發票</span><span class="sxs-lookup"><span data-stu-id="bc48d-179">Invoice in customer currency</span></span> 

<span data-ttu-id="bc48d-180">透過 Azure 方案的 Azure 服務會以美元計價，並以客戶國家/地區指派貨幣來計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-180">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="bc48d-181">如果計費貨幣不是美元，則使用的外幣匯率 (FX) 費率會顯示在發票的最後一頁。</span><span class="sxs-lookup"><span data-stu-id="bc48d-181">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="bc48d-182">FX 費率是每月決定，並套用至下列發票。</span><span class="sxs-lookup"><span data-stu-id="bc48d-182">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="bc48d-183">如需國家/地區貨幣的完整清單，請參閱[新的商務供應項目國家/地區可用性和客戶貨幣對照表](https://go.microsoft.com/fwlink/?linkid=2112354)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-183">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span> 

<span data-ttu-id="bc48d-184">Microsoft 將使用 Thomson Reuters，來判斷用來決定定價貨幣至計費貨幣轉換的 FX 費率。</span><span class="sxs-lookup"><span data-stu-id="bc48d-184">Microsoft will use Thomson Reuters to determine the FX rates used to determine pricing currency to billing currency conversion.</span></span> <span data-ttu-id="bc48d-185">FX 費率會重新整理，並在其套用當月第一天的前一天可供使用。</span><span class="sxs-lookup"><span data-stu-id="bc48d-185">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

<span data-ttu-id="bc48d-186">**範例**：服務期間 8 月 1 日 - 8 月 31 日的使用費用，會使用在 7 月 31 日發佈的 FX 費率來計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-186">**Example**:  Usage charges for the service period August 1 - August 31 will be billed using the FX rate published on July 31.</span></span> <span data-ttu-id="bc48d-187">這些費用會出現在 9 月發票上，而 FX 費率會在發票的最後一頁上註明。</span><span class="sxs-lookup"><span data-stu-id="bc48d-187">These charges will appear on the September invoice and the FX rate will be noted on the last page of the invoice.</span></span> 

 
## <a name="azure-reservations"></a><span data-ttu-id="bc48d-188">Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="bc48d-188">Azure reservations</span></span> 

<span data-ttu-id="bc48d-189">如果透過 Azure 方案購買 [Azure Reservations](https://docs.microsoft.com/partner-center/azure-reservations)，一開始就只能在合作夥伴中心選擇一次性計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-189">If purchasing [Azure reservations](https://docs.microsoft.com/partner-center/azure-reservations) through an Azure plan, initially,  it will only be possible to choose one-time billing in Partner Center.</span></span> <span data-ttu-id="bc48d-190">在 Azure 入口網站上可以使用每月計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-190">Monthly billing is available on the Azure portal.</span></span> <span data-ttu-id="bc48d-191">合作夥伴中心將於日後提供每月計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-191">Monthly billing will be available in Partner Center at a later date.</span></span> 

## <a name="azure-spending"></a><span data-ttu-id="bc48d-192">Azure 費用</span><span class="sxs-lookup"><span data-stu-id="bc48d-192">Azure spending</span></span> 

<span data-ttu-id="bc48d-193">現有的 Azure 消費經驗已更新，可支援合作夥伴中心內的新 Azure 方案計費。</span><span class="sxs-lookup"><span data-stu-id="bc48d-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="bc48d-194">這讓合作夥伴可以：</span><span class="sxs-lookup"><span data-stu-id="bc48d-194">This enables partners to:</span></span>

- <span data-ttu-id="bc48d-195">查看、管理及接收針對客戶層級設定的預算警示</span><span class="sxs-lookup"><span data-stu-id="bc48d-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="bc48d-196">查看 Azure 方案中的預估支出總計 (依資源和計量層級細分)</span><span class="sxs-lookup"><span data-stu-id="bc48d-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="bc48d-197">因為透過 Azure 方案的 Azure 服務計費模式是後付款使用方式，所以若要避免帳單超出預期，合作夥伴可以套用每月預算，並追蹤使用量的百分比。</span><span class="sxs-lookup"><span data-stu-id="bc48d-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="bc48d-198">預算可以一次套用至一個客戶或多個客戶。</span><span class="sxs-lookup"><span data-stu-id="bc48d-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

![Azure 費用](images/azure/azurespend.png)

<span data-ttu-id="bc48d-200">**詳細資訊**</span><span class="sxs-lookup"><span data-stu-id="bc48d-200">**For more information**</span></span>

-  <span data-ttu-id="bc48d-201">合作夥伴所獲得信用點數 (PEC) 的計算方式，位於可透過合作夥伴中心[儀表板](https://partner.microsoft.com/en-us/dashboard/)取得的價目表 (需要登入)。</span><span class="sxs-lookup"><span data-stu-id="bc48d-201">How the partner earned credit (PEC) is calculated is located on the price list available through your Partner Center [dashboard](https://partner.microsoft.com/en-us/dashboard/) (sign in required).</span></span> 
   
-  [<span data-ttu-id="bc48d-202">購買 Azure 方案</span><span class="sxs-lookup"><span data-stu-id="bc48d-202">Purchase the Azure plan</span></span>](purchase-azure-plan.md)

-  [<span data-ttu-id="bc48d-203">CSP 中新商務體驗的價目表</span><span class="sxs-lookup"><span data-stu-id="bc48d-203">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)
