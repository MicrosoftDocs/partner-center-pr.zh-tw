---
title: 管理合作夥伴帳戶中的位置
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何新增位置，以及如何在獎勵計畫、雲端解決方案提供者業務、訂閱和其他交易中使用 MPN 識別碼。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925027"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="db0e7-103">管理您的 MPN 帳戶位置並新增位置</span><span class="sxs-lookup"><span data-stu-id="db0e7-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="db0e7-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="db0e7-104">**Appropriate roles**</span></span>

- <span data-ttu-id="db0e7-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="db0e7-105">Global admin</span></span>
- <span data-ttu-id="db0e7-106">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="db0e7-106">Account admin</span></span>

<span data-ttu-id="db0e7-107">位置 MPN 識別碼可識別公司的每個特定位置。</span><span class="sxs-lookup"><span data-stu-id="db0e7-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="db0e7-108">您可以使用位置 MPN 識別碼來註冊獎勵計畫、交易雲端解決方案提供者 (CSP) 業務以及其他商業交易。</span><span class="sxs-lookup"><span data-stu-id="db0e7-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="db0e7-109">全域 MPN 識別碼可用於非交易式活動，例如支援要求。</span><span class="sxs-lookup"><span data-stu-id="db0e7-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="db0e7-110">以下為典型的案例：</span><span class="sxs-lookup"><span data-stu-id="db0e7-110">The following is a typical scenario:</span></span>

<span data-ttu-id="db0e7-111">Contoso 在英國有其合作夥伴通用帳戶 (PGA)。</span><span class="sxs-lookup"><span data-stu-id="db0e7-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="db0e7-112">這是其已註冊的合法公司，而且有一個用於管理所有非交易業務的全域 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="db0e7-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="db0e7-113">Contoso 在英國、法國和美國的其他位置也有相當於分公司或部門的合作夥伴位置帳戶 (PLA)。</span><span class="sxs-lookup"><span data-stu-id="db0e7-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="db0e7-114">在 MPN 帳戶結構中，這些 PLA 會以唯一的位置 MPN 識別碼來表示。</span><span class="sxs-lookup"><span data-stu-id="db0e7-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="db0e7-115">PLA 可用於交易業務，例如 CSP 或獎勵計畫。</span><span class="sxs-lookup"><span data-stu-id="db0e7-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="db0e7-116">支出會繫結至特定位置。</span><span class="sxs-lookup"><span data-stu-id="db0e7-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="db0e7-117">CSP 租用戶與 MPN 位置識別碼之間有 1 對 1 的關聯性。</span><span class="sxs-lookup"><span data-stu-id="db0e7-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的結構":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="db0e7-119">為 CSP 商務新增帳戶的必要條件</span><span class="sxs-lookup"><span data-stu-id="db0e7-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="db0e7-120">若要加入新的 CSP 商務帳戶，請先確定您已滿足必要條件。</span><span class="sxs-lookup"><span data-stu-id="db0e7-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="db0e7-121">您的國家/地區必須要有一個位置 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="db0e7-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="db0e7-122">若要建立新的 MPN 位置，請閱讀下方的「新增 MPN 位置」。</span><span class="sxs-lookup"><span data-stu-id="db0e7-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="db0e7-123">若要建立新的 CSP 間接轉銷商註冊，請參閱 [使用間接提供者的工作](indirect-reseller-tasks-in-partner-center.md#get-started)</span><span class="sxs-lookup"><span data-stu-id="db0e7-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="db0e7-124">請記得 **使用新的 CSP 帳戶\*\*\*\*新** 的認證登入。</span><span class="sxs-lookup"><span data-stu-id="db0e7-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="db0e7-125">請不要使用現有認證，因為合作夥伴中心會將您識別為已擁有帳戶。</span><span class="sxs-lookup"><span data-stu-id="db0e7-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="db0e7-126">接受 Microsoft 合作夥伴合約並啟用帳戶。</span><span class="sxs-lookup"><span data-stu-id="db0e7-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="db0e7-127">新增 MPN 位置</span><span class="sxs-lookup"><span data-stu-id="db0e7-127">Add an MPN location</span></span>

1. <span data-ttu-id="db0e7-128">使用合作夥伴中心中的 MPN 帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="db0e7-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="db0e7-129"> (您的 MPN 認證可能與您) 的 CSP 認證不同。</span><span class="sxs-lookup"><span data-stu-id="db0e7-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="db0e7-130">MPN 帳戶應具備全域管理員或帳戶系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="db0e7-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="db0e7-131">從 [ **設定] 圖示** 選取 **帳戶設定** ，然後選取 [ **組織設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="db0e7-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="db0e7-132">選取 [ **法律聲明** ]，然後在 [ **夥伴** ] 索引標籤上，選取 [ **商務位置]，** 然後按一下 [ **新增位置]。**</span><span class="sxs-lookup"><span data-stu-id="db0e7-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="db0e7-133">提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和連絡人。</span><span class="sxs-lookup"><span data-stu-id="db0e7-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="db0e7-134">按一下 [ **新增位置**]。</span><span class="sxs-lookup"><span data-stu-id="db0e7-134">Click **Add location**.</span></span> <span data-ttu-id="db0e7-135">這會為新的位置建立新的 MPN 識別碼，您可以將其用於 CSP 交易和獎勵。</span><span class="sxs-lookup"><span data-stu-id="db0e7-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新增法律聲明企業":::

> [!NOTE]
> <span data-ttu-id="db0e7-137">在合作夥伴中心新增位置後，即無法將其移除。</span><span class="sxs-lookup"><span data-stu-id="db0e7-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="db0e7-138">如果您已使用正確的 MPN 識別碼來登入，您會在合作夥伴中心的左側功能表中看到 **MPN**。</span><span class="sxs-lookup"><span data-stu-id="db0e7-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="db0e7-139">變更合作夥伴通用帳戶的國家/地區</span><span class="sxs-lookup"><span data-stu-id="db0e7-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="db0e7-140">使用合作夥伴中心中的 MPN 帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="db0e7-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="db0e7-141"> (您的 MPN 認證可能與您) 的 CSP 認證不同。</span><span class="sxs-lookup"><span data-stu-id="db0e7-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="db0e7-142">MPN 帳戶應具備全域管理員或帳戶系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="db0e7-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="db0e7-143">在 [ **夥伴** ] 索引標籤上，移至 [ **商務位置** ] 並檢查位置清單，以確保列出您想要的位置，以列出您的法律實體。</span><span class="sxs-lookup"><span data-stu-id="db0e7-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="db0e7-144">若要新增位置，請按一下 [ **新增位置**]，然後在 [飛出] 中提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和主要連絡人。</span><span class="sxs-lookup"><span data-stu-id="db0e7-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="db0e7-145">選取 [**國家/地區**] 下拉式清單旁的 [**變更您的國家**/地區]，然後依照步驟執行。</span><span class="sxs-lookup"><span data-stu-id="db0e7-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法律聲明商務設定檔資料飛出":::

5. <span data-ttu-id="db0e7-147">按一下 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="db0e7-147">Click **Save**.</span></span>

6. <span data-ttu-id="db0e7-148">MPN global account country 將會變更為新的法律國家/地區。</span><span class="sxs-lookup"><span data-stu-id="db0e7-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="db0e7-149">後續步驟</span><span class="sxs-lookup"><span data-stu-id="db0e7-149">Next steps</span></span>

- <span data-ttu-id="db0e7-150">了解[驗證程序](verification-responses.md)。</span><span class="sxs-lookup"><span data-stu-id="db0e7-150">Learn about the [verification process](verification-responses.md).</span></span>
