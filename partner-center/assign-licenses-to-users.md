---
title: 管理客戶帳戶中的使用者
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何為客戶建立使用者帳戶、新增或移除使用者授權、重設使用者密碼、刪除使用者帳戶，或將其還原。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527674"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="b25c2-103">合作夥伴中心內客戶帳戶的使用者管理工作</span><span class="sxs-lookup"><span data-stu-id="b25c2-103">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="b25c2-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="b25c2-104">**Applies to**</span></span>

- <span data-ttu-id="b25c2-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="b25c2-105">Partner Center</span></span>

<span data-ttu-id="b25c2-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="b25c2-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b25c2-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="b25c2-107">Global admin</span></span>
- <span data-ttu-id="b25c2-108">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="b25c2-108">User management admin</span></span>
- <span data-ttu-id="b25c2-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="b25c2-109">Admin agent</span></span>
- <span data-ttu-id="b25c2-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="b25c2-110">Sales agent</span></span>
- <span data-ttu-id="b25c2-111">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="b25c2-111">Helpdesk agent</span></span>

<span data-ttu-id="b25c2-112">您可以在客戶的帳戶中建立及刪除新的使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="b25c2-113">您也可以還原在刪除後的30天內，您先前刪除的一個或多個使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="b25c2-114">使用者先前的訂閱指派同樣會還原 (假設他們之前的配置可用)</span><span class="sxs-lookup"><span data-stu-id="b25c2-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="b25c2-115">當您為客戶購買新的訂用帳戶時，客戶應該會提供一份清單，列出所有需要帳戶的使用者、其使用者權限，以及每個使用者所需的服務。</span><span class="sxs-lookup"><span data-stu-id="b25c2-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="b25c2-116">您可以使用 [與 Excel 相容的 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)來匯入名稱，一次[指派訂閱給多個使用者](bulk-license-provisioning-for-multiple-users.md)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="b25c2-117">為客戶建立使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="b25c2-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="b25c2-118">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b25c2-119">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-119">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b25c2-120">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b25c2-120">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="b25c2-121">針對您新增的每個使用者，選取 **\[新增訂閱\]**，然後填入相關資訊 (包括權限和授權)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-121">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="b25c2-122">[儲存] 變更。</span><span class="sxs-lookup"><span data-stu-id="b25c2-122">**Save** your changes.</span></span>

5. <span data-ttu-id="b25c2-123">請務必記錄使用者名稱和暫時密碼，以傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="b25c2-124">如果您要以是一次加入一個的方式新增多個使用者，請使用 **\[新增其他使用者\]**。</span><span class="sxs-lookup"><span data-stu-id="b25c2-124">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="b25c2-125">您也可以透過[匯入 Excel 相容 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)，一次新增多個使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="b25c2-126">您可以等到新增一整組使用者之後，再從確認畫面以電子郵件傳送或直接列印這些名稱和密碼。</span><span class="sxs-lookup"><span data-stu-id="b25c2-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="b25c2-127">新增或移除客戶的使用者授權</span><span class="sxs-lookup"><span data-stu-id="b25c2-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="b25c2-128">下列步驟適用于新增或移除 Microsoft 產品的使用者授權。</span><span class="sxs-lookup"><span data-stu-id="b25c2-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="b25c2-129">若要在商業 marketplace 中新增或移除以授權為基礎的 SaaS 訂用帳戶的使用者授權，請參閱[新增或移除 SaaS 訂閱的授權](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="b25c2-130">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b25c2-131">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-131">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="b25c2-132">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b25c2-132">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="b25c2-133">從清單中選擇一或多位使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-133">Choose one or more users from the list.</span></span> <span data-ttu-id="b25c2-134">例如，如果客戶剛購買新的授權，而您想要將它們指派給尚未擁有的人員，您可以使用 [**篩選使用者依據**] 選項來尋找正確的群組。</span><span class="sxs-lookup"><span data-stu-id="b25c2-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="b25c2-135">選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-135">Select **Manage licenses**.</span></span> <span data-ttu-id="b25c2-136">進行變更，然後 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-136">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="b25c2-137">針對[Azure Marketplace 產品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)，授權指派和啟用是透過發行產品的獨立軟體廠商（ISV）來管理。</span><span class="sxs-lookup"><span data-stu-id="b25c2-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="b25c2-138">為客戶重設使用者的密碼</span><span class="sxs-lookup"><span data-stu-id="b25c2-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="b25c2-139">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="b25c2-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="b25c2-140">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-140">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="b25c2-141">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b25c2-141">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="b25c2-142">從清單中選擇使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="b25c2-143">在畫面底部，選取 [**重設密碼**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-143">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="b25c2-144">將新的暫時密碼傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="b25c2-145">為客戶刪除使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="b25c2-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="b25c2-146">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-146">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b25c2-147">從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="b25c2-148">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b25c2-148">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="b25c2-149">從清單中選擇使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="b25c2-150">在畫面底部，選取 [刪除使用者帳戶]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="b25c2-150">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="b25c2-151">如果您需要還原此帳戶，您可以在 \[客戶\] 之 **\[使用者和授權\]** 清單的 **\[刪除的使用者\]** 索引標籤中找到該帳戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="b25c2-152">您有 30 天的期限可以還原刪除的使用者。</span><span class="sxs-lookup"><span data-stu-id="b25c2-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="b25c2-153">還原刪除的使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="b25c2-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="b25c2-154">從 [**合作夥伴中心**] 功能表選取 [**客戶**]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b25c2-154">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="b25c2-155">選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-155">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="b25c2-156">選取 **\[刪除的使用者 ( )\]** 索引標籤，其中應該會顯示 **(1)**，如果有多個可還原的已刪除使用者，則顯示更大的數字。</span><span class="sxs-lookup"><span data-stu-id="b25c2-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="b25c2-157">選取一或多個 [已刪除的使用者] 核取方塊，然後選取 [**還原**]。</span><span class="sxs-lookup"><span data-stu-id="b25c2-157">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="b25c2-158">所有選取的使用者帳戶都會重新出現在 [**使用者和授權**] 頁面中。</span><span class="sxs-lookup"><span data-stu-id="b25c2-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="b25c2-159">相關主題</span><span class="sxs-lookup"><span data-stu-id="b25c2-159">Related topics</span></span>


[<span data-ttu-id="b25c2-160">指派或撤銷多個使用者的授權</span><span class="sxs-lookup"><span data-stu-id="b25c2-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="b25c2-161">為客戶帳戶建立多位使用者</span><span class="sxs-lookup"><span data-stu-id="b25c2-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)