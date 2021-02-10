---
title: 管理合作夥伴帳戶中的位置
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何新增位置，以及如何在獎勵計畫、雲端解決方案提供者業務、訂閱和其他交易中使用 MPN 識別碼。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005910"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="fb074-103">管理您的 MPN 帳戶位置，並新增 (刪除) 位置</span><span class="sxs-lookup"><span data-stu-id="fb074-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="fb074-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="fb074-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fb074-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="fb074-105">Global admin</span></span>
- <span data-ttu-id="fb074-106">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="fb074-106">Account admin</span></span>

<span data-ttu-id="fb074-107">位置 MPN 識別碼可識別公司的每個特定位置。</span><span class="sxs-lookup"><span data-stu-id="fb074-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="fb074-108">您可以使用位置 MPN 識別碼來註冊獎勵計畫、交易雲端解決方案提供者 (CSP) 業務以及其他商業交易。</span><span class="sxs-lookup"><span data-stu-id="fb074-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="fb074-109">全域 MPN 識別碼可用於非交易式活動，例如支援要求。</span><span class="sxs-lookup"><span data-stu-id="fb074-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="fb074-110">以下為典型的案例：</span><span class="sxs-lookup"><span data-stu-id="fb074-110">The following is a typical scenario:</span></span>

<span data-ttu-id="fb074-111">Contoso 在英國有其合作夥伴通用帳戶 (PGA)。</span><span class="sxs-lookup"><span data-stu-id="fb074-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="fb074-112">這是其已註冊的合法公司，而且有一個用於管理所有非交易業務的全域 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="fb074-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="fb074-113">Contoso 在英國、法國和美國的其他位置也有相當於分公司或部門的合作夥伴位置帳戶 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="fb074-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="fb074-114">在 MPN 帳戶結構中，這些 PLA 會以唯一的位置 MPN 識別碼來表示。</span><span class="sxs-lookup"><span data-stu-id="fb074-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="fb074-115">PLA 可用於交易業務，例如 CSP 或獎勵計畫。</span><span class="sxs-lookup"><span data-stu-id="fb074-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="fb074-116">支出會繫結至特定位置。</span><span class="sxs-lookup"><span data-stu-id="fb074-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="fb074-117">CSP 租用戶與 MPN 位置識別碼之間有 1 對 1 的關聯性。</span><span class="sxs-lookup"><span data-stu-id="fb074-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的結構":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="fb074-119">為 CSP 商務新增帳戶的必要條件</span><span class="sxs-lookup"><span data-stu-id="fb074-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="fb074-120">若要加入新的 CSP 商務帳戶，請先確定您已滿足必要條件。</span><span class="sxs-lookup"><span data-stu-id="fb074-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="fb074-121">您的國家/地區必須要有一個位置 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="fb074-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="fb074-122">若要建立新的 MPN 位置，請閱讀下方的「新增 MPN 位置」。</span><span class="sxs-lookup"><span data-stu-id="fb074-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="fb074-123">若要建立新的 CSP 間接轉銷商註冊，請參閱 [使用間接提供者的工作](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="fb074-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="fb074-124">請記得 **使用新的 CSP 帳戶\*\*\*\*新** 的認證登入。</span><span class="sxs-lookup"><span data-stu-id="fb074-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="fb074-125">請不要使用現有認證，因為合作夥伴中心會將您識別為已擁有帳戶。</span><span class="sxs-lookup"><span data-stu-id="fb074-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="fb074-126">接受 Microsoft 合作夥伴合約並啟用帳戶。</span><span class="sxs-lookup"><span data-stu-id="fb074-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="fb074-127">如果您想要註冊為直接帳單合作夥伴，請閱讀 [直接帳單合作夥伴的需求](direct-partner-new-requirements.md)</span><span class="sxs-lookup"><span data-stu-id="fb074-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="fb074-128">查看您的 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="fb074-128">View your MPN locations</span></span>

1. <span data-ttu-id="fb074-129">使用您的 MPN 帳號憑證登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home) 。</span><span class="sxs-lookup"><span data-stu-id="fb074-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="fb074-130"> (您的 MPN 認證可能與您的 CSP 認證不同) </span><span class="sxs-lookup"><span data-stu-id="fb074-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="fb074-131">從 [ **設定** ] 圖示，選取 [ **帳戶設定**]、[ **組織設定檔**]、[ **法律**]。</span><span class="sxs-lookup"><span data-stu-id="fb074-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="fb074-132">在 [ **夥伴** ] 索引標籤上，確認沒有橫幅錯誤訊息要求您修正從 PMC 遷移的位置。</span><span class="sxs-lookup"><span data-stu-id="fb074-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="fb074-133">如果有，請遵循指示並修正這些位置。</span><span class="sxs-lookup"><span data-stu-id="fb074-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="fb074-134">如果沒有錯誤訊息，請從 [  **設定**] 中選取 [  **帳戶設定**]、[ **組織設定檔**]、[ **識別碼**]。</span><span class="sxs-lookup"><span data-stu-id="fb074-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="fb074-135">找出類型為 "Location" 的 MPN 識別碼，此識別碼符合此 CSP 帳戶的國家/地區，並使用它來搜尋下列專案並完成關聯。</span><span class="sxs-lookup"><span data-stu-id="fb074-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="fb074-136">如果找不到符合您想要使用之 CSP 帳戶的位置 MPN 識別碼，您可以新增新的位置，以建立新的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="fb074-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="fb074-137">請參閱下方 **的新增 MPN 位置** 。</span><span class="sxs-lookup"><span data-stu-id="fb074-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="fb074-138">新增 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="fb074-138">Add an MPN location</span></span>

1. <span data-ttu-id="fb074-139">使用合作夥伴中心中的 MPN 帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="fb074-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fb074-140"> (您的 MPN 認證可能與您) 的 CSP 認證不同。</span><span class="sxs-lookup"><span data-stu-id="fb074-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fb074-141">MPN 帳戶應具備全域管理員或帳戶系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="fb074-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="fb074-142">從 [ **設定] 圖示** 選取 **帳戶設定** ，然後選取 [ **組織設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="fb074-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="fb074-143">選取 [ **法律聲明** ]，然後在 [ **夥伴** ] 索引標籤上，選取 [ **商務位置]，** 然後按一下 [ **新增位置]。**</span><span class="sxs-lookup"><span data-stu-id="fb074-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="fb074-144">提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和連絡人。</span><span class="sxs-lookup"><span data-stu-id="fb074-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="fb074-145">按一下 [ **新增位置**]。</span><span class="sxs-lookup"><span data-stu-id="fb074-145">Click **Add location**.</span></span> <span data-ttu-id="fb074-146">這會為新的位置建立新的 MPN 識別碼，您可以將其用於 CSP 交易和獎勵。</span><span class="sxs-lookup"><span data-stu-id="fb074-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新增法律聲明企業":::

> [!NOTE]
> <span data-ttu-id="fb074-148">在合作夥伴中心中加入位置之後，您就無法將它移除。</span><span class="sxs-lookup"><span data-stu-id="fb074-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="fb074-149">如果您已使用正確的 MPN 識別碼來登入，您會在合作夥伴中心的左側功能表中看到 **MPN**。</span><span class="sxs-lookup"><span data-stu-id="fb074-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="fb074-150">刪除位置</span><span class="sxs-lookup"><span data-stu-id="fb074-150">Delete a location</span></span>

<span data-ttu-id="fb074-151">若要從您的帳戶刪除位置，您必須聯絡 [合作夥伴支援](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)。</span><span class="sxs-lookup"><span data-stu-id="fb074-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="fb074-152">請確定您瞭解此動作的影響。</span><span class="sxs-lookup"><span data-stu-id="fb074-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="fb074-153">無法抓取已刪除的位置，且系結至該特定 MPN 識別碼的任何系結，將無法再辨識或對您的公司有效。</span><span class="sxs-lookup"><span data-stu-id="fb074-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="fb074-154">變更合作夥伴通用帳戶的國家/地區</span><span class="sxs-lookup"><span data-stu-id="fb074-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="fb074-155">使用合作夥伴中心中的 MPN 帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="fb074-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fb074-156"> (您的 MPN 認證可能與您) 的 CSP 認證不同。</span><span class="sxs-lookup"><span data-stu-id="fb074-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fb074-157">MPN 帳戶應具備全域管理員或帳戶系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="fb074-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="fb074-158">在 [ **夥伴** ] 索引標籤上，移至 [ **商務位置** ] 並檢查位置清單，以確保列出您想要的位置，以列出您的法律實體。</span><span class="sxs-lookup"><span data-stu-id="fb074-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="fb074-159">若要新增位置，請按一下 [ **新增位置**]，然後在 [飛出] 中提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="fb074-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="fb074-160">選取 [**國家/地區**] 下拉式清單旁的 [**變更您的國家**/地區]，然後依照步驟執行。</span><span class="sxs-lookup"><span data-stu-id="fb074-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法律聲明商務設定檔資料飛出":::

5. <span data-ttu-id="fb074-162">按一下 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="fb074-162">Click **Save**.</span></span>

6. <span data-ttu-id="fb074-163">MPN global account country 將會變更為新的法律國家/地區。</span><span class="sxs-lookup"><span data-stu-id="fb074-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="fb074-164">後續步驟</span><span class="sxs-lookup"><span data-stu-id="fb074-164">Next steps</span></span>

- <span data-ttu-id="fb074-165">了解[驗證程序](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="fb074-165">Learn about the [verification process](verification-responses.md).</span></span>
