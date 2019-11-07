---
title: 代表您的客戶購買 Microsoft Azure Reservations | 合作夥伴中心
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 您可以在合作夥伴中心代表您的客戶購買 Azure 保留。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, 管理, 計費, 購買
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: c995072056fd70f1e0fb71a2b664242c54bd989f
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653831"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a><span data-ttu-id="ca5cf-104">代表您的客戶在合作夥伴中心購買 Microsoft Azure 保留</span><span class="sxs-lookup"><span data-stu-id="ca5cf-104">Buy Microsoft Azure reservations on behalf of your customers in Partner Center</span></span> 

<span data-ttu-id="ca5cf-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="ca5cf-105">**Applies to**</span></span>

-  <span data-ttu-id="ca5cf-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="ca5cf-106">Partner Center</span></span>
-  <span data-ttu-id="ca5cf-107">Microsoft Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="ca5cf-107">Microsoft Azure portal</span></span>
-  <span data-ttu-id="ca5cf-108">雲端解決方案提供者中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="ca5cf-108">Partners in CSP</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="ca5cf-109">在您開始前</span><span class="sxs-lookup"><span data-stu-id="ca5cf-109">Before you begin</span></span>

<span data-ttu-id="ca5cf-110">請先參閱下面的重要資訊，然後再代表您的客戶購買 Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-110">Review the important information below before you buy Azure reservations on behalf of your customers.</span></span>

- <span data-ttu-id="ca5cf-111">如果您的客戶簽署新的 Microsoft 客戶合約時，[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)，您必須在 azure 方案下購買 azure 保留。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-111">If and when your customer signs the new Microsoft Customer Agreement [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md), you must purchase Azure reservations under the Azure plan.</span></span> <span data-ttu-id="ca5cf-112">如需詳細資訊，請參閱[購買 Azure 方案](purchase-azure-plan.md)。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-112">For more information, read [Purchase Azure Plan](purchase-azure-plan.md).</span></span>

-   <span data-ttu-id="ca5cf-113">在您代表客戶購買保留區之前，客戶必須已擁有有效的 Azure 訂閱</span><span class="sxs-lookup"><span data-stu-id="ca5cf-113">Customers must already have an active Azure subscription before you can purchase reservations on their behalf</span></span>
  
-   <span data-ttu-id="ca5cf-114">軟體訂用帳戶成本（例如 SQL Database 或 SUSE Linux 軟體）不包含在 Azure 保留價格中</span><span class="sxs-lookup"><span data-stu-id="ca5cf-114">Software subscription costs such as SQL Database or SUSE Linux software are not included in Azure reservation prices</span></span>

-   <span data-ttu-id="ca5cf-115">除非您的位置是巴西，否則 Microsoft 的商業定價不包含稅金。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-115">Microsoft's commercial pricing to you does not include taxes, unless your location is Brazil.</span></span> <span data-ttu-id="ca5cf-116">如果您的地點是巴西，則您的商業價格包含適當的稅額</span><span class="sxs-lookup"><span data-stu-id="ca5cf-116">If your location is Brazil, the commercial price to you includes the appropriate taxes</span></span> 
 
-   <span data-ttu-id="ca5cf-117">銷售人員和技術支援中心需能代表客戶明確的存取 Azure 訂閱，以便在 Azure 入口網站與檔案支援要求中購買或管理訂閱，包括換貨與退款</span><span class="sxs-lookup"><span data-stu-id="ca5cf-117">Sales and help desk agents need explicit access to the Azure subscription so they can buy or manage it in the Azure portal and file support requests, including for exchanges and refunds, on behalf of the customer</span></span>  

-   <span data-ttu-id="ca5cf-118">如果您是間接提供者，而且您透過 Azure 入口網站購買 Azure 保留專案，則會從您選取的 Azure CSP 訂用帳戶繼承「記錄」（間接轉銷商）的夥伴。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-118">If you're an indirect provider and you buy Azure reservations through the Azure portal, the Partner on Record (indirect reseller) is inherited from the Azure CSP subscription you select.</span></span> 

-   <span data-ttu-id="ca5cf-119">購買後無法變更 Azure 保留的記錄合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-119">The Partner of Record for Azure reservations cannot be changed post-purchase.</span></span> <span data-ttu-id="ca5cf-120">您可以取消現有的保留區，並透過新的記錄可查夥伴購買新的保留區。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-120">You can cancel the existing reservation and purchase a new one with the new Partner on Record.</span></span> 

