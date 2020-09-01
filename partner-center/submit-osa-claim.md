---
title: 透過 CPOR 模型建立客戶關聯
ms.topic: article
ms.date: 08/31/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 透過 CPOR 建立客戶關聯， (宣稱記錄) 模型的夥伴。 協助管理 Microsoft 365 和 Dynamics 365 客戶的銷售、使用、& 獎勵。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d5b14759803beb73cc970bf5fb96747048b8bdc1
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220366"
---
# <a name="create-a-customer-association-via-the-cpor-model--use-for-microsoft-365-and-dynamics-365-customers"></a><span data-ttu-id="62bb3-104">透過 CPOR 模型建立客戶關聯–用於 Microsoft 365 與 Dynamics 365 客戶</span><span class="sxs-lookup"><span data-stu-id="62bb3-104">Create a customer association via the CPOR model – use for Microsoft 365 and Dynamics 365 customers</span></span>

<span data-ttu-id="62bb3-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="62bb3-105">**Applies to**</span></span>

- <span data-ttu-id="62bb3-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="62bb3-106">Partner Center</span></span>

<span data-ttu-id="62bb3-107">**適當的角色：**</span><span class="sxs-lookup"><span data-stu-id="62bb3-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="62bb3-108">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="62bb3-108">Incentives admin</span></span>

