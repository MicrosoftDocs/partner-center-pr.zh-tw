---
title: 在合作夥伴中心建立及管理支出與稅務設定檔
ms.topic: article
ms.date: 06/29/2020
description: 您必須先建立您的付款和稅務設定檔，才能支付獎勵的工作費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: ed8820065c8c009e64419e58fa11758a27f95d7e
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114083"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="234e5-103">合作夥伴中心的支出和稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="234e5-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="234e5-104">適用於︰</span><span class="sxs-lookup"><span data-stu-id="234e5-104">Applies to:</span></span>

- <span data-ttu-id="234e5-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="234e5-105">Partner Center</span></span>

<span data-ttu-id="234e5-106">您必須先將有效的支出和稅務設定檔與計畫和 MPN 的位置產生關聯，才能收到特定 MPN 位置的獎勵計畫款項。</span><span class="sxs-lookup"><span data-stu-id="234e5-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="234e5-107">Microsoft 將使用此支出與稅務設定檔來發出款項。</span><span class="sxs-lookup"><span data-stu-id="234e5-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="234e5-108">視獎勵計畫的規則而定，您可能可以使用電子銀行轉帳或貸記通知單來付款。</span><span class="sxs-lookup"><span data-stu-id="234e5-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="234e5-109">適當的角色：</span><span class="sxs-lookup"><span data-stu-id="234e5-109">Appropriate roles:</span></span>