-   <span data-ttu-id="ca5cf-121">如果客戶想將 Azure 訂閱從直接或 EA 轉移至雲端解決方案提供者，保留區無法轉移。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-121">If a customer wants to transfer an Azure subscription from Direct or EA to CSP, reservations do not get transferred.</span></span> 

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="ca5cf-122">Azure 保留無法使用的市場</span><span class="sxs-lookup"><span data-stu-id="ca5cf-122">Azure reservations unavailable markets</span></span>

>[!IMPORTANT] 
><span data-ttu-id="ca5cf-123">下列市場*不*提供 Azure 保留：</span><span class="sxs-lookup"><span data-stu-id="ca5cf-123">Azure reservations *are not* available in the following markets:</span></span>  
>  
> | <span data-ttu-id="ca5cf-124">無法使用的市場</span><span class="sxs-lookup"><span data-stu-id="ca5cf-124">Unavailable markets</span></span> | &nbsp; | &nbsp; |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="ca5cf-125">奧蘭島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-125">Åland Islands</span></span>     | <span data-ttu-id="ca5cf-126">格陵蘭 (丹麥)</span><span class="sxs-lookup"><span data-stu-id="ca5cf-126">Greenland</span></span>     | <span data-ttu-id="ca5cf-127">巴布亞紐幾內亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-127">Papua New Guinea</span></span>     |
> | <span data-ttu-id="ca5cf-128">美屬薩摩亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-128">American Samoa</span></span>     | <span data-ttu-id="ca5cf-129">格瑞那達</span><span class="sxs-lookup"><span data-stu-id="ca5cf-129">Grenada</span></span>     | <span data-ttu-id="ca5cf-130">皮特康群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-130">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="ca5cf-131">安道爾</span><span class="sxs-lookup"><span data-stu-id="ca5cf-131">Andorra</span></span>     | <span data-ttu-id="ca5cf-132">瓜地洛普</span><span class="sxs-lookup"><span data-stu-id="ca5cf-132">Guadeloupe</span></span>     | <span data-ttu-id="ca5cf-133">留尼旺</span><span class="sxs-lookup"><span data-stu-id="ca5cf-133">Reunion</span></span>     |
> | <span data-ttu-id="ca5cf-134">安圭拉</span><span class="sxs-lookup"><span data-stu-id="ca5cf-134">Anguilla</span></span>     | <span data-ttu-id="ca5cf-135">關島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-135">Guam</span></span>     | <span data-ttu-id="ca5cf-136">沙巴</span><span class="sxs-lookup"><span data-stu-id="ca5cf-136">Saba</span></span>   |
> | <span data-ttu-id="ca5cf-137">南極大陸</span><span class="sxs-lookup"><span data-stu-id="ca5cf-137">Antarctica</span></span>     | <span data-ttu-id="ca5cf-138">根息</span><span class="sxs-lookup"><span data-stu-id="ca5cf-138">Guernsey</span></span>     | <span data-ttu-id="ca5cf-139">聖巴瑟米</span><span class="sxs-lookup"><span data-stu-id="ca5cf-139">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="ca5cf-140">安地卡及巴布達</span><span class="sxs-lookup"><span data-stu-id="ca5cf-140">Antigua and Barbuda</span></span>       | <span data-ttu-id="ca5cf-141">幾內亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-141">Guinea</span></span>     | <span data-ttu-id="ca5cf-142">聖露西亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-142">Saint Lucia</span></span>   |
> | <span data-ttu-id="ca5cf-143">阿路巴</span><span class="sxs-lookup"><span data-stu-id="ca5cf-143">Aruba</span></span>       | <span data-ttu-id="ca5cf-144">幾內亞比索</span><span class="sxs-lookup"><span data-stu-id="ca5cf-144">Guinea-Bissau</span></span>     | <span data-ttu-id="ca5cf-145">聖馬丁</span><span class="sxs-lookup"><span data-stu-id="ca5cf-145">Saint Martin</span></span>   |
> | <span data-ttu-id="ca5cf-146">亞塞拜然</span><span class="sxs-lookup"><span data-stu-id="ca5cf-146">Azerbaijan</span></span>       | <span data-ttu-id="ca5cf-147">蓋亞納</span><span class="sxs-lookup"><span data-stu-id="ca5cf-147">Guyana</span></span>     | <span data-ttu-id="ca5cf-148">聖匹島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-148">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="ca5cf-149">貝南</span><span class="sxs-lookup"><span data-stu-id="ca5cf-149">Benin</span></span>     | <span data-ttu-id="ca5cf-150">海地</span><span class="sxs-lookup"><span data-stu-id="ca5cf-150">Haiti</span></span>       | <span data-ttu-id="ca5cf-151">聖文森及格瑞那丁</span><span class="sxs-lookup"><span data-stu-id="ca5cf-151">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="ca5cf-152">不丹</span><span class="sxs-lookup"><span data-stu-id="ca5cf-152">Bhutan</span></span>     | <span data-ttu-id="ca5cf-153">赫德島及麥當勞群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-153">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="ca5cf-154">薩摩亞獨立國</span><span class="sxs-lookup"><span data-stu-id="ca5cf-154">Samoa</span></span>     |
> | <span data-ttu-id="ca5cf-155">波奈</span><span class="sxs-lookup"><span data-stu-id="ca5cf-155">Bonaire</span></span>     | <span data-ttu-id="ca5cf-156">曼城島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-156">Isle of Man</span></span>     | <span data-ttu-id="ca5cf-157">聖馬利諾</span><span class="sxs-lookup"><span data-stu-id="ca5cf-157">San Marino</span></span>     |
> | <span data-ttu-id="ca5cf-158">布威島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-158">Bouvet Island</span></span>     | <span data-ttu-id="ca5cf-159">Jan 馬延</span><span class="sxs-lookup"><span data-stu-id="ca5cf-159">Jan Mayen</span></span>     | <span data-ttu-id="ca5cf-160">聖多美普林西比</span><span class="sxs-lookup"><span data-stu-id="ca5cf-160">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="ca5cf-161">英屬印度洋領土</span><span class="sxs-lookup"><span data-stu-id="ca5cf-161">British Indian Ocean Territory</span></span>       | <span data-ttu-id="ca5cf-162">澤西島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-162">Jersey</span></span>     | <span data-ttu-id="ca5cf-163">塞席爾</span><span class="sxs-lookup"><span data-stu-id="ca5cf-163">Seychelles</span></span>   |
> | <span data-ttu-id="ca5cf-164">英屬維爾京群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-164">British Virgin Islands</span></span>     | <span data-ttu-id="ca5cf-165">吉里巴斯</span><span class="sxs-lookup"><span data-stu-id="ca5cf-165">Kiribati</span></span>       | <span data-ttu-id="ca5cf-166">獅子山</span><span class="sxs-lookup"><span data-stu-id="ca5cf-166">Sierra Leone</span></span>   |
> | <span data-ttu-id="ca5cf-167">布吉納法索</span><span class="sxs-lookup"><span data-stu-id="ca5cf-167">Burkina Faso</span></span>     | <span data-ttu-id="ca5cf-168">科索沃</span><span class="sxs-lookup"><span data-stu-id="ca5cf-168">Kosovo</span></span>     | <span data-ttu-id="ca5cf-169">聖尤斯特斯</span><span class="sxs-lookup"><span data-stu-id="ca5cf-169">Sint Eustatius</span></span>     |
> | <span data-ttu-id="ca5cf-170">蒲隆地</span><span class="sxs-lookup"><span data-stu-id="ca5cf-170">Burundi</span></span>     | <span data-ttu-id="ca5cf-171">寮國</span><span class="sxs-lookup"><span data-stu-id="ca5cf-171">Laos</span></span>     | <span data-ttu-id="ca5cf-172">荷屬聖馬丁</span><span class="sxs-lookup"><span data-stu-id="ca5cf-172">Sint Maarten</span></span>     |
> | <span data-ttu-id="ca5cf-173">柬埔寨</span><span class="sxs-lookup"><span data-stu-id="ca5cf-173">Cambodia</span></span>     | <span data-ttu-id="ca5cf-174">賴索托</span><span class="sxs-lookup"><span data-stu-id="ca5cf-174">Lesotho</span></span>     | <span data-ttu-id="ca5cf-175">索羅門群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-175">Solomon Islands</span></span>     |
> | <span data-ttu-id="ca5cf-176">中非共和國</span><span class="sxs-lookup"><span data-stu-id="ca5cf-176">Central African Republic</span></span>     | <span data-ttu-id="ca5cf-177">賴比瑞亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-177">Liberia</span></span>     | <span data-ttu-id="ca5cf-178">索馬利亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-178">Somalia</span></span>     |
> | <span data-ttu-id="ca5cf-179">查德</span><span class="sxs-lookup"><span data-stu-id="ca5cf-179">Chad</span></span>     | <span data-ttu-id="ca5cf-180">馬達加斯加</span><span class="sxs-lookup"><span data-stu-id="ca5cf-180">Madagascar</span></span>     | <span data-ttu-id="ca5cf-181">南喬治亞與南三明治群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-181">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="ca5cf-182">中國</span><span class="sxs-lookup"><span data-stu-id="ca5cf-182">China</span></span>     | <span data-ttu-id="ca5cf-183">馬拉威</span><span class="sxs-lookup"><span data-stu-id="ca5cf-183">Malawi</span></span>     | <span data-ttu-id="ca5cf-184">南蘇丹</span><span class="sxs-lookup"><span data-stu-id="ca5cf-184">South Sudan</span></span>     |
> | <span data-ttu-id="ca5cf-185">聖誕島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-185">Christmas Island</span></span>     | <span data-ttu-id="ca5cf-186">馬爾地夫</span><span class="sxs-lookup"><span data-stu-id="ca5cf-186">Maldives</span></span>     | <span data-ttu-id="ca5cf-187">聖赫勒拿、阿森松、特裡斯坦達庫尼亞群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-187">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="ca5cf-188">可可斯群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-188">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="ca5cf-189">馬利</span><span class="sxs-lookup"><span data-stu-id="ca5cf-189">Mali</span></span>     | <span data-ttu-id="ca5cf-190">蘇利南</span><span class="sxs-lookup"><span data-stu-id="ca5cf-190">Suriname</span></span>     |
> | <span data-ttu-id="ca5cf-191">葛摩</span><span class="sxs-lookup"><span data-stu-id="ca5cf-191">Comoros</span></span>     | <span data-ttu-id="ca5cf-192">馬紹爾群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-192">Marshall Islands</span></span>     | <span data-ttu-id="ca5cf-193">冷岸</span><span class="sxs-lookup"><span data-stu-id="ca5cf-193">Svalbard</span></span>     |
> | <span data-ttu-id="ca5cf-194">剛果共和國</span><span class="sxs-lookup"><span data-stu-id="ca5cf-194">Congo</span></span>     | <span data-ttu-id="ca5cf-195">馬丁尼克島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-195">Martinique</span></span>     | <span data-ttu-id="ca5cf-196">史瓦濟蘭</span><span class="sxs-lookup"><span data-stu-id="ca5cf-196">Swaziland</span></span>     |
> | <span data-ttu-id="ca5cf-197">剛果民主共和國 (DRC)</span><span class="sxs-lookup"><span data-stu-id="ca5cf-197">Congo (DRC)</span></span>     | <span data-ttu-id="ca5cf-198">茅利塔尼亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-198">Mauritania</span></span>     | <span data-ttu-id="ca5cf-199">東帝汶</span><span class="sxs-lookup"><span data-stu-id="ca5cf-199">Timor-Leste</span></span>   |
> | <span data-ttu-id="ca5cf-200">柯克群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-200">Cook Islands</span></span>     | <span data-ttu-id="ca5cf-201">馬約特島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-201">Mayotte</span></span>     | <span data-ttu-id="ca5cf-202">多哥</span><span class="sxs-lookup"><span data-stu-id="ca5cf-202">Togo</span></span>   |
> | <span data-ttu-id="ca5cf-203">吉布地</span><span class="sxs-lookup"><span data-stu-id="ca5cf-203">Djibouti</span></span>     | <span data-ttu-id="ca5cf-204">密克羅尼西亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-204">Micronesia</span></span>     | <span data-ttu-id="ca5cf-205">托克勞群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-205">Tokelau</span></span>   |
> | <span data-ttu-id="ca5cf-206">多米尼克</span><span class="sxs-lookup"><span data-stu-id="ca5cf-206">Dominica</span></span>     | <span data-ttu-id="ca5cf-207">蒙特色拉特島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-207">Montserrat</span></span>     | <span data-ttu-id="ca5cf-208">東加</span><span class="sxs-lookup"><span data-stu-id="ca5cf-208">Tonga</span></span>   |
> | <span data-ttu-id="ca5cf-209">赤道幾內亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-209">Equatorial Guinea</span></span>     | <span data-ttu-id="ca5cf-210">莫三比克</span><span class="sxs-lookup"><span data-stu-id="ca5cf-210">Mozambique</span></span>     | <span data-ttu-id="ca5cf-211">土克斯及開科斯群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-211">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="ca5cf-212">厄利垂亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-212">Eritrea</span></span>     | <span data-ttu-id="ca5cf-213">緬甸文</span><span class="sxs-lookup"><span data-stu-id="ca5cf-213">Myanmar</span></span>     | <span data-ttu-id="ca5cf-214">吐瓦魯</span><span class="sxs-lookup"><span data-stu-id="ca5cf-214">Tuvalu</span></span>   |
> | <span data-ttu-id="ca5cf-215">福克蘭群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-215">Falkland Islands</span></span>     | <span data-ttu-id="ca5cf-216">諾魯</span><span class="sxs-lookup"><span data-stu-id="ca5cf-216">Nauru</span></span>     | <span data-ttu-id="ca5cf-217">美國外島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-217">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="ca5cf-218">法屬圭亞那</span><span class="sxs-lookup"><span data-stu-id="ca5cf-218">French Guiana</span></span>     | <span data-ttu-id="ca5cf-219">新喀里多尼亞群島領土</span><span class="sxs-lookup"><span data-stu-id="ca5cf-219">New Caledonia</span></span>     | <span data-ttu-id="ca5cf-220">萬那杜</span><span class="sxs-lookup"><span data-stu-id="ca5cf-220">Vanuatu</span></span>   |
> | <span data-ttu-id="ca5cf-221">法屬玻里尼西亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-221">French Polynesia</span></span>     | <span data-ttu-id="ca5cf-222">尼日</span><span class="sxs-lookup"><span data-stu-id="ca5cf-222">Niger</span></span>     | <span data-ttu-id="ca5cf-223">梵蒂岡</span><span class="sxs-lookup"><span data-stu-id="ca5cf-223">Vatican City</span></span>   |
> | <span data-ttu-id="ca5cf-224">法屬南半球領土</span><span class="sxs-lookup"><span data-stu-id="ca5cf-224">French Southern Territories</span></span>     | <span data-ttu-id="ca5cf-225">紐威島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-225">Niue</span></span>     | <span data-ttu-id="ca5cf-226">瓦利斯及福杜納</span><span class="sxs-lookup"><span data-stu-id="ca5cf-226">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="ca5cf-227">加彭</span><span class="sxs-lookup"><span data-stu-id="ca5cf-227">Gabon</span></span>     | <span data-ttu-id="ca5cf-228">諾福克島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-228">Norfolk Island</span></span>     | <span data-ttu-id="ca5cf-229">葉門</span><span class="sxs-lookup"><span data-stu-id="ca5cf-229">Yemen</span></span>   |
> | <span data-ttu-id="ca5cf-230">甘比亞</span><span class="sxs-lookup"><span data-stu-id="ca5cf-230">Gambia</span></span>     | <span data-ttu-id="ca5cf-231">北馬里安納群島</span><span class="sxs-lookup"><span data-stu-id="ca5cf-231">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="ca5cf-232">直布羅陀</span><span class="sxs-lookup"><span data-stu-id="ca5cf-232">Gibraltar</span></span>     | <span data-ttu-id="ca5cf-233">帛琉</span><span class="sxs-lookup"><span data-stu-id="ca5cf-233">Palau</span></span>       |    |

## <a name="purchase-azure-reservations"></a><span data-ttu-id="ca5cf-234">購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="ca5cf-234">Purchase Azure reservations</span></span>

<span data-ttu-id="ca5cf-235">請遵循下列步驟，代表您的客戶在合作夥伴中心購買 Microsoft Azure 保留。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-235">Follow the steps below to buy Microsoft Azure reservations on behalf of your customers in Partner Center.</span></span>

1. <span data-ttu-id="ca5cf-236">從 [合作夥伴中心] 功能表選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-236">Select **Customers** from the Partner Center menu.</span></span>  

2. <span data-ttu-id="ca5cf-237">在 [**客戶**] 頁面上，尋找想要購買 Azure 保留的客戶，然後選取向下箭號以展開客戶的資料列。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-237">On your **Customers** page, find the customer who wants to purchase Azure reservations and then select the down arrow to expand the customer's row.</span></span>  

3. <span data-ttu-id="ca5cf-238">選取 [新增產品]，然後選取 [Azure]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-238">Select **Add products** and then select **Azure**.</span></span> 

    <span data-ttu-id="ca5cf-239">a.</span><span class="sxs-lookup"><span data-stu-id="ca5cf-239">a.</span></span> <span data-ttu-id="ca5cf-240">從 [區段] 清單中選擇客戶的市場區段。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-240">Choose the customer's market segment from the **Segment** list.</span></span>

    <span data-ttu-id="ca5cf-241">b。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-241">b.</span></span> <span data-ttu-id="ca5cf-242">從 [產品**類型**] 清單中選擇 [**保留**]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-242">Choose **Reservations** from the product **Type** list.</span></span>

    <span data-ttu-id="ca5cf-243">c.</span><span class="sxs-lookup"><span data-stu-id="ca5cf-243">c.</span></span> <span data-ttu-id="ca5cf-244">從 [保留類型] 清單中選擇客戶想要的保留類型。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-244">Choose the type of reservation the customer wants from the **Reservations type** list.</span></span>

4. <span data-ttu-id="ca5cf-245">Azure Reservations 必須關聯至有效的 Azure 訂閱。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-245">Azure reservations must be associated with an active Azure subscription.</span></span> <span data-ttu-id="ca5cf-246">從 [**客戶訂**用帳戶] 清單中，選擇您想要新增 Azure 保留的客戶訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-246">Choose the customer's subscription you want to add Azure reservations to from the **Customer subscription** list.</span></span> 

   >[!IMPORTANT]
   ><span data-ttu-id="ca5cf-247">如果客戶還沒有作用中的 Azure 訂用帳戶，請選取 [ **Azure** ] 立即加入一個。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-247">If the customer doesn't already have an active Azure subscription, select **Azure** to add one now.</span></span> 

5. <span data-ttu-id="ca5cf-248">使用篩選器來尋找符合客戶需求之虛擬機器上的 Azure 保留專案。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-248">Use the filters to find Azure reservations on virtual machines that meet your customer's requirements.</span></span>  

6. <span data-ttu-id="ca5cf-249">找到您想要購買的保留後，請輸入客戶在**數量**中所需的保留實例數目，然後選取 [**新增至購物車**]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-249">After you find the reservation(s) you want to buy, enter the number of reserved instances the customer will need in **Quantity** and then select **Add to cart**.</span></span>  

7. <span data-ttu-id="ca5cf-250">重複步驟5和6，直到您將所有必要的專案新增至訂單為止。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-250">Repeat steps 5 and 6 until you've added all the necessary items to the order.</span></span> <span data-ttu-id="ca5cf-251">選取 [檢閱] 確認您的訂單正確無誤。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-251">Select **Review** to verify that your order is correct.</span></span>  

8. <span data-ttu-id="ca5cf-252">在 **\[檢視您的訂單\]** 頁面上，您可以：</span><span class="sxs-lookup"><span data-stu-id="ca5cf-252">On the **Review your orders** page, you can:</span></span> 

    - <span data-ttu-id="ca5cf-253">確認或變更保留執行個體數量。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-253">Verify or change the reserved instances quantity.</span></span>

    - <span data-ttu-id="ca5cf-254">選取保留範圍。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-254">Select the reservation's scope.</span></span> <span data-ttu-id="ca5cf-255">保留的範圍可以涵蓋一個訂用帳戶或多個訂用帳戶（共用範圍）。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-255">The reservation's scope can cover one subscription or multiple subscriptions (shared scope).</span></span> <span data-ttu-id="ca5cf-256">如果您將保留範圍限定為單一訂用帳戶，則保留折扣僅適用于此訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-256">If you scope the reservation to a single subscription, the reservation discount is applied to this subscription only.</span></span> <span data-ttu-id="ca5cf-257">如果您選取 [共用]，保留折扣會套用至客戶帳單內容內的任何訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-257">If you select shared, the reservation discount is applied to any subscriptions within the customer's billing context.</span></span> 

      >[!NOTE] 
      ><span data-ttu-id="ca5cf-258">如果您選擇將保留範圍限制為單一 Azure 訂用帳戶，您可能需要增加訂用帳戶的 vCPU 配額。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-258">If you opt to limit the reservation's scope to a single Azure subscription, you may need to increase the subscription's vCPU quota.</span></span> <span data-ttu-id="ca5cf-259">若要增加訂用帳戶的 vCPU 配額，您必須在 Azure 入口網站中建立支援要求。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-259">To increase the subscription's vCPU quota, you'll need to create a support request in the Azure portal.</span></span> <span data-ttu-id="ca5cf-260">請遵循[本主題中](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request)的指示來建立要求。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-260">Follow the instructions [in this topic](https://docs.microsoft.com/azure/azure-supportability/resource-manager-core-quotas-request) to create the request.</span></span> 

      >[!NOTE]   
      ><span data-ttu-id="ca5cf-261">如果您的客戶在 Azure 方案底下，**範圍**將會設定為 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-261">If your customer is under the Azure plan, **Scope**  will be set to **Shared**.</span></span> 

    - <span data-ttu-id="ca5cf-262">如果您是提供者合作夥伴，請選取您想要與產品建立關聯的經銷商。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-262">If you're a provider partner, select the reseller you want to associate with the product.</span></span>
    
    - <span data-ttu-id="ca5cf-263">如果您的 Azure 保留支援 [計費方案] 選項，您可以從下拉式功能表中選取 [每月計費頻率]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-263">If your Azure reservation supports the Billing plan option, you can select the billing frequency as monthly from the dropdown menu.</span></span> 
    - <span data-ttu-id="ca5cf-264">如果您的 Azure 保留不支援 [計費方案] 選項，您的計費頻率會預設為 [一次計費]。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-264">If your Azure reservation does not support the Billing plan option, your billing frequency defaults to one time billing.</span></span> 

9. <span data-ttu-id="ca5cf-265">選取 **\[購買\]** 購買訂單。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-265">Select **Buy** to purchase the order.</span></span> <span data-ttu-id="ca5cf-266">您的訂單詳細資料（包括訂單號碼）會顯示在 [**確認**] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-266">The details of your order, including your order number, are displayed on the **Confirm** page.</span></span> <span data-ttu-id="ca5cf-267">選取 [完成] 移至 [訂購記錄] 頁面。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-267">Select **Done** to go to your **Order history** page.</span></span> 

10. <span data-ttu-id="ca5cf-268">若要管理 Azure 入口網站中的客戶保留，請在 **[客戶] 頁面上**尋找客戶，然後選取向下箭號以展開客戶的資料列。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-268">To manage the customer's reservation in the Azure portal, find the customer on your **Customers** page and then select the down arrow to expand the customer's row.</span></span> <span data-ttu-id="ca5cf-269">選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="ca5cf-269">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="ca5cf-270">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="ca5cf-270">Azure reservations resources</span></span>
|<span data-ttu-id="ca5cf-271">**如需相關資訊**</span><span class="sxs-lookup"><span data-stu-id="ca5cf-271">**For information about**</span></span>   |<span data-ttu-id="ca5cf-272">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="ca5cf-272">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="ca5cf-273">雲端解決方案提供者中的 Azure Reservations 概觀</span><span class="sxs-lookup"><span data-stu-id="ca5cf-273">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="ca5cf-274">銷售 Microsoft Azure 保留實例</span><span class="sxs-lookup"><span data-stu-id="ca5cf-274">Sell Microsoft Azure Reserved Instances</span></span>](azure-reservations.md) |
|<span data-ttu-id="ca5cf-275">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="ca5cf-275">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="ca5cf-276">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="ca5cf-276">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="ca5cf-277">判斷正確的 VM 大小，並確認客戶 VM 使用率</span><span class="sxs-lookup"><span data-stu-id="ca5cf-277">Determine the correct VM size and verify customer VM usage</span></span>   |[<span data-ttu-id="ca5cf-278">Azure 保留使用量上限的 VM 大小</span><span class="sxs-lookup"><span data-stu-id="ca5cf-278">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="ca5cf-279">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="ca5cf-279">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="ca5cf-280">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="ca5cf-280">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>
|

 


 
