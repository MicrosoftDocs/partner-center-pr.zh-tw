---
title: 獎勵客戶關聯問題
description: 瞭解如何解決在 (CPOR) 客戶關聯時，與索取的記錄夥伴合作時所產生的問題。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 08/31/2020
ms.openlocfilehash: 8b1ab61422dd6583a66c6968ac202403e64cdd4e
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220616"
---
# <a name="incentives-customer-association-issues"></a>獎勵客戶關聯問題

**適用於：**

- 合作夥伴中心

**適當的角色：**

- 帳單系統管理員
- 全域系統管理員
- 獎勵管理員

下列內容將協助您解決當您使用客戶關聯時可能出現的問題。

## <a name="domain-tenant-mismatch"></a>網域租使用者不符

在 [記錄的宣告夥伴] (CPOR) 關聯宣告流程] 中，系統會要求您提供客戶租使用者識別碼和子域。 如果您收到錯誤訊息，指出它們不符，請洽詢您的客戶以確定您有正確的詳細資料。

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR 關聯宣告流程中的訂用帳戶錯誤

在 CPOR 關聯宣告流程中，系統可能會要求您為您嘗試透過 Business Applications (Dynamics 365) 提出的產品提供訂用帳戶。 我們會要求您提供訂用帳戶，因為我們會動態檢查產品和訂用帳戶是否屬於所宣告的租使用者。 我們也會檢查訂用帳戶是否為主動/寬限期狀態。

如果您收到錯誤，可能有幾個原因：

- 選取的產品不存在於客戶的租用戶上
- 提供的訂用帳戶並非 Dynamics 的訂用帳戶
- 提供的訂閱適用於 CSP
- 客戶尚未針對該訂用帳戶啟用/布建產品
- 該訂閱已經宣告過
- 提供的識別碼不是訂用帳戶識別碼

如果您有關于訂用帳戶精確度的問題，請與您的客戶合作，以確保訂用帳戶正確無誤，而且您使用的是正確的租使用者識別碼。

如果此路由尚未解決您的問題，請聯絡 [支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。

## <a name="when-subscriptions-will-be-available-to-claim"></a>當訂用帳戶可供領取時

宣告訂用帳戶時，如果尚未布建訂用帳戶，您將會收到錯誤。 客戶需要採取幾個步驟，才能讓 CPOR 平臺取得訂用帳戶，並讓它可供領取。 如果您在嘗試索取訂用帳戶時收到錯誤，請洽詢您的客戶，確定該訂用帳戶已布建，且您宣稱的訂用帳戶正確無誤。 如果您已取得此路由，請聯絡 [支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。

## <a name="which-activity-do-i-choose"></a>我選擇哪個活動？

CPOR 宣告平臺允許與 Business Applications 和 Microsoft 365 解決方案區域相關的 CPOR 關聯宣告。 適用于每個解決方案區域的活動如下所示。 根據描述選取正確的活動，以避免未來必須回收。 宣告不正確的活動可能會導致缺少資格和獎勵收益。


| 解決方案領域 | 活動 | 適用于 |
| ------ | ----------- | ----------- |
| 商務應用程式      | 問答   | 如果您對購買合格產品有影響，且想要申請售前獎勵，請選取此項。 只有當客戶透過大量授權合約或 Web 直接購買這些產品時，才適用此選項。 |
|    |  使用方式  | 如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。 只有當客戶透過大量授權合約或 Web 直接購買這些產品時，才適用此選項。 |
|    | 收益關聯   | 如果您對其合格產品的選擇是否受到影響，請加以選取。 此選項僅適用于收入關聯，不適用於獎勵款項。 只有當客戶透過大量授權合約或 Web 直接購買這些產品時，才適用此選項。   |
| Microsoft 365   | 使用方式   | 如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。 |

## <a name="which-mpn-do-i-choose"></a>我選擇哪個 MPN？

在 CPOR 關聯宣告流程中，系統會要求您選擇應該與您在終端客戶宣稱的工作相關聯的公司 MPN。 您的公司可能有許多 MPNs，其中有些可能是在獎勵計畫中註冊，而其他則與夥伴類型相關聯，例如 FRP FastTrack。 CPOR 關聯宣告流程將會識別哪些 MPNs 已在激勵計畫中註冊，但不會告訴您它是否為特定的合作夥伴類型 MPN。 請務必選取正確的 MPN，以避免未來需要回收。 宣告不正確的 MPN 可能會導致缺少資格和獎勵收益。

如果您不知道要使用哪一個 MPN，請洽詢您的全域管理員。

如果您想要使用的 MPN 尚未註冊，您可以在 [獎勵總覽](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) 索引標籤中管理該選項， (登入所需的) 。

## <a name="choosing-a-product-vs-entering-a-subscription"></a>選擇產品與輸入訂用帳戶

當您索取並核准 Dynamics 產品時，合作夥伴可以在 CPOR 關聯宣告本身中查看訂用帳戶識別碼。 當索取此訂用帳戶時，該訂用帳戶會處於作用中狀態或處於寬限期狀態，但可能會有一段時間，且必須在個別的 CPOR 關聯宣告中宣告新的訂用帳戶。

## <a name="competing-claims"></a>競爭宣告

如果您要為客戶建立 CPOR 關聯宣告，而其產品 (s) 已與另一個夥伴相關聯，則您的宣告將會通過仲裁：

1. 在您建立新的客戶關聯後，Microsoft 將會驗證所提供關聯和執行證明的詳細資料，以確保其正確性。

2. 如果您和另一個合作夥伴宣告相同的客戶和產品/工作負載，Microsoft 將會檢查每個夥伴的執行檔證明，以決定要核准的合作夥伴。

3. 可能會從這兩個夥伴要求其他資訊，這可能會導致處理關聯要求的延遲。

4. 您的 CPOR 關聯宣告仍會在五個工作天內進行審核，但其狀態可能會在較長一段時間內保持 _審核_ 狀態。 當 Microsoft 與目前擁有產品/工作負載的夥伴合作時，就會發生這種情況。 如果是這種情況，您將會在宣告的 [批註] 區段中收到通知。 

>[!IMPORTANT]
>如果我們需要其他資訊來驗證您的 CPOR association 證明 (PoE) ，我們會透過 [CPOR 關聯宣告批註] 區段與您聯繫。

## <a name="next-steps"></a>後續步驟

- [開始使用獎勵](incentives-get-started-intro.md)
