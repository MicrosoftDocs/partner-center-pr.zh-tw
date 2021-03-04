---
title: 合作夥伴中心的支出和稅金設定檔
ms.topic: how-to
ms.date: 02/24/2021
description: 建立及管理您的付款和稅務設定檔，以便支付獎勵工作的費用。 包括建立、管理及使用不同的設定檔。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ba8c1a811d66a5e6233f625c3981283341ea546c
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756600"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="95bed-104">在合作夥伴中心建立和管理獎勵支出和稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="95bed-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>


<span data-ttu-id="95bed-105">**適當的角色：**</span><span class="sxs-lookup"><span data-stu-id="95bed-105">**Appropriate roles:**</span></span>

- <span data-ttu-id="95bed-106">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="95bed-106">Incentives admin</span></span>
- <span data-ttu-id="95bed-107">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="95bed-107">Account admin</span></span>
- <span data-ttu-id="95bed-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="95bed-108">Global admin</span></span>

<span data-ttu-id="95bed-109">您必須先將有效的支出和稅務設定檔與計畫和 MPN 的位置產生關聯，才能收到特定 MPN 位置的獎勵計畫款項。</span><span class="sxs-lookup"><span data-stu-id="95bed-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="95bed-110">Microsoft 將使用此支出與稅務設定檔來發出款項。</span><span class="sxs-lookup"><span data-stu-id="95bed-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="95bed-111">視獎勵計畫的規則而定，您可能可以使用電子銀行轉帳或貸記通知單來付款。</span><span class="sxs-lookup"><span data-stu-id="95bed-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="95bed-112">角色、貨幣及其他 Microsoft 程式</span><span class="sxs-lookup"><span data-stu-id="95bed-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="95bed-113">開始使用您的付款和稅務設定檔之前，請務必先瞭解下列資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="95bed-114">角色和權限</span><span class="sxs-lookup"><span data-stu-id="95bed-114">Roles and permissions</span></span>

<span data-ttu-id="95bed-115">您必須是獎勵系統管理員，才能輸入報酬金的銀行和稅務資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="95bed-116">如果您是 MPN/帳戶系統管理員，您可以將自己和/或同事指派為獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="95bed-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="95bed-117">如果您需要要求獎勵系統管理員許可權，請洽詢您的 MPN 系統管理員或全域管理員。您可以登入「 [合作夥伴中心」儀表板](https://partner.microsoft.com/dashboard/)，找出貴公司中有哪些人擁有這些角色。</span><span class="sxs-lookup"><span data-stu-id="95bed-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="95bed-118">從右上方的 **設定** 圖示中，選取 [ **使用者管理** ]，然後篩選全域管理員。</span><span class="sxs-lookup"><span data-stu-id="95bed-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="95bed-119">獎勵使用者可以查看獎勵收益和付款詳細資料和報表，但無法編輯銀行和稅務詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="95bed-120">選擇您的付款貨幣</span><span class="sxs-lookup"><span data-stu-id="95bed-120">Choose your disbursement currency</span></span>

