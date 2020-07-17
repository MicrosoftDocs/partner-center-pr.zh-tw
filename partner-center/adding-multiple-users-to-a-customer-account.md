---
title: 為客戶帳戶新增多個使用者
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何一次將多個使用者新增至客戶的帳戶。 使用逗號分隔值（.csv）檔案格式，將資料檔案上傳至合作夥伴中心。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436307"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="8453f-104">將多個使用者新增至客戶帳戶-將資料檔案上傳至合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="8453f-104">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="8453f-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="8453f-105">**Applies to**</span></span>

- <span data-ttu-id="8453f-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="8453f-106">Partner Center</span></span>

<span data-ttu-id="8453f-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="8453f-107">**Appropriate roles**</span></span>

- <span data-ttu-id="8453f-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="8453f-108">Global admin</span></span>

<span data-ttu-id="8453f-109">您可以將多個使用者一次新增至客戶的帳戶，方法是將以逗點分隔值檔案格式（.csv）中的資料檔案上傳至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="8453f-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="8453f-110">您可以從合作夥伴中心下載範例資料檔案，然後進行編輯以供您使用，或者您可以使用以下定義的資料模型來建立新的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="8453f-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="8453f-111">資料檔案需求</span><span class="sxs-lookup"><span data-stu-id="8453f-111">Data file requirements</span></span>

<span data-ttu-id="8453f-112">若要使用大量上傳程式，將多個使用者新增至客戶的帳戶，您必須符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="8453f-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="8453f-113">您必須擁有對客戶帳戶的全域系統管理員權限；</span><span class="sxs-lookup"><span data-stu-id="8453f-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="8453f-114">每位使用者都必須有唯一的電子郵件地址，並已附加到客戶的電子郵件網域；</span><span class="sxs-lookup"><span data-stu-id="8453f-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="8453f-115">您一次最多可以上傳 100 筆記錄。</span><span class="sxs-lookup"><span data-stu-id="8453f-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="8453f-116">如果您需要新增超過 100 位使用者，請建立並上傳其他資料檔案。</span><span class="sxs-lookup"><span data-stu-id="8453f-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="8453f-117">所有使用者都必須位於相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="8453f-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="8453f-118">請只輸入下面描述的資料。</span><span class="sxs-lookup"><span data-stu-id="8453f-118">Enter only the data described below.</span></span> <span data-ttu-id="8453f-119">沒有直接關聯的資料將會導致上傳失敗。</span><span class="sxs-lookup"><span data-stu-id="8453f-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="8453f-120">請在資料檔案中輸入以下資料：</span><span class="sxs-lookup"><span data-stu-id="8453f-120">Enter the following data in the data file:</span></span>

| <span data-ttu-id="8453f-121">**資料行名稱**</span><span class="sxs-lookup"><span data-stu-id="8453f-121">**Column name**</span></span> | <span data-ttu-id="8453f-122">**說明**</span><span class="sxs-lookup"><span data-stu-id="8453f-122">**Description**</span></span>  | <span data-ttu-id="8453f-123">**限制**</span><span class="sxs-lookup"><span data-stu-id="8453f-123">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="8453f-124">名字</span><span class="sxs-lookup"><span data-stu-id="8453f-124">First name</span></span>  | <span data-ttu-id="8453f-125">使用者的名字（選擇性欄位）</span><span class="sxs-lookup"><span data-stu-id="8453f-125">User's first name (optional field)</span></span>  | <span data-ttu-id="8453f-126">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="8453f-126">50-character limit</span></span>  |
| <span data-ttu-id="8453f-127">姓氏</span><span class="sxs-lookup"><span data-stu-id="8453f-127">Last name</span></span>  | <span data-ttu-id="8453f-128">使用者的姓氏 (選擇性欄位)</span><span class="sxs-lookup"><span data-stu-id="8453f-128">User's last name (optional field)</span></span>  | <span data-ttu-id="8453f-129">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="8453f-129">50-character limit</span></span>  |
| <span data-ttu-id="8453f-130">顯示名稱</span><span class="sxs-lookup"><span data-stu-id="8453f-130">Display name</span></span>    | <span data-ttu-id="8453f-131">顯示在合作夥伴中心的名稱（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="8453f-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="8453f-132">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="8453f-132">50-character limit</span></span>                         |
| <span data-ttu-id="8453f-133">電子郵件</span><span class="sxs-lookup"><span data-stu-id="8453f-133">Email</span></span>   | <span data-ttu-id="8453f-134">使用者在 customer 公司的公司電子郵件地址（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="8453f-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="8453f-135">每個使用者都必須有唯一的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="8453f-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="8453f-136">狀態更新</span><span class="sxs-lookup"><span data-stu-id="8453f-136">Status update</span></span>   | <span data-ttu-id="8453f-137">用來指示是否已經成功建立新的使用者記錄</span><span class="sxs-lookup"><span data-stu-id="8453f-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="8453f-138">\*\*保留空白\*\*</span><span class="sxs-lookup"><span data-stu-id="8453f-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="8453f-139">建立多位使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="8453f-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="8453f-140">建立包含上述資料並以逗號分隔值 (.csv) 的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="8453f-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="8453f-141">儲存檔案以便您在之後的步驟中瀏覽該檔案。</span><span class="sxs-lookup"><span data-stu-id="8453f-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="8453f-142">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="8453f-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="8453f-143">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="8453f-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="8453f-144">選取客戶的 [**使用者和授權**] 索引標籤，然後選取 [**上傳使用者**]。</span><span class="sxs-lookup"><span data-stu-id="8453f-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="8453f-145">在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]**。</span><span class="sxs-lookup"><span data-stu-id="8453f-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="8453f-146">在檔案選取器中，選取您的資料檔案，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="8453f-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="8453f-147">選取 [驗證]。</span><span class="sxs-lookup"><span data-stu-id="8453f-147">Select **Validate**.</span></span>

    <span data-ttu-id="8453f-148">**注意**   大部分的帳戶建立錯誤是由資料檔案問題所造成，包括遺漏資訊、格式不正確或重複的電子郵件地址，或檔案中有太多記錄。</span><span class="sxs-lookup"><span data-stu-id="8453f-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="8453f-149">合作夥伴中心驗證檔案之後，請選取新使用者的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="8453f-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="8453f-150">選取 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="8453f-150">Select **Save**.</span></span>
10. <span data-ttu-id="8453f-151">下載使用者的暫存密碼資訊。</span><span class="sxs-lookup"><span data-stu-id="8453f-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="8453f-152">**重要：** 請務必立即下載包含暫時密碼的檔案，因為您無法在之後執行此作業。</span><span class="sxs-lookup"><span data-stu-id="8453f-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="8453f-153">新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。</span><span class="sxs-lookup"><span data-stu-id="8453f-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="8453f-154">新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。</span><span class="sxs-lookup"><span data-stu-id="8453f-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



