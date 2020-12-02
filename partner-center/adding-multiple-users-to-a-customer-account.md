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
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>將使用者的 .csv 檔案上傳至客戶的帳戶


**適當的角色**

- 全域系統管理員

將多個使用者同時新增至客戶的帳戶，方法是將以逗點分隔值檔案格式 ( .csv) 的資料檔案上傳至合作夥伴中心。 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>建立客戶使用者的檔案，並上傳至客戶帳戶

1. 建立包含上述資料並以逗號分隔值 (.csv) 的資料檔案。 儲存檔案以便您在之後的步驟中瀏覽該檔案。 請參閱 [.csv 檔案的欄位，以匯入多個使用者的客戶帳戶](file-customer-users.md)。 

2. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

3. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

4. 選取客戶的 [ **使用者和授權** ] 索引標籤，然後選取 **[上傳使用者**]。

5. 在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]**。

6. 在檔案選取器中，選取您的資料檔案，然後選取 [ **開啟**]。

7. 選取 [驗證]。

    **注意** 大部分帳戶建立錯誤的原因出自資料檔案問題，包括資訊遺失、格式不正確或電子郵件地址重複，或是檔案中有太多筆記錄。

8. 在合作夥伴中心驗證檔案之後，請選取新使用者的地理 **位置** 。
9. 選取 [儲存]。
10. 下載使用者的暫存密碼資訊。

    >[!IMPORTANT]
    > 請務必立即下載具有暫時密碼的檔案，因為您稍後將無法再進行。 新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。

11. 新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。 

## <a name="next-steps"></a>後續步驟

- [提供客戶合作夥伴中心的許可權，以購買自己的產品或服務](give-customers-permission.md)