<span data-ttu-id="62bb3-109">從2019年10月1日開始，Microsoft 會開始使用 (CPOR) 模型的宣稱合作夥伴來管理您與 Microsoft 365 和 Dynamics 365 客戶的關聯與 Dynamics 客戶有關線上服務諮詢 (OSA) 銷售、線上服務使用 (OSU) -Microsoft 365 和 OSU 商務應用程式獎勵。</span><span class="sxs-lookup"><span data-stu-id="62bb3-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="62bb3-110">客戶關聯 (CPOR) 宣告僅適用于線上服務諮詢 (OSA) 銷售、線上服務使用 (OSU) -Microsoft 365 和 OSU 商務應用程式獎勵計畫。</span><span class="sxs-lookup"><span data-stu-id="62bb3-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="62bb3-111">如果您要為另一個程式（例如雲端解決方案提供者、受管理的轉銷商、託管或表面）提交共同作業索賠，請參閱此處所述的共同作業宣告程式。</span><span class="sxs-lookup"><span data-stu-id="62bb3-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="62bb3-112">當您提交宣告時，Microsoft 會進行驗證。</span><span class="sxs-lookup"><span data-stu-id="62bb3-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="62bb3-113">我們可能會在此時要求您提供更多資訊。</span><span class="sxs-lookup"><span data-stu-id="62bb3-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="62bb3-114">我們也會通知客戶您的關聯要求。</span><span class="sxs-lookup"><span data-stu-id="62bb3-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="62bb3-115">客戶有五個工作天可退出宣告。如果未退出宣告，與此特定租使用者和工作負載的關聯將會是官方的。</span><span class="sxs-lookup"><span data-stu-id="62bb3-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="62bb3-116">至此，您將可存取客戶的使用量資料。</span><span class="sxs-lookup"><span data-stu-id="62bb3-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="62bb3-117">您將需要下列資訊才能完成宣告：</span><span class="sxs-lookup"><span data-stu-id="62bb3-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="62bb3-118">進行宣告之實體的**MPN 識別碼**</span><span class="sxs-lookup"><span data-stu-id="62bb3-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="62bb3-119">客戶的**功能變數名稱**[找到此](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="62bb3-119">Customer's **domain name** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="62bb3-120">客戶的**目錄識別碼**或**租使用者識別碼**[尋找此](find-domain-name.md)</span><span class="sxs-lookup"><span data-stu-id="62bb3-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-domain-name.md)</span></span>

- <span data-ttu-id="62bb3-121">**解決方案區域**，例如 Business Applications 或 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="62bb3-121">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="62bb3-122">您已執行的 **活動** ，以及您想要進行的宣告類型，例如售前、使用量或收入關聯</span><span class="sxs-lookup"><span data-stu-id="62bb3-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="62bb3-123">您客戶的 **連絡人名稱**、標題和電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="62bb3-123">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="62bb3-124">針對 Dynamics 365，您也需要提供客戶的 **技術連絡人** 名稱、標題和電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="62bb3-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="62bb3-125">您自己公司的 **連絡人名稱** 和電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="62bb3-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="62bb3-126">您將建立此宣告的**名稱**</span><span class="sxs-lookup"><span data-stu-id="62bb3-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="62bb3-127">\*\*產品 (s) \*\*或工作負載 () 您所宣稱的</span><span class="sxs-lookup"><span data-stu-id="62bb3-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="62bb3-128">\*\*執行證明 (PoE) \*\*，例如客戶所簽署的工作說明。</span><span class="sxs-lookup"><span data-stu-id="62bb3-128">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="62bb3-129">您也可以下載 PoE 範本以供使用。</span><span class="sxs-lookup"><span data-stu-id="62bb3-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="62bb3-130">適用于僅索取收入關聯的合作夥伴： **Dynamics 解決方案賣方名稱**、 **客戶名稱**，以及 **ISV 產品/解決方案的名稱**。</span><span class="sxs-lookup"><span data-stu-id="62bb3-130">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="62bb3-131">您也應該瞭解下列幾點：</span><span class="sxs-lookup"><span data-stu-id="62bb3-131">You should also understand the following points:</span></span>

- <span data-ttu-id="62bb3-132">如果您有現有的 Microsoft 365 客戶，您必須使用此程式，重新與想要繼續獲得 OSU 獎勵的客戶建立關聯。</span><span class="sxs-lookup"><span data-stu-id="62bb3-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="62bb3-133">如果您現有與 Dynamics 365 或 Power BI 客戶的關聯，這些關聯將會維持有效，直到其訂閱到期為止。</span><span class="sxs-lookup"><span data-stu-id="62bb3-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="62bb3-134">客戶可以有多個夥伴，但 OSU Microsoft 365) 的每個工作負載 (或針對 OSA 銷售和 OSU Business Applications 的訂用帳戶 (只能與一個合作夥伴相關聯。</span><span class="sxs-lookup"><span data-stu-id="62bb3-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="62bb3-135">建立客戶關聯</span><span class="sxs-lookup"><span data-stu-id="62bb3-135">Create a customer association</span></span>

1. <span data-ttu-id="62bb3-136">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="62bb3-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="62bb3-137">選取 [**獎勵**] 索引標籤，選取 [總覽]，然後選取 **[\*\*\*\*客戶關聯**]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-137">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="62bb3-138">在 [客戶關聯] 頁面的頂端，選取 [ **+ 客戶關聯**]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-138">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="62bb3-139">選取要與客戶相關聯合作夥伴位置的 **MPN 識別碼**，然後新增客戶的網域名稱和目錄識別碼。</span><span class="sxs-lookup"><span data-stu-id="62bb3-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="62bb3-140">尋找</span><span class="sxs-lookup"><span data-stu-id="62bb3-140">Find this</span></span>](find-domain-name.md)

5. <span data-ttu-id="62bb3-141">選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-141">Select **Continue**.</span></span>

6. <span data-ttu-id="62bb3-142">選取 **解決方案區域** 和 **活動**。</span><span class="sxs-lookup"><span data-stu-id="62bb3-142">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="62bb3-143">如果您選取 [Business Applications，請選取 [ **使用量] 和/或 [售前**] 或 [ **收入關聯**]，然後選取 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-143">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="62bb3-144">如果您選取 [收益關聯]，系統會提示您輸入與下列內容稍有不同的資訊。</span><span class="sxs-lookup"><span data-stu-id="62bb3-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="62bb3-145">在 [ **關聯客戶** ] 頁面上輸入適當的資訊，然後選取 [ **建立**宣告]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="62bb3-146">選取與此客戶關聯相關聯的產品 () ，然後選取 [ **繼續**]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-146">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="62bb3-147">完成客戶連絡人資訊和貴公司的連絡人資訊。</span><span class="sxs-lookup"><span data-stu-id="62bb3-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="62bb3-148">所有欄位皆為必填項目。</span><span class="sxs-lookup"><span data-stu-id="62bb3-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="62bb3-149">如果您的產品是 Dynamics 365，而您選擇的產品有此特定客戶的多個訂用帳戶，您也必須輸入訂用帳戶識別碼。</span><span class="sxs-lookup"><span data-stu-id="62bb3-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="62bb3-150"> (PoE) 提供您的執行證明。</span><span class="sxs-lookup"><span data-stu-id="62bb3-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="62bb3-151">您可以將其拖曳到方塊中，瀏覽至您自己的支援文件，或選取 [下載範本] 以使用範本。</span><span class="sxs-lookup"><span data-stu-id="62bb3-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="62bb3-152">如有需要，請新增並儲存註解，然後選取 [提交申請]。</span><span class="sxs-lookup"><span data-stu-id="62bb3-152">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="62bb3-153">我們會傳送一封電子郵件給客戶，要求核准您的客戶關係。</span><span class="sxs-lookup"><span data-stu-id="62bb3-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="62bb3-154">當您提交客戶關聯之後，就無法加以編輯。</span><span class="sxs-lookup"><span data-stu-id="62bb3-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="62bb3-155">您的客戶關聯狀態會出現在**狀態**欄位中。</span><span class="sxs-lookup"><span data-stu-id="62bb3-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="62bb3-156">選取 [歷程記錄] 以檢視客戶關聯的歷程記錄。</span><span class="sxs-lookup"><span data-stu-id="62bb3-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="62bb3-157">後續步驟</span><span class="sxs-lookup"><span data-stu-id="62bb3-157">Next steps</span></span>

- [<span data-ttu-id="62bb3-158">管理客戶關聯</span><span class="sxs-lookup"><span data-stu-id="62bb3-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)