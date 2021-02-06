---
title: 合作夥伴中心的支出和稅金設定檔
ms.topic: how-to
ms.date: 11/12/2020
description: 建立及管理您的付款和稅務設定檔，以便支付獎勵工作的費用。 包括建立、管理及使用不同的設定檔。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 282fdacc8689ff71e885a2f0ea01ce9570611707
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624233"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="39ec9-104">在合作夥伴中心中建立及管理獎勵支出和稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="39ec9-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="39ec9-105">**適當的角色：**</span><span class="sxs-lookup"><span data-stu-id="39ec9-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="39ec9-106">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="39ec9-106">Incentives admin</span></span>
- <span data-ttu-id="39ec9-107">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="39ec9-107">Account admin</span></span>
- <span data-ttu-id="39ec9-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="39ec9-108">Global admin</span></span>

<span data-ttu-id="39ec9-109">您必須先將有效的支出和稅務設定檔與計畫和 MPN 的位置產生關聯，才能收到特定 MPN 位置的獎勵計畫款項。</span><span class="sxs-lookup"><span data-stu-id="39ec9-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="39ec9-110">Microsoft 將使用此支出與稅務設定檔來發出款項。</span><span class="sxs-lookup"><span data-stu-id="39ec9-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="39ec9-111">視獎勵計畫的規則而定，您可能可以使用電子銀行轉帳或貸記通知單來付款。</span><span class="sxs-lookup"><span data-stu-id="39ec9-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="39ec9-112">角色、貨幣及其他 Microsoft 程式</span><span class="sxs-lookup"><span data-stu-id="39ec9-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="39ec9-113">開始使用您的付款和稅務設定檔之前，請務必先瞭解下列資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="39ec9-114">角色和權限</span><span class="sxs-lookup"><span data-stu-id="39ec9-114">Roles and permissions</span></span>

<span data-ttu-id="39ec9-115">您必須是獎勵系統管理員，才能輸入報酬金的銀行和稅務資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="39ec9-116">如果您是 MPN/帳戶系統管理員，您可以將自己和/或同事指派為獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="39ec9-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="39ec9-117">如果您需要要求獎勵系統管理員許可權，請洽詢您的 MPN 系統管理員或全域管理員。您可以登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)，找出貴公司中的誰擁有這些角色。</span><span class="sxs-lookup"><span data-stu-id="39ec9-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="39ec9-118">從右上方的 **設定** 圖示中，選取 [ **使用者管理** ]，然後篩選全域管理員。</span><span class="sxs-lookup"><span data-stu-id="39ec9-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="39ec9-119">獎勵使用者可以查看獎勵收益和付款詳細資料和報表，但無法編輯銀行和稅務詳細資料。</span><span class="sxs-lookup"><span data-stu-id="39ec9-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="39ec9-120">選擇您的付款貨幣</span><span class="sxs-lookup"><span data-stu-id="39ec9-120">Choose your disbursement currency</span></span>

