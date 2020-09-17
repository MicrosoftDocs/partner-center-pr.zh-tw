---
title: 透過雲端解決方案提供者銷售軟體訂閱
ms.topic: how-to
ms.date: 06/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解雲端解決方案提供者計畫中的合作夥伴如何使用合作夥伴中心為客戶購買、管理、銷售和取消 Azure 保留的執行個體與伺服器訂閱。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 467f46b2e6dfc41730970abe9005e1f2d28409f3
ms.sourcegitcommit: e06327ece344125fa579aae8da6042c2f32b4a8e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/09/2020
ms.locfileid: "89614151"
---
# <a name="sell-software-subscriptions-through-the-cloud-solution-provider-csp-program"></a><span data-ttu-id="37f11-103">透過雲端解決方案提供者 (CSP) 方案銷售軟體訂閱</span><span class="sxs-lookup"><span data-stu-id="37f11-103">Sell software subscriptions through the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="37f11-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="37f11-104">**Applies to**</span></span>

- <span data-ttu-id="37f11-105">雲端解決方案提供者</span><span class="sxs-lookup"><span data-stu-id="37f11-105">Cloud Solution Providers</span></span>

<span data-ttu-id="37f11-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="37f11-106">**Appropriate roles**</span></span>

- <span data-ttu-id="37f11-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="37f11-107">Admin agent</span></span>
- <span data-ttu-id="37f11-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="37f11-108">Global admin</span></span>

<span data-ttu-id="37f11-109">透過 Azure 保留和伺服器訂閱 (Windows Server 和 SQL Server 訂閱)，雲端解決方案提供者計畫中的合作夥伴將更能因應客戶快速增長的需求，以更具成本效益的解決方案支援具有高度可預測性與持續性的雲端工作負載。</span><span class="sxs-lookup"><span data-stu-id="37f11-109">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions),partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="37f11-110">您現在可以運用 Azure Hybrid Benefit，透過合作夥伴中心和 Azure 入口網站，代表商業客戶取得、佈建和管理 Azure 保留和伺服器訂閱。</span><span class="sxs-lookup"><span data-stu-id="37f11-110">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure portal by taking advantage of the Azure Hybrid Benefit.</span></span>

<span data-ttu-id="37f11-111">Azure Hybrid Benefit 有助於讓您的 Windows Server 授權發揮更大的效益，並可節省高達 40% 的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="37f11-111">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="37f11-112">您可以將權益搭配用於軟體保證所涵蓋的 Windows Server Datacenter 和 Standard Edition 授權。</span><span class="sxs-lookup"><span data-stu-id="37f11-112">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="37f11-113">根據版本，您可以轉換或重複使用在 Azure 中執行 Windows Server 虛擬機器的授權，並支付較低的基本計算費率 (例如 Linux 虛擬機器費率)。</span><span class="sxs-lookup"><span data-stu-id="37f11-113">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, for example).</span></span>

## <a name="azure-reservations-unavailable-markets"></a><span data-ttu-id="37f11-114">未提供 Azure 保留的市場</span><span class="sxs-lookup"><span data-stu-id="37f11-114">Azure reservations unavailable markets</span></span>

