---
title: 將租使用者新增至您的合作夥伴中心帳戶
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心帳戶中新增、合併或管理多個 Azure AD 租使用者，並瞭解您可能會想要這麼做的原因。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124800"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="c3cf2-103">在您的合作夥伴中心帳戶中新增和管理多個租使用者</span><span class="sxs-lookup"><span data-stu-id="c3cf2-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="c3cf2-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="c3cf2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c3cf2-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="c3cf2-105">Global admin</span></span>
- <span data-ttu-id="c3cf2-106">帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="c3cf2-106">Account admin</span></span>

<span data-ttu-id="c3cf2-107">本文討論如何為您的公司將多個 Azure Active Directory (Azure AD) 租使用者，然後在您的合作夥伴中心帳戶中新增及管理這些租使用者。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="c3cf2-108">有許多原因需要這麼做。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-108">There are many reasons to do so.</span></span> <span data-ttu-id="c3cf2-109">例如：</span><span class="sxs-lookup"><span data-stu-id="c3cf2-109">For example:</span></span>

- <span data-ttu-id="c3cf2-110">假設您的公司 Contoso 已獲得另一家 Fabrikam。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="c3cf2-111">您希望兩個公司保持獨立，但您希望新的員工能夠使用合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="c3cf2-112">在此情況下，您會將新公司的 Azure AD 租使用者與您的合作夥伴通用帳戶 (PGA) 相關聯。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="c3cf2-113">此關聯可讓兩個公司的使用者在合作夥伴中心內工作。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="c3cf2-114">如果您使用多個租使用者執行業務 (例如， *contoso.com*、 *contoso.uk* 和 *contoso.in*) ，您可以使用多租使用者將這些租使用者群組在相同的電腦帳戶中。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="c3cf2-115">如果合併和收購指導方針要求您使用兩個公司的租使用者，您可以同時使用 *constoso.com* 和 *fabrikam.com* 租使用者。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="c3cf2-116">任何租使用者的使用者都必須能夠：</span><span class="sxs-lookup"><span data-stu-id="c3cf2-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="c3cf2-117">存取合作夥伴中心以取得訓練、數位下載或 Microsoft 認證專業人員 (MCP) 關聯。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="c3cf2-118">指派合作夥伴中心角色，例如 Microsoft Partner Network (MPN) 系統管理員或獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="c3cf2-119">將 Azure AD 租使用者新增至您的帳戶</span><span class="sxs-lookup"><span data-stu-id="c3cf2-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="c3cf2-120">以全域管理員身分登入 [Microsoft 合作夥伴中心](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="c3cf2-121">選取右上方的 [**設定**]，選取 [**帳戶設定**]，然後選取 [租使用者 **]。**</span><span class="sxs-lookup"><span data-stu-id="c3cf2-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="[Azure AD 設定檔] 窗格上 [關聯] 按鈕的螢幕擷取畫面。"::: 

1. <span data-ttu-id="c3cf2-123">選取 [ **關聯**]，然後指定您要關聯的租使用者。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="c3cf2-124">在提示字元中，以全域管理員身分登入您想要關聯的租使用者，然後選取 [ **確認**]。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[確認新的 Azure AD 關聯] 窗格上 [確認] 按鈕的螢幕擷取畫面。"::: 

   <span data-ttu-id="c3cf2-126">確認關聯之後，就會顯示 **所有設定** 的訊息。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="c3cf2-127">若要查看新增的租使用者，請選取 [ **返回租使用者管理**]。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="c3cf2-128">如果租使用者已與另一個合作夥伴中心帳戶相關聯，您就無法將該租使用者與帳戶產生關聯。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="c3cf2-129">從您的帳戶移除租使用者</span><span class="sxs-lookup"><span data-stu-id="c3cf2-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="c3cf2-130">以全域管理員身分登入 [Microsoft 合作夥伴中心](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="c3cf2-131">選取右上方的 [ **設定** ] 圖示，然後選取 [ **帳戶設定**]。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="c3cf2-132">在左窗格中 **，選取 [** 租使用者]。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="c3cf2-133">在 [ **管理 AZURE AD** 租使用者] 底下，選取 [ **夥伴** ] 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="c3cf2-134">選取您要移除其關聯的租使用者旁的 [ **移除** ]。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="目前租使用者關聯及其 [移除] 連結的螢幕擷取畫面。":::

   <span data-ttu-id="c3cf2-136">如先前的螢幕擷取畫面所示，除了主要租使用者和您目前登入的租使用者之外，所有相關聯的租使用者都會啟用 [ **移除** ] 連結。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="c3cf2-137">當您移除租使用者時，該租使用者上的使用者將無法再存取合作夥伴中心帳戶，因此移除可能會影響您的專長認證。</span><span class="sxs-lookup"><span data-stu-id="c3cf2-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c3cf2-138">接下來的步驟</span><span class="sxs-lookup"><span data-stu-id="c3cf2-138">Next steps</span></span>

- [<span data-ttu-id="c3cf2-139">建立使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="c3cf2-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






