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
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>將使用者的 .csv 檔案上傳至客戶的帳戶


**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員

以逗點分隔值檔案格式（.csv）將資料檔案上傳至合作夥伴中心，一次將多個使用者新增至客戶的帳戶。 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>建立客戶使用者的檔案，並上傳至客戶帳戶

1. 建立包含上述資料並以逗號分隔值 (.csv) 的資料檔案。 儲存檔案以便您在之後的步驟中瀏覽該檔案。 請參閱 .csv 檔案的[欄位，以匯入客戶帳戶的多個使用者](file-customer-users.md)。 

2. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

3. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

4. 選取客戶的 [**使用者和授權**] 索引標籤，然後選取 [**上傳使用者**]。

5. 在 **\[上傳使用者資訊\]** 底下，選取 **\[瀏覽\]**。

6. 在檔案選取器中，選取您的資料檔案，然後選取 [**開啟**]。

7. 選取 [驗證]。

    **注意**   大部分的帳戶建立錯誤是由資料檔案問題所造成，包括遺漏資訊、格式不正確或重複的電子郵件地址，或檔案中有太多記錄。

8. 合作夥伴中心驗證檔案之後，請選取新使用者的地理**位置**。
9. 選取 [儲存]  。
10. 下載使用者的暫存密碼資訊。

    >[!IMPORTANT]
    > 請務必立即下載含有暫時密碼的檔案，因為您稍後將無法執行此動作。 新的使用者必須他們新帳戶的暫時密碼登入他們的新帳戶。

11. 新的使用者會自動獲派 **\[可以使用授權與服務\]** 的權限。 

## <a name="next-steps"></a>後續步驟

- [授與客戶合作夥伴中心的許可權，以購買自己的產品或服務](give-customers-permission.md)
