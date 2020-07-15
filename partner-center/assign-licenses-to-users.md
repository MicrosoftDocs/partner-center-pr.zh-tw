---
title: 管理客戶帳戶中的使用者
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何為客戶建立使用者帳戶、新增或移除使用者授權、重設使用者密碼、刪除使用者帳戶，或將其還原。
author: BillLinzbach
ms.author: BillLi
Keywords: 客戶管理、帳戶、建立帳戶、授權、指派授權、使用者管理、密碼、重設密碼、變更密碼
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 57d5a91fda593b47d6e22b3682d0072b256ae655
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377682"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="25a18-104">合作夥伴中心內客戶帳戶的使用者管理工作</span><span class="sxs-lookup"><span data-stu-id="25a18-104">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="25a18-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="25a18-105">**Applies to**</span></span>

- <span data-ttu-id="25a18-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="25a18-106">Partner Center</span></span>

<span data-ttu-id="25a18-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="25a18-107">**Appropriate roles**</span></span>

- <span data-ttu-id="25a18-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="25a18-108">Global admin</span></span>
- <span data-ttu-id="25a18-109">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="25a18-109">User management admin</span></span>
- <span data-ttu-id="25a18-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="25a18-110">Admin agent</span></span>
- <span data-ttu-id="25a18-111">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="25a18-111">Sales agent</span></span>
- <span data-ttu-id="25a18-112">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="25a18-112">Helpdesk agent</span></span>

<span data-ttu-id="25a18-113">您可以在客戶的帳戶中建立及刪除新的使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-113">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="25a18-114">您也可以還原在刪除後的30天內，您先前刪除的一個或多個使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-114">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="25a18-115">使用者先前的訂閱指派同樣會還原 (假設他們之前的配置可用)</span><span class="sxs-lookup"><span data-stu-id="25a18-115">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="25a18-116">當您為客戶購買新的訂用帳戶時，客戶應該會提供一份清單，列出所有需要帳戶的使用者、其使用者權限，以及每個使用者所需的服務。</span><span class="sxs-lookup"><span data-stu-id="25a18-116">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="25a18-117">您可以使用 [與 Excel 相容的 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)來匯入名稱，一次[指派訂閱給多個使用者](bulk-license-provisioning-for-multiple-users.md)。</span><span class="sxs-lookup"><span data-stu-id="25a18-117">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="25a18-118">為客戶建立使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="25a18-118">Create user accounts for a customer</span></span>

1. <span data-ttu-id="25a18-119">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="25a18-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="25a18-120">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-120">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="25a18-121">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="25a18-121">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="25a18-122">針對您新增的每個使用者，選取 **\[新增訂閱\]**，然後填入相關資訊 (包括權限和授權)。</span><span class="sxs-lookup"><span data-stu-id="25a18-122">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="25a18-123">[儲存] 變更。</span><span class="sxs-lookup"><span data-stu-id="25a18-123">**Save** your changes.</span></span>

5. <span data-ttu-id="25a18-124">請務必記錄使用者名稱和暫時密碼，以傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-124">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="25a18-125">如果您要以是一次加入一個的方式新增多個使用者，請使用 **\[新增其他使用者\]**。</span><span class="sxs-lookup"><span data-stu-id="25a18-125">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="25a18-126">您也可以透過[匯入 Excel 相容 .csv 試算表檔案](adding-multiple-users-to-a-customer-account.md)，一次新增多個使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-126">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="25a18-127">您可以等到新增一整組使用者之後，再從確認畫面以電子郵件傳送或直接列印這些名稱和密碼。</span><span class="sxs-lookup"><span data-stu-id="25a18-127">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="25a18-128">新增或移除客戶的使用者授權</span><span class="sxs-lookup"><span data-stu-id="25a18-128">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="25a18-129">下列步驟適用于新增或移除 Microsoft 產品的使用者授權。</span><span class="sxs-lookup"><span data-stu-id="25a18-129">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="25a18-130">若要在商業 marketplace 中新增或移除以授權為基礎的 SaaS 訂用帳戶的使用者授權，請參閱[新增或移除 SaaS 訂閱的授權](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。</span><span class="sxs-lookup"><span data-stu-id="25a18-130">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="25a18-131">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="25a18-131">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="25a18-132">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-132">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="25a18-133">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="25a18-133">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="25a18-134">從清單中選擇一或多位使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-134">Choose one or more users from the list.</span></span> <span data-ttu-id="25a18-135">例如，如果客戶剛購買新的授權，而您想要將它們指派給尚未擁有的人員，您可以使用 [**篩選使用者依據**] 選項來尋找正確的群組。</span><span class="sxs-lookup"><span data-stu-id="25a18-135">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="25a18-136">選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-136">Select **Manage licenses**.</span></span> <span data-ttu-id="25a18-137">進行變更，然後 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-137">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="25a18-138">針對[Azure Marketplace 產品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)，授權指派和啟用是透過發行產品的獨立軟體廠商（ISV）來管理。</span><span class="sxs-lookup"><span data-stu-id="25a18-138">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="25a18-139">為客戶重設使用者的密碼</span><span class="sxs-lookup"><span data-stu-id="25a18-139">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="25a18-140">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="25a18-140">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="25a18-141">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-141">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="25a18-142">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="25a18-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="25a18-143">從清單中選擇使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-143">Choose the user from the list.</span></span>

4.  <span data-ttu-id="25a18-144">在畫面底部，選取 [**重設密碼**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-144">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="25a18-145">將新的暫時密碼傳送給使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-145">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="25a18-146">為客戶刪除使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="25a18-146">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="25a18-147">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-147">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="25a18-148">從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-148">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="25a18-149">在客戶功能表中，選取 [使用者與授權]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="25a18-149">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="25a18-150">從清單中選擇使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-150">Choose the user from the list.</span></span>

3.  <span data-ttu-id="25a18-151">在畫面底部，選取 [刪除使用者帳戶]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="25a18-151">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="25a18-152">如果您需要還原此帳戶，您可以在 \[客戶\] 之 **\[使用者和授權\]** 清單的 **\[刪除的使用者\]** 索引標籤中找到該帳戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-152">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="25a18-153">您有 30 天的期限可以還原刪除的使用者。</span><span class="sxs-lookup"><span data-stu-id="25a18-153">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="25a18-154">還原刪除的使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="25a18-154">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="25a18-155">從 [**合作夥伴中心**] 功能表選取 [**客戶**]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="25a18-155">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="25a18-156">選取 [**使用者和授權**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-156">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="25a18-157">選取 **\[刪除的使用者 ( )\]** 索引標籤，其中應該會顯示 **(1)**，如果有多個可還原的已刪除使用者，則顯示更大的數字。</span><span class="sxs-lookup"><span data-stu-id="25a18-157">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="25a18-158">選取一或多個 [已刪除的使用者] 核取方塊，然後選取 [**還原**]。</span><span class="sxs-lookup"><span data-stu-id="25a18-158">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="25a18-159">所有選取的使用者帳戶都會重新出現在 [**使用者和授權**] 頁面中。</span><span class="sxs-lookup"><span data-stu-id="25a18-159">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="25a18-160">相關主題</span><span class="sxs-lookup"><span data-stu-id="25a18-160">Related topics</span></span>


[<span data-ttu-id="25a18-161">指派或撤銷多個使用者的授權</span><span class="sxs-lookup"><span data-stu-id="25a18-161">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="25a18-162">為客戶帳戶建立多位使用者</span><span class="sxs-lookup"><span data-stu-id="25a18-162">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)