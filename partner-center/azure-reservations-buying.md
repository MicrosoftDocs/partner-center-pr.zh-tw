---
title: 代表您的客戶購買 Microsoft Azure Reservations | 合作夥伴中心
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何在合作夥伴中心代表您的客戶購買或購買 Azure 保留。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, 管理, 計費, 購買
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2a7e249ddae377acb742d78cf505aa7b97cf84c4
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253234"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a><span data-ttu-id="1413c-104">代表您的客戶在合作夥伴中心購買 Microsoft Azure 保留</span><span class="sxs-lookup"><span data-stu-id="1413c-104">Buy Microsoft Azure reservations on behalf of your customers in Partner Center</span></span> 

<span data-ttu-id="1413c-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="1413c-105">**Applies to**</span></span>

-  <span data-ttu-id="1413c-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="1413c-106">Partner Center</span></span>
-  <span data-ttu-id="1413c-107">Microsoft Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="1413c-107">Microsoft Azure portal</span></span>
-  <span data-ttu-id="1413c-108">雲端解決方案提供者中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="1413c-108">Partners in CSP</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="1413c-109">開始之前</span><span class="sxs-lookup"><span data-stu-id="1413c-109">Before you begin</span></span>

<span data-ttu-id="1413c-110">請先參閱下面的重要資訊，然後再代表您的客戶購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="1413c-110">Review the important information below before you buy Azure reservations on behalf of your customers.</span></span>