>[!IMPORTANT]
><span data-ttu-id="37f11-115">以下是**未提供** Azure 保留的市場：</span><span class="sxs-lookup"><span data-stu-id="37f11-115">Azure reservations **are not** available in the following markets:</span></span>  
>  
> <span data-ttu-id="37f11-116">**不適用的市場 (以字母順序排序)**</span><span class="sxs-lookup"><span data-stu-id="37f11-116">**Unavailable markets (in alphabetical order)**</span></span>
>
> |<span data-ttu-id="37f11-117">A 到 Gi</span><span class="sxs-lookup"><span data-stu-id="37f11-117">A to Gi</span></span>   | <span data-ttu-id="37f11-118">Gr 到 Pal</span><span class="sxs-lookup"><span data-stu-id="37f11-118">Gr to Pal</span></span>  | <span data-ttu-id="37f11-119">Pap 到 Z</span><span class="sxs-lookup"><span data-stu-id="37f11-119">Pap to Z</span></span> |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | <span data-ttu-id="37f11-120">奧蘭島</span><span class="sxs-lookup"><span data-stu-id="37f11-120">Aland Islands</span></span>     | <span data-ttu-id="37f11-121">格陵蘭</span><span class="sxs-lookup"><span data-stu-id="37f11-121">Greenland</span></span>     | <span data-ttu-id="37f11-122">巴布亞紐幾內亞</span><span class="sxs-lookup"><span data-stu-id="37f11-122">Papua New Guinea</span></span>     |
> | <span data-ttu-id="37f11-123">美屬薩摩亞</span><span class="sxs-lookup"><span data-stu-id="37f11-123">American Samoa</span></span>     | <span data-ttu-id="37f11-124">格瑞那達</span><span class="sxs-lookup"><span data-stu-id="37f11-124">Grenada</span></span>     | <span data-ttu-id="37f11-125">皮特康群島</span><span class="sxs-lookup"><span data-stu-id="37f11-125">Pitcairn Islands</span></span>     |
> | <span data-ttu-id="37f11-126">安道爾</span><span class="sxs-lookup"><span data-stu-id="37f11-126">Andorra</span></span>     | <span data-ttu-id="37f11-127">哥德普洛</span><span class="sxs-lookup"><span data-stu-id="37f11-127">Guadeloupe</span></span>     | <span data-ttu-id="37f11-128">留尼旺</span><span class="sxs-lookup"><span data-stu-id="37f11-128">Reunion</span></span>     |
> | <span data-ttu-id="37f11-129">安圭拉</span><span class="sxs-lookup"><span data-stu-id="37f11-129">Anguilla</span></span>     | <span data-ttu-id="37f11-130">關島</span><span class="sxs-lookup"><span data-stu-id="37f11-130">Guam</span></span>     | <span data-ttu-id="37f11-131">沙巴</span><span class="sxs-lookup"><span data-stu-id="37f11-131">Saba</span></span>   |
> | <span data-ttu-id="37f11-132">南極大陸</span><span class="sxs-lookup"><span data-stu-id="37f11-132">Antarctica</span></span>     | <span data-ttu-id="37f11-133">根息</span><span class="sxs-lookup"><span data-stu-id="37f11-133">Guernsey</span></span>     | <span data-ttu-id="37f11-134">聖巴瑟米</span><span class="sxs-lookup"><span data-stu-id="37f11-134">Saint Barthélemy</span></span>   |
> | <span data-ttu-id="37f11-135">安地卡及巴布達</span><span class="sxs-lookup"><span data-stu-id="37f11-135">Antigua and Barbuda</span></span>       | <span data-ttu-id="37f11-136">幾內亞</span><span class="sxs-lookup"><span data-stu-id="37f11-136">Guinea</span></span>     | <span data-ttu-id="37f11-137">聖露西亞</span><span class="sxs-lookup"><span data-stu-id="37f11-137">Saint Lucia</span></span>   |
> | <span data-ttu-id="37f11-138">阿路巴</span><span class="sxs-lookup"><span data-stu-id="37f11-138">Aruba</span></span>       | <span data-ttu-id="37f11-139">幾內亞比索</span><span class="sxs-lookup"><span data-stu-id="37f11-139">Guinea-Bissau</span></span>     | <span data-ttu-id="37f11-140">聖馬丁</span><span class="sxs-lookup"><span data-stu-id="37f11-140">Saint Martin</span></span>   |
> | <span data-ttu-id="37f11-141">亞塞拜然</span><span class="sxs-lookup"><span data-stu-id="37f11-141">Azerbaijan</span></span>       | <span data-ttu-id="37f11-142">蓋亞納</span><span class="sxs-lookup"><span data-stu-id="37f11-142">Guyana</span></span>     | <span data-ttu-id="37f11-143">聖匹島</span><span class="sxs-lookup"><span data-stu-id="37f11-143">Saint Pierre and Miquelon</span></span>   |
> | <span data-ttu-id="37f11-144">貝南</span><span class="sxs-lookup"><span data-stu-id="37f11-144">Benin</span></span>     | <span data-ttu-id="37f11-145">海地</span><span class="sxs-lookup"><span data-stu-id="37f11-145">Haiti</span></span>       | <span data-ttu-id="37f11-146">聖文森及格瑞那丁</span><span class="sxs-lookup"><span data-stu-id="37f11-146">Saint Vincent and the Grenadines</span></span>     |
> | <span data-ttu-id="37f11-147">不丹</span><span class="sxs-lookup"><span data-stu-id="37f11-147">Bhutan</span></span>     | <span data-ttu-id="37f11-148">赫德島及麥當勞群島</span><span class="sxs-lookup"><span data-stu-id="37f11-148">Heard Island and McDonald Islands</span></span>       | <span data-ttu-id="37f11-149">薩摩亞獨立國</span><span class="sxs-lookup"><span data-stu-id="37f11-149">Samoa</span></span>     |
> | <span data-ttu-id="37f11-150">波奈</span><span class="sxs-lookup"><span data-stu-id="37f11-150">Bonaire</span></span>     | <span data-ttu-id="37f11-151">曼城島</span><span class="sxs-lookup"><span data-stu-id="37f11-151">Isle of Man</span></span>     | <span data-ttu-id="37f11-152">聖馬利諾</span><span class="sxs-lookup"><span data-stu-id="37f11-152">San Marino</span></span>     |
> | <span data-ttu-id="37f11-153">布威島</span><span class="sxs-lookup"><span data-stu-id="37f11-153">Bouvet Island</span></span>     | <span data-ttu-id="37f11-154">尖棉</span><span class="sxs-lookup"><span data-stu-id="37f11-154">Jan Mayen</span></span>     | <span data-ttu-id="37f11-155">聖多美普林西比</span><span class="sxs-lookup"><span data-stu-id="37f11-155">São Tomé and Príncipe</span></span>   |
> | <span data-ttu-id="37f11-156">英屬印度洋領土</span><span class="sxs-lookup"><span data-stu-id="37f11-156">British Indian Ocean Territory</span></span>       | <span data-ttu-id="37f11-157">澤西島</span><span class="sxs-lookup"><span data-stu-id="37f11-157">Jersey</span></span>     | <span data-ttu-id="37f11-158">塞席爾</span><span class="sxs-lookup"><span data-stu-id="37f11-158">Seychelles</span></span>   |
> | <span data-ttu-id="37f11-159">英屬維爾京群島</span><span class="sxs-lookup"><span data-stu-id="37f11-159">British Virgin Islands</span></span>     | <span data-ttu-id="37f11-160">吉里巴斯</span><span class="sxs-lookup"><span data-stu-id="37f11-160">Kiribati</span></span>       | <span data-ttu-id="37f11-161">獅子山</span><span class="sxs-lookup"><span data-stu-id="37f11-161">Sierra Leone</span></span>   |
> | <span data-ttu-id="37f11-162">布吉納法索</span><span class="sxs-lookup"><span data-stu-id="37f11-162">Burkina Faso</span></span>     | <span data-ttu-id="37f11-163">科索沃</span><span class="sxs-lookup"><span data-stu-id="37f11-163">Kosovo</span></span>     | <span data-ttu-id="37f11-164">聖佑達修斯</span><span class="sxs-lookup"><span data-stu-id="37f11-164">Sint Eustatius</span></span>     |
> | <span data-ttu-id="37f11-165">蒲隆地</span><span class="sxs-lookup"><span data-stu-id="37f11-165">Burundi</span></span>     | <span data-ttu-id="37f11-166">寮國</span><span class="sxs-lookup"><span data-stu-id="37f11-166">Laos</span></span>     | <span data-ttu-id="37f11-167">荷屬聖馬丁</span><span class="sxs-lookup"><span data-stu-id="37f11-167">Sint Maarten</span></span>     |
> | <span data-ttu-id="37f11-168">柬埔寨</span><span class="sxs-lookup"><span data-stu-id="37f11-168">Cambodia</span></span>     | <span data-ttu-id="37f11-169">賴索托</span><span class="sxs-lookup"><span data-stu-id="37f11-169">Lesotho</span></span>     | <span data-ttu-id="37f11-170">索羅門群島</span><span class="sxs-lookup"><span data-stu-id="37f11-170">Solomon Islands</span></span>     |
> | <span data-ttu-id="37f11-171">中非共和國</span><span class="sxs-lookup"><span data-stu-id="37f11-171">Central African Republic</span></span>     | <span data-ttu-id="37f11-172">賴比瑞亞</span><span class="sxs-lookup"><span data-stu-id="37f11-172">Liberia</span></span>     | <span data-ttu-id="37f11-173">索馬利亞</span><span class="sxs-lookup"><span data-stu-id="37f11-173">Somalia</span></span>     |
> | <span data-ttu-id="37f11-174">查德</span><span class="sxs-lookup"><span data-stu-id="37f11-174">Chad</span></span>     | <span data-ttu-id="37f11-175">馬達加斯加</span><span class="sxs-lookup"><span data-stu-id="37f11-175">Madagascar</span></span>     | <span data-ttu-id="37f11-176">南喬治亞與南三明治群島</span><span class="sxs-lookup"><span data-stu-id="37f11-176">South Georgia and South Sandwich Islands</span></span>     |
> | <span data-ttu-id="37f11-177">中國</span><span class="sxs-lookup"><span data-stu-id="37f11-177">China</span></span>     | <span data-ttu-id="37f11-178">馬拉威</span><span class="sxs-lookup"><span data-stu-id="37f11-178">Malawi</span></span>     | <span data-ttu-id="37f11-179">南蘇丹</span><span class="sxs-lookup"><span data-stu-id="37f11-179">South Sudan</span></span>     |
> | <span data-ttu-id="37f11-180">聖誕島</span><span class="sxs-lookup"><span data-stu-id="37f11-180">Christmas Island</span></span>     | <span data-ttu-id="37f11-181">馬爾地夫</span><span class="sxs-lookup"><span data-stu-id="37f11-181">Maldives</span></span>     | <span data-ttu-id="37f11-182">聖赫勒拿、阿森松、特里斯坦達庫尼亞群島</span><span class="sxs-lookup"><span data-stu-id="37f11-182">St Helena, Ascension, Tristan da Cunha</span></span>     |
> | <span data-ttu-id="37f11-183">可可斯群島</span><span class="sxs-lookup"><span data-stu-id="37f11-183">Cocos (Keeling) Islands</span></span>     | <span data-ttu-id="37f11-184">馬利</span><span class="sxs-lookup"><span data-stu-id="37f11-184">Mali</span></span>     | <span data-ttu-id="37f11-185">蘇利南</span><span class="sxs-lookup"><span data-stu-id="37f11-185">Suriname</span></span>     |
> | <span data-ttu-id="37f11-186">葛摩</span><span class="sxs-lookup"><span data-stu-id="37f11-186">Comoros</span></span>     | <span data-ttu-id="37f11-187">馬紹爾群島</span><span class="sxs-lookup"><span data-stu-id="37f11-187">Marshall Islands</span></span>     | <span data-ttu-id="37f11-188">冷岸</span><span class="sxs-lookup"><span data-stu-id="37f11-188">Svalbard</span></span>     |
> | <span data-ttu-id="37f11-189">剛果共和國</span><span class="sxs-lookup"><span data-stu-id="37f11-189">Congo</span></span>     | <span data-ttu-id="37f11-190">馬丁尼克</span><span class="sxs-lookup"><span data-stu-id="37f11-190">Martinique</span></span>     | <span data-ttu-id="37f11-191">史瓦濟蘭</span><span class="sxs-lookup"><span data-stu-id="37f11-191">Swaziland</span></span>     |
> | <span data-ttu-id="37f11-192">剛果民主共和國 (DRC)</span><span class="sxs-lookup"><span data-stu-id="37f11-192">Congo (DRC)</span></span>     | <span data-ttu-id="37f11-193">茅利塔尼亞</span><span class="sxs-lookup"><span data-stu-id="37f11-193">Mauritania</span></span>     | <span data-ttu-id="37f11-194">東帝汶</span><span class="sxs-lookup"><span data-stu-id="37f11-194">Timor-Leste</span></span>   |
> | <span data-ttu-id="37f11-195">柯克群島</span><span class="sxs-lookup"><span data-stu-id="37f11-195">Cook Islands</span></span>     | <span data-ttu-id="37f11-196">馬約特島</span><span class="sxs-lookup"><span data-stu-id="37f11-196">Mayotte</span></span>     | <span data-ttu-id="37f11-197">多哥</span><span class="sxs-lookup"><span data-stu-id="37f11-197">Togo</span></span>   |
> | <span data-ttu-id="37f11-198">吉布地</span><span class="sxs-lookup"><span data-stu-id="37f11-198">Djibouti</span></span>     | <span data-ttu-id="37f11-199">密克羅尼西亞</span><span class="sxs-lookup"><span data-stu-id="37f11-199">Micronesia</span></span>     | <span data-ttu-id="37f11-200">托克勞群島</span><span class="sxs-lookup"><span data-stu-id="37f11-200">Tokelau</span></span>   |
> | <span data-ttu-id="37f11-201">多米尼克</span><span class="sxs-lookup"><span data-stu-id="37f11-201">Dominica</span></span>     | <span data-ttu-id="37f11-202">蒙特色拉特島</span><span class="sxs-lookup"><span data-stu-id="37f11-202">Montserrat</span></span>     | <span data-ttu-id="37f11-203">東加</span><span class="sxs-lookup"><span data-stu-id="37f11-203">Tonga</span></span>   |
> | <span data-ttu-id="37f11-204">赤道幾內亞</span><span class="sxs-lookup"><span data-stu-id="37f11-204">Equatorial Guinea</span></span>     | <span data-ttu-id="37f11-205">莫三比克</span><span class="sxs-lookup"><span data-stu-id="37f11-205">Mozambique</span></span>     | <span data-ttu-id="37f11-206">土克斯及開科斯群島</span><span class="sxs-lookup"><span data-stu-id="37f11-206">Turks and Caicos Islands</span></span>   |
> | <span data-ttu-id="37f11-207">厄利垂亞</span><span class="sxs-lookup"><span data-stu-id="37f11-207">Eritrea</span></span>     | <span data-ttu-id="37f11-208">緬甸</span><span class="sxs-lookup"><span data-stu-id="37f11-208">Myanmar</span></span>     | <span data-ttu-id="37f11-209">吐瓦魯</span><span class="sxs-lookup"><span data-stu-id="37f11-209">Tuvalu</span></span>   |
> | <span data-ttu-id="37f11-210">福克蘭群島</span><span class="sxs-lookup"><span data-stu-id="37f11-210">Falkland Islands</span></span>     | <span data-ttu-id="37f11-211">諾魯</span><span class="sxs-lookup"><span data-stu-id="37f11-211">Nauru</span></span>     | <span data-ttu-id="37f11-212">美國外島</span><span class="sxs-lookup"><span data-stu-id="37f11-212">U.S. Outlying Islands</span></span>   |
> | <span data-ttu-id="37f11-213">法屬圭亞那</span><span class="sxs-lookup"><span data-stu-id="37f11-213">French Guiana</span></span>     | <span data-ttu-id="37f11-214">新喀里多尼亞群島</span><span class="sxs-lookup"><span data-stu-id="37f11-214">New Caledonia</span></span>     | <span data-ttu-id="37f11-215">萬那杜</span><span class="sxs-lookup"><span data-stu-id="37f11-215">Vanuatu</span></span>   |
> | <span data-ttu-id="37f11-216">法屬玻里尼西亞</span><span class="sxs-lookup"><span data-stu-id="37f11-216">French Polynesia</span></span>     | <span data-ttu-id="37f11-217">尼日</span><span class="sxs-lookup"><span data-stu-id="37f11-217">Niger</span></span>     | <span data-ttu-id="37f11-218">梵蒂岡</span><span class="sxs-lookup"><span data-stu-id="37f11-218">Vatican City</span></span>   |
> | <span data-ttu-id="37f11-219">法屬南半球領土</span><span class="sxs-lookup"><span data-stu-id="37f11-219">French Southern Territories</span></span>     | <span data-ttu-id="37f11-220">紐威島</span><span class="sxs-lookup"><span data-stu-id="37f11-220">Niue</span></span>     | <span data-ttu-id="37f11-221">瓦利斯及福杜納</span><span class="sxs-lookup"><span data-stu-id="37f11-221">Wallis and Futuna</span></span>   |
> | <span data-ttu-id="37f11-222">加彭</span><span class="sxs-lookup"><span data-stu-id="37f11-222">Gabon</span></span>     | <span data-ttu-id="37f11-223">諾福克島</span><span class="sxs-lookup"><span data-stu-id="37f11-223">Norfolk Island</span></span>     | <span data-ttu-id="37f11-224">葉門</span><span class="sxs-lookup"><span data-stu-id="37f11-224">Yemen</span></span>   |
> | <span data-ttu-id="37f11-225">甘比亞</span><span class="sxs-lookup"><span data-stu-id="37f11-225">Gambia</span></span>     | <span data-ttu-id="37f11-226">北馬里安納群島</span><span class="sxs-lookup"><span data-stu-id="37f11-226">Northern Mariana Islands</span></span>     |    |
> | <span data-ttu-id="37f11-227">直布羅陀</span><span class="sxs-lookup"><span data-stu-id="37f11-227">Gibraltar</span></span>     | <span data-ttu-id="37f11-228">帛琉</span><span class="sxs-lookup"><span data-stu-id="37f11-228">Palau</span></span>       |    |

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="37f11-229">代表客戶購買軟體訂閱</span><span class="sxs-lookup"><span data-stu-id="37f11-229">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="37f11-230">若要代表客戶購買軟體訂閱：</span><span class="sxs-lookup"><span data-stu-id="37f11-230">To buy software subscriptions on behalf of a customer:</span></span>

