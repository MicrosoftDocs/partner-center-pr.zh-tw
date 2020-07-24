---
title: 商業 marketplace 產品的帳單
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解在合作夥伴中心內從商業 marketplace 購買客戶的 ISV SaaS 產品或訂用帳戶的計費方式。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5c506e1f3dd5e1ffcac1d7017687b1b36718745
ms.sourcegitcommit: 37562b0e29ab921b6b454bb9801376f1feedb715
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "86943472"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a><span data-ttu-id="7c1f5-103">合作夥伴中心內的商業 marketplace 產品和訂用帳戶計費</span><span class="sxs-lookup"><span data-stu-id="7c1f5-103">Billing for commercial marketplace products and subscriptions in Partner Center</span></span>

<span data-ttu-id="7c1f5-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="7c1f5-104">**Applies to**</span></span>

- <span data-ttu-id="7c1f5-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="7c1f5-105">Partner Center</span></span>
- <span data-ttu-id="7c1f5-106">雲端解決方案提供者方案中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="7c1f5-106">Partners in the CSP program</span></span>

<span data-ttu-id="7c1f5-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="7c1f5-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7c1f5-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7c1f5-108">Global admin</span></span>
- <span data-ttu-id="7c1f5-109">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="7c1f5-109">Billing admin</span></span>

<span data-ttu-id="7c1f5-110">身為 CSP 計畫的合作夥伴，您可以使用合作夥伴中心，從商用 marketplace 中的 ISV 發行者購買授權型 SaaS 產品。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-110">As a partner in the CSP program, you can use Partner Center to purchase license-based SaaS products from ISV publishers in the commercial marketplace.</span></span> <span data-ttu-id="7c1f5-111">這麼做之後，您就可以存取這些購買類型的帳單。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-111">After you do so, you can access a bill for these types of purchases.</span></span> <span data-ttu-id="7c1f5-112">計費週期會在日曆月份的第一天開始，並在日曆月份的最後一天結束。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-112">The billing period starts on the first day of the calendar month and ends on the last day of the calendar month.</span></span> <span data-ttu-id="7c1f5-113">在下個月的第8天可取得發票。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-113">Invoices are made available on the 8th day of the following month.</span></span>