- <span data-ttu-id="234e5-110">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="234e5-110">Incentives admin</span></span>
- <span data-ttu-id="234e5-111">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="234e5-111">Billing admin</span></span>
- <span data-ttu-id="234e5-112">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="234e5-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="234e5-113">在合作夥伴中心建立及管理支出與稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="234e5-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="234e5-114">下列各節將逐步引導您完成在合作夥伴中心建立及管理付款和稅務設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="234e5-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="234e5-115">您必須是獎勵系統管理員，才能在合作夥伴中心建立或管理付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="234e5-116">獎勵角色必須指派給每個獎勵計畫底下的每個 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="234e5-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="234e5-117">如需如何在合作夥伴中心新增獎勵管理員的詳細資訊，請參閱[如何在合作夥伴中心新增獎勵使用者或系統管理員](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="234e5-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="234e5-118">存取合作夥伴中心的支出和稅務區段</span><span class="sxs-lookup"><span data-stu-id="234e5-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="234e5-119">使用您的 AAD 帳戶（公司帳戶）或適當的電子郵件地址（如果有指派）登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="234e5-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="234e5-120">您可以在一個 AAD 帳戶內註冊多個網域。</span><span class="sxs-lookup"><span data-stu-id="234e5-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="234e5-121">請洽詢您的全域管理員，以判斷哪些網域相關聯。</span><span class="sxs-lookup"><span data-stu-id="234e5-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="234e5-122">如果您只能夠使用網域登入 **@onmicrosoft.com** ，請洽詢您的帳戶管理員，將其他網域新增至 AAD 帳戶。</span><span class="sxs-lookup"><span data-stu-id="234e5-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="234e5-123">如果系統提示您選取**公司或學校帳戶**或**個人帳戶**，請選取 [**公司或學校帳戶**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="234e5-124">選取齒輪圖示以開啟 [**設定**] 功能表，然後選取 [**合作夥伴設定**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="234e5-125">在 [**帳戶設定**] 功能表中，選取 [**支出和稅金**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="234e5-126">將支出和稅務設定檔指派給個別程式</span><span class="sxs-lookup"><span data-stu-id="234e5-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="234e5-127">在 [合作夥伴中心] 中，選取齒輪圖示以開啟 [**設定**] 功能表。</span><span class="sxs-lookup"><span data-stu-id="234e5-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="234e5-128">選取 [**合作夥伴設定**]，展開 [付款**和稅金] 區段**，然後選取 [付款**和稅務設定檔指派**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="234e5-129">系統會顯示您的程式清單。</span><span class="sxs-lookup"><span data-stu-id="234e5-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="234e5-130">選取程式旁的箭號，以查看設定檔詳細資料。</span><span class="sxs-lookup"><span data-stu-id="234e5-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="234e5-131">在 [**稅務設定檔**] 下拉式功能表中，選取您想要的稅務設定檔，或選取 [建立新的設定檔] 選項。</span><span class="sxs-lookup"><span data-stu-id="234e5-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="234e5-132">當您選取建立新設定檔的選項時，系統會將您適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="234e5-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="234e5-133">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="234e5-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="234e5-134">下面提供建立新稅務設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="234e5-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="234e5-135">選取 [**付款條件**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="234e5-136">如果您已選取 [**電子銀行轉移**為付款條件]，請在 [付款設定檔] 下拉式清單中選取您想要的付款設定檔，或選取建立新設定檔的選項。</span><span class="sxs-lookup"><span data-stu-id="234e5-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="234e5-137">當您選取建立新設定檔的選項時，系統會將您適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="234e5-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="234e5-138">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="234e5-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="234e5-139">以下提供建立新付款設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="234e5-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="234e5-140">如果您已選取 [**點數注意事項**] 做為付款方法，請完成驗證，以確認參考的 SAP 編號屬於您的組織。</span><span class="sxs-lookup"><span data-stu-id="234e5-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="234e5-141">如果列出多個 Microsoft 商業實體，您必須為每個實體選取一個付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="234e5-142">付款方法的可用性取決於獎勵計畫的規則。</span><span class="sxs-lookup"><span data-stu-id="234e5-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="234e5-143">選取 [**貨幣**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="234e5-144">當您完成所有付款欄位時，請選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="234e5-145">建立您的銀行設定檔</span><span class="sxs-lookup"><span data-stu-id="234e5-145">Create your bank profile</span></span>

<span data-ttu-id="234e5-146">銀行設定檔是在組織層級建立，可讓您在組織內的多個 MPN 識別碼和獎勵方案之間指派相同的銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="234e5-147">將銀行設定檔套用至不同國家/地區時可能會發生例外狀況，因為可能會套用不同的銀行和稅務規則。</span><span class="sxs-lookup"><span data-stu-id="234e5-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="234e5-148">在下列頁面上，需要有星號的欄位。</span><span class="sxs-lookup"><span data-stu-id="234e5-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="234e5-149">如果您不知道什麼是欄位，請選取資訊圖示。</span><span class="sxs-lookup"><span data-stu-id="234e5-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="234e5-150">在 [**詳細資料**] 頁面上，填寫下欄欄位： [**設定檔名稱]：** 輸入唯一名稱來識別此付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="234e5-151">**銀行帳戶位置：** 貴公司的銀行所在國家/地區。</span><span class="sxs-lookup"><span data-stu-id="234e5-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="234e5-152">**付款方法：**「合作夥伴中心」的慣用付款條件是「電子銀行傳輸」。</span><span class="sxs-lookup"><span data-stu-id="234e5-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="234e5-153">選取 [下一步]。</span><span class="sxs-lookup"><span data-stu-id="234e5-153">Select **Next**.</span></span>

3. <span data-ttu-id="234e5-154">在 [**銀行帳戶**] 頁面上，輸入您的資訊。</span><span class="sxs-lookup"><span data-stu-id="234e5-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="234e5-155">此頁面上顯示的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="234e5-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="234e5-156">選取 [下一步]。</span><span class="sxs-lookup"><span data-stu-id="234e5-156">Select **Next**.</span></span>

5. <span data-ttu-id="234e5-157">在 [**受益人**] 頁面上，輸入適當的資訊。</span><span class="sxs-lookup"><span data-stu-id="234e5-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="234e5-158">如果您的公司需要討論您的帳戶，這些受益者就是銀行所要聯繫的人員。</span><span class="sxs-lookup"><span data-stu-id="234e5-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="234e5-159">當欄位完成時，請選取 **[完成]**，然後選取 [**確認**] 以建立您的銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="234e5-160">系統會將您重新導向至 [付款**和稅務設定檔**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="234e5-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="234e5-161">新設定檔的狀態會反映擱置中的**Microsoft 驗證**，直到驗證完成為止。</span><span class="sxs-lookup"><span data-stu-id="234e5-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="234e5-162">這可能需要最多48小時的時間。</span><span class="sxs-lookup"><span data-stu-id="234e5-162">This may take up to 48 hours.</span></span> <span data-ttu-id="234e5-163">驗證完成後，您的設定檔狀態會反映出**已核准**或**需要採取的動作**。</span><span class="sxs-lookup"><span data-stu-id="234e5-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="234e5-164">如果**需要動作**，請重複上述的步驟，以提供必要的資訊。</span><span class="sxs-lookup"><span data-stu-id="234e5-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="234e5-165">建立您的稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="234e5-165">Create your tax profile</span></span>

<span data-ttu-id="234e5-166">請使用下列程式，為 Microsoft 提供貴組織所需的稅務資訊。</span><span class="sxs-lookup"><span data-stu-id="234e5-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="234e5-167">本節中的頁面是動態的，而且會根據您的國家或地區而有所不同。</span><span class="sxs-lookup"><span data-stu-id="234e5-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="234e5-168">如果您需要協助以識別正確的稅務資訊，請洽詢您所在國家/地區的適當政府來源。</span><span class="sxs-lookup"><span data-stu-id="234e5-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="234e5-169">對於美洲的合作夥伴公司，如果您需要完成 W8 或 W9 表單的相關資訊，下列位址會帶您前往 IRS 網站：</span><span class="sxs-lookup"><span data-stu-id="234e5-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="234e5-170">僅輸入您公司的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="234e5-170">Enter only details for your company.</span></span> <span data-ttu-id="234e5-171">絕對不要輸入個人詳細資料。</span><span class="sxs-lookup"><span data-stu-id="234e5-171">Never enter personal details.</span></span>

1. <span data-ttu-id="234e5-172">在 [**商務設定檔**] 頁面上，填寫必要的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="234e5-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="234e5-173">在 [**安裝**] 頁面上，選取適用于您公司的選項。</span><span class="sxs-lookup"><span data-stu-id="234e5-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="234e5-174">如果您的公司僅納入美國，或此設定檔適用于個人，請選取左側的選項。</span><span class="sxs-lookup"><span data-stu-id="234e5-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="234e5-175">如果您的公司已納入美國以外的地區，請選取右側的選項，然後從清單中選取您的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="234e5-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="234e5-176">選取 [下一步]。</span><span class="sxs-lookup"><span data-stu-id="234e5-176">Select **Next**.</span></span> 

4. <span data-ttu-id="234e5-177">在 [**稅務狀態**] 頁面上，輸入必要的資訊，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="234e5-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="234e5-178">此頁面上的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="234e5-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="234e5-179">您的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="234e5-179">your details.</span></span> 

5. <span data-ttu-id="234e5-180">在 [**其他檔**] 頁面上，所需的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="234e5-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="234e5-181">選取 **[流覽]** 以上傳您的國家或地區所需的任何檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="234e5-182">當檔案名稱顯示時，選取 [**上傳**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="234e5-183">如果您需要移除檔，請選取 [**移除**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="234e5-184">若要儲存並繼續，請選取 **[完成]**。</span><span class="sxs-lookup"><span data-stu-id="234e5-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="234e5-185">在快顯訊息上選取 [**確認**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="234e5-186">系統會將您帶回 [付款**與稅務設定**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="234e5-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="234e5-187">支出和稅務設定檔常見問題</span><span class="sxs-lookup"><span data-stu-id="234e5-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="234e5-188">為什麼我需要提供我的支出和（或）稅務詳細資料？</span><span class="sxs-lookup"><span data-stu-id="234e5-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="234e5-189">若要接收 Microsoft 獎勵計畫的支出，您必須提供有效的支出和稅務詳細資料，以完成註冊。</span><span class="sxs-lookup"><span data-stu-id="234e5-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="234e5-190">只有當您提供的付款和稅務設定檔是由 Microsoft 驗證時，才會將註冊視為完成。</span><span class="sxs-lookup"><span data-stu-id="234e5-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="234e5-191">如何? 知道我需要提供/更新我的支出和（或）稅務詳細資料嗎？</span><span class="sxs-lookup"><span data-stu-id="234e5-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="234e5-192">所有在新的獎勵計畫中註冊的合作夥伴，都必須提供有效的支出和稅務詳細資料，才能完成註冊。</span><span class="sxs-lookup"><span data-stu-id="234e5-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="234e5-193">如果您的獎勵計畫的規則變更，或設定檔的各個層面過期或過期，您可能也需要提供更新的資訊。</span><span class="sxs-lookup"><span data-stu-id="234e5-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="234e5-194">如果發生這種情況，您的 [總覽] 頁面將會顯示 [**需要動作–更新 bank] 和/或 [稅務設定檔**] 的狀態。</span><span class="sxs-lookup"><span data-stu-id="234e5-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="234e5-195">我要如何提供/更新支出和/或稅務詳細資料？</span><span class="sxs-lookup"><span data-stu-id="234e5-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="234e5-196">如需如何在合作夥伴中心更新付款和稅務詳細資料的詳細資訊，請參閱[如何在合作夥伴中心建立和管理銀行和稅務設定檔](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="234e5-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="234e5-197">為什麼我指派支出與稅務設定檔時看不到我的註冊？</span><span class="sxs-lookup"><span data-stu-id="234e5-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="234e5-198">只有 MPN 位置的獎勵管理員可以建立及管理支出與稅務設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="234e5-199">可能是您沒有適當的權限，或者您使用沒有這些權限的帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="234e5-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="234e5-200">請連絡貴組織的管理員，以管理銀行與稅金的權限。</span><span class="sxs-lookup"><span data-stu-id="234e5-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="234e5-201">我可以在哪裡看到我的組織可以使用的付款與稅務設定檔？</span><span class="sxs-lookup"><span data-stu-id="234e5-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="234e5-202">請使用下列程式來查看付款和稅務設定檔：</span><span class="sxs-lookup"><span data-stu-id="234e5-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="234e5-203">登入合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="234e5-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="234e5-204">選取齒輪圖示以開啟 [設定] 功能表。</span><span class="sxs-lookup"><span data-stu-id="234e5-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="234e5-205">選取 [**合作夥伴設定**]。</span><span class="sxs-lookup"><span data-stu-id="234e5-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="234e5-206">在 [帳戶設定] **下**選取 [支出與稅務]，然後選取 [發放款與稅金設定檔]。</span><span class="sxs-lookup"><span data-stu-id="234e5-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="234e5-207">您會看到所有現有的付款與稅務設定檔，以及狀態與編輯能力。</span><span class="sxs-lookup"><span data-stu-id="234e5-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="234e5-208">我的組織參與多項獎勵計畫。</span><span class="sxs-lookup"><span data-stu-id="234e5-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="234e5-209">我是否需要提供我的付款和稅務設定檔多次？</span><span class="sxs-lookup"><span data-stu-id="234e5-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="234e5-210">使用付款設定檔，這通常是由您自行決定。</span><span class="sxs-lookup"><span data-stu-id="234e5-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="234e5-211">付款設定檔是在組織層級建立，可讓您在組織內的多個 MPN 識別碼與獎勵計畫之間指派相同的銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="234e5-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="234e5-212">在大部分的情況下，您可以重複使用現有的設定檔或建立一個新的。</span><span class="sxs-lookup"><span data-stu-id="234e5-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="234e5-213">在將您的銀行設定檔套用至不同的國家或地區時，可能會有一些例外，因為可能適用當地銀行或稅務規則。</span><span class="sxs-lookup"><span data-stu-id="234e5-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="234e5-214">針對 MPN 位置所建立的稅務設定檔會重複使用，並在相同的 MPN 位置參與其他獎勵計畫時自動填入。</span><span class="sxs-lookup"><span data-stu-id="234e5-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="234e5-215">但可能有例外。</span><span class="sxs-lookup"><span data-stu-id="234e5-215">But there can be exceptions.</span></span> <span data-ttu-id="234e5-216">例如，新獎勵計畫的支出規則可能需要稅務設定檔的其他詳細資料。</span><span class="sxs-lookup"><span data-stu-id="234e5-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="234e5-217">我只能夠使用我的網域登入 @onmicrosoft.com 。</span><span class="sxs-lookup"><span data-stu-id="234e5-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="234e5-218">我該怎麼辦？</span><span class="sxs-lookup"><span data-stu-id="234e5-218">What should I do?</span></span>

<span data-ttu-id="234e5-219">請洽詢您的帳戶管理員，將其他網域新增到 AAD 帳戶。</span><span class="sxs-lookup"><span data-stu-id="234e5-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
