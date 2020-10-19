---
title: 針對設定合作夥伴中心帳戶或 MPN 續約問題進行疑難排解
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 針對嘗試註冊合作夥伴中心時發生的問題進行疑難排解。 使用付款條件、忘記密碼等解決問題的答案。
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92174843"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="9ec9b-104">針對帳戶設定或 MPN 續約問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="9ec9b-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="9ec9b-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="9ec9b-105">**Applies to**</span></span>

- <span data-ttu-id="9ec9b-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="9ec9b-106">Partner Center</span></span>
 
<span data-ttu-id="9ec9b-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="9ec9b-107">**Appropriate roles**</span></span>

- <span data-ttu-id="9ec9b-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="9ec9b-108">Global admin</span></span>
- <span data-ttu-id="9ec9b-109">MPN 合作夥伴系統管理員</span><span class="sxs-lookup"><span data-stu-id="9ec9b-109">MPN partner admin</span></span> 
 
<span data-ttu-id="9ec9b-110">以下是一些針對設定合作夥伴中心帳戶時所發生的常見問題進行疑難排解的建議。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="9ec9b-111">如果您要從 Partner Membership Center 進行遷移，而且無法編輯任何公司資訊欄位，會發生什麼事</span><span class="sxs-lookup"><span data-stu-id="9ec9b-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="9ec9b-112">如果您的公司已經有合作夥伴中心的 (說 CSP 帳戶) –您將會看到唯讀畫面。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="9ec9b-113">此畫面會顯示合作夥伴中心中現有公司的所有相關資訊。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="9ec9b-114">您無法變更此畫面上的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-114">You can't change the details on this screen.</span></span> <span data-ttu-id="9ec9b-115">這是設計的，而不是錯誤。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-115">This is by design and not an error.</span></span>

<span data-ttu-id="9ec9b-116">選取 [ **接受** ] 並 **繼續** 進行。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="9ec9b-117">如果 IT 部門已關閉合作夥伴中心的 **註冊**。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="9ec9b-118">您會看到此訊息是因為病毒使用者已停用，或在 Azure AD 的租使用者上停用病毒註冊。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="9ec9b-119">您 Azure AD 帳戶的全域管理員可以執行下列 PowerShell 命令來啟用所需的功能：</span><span class="sxs-lookup"><span data-stu-id="9ec9b-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="9ec9b-120">**Set-msolcompanysettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="9ec9b-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="9ec9b-121">如需詳細資訊，請參閱 [自助式註冊](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="9ec9b-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="9ec9b-122">忘記密碼</span><span class="sxs-lookup"><span data-stu-id="9ec9b-122">You forgot your password</span></span>

<span data-ttu-id="9ec9b-123">如果您忘了密碼，請在登入頁面上選取 [ **無法存取您的帳戶？** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="9ec9b-124">此選項可讓您重設密碼，或要求您的全域管理員為您指派新的認證。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="9ec9b-125">在 [告訴我們您的公司] scree 上，您會收到「發生錯誤」錯誤</span><span class="sxs-lookup"><span data-stu-id="9ec9b-125">On the “Tell us about your company” scree, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="9ec9b-126">如果您不小心在公司電話號碼中使用特殊字元、空格或國家/地區代碼，則通常會出現此錯誤訊息。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="9ec9b-127">[電話號碼] 欄位中輸入的值最多隻能包含10個字元。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="9ec9b-128">您的信用卡購買收到錯誤訊息，指出「您的訂單已遭到拒絕。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="9ec9b-129">請驗證您的資訊」</span><span class="sxs-lookup"><span data-stu-id="9ec9b-129">Please verify your information”</span></span>


<span data-ttu-id="9ec9b-130">請一律使用與信用卡相對應的位址，而不是您的法律實體。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="9ec9b-131">此外，請確定郵遞區號正確，並對應至您所使用的位址。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="9ec9b-132">您想要從離線付款切換至線上付款條件</span><span class="sxs-lookup"><span data-stu-id="9ec9b-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="9ec9b-133">您將需要使用慣用的付款條件來取消原始訂單和重新購買。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="9ec9b-134">若要取消訂單：</span><span class="sxs-lookup"><span data-stu-id="9ec9b-134">To cancel an order:</span></span>

1. <span data-ttu-id="9ec9b-135">選取儀表板中的 [ **成員資格** 供應專案] 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="9ec9b-136">選取 [**取消訂單**]</span><span class="sxs-lookup"><span data-stu-id="9ec9b-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="9ec9b-137">確認視窗會出現，您必須確認才能取消最初訂單。</span><span class="sxs-lookup"><span data-stu-id="9ec9b-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9ec9b-138">後續步驟</span><span class="sxs-lookup"><span data-stu-id="9ec9b-138">Next steps</span></span>

- [<span data-ttu-id="9ec9b-139">管理您的合作夥伴中心帳戶</span><span class="sxs-lookup"><span data-stu-id="9ec9b-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="9ec9b-140">如何讀取帳單和偵察檔案</span><span class="sxs-lookup"><span data-stu-id="9ec9b-140">How to read your bill and recon file</span></span>](read-your-bill.md)