<span data-ttu-id="7c1f5-114">您可以從合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)或使用[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/)來存取發票。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-114">You can access invoices from either the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) or by using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="7c1f5-115">CSP 計畫中的合作夥伴會針對客戶購買的 ISV 商業 marketplace 解決方案計費，其方式是從合作夥伴中心或 Azure 入口網站購買這些產品（使用客戶先前的 CSP 購買 Azure 租使用者）。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-115">Partners in the CSP program are billed for ISV commercial marketplace solutions purchased for a customer when they purchase those products from either Partner Center or from the Azure portal (using the customer's prior, CSP-purchased Azure tenant).</span></span>

>[!NOTE]
><span data-ttu-id="7c1f5-116">如果客戶使用自己的 Azure AD 租使用者（而不是從 CSP 方案中的合作夥伴購買），客戶也可以選擇直接從（[Microsoft AppSource](https://appsource.microsoft.com/)或[Azure Marketplace](https://azuremarketplace.microsoft.com/)）購買自己的 ISV SaaS 解決方案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-116">If customers use their own Azure AD tenant (not one purchased from a partner in the CSP program), customers can also choose to purchase their own ISV SaaS solution directly from ([Microsoft AppSource](https://appsource.microsoft.com/) or [Azure Marketplace](https://azuremarketplace.microsoft.com/)).</span></span> <span data-ttu-id="7c1f5-117">如果他們這麼做，他們會直接從 Microsoft 收到自己的帳單。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-117">If they do so, they will receive their own bill directly from Microsoft.</span></span> <span data-ttu-id="7c1f5-118">同樣地，如果 CSP 方案中的合作夥伴將 Azure 訂用帳戶或新的 Azure 方案銷售給客戶，並將該租使用者的[角色型存取權](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)授與客戶（或間接轉銷**商），** 則該客戶（或間接轉銷商）也可以購買商業 marketplace 供應專案，而不需要事先核准或通知給 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-118">Likewise, if a partner in the CSP program sells an Azure subscription or the new Azure plan to the customer and grants the customer (or indirect reseller) [role-based access](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) to that tenant (assigning any role to the customer besides **Reader**), that customer (or indirect reseller) can also purchase commercial marketplace offers without prior approval or notification to the CSP partner.</span></span> <span data-ttu-id="7c1f5-119">在這些情況下，Microsoft 不會直接向 CSP 計畫中的合作夥伴通知其客戶所進行的購買。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-119">In these cases, Microsoft will not directly notify partners in the CSP program about purchases made by their customers.</span></span> <span data-ttu-id="7c1f5-120">不過，Microsoft 會提供選擇性的[Azure 監視器](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)機制，讓您可以用來設定 Azure 訂用帳戶上活動的警示或通知。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-120">However, Microsoft does offer an optional [Azure Monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) mechanism that you can use to set alerts or notifications about activity on an Azure subscription.</span></span>

## <a name="access-billing-information-for-commercial-marketplace-products"></a><span data-ttu-id="7c1f5-121">存取商業 marketplace 產品的帳單資訊</span><span class="sxs-lookup"><span data-stu-id="7c1f5-121">Access billing information for commercial marketplace products</span></span>

<span data-ttu-id="7c1f5-122">貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-122">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span> <span data-ttu-id="7c1f5-123">若要存取商業 marketplace 產品購買的最新發票和對帳檔案：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-123">To access the latest invoice and reconciliation file for commercial marketplace product purchases:</span></span>

1. <span data-ttu-id="7c1f5-124">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-124">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="7c1f5-125">從 [合作夥伴中心] 功能表中，選取 [計費]。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-125">From the Partner Center menu, select **Billing**.</span></span> 

    <span data-ttu-id="7c1f5-126">您會在 [帳單] 頁面頂端看到兩個索引標籤： [**週期性**] 和 [**週期性] 和**[單次購買]。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-126">You will see two tabs at the top of the Billing page: **Recurring** and **Recurring and one-time purchases**.</span></span> <span data-ttu-id="7c1f5-127">每個索引標籤都可讓您存取不同 marketplace 產品的發票和對帳（偵察）檔案：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-127">Each tab lets you access invoice and reconciliation (recon) files for different marketplace products:</span></span>

    - <span data-ttu-id="7c1f5-128">**週期性**索引標籤：顯示與 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro 和 Microsoft Azure 相關之訂閱的發票和對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-128">**Recurring** tab: Shows invoice and reconciliation files for subscriptions related to Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro, and Microsoft Azure.</span></span>

    - <span data-ttu-id="7c1f5-129">**週期性和一次性購買**索引標籤：顯示 azure 方案、azure 保留、軟體和商用 marketplace 產品的發票和對帳檔案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-129">**Recurring and one-time purchases** tab: Shows invoice and reconciliation files for Azure plan, Azure reservations, software and commercial marketplace products.</span></span>
  
3. <span data-ttu-id="7c1f5-130">選取 [**週期性和一次性購買**] 索引標籤。如果您以不同的貨幣購買客戶的訂用帳戶，您會看到每個貨幣的索引標籤。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-130">Select the **Recurring and one-time purchases** tab. If you purchased subscriptions for a customer in a different currency, you will see a tab for each currency.</span></span> <span data-ttu-id="7c1f5-131">您可以進行一些 fr： om 這個頁面：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-131">You can do a few things fr:om this page:</span></span>

    - <span data-ttu-id="7c1f5-132">若要查看最新的發票和對帳檔案，請選取 [**發票**或**對帳**檔案]。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-132">To see the latest invoice and reconciliation file, select **Invoice** or **Reconciliation file**.</span></span> <span data-ttu-id="7c1f5-133">（如果您想要的話，也可以使用[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/)來存取最新的發票和偵察檔案資料。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-133">(If you wanted to, you can also access the latest invoice and recon file data using [Partner Center APIs](https://docs.microsoft.com/partner-center/develop/).</span></span>

    - <span data-ttu-id="7c1f5-134">若要查看先前的發票和偵察檔案，請展開下方的 [**帳單記錄**] 列。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-134">To see earlier invoices and recon files, expand the **Billing history** row below.</span></span>

    - <span data-ttu-id="7c1f5-135">若要根據最新的帳戶活動，隨時檢查預估的帳戶餘額或帳單，請選取 [**估價**] 標題下方的連結。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-135">To check your estimated account balance or bill at any time based on the latest account activity, select a link under the **Estimates** heading.</span></span>  

    >[!NOTE]
    > <span data-ttu-id="7c1f5-136">當我們在當月第8天張貼帳單時，將會包含稅金和任何其他適用的費用和信用額度。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-136">When we post your bill on the 8th day of the month, it will include taxes and any other applicable charges and credits.</span></span> <span data-ttu-id="7c1f5-137">這表示最終到期金額可能與您在計費期間所看到的數量不同。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-137">This means the final amount due might differ from what you see during the billing period.</span></span>

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a><span data-ttu-id="7c1f5-138">深入瞭解商業 marketplace 產品的發票和偵察檔</span><span class="sxs-lookup"><span data-stu-id="7c1f5-138">More about invoices and recon files for commercial marketplace products</span></span>

<span data-ttu-id="7c1f5-139">本節針對向協力廠商 ISV 發行者購買的客戶提供的商用 marketplace SaaS 訂閱的發票和對帳檔案的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-139">This section offers more information about invoice and reconciliation files for commercial marketplace SaaS subscriptions purchased for customers from third-party ISV publishers.</span></span>

<span data-ttu-id="7c1f5-140">當您從 [合作夥伴中心] 功能表中的 [**計費**] 選項選取 [**週期性] 和**[單次購買] 時，您會取得發票和對帳檔案的存取權，以取得與 Microsoft （第一方）和 ISV （協力廠商）購買相關的費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-140">When you select **Recurring and one-time purchases** from the **Billing** option in the Partner Center menu, you gain access to invoices and reconciliation files for charges related to both Microsoft (first-party) and ISV (third-party) purchases.</span></span> <span data-ttu-id="7c1f5-141">這些購買專案可能會與下列專案相關聯：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-141">These purchases may be associated with:</span></span>

- <span data-ttu-id="7c1f5-142">SaaS 訂閱（來自 Microsoft 或 ISV 發行者）</span><span class="sxs-lookup"><span data-stu-id="7c1f5-142">SaaS subscriptions (from either Microsoft or ISV publishers)</span></span>

- <span data-ttu-id="7c1f5-143">Azure 方案</span><span class="sxs-lookup"><span data-stu-id="7c1f5-143">Azure plan</span></span>

- <span data-ttu-id="7c1f5-144">Azure 保留</span><span class="sxs-lookup"><span data-stu-id="7c1f5-144">Azure reservations</span></span>

- <span data-ttu-id="7c1f5-145">其他以訂閱為基礎的軟體（來自 Microsoft 或 ISV 發行者）</span><span class="sxs-lookup"><span data-stu-id="7c1f5-145">Other subscription-based software (from either Microsoft or ISV publishers)</span></span>

<span data-ttu-id="7c1f5-146">這些購買的範例可能包括 SUSE Linux 軟體（軟體訂用帳戶）或 Azure ISV SaaS 產品訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-146">Examples of these purchases might include SUSE Linux software (a software subscription) or an Azure ISV SaaS product subscription.</span></span>

>[!NOTE]
> <span data-ttu-id="7c1f5-147">如需有關如何讀取發票和偵察檔的詳細資訊，請參閱[計費總覽](billing.md)。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-147">For more information about how to read invoice and recon files, see also [Billing overview](billing.md).</span></span>

### <a name="tips-on-reading-your-invoice"></a><span data-ttu-id="7c1f5-148">閱讀發票的秘訣</span><span class="sxs-lookup"><span data-stu-id="7c1f5-148">Tips on reading your invoice</span></span>

<span data-ttu-id="7c1f5-149">當您從協力廠商 ISV 發行者購買以授權為基礎的 SaaS 產品時，您只會看到發票上的授權費用費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-149">When you purchase a license-based SaaS product from a third-party ISV publisher, you will only see charges for the license fee on your invoice.</span></span> <span data-ttu-id="7c1f5-150">即使 ISV 的 SaaS 產品使用（或使用）基礎 Azure 基礎結構資源，也是如此。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-150">This is true even when the ISV's SaaS product uses (or consumes) underlying Azure infrastructure resources.</span></span> <span data-ttu-id="7c1f5-151">這是因為 ISV 的 SaaS 產品的客戶 Azure 基礎結構使用量費用，會直接向 ISV 收費。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-151">That is because your customer's Azure infrastructure usage charges for an ISV's SaaS product are billed directly to the ISV.</span></span> <span data-ttu-id="7c1f5-152">（Isv 會在自己的 Azure 使用量每日評分的發票對帳檔案中看到相關聯的 Azure 耗用量費用。）</span><span class="sxs-lookup"><span data-stu-id="7c1f5-152">(ISVs will see associated Azure consumption charges in their own Azure usage daily-rated invoice reconciliation file.)</span></span>

<span data-ttu-id="7c1f5-153">您的發票將包含數個頁面：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-153">Your invoice will contain several pages:</span></span>

- <span data-ttu-id="7c1f5-154">**發票的第1頁：** 包含 CSP 計畫合作夥伴帳單詳細資料的摘要總覽。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-154">**Page 1 of the invoice:** Contains a summary overview of the CSP program partner's billing details.</span></span> <span data-ttu-id="7c1f5-155">這包括計費期間的費用摘要、發票編號、付款條款（Net 60 天），以及按網路或核取的計費付款方法。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-155">This includes a summary of charges for the billing period, an invoice number, payment terms (Net 60 days), and billing payment methods to pay by wire or by check.</span></span>

- <span data-ttu-id="7c1f5-156">**發票的第2頁（以及任何後續頁面）：** 從商用 marketplace 購買第一方的 Microsoft 購買和協力廠商 ISV （以授權為基礎）的費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-156">**Page 2 (and any subsequent pages) of the invoice:** Details charges for both first-party Microsoft purchases and third-party ISV (license-based) purchases from the commercial marketplace.</span></span> <span data-ttu-id="7c1f5-157">您可以根據每個產品名稱底下的**發行者**行，識別以 ISV 授權為基礎的購買專案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-157">You can identify ISV license-based purchases by the **Publisher** line beneath each product name.</span></span> <span data-ttu-id="7c1f5-158">相關聯的對帳檔案會針對特定發票費用提供更多計費詳細資料。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-158">The associated reconciliation file offers more billing details for specific invoice charges.</span></span>

- <span data-ttu-id="7c1f5-159">**發票的最後一頁：** 如果您向 ISV 收取以授權為基礎的 marketplace 產品費用，此最終頁面將會顯示 ISV 發行者名稱和位址的更多詳細資料。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-159">**Final page of the invoice:** If you were charged for license-based marketplace products from an ISV, this final page will display more details about the ISV publisher's name and address.</span></span>

### <a name="tips-on-reading-your-reconciliation-file"></a><span data-ttu-id="7c1f5-160">讀取對帳檔案的秘訣</span><span class="sxs-lookup"><span data-stu-id="7c1f5-160">Tips on reading your reconciliation file</span></span>

<span data-ttu-id="7c1f5-161">**週期性和一次性採購**對帳檔案包含數個數據行，其中含有對應至發票費用的其他詳細資料。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-161">The **Recurring and one-time purchases** reconciliation file contains several columns with additional details that map to the charges in your invoice.</span></span> <span data-ttu-id="7c1f5-162">[ **PublisherName** ] 欄會顯示購買是來自 Microsoft 或協力廠商 ISV 發行者。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-162">The **PublisherName** column shows whether the purchase is from Microsoft or a third-party ISV publisher.</span></span>

<span data-ttu-id="7c1f5-163">您的對帳檔案中的某些費用可能會顯示為 $0 的成本。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-163">Some charges in your reconciliation file may appear with a cost of $0.</span></span> <span data-ttu-id="7c1f5-164">這可能是因為 ISV 「免費試用」供應專案（通常是30或60天）或自備授權供應專案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-164">This may be due to an ISV "free trial" offer (usually 30 or 60 days) or a Bring Your Own License offer.</span></span>

<span data-ttu-id="7c1f5-165">在免費試用 ISV 提供的案例中：</span><span class="sxs-lookup"><span data-stu-id="7c1f5-165">In the case of free trial ISV offers:</span></span>

- <span data-ttu-id="7c1f5-166">免費試用期間涵蓋了 ISV 以授權為基礎的 SaaS 產品在這段時間內的成本。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-166">The free trial period covers the cost of the ISV's license-based SaaS product during that time.</span></span> <span data-ttu-id="7c1f5-167">該 SaaS 產品的相關 Azure 基礎結構使用也不會向您收取費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-167">You will also not be charged for associated Azure infrastructure use of that SaaS product.</span></span>  <span data-ttu-id="7c1f5-168">不過，如果您使用以使用量為基礎的 ISV 供應專案，免費試用不會包含基礎 Azure 基礎結構使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-168">If you are using a usage-based ISV offer, however, the free trial does not include the cost of underlying Azure infrastructure usage.</span></span> <span data-ttu-id="7c1f5-169">在此情況下，Azure 基礎結構使用量費用將會出現在個別的 Azure 對帳檔案中。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-169">In this case, Azure infrastructure usage charges will appear in a separate Azure reconciliation file.</span></span>

- <span data-ttu-id="7c1f5-170">當您為客戶購買及部署 ISV 的免費試用版合格產品時，ISV 發行者會自動在免費試用版中註冊客戶。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-170">When you purchase and deploy an ISV's free trial-eligible product for your customer, the customer is automatically enrolled in the free trial by the ISV publisher.</span></span> <span data-ttu-id="7c1f5-171">免費試用期間會在 ISV 發行者定義的期間之後自動結束。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-171">The free trial period ends automatically after the period defined by the ISV publisher.</span></span> <span data-ttu-id="7c1f5-172">一段期間結束後，就會向客戶收取費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-172">After the period ends, the customer will be charged.</span></span> <span data-ttu-id="7c1f5-173">這表示，對帳檔案可能會顯示兩個適用于試用版產品的資料列：一個追蹤試用期，另一個則追蹤付費供應專案（在試用期結束之前，會顯示 $0 的成本）。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-173">This means the reconciliation file may show two rows for a trial-eligible product: One that tracks the trial period and one that tracks the paid offer (which will display a cost of $0 until after the trial period ends).</span></span> <span data-ttu-id="7c1f5-174">試用期結束後，顯示付費供應專案的資料列就會開始顯示費用。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-174">Once the trial ends, the row showing the paid offer will start to show charges.</span></span> 

<span data-ttu-id="7c1f5-175">如需每個資料行所代表之內容的詳細資訊，請參閱[使用您的對帳](use-the-reconciliation-files.md)檔案。</span><span class="sxs-lookup"><span data-stu-id="7c1f5-175">For more information about what each column represents, see [Use your reconciliation files](use-the-reconciliation-files.md).</span></span> <span data-ttu-id="7c1f5-176">另請參閱[合作夥伴中心的帳單類型](billing-different-types.md)</span><span class="sxs-lookup"><span data-stu-id="7c1f5-176">See also [Types of billing in Partner Center](billing-different-types.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="7c1f5-177">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="7c1f5-177">Next steps</span></span>

- [<span data-ttu-id="7c1f5-178">管理客戶的商業 marketplace 產品</span><span class="sxs-lookup"><span data-stu-id="7c1f5-178">Manage commercial marketplace products for customers</span></span>](csp-commercial-marketplace-manage.md)
- [<span data-ttu-id="7c1f5-179">瞭解商業 marketplace 產品的支援</span><span class="sxs-lookup"><span data-stu-id="7c1f5-179">Learn about support for commercial marketplace products</span></span>](csp-commercial-marketplace-support.md)
