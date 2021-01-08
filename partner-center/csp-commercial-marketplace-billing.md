---
title: 商業 marketplace 產品的帳單
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心中從商用 marketplace 購買 ISV SaaS 產品或訂用帳戶的計費方式。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10592c7f8a3b1f075bc726161603859552b29961
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979527"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a><span data-ttu-id="4637c-103">合作夥伴中心中的商業 marketplace 產品和訂閱帳單</span><span class="sxs-lookup"><span data-stu-id="4637c-103">Billing for commercial marketplace products and subscriptions in Partner Center</span></span>


<span data-ttu-id="4637c-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="4637c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4637c-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="4637c-105">Global admin</span></span>
- <span data-ttu-id="4637c-106">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="4637c-106">Billing admin</span></span>

<span data-ttu-id="4637c-107">作為 CSP 方案中的合作夥伴，您可以使用合作夥伴中心，從商業市集中的 ISV 發行者購買以授權為基礎的 SaaS 產品。</span><span class="sxs-lookup"><span data-stu-id="4637c-107">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="4637c-108">這麼做之後，您就可以存取這些購買類型的帳單。</span><span class="sxs-lookup"><span data-stu-id="4637c-108">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="4637c-109">計費週期會在行事曆月份的第一天開始，並于日曆月份的最後一天結束。</span><span class="sxs-lookup"><span data-stu-id="4637c-109">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="4637c-110">發票會在下個月的第8天提供使用。</span><span class="sxs-lookup"><span data-stu-id="4637c-110">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="4637c-111">您可以從合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/) 或使用 [合作夥伴中心 api](/partner-center/develop/)存取發票。</span><span class="sxs-lookup"><span data-stu-id="4637c-111">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](/partner-center/develop/).</span></span>

<span data-ttu-id="4637c-112">CSP 方案中的合作夥伴會在購買這些產品時，向客戶購買的 ISV 商用 marketplace 解決方案計費，方法是使用客戶先前購買的 Azure 租使用者) 合作夥伴中心或 Azure 入口網站 (。</span><span class="sxs-lookup"><span data-stu-id="4637c-112">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="4637c-113">如果客戶使用自己的 Azure AD 租使用者 (而不是從 CSP 方案) 中的合作夥伴購買，客戶也可以選擇直接從 ([Microsoft AppSource](https://appsource.microsoft.com/) 或 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) 購買自己的 ISV SaaS 解決方案。</span><span class="sxs-lookup"><span data-stu-id="4637c-113">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="4637c-114">如果有，則會直接從 Microsoft 收到自己的帳單。</span><span class="sxs-lookup"><span data-stu-id="4637c-114">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="4637c-115">同樣地，如果 CSP 方案中的合作夥伴將 Azure 訂用帳戶或新的 Azure 方案銷售給客戶，並將該租使用者的角色型存取權授與客戶 (或間接轉銷商) 該租使用者的以 [角色為基礎的存取權](/azure/role-based-access-control/built-in-roles) (將任何角色指派 **給) 客戶** (，而不需事先核准或向 CSP 合作夥伴提出通知。</span><span class="sxs-lookup"><span data-stu-id="4637c-115">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="4637c-116">在這些情況下，Microsoft 不會直接通知 CSP 方案中的合作夥伴購買客戶的情況。</span><span class="sxs-lookup"><span data-stu-id="4637c-116">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="4637c-117">不過，Microsoft 提供了選用的 [Azure 監視器](/azure/azure-monitor/platform/alerts-activity-log) 機制，可讓您用來設定 Azure 訂用帳戶上的活動警示或通知。</span><span class="sxs-lookup"><span data-stu-id="4637c-117">However, Microsoft does offer an optional [Azure Monitor](/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="4637c-118">存取商用 marketplace 產品的帳單資訊</span><span class="sxs-lookup"><span data-stu-id="4637c-118">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="4637c-119">貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。</span><span class="sxs-lookup"><span data-stu-id="4637c-119">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="4637c-120">若要存取最新的發票和對帳檔案以進行商業 marketplace 產品購買：</span><span class="sxs-lookup"><span data-stu-id="4637c-120">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="4637c-121">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="4637c-121">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="4637c-122">從 [合作夥伴中心] 功能表中，選取 [計費]。</span><span class="sxs-lookup"><span data-stu-id="4637c-122">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="4637c-123">您會在 [帳單] 頁面頂端看到兩個索引標籤： **週期性** 和 **週期性和一次性購買**。</span><span class="sxs-lookup"><span data-stu-id="4637c-123">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="4637c-124">每個索引標籤可讓您存取不同 marketplace 產品的發票和對帳 (偵察) 檔案：</span><span class="sxs-lookup"><span data-stu-id="4637c-124">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="4637c-125">**週期性** 索引標籤：顯示與 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro 和 Microsoft Azure 相關之訂閱的發票和對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="4637c-125">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="4637c-126">**週期性和單次購買** 索引標籤：顯示 azure 方案、azure 保留、軟體和商用 marketplace 產品的發票和對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="4637c-126">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="4637c-127">選取 [ **週期性和一次性購買** ] 索引標籤。如果您以不同的貨幣購買客戶的訂用帳戶，您會看到每個貨幣的索引標籤。</span><span class="sxs-lookup"><span data-stu-id="4637c-127">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="4637c-128">您可以執行下列工作： om 這個頁面：</span><span class="sxs-lookup"><span data-stu-id="4637c-128">You can do a few things fr:om this page:</span></span>

    - <span data-ttu-id="4637c-129">若要查看最新的發票和對帳檔案，請選取 **發票** 或 **對帳** 檔案。</span><span class="sxs-lookup"><span data-stu-id="4637c-129">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="4637c-130"> (如果您想要的話，也可以使用 [合作夥伴中心 api](/partner-center/develop/)來存取最新的發票和偵察檔案資料。</span><span class="sxs-lookup"><span data-stu-id="4637c-130">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](/partner-center/develop/).</span></span>

    - <span data-ttu-id="4637c-131">若要查看先前的發票和偵察檔，請展開下方的 **計費記錄** 資料列。</span><span class="sxs-lookup"><span data-stu-id="4637c-131">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="4637c-132">若要根據最新的帳戶活動隨時檢查估計的帳戶餘額或帳單，請選取 [ **估價** ] 標題下的連結。</span><span class="sxs-lookup"><span data-stu-id="4637c-132">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="4637c-133">當我們在每個月的第8天張貼帳單時，會包含稅金及任何其他適用的費用和信用額度。</span><span class="sxs-lookup"><span data-stu-id="4637c-133">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="4637c-134">這表示最終到期金額可能與您在計費期間所看到的數量不同。</span><span class="sxs-lookup"><span data-stu-id="4637c-134">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="4637c-135">深入瞭解商用 marketplace 產品的發票和偵察檔案</span><span class="sxs-lookup"><span data-stu-id="4637c-135">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="4637c-136">本節針對從協力廠商 ISV 發行者購買給客戶的商業 marketplace SaaS 訂用帳戶，提供發票和對帳檔案的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="4637c-136">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="4637c-137">當您從 [合作夥伴中心] 功能表的 [**計費**] 選項中選取 [**週期性和一次性購買**] 時，您可以存取發票和對帳檔案，以取得與 Microsoft (第一方) 和 ISV (協力廠商) 購買相關的費用。</span><span class="sxs-lookup"><span data-stu-id="4637c-137">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="4637c-138">這些購買專案可能與下列專案相關：</span><span class="sxs-lookup"><span data-stu-id="4637c-138">These purchases may be associated with:</span></span>

- <span data-ttu-id="4637c-139">從 Microsoft 或 ISV 發行者 (的 SaaS 訂閱) </span><span class="sxs-lookup"><span data-stu-id="4637c-139">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="4637c-140">Azure 方案</span><span class="sxs-lookup"><span data-stu-id="4637c-140">Azure plan</span></span>

- <span data-ttu-id="4637c-141">Azure 保留</span><span class="sxs-lookup"><span data-stu-id="4637c-141">Azure reservations</span></span>

- <span data-ttu-id="4637c-142">其他以訂用帳戶為基礎的軟體 (從 Microsoft 或 ISV 發行者) </span><span class="sxs-lookup"><span data-stu-id="4637c-142">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="4637c-143">這些購買的範例可能包括 SUSE Linux 軟體 (軟體訂用帳戶) 或 Azure ISV SaaS 產品訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="4637c-143">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="4637c-144">如需有關如何讀取發票和偵察檔案的詳細資訊，請參閱 [帳單總覽](billing.md)。</span><span class="sxs-lookup"><span data-stu-id="4637c-144">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="4637c-145">讀取發票的秘訣</span><span class="sxs-lookup"><span data-stu-id="4637c-145">Tips on reading your invoice</span></span>

<span data-ttu-id="4637c-146">當您從協力廠商 ISV 發行者購買以授權為基礎的 SaaS 產品時，您只會看到發票上的授權費用費用。</span><span class="sxs-lookup"><span data-stu-id="4637c-146">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="4637c-147">即使 ISV 的 SaaS 產品使用 (或取用) 基礎的 Azure 基礎結構資源，也是如此。</span><span class="sxs-lookup"><span data-stu-id="4637c-147">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="4637c-148">這是因為您客戶對 ISV SaaS 產品的 Azure 基礎結構使用費用，會直接向 ISV 收費。</span><span class="sxs-lookup"><span data-stu-id="4637c-148">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="4637c-149"> (Isv 會在其各自的 Azure 使用量每日分級的發票對帳檔案中看到相關聯的 Azure 使用量費用。 ) </span><span class="sxs-lookup"><span data-stu-id="4637c-149">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="4637c-150">您的發票將包含數個頁面：</span><span class="sxs-lookup"><span data-stu-id="4637c-150">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="4637c-151">**發票的第1頁：** 包含 CSP 方案夥伴帳單詳細資料的摘要總覽。</span><span class="sxs-lookup"><span data-stu-id="4637c-151">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="4637c-152">這包括計費週期的費用摘要、發票號碼、付款條款 (淨60天) ，以及透過網路付款或依檢查付款的計費方法。</span><span class="sxs-lookup"><span data-stu-id="4637c-152">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="4637c-153">**第2頁 (以及發票的任何後續頁面) ：** 針對第一方的 Microsoft 購買和協力廠商 ISV (以授權為基礎的) 從商用 marketplace 購買的費用詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4637c-153">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="4637c-154">您可以根據每個產品名稱底下的 **發行者** 行，識別 ISV 授權型購買。</span><span class="sxs-lookup"><span data-stu-id="4637c-154">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="4637c-155">相關聯的對帳檔案會針對特定發票費用提供更多帳單詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4637c-155">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="4637c-156">**發票的最終頁面：** 如果您向 ISV 收取以授權為基礎的 marketplace 產品的費用，此最終頁面將會顯示 ISV 發行者的名稱和位址的更多詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4637c-156">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="4637c-157">讀取對帳檔案的秘訣</span><span class="sxs-lookup"><span data-stu-id="4637c-157">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="4637c-158">**週期性和單次採購** 對帳檔案包含數個數據行，其中包含對應至發票費用的額外詳細資料。</span><span class="sxs-lookup"><span data-stu-id="4637c-158">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="4637c-159">[ **PublisherName** ] 欄會顯示購買是來自 Microsoft 或協力廠商 ISV 發行者。</span><span class="sxs-lookup"><span data-stu-id="4637c-159">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="4637c-160">對帳檔案中的某些費用可能會以 $0 的成本顯示。</span><span class="sxs-lookup"><span data-stu-id="4637c-160">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="4637c-161">這可能是因為 ISV 「免費試用」供應專案， (通常是30或60天) 或自備授權供應專案。</span><span class="sxs-lookup"><span data-stu-id="4637c-161">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="4637c-162">在免費試用 ISV 提供的案例中：</span><span class="sxs-lookup"><span data-stu-id="4637c-162">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="4637c-163">免費試用期涵蓋了 ISV 以授權為基礎的 SaaS 產品在這段時間的成本。</span><span class="sxs-lookup"><span data-stu-id="4637c-163">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="4637c-164">您也不需要支付該 SaaS 產品的相關 Azure 基礎結構使用費用。</span><span class="sxs-lookup"><span data-stu-id="4637c-164">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="4637c-165">但是，如果您使用以使用量為基礎的 ISV 供應專案，則免費試用版不包含基礎 Azure 基礎結構使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="4637c-165">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="4637c-166">在此情況下，Azure 基礎結構使用量費用會出現在個別的 Azure 對帳檔案中。</span><span class="sxs-lookup"><span data-stu-id="4637c-166">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="4637c-167">當您為客戶購買並部署 ISV 的免費試用版產品時，ISV 發行者會自動在免費試用版中註冊客戶。</span><span class="sxs-lookup"><span data-stu-id="4637c-167">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="4637c-168">免費試用期間會在 ISV 發行者所定義的期間後自動結束。</span><span class="sxs-lookup"><span data-stu-id="4637c-168">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="4637c-169">在該期間結束之後，將會向客戶收取費用。</span><span class="sxs-lookup"><span data-stu-id="4637c-169">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="4637c-170">這表示，對帳檔案可能會針對符合試用資格的產品顯示兩個數據列：一個會追蹤試用期間，另一個則會追蹤付費供應專案 (這會顯示 $0，直到試用期結束) 為止。</span><span class="sxs-lookup"><span data-stu-id="4637c-170">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="4637c-171">試用期結束後，顯示付費供應專案的資料列就會開始顯示費用。</span><span class="sxs-lookup"><span data-stu-id="4637c-171">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="4637c-172">如需每個資料行代表什麼的詳細資訊，請參閱 [使用您的對帳](use-the-reconciliation-files.md)檔案。</span><span class="sxs-lookup"><span data-stu-id="4637c-172">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="4637c-173">另請參閱 [合作夥伴中心中的計費類型](billing-different-types.md)</span><span class="sxs-lookup"><span data-stu-id="4637c-173">See also [Types of billing in Partner Center](billing-different-types.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="4637c-174">後續步驟</span><span class="sxs-lookup"><span data-stu-id="4637c-174">Next steps</span></span>

- [<span data-ttu-id="4637c-175">管理客戶的商業 marketplace 產品</span><span class="sxs-lookup"><span data-stu-id="4637c-175">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="4637c-176">瞭解商業 marketplace 產品的支援</span><span class="sxs-lookup"><span data-stu-id="4637c-176">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)