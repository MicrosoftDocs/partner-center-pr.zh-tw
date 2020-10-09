---
title: 管理合作夥伴帳戶中的位置
ms.topic: article
ms.date: 10/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何新增位置，以及如何在獎勵計畫、雲端解決方案提供者業務、訂閱和其他交易中使用 MPN 識別碼。
author: vinayks
ms.author: vinayks
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c9bc3ffc09b657ab6e3e7e2dcda576898c96803d
ms.sourcegitcommit: d9c7890520ecd37a7651e976d540cfe65c51be54
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/02/2020
ms.locfileid: "91663891"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="e6204-103">管理您的 MPN 帳戶位置並新增位置</span><span class="sxs-lookup"><span data-stu-id="e6204-103">Manage your MPN account locations and add a new location</span></span>

<span data-ttu-id="e6204-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="e6204-104">**Applies to**</span></span>

- <span data-ttu-id="e6204-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e6204-105">Partner Center</span></span>

<span data-ttu-id="e6204-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="e6204-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e6204-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="e6204-107">Global admin</span></span>
- <span data-ttu-id="e6204-108">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="e6204-108">Account admin</span></span>

<span data-ttu-id="e6204-109">位置 MPN 識別碼可識別公司的每個特定位置。</span><span class="sxs-lookup"><span data-stu-id="e6204-109">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="e6204-110">您可以使用位置 MPN 識別碼來註冊獎勵計畫、交易雲端解決方案提供者 (CSP) 業務以及其他商業交易。</span><span class="sxs-lookup"><span data-stu-id="e6204-110">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="e6204-111">全域 MPN 識別碼可用於非交易式活動，例如支援要求。</span><span class="sxs-lookup"><span data-stu-id="e6204-111">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="e6204-112">以下為典型的案例：</span><span class="sxs-lookup"><span data-stu-id="e6204-112">The following is a typical scenario:</span></span>

<span data-ttu-id="e6204-113">Contoso 在英國有其合作夥伴通用帳戶 (PGA) 位置。</span><span class="sxs-lookup"><span data-stu-id="e6204-113">Contoso has its Partner global account (PGA) location in the UK.</span></span> <span data-ttu-id="e6204-114">這是其已註冊的合法公司，而且此公司有一個用於管理所有非交易業務的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="e6204-114">This is their registered legal business, and it has one MPN ID used for managing all non-transactional business.</span></span> <span data-ttu-id="e6204-115">Contoso 在英國、法國和美國的其他位置也有相當於分公司或部門的合作夥伴位置帳戶 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="e6204-115">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="e6204-116">在 MPN 帳戶結構中，這些 PLA 會以唯一的位置 MPN 識別碼來表示。</span><span class="sxs-lookup"><span data-stu-id="e6204-116">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="e6204-117">PLA 可用於交易業務，例如 CSP 或獎勵計畫。</span><span class="sxs-lookup"><span data-stu-id="e6204-117">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="e6204-118">支出會繫結至特定位置。</span><span class="sxs-lookup"><span data-stu-id="e6204-118">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="e6204-119">CSP 租用戶與 MPN 位置識別碼之間有 1 對 1 的關聯性。</span><span class="sxs-lookup"><span data-stu-id="e6204-119">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/accountsettings/accountstructure.png" alt-text="MPN 位置的結構":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a><span data-ttu-id="e6204-121">為 CSP 業務新增位置的必要條件</span><span class="sxs-lookup"><span data-stu-id="e6204-121">Prerequisites in order to add a new location for a CSP business</span></span>

<span data-ttu-id="e6204-122">若要新增 CSP 業務位置，有幾個必要條件：</span><span class="sxs-lookup"><span data-stu-id="e6204-122">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="e6204-123">您必須在想要執行業務的國家/地區中擁有位置 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="e6204-123">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="e6204-124">您在尚未註冊 CSP 的業務區域中需要新的 Azure AD 租用戶。</span><span class="sxs-lookup"><span data-stu-id="e6204-124">You need a new Azure AD tenant in the region of business which is not already enrolled into CSP.</span></span> <span data-ttu-id="e6204-125">當您註冊 CSP 時，請建立此項目。</span><span class="sxs-lookup"><span data-stu-id="e6204-125">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="e6204-126">使用新的 AAD 租用戶在區域中註冊 CSP 計畫。</span><span class="sxs-lookup"><span data-stu-id="e6204-126">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="e6204-127">提供合法公司的詳細資料，包括合法公司名稱、地址、主要連絡人詳細資料。</span><span class="sxs-lookup"><span data-stu-id="e6204-127">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="e6204-128">此帳戶會進行驗證，因此請務必新增有效的資訊。</span><span class="sxs-lookup"><span data-stu-id="e6204-128">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="e6204-129">請記得使用**新的** Azure AD 租用戶的**新**認證來登入。</span><span class="sxs-lookup"><span data-stu-id="e6204-129">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="e6204-130">請不要使用現有認證，因為合作夥伴中心會將您識別為已擁有帳戶。</span><span class="sxs-lookup"><span data-stu-id="e6204-130">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="e6204-131">接受 Microsoft 合作夥伴合約並啟用帳戶。</span><span class="sxs-lookup"><span data-stu-id="e6204-131">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-a-location"></a><span data-ttu-id="e6204-132">新增位置</span><span class="sxs-lookup"><span data-stu-id="e6204-132">Add a location</span></span>

1. <span data-ttu-id="e6204-133">從 [設定] 圖示選取 [合作夥伴設定]。</span><span class="sxs-lookup"><span data-stu-id="e6204-133">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="e6204-134">選取 [位置]。</span><span class="sxs-lookup"><span data-stu-id="e6204-134">Select **Locations.**</span></span>

3. <span data-ttu-id="e6204-135">選取 [新增位置]。</span><span class="sxs-lookup"><span data-stu-id="e6204-135">Select **Add a location**.</span></span>  

4. <span data-ttu-id="e6204-136">在 [新增位置] 頁面上，插入要新增至公司之位置的地址詳細資料，以及該位置的主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="e6204-136">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="e6204-137">在合作夥伴中心新增位置後，即無法將其移除。</span><span class="sxs-lookup"><span data-stu-id="e6204-137">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="e6204-138">變更全球合作夥伴帳戶位置</span><span class="sxs-lookup"><span data-stu-id="e6204-138">Change Global partner account location</span></span>

1. <span data-ttu-id="e6204-139">在 [位置] 頁面上檢查位置清單，以確定您要作為法律實體的位置已列出。</span><span class="sxs-lookup"><span data-stu-id="e6204-139">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="e6204-140">如果沒有，請新增它。</span><span class="sxs-lookup"><span data-stu-id="e6204-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 位置的結構":::

2. <span data-ttu-id="e6204-142">選取 [合作夥伴設定檔]，然後選取 [更新法定公司設定檔]。</span><span class="sxs-lookup"><span data-stu-id="e6204-142">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 位置的結構":::

3. <span data-ttu-id="e6204-144">選取區域和法律實體，然後加以**提交**。</span><span class="sxs-lookup"><span data-stu-id="e6204-144">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 位置的結構":::

## <a name="next-steps"></a><span data-ttu-id="e6204-146">後續步驟</span><span class="sxs-lookup"><span data-stu-id="e6204-146">Next steps</span></span>

- <span data-ttu-id="e6204-147">了解[驗證程序](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="e6204-147">Learn about the [verification process](verification-responses.md).</span></span>
