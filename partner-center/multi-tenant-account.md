---
title: 將其他租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 透過您的合作夥伴中心帳戶管理多個租使用者
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389507"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="869aa-103">在合作夥伴中心帳戶中新增和管理多個租使用者</span><span class="sxs-lookup"><span data-stu-id="869aa-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="869aa-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="869aa-104">**Applies to**</span></span>

- <span data-ttu-id="869aa-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="869aa-105">Partner Center</span></span>

<span data-ttu-id="869aa-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="869aa-106">**Appropriate roles**</span></span>

- <span data-ttu-id="869aa-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="869aa-107">Global admin</span></span>

<span data-ttu-id="869aa-108">您可能需要在合作夥伴中心帳戶中管理多個 Azure AD 租使用者的原因有很多。</span><span class="sxs-lookup"><span data-stu-id="869aa-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="869aa-109">例如，您的公司可能購買另一家公司，而您希望新公司的員工能夠使用合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="869aa-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="869aa-110">不過，您想要讓兩個公司保持獨立。</span><span class="sxs-lookup"><span data-stu-id="869aa-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="869aa-111">在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶（PNG）產生關聯。</span><span class="sxs-lookup"><span data-stu-id="869aa-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="869aa-112">此關聯可讓兩家公司的使用者在合作夥伴中心內工作。</span><span class="sxs-lookup"><span data-stu-id="869aa-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="869aa-113">將另一個 Azure AD 租使用者新增至您的帳戶</span><span class="sxs-lookup"><span data-stu-id="869aa-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="869aa-114">身為全域管理員，請登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="869aa-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="869aa-115">從 [**設定**]**圖示選取 [\*\*\*\*帳戶設定**]，然後選取 [租使用者]。</span><span class="sxs-lookup"><span data-stu-id="869aa-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="建立租使用者的關聯"::: 

3. <span data-ttu-id="869aa-117">選取 [**關聯另一個 AD 租**使用者]，並指定您想要建立關聯的租使用者。</span><span class="sxs-lookup"><span data-stu-id="869aa-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="869aa-118">身為全域管理員，請登入您想要建立關聯的租使用者，並確認該關聯。</span><span class="sxs-lookup"><span data-stu-id="869aa-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="確認關聯租使用者"::: 

5. <span data-ttu-id="869aa-120">確認之後，您會看到**所有設定**通知。</span><span class="sxs-lookup"><span data-stu-id="869aa-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="869aa-121">選取 [**回到租使用者管理**]，您就會看到已列出新加入的租使用者。</span><span class="sxs-lookup"><span data-stu-id="869aa-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="869aa-122">後續步驟</span><span class="sxs-lookup"><span data-stu-id="869aa-122">Next steps</span></span>

- [<span data-ttu-id="869aa-123">新增使用者</span><span class="sxs-lookup"><span data-stu-id="869aa-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
