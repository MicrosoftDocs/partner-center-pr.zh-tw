---
title: 合併夥伴帳戶與另一個夥伴帳戶 |合作夥伴中心
ms.topic: article
ms.date: 02/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 具有 mpn 識別碼和合作夥伴中心帳戶的公司可以合併其帳戶。
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 5194f9ca6bcd843a748a2f6035fdd14422712548
ms.sourcegitcommit: 5379fbbe7fab1a26314c42bca40674c7f2faa432
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/27/2020
ms.locfileid: "77672650"
---
# <a name="merging-your-partner-account-with-another-partner-account"></a><span data-ttu-id="bb6a3-103">合併夥伴帳戶與另一個夥伴帳戶</span><span class="sxs-lookup"><span data-stu-id="bb6a3-103">Merging your partner account with another partner account</span></span>

<span data-ttu-id="bb6a3-104">**相關角色**</span><span class="sxs-lookup"><span data-stu-id="bb6a3-104">**Applicable roles**</span></span>

- <span data-ttu-id="bb6a3-105">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="bb6a3-105">Account admin</span></span>
- <span data-ttu-id="bb6a3-106">MPN 管理員</span><span class="sxs-lookup"><span data-stu-id="bb6a3-106">MPN admin</span></span>

<span data-ttu-id="bb6a3-107">有兩個或更多公司使用中的 Microsoft 合作夥伴，並在合作夥伴中心擁有帳戶，可以選擇合併他們的帳戶。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-107">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span> 

## <a name="what-happens-when-two-partners-decide-to-merge-their-partner-center-accounts"></a><span data-ttu-id="bb6a3-108">當兩個合作夥伴決定合併其合作夥伴中心帳戶時，會發生什麼事</span><span class="sxs-lookup"><span data-stu-id="bb6a3-108">What happens when two partners decide to merge their Partner Center accounts</span></span>

- <span data-ttu-id="bb6a3-109">起始合併的夥伴將會是合作夥伴通用帳戶（PGA）。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-109">The partner who initiates the merger will be the Partner global account (PGA).</span></span> 

- <span data-ttu-id="bb6a3-110">受邀組織的 PGA 會成為起始公司的位置。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-110">The invited organization’s PGA becomes a location of the initiating company.</span></span>  

- <span data-ttu-id="bb6a3-111">合併帳戶的所有位置都會變成 PGA 底下的位置。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-111">All the locations of the merging account become locations under the PGA.</span></span> 

- <span data-ttu-id="bb6a3-112">帳戶合併完成後，您會在 PGA 設定檔中看到這兩個帳戶的詳細資料，例如位置和使用者。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-112">Once the account merger is complete, you will see both accounts' details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="bb6a3-113">您無法還原此進程。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-113">You can't reverse this process.</span></span> 

- <span data-ttu-id="bb6a3-114">在此合併期間，會保留所有位置的 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-114">All MPN IDs for locations are preserved during this consolidation.</span></span> 

- <span data-ttu-id="bb6a3-115">使用者的角色會一併停用。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-115">Users' roles are brought over.</span></span> <span data-ttu-id="bb6a3-116">例如，如果使用者已是特定位置的獎勵系統管理員，他們在合併之後仍然會有該角色，而且能夠看到他們在合併之前看到的獎勵。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-116">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw before the merger.</span></span> 

- <span data-ttu-id="bb6a3-117">Azure AD 租使用者和 CSP 帳戶不會合並。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-117">Azure AD tenants and CSP accounts aren't merged.</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="bb6a3-118">合併帳戶的觀點</span><span class="sxs-lookup"><span data-stu-id="bb6a3-118">View of merged accounts</span></span>

![合併的帳戶](images/AccountMerge_graphic.png)


## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="bb6a3-120">如果您已受邀將合作夥伴中心帳戶與另一個合作夥伴中心帳戶合併，該怎麼辦</span><span class="sxs-lookup"><span data-stu-id="bb6a3-120">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="bb6a3-121">如果您決定接受合併的邀請：</span><span class="sxs-lookup"><span data-stu-id="bb6a3-121">If you decide to accept the invitation to merge:</span></span>

- <span data-ttu-id="bb6a3-122">您的 MPN 識別碼和位置將會合並至邀請您的合作夥伴帳戶的 PGA。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-122">Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span> 

- <span data-ttu-id="bb6a3-123">您將能夠在 PGA 設定檔下看到所有的帳戶資訊。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-123">You will be able to see all your account information under the PGA profile.</span></span>

- <span data-ttu-id="bb6a3-124">您的使用者將會帶入已合併的帳戶，並將其角色原封不動。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-124">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="bb6a3-125">在合併之後，這兩家公司都將保留現有的權益和專長，直到續約為止。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-125">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="bb6a3-126">在續訂時，系統會將帳戶視為一家公司，而標準更新規則將會生效。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-126">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>  