1. <span data-ttu-id="37f11-231">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="37f11-231">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="37f11-232">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="37f11-232">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="37f11-233">在客戶的詳細資料頁面中選取 [新增產品]，然後依照畫面上的指示建立訂單並支付其費用。</span><span class="sxs-lookup"><span data-stu-id="37f11-233">From the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="37f11-234">除了澳洲和巴西以外，所有商業客戶定價都不含稅金。</span><span class="sxs-lookup"><span data-stu-id="37f11-234">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="37f11-235">澳洲和巴西的價格則包含稅金。</span><span class="sxs-lookup"><span data-stu-id="37f11-235">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="37f11-236">啟用及管理軟體訂閱</span><span class="sxs-lookup"><span data-stu-id="37f11-236">Activate and manage software subscriptions</span></span>

<span data-ttu-id="37f11-237">購買軟體訂閱後，請依照下列步驟加以下載。</span><span class="sxs-lookup"><span data-stu-id="37f11-237">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="37f11-238">您必須是系統管理代理人，才能下載軟體並取得啟用金鑰。</span><span class="sxs-lookup"><span data-stu-id="37f11-238">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="37f11-239">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="37f11-239">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="37f11-240">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="37f11-240">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="37f11-241">移至客戶的詳細資料頁面，然後選取 [軟體]。</span><span class="sxs-lookup"><span data-stu-id="37f11-241">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="37f11-242">您會看到您已代表客戶購買的所有軟體清單。</span><span class="sxs-lookup"><span data-stu-id="37f11-242">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 

