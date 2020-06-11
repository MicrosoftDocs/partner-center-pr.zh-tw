---
title: Azure 方案 - 管理訂用帳戶與資源
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解合作夥伴如何使用不同的角色型存取控制 (RBAC) 選項，來對客戶 Azure 資源的操作進行控制和管理。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ea0b7d781cebb963ad802cb73c7d956729dcb2e
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84452625"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a><span data-ttu-id="4b886-103">管理 Azure 方案下的訂用帳戶和資源</span><span class="sxs-lookup"><span data-stu-id="4b886-103">Manage subscriptions and resources under the Azure plan</span></span>

<span data-ttu-id="4b886-104">當您將客戶轉換至 Azure 方案時，預設會在 Azure 中獲指派特殊系統管理權限 (透過代表管理員的訂用帳戶擁有者權限)。</span><span class="sxs-lookup"><span data-stu-id="4b886-104">When you transition a customer to the Azure plan, you are assigned privileged admin rights in Azure (subscription owner rights through admin on behalf of) by default.</span></span>

 > [!NOTE]
 > <span data-ttu-id="4b886-105">客戶可以在訂用帳戶、資源群組或工作負載層級移除 Azure 訂用帳戶的系統管理員權限。</span><span class="sxs-lookup"><span data-stu-id="4b886-105">Admin rights to the Azure subscription can be removed by the customer at a subscription, resource group, or workload level.</span></span> 

 <span data-ttu-id="4b886-106">合作夥伴可以使用透過角色型存取控制功能 (RBAC) 提供的不同選項，在 CSP 中取得客戶 Azure 資源的全天候操作控制和管理。</span><span class="sxs-lookup"><span data-stu-id="4b886-106">Partners can gain 24x7 operational control and management of a customer's Azure resources in CSP by using different options provided through the role-based access control feature (RBAC).</span></span> 