- <span data-ttu-id="1413c-111">如果您的客戶簽署新的 Microsoft 客戶合約時，[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)，您必須在 azure 方案下購買 azure 保留。</span><span class="sxs-lookup"><span data-stu-id="1413c-111">If and when your customer signs the new Microsoft Customer Agreement [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md), you must purchase Azure reservations under the Azure plan.</span></span> <span data-ttu-id="1413c-112">如需詳細資訊，請參閱[購買 Azure 方案](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="1413c-112">For more information, read [Purchase Azure Plan](purchase-azure-plan.md).</span></span>

-   <span data-ttu-id="1413c-113">在您代表客戶購買保留區之前，客戶必須已擁有有效的 Azure 訂閱</span><span class="sxs-lookup"><span data-stu-id="1413c-113">Customers must already have an active Azure subscription before you can purchase reservations on their behalf</span></span>
  
-   <span data-ttu-id="1413c-114">軟體訂用帳戶成本（例如 SQL Database 或 SUSE Linux 軟體）不包含在 Azure 保留價格中</span><span class="sxs-lookup"><span data-stu-id="1413c-114">Software subscription costs such as SQL Database or SUSE Linux software are not included in Azure reservation prices</span></span>

-   <span data-ttu-id="1413c-115">除非您的位置是巴西，否則 Microsoft 的商業定價不包含稅金。</span><span class="sxs-lookup"><span data-stu-id="1413c-115">Microsoft's commercial pricing to you does not include taxes, unless your location is Brazil.</span></span> <span data-ttu-id="1413c-116">如果您的地點是巴西，則您的商業價格包含適當的稅額</span><span class="sxs-lookup"><span data-stu-id="1413c-116">If your location is Brazil, the commercial price to you includes the appropriate taxes</span></span> 
 
-   <span data-ttu-id="1413c-117">銷售人員和技術支援中心需能代表客戶明確的存取 Azure 訂閱，以便在 Azure 入口網站與檔案支援要求中購買或管理訂閱，包括換貨與退款</span><span class="sxs-lookup"><span data-stu-id="1413c-117">Sales and help desk agents need explicit access to the Azure subscription so they can buy or manage it in the Azure portal and file support requests, including for exchanges and refunds, on behalf of the customer</span></span>  

-   <span data-ttu-id="1413c-118">如果您是間接提供者，而且您透過 Azure 入口網站購買 Azure 保留專案，則會從您選取的 Azure CSP 訂用帳戶繼承「記錄」（間接轉銷商）的夥伴。</span><span class="sxs-lookup"><span data-stu-id="1413c-118">If you're an indirect provider and you buy Azure reservations through the Azure portal, the Partner on Record (indirect reseller) is inherited from the Azure CSP subscription you select.</span></span> 

-   <span data-ttu-id="1413c-119">購買後無法變更 Azure 保留的記錄合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="1413c-119">The Partner of Record for Azure reservations cannot be changed post-purchase.</span></span> <span data-ttu-id="1413c-120">您可以取消現有的保留區，並透過新的記錄可查夥伴購買新的保留區。</span><span class="sxs-lookup"><span data-stu-id="1413c-120">You can cancel the existing reservation and purchase a new one with the new Partner on Record.</span></span> 

-   <span data-ttu-id="1413c-121">如果客戶想將 Azure 訂閱從直接或 EA 轉移至雲端解決方案提供者，保留區無法轉移。</span><span class="sxs-lookup"><span data-stu-id="1413c-121">If a customer wants to transfer an Azure subscription from Direct or EA to CSP, reservations do not get transferred.</span></span> 

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="1413c-122">Azure 保留無法使用的市場</span><span class="sxs-lookup"><span data-stu-id="1413c-122">Azure reservations unavailable markets</span></span>

>[!IMPORTANT] 
><span data-ttu-id="1413c-123">下列市場*不*提供 Azure 保留：</span><span class="sxs-lookup"><span data-stu-id="1413c-123">Azure reservations *are not* available in the following markets:</span></span>  
>  
> | <span data-ttu-id="1413c-124">無法使用的市場</span><span class="sxs-lookup"><span data-stu-id="1413c-124">Unavailable markets</span></span> | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="1413c-125">奧蘭島</span><span class="sxs-lookup"><span data-stu-id="1413c-125">Åland Islands</span></span>     | <span data-ttu-id="1413c-126">格陵蘭</span><span class="sxs-lookup"><span data-stu-id="1413c-126">Greenland</span></span>     | <span data-ttu-id="1413c-127">巴布亞紐幾內亞</span><span class="sxs-lookup"><span data-stu-id="1413c-127">Papua New Guinea</span></span>     |
> | <span data-ttu-id="1413c-128">美屬薩摩亞</span><span class="sxs-lookup"><span data-stu-id="1413c-128">American Samoa</span></span>     | <span data-ttu-id="1413c-129">格瑞那達</span><span class="sxs-lookup"><span data-stu-id="1413c-129">Grenada</span></span>     | <span data-ttu-id="1413c-130">皮特康群島</span><span class="sxs-lookup"><span data-stu-id="1413c-130">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="1413c-131">安道爾</span><span class="sxs-lookup"><span data-stu-id="1413c-131">Andorra</span></span>     | <span data-ttu-id="1413c-132">哥德普洛</span><span class="sxs-lookup"><span data-stu-id="1413c-132">Guadeloupe</span></span>     | <span data-ttu-id="1413c-133">留尼旺</span><span class="sxs-lookup"><span data-stu-id="1413c-133">Reunion</span></span>     |
> | <span data-ttu-id="1413c-134">安圭拉</span><span class="sxs-lookup"><span data-stu-id="1413c-134">Anguilla</span></span>     | <span data-ttu-id="1413c-135">關島</span><span class="sxs-lookup"><span data-stu-id="1413c-135">Guam</span></span>     | <span data-ttu-id="1413c-136">沙巴</span><span class="sxs-lookup"><span data-stu-id="1413c-136">Saba</span></span>   |
> | <span data-ttu-id="1413c-137">南極大陸</span><span class="sxs-lookup"><span data-stu-id="1413c-137">Antarctica</span></span>     | <span data-ttu-id="1413c-138">根息</span><span class="sxs-lookup"><span data-stu-id="1413c-138">Guernsey</span></span>     | <span data-ttu-id="1413c-139">聖巴瑟米</span><span class="sxs-lookup"><span data-stu-id="1413c-139">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="1413c-140">安地卡及巴布達</span><span class="sxs-lookup"><span data-stu-id="1413c-140">Antigua and Barbuda</span></span>       | <span data-ttu-id="1413c-141">幾內亞</span><span class="sxs-lookup"><span data-stu-id="1413c-141">Guinea</span></span>     | <span data-ttu-id="1413c-142">聖露西亞</span><span class="sxs-lookup"><span data-stu-id="1413c-142">Saint Lucia</span></span>   |
> | <span data-ttu-id="1413c-143">阿路巴</span><span class="sxs-lookup"><span data-stu-id="1413c-143">Aruba</span></span>       | <span data-ttu-id="1413c-144">幾內亞比索</span><span class="sxs-lookup"><span data-stu-id="1413c-144">Guinea-Bissau</span></span>     | <span data-ttu-id="1413c-145">聖馬丁</span><span class="sxs-lookup"><span data-stu-id="1413c-145">Saint Martin</span></span>   |
> | <span data-ttu-id="1413c-146">亞塞拜然</span><span class="sxs-lookup"><span data-stu-id="1413c-146">Azerbaijan</span></span>       | <span data-ttu-id="1413c-147">蓋亞納</span><span class="sxs-lookup"><span data-stu-id="1413c-147">Guyana</span></span>     | <span data-ttu-id="1413c-148">聖匹島</span><span class="sxs-lookup"><span data-stu-id="1413c-148">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="1413c-149">貝南</span><span class="sxs-lookup"><span data-stu-id="1413c-149">Benin</span></span>     | <span data-ttu-id="1413c-150">海地</span><span class="sxs-lookup"><span data-stu-id="1413c-150">Haiti</span></span>       | <span data-ttu-id="1413c-151">聖文森及格瑞那丁</span><span class="sxs-lookup"><span data-stu-id="1413c-151">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="1413c-152">不丹</span><span class="sxs-lookup"><span data-stu-id="1413c-152">Bhutan</span></span>     | <span data-ttu-id="1413c-153">赫德島及麥當勞群島</span><span class="sxs-lookup"><span data-stu-id="1413c-153">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="1413c-154">薩摩亞獨立國</span><span class="sxs-lookup"><span data-stu-id="1413c-154">Samoa</span></span>     |
> | <span data-ttu-id="1413c-155">波奈</span><span class="sxs-lookup"><span data-stu-id="1413c-155">Bonaire</span></span>     | <span data-ttu-id="1413c-156">曼城島</span><span class="sxs-lookup"><span data-stu-id="1413c-156">Isle of Man</span></span>     | <span data-ttu-id="1413c-157">聖馬利諾</span><span class="sxs-lookup"><span data-stu-id="1413c-157">San Marino</span></span>     |
> | <span data-ttu-id="1413c-158">布威島</span><span class="sxs-lookup"><span data-stu-id="1413c-158">Bouvet Island</span></span>     | <span data-ttu-id="1413c-159">Jan 馬延</span><span class="sxs-lookup"><span data-stu-id="1413c-159">Jan Mayen</span></span>     | <span data-ttu-id="1413c-160">聖多美普林西比</span><span class="sxs-lookup"><span data-stu-id="1413c-160">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="1413c-161">英屬印度洋領土</span><span class="sxs-lookup"><span data-stu-id="1413c-161">British Indian Ocean Territory</span></span>       | <span data-ttu-id="1413c-162">澤西島</span><span class="sxs-lookup"><span data-stu-id="1413c-162">Jersey</span></span>     | <span data-ttu-id="1413c-163">塞席爾</span><span class="sxs-lookup"><span data-stu-id="1413c-163">Seychelles</span></span>   |
> | <span data-ttu-id="1413c-164">英屬維爾京群島</span><span class="sxs-lookup"><span data-stu-id="1413c-164">British Virgin Islands</span></span>     | <span data-ttu-id="1413c-165">吉里巴斯</span><span class="sxs-lookup"><span data-stu-id="1413c-165">Kiribati</span></span>       | <span data-ttu-id="1413c-166">獅子山</span><span class="sxs-lookup"><span data-stu-id="1413c-166">Sierra Leone</span></span>   |
> | <span data-ttu-id="1413c-167">布吉納法索</span><span class="sxs-lookup"><span data-stu-id="1413c-167">Burkina Faso</span></span>     | <span data-ttu-id="1413c-168">科索沃</span><span class="sxs-lookup"><span data-stu-id="1413c-168">Kosovo</span></span>     | <span data-ttu-id="1413c-169">聖尤斯特斯</span><span class="sxs-lookup"><span data-stu-id="1413c-169">Sint Eustatius</span></span>     |
> | <span data-ttu-id="1413c-170">蒲隆地</span><span class="sxs-lookup"><span data-stu-id="1413c-170">Burundi</span></span>     | <span data-ttu-id="1413c-171">寮國</span><span class="sxs-lookup"><span data-stu-id="1413c-171">Laos</span></span>     | <span data-ttu-id="1413c-172">荷屬聖馬丁</span><span class="sxs-lookup"><span data-stu-id="1413c-172">Sint Maarten</span></span>     |
> | <span data-ttu-id="1413c-173">柬埔寨</span><span class="sxs-lookup"><span data-stu-id="1413c-173">Cambodia</span></span>     | <span data-ttu-id="1413c-174">賴索托</span><span class="sxs-lookup"><span data-stu-id="1413c-174">Lesotho</span></span>     | <span data-ttu-id="1413c-175">索羅門群島</span><span class="sxs-lookup"><span data-stu-id="1413c-175">Solomon Islands</span></span>     |
> | <span data-ttu-id="1413c-176">中非共和國</span><span class="sxs-lookup"><span data-stu-id="1413c-176">Central African Republic</span></span>     | <span data-ttu-id="1413c-177">賴比瑞亞</span><span class="sxs-lookup"><span data-stu-id="1413c-177">Liberia</span></span>     | <span data-ttu-id="1413c-178">索馬利亞</span><span class="sxs-lookup"><span data-stu-id="1413c-178">Somalia</span></span>     |
> | <span data-ttu-id="1413c-179">查德</span><span class="sxs-lookup"><span data-stu-id="1413c-179">Chad</span></span>     | <span data-ttu-id="1413c-180">馬達加斯加</span><span class="sxs-lookup"><span data-stu-id="1413c-180">Madagascar</span></span>     | <span data-ttu-id="1413c-181">南喬治亞與南三明治群島</span><span class="sxs-lookup"><span data-stu-id="1413c-181">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="1413c-182">中國</span><span class="sxs-lookup"><span data-stu-id="1413c-182">China</span></span>     | <span data-ttu-id="1413c-183">馬拉威</span><span class="sxs-lookup"><span data-stu-id="1413c-183">Malawi</span></span>     | <span data-ttu-id="1413c-184">南蘇丹</span><span class="sxs-lookup"><span data-stu-id="1413c-184">South Sudan</span></span>     |
> | <span data-ttu-id="1413c-185">聖誕島</span><span class="sxs-lookup"><span data-stu-id="1413c-185">Christmas Island</span></span>     | <span data-ttu-id="1413c-186">馬爾地夫</span><span class="sxs-lookup"><span data-stu-id="1413c-186">Maldives</span></span>     | <span data-ttu-id="1413c-187">聖赫勒拿、阿森松、特裡斯坦達庫尼亞群島</span><span class="sxs-lookup"><span data-stu-id="1413c-187">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="1413c-188">可可斯群島</span><span class="sxs-lookup"><span data-stu-id="1413c-188">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="1413c-189">馬利</span><span class="sxs-lookup"><span data-stu-id="1413c-189">Mali</span></span>     | <span data-ttu-id="1413c-190">蘇利南</span><span class="sxs-lookup"><span data-stu-id="1413c-190">Suriname</span></span>     |
> | <span data-ttu-id="1413c-191">葛摩</span><span class="sxs-lookup"><span data-stu-id="1413c-191">Comoros</span></span>     | <span data-ttu-id="1413c-192">馬紹爾群島</span><span class="sxs-lookup"><span data-stu-id="1413c-192">Marshall Islands</span></span>     | <span data-ttu-id="1413c-193">冷岸</span><span class="sxs-lookup"><span data-stu-id="1413c-193">Svalbard</span></span>     |
> | <span data-ttu-id="1413c-194">剛果共和國</span><span class="sxs-lookup"><span data-stu-id="1413c-194">Congo</span></span>     | <span data-ttu-id="1413c-195">馬丁尼克</span><span class="sxs-lookup"><span data-stu-id="1413c-195">Martinique</span></span>     | <span data-ttu-id="1413c-196">史瓦濟蘭</span><span class="sxs-lookup"><span data-stu-id="1413c-196">Swaziland</span></span>     |
> | <span data-ttu-id="1413c-197">剛果民主共和國 (DRC)</span><span class="sxs-lookup"><span data-stu-id="1413c-197">Congo (DRC)</span></span>     | <span data-ttu-id="1413c-198">茅利塔尼亞</span><span class="sxs-lookup"><span data-stu-id="1413c-198">Mauritania</span></span>     | <span data-ttu-id="1413c-199">東帝汶</span><span class="sxs-lookup"><span data-stu-id="1413c-199">Timor-Leste</span></span>   |
> | <span data-ttu-id="1413c-200">柯克群島</span><span class="sxs-lookup"><span data-stu-id="1413c-200">Cook Islands</span></span>     | <span data-ttu-id="1413c-201">馬約特島</span><span class="sxs-lookup"><span data-stu-id="1413c-201">Mayotte</span></span>     | <span data-ttu-id="1413c-202">多哥</span><span class="sxs-lookup"><span data-stu-id="1413c-202">Togo</span></span>   |
> | <span data-ttu-id="1413c-203">吉布地</span><span class="sxs-lookup"><span data-stu-id="1413c-203">Djibouti</span></span>     | <span data-ttu-id="1413c-204">密克羅尼西亞</span><span class="sxs-lookup"><span data-stu-id="1413c-204">Micronesia</span></span>     | <span data-ttu-id="1413c-205">托克勞群島</span><span class="sxs-lookup"><span data-stu-id="1413c-205">Tokelau</span></span>   |
> | <span data-ttu-id="1413c-206">多米尼克</span><span class="sxs-lookup"><span data-stu-id="1413c-206">Dominica</span></span>     | <span data-ttu-id="1413c-207">蒙特色拉特島</span><span class="sxs-lookup"><span data-stu-id="1413c-207">Montserrat</span></span>     | <span data-ttu-id="1413c-208">東加</span><span class="sxs-lookup"><span data-stu-id="1413c-208">Tonga</span></span>   |
> | <span data-ttu-id="1413c-209">赤道幾內亞</span><span class="sxs-lookup"><span data-stu-id="1413c-209">Equatorial Guinea</span></span>     | <span data-ttu-id="1413c-210">莫三比克</span><span class="sxs-lookup"><span data-stu-id="1413c-210">Mozambique</span></span>     | <span data-ttu-id="1413c-211">土克斯及開科斯群島</span><span class="sxs-lookup"><span data-stu-id="1413c-211">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="1413c-212">厄利垂亞</span><span class="sxs-lookup"><span data-stu-id="1413c-212">Eritrea</span></span>     | <span data-ttu-id="1413c-213">緬甸文</span><span class="sxs-lookup"><span data-stu-id="1413c-213">Myanmar</span></span>     | <span data-ttu-id="1413c-214">吐瓦魯</span><span class="sxs-lookup"><span data-stu-id="1413c-214">Tuvalu</span></span>   |
> | <span data-ttu-id="1413c-215">福克蘭群島</span><span class="sxs-lookup"><span data-stu-id="1413c-215">Falkland Islands</span></span>     | <span data-ttu-id="1413c-216">諾魯</span><span class="sxs-lookup"><span data-stu-id="1413c-216">Nauru</span></span>     | <span data-ttu-id="1413c-217">美國外島</span><span class="sxs-lookup"><span data-stu-id="1413c-217">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="1413c-218">法屬圭亞那</span><span class="sxs-lookup"><span data-stu-id="1413c-218">French Guiana</span></span>     | <span data-ttu-id="1413c-219">新喀里多尼亞群島</span><span class="sxs-lookup"><span data-stu-id="1413c-219">New Caledonia</span></span>     | <span data-ttu-id="1413c-220">萬那杜</span><span class="sxs-lookup"><span data-stu-id="1413c-220">Vanuatu</span></span>   |
> | <span data-ttu-id="1413c-221">法屬玻里尼西亞</span><span class="sxs-lookup"><span data-stu-id="1413c-221">French Polynesia</span></span>     | <span data-ttu-id="1413c-222">尼日</span><span class="sxs-lookup"><span data-stu-id="1413c-222">Niger</span></span>     | <span data-ttu-id="1413c-223">梵蒂岡</span><span class="sxs-lookup"><span data-stu-id="1413c-223">Vatican City</span></span>   |
> | <span data-ttu-id="1413c-224">法屬南半球領土</span><span class="sxs-lookup"><span data-stu-id="1413c-224">French Southern Territories</span></span>     | <span data-ttu-id="1413c-225">紐威島</span><span class="sxs-lookup"><span data-stu-id="1413c-225">Niue</span></span>     | <span data-ttu-id="1413c-226">瓦利斯及福杜納</span><span class="sxs-lookup"><span data-stu-id="1413c-226">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="1413c-227">加彭</span><span class="sxs-lookup"><span data-stu-id="1413c-227">Gabon</span></span>     | <span data-ttu-id="1413c-228">諾福克島</span><span class="sxs-lookup"><span data-stu-id="1413c-228">Norfolk Island</span></span>     | <span data-ttu-id="1413c-229">葉門</span><span class="sxs-lookup"><span data-stu-id="1413c-229">Yemen</span></span>   |
> | <span data-ttu-id="1413c-230">甘比亞</span><span class="sxs-lookup"><span data-stu-id="1413c-230">Gambia</span></span>     | <span data-ttu-id="1413c-231">北馬里安納群島</span><span class="sxs-lookup"><span data-stu-id="1413c-231">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="1413c-232">直布羅陀</span><span class="sxs-lookup"><span data-stu-id="1413c-232">Gibraltar</span></span>     | <span data-ttu-id="1413c-233">帛琉</span><span class="sxs-lookup"><span data-stu-id="1413c-233">Palau</span></span>       |    |

## <a name="purchase-azure-reservations"></a><span data-ttu-id="1413c-234">購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="1413c-234">Purchase Azure reservations</span></span>

<span data-ttu-id="1413c-235">請遵循下列步驟，代表您的客戶在合作夥伴中心購買 Microsoft Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="1413c-235">Follow the steps below to buy Microsoft Azure reservations on behalf of your customers in Partner Center.</span></span>

1. <span data-ttu-id="1413c-236">從 [合作夥伴中心] 功能表選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="1413c-236">Select **Customers** from the Partner Center menu.</span></span>  

2. <span data-ttu-id="1413c-237">在 [**客戶**] 頁面上，尋找想要購買 Azure 保留的客戶，然後選取向下箭號以展開客戶的資料列。</span><span class="sxs-lookup"><span data-stu-id="1413c-237">On your **Customers** page, find the customer who wants to purchase Azure reservations and then select the down arrow to expand the customer's row.</span></span>  

3. <span data-ttu-id="1413c-238">選取 **\[新增產品\]** ，然後選取 **\[Azure\]** 。</span><span class="sxs-lookup"><span data-stu-id="1413c-238">Select **Add products** and then select **Azure**.</span></span> 

    <span data-ttu-id="1413c-239">a.</span><span class="sxs-lookup"><span data-stu-id="1413c-239">a.</span></span> <span data-ttu-id="1413c-240">從 [區段] 清單中選擇客戶的市場區段。</span><span class="sxs-lookup"><span data-stu-id="1413c-240">Choose the customer's market segment from the **Segment** list.</span></span>

    <span data-ttu-id="1413c-241">b.</span><span class="sxs-lookup"><span data-stu-id="1413c-241">b.</span></span> <span data-ttu-id="1413c-242">從 [產品**類型**] 清單中選擇 [**保留**]。</span><span class="sxs-lookup"><span data-stu-id="1413c-242">Choose **Reservations** from the product **Type** list.</span></span>

    <span data-ttu-id="1413c-243">c.</span><span class="sxs-lookup"><span data-stu-id="1413c-243">c.</span></span> <span data-ttu-id="1413c-244">從 [保留類型] 清單中選擇客戶想要的保留類型。</span><span class="sxs-lookup"><span data-stu-id="1413c-244">Choose the type of reservation the customer wants from the **Reservations type** list.</span></span>

4. <span data-ttu-id="1413c-245">Azure Reservations 必須關聯至有效的 Azure 訂閱。</span><span class="sxs-lookup"><span data-stu-id="1413c-245">Azure reservations must be associated with an active Azure subscription.</span></span> <span data-ttu-id="1413c-246">從 [**客戶訂**用帳戶] 清單中，選擇您想要新增 Azure 保留的客戶訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="1413c-246">Choose the customer's subscription you want to add Azure reservations to from the **Customer subscription** list.</span></span> 

   >[!IMPORTANT]
   ><span data-ttu-id="1413c-247">如果客戶還沒有作用中的 Azure 訂用帳戶，請選取 [ **Azure** ] 立即加入一個。</span><span class="sxs-lookup"><span data-stu-id="1413c-247">If the customer doesn't already have an active Azure subscription, select **Azure** to add one now.</span></span> 

5. <span data-ttu-id="1413c-248">使用篩選器來尋找符合客戶需求之虛擬機器上的 Azure 保留專案。</span><span class="sxs-lookup"><span data-stu-id="1413c-248">Use the filters to find Azure reservations on virtual machines that meet your customer's requirements.</span></span>  

6. <span data-ttu-id="1413c-249">找到您想要購買的保留後，請輸入客戶在**數量**中所需的保留實例數目，然後選取 [**新增至購物車**]。</span><span class="sxs-lookup"><span data-stu-id="1413c-249">After you find the reservation(s) you want to buy, enter the number of reserved instances the customer will need in **Quantity** and then select **Add to cart**.</span></span>  

7. <span data-ttu-id="1413c-250">重複步驟5和6，直到您將所有必要的專案新增至訂單為止。</span><span class="sxs-lookup"><span data-stu-id="1413c-250">Repeat steps 5 and 6 until you've added all the necessary items to the order.</span></span> <span data-ttu-id="1413c-251">選取 [檢閱] 確認您的訂單正確無誤。</span><span class="sxs-lookup"><span data-stu-id="1413c-251">Select **Review** to verify that your order is correct.</span></span>  

8. <span data-ttu-id="1413c-252">在 **\[檢視您的訂單\]** 頁面上，您可以：</span><span class="sxs-lookup"><span data-stu-id="1413c-252">On the **Review your orders** page, you can:</span></span> 

    - <span data-ttu-id="1413c-253">確認或變更保留執行個體數量。</span><span class="sxs-lookup"><span data-stu-id="1413c-253">Verify or change the reserved instances quantity.</span></span>

    - <span data-ttu-id="1413c-254">選取保留範圍。</span><span class="sxs-lookup"><span data-stu-id="1413c-254">Select the reservation's scope.</span></span> <span data-ttu-id="1413c-255">保留的範圍可以涵蓋一個訂用帳戶或多個訂用帳戶（共用範圍）。</span><span class="sxs-lookup"><span data-stu-id="1413c-255">The reservation's scope can cover one subscription or multiple subscriptions (shared scope).</span></span> <span data-ttu-id="1413c-256">如果您將保留範圍限定為單一訂用帳戶，則保留折扣僅適用于此訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="1413c-256">If you scope the reservation to a single subscription, the reservation discount is applied to this subscription only.</span></span> <span data-ttu-id="1413c-257">如果您選取 [共用]，保留折扣會套用至客戶帳單內容內的任何訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="1413c-257">If you select shared, the reservation discount is applied to any subscriptions within the customer's billing context.</span></span> 

      >[!NOTE] 
      ><span data-ttu-id="1413c-258">如果您選擇將保留範圍限制為單一 Azure 訂用帳戶，您可能需要增加訂用帳戶的 vCPU 配額。</span><span class="sxs-lookup"><span data-stu-id="1413c-258">If you opt to limit the reservation's scope to a single Azure subscription, you may need to increase the subscription's vCPU quota.</span></span> <span data-ttu-id="1413c-259">若要增加訂用帳戶的 vCPU 配額，您必須在 Azure 入口網站中建立支援要求。</span><span class="sxs-lookup"><span data-stu-id="1413c-259">To increase the subscription's vCPU quota, you'll need to create a support request in the Azure portal.</span></span> <span data-ttu-id="1413c-260">請遵循[本主題中](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request)的指示來建立要求。</span><span class="sxs-lookup"><span data-stu-id="1413c-260">Follow the instructions [in this topic](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request) to create the request.</span></span> 

      >[!NOTE]   
      ><span data-ttu-id="1413c-261">如果您的客戶在 Azure 方案底下，**範圍**將會設定為 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="1413c-261">If your customer is under the Azure plan, **Scope**  will be set to **Shared**.</span></span> 

    - <span data-ttu-id="1413c-262">如果您是提供者合作夥伴，請選取您想要與產品建立關聯的經銷商。</span><span class="sxs-lookup"><span data-stu-id="1413c-262">If you're a provider partner, select the reseller you want to associate with the product.</span></span>
    
    - <span data-ttu-id="1413c-263">如果您的 Azure 保留支援 [計費方案] 選項，您可以從下拉式功能表中選取 [每月計費頻率]。</span><span class="sxs-lookup"><span data-stu-id="1413c-263">If your Azure reservation supports the Billing plan option, you can select the billing frequency as monthly from the dropdown menu.</span></span> 
    - <span data-ttu-id="1413c-264">如果您的 Azure 保留不支援 [計費方案] 選項，您的計費頻率會預設為 [一次計費]。</span><span class="sxs-lookup"><span data-stu-id="1413c-264">If your Azure reservation does not support the Billing plan option, your billing frequency defaults to one time billing.</span></span> 

9. <span data-ttu-id="1413c-265">選取 **\[購買\]** 購買訂單。</span><span class="sxs-lookup"><span data-stu-id="1413c-265">Select **Buy** to purchase the order.</span></span> <span data-ttu-id="1413c-266">您的訂單詳細資料（包括訂單號碼）會顯示在 [**確認**] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="1413c-266">The details of your order, including your order number, are displayed on the **Confirm** page.</span></span> <span data-ttu-id="1413c-267">選取 [完成] 移至 [訂購記錄] 頁面。</span><span class="sxs-lookup"><span data-stu-id="1413c-267">Select **Done** to go to your **Order history** page.</span></span> 

10. <span data-ttu-id="1413c-268">若要管理 Azure 入口網站中的客戶保留，請在 **[客戶] 頁面上**尋找客戶，然後選取向下箭號以展開客戶的資料列。</span><span class="sxs-lookup"><span data-stu-id="1413c-268">To manage the customer's reservation in the Azure portal, find the customer on your **Customers** page and then select the down arrow to expand the customer's row.</span></span> <span data-ttu-id="1413c-269">選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="1413c-269">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="1413c-270">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="1413c-270">Azure reservations resources</span></span>
|<span data-ttu-id="1413c-271">**如需相關資訊**</span><span class="sxs-lookup"><span data-stu-id="1413c-271">**For information about**</span></span>   |<span data-ttu-id="1413c-272">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="1413c-272">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="1413c-273">雲端解決方案提供者中的 Azure Reservations 概觀</span><span class="sxs-lookup"><span data-stu-id="1413c-273">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="1413c-274">銷售 Microsoft Azure 保留實例</span><span class="sxs-lookup"><span data-stu-id="1413c-274">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="1413c-275">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="1413c-275">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="1413c-276">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="1413c-276">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="1413c-277">判斷正確的 VM 大小，並確認客戶 VM 使用率</span><span class="sxs-lookup"><span data-stu-id="1413c-277">Determine the correct VM size and verify customer VM usage</span></span>   |[<span data-ttu-id="1413c-278">Azure 保留使用量上限的 VM 大小</span><span class="sxs-lookup"><span data-stu-id="1413c-278">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="1413c-279">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="1413c-279">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="1413c-280">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="1413c-280">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
|

 


 