4. <span data-ttu-id="37f11-243">展開您要下載的產品。</span><span class="sxs-lookup"><span data-stu-id="37f11-243">Expand the product you want to download.</span></span> <span data-ttu-id="37f11-244">在 [選取產品] 欄位中，選取您想要的 [版本]、[語言] 和 [檔案類型/OS]。</span><span class="sxs-lookup"><span data-stu-id="37f11-244">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 

5. <span data-ttu-id="37f11-245">選取 [提交] 以顯示特定產品。</span><span class="sxs-lookup"><span data-stu-id="37f11-245">Select **Submit** to display the specific products.</span></span> 

6. <span data-ttu-id="37f11-246">選取 [取得金鑰和下載項目]。</span><span class="sxs-lookup"><span data-stu-id="37f11-246">Select **Get keys and downloads**.</span></span> 

7. <span data-ttu-id="37f11-247">選取 [下載] 以開始下載，或選取 [複製連結] 以複製連結並將其傳送給客戶。</span><span class="sxs-lookup"><span data-stu-id="37f11-247">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="37f11-248">此連結會在兩個星期後或下載 50 次後到期 (視何者先發生)。</span><span class="sxs-lookup"><span data-stu-id="37f11-248">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="37f11-249">連結過期之後，請回到此頁面並再次選取 [取得金鑰和下載項目]，以再啟用另外兩週或 50 次下載。</span><span class="sxs-lookup"><span data-stu-id="37f11-249">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="37f11-250">您可以依需求執行此動作，次數不限。</span><span class="sxs-lookup"><span data-stu-id="37f11-250">You can do this as many times as you need to.</span></span> 

