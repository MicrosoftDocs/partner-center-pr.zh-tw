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
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>藉由建立 .csv 檔案，將多個使用者新增至客戶帳戶

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員

以逗點分隔值檔案格式（.csv）將資料檔案上傳至合作夥伴中心，一次將多個使用者新增至客戶的帳戶。 您可以從合作夥伴中心下載範例資料檔案，然後進行編輯以供您使用，或者您可以使用以下定義的資料模型來建立新的資料檔案。

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>資料檔案需求

若要使用大量上傳程式，將多個使用者新增至客戶的帳戶，您必須符合下列需求：

- 您必須擁有對客戶帳戶的全域系統管理員權限；
- 每位使用者都必須有唯一的電子郵件地址，並已附加到客戶的電子郵件網域；
- 您一次最多可以上傳 100 筆記錄。 如果您需要新增超過 100 位使用者，請建立並上傳其他資料檔案。
- 所有使用者都必須位於相同的地理**位置**。
- 請只輸入下面描述的資料。 沒有直接關聯的資料將會導致上傳失敗。

請在資料檔案中輸入以下資料：

| **資料行名稱** | **說明**  | **限制**  |
|:-------- |:------  |:----- |
| 名字  | 使用者的名字（選擇性欄位）  | 50 個字元的限制  |
| 姓氏  | 使用者的姓氏 (選擇性欄位)  | 50 個字元的限制  |
| 顯示名稱    | 顯示在合作夥伴中心的名稱（必要欄位）                            | 50 個字元的限制                         |
| 電子郵件   | 使用者在 customer 公司的公司電子郵件地址（必要欄位）           | 每個使用者都必須有唯一的電子郵件地址 |
| 狀態更新   | 用來指示是否已經成功建立新的使用者記錄 | \*\*保留空白\*\*                        |

## <a name="next-steps"></a>後續步驟

- [如何為客戶新增多個使用者](adding-multiple-users-to-a-customer-account.md)