---
title: 為客戶帳戶新增多個使用者
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要將多個使用者新增至客戶的帳戶，請使用逗號分隔值（.csv）檔案格式，將資料檔案上傳至合作夥伴中心。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0a9b2ed89b10e43c31d00777054839f3208e5c16
ms.sourcegitcommit: 32516c30e90ee78415e5537d2b8ccf467f56a82d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "87535738"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="83aa3-103">將使用者的 .csv 檔案上傳至客戶的帳戶</span><span class="sxs-lookup"><span data-stu-id="83aa3-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="83aa3-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="83aa3-104">**Applies to**</span></span>

- <span data-ttu-id="83aa3-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="83aa3-105">Partner Center</span></span>

<span data-ttu-id="83aa3-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="83aa3-106">**Appropriate roles**</span></span>

- <span data-ttu-id="83aa3-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="83aa3-107">Global admin</span></span>

<span data-ttu-id="83aa3-108">以逗點分隔值檔案格式（.csv）將資料檔案上傳至合作夥伴中心，一次將多個使用者新增至客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="83aa3-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="83aa3-109">建立客戶使用者的檔案，並上傳至客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="83aa3-109">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="83aa3-110">建立包含上述資料並以逗號分隔值 (.csv) 的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="83aa3-110">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="83aa3-111">儲存檔案以便您在之後的步驟中瀏覽該檔案。</span><span class="sxs-lookup"><span data-stu-id="83aa3-111">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="83aa3-112">請參閱 .csv 檔案的[欄位，以匯入客戶帳戶的多個使用者](file-customer-users.md)。</span><span class="sxs-lookup"><span data-stu-id="83aa3-112">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="83aa3-113">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="83aa3-113">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="83aa3-114">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="83aa3-114">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="83aa3-115">選取客戶的 [**使用者和授權**] 索引標籤，然後選取 [**上傳使用者**]。</span><span class="sxs-lookup"><span data-stu-id="83aa3-115">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="83aa3-116">在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]**。</span><span class="sxs-lookup"><span data-stu-id="83aa3-116">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="83aa3-117">在檔案選取器中，選取您的資料檔案，然後選取 [**開啟**]。</span><span class="sxs-lookup"><span data-stu-id="83aa3-117">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="83aa3-118">選取 [驗證]。</span><span class="sxs-lookup"><span data-stu-id="83aa3-118">Select **Validate**.</span></span>

    <span data-ttu-id="83aa3-119">**注意**   大部分的帳戶建立錯誤是由資料檔案問題所造成，包括遺漏資訊、格式不正確或重複的電子郵件地址，或檔案中有太多記錄。</span><span class="sxs-lookup"><span data-stu-id="83aa3-119">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="83aa3-120">合作夥伴中心驗證檔案之後，請選取新使用者的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="83aa3-120">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="83aa3-121">選取 [儲存]  。</span><span class="sxs-lookup"><span data-stu-id="83aa3-121">Select **Save**.</span></span>
10. <span data-ttu-id="83aa3-122">下載使用者的暫存密碼資訊。</span><span class="sxs-lookup"><span data-stu-id="83aa3-122">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="83aa3-123">請務必立即下載含有暫時密碼的檔案，因為您稍後將無法執行此動作。</span><span class="sxs-lookup"><span data-stu-id="83aa3-123">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="83aa3-124">新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。</span><span class="sxs-lookup"><span data-stu-id="83aa3-124">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="83aa3-125">新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。</span><span class="sxs-lookup"><span data-stu-id="83aa3-125">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="83aa3-126">後續步驟</span><span class="sxs-lookup"><span data-stu-id="83aa3-126">Next steps</span></span>

- [<span data-ttu-id="83aa3-127">授與客戶合作夥伴中心的許可權，以購買自己的產品或服務</span><span class="sxs-lookup"><span data-stu-id="83aa3-127">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