<span data-ttu-id="95bed-121">當您設定付款設定檔時，會以您選取的貨幣來進行獎勵款項。</span><span class="sxs-lookup"><span data-stu-id="95bed-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="95bed-122">付款將會使用 Microsoft 每月設定的匯率計算。</span><span class="sxs-lookup"><span data-stu-id="95bed-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="95bed-123">由於選取的貨幣，您將負責任何值的變更。</span><span class="sxs-lookup"><span data-stu-id="95bed-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="95bed-124">針對不同的 Microsoft 程式使用不同的設定檔</span><span class="sxs-lookup"><span data-stu-id="95bed-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="95bed-125">如果您的公司已在多個獎勵方案中註冊，您可以對所有帳戶使用相同的付款帳戶，或針對不同的程式選擇使用不同的付款帳戶。</span><span class="sxs-lookup"><span data-stu-id="95bed-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="95bed-126">在合作夥伴中心建立及管理支出與稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="95bed-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="95bed-127">下列各節將逐步引導您完成在合作夥伴中心建立和管理付款和稅務設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="95bed-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="95bed-128">您必須是獎勵系統管理員，才能在合作夥伴中心建立或管理付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="95bed-129">獎勵角色必須指派給每個獎勵計畫下的每個 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="95bed-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="95bed-130">如需有關如何在合作夥伴中心新增獎勵管理員的詳細資訊，請參閱 [建立使用者帳戶](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="95bed-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="95bed-131">存取合作夥伴中心的付款和稅務區段</span><span class="sxs-lookup"><span data-stu-id="95bed-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="95bed-132">使用您的 Azure Active Directory (Azure AD) 帳戶 (公司帳戶) 或已指派的適當電子郵件地址，登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/) 。</span><span class="sxs-lookup"><span data-stu-id="95bed-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="95bed-133">您可以在一個 Azure AD 帳戶內註冊多個網域。</span><span class="sxs-lookup"><span data-stu-id="95bed-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="95bed-134">請洽詢您的全域系統管理員，以判斷哪些網域相關聯。</span><span class="sxs-lookup"><span data-stu-id="95bed-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="95bed-135">如果您只能使用網域登入 @onmicrosoft.com ，請洽詢您的帳戶管理員，將其他網域新增至 AZURE AD 帳戶。</span><span class="sxs-lookup"><span data-stu-id="95bed-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="95bed-136">如果系統提示您選取 [ **公司或學校帳戶** ] 或 [ **個人帳戶**]，請選取 [ **公司或學校帳戶**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="95bed-137">選取齒輪圖示以開啟 [ **設定** ] 功能表，然後選取 [ **帳戶設定**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="95bed-138">在 [ **帳戶設定** ] 功能表中，選取 [付款 **和稅金**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="95bed-139">將付款和稅務設定檔指派給個別的程式</span><span class="sxs-lookup"><span data-stu-id="95bed-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="95bed-140">登入 [ [合作夥伴中心] 儀表板](https://partner.microsoft.com/dashboard/)，然後選取齒輪圖示以開啟 [ **設定** ] 功能表。</span><span class="sxs-lookup"><span data-stu-id="95bed-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="95bed-141">選取 [ **帳戶設定**]，展開 [支付 **和稅務] 區段**，然後選取 [支付 **和稅務設定檔指派**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="95bed-142">系統將會顯示您的程式清單。</span><span class="sxs-lookup"><span data-stu-id="95bed-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="95bed-143">選取程式旁邊的箭號，以查看設定檔詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="95bed-144">在 [ **稅務設定檔** ] 下拉式功能表中，選取您要的稅務設定檔，或選取選項來建立新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="95bed-145">當您選取選項來建立新的設定檔時，系統會適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="95bed-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="95bed-146">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="95bed-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="95bed-147">以下提供建立新的稅務設定檔的程式。</span><span class="sxs-lookup"><span data-stu-id="95bed-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="95bed-148">選取 **付款方法**。</span><span class="sxs-lookup"><span data-stu-id="95bed-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="95bed-149">如果您已選取 [ **電子銀行轉移** ] 作為付款條件，請選取您想要的付款設定檔，或選取選項來建立新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="95bed-150">當您選取選項來建立新的設定檔時，系統會適當地重新導向。</span><span class="sxs-lookup"><span data-stu-id="95bed-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="95bed-151">在快顯視窗中選取 [繼續]。</span><span class="sxs-lookup"><span data-stu-id="95bed-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="95bed-152">以下提供建立新付款設定檔的流程。</span><span class="sxs-lookup"><span data-stu-id="95bed-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="95bed-153">如果您已選取 [ **信用卡] 附注** 作為付款條件，請完成驗證。</span><span class="sxs-lookup"><span data-stu-id="95bed-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="95bed-154">這會確認參考的 SAP 編號屬於您的組織。</span><span class="sxs-lookup"><span data-stu-id="95bed-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="95bed-155">如果列出多個 Microsoft 商務實體，您必須為每個實體選取付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="95bed-156">付款方法的可用性取決於獎勵計畫的規則。</span><span class="sxs-lookup"><span data-stu-id="95bed-156">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="95bed-157">如果您的位置 MPN 識別碼是由特定獎勵方案的當地 Microsoft 子公司支付，並允許 LRD (有限的風險散發者) 點數備忘錄作為付款條件，則您的付款設定檔將會預先填入 LRD 信用額度付款方法。</span><span class="sxs-lookup"><span data-stu-id="95bed-157">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="95bed-158">在個別「獎勵計畫」和「位置 MPN 識別碼」的 [LRD 信用卡附注付款方法] 資料列上，您會在 [付款設定檔] 區段中看到 [已 **確認** ] 或 [ **需要驗證** ] 狀態。</span><span class="sxs-lookup"><span data-stu-id="95bed-158">On the LRD credit note payment method row for the respective incentive program and location MPN ID you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="95bed-159">選取 **所需的驗證** ，以確認和確認與 location MPN 和付款方法相關聯的 CSP 租使用者識別碼詳細資料，以接收信用額度付款。</span><span class="sxs-lookup"><span data-stu-id="95bed-159">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="95bed-160">在 [ **信用評論詳細資料** ] 對話方塊中，檢查並確認提供的 CSP 租使用者識別碼和詳細資料正確無誤。</span><span class="sxs-lookup"><span data-stu-id="95bed-160">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="95bed-161">如果您有一個以上的租使用者識別碼，請仔細選取您要在其上收到付款的 CSP 租使用者識別碼。</span><span class="sxs-lookup"><span data-stu-id="95bed-161">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="95bed-162">接下來，選取 [ **確認** ] 以確認您的公司詳細資料是否正確，以及是否應該對您選取的 CSP 租使用者識別碼進行獎勵付款。</span><span class="sxs-lookup"><span data-stu-id="95bed-162">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="95bed-163">如果狀態顯示為 [已 **確認**]，表示 CSP 租使用者識別碼的指派已完成，且不需要採取進一步的動作。</span><span class="sxs-lookup"><span data-stu-id="95bed-163">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="95bed-164">您仍然可以選取 [已確認] 以查看指派的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-164">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="95bed-165">在需要合作夥伴明確要求套用免稅的國家/地區，將會有一個選項可在 [獎勵方案和位置 MPN] 的 [稅務設定檔] 區段中，于稅務設定檔旁邊套用免稅。</span><span class="sxs-lookup"><span data-stu-id="95bed-165">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="95bed-166">核取此方塊會將免稅權益套用至您的獎勵點數注意事項。</span><span class="sxs-lookup"><span data-stu-id="95bed-166">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="95bed-167">目前，此付款條件僅適用于澳大利亞、紐西蘭和加拿大合作夥伴，適用于 Microsoft Commerce 獎勵方案。</span><span class="sxs-lookup"><span data-stu-id="95bed-167">Currently, this payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="95bed-168">如果您是這三個國家/地區的直接帳單合作夥伴或間接提供者，而這三個國家/地區註冊了 MCI 方案，而且您沒有看到 LRD 的點數提示作為可用的付款條件，請確認您的租使用者識別碼與相關的夥伴 MPN 位置帳戶相關聯。</span><span class="sxs-lookup"><span data-stu-id="95bed-168">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="95bed-169">如需此操作的詳細資訊，請參閱 [如何更新您的組織設定檔](update-your-partner-profile.md)。</span><span class="sxs-lookup"><span data-stu-id="95bed-169">For more information on this read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="95bed-170">選取 **貨幣**。</span><span class="sxs-lookup"><span data-stu-id="95bed-170">Select the **Currency**.</span></span>

6. <span data-ttu-id="95bed-171">當您完成所有的付款欄位時，請選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-171">When you’ve completed all of the payment fields, select **Submit**.</span></span>


## <a name="create-your-bank-profile"></a><span data-ttu-id="95bed-172">建立您的銀行設定檔</span><span class="sxs-lookup"><span data-stu-id="95bed-172">Create your bank profile</span></span>

<span data-ttu-id="95bed-173">銀行設定檔會在組織層級建立。</span><span class="sxs-lookup"><span data-stu-id="95bed-173">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="95bed-174">這可在組織內的多個 MPN 識別碼和獎勵方案之間指派一個銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-174">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="95bed-175">將銀行設定檔套用至不同的國家/地區時可能會發生例外狀況，因為可能會有不同的銀行和稅務規則。</span><span class="sxs-lookup"><span data-stu-id="95bed-175">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="95bed-176">在下列頁面上，需要有星號的欄位。</span><span class="sxs-lookup"><span data-stu-id="95bed-176">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="95bed-177">如果您不知道欄位是什麼，請選取資訊圖示。</span><span class="sxs-lookup"><span data-stu-id="95bed-177">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="95bed-178">在 [ **詳細資料** ] 頁面上，完成下欄欄位： **設定檔名稱：** 輸入唯一名稱來識別此付款設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-178">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="95bed-179">**銀行帳戶位置：** 公司銀行所在的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="95bed-179">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="95bed-180">**付款方法：** 合作夥伴中心的慣用付款方法是電子銀行轉帳。</span><span class="sxs-lookup"><span data-stu-id="95bed-180">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="95bed-181">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="95bed-181">Select **Next**.</span></span>

3. <span data-ttu-id="95bed-182">在 [ **銀行帳戶** ] 頁面上，輸入您的資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-182">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="95bed-183">此頁面上顯示的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="95bed-183">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="95bed-184">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="95bed-184">Select **Next**.</span></span>

5. <span data-ttu-id="95bed-185">在 [ **受益人** ] 頁面上，輸入適當的資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-185">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="95bed-186">如果您的公司需要討論您的帳戶，則這些受益人就是貴公司的人員。</span><span class="sxs-lookup"><span data-stu-id="95bed-186">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="95bed-187">當欄位完成時，請選取 **[完成]**，然後選取 [ **確認** ] 以建立您的銀行設定檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-187">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="95bed-188">系統會將您重新導向至 [付款 **和稅務設定檔** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="95bed-188">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="95bed-189">新設定檔的狀態將反映擱置中的 **Microsoft 驗證** ，直到驗證完成為止。</span><span class="sxs-lookup"><span data-stu-id="95bed-189">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="95bed-190">此程式最多可能需要48小時的時間。</span><span class="sxs-lookup"><span data-stu-id="95bed-190">This process may take up to 48 hours.</span></span> <span data-ttu-id="95bed-191">完成驗證之後，您的設定檔狀態將會反映出 **所需** 的 **核准** 或動作。</span><span class="sxs-lookup"><span data-stu-id="95bed-191">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="95bed-192">如果 **需要採取動作**，請重複上述步驟以提供必要的資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-192">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="95bed-193">建立您的稅務設定檔</span><span class="sxs-lookup"><span data-stu-id="95bed-193">Create your tax profile</span></span>

<span data-ttu-id="95bed-194">使用下列程式，為 Microsoft 提供貴組織所需的稅務資訊。</span><span class="sxs-lookup"><span data-stu-id="95bed-194">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="95bed-195">本節中的頁面為動態，而且會根據您的國家或地區而有所不同。</span><span class="sxs-lookup"><span data-stu-id="95bed-195">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="95bed-196">如果您需要協助來識別正確的稅務資訊，請在您的國家/地區中聯絡適當的政府來源。</span><span class="sxs-lookup"><span data-stu-id="95bed-196">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="95bed-197">針對美洲的合作夥伴公司，如果您需要填寫 W8 或 W9 表單的相關資訊，下列位址會帶您前往 IRS 網站：</span><span class="sxs-lookup"><span data-stu-id="95bed-197">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="95bed-198">只輸入您公司的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-198">Enter only details for your company.</span></span> <span data-ttu-id="95bed-199">絕不輸入個人詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-199">Never enter personal details.</span></span>

1. <span data-ttu-id="95bed-200">在 [ **商務設定檔** ] 頁面上，填寫必要的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="95bed-200">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="95bed-201">在 [ **安裝** ] 頁面上，選取適用于您公司的選項。</span><span class="sxs-lookup"><span data-stu-id="95bed-201">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="95bed-202">如果您的公司僅納入美國，或此設定檔適用于個人，請選取左邊的選項。</span><span class="sxs-lookup"><span data-stu-id="95bed-202">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="95bed-203">如果您的公司是在美國以外的地區，請選取右側的選項，然後從清單中選取您的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="95bed-203">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="95bed-204">選取 [下一步] 。</span><span class="sxs-lookup"><span data-stu-id="95bed-204">Select **Next**.</span></span> 

4. <span data-ttu-id="95bed-205">在 [ **稅務狀態** ] 頁面上，輸入必要的資訊，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="95bed-205">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="95bed-206">此頁面上的欄位會因國家/地區而異。</span><span class="sxs-lookup"><span data-stu-id="95bed-206">Fields on this page will vary by country.</span></span> <span data-ttu-id="95bed-207">您的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="95bed-207">your details.</span></span> 

5. <span data-ttu-id="95bed-208">在 [ **其他檔** ] 頁面上，選取必要的欄位，然後選取 **[下一步]**。</span><span class="sxs-lookup"><span data-stu-id="95bed-208">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="95bed-209">選取 **[流覽]** 以上傳您的國家或地區所需的任何檔。</span><span class="sxs-lookup"><span data-stu-id="95bed-209">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="95bed-210">當檔案名稱顯示時，選取 [ **上傳**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-210">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="95bed-211">如果您需要移除檔，請選取 [ **移除**]。</span><span class="sxs-lookup"><span data-stu-id="95bed-211">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="95bed-212">若要儲存並繼續，請選取 **[完成]**。</span><span class="sxs-lookup"><span data-stu-id="95bed-212">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="95bed-213">選取快顯視窗上的 [ **確認** ]。</span><span class="sxs-lookup"><span data-stu-id="95bed-213">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="95bed-214">您將會回到 [付款 **和稅務設定** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="95bed-214">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="95bed-215">下一步</span><span class="sxs-lookup"><span data-stu-id="95bed-215">Next steps</span></span>

- [<span data-ttu-id="95bed-216">支出和稅金的常見問題</span><span class="sxs-lookup"><span data-stu-id="95bed-216">Common questions about payouts and taxes</span></span>](payout-faq.md)
