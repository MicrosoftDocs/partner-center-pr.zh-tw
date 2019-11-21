---
title: 為客戶帳戶建立多位使用者 | 合作夥伴中心
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 以逗點分隔值檔案格式（.csv）將資料檔案上傳至合作夥伴中心，以瞭解如何一次將多個使用者新增至客戶的帳戶。
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: 大量上傳, 新增多個使用者至客戶的帳戶, 新增客戶使用者, 大量上傳客戶使用者, 客戶帳戶, 客戶使用者, 使用者
ms.localizationpriority: medium
ms.openlocfilehash: 5c9de7ed78a0494790b447d1755d5eef70a89cca
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253183"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="b67f2-104">將多個使用者新增到客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="b67f2-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="b67f2-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="b67f2-105">**Applies to**</span></span>

-  <span data-ttu-id="b67f2-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="b67f2-106">Partner Center</span></span>

<span data-ttu-id="b67f2-107">您可以將多個使用者一次新增至客戶的帳戶，方法是將以逗點分隔值檔案格式（.csv）中的資料檔案上傳至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="b67f2-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b67f2-108">您可以從合作夥伴中心下載範例資料檔案，然後進行編輯以供您使用，或者您可以使用以下定義的資料模型來建立新的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="b67f2-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b67f2-109">資料檔案需求</span><span class="sxs-lookup"><span data-stu-id="b67f2-109">Data file requirements</span></span>


<span data-ttu-id="b67f2-110">若要使用大量上傳程式，將多個使用者新增至客戶的帳戶，您必須符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="b67f2-110">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

-   <span data-ttu-id="b67f2-111">您必須擁有對客戶帳戶的全域系統管理員權限；</span><span class="sxs-lookup"><span data-stu-id="b67f2-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="b67f2-112">每位使用者都必須有唯一的電子郵件地址，並已附加到客戶的電子郵件網域；</span><span class="sxs-lookup"><span data-stu-id="b67f2-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="b67f2-113">您一次最多可以上傳 100 筆記錄。</span><span class="sxs-lookup"><span data-stu-id="b67f2-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b67f2-114">如果您需要新增超過 100 位使用者，請建立並上傳其他資料檔案。</span><span class="sxs-lookup"><span data-stu-id="b67f2-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="b67f2-115">所有使用者都必須位於相同地理 **\[位置\]** 。</span><span class="sxs-lookup"><span data-stu-id="b67f2-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="b67f2-116">請只輸入下面描述的資料。</span><span class="sxs-lookup"><span data-stu-id="b67f2-116">Enter only the data described below.</span></span> <span data-ttu-id="b67f2-117">沒有直接關聯的資料將會導致上傳失敗。</span><span class="sxs-lookup"><span data-stu-id="b67f2-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b67f2-118">請在資料檔案中輸入以下資料：</span><span class="sxs-lookup"><span data-stu-id="b67f2-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="b67f2-119">**資料行名稱**</span><span class="sxs-lookup"><span data-stu-id="b67f2-119">**Column name**</span></span> | <span data-ttu-id="b67f2-120">**描述**</span><span class="sxs-lookup"><span data-stu-id="b67f2-120">**Description**</span></span>                                                              | <span data-ttu-id="b67f2-121">**局限**</span><span class="sxs-lookup"><span data-stu-id="b67f2-121">**Limitation**</span></span>                             |
| <span data-ttu-id="b67f2-122">名字</span><span class="sxs-lookup"><span data-stu-id="b67f2-122">First name</span></span>      | <span data-ttu-id="b67f2-123">使用者的名字（選擇性欄位）</span><span class="sxs-lookup"><span data-stu-id="b67f2-123">User's first name (optional field)</span></span>                                           | <span data-ttu-id="b67f2-124">50 個字元限制</span><span class="sxs-lookup"><span data-stu-id="b67f2-124">50-character limit</span></span>                         |
| <span data-ttu-id="b67f2-125">姓氏</span><span class="sxs-lookup"><span data-stu-id="b67f2-125">Last name</span></span>       | <span data-ttu-id="b67f2-126">使用者的姓氏 (選擇性欄位)</span><span class="sxs-lookup"><span data-stu-id="b67f2-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="b67f2-127">50 個字元限制</span><span class="sxs-lookup"><span data-stu-id="b67f2-127">50-character limit</span></span>                         |
| <span data-ttu-id="b67f2-128">顯示名稱</span><span class="sxs-lookup"><span data-stu-id="b67f2-128">Display name</span></span>    | <span data-ttu-id="b67f2-129">顯示在合作夥伴中心的名稱（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="b67f2-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b67f2-130">50 個字元限制</span><span class="sxs-lookup"><span data-stu-id="b67f2-130">50-character limit</span></span>                         |
| <span data-ttu-id="b67f2-131">電子郵件</span><span class="sxs-lookup"><span data-stu-id="b67f2-131">Email</span></span>           | <span data-ttu-id="b67f2-132">使用者在 customer 公司的公司電子郵件地址（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="b67f2-132">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="b67f2-133">每位使用者都必須有唯一電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="b67f2-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b67f2-134">狀態更新</span><span class="sxs-lookup"><span data-stu-id="b67f2-134">Status update</span></span>   | <span data-ttu-id="b67f2-135">用來指示是否已經成功建立新的使用者記錄</span><span class="sxs-lookup"><span data-stu-id="b67f2-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="b67f2-136">\*\*留空的\*\*</span><span class="sxs-lookup"><span data-stu-id="b67f2-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="b67f2-137">建立多個使用者帳戶</span><span class="sxs-lookup"><span data-stu-id="b67f2-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="b67f2-138">建立包含上述資料的逗號分隔值 (.csv) 資料檔案。</span><span class="sxs-lookup"><span data-stu-id="b67f2-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="b67f2-139">儲存檔案以便您在之後的步驟中瀏覽該檔案。</span><span class="sxs-lookup"><span data-stu-id="b67f2-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="b67f2-140">從 [**合作夥伴中心**] 功能表中，選取 [**客戶**]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="b67f2-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="b67f2-141">選取 \[上傳使用者\]。</span><span class="sxs-lookup"><span data-stu-id="b67f2-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="b67f2-142">在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]** 。</span><span class="sxs-lookup"><span data-stu-id="b67f2-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="b67f2-143">在檔案選取器中，選取您的資料檔案，然後選取 **\[開啟\]** 。</span><span class="sxs-lookup"><span data-stu-id="b67f2-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="b67f2-144">選取 **\[驗證\]** 。</span><span class="sxs-lookup"><span data-stu-id="b67f2-144">Select **Validate**.</span></span>

    <span data-ttu-id="b67f2-145">**注意**  大部分的帳戶建立錯誤是由資料檔案問題所造成，包括遺漏資訊、格式不正確或重複的電子郵件地址，或檔案中的記錄太多。</span><span class="sxs-lookup"><span data-stu-id="b67f2-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="b67f2-146">合作夥伴中心驗證檔案之後，請選取新使用者的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="b67f2-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="b67f2-147">選取 \[儲存\]。</span><span class="sxs-lookup"><span data-stu-id="b67f2-147">Select **Save**.</span></span>
9.  <span data-ttu-id="b67f2-148">下載使用者的暫時密碼資訊。</span><span class="sxs-lookup"><span data-stu-id="b67f2-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="b67f2-149">**重要：** 請務必立即下載包含暫時密碼的檔案，因為您無法在之後執行此作業。</span><span class="sxs-lookup"><span data-stu-id="b67f2-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="b67f2-150">新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。</span><span class="sxs-lookup"><span data-stu-id="b67f2-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="b67f2-151">新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。</span><span class="sxs-lookup"><span data-stu-id="b67f2-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