- <span data-ttu-id="4b886-107">**系統管理員代表 (AOBO)** - 使用 [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 時，在合作夥伴租用戶中具有系統管理代理人角色的任何使用者，都將擁有您透過 CSP 計畫所建立 Azure 訂用帳戶的 RBAC 擁有者存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-107">**Admin on Behalf Of (AOBO)** - With [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), any user with the Admin Agent role in the partner tenant will have RBAC owner access to Azure subscriptions that you create through the CSP program.</span></span>

- <span data-ttu-id="4b886-108">**Azure Lighthouse**：AOBO 不允許彈性建立與不同客戶一起使用的不同群組，或為群組或使用者啟用不同的角色。</span><span class="sxs-lookup"><span data-stu-id="4b886-108">**Azure Lighthouse**: AOBO doesn't allow the flexibility to create distinct groups that work with different customers, or to enable different roles for groups or users.</span></span> <span data-ttu-id="4b886-109">使用 Azure Lighthouse，您可以將不同的群組指派給不同的客戶或角色。</span><span class="sxs-lookup"><span data-stu-id="4b886-109">Using Azure Lighthouse, you can assign different groups to different customers or roles.</span></span> <span data-ttu-id="4b886-110">因為使用者會透過 Azure 委派的資源管理來擁有適當的存取層級，所以您可以減少擁有系統管理代理人角色的使用者人數 (因而擁有完整的 AOBO 存取權)。</span><span class="sxs-lookup"><span data-stu-id="4b886-110">Because users will have the appropriate level of access through Azure delegated resource management, you can reduce the number of users who have the Admin Agent role (and thus have full AOBO access).</span></span> <span data-ttu-id="4b886-111">藉由限制對客戶資源的不必要存取來協助改善安全性。</span><span class="sxs-lookup"><span data-stu-id="4b886-111">This helps improve security by limiting unnecessary access to your customers' resources.</span></span> <span data-ttu-id="4b886-112">它也可讓您更有彈性地大規模管理多個客戶。</span><span class="sxs-lookup"><span data-stu-id="4b886-112">It also gives you more flexibility to manage multiple customers at scale.</span></span> <span data-ttu-id="4b886-113">如需詳細資訊，請參閱 [Azure Lighthouse 與雲端解決方案提供者計畫](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider)。</span><span class="sxs-lookup"><span data-stu-id="4b886-113">For more information, read [Azure Lighthouse and the Cloud Solution Provider program](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).</span></span>

-  <span data-ttu-id="4b886-114">**目錄或來賓使用者或[服務主體](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** ：您可以藉由在客戶目錄中新增使用者，或新增來賓使用者並指派特定 RBAC 角色，委派對 CSP 訂用帳戶的細微存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-114">**Directory or Guest Users or [Service Principals](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)**: You can delegate granular access to CSP subscriptions by adding users in the customer directory or adding guest users and assigning specific RBAC roles.</span></span> 

<span data-ttu-id="4b886-115">Microsoft 建議使用者擁有執行其工作所需的最小權限，作為安全性做法。</span><span class="sxs-lookup"><span data-stu-id="4b886-115">Microsoft recommends that users have the minimum permissions they need to perform their work as a security practice.</span></span> <span data-ttu-id="4b886-116">請參閱 [Azure Active Directory Privileged Identity Management 資源](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)。</span><span class="sxs-lookup"><span data-stu-id="4b886-116">See [Azure Active Directory Privileged Identity Management resources](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span> 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a><span data-ttu-id="4b886-117">將您的合作夥伴識別碼 (MPN 識別碼) 連結至您的認證，以管理客戶的 Azure 資源</span><span class="sxs-lookup"><span data-stu-id="4b886-117">Link your partner ID (MPN ID)to your credentials for managing customer's Azure resources</span></span>

<span data-ttu-id="4b886-118">下表顯示用來將您的合作夥伴識別碼與各種 RBAC 存取選項產生關聯的方法。</span><span class="sxs-lookup"><span data-stu-id="4b886-118">The following table shows the methods used to associate your partner ID with various RBAC access options.</span></span>

|<span data-ttu-id="4b886-119">**類別**</span><span class="sxs-lookup"><span data-stu-id="4b886-119">**Category**</span></span>   |<span data-ttu-id="4b886-120">**案例**</span><span class="sxs-lookup"><span data-stu-id="4b886-120">**Scenario**</span></span>   |<span data-ttu-id="4b886-121">**MPN 識別碼關聯**</span><span class="sxs-lookup"><span data-stu-id="4b886-121">**MPN ID association**</span></span>|
|-----------------|:------------------------|:------------------|
|<span data-ttu-id="4b886-122">AOBO</span><span class="sxs-lookup"><span data-stu-id="4b886-122">AOBO</span></span>   |<span data-ttu-id="4b886-123">CSP 直接合作夥伴或間接提供者會為客戶建立訂用帳戶，讓 CSP 直接合作夥伴或間接提供者成為使用 AOBO 作為訂用帳戶的預設擁有者；CSP 直接合作夥伴或間接提供者會使用 AOBO 為間接經銷商授與訂用帳戶的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-123">CSP direct partner or indirect provider creates the subscription for the customer making the CSP direct partner or indirect provider default owner of the subscription using AOBO.; CSP direct partner or indirect provider give indirect reseller access to the subscription using AOBO.</span></span>|<span data-ttu-id="4b886-124">自動 (不需要合作夥伴工作)</span><span class="sxs-lookup"><span data-stu-id="4b886-124">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="4b886-125">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="4b886-125">Azure Lighthouse</span></span>|<span data-ttu-id="4b886-126">合作夥伴會[在 Marketplace 中建立新的受控服務供應項目](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers)。</span><span class="sxs-lookup"><span data-stu-id="4b886-126">Partner creates a new [Managed Services offer in Marketplace](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers).</span></span> <span data-ttu-id="4b886-127">CSP 訂用帳戶已接受此供應項目，合作夥伴可以取得 CSP 訂用帳戶的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-127">This offer is accepted on the CSP subscription and partner gets access to the CSP subscription.</span></span>|<span data-ttu-id="4b886-128">自動 (不需要合作夥伴工作)</span><span class="sxs-lookup"><span data-stu-id="4b886-128">Automatic (no partner work required)</span></span>|
|<span data-ttu-id="4b886-129">Azure Lighthouse</span><span class="sxs-lookup"><span data-stu-id="4b886-129">Azure Lighthouse</span></span>|<span data-ttu-id="4b886-130">合作夥伴在 Azure 訂用帳戶中部署 [ARM 範本 ](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer)</span><span class="sxs-lookup"><span data-stu-id="4b886-130">Partner deploys [ARM template](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) in Azure subscription</span></span>|<span data-ttu-id="4b886-131">合作夥伴必須將 MPN 識別碼與合作夥伴租用戶中的使用者或服務主體產生關聯。</span><span class="sxs-lookup"><span data-stu-id="4b886-131">Partner needs to associate the MPN ID to the user or service principal in the partner tenant.</span></span> <span data-ttu-id="4b886-132">如需詳細資訊 - [連結合作夥伴識別碼](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="4b886-132">For more information - [Link Partner ID](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>|
|<span data-ttu-id="4b886-133">目錄或來賓使用者</span><span class="sxs-lookup"><span data-stu-id="4b886-133">Directory or guest user</span></span>|<span data-ttu-id="4b886-134">夥伴會在客戶目錄中建立新的使用者或服務主體，並為使用者提供 CSP 訂用帳戶的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-134">Partner creates a new user or service principal in the customer directory and gives access to the CSP subscription to the user.</span></span> <span data-ttu-id="4b886-135">合作夥伴會在客戶目錄中建立新的使用者或服務主體。</span><span class="sxs-lookup"><span data-stu-id="4b886-135">Partner creates a new user or service principal in the customer directory.</span></span> <span data-ttu-id="4b886-136">合作夥伴會將使用者新增至群組，並且為群組提供 CSP 訂用帳戶的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-136">Partner adds the user to a group and gives access to the CSP subscription to the group.</span></span>|<span data-ttu-id="4b886-137">合作夥伴必須將 MPN 識別碼與客戶租用戶中的使用者或服務主體產生關聯。</span><span class="sxs-lookup"><span data-stu-id="4b886-137">Partner needs to associate the MPN ID to the user or service principal in the customer tenant.</span></span> <span data-ttu-id="4b886-138">如需詳細資訊 - [連結合作夥伴識別碼](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)。</span><span class="sxs-lookup"><span data-stu-id="4b886-138">For more information - [Link Partner ID](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>|

## <a name="confirm-that-you-have-admin-access"></a><span data-ttu-id="4b886-139">確認您具有系統管理員存取權</span><span class="sxs-lookup"><span data-stu-id="4b886-139">Confirm that you have admin access</span></span>

<span data-ttu-id="4b886-140">您需要系統管理員存取權來管理您的客戶服務，並接收所獲得的信用點數。</span><span class="sxs-lookup"><span data-stu-id="4b886-140">You require admin access to manage your customer's services and to received earned credits.</span></span> <span data-ttu-id="4b886-141">如需所獲得信用點數的詳細資訊，請參閱[合作夥伴所獲得的信用點數](partner-earned-credit.md)。</span><span class="sxs-lookup"><span data-stu-id="4b886-141">Read [Partner earned credits](partner-earned-credit.md) for detailed information on earned credits.</span></span> <span data-ttu-id="4b886-142">您有兩種方式可確保您知道您具有系統管理員存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-142">You have two ways to make sure you know that you have admin access.</span></span>

- <span data-ttu-id="4b886-143">檢閱每日使用量檔案 - 可以透過檢閱每日使用量檔案中的單價和有效單位價格來判斷，並確認是否已套用折扣。</span><span class="sxs-lookup"><span data-stu-id="4b886-143">Review the daily usage file - This can be determined by reviewing the unit price and effective unit price within the daily usage file and confirming if a discount is being applied.</span></span> <span data-ttu-id="4b886-144">如果您收到折扣，您是系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4b886-144">If you are receiving the discount you are the admin.</span></span>

- <span data-ttu-id="4b886-145">建立 Azure 監視器警示 - 您可以建立 Azure 監視器活動記錄[警示](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)，以便在您的 RBAC 存取權從 CSP 訂用帳戶中移除時收到通知。</span><span class="sxs-lookup"><span data-stu-id="4b886-145">Create an Azure monitor alert - You can create an Azure Monitor activity log [alert](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) to be notified of  when your RBAC access is removed from CSP subscription.</span></span>

### <a name="create-an-azure-monitor-alert"></a><span data-ttu-id="4b886-146">建立 Azure 監視器警示</span><span class="sxs-lookup"><span data-stu-id="4b886-146">Create an Azure monitor alert</span></span>

1. <span data-ttu-id="4b886-147">建立警示。</span><span class="sxs-lookup"><span data-stu-id="4b886-147">Create alert.</span></span>

:::image type="content" source="images/azure/azurealert1.png" alt-text="Azure 警示":::

2. <span data-ttu-id="4b886-149">選取您想要讓警示採取的動作類型。例如，如果您指定要使用電子郵件，您會收到一封電子郵件，通知您是否發生任何角色指派刪除。</span><span class="sxs-lookup"><span data-stu-id="4b886-149">Select the type of action you want the alert to take.For example, if you specify that you want an email, you will receive an email notifying you if any role assignment deletion occurs.</span></span>

:::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="設定警示":::

### <a name="aobo-removal"></a><span data-ttu-id="4b886-151">AOBO 移除</span><span class="sxs-lookup"><span data-stu-id="4b886-151">AOBO removal</span></span>

<span data-ttu-id="4b886-152">客戶可以前往 Azure 入口網站上的 **Access 控制**，來管理其訂用帳戶的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-152">Customers can manage access to their subscriptions by going to **Access Control** on the Azure portal.</span></span> <span data-ttu-id="4b886-153">從 [角色指派] 索引標籤中，選取 [移除存取權]。</span><span class="sxs-lookup"><span data-stu-id="4b886-153">From the **Role assignments** tab, they select **Remove access**.</span></span> <span data-ttu-id="4b886-154">如果發生這種情況，您可以：</span><span class="sxs-lookup"><span data-stu-id="4b886-154">If this happens, you can:</span></span>

- <span data-ttu-id="4b886-155">與您的客戶交談，查看是否可以恢復系統管理員存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-155">Talk with your customer to see if admin access can be reinstated.</span></span>
- <span data-ttu-id="4b886-156">使用透過[角色型存取控制 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview) 提供的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-156">Use the access provided through [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview).</span></span>
- <span data-ttu-id="4b886-157">使用透過 [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/) 提供的存取權。</span><span class="sxs-lookup"><span data-stu-id="4b886-157">Use access provided through [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).</span></span>

<span data-ttu-id="4b886-158">角色型存取權與系統管理員存取權不同。</span><span class="sxs-lookup"><span data-stu-id="4b886-158">Role-based access differs from admin access.</span></span> <span data-ttu-id="4b886-159">角色會精確地分隔您可以和不可以執行的動作。</span><span class="sxs-lookup"><span data-stu-id="4b886-159">Roles delimit precisely what you can and can't do.</span></span> <span data-ttu-id="4b886-160">系統管理員存取權較廣泛。</span><span class="sxs-lookup"><span data-stu-id="4b886-160">Admin access is broader.</span></span>

<span data-ttu-id="4b886-161">若要查看有資格獲得 PEC 的角色，請參閱[合作夥伴所獲得信用點數的角色和權限](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)。</span><span class="sxs-lookup"><span data-stu-id="4b886-161">To see the roles eligible to earn PEC, read [Roles and permissions for the partner earned credit](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).</span></span>




<span data-ttu-id="4b886-162">**詳細資訊**</span><span class="sxs-lookup"><span data-stu-id="4b886-162">**For more information**</span></span>

- [<span data-ttu-id="4b886-163">撤銷及恢復 Azure CSP 訂用帳戶的系統管理員權限</span><span class="sxs-lookup"><span data-stu-id="4b886-163">Revoking and reinstating admin privileges for Azure CSP subscriptions</span></span>](revoke-reinstate-csp.md)

- [<span data-ttu-id="4b886-164">合作夥伴所獲得信用點數 - 概觀</span><span class="sxs-lookup"><span data-stu-id="4b886-164">Partner earned credit - overview</span></span>](partner-earned-credit.md)

- [<span data-ttu-id="4b886-165">受控服務的合作夥伴所獲得信用點數</span><span class="sxs-lookup"><span data-stu-id="4b886-165">Partner earned credit for managed services</span></span>](partner-earned-credit-explanation.md)