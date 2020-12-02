---
title: 為客戶帳戶新增多位使用者
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要將多個使用者新增至客戶的帳戶，請使用逗點分隔值 ( .csv) 檔案格式，將資料檔案上傳至合作夥伴中心。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474184"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="cf76c-103">將使用者的 .csv 檔案上傳至客戶的帳戶</span><span class="sxs-lookup"><span data-stu-id="cf76c-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="cf76c-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="cf76c-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cf76c-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="cf76c-105">Global admin</span></span>

<span data-ttu-id="cf76c-106">將多個使用者同時新增至客戶的帳戶，方法是將以逗點分隔值檔案格式 ( .csv) 的資料檔案上傳至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="cf76c-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="cf76c-107">建立客戶使用者的檔案，並上傳至客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="cf76c-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="cf76c-108">建立包含上述資料並以逗號分隔值 (.csv) 的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="cf76c-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="cf76c-109">儲存檔案以便您在之後的步驟中瀏覽該檔案。</span><span class="sxs-lookup"><span data-stu-id="cf76c-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="cf76c-110">請參閱 [.csv 檔案的欄位，以匯入多個使用者的客戶帳戶](file-customer-users.md)。</span><span class="sxs-lookup"><span data-stu-id="cf76c-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="cf76c-111">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="cf76c-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="cf76c-112">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="cf76c-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="cf76c-113">選取客戶的 [ **使用者和授權** ] 索引標籤，然後選取 **[上傳使用者**]。</span><span class="sxs-lookup"><span data-stu-id="cf76c-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="cf76c-114">在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]**。</span><span class="sxs-lookup"><span data-stu-id="cf76c-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="cf76c-115">在檔案選取器中，選取您的資料檔案，然後選取 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="cf76c-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="cf76c-116">選取 [驗證]。</span><span class="sxs-lookup"><span data-stu-id="cf76c-116">Select **Validate**.</span></span>

    <span data-ttu-id="cf76c-117">**注意** 大部分帳戶建立錯誤的原因出自資料檔案問題，包括資訊遺失、格式不正確或電子郵件地址重複，或是檔案中有太多筆記錄。</span><span class="sxs-lookup"><span data-stu-id="cf76c-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="cf76c-118">在合作夥伴中心驗證檔案之後，請選取新使用者的地理 **位置** 。</span><span class="sxs-lookup"><span data-stu-id="cf76c-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="cf76c-119">選取 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="cf76c-119">Select **Save**.</span></span>
10. <span data-ttu-id="cf76c-120">下載使用者的暫存密碼資訊。</span><span class="sxs-lookup"><span data-stu-id="cf76c-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="cf76c-121">請務必立即下載具有暫時密碼的檔案，因為您稍後將無法再進行。</span><span class="sxs-lookup"><span data-stu-id="cf76c-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="cf76c-122">新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。</span><span class="sxs-lookup"><span data-stu-id="cf76c-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="cf76c-123">新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。</span><span class="sxs-lookup"><span data-stu-id="cf76c-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="cf76c-124">後續步驟</span><span class="sxs-lookup"><span data-stu-id="cf76c-124">Next steps</span></span>

- [<span data-ttu-id="cf76c-125">提供客戶合作夥伴中心的許可權，以購買自己的產品或服務</span><span class="sxs-lookup"><span data-stu-id="cf76c-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
