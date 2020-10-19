---
title: 將其他租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在您的合作夥伴中心帳戶中新增、合併或管理多個 Azure AD 租使用者。 深入瞭解您可能會想要進行的一些原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175167"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="7e7bf-104">在您的合作夥伴中心帳戶中新增和管理多個租使用者</span><span class="sxs-lookup"><span data-stu-id="7e7bf-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="7e7bf-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="7e7bf-105">**Applies to**</span></span>

- <span data-ttu-id="7e7bf-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="7e7bf-106">Partner Center</span></span>

<span data-ttu-id="7e7bf-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="7e7bf-107">**Appropriate roles**</span></span>

- <span data-ttu-id="7e7bf-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="7e7bf-108">Global admin</span></span>

<span data-ttu-id="7e7bf-109">這項功能可讓您管理貴公司的多個租用戶，並將其合併到您的合作夥伴中心帳戶。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="7e7bf-110">您可能需要在合作夥伴中心帳戶中管理多個 Azure AD 租使用者的原因有很多。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="7e7bf-111">例如：</span><span class="sxs-lookup"><span data-stu-id="7e7bf-111">For example:</span></span>

- <span data-ttu-id="7e7bf-112">您的公司可能會購買另一家公司，而您希望新公司中的員工能夠使用合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="7e7bf-113">不過，您希望兩個公司保持獨立。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="7e7bf-114">在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶 (PGA) 產生關聯。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="7e7bf-115">此關聯可讓兩個公司的使用者在合作夥伴中心中工作。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="7e7bf-116">如果您有一個以上的租使用者來執行您的商務 (例如 contoso.com、contoso.uk、contoso.in) 您可以使用多租使用者將它們系結到相同的電腦帳戶。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="7e7bf-117">合併和收購需要您使用多個租使用者 (例如，如果 Contoso 取得 Fabrikam，您就必須能夠同時使用 Constoso.com 和 Fabrikam.com 各自的租使用者) 。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="7e7bf-118">來自任何租使用者的使用者都必須能夠：</span><span class="sxs-lookup"><span data-stu-id="7e7bf-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="7e7bf-119">存取合作夥伴中心用於訓練、數位下載、MCP 關聯</span><span class="sxs-lookup"><span data-stu-id="7e7bf-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="7e7bf-120">指派合作夥伴中心角色，例如 MPN Admin、獎勵系統管理員等等。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="7e7bf-121">將另一個 Azure AD 租使用者新增至您的帳戶</span><span class="sxs-lookup"><span data-stu-id="7e7bf-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="7e7bf-122">以全域管理員身分登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="7e7bf-123">從 [**設定**]**圖示選取 [\*\*\*\*帳戶設定**]，然後選取 [租使用者]。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="建立租使用者的關聯"::: 

3. <span data-ttu-id="7e7bf-125">選取 [ **建立其他 AD 租** 使用者的關聯]，並指出您要關聯的租使用者。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="7e7bf-126">以全域管理員身分登入您想要關聯的租使用者，並確認該關聯。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="建立租使用者的關聯"::: 

5. <span data-ttu-id="7e7bf-128">確認之後，您會看到所有的 **設定** 通知。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="7e7bf-129">選取 [ **返回租使用者管理** ]，您會看到列出新加入的租使用者。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="7e7bf-130">如果租使用者已經與另一個合作夥伴中心帳戶建立關聯，您就無法將它與帳戶產生關聯。</span><span class="sxs-lookup"><span data-stu-id="7e7bf-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="7e7bf-131">後續步驟</span><span class="sxs-lookup"><span data-stu-id="7e7bf-131">Next steps</span></span>

- [<span data-ttu-id="7e7bf-132">新增使用者</span><span class="sxs-lookup"><span data-stu-id="7e7bf-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