<span data-ttu-id="39ec9-121">當您設定付款設定檔時，會以您選取的貨幣來進行獎勵款項。</span><span class="sxs-lookup"><span data-stu-id="39ec9-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="39ec9-122">付款將會使用 Microsoft 每月設定的匯率計算。</span><span class="sxs-lookup"><span data-stu-id="39ec9-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="39ec9-123">由於選取的貨幣，您將負責任何值的變更。</span><span class="sxs-lookup"><span data-stu-id="39ec9-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="39ec9-124">針對不同的 Microsoft 程式使用不同的設定檔</span><span class="sxs-lookup"><span data-stu-id="39ec9-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="39ec9-125">如果您的公司已在多個獎勵方案中註冊，您可以對所有帳戶使用相同的付款帳戶，或針對不同的程式選擇使用不同的付款帳戶。</span><span class="sxs-lookup"><span data-stu-id="39ec9-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="39ec9-126">在合作夥伴中心建立及管理支出與稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="39ec9-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="39ec9-127">下列各節將逐步引導您在合作夥伴中心中建立和管理付款和稅務設定檔的流程。</span><span class="sxs-lookup"><span data-stu-id="39ec9-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="39ec9-128">您必須是獎勵系統管理員，才能在合作夥伴中心中建立或管理付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="39ec9-129">獎勵角色必須指派給每個獎勵計畫下的每個 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="39ec9-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="39ec9-130">如需有關如何在合作夥伴中心中新增「獎勵管理員」的詳細資訊，請參閱 [建立使用者帳戶](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="39ec9-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="39ec9-131">存取合作夥伴中心中的付款和稅務區段</span><span class="sxs-lookup"><span data-stu-id="39ec9-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="39ec9-132">使用您的 Azure Active Directory (Azure AD) 帳戶 (公司帳戶) ，或已指派適當的電子郵件地址，登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/) 。</span><span class="sxs-lookup"><span data-stu-id="39ec9-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="39ec9-133">您可以在一個 Azure AD 帳戶內註冊多個網域。</span><span class="sxs-lookup"><span data-stu-id="39ec9-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="39ec9-134">請洽詢您的全域系統管理員，以判斷哪些網域相關聯。</span><span class="sxs-lookup"><span data-stu-id="39ec9-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="39ec9-135">如果您只能使用網域登入 @onmicrosoft.com ，請洽詢您的帳戶管理員，將其他網域新增至 Azure AD 帳戶。</span><span class="sxs-lookup"><span data-stu-id="39ec9-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="39ec9-136">如果系統提示您選取 [ **公司或學校帳戶** ] 或 [ **個人帳戶**]，請選取 [ **公司或學校帳戶**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="39ec9-137">選取齒輪圖示以開啟 [ **設定** ] 功能表，然後選取 [ **帳戶設定**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="39ec9-138">在 [ **帳戶設定** ] 功能表中，選取 [付款 **和稅金**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="39ec9-139">將付款和稅務設定檔指派給個別的程式</span><span class="sxs-lookup"><span data-stu-id="39ec9-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="39ec9-140">登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)，然後選取齒輪圖示以開啟 [ **設定** ] 功能表。</span><span class="sxs-lookup"><span data-stu-id="39ec9-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="39ec9-141">選取 [ **帳戶設定**]，展開 [支付 **和稅務] 區段**，然後選取 [支付 **和稅務設定檔指派**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="39ec9-142">系統將會顯示您的程式清單。</span><span class="sxs-lookup"><span data-stu-id="39ec9-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="39ec9-143">選取程式旁邊的箭號，以查看設定檔詳細資料。</span><span class="sxs-lookup"><span data-stu-id="39ec9-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="39ec9-144">在 [ **稅務設定檔** ] 下拉式功能表中，選取您要的稅務設定檔，或選取選項來建立新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="39ec9-145">當您選取選項來建立新的設定檔時，系統會適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="39ec9-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="39ec9-146">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="39ec9-147">以下提供建立新的稅務設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="39ec9-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="39ec9-148">選取 **付款方法**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="39ec9-149">如果您已選取 [ **電子銀行轉移** ] 作為付款條件，請選取您想要的付款設定檔，或選取選項來建立新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="39ec9-150">當您選取選項來建立新的設定檔時，系統會適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="39ec9-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="39ec9-151">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="39ec9-152">以下提供建立新付款設定檔的流程。</span><span class="sxs-lookup"><span data-stu-id="39ec9-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="39ec9-153">如果您已選取 [ **信用卡] 附注** 作為付款條件，請完成驗證。</span><span class="sxs-lookup"><span data-stu-id="39ec9-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="39ec9-154">這會確認參考的 SAP 編號屬於您的組織。</span><span class="sxs-lookup"><span data-stu-id="39ec9-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="39ec9-155">如果列出多個 Microsoft 商務實體，您必須為每個實體選取付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="39ec9-156">付款方法的可用性取決於獎勵計畫的規則。</span><span class="sxs-lookup"><span data-stu-id="39ec9-156">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="39ec9-157">選取 **貨幣**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-157">Select the **Currency**.</span></span>

6. <span data-ttu-id="39ec9-158">當您完成所有的付款欄位時，請選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-158">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="39ec9-159">建立您的銀行設定檔</span><span class="sxs-lookup"><span data-stu-id="39ec9-159">Create your bank profile</span></span>

<span data-ttu-id="39ec9-160">銀行設定檔會在組織層級建立。</span><span class="sxs-lookup"><span data-stu-id="39ec9-160">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="39ec9-161">這可在組織內的多個 MPN 識別碼和獎勵方案之間指派一個銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-161">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="39ec9-162">將銀行設定檔套用至不同的國家/地區時可能會發生例外狀況，因為可能會有不同的銀行和稅務規則。</span><span class="sxs-lookup"><span data-stu-id="39ec9-162">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="39ec9-163">在下列頁面上，需要有星號的欄位。</span><span class="sxs-lookup"><span data-stu-id="39ec9-163">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="39ec9-164">如果您不知道欄位是什麼，請選取資訊圖示。</span><span class="sxs-lookup"><span data-stu-id="39ec9-164">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="39ec9-165">在 [ **詳細資料** ] 頁面上，完成下欄欄位： **設定檔名稱：** 輸入唯一名稱來識別此付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-165">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="39ec9-166">**銀行帳戶位置：** 公司銀行所在的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="39ec9-166">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="39ec9-167">**付款方法：** 合作夥伴中心的慣用付款條件是「電子銀行傳輸」。</span><span class="sxs-lookup"><span data-stu-id="39ec9-167">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="39ec9-168">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="39ec9-168">Select **Next**.</span></span>

3. <span data-ttu-id="39ec9-169">在 [ **銀行帳戶** ] 頁面上，輸入您的資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-169">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="39ec9-170">此頁面上顯示的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="39ec9-170">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="39ec9-171">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="39ec9-171">Select **Next**.</span></span>

5. <span data-ttu-id="39ec9-172">在 [ **受益人** ] 頁面上，輸入適當的資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-172">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="39ec9-173">如果您的公司需要討論您的帳戶，則這些受益人就是貴公司的人員。</span><span class="sxs-lookup"><span data-stu-id="39ec9-173">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="39ec9-174">當欄位完成時，請選取 **[完成]**，然後選取 [ **確認** ] 以建立您的銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-174">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="39ec9-175">系統會將您重新導向至 [付款 **和稅務設定檔** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="39ec9-175">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="39ec9-176">新設定檔的狀態將反映擱置中的 **Microsoft 驗證** ，直到驗證完成為止。</span><span class="sxs-lookup"><span data-stu-id="39ec9-176">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="39ec9-177">此程式最多可能需要48小時的時間。</span><span class="sxs-lookup"><span data-stu-id="39ec9-177">This process may take up to 48 hours.</span></span> <span data-ttu-id="39ec9-178">完成驗證之後，您的設定檔狀態將會反映出 **所需** 的 **核准** 或動作。</span><span class="sxs-lookup"><span data-stu-id="39ec9-178">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="39ec9-179">如果 **需要採取動作**，請重複上述步驟以提供必要的資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-179">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="39ec9-180">建立您的稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="39ec9-180">Create your tax profile</span></span>

<span data-ttu-id="39ec9-181">使用下列程式，為 Microsoft 提供貴組織所需的稅務資訊。</span><span class="sxs-lookup"><span data-stu-id="39ec9-181">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="39ec9-182">本節中的頁面為動態，而且會根據您的國家或地區而有所不同。</span><span class="sxs-lookup"><span data-stu-id="39ec9-182">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="39ec9-183">如果您需要協助來識別正確的稅務資訊，請在您的國家/地區中聯絡適當的政府來源。</span><span class="sxs-lookup"><span data-stu-id="39ec9-183">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="39ec9-184">針對美洲的合作夥伴公司，如果您需要填寫 W8 或 W9 表單的相關資訊，下列位址會帶您前往 IRS 網站：</span><span class="sxs-lookup"><span data-stu-id="39ec9-184">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="39ec9-185">只輸入您公司的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="39ec9-185">Enter only details for your company.</span></span> <span data-ttu-id="39ec9-186">絕不輸入個人詳細資料。</span><span class="sxs-lookup"><span data-stu-id="39ec9-186">Never enter personal details.</span></span>

1. <span data-ttu-id="39ec9-187">在 [ **商務設定檔** ] 頁面上，填寫必要的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-187">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="39ec9-188">在 [ **安裝** ] 頁面上，選取適用于您公司的選項。</span><span class="sxs-lookup"><span data-stu-id="39ec9-188">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="39ec9-189">如果您的公司僅納入美國，或此設定檔適用于個人，請選取左邊的選項。</span><span class="sxs-lookup"><span data-stu-id="39ec9-189">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="39ec9-190">如果您的公司是在美國以外的地區，請選取右側的選項，然後從清單中選取您的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="39ec9-190">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="39ec9-191">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="39ec9-191">Select **Next**.</span></span> 

4. <span data-ttu-id="39ec9-192">在 [ **稅務狀態** ] 頁面上，輸入必要的資訊，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-192">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="39ec9-193">此頁面上的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="39ec9-193">Fields on this page will vary by country.</span></span> <span data-ttu-id="39ec9-194">您的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="39ec9-194">your details.</span></span> 

5. <span data-ttu-id="39ec9-195">在 [ **其他檔** ] 頁面上，選取必要的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-195">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="39ec9-196">選取 **[流覽]** 以上傳您的國家或地區所需的任何檔。</span><span class="sxs-lookup"><span data-stu-id="39ec9-196">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="39ec9-197">當檔案名稱顯示時，選取 [ **上傳**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-197">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="39ec9-198">如果您需要移除檔，請選取 [ **移除**]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-198">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="39ec9-199">若要儲存並繼續，請選取 **[完成]**。</span><span class="sxs-lookup"><span data-stu-id="39ec9-199">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="39ec9-200">選取快顯視窗上的 [ **確認** ]。</span><span class="sxs-lookup"><span data-stu-id="39ec9-200">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="39ec9-201">您將會回到 [付款 **和稅務設定** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="39ec9-201">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="39ec9-202">下一步</span><span class="sxs-lookup"><span data-stu-id="39ec9-202">Next steps</span></span>

- [<span data-ttu-id="39ec9-203">支出和稅金的常見問題</span><span class="sxs-lookup"><span data-stu-id="39ec9-203">Common questions about payouts and taxes</span></span>](payout-faq.md)