## <a name="how-benefits-and-competencies-are-affected-when-partners-elect-to-merge-their-accounts"></a><span data-ttu-id="bb6a3-127">當合作夥伴選擇合併其帳戶時，優點和專長的影響</span><span class="sxs-lookup"><span data-stu-id="bb6a3-127">How benefits and competencies are affected when partners elect to merge their accounts</span></span>

- <span data-ttu-id="bb6a3-128">匯總期間會保留所有現有的專長認證（金級/銀級）、購買（地圖/金級/銀級）和相關聯的權益。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-128">All existing competencies (Gold/Silver), purchases (MAPS/Gold/Silver) and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="bb6a3-129">如果這兩家公司都具有相同的專長認證，但其中一家公司的專長認證是金級，而另一家公司是銀級，則將獲得最高專長的專長認證。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-129">If both companies have the same competency but one company's competency is gold and the other company's is silver, the competency with highest proficiency level will be awarded.</span></span> <span data-ttu-id="bb6a3-130">合作夥伴在續訂之前，會有一組銀級和一組黃金優勢。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-130">Partners will have one set of silver and one set of gold benefits for that competency until renewal.</span></span>

- <span data-ttu-id="bb6a3-131">地圖的最高週年日會在合併之後保留。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-131">Highest anniversary date for MAPS will be retained after the merger.</span></span> <span data-ttu-id="bb6a3-132">例如，如果公司1的週年日是2020年6月的地圖更新，而 company 2 的地圖年10月的日是2020，則 Microsoft 將使用10月2020日作為合併公司的新週年日。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-132">For example, if the anniversary date for company 1 is June 2020 for MAPS renewal and the anniversary date for MAPS renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="bb6a3-133">在帳戶合併期間和更新期間，每個帳戶都將保留其對應權益。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-133">During the account merge and until renewal, each account will retain their MAPS benefits.</span></span> <span data-ttu-id="bb6a3-134">更新時，適用標準地圖更新規則。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-134">At renewal, standard MAPs renewal rules apply.</span></span>  

- <span data-ttu-id="bb6a3-135">這兩家公司的 MCP 識別碼關聯將會保留，並與 PGA MPN 識別碼相關聯。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-135">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="bb6a3-136">上市的技術優勢是以專長認證核心權益的形式提供。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-136">Go-to-market technical benefits are offered as competency core benefit.</span></span>  

- <span data-ttu-id="bb6a3-137">所有獎勵都會保留在每個位置。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-137">All incentives are preserved per location.</span></span> 

- <span data-ttu-id="bb6a3-138">Azure 專家的 MSP 權益會保留到續訂為止。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-138">Azure Expert MSP benefits are retained until renewal.</span></span> 

- <span data-ttu-id="bb6a3-139">會保留這兩個帳戶的 Advanced 特殊化。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-139">Advanced specializations across both accounts are retained.</span></span> 

- <span data-ttu-id="bb6a3-140">會保留這兩個帳戶之間的軟體保證券。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-140">Software assurance vouchers across both accounts are retained.</span></span>

## <a name="invite-a-company-to-merge-its-partner-center-account-with-yours"></a><span data-ttu-id="bb6a3-141">邀請公司與您的合作夥伴中心帳戶合併</span><span class="sxs-lookup"><span data-stu-id="bb6a3-141">Invite a company to merge its Partner Center account with yours</span></span> 

><span data-ttu-id="bb6a3-142">下若要執行合併，您必須是公司的 MPN 管理員或帳戶管理員。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-142">[Note] To perform the merger, you must be the MPN admin or the Account admin for your company.</span></span>

1. <span data-ttu-id="bb6a3-143">從您的合作夥伴中心儀表板選取 [**設定**]。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-143">Select **Settings** from your Partner Center dashboard.</span></span>

2. <span data-ttu-id="bb6a3-144">選取 [**帳戶合併**]。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-144">Select **Account merge**.</span></span>

3. <span data-ttu-id="bb6a3-145">新增位於您想要邀請之帳戶的夥伴設定檔中的 MPN 識別碼，以與您合併。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-145">Add the MPN ID located in the Partner profile of the account you want to invite to merge with you.</span></span> <span data-ttu-id="bb6a3-146">您必須使用其合作夥伴全域 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-146">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="bb6a3-147">您不能使用位置 MPN 識別碼。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-147">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="bb6a3-148">當您選取 [**合併**] 時，會將邀請傳送給夥伴公司。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-148">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="bb6a3-149">當他們接受您的要求時，您可以在合作夥伴中心內起始合併。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-149">When they accept your request, you can initiate the merge within Partner Center.</span></span> <span data-ttu-id="bb6a3-150">如果公司拒絕您的合併要求，他們就有機會解釋他們為什麼會拒絕要求。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-150">If the company rejects your request to merge, they have the opportunity to explain why they rejected the request.</span></span> <span data-ttu-id="bb6a3-151">您可以在**合併歷程記錄**下，取得所有帳戶合併的清單。</span><span class="sxs-lookup"><span data-stu-id="bb6a3-151">A list of all your account mergers is available to you under **Merge history**.</span></span>