## <a name="server-subscription-download-and-license-keys-available-through-microsoft-365-admin-center-for-customers"></a><span data-ttu-id="37f11-251">可以透過 Microsoft 365 系統管理中心為客戶提供伺服器訂閱下載和授權金鑰</span><span class="sxs-lookup"><span data-stu-id="37f11-251">Server subscription download and license keys available through Microsoft 365 Admin Center for customers</span></span> 

<span data-ttu-id="37f11-252">您的客戶能夠從 Microsoft 365 系統管理中心取得雲端解決方案提供者伺服器訂閱授權金鑰和下載。</span><span class="sxs-lookup"><span data-stu-id="37f11-252">Your customers will be able to get CSP server subscription license keys and downloads from Microsoft 365 Admin Center.</span></span> <span data-ttu-id="37f11-253">若要查看其雲端解決方案提供者伺服器訂閱授權金鑰和下載，客戶必須前往 [Microsoft 365 系統管理中心] > [計費] > 您的產品 > [軟體] 索引標籤。如需詳細資訊，請參閱 [[計費] 底下的 [軟體] 索引標籤](https://docs.microsoft.com/microsoft-365/admin/whats-new-in-preview#billing--subscriptions)。</span><span class="sxs-lookup"><span data-stu-id="37f11-253">To see their CSP server subscription license keys and downloads, customer must go to Microsoft 365 Admin Center > **Billing > Your products > Software tab**. For more details refer [Software Tab under Billing](https://docs.microsoft.com/microsoft-365/admin/whats-new-in-preview#billing--subscriptions).</span></span>  

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="37f11-254">檢視軟體金鑰存取和軟體下載的活動</span><span class="sxs-lookup"><span data-stu-id="37f11-254">View activity for software key access and software downloads</span></span>

<span data-ttu-id="37f11-255">基於稽核或合規性目的，您可能需要檢查曾存取伺服器訂閱軟體金鑰或下載伺服器訂閱軟體的使用者清單。</span><span class="sxs-lookup"><span data-stu-id="37f11-255">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="37f11-256">請使用下列程序來存取這項資訊。</span><span class="sxs-lookup"><span data-stu-id="37f11-256">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="37f11-257">您必須是全域管理員、帳戶管理員、推薦管理員或行銷內容管理員，才能看到這些活動記錄。</span><span class="sxs-lookup"><span data-stu-id="37f11-257">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1. <span data-ttu-id="37f11-258">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="37f11-258">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="37f11-259">選取位於右上角的齒輪圖示。</span><span class="sxs-lookup"><span data-stu-id="37f11-259">Select the gear icon from the upper right corner.</span></span>

3. <span data-ttu-id="37f11-260">在功能表中，選取 [活動記錄]。</span><span class="sxs-lookup"><span data-stu-id="37f11-260">In the menu, select **Activity log**.</span></span>

4. <span data-ttu-id="37f11-261">輸入您要查看的活動所屬的日期範圍。</span><span class="sxs-lookup"><span data-stu-id="37f11-261">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="37f11-262">活動記錄會顯示在您指定的時間內曾存取軟體金鑰或下載軟體的使用者清單。</span><span class="sxs-lookup"><span data-stu-id="37f11-262">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="37f11-263">取消購買</span><span class="sxs-lookup"><span data-stu-id="37f11-263">Cancel a purchase</span></span>

<span data-ttu-id="37f11-264">您可以在購買日期起算的 60 天內取消軟體購買。</span><span class="sxs-lookup"><span data-stu-id="37f11-264">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="37f11-265">如果您在這前 60 天的期間內取消購買，則無須支付提前終止費用。</span><span class="sxs-lookup"><span data-stu-id="37f11-265">If you cancel within this first 60-day period, you will not be charged an early termination fee.</span></span> <span data-ttu-id="37f11-266">在 60 天後，您就無法再取消購買。</span><span class="sxs-lookup"><span data-stu-id="37f11-266">After 60 days, you can no longer cancel a purchase.</span></span> <span data-ttu-id="37f11-267">(請參閱注意事項，以了解此取消規則的主要限制。</span><span class="sxs-lookup"><span data-stu-id="37f11-267">(See Note for key restrictions to this cancellation rule.</span></span> <span data-ttu-id="37f11-268">若要了解取消軟體購買的後續事項，請參閱下列步驟之後的重要注意事項。)</span><span class="sxs-lookup"><span data-stu-id="37f11-268">To learn about what happens after you cancel a software purchase, see also Important note after these steps.)</span></span> 

>[!NOTE]
><span data-ttu-id="37f11-269">下列關於取消購買的步驟僅適用於能夠在特定時間範圍內取消購買的軟體，例如在購買後的 60 天內。</span><span class="sxs-lookup"><span data-stu-id="37f11-269">The following steps to cancel a purchase apply only to software that qualifies for cancellation within a specific cancellation window, such as within the first 60 days after purchase.</span></span> <span data-ttu-id="37f11-270">這些步驟也不適用於 Azure 中的 SUSE Linux 或 RedHat 軟體方案。</span><span class="sxs-lookup"><span data-stu-id="37f11-270">These steps also do not apply to a SUSE Linux or RedHat software plan in Azure.</span></span> <span data-ttu-id="37f11-271">目前，您無法取消或交換 SUSE 或 RedHat 軟體方案。</span><span class="sxs-lookup"><span data-stu-id="37f11-271">At this time, you cannot cancel or exchange a SUSE or RedHat software plan.</span></span> <span data-ttu-id="37f11-272">請[深入了解](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges) SUSE Linux 或 RedHat 方案的使用方式。</span><span class="sxs-lookup"><span data-stu-id="37f11-272">[Learn more](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges) about using SUSE Linux or RedHat plans.</span></span>

<span data-ttu-id="37f11-273">請依照下列步驟取消購買：</span><span class="sxs-lookup"><span data-stu-id="37f11-273">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="37f11-274">您必須是系統管理代理人，才能取消購買。</span><span class="sxs-lookup"><span data-stu-id="37f11-274">You must be an Admin agent to cancel a purchase.</span></span> <span data-ttu-id="37f11-275">下列步驟說明如何在合作夥伴中心儀表板中取消購買。</span><span class="sxs-lookup"><span data-stu-id="37f11-275">The following steps describe how to cancel a purchase in the Partner Center dashboard.</span></span> <span data-ttu-id="37f11-276">您也可以使用[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases) 來執行此動作。</span><span class="sxs-lookup"><span data-stu-id="37f11-276">You can also do this using the [Partner Center API](https://docs.microsoft.com/partner-center/develop/cancel-software-purchases).</span></span>

1. <span data-ttu-id="37f11-277">開始進行取消程序之前，請確定您具有下列各項：</span><span class="sxs-lookup"><span data-stu-id="37f11-277">Before you start the cancellation process, make sure you have the following:</span></span>

    - <span data-ttu-id="37f11-278">客戶的名稱、租用戶 GUID 或網域名稱</span><span class="sxs-lookup"><span data-stu-id="37f11-278">The customer's name, tenant GUID or domain name</span></span>

    - <span data-ttu-id="37f11-279">您要取消的產品名稱</span><span class="sxs-lookup"><span data-stu-id="37f11-279">The name of the product you want to cancel</span></span>
    
    - <span data-ttu-id="37f11-280">訂單識別碼</span><span class="sxs-lookup"><span data-stu-id="37f11-280">The Order ID</span></span>

2. <span data-ttu-id="37f11-281">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="37f11-281">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="37f11-282">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="37f11-282">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="37f11-283">在客戶的詳細資料頁面上選取 [軟體]，以查看為客戶購買的軟體清單。</span><span class="sxs-lookup"><span data-stu-id="37f11-283">On the customer's details page, select **Software** to see the list of software purchased for the customer.</span></span> 

5. <span data-ttu-id="37f11-284">找出您要取消的軟體購買，然後選取 [取消]。</span><span class="sxs-lookup"><span data-stu-id="37f11-284">Locate the software purchase you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="37f11-285">此時會出現一個對話方塊。</span><span class="sxs-lookup"><span data-stu-id="37f11-285">A dialog box will appear.</span></span>

6. <span data-ttu-id="37f11-286">在 [訂單號碼] 下拉式清單中，選取您要取消的正確訂單識別碼。</span><span class="sxs-lookup"><span data-stu-id="37f11-286">From the Order number drop-down list, select the correct order ID number you want to cancel.</span></span> <span data-ttu-id="37f11-287">(您可以在客戶的 [訂單歷程記錄] 頁面中深入了解訂單或訂單識別碼的詳細資訊。)</span><span class="sxs-lookup"><span data-stu-id="37f11-287">(You can learn more information about an order or order ID number from the customer's **Order history** page.)</span></span>

7. <span data-ttu-id="37f11-288">選取核取方塊以確認您已閱讀關於取消的**重要**訊息。</span><span class="sxs-lookup"><span data-stu-id="37f11-288">Select the checkbox to acknowledge that you have read the **Important** message concerning cancellation.</span></span> <span data-ttu-id="37f11-289">(請參閱下列**重要**注意事項，以深入了解取消購買的後續事務)。</span><span class="sxs-lookup"><span data-stu-id="37f11-289">(Refer to the **Important** note below to learn more about what happens after you cancel a purchase.)</span></span>

8. <span data-ttu-id="37f11-290">選取 [提交] 以取消購買。</span><span class="sxs-lookup"><span data-stu-id="37f11-290">Select **Submit** to cancel your purchase.</span></span> <span data-ttu-id="37f11-291">如果您想要取消客戶的多個訂單，您必須對每個唯一的訂單識別碼再次執行步驟 4 到 6。</span><span class="sxs-lookup"><span data-stu-id="37f11-291">If you want to cancel multiple orders for a customer, you will need to perform Steps 4 through 6 again for each, unique order ID number.</span></span>

<span data-ttu-id="37f11-292">當您嘗試取消訂單時，合作夥伴中心也可能會為您提供其他資訊 (顯示在 [訂單號碼] 下拉式清單下方)。</span><span class="sxs-lookup"><span data-stu-id="37f11-292">When you attempt to cancel an order, Partner Center may also give you other information (that appears below the Order number drop-down list).</span></span> <span data-ttu-id="37f11-293">這類資訊可能包括：</span><span class="sxs-lookup"><span data-stu-id="37f11-293">This information can include:</span></span>

- <span data-ttu-id="37f11-294">您還剩下多少天可取消該訂單</span><span class="sxs-lookup"><span data-stu-id="37f11-294">How many days remain for you to cancel that particular order</span></span>

- <span data-ttu-id="37f11-295">您是否已超過取消時間範圍，而已無法再取消訂單</span><span class="sxs-lookup"><span data-stu-id="37f11-295">Whether you have already passed the cancellation window and can no longer cancel the order</span></span>

- <span data-ttu-id="37f11-296">如果我們需要您提供更多關於取消要求的資訊，您可能會收到**客戶支援要求**表單的連結。</span><span class="sxs-lookup"><span data-stu-id="37f11-296">If we need more information about your cancellation request, you may be given a link to a **customer support request** form.</span></span>

>[!IMPORTANT]
><span data-ttu-id="37f11-297">在您取消訂單後，將會出現確認取消的訊息。</span><span class="sxs-lookup"><span data-stu-id="37f11-297">After you cancel an order, a message confirming your cancellation will appear.</span></span> <span data-ttu-id="37f11-298">不過，最多可能需經過 15 分鐘的延遲，取消的訂單才會顯示在合作夥伴中心儀表板上。</span><span class="sxs-lookup"><span data-stu-id="37f11-298">There may be a delay of up to 15 minutes, however, before the cancellation appears on the Partner Center dashboard.</span></span> 

### <a name="post-cancellation-details"></a><span data-ttu-id="37f11-299">取消後的詳細資料</span><span class="sxs-lookup"><span data-stu-id="37f11-299">Post-cancellation details</span></span>

<span data-ttu-id="37f11-300">在您取消購買後：</span><span class="sxs-lookup"><span data-stu-id="37f11-300">After you cancel a purchase:</span></span>

- <span data-ttu-id="37f11-301">所有相關的軟體金鑰和下載連結都會撤銷。</span><span class="sxs-lookup"><span data-stu-id="37f11-301">All related software keys and download links will be revoked.</span></span> <span data-ttu-id="37f11-302">這表示您或客戶都不能再使用與此購買有關的軟體金鑰和下載連結。</span><span class="sxs-lookup"><span data-stu-id="37f11-302">This means neither you nor your customer can use the software keys and download links any longer related to this purchase.</span></span> <span data-ttu-id="37f11-303">您和客戶須負責停止使用所有已取消的軟體。</span><span class="sxs-lookup"><span data-stu-id="37f11-303">You and your customer are responsible for discontinuing the use of all canceled software.</span></span> <span data-ttu-id="37f11-304">您也必須負責解除安裝已取消的軟體，並移除任何相關的軟體下載和連結。</span><span class="sxs-lookup"><span data-stu-id="37f11-304">You are also responsible for uninstalling the canceled software and removing any, related software downloads and links.</span></span>

- <span data-ttu-id="37f11-305">已取消的項目仍會顯示在客戶的軟體詳細資料頁面上，但啟用金鑰將無法使用。</span><span class="sxs-lookup"><span data-stu-id="37f11-305">The canceled item will still appear on the customer's Software details page but the activation key will not be available.</span></span>

- <span data-ttu-id="37f11-306">對於已取消的訂單，其點數將會出現在您下個月的發票上。</span><span class="sxs-lookup"><span data-stu-id="37f11-306">A credit for the canceled order will appear on your next monthly invoice.</span></span> <span data-ttu-id="37f11-307">永久軟體會收到 100% 的點數，而軟體訂閱則會收到按比例計算的點數。</span><span class="sxs-lookup"><span data-stu-id="37f11-307">Perpetual software will receive a 100% credit and software subscriptions will receive a prorated credit.</span></span>

### <a name="submit-a-customer-support-request-to-cancel-a-purchase"></a><span data-ttu-id="37f11-308">提交客戶支援要求以取消購買</span><span class="sxs-lookup"><span data-stu-id="37f11-308">Submit a customer support request to cancel a purchase</span></span>

<span data-ttu-id="37f11-309">如果您嘗試透過合作夥伴中心來取消軟體購買，但被告知需提供更多資訊，並填寫客戶支援要求表單，下列步驟可能有所幫助：</span><span class="sxs-lookup"><span data-stu-id="37f11-309">If you tried to cancel a software purchase via Partner Center but were told to provide more information and fill out a customer support request form, these steps may help you:</span></span>

1. <span data-ttu-id="37f11-310">當您從 [取消購買] 視窗選取 [客戶支援要求] 連結時，將會開啟 [回報合作夥伴中心相關問題] 頁面。</span><span class="sxs-lookup"><span data-stu-id="37f11-310">When you select the **customer support request** link from the Cancel purchase window, the **Report a problem with Partner Center** page will open.</span></span>

2. <span data-ttu-id="37f11-311">在 [詳細資料] 下的 [問題類型] 清單中，選取 [代表客戶的雲端解決方案提供者購買/退款]。</span><span class="sxs-lookup"><span data-stu-id="37f11-311">Under **Details**, in the Type of problem list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

3. <span data-ttu-id="37f11-312">填寫 [影響] 和 [標題] 欄位。</span><span class="sxs-lookup"><span data-stu-id="37f11-312">Fill in the Impact and Title fields.</span></span>

4. <span data-ttu-id="37f11-313">在 [描述] 欄位中，提供下列各項：</span><span class="sxs-lookup"><span data-stu-id="37f11-313">In the Description field, provide the following:</span></span>

    - <span data-ttu-id="37f11-314">客戶租用戶 GUID 或網域名稱</span><span class="sxs-lookup"><span data-stu-id="37f11-314">The customer tenant GUID or domain name</span></span>
    
    - <span data-ttu-id="37f11-315">訂單識別碼或訂閱識別碼</span><span class="sxs-lookup"><span data-stu-id="37f11-315">Order ID or Subscription ID</span></span>
    
    - <span data-ttu-id="37f11-316">退款原因</span><span class="sxs-lookup"><span data-stu-id="37f11-316">Refund reason</span></span>

    - <span data-ttu-id="37f11-317">要求金額</span><span class="sxs-lookup"><span data-stu-id="37f11-317">Amount requested</span></span>

5. <span data-ttu-id="37f11-318">在 [連絡人] 欄位中，輸入您的名稱、電子郵件地址及電話號碼。</span><span class="sxs-lookup"><span data-stu-id="37f11-318">In the Contact field, enter your name, email address, and phone number.</span></span>

6. <span data-ttu-id="37f11-319">如果您因故需附加檔案，請選取 [新增檔案]。</span><span class="sxs-lookup"><span data-stu-id="37f11-319">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="37f11-320">這是選擇性步驟。</span><span class="sxs-lookup"><span data-stu-id="37f11-320">This step is optional.</span></span>

7. <span data-ttu-id="37f11-321">完成時，選取 [提交]。</span><span class="sxs-lookup"><span data-stu-id="37f11-321">When you're finished, select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="37f11-322">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="37f11-322">Next steps</span></span>

- [<span data-ttu-id="37f11-323">使用合作夥伴中心以銷售商業市集產品的客戶訂閱</span><span class="sxs-lookup"><span data-stu-id="37f11-323">Use Partner Center to sell customers subscriptions to commercial marketplace products</span></span>](sell-marketplace-products.md)
 
- [<span data-ttu-id="37f11-324">在合作夥伴中心指派 Azure 訂用帳戶給您的客戶</span><span class="sxs-lookup"><span data-stu-id="37f11-324">Assigning Azure subscriptions to customers in Partner Center</span></span>](assign-azure-subscriptions.md)