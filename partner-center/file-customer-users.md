---
title: 用於為客戶帳戶匯入多個使用者之 .csv 檔案的欄位
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 若要將多個使用者新增至客戶帳戶，請建立包含適當欄位的逗點分隔值（.csv）檔案。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528176"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="e5ddc-103">藉由建立 .csv 檔案，將多個使用者新增至客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="e5ddc-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="e5ddc-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="e5ddc-104">**Applies to**</span></span>

- <span data-ttu-id="e5ddc-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e5ddc-105">Partner Center</span></span>

<span data-ttu-id="e5ddc-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="e5ddc-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e5ddc-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="e5ddc-107">Global admin</span></span>

<span data-ttu-id="e5ddc-108">以逗點分隔值檔案格式（.csv）將資料檔案上傳至合作夥伴中心，一次將多個使用者新增至客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="e5ddc-109">您可以從合作夥伴中心下載範例資料檔案，然後進行編輯以供您使用，或者您可以使用以下定義的資料模型來建立新的資料檔案。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="e5ddc-110">資料檔案需求</span><span class="sxs-lookup"><span data-stu-id="e5ddc-110">Data file requirements</span></span>

<span data-ttu-id="e5ddc-111">若要使用大量上傳程式，將多個使用者新增至客戶的帳戶，您必須符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="e5ddc-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="e5ddc-112">您必須擁有對客戶帳戶的全域系統管理員權限；</span><span class="sxs-lookup"><span data-stu-id="e5ddc-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="e5ddc-113">每位使用者都必須有唯一的電子郵件地址，並已附加到客戶的電子郵件網域；</span><span class="sxs-lookup"><span data-stu-id="e5ddc-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="e5ddc-114">您一次最多可以上傳 100 筆記錄。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="e5ddc-115">如果您需要新增超過 100 位使用者，請建立並上傳其他資料檔案。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="e5ddc-116">所有使用者都必須位於相同的地理**位置**。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="e5ddc-117">請只輸入下面描述的資料。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-117">Enter only the data described below.</span></span> <span data-ttu-id="e5ddc-118">沒有直接關聯的資料將會導致上傳失敗。</span><span class="sxs-lookup"><span data-stu-id="e5ddc-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="e5ddc-119">請在資料檔案中輸入以下資料：</span><span class="sxs-lookup"><span data-stu-id="e5ddc-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="e5ddc-120">**資料行名稱**</span><span class="sxs-lookup"><span data-stu-id="e5ddc-120">**Column name**</span></span> | <span data-ttu-id="e5ddc-121">**說明**</span><span class="sxs-lookup"><span data-stu-id="e5ddc-121">**Description**</span></span>  | <span data-ttu-id="e5ddc-122">**限制**</span><span class="sxs-lookup"><span data-stu-id="e5ddc-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="e5ddc-123">名字</span><span class="sxs-lookup"><span data-stu-id="e5ddc-123">First name</span></span>  | <span data-ttu-id="e5ddc-124">使用者的名字（選擇性欄位）</span><span class="sxs-lookup"><span data-stu-id="e5ddc-124">User's first name (optional field)</span></span>  | <span data-ttu-id="e5ddc-125">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="e5ddc-125">50-character limit</span></span>  |
| <span data-ttu-id="e5ddc-126">姓氏</span><span class="sxs-lookup"><span data-stu-id="e5ddc-126">Last name</span></span>  | <span data-ttu-id="e5ddc-127">使用者的姓氏 (選擇性欄位)</span><span class="sxs-lookup"><span data-stu-id="e5ddc-127">User's last name (optional field)</span></span>  | <span data-ttu-id="e5ddc-128">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="e5ddc-128">50-character limit</span></span>  |
| <span data-ttu-id="e5ddc-129">顯示名稱</span><span class="sxs-lookup"><span data-stu-id="e5ddc-129">Display name</span></span>    | <span data-ttu-id="e5ddc-130">顯示在合作夥伴中心的名稱（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="e5ddc-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="e5ddc-131">50 個字元的限制</span><span class="sxs-lookup"><span data-stu-id="e5ddc-131">50-character limit</span></span>                         |
| <span data-ttu-id="e5ddc-132">電子郵件</span><span class="sxs-lookup"><span data-stu-id="e5ddc-132">Email</span></span>   | <span data-ttu-id="e5ddc-133">使用者在 customer 公司的公司電子郵件地址（必要欄位）</span><span class="sxs-lookup"><span data-stu-id="e5ddc-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="e5ddc-134">每個使用者都必須有唯一的電子郵件地址</span><span class="sxs-lookup"><span data-stu-id="e5ddc-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="e5ddc-135">狀態更新</span><span class="sxs-lookup"><span data-stu-id="e5ddc-135">Status update</span></span>   | <span data-ttu-id="e5ddc-136">用來指示是否已經成功建立新的使用者記錄</span><span class="sxs-lookup"><span data-stu-id="e5ddc-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="e5ddc-137">\*\*保留空白\*\*</span><span class="sxs-lookup"><span data-stu-id="e5ddc-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="e5ddc-138">後續步驟</span><span class="sxs-lookup"><span data-stu-id="e5ddc-138">Next steps</span></span>

- [<span data-ttu-id="e5ddc-139">如何為客戶新增多個使用者</span><span class="sxs-lookup"><span data-stu-id="e5ddc-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)