---
title: 客戶關聯問題
description: 瞭解如何解決使用已宣告的記錄夥伴（CPOR）客戶關聯時所出現的問題。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: e5ad52e128aba9884fafea3900a3c03d31d4868f
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719324"
---
# <a name="customer-association-issues"></a>客戶關聯問題

適用於：

- 合作夥伴中心

下列內容將協助您解決當您使用客戶關聯時可能會出現的問題。

適當的角色：

- 帳單系統管理員
- 全域系統管理員
- 獎勵管理員

## <a name="domain-tenant-mismatch"></a>網域-租使用者不符

在領取的記錄（CPOR）關聯宣告流程合作夥伴中，系統會要求您提供客戶租使用者識別碼和子域。 如果您收到錯誤訊息，指出它們不相符，請洽詢您的客戶，以確保您有正確的詳細資料。

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>CPOR 關聯宣告流程中的訂用帳戶錯誤

在 CPOR 關聯宣告流程中，系統可能會要求您透過 Business Applications （Dynamics 365）為您嘗試宣告的產品提供訂用帳戶。 我們會要求您提供訂用帳戶，因為我們會動態檢查產品和訂用帳戶是否屬於所宣告的租使用者。 我們也正在檢查訂用帳戶是否為使用中/處於「寬限期」狀態。

如果您收到錯誤，可能有幾個原因：

- 選取的產品不存在於客戶的租用戶上
- 提供的訂用帳戶不適用於 Dynamics
- 提供的訂閱適用於 CSP
- 客戶尚未啟用/布建該訂用帳戶的產品
- 該訂閱已經宣告過
- 提供的識別碼不是訂用帳戶 ID

如果您有關于訂用帳戶精確度的問題，請與您的客戶合作，以確保訂用帳戶正確，且您使用的是正確的租使用者識別碼。

如果此路由尚未解決您的問題，請聯絡[支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。

## <a name="when-subscriptions-will-be-available-to-claim"></a>當訂閱將可供宣告

在宣告訂用帳戶時，如果尚未布建訂用帳戶，您將會收到錯誤。 客戶必須採取幾個步驟，訂用帳戶才可供 CPOR 平臺進行挑選，並使其可供索取。 如果您在嘗試宣告訂用帳戶時收到錯誤，請洽詢您的客戶，確保其已布建，且您所索取的訂用帳戶正確無誤。 如果您已經取得此路由，請聯絡[支援](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)人員。

## <a name="which-activity-do-i-choose"></a>我要選擇哪一個活動？

CPOR 聲稱平臺允許與 Business Applications 和 Microsoft 365 解決方案區域相關的 CPOR 關聯宣告。 適用于每個解決方案區域的活動如下。 根據描述來選取正確的活動，以避免未來需要回收。 宣告不正確的活動可能會導致缺少資格和獎勵收益。


| 解決方案領域 | 活動 | 適用于 |
| ------ | ----------- | ----------- |
| 商務應用程式      | 售前   | 如果您影響其購買合格產品，而且想要申請售前獎勵，請選取此項。 只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。 |
|    |  使用方式  | 如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。 只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。 |
|    | 收益關聯   | 如果您將其合格產品的選取範圍影響為商業影響因素，請選取此選項。 此選項僅適用于收益關聯，而不是獎勵付款。 只有當客戶透過大量授權合約或 Web Direct 購買這些產品時，才適用此選項。   |
| Microsoft 365   | 使用方式   | 如果您要推動其採用和使用合格的工作負載，而且想要申請使用獎勵，請選取此項。 |

## <a name="which-mpn-do-i-choose"></a>我要選擇哪一種 MPN？

在 CPOR 關聯宣告流程中，系統會要求您選擇應該與您在終端客戶所宣稱之工作相關聯的公司 MPN。 您的公司可能有許多 MPNs，其中一些可能已在獎勵計畫中註冊，而其他人則與合作夥伴類型（例如 FRP FastTrack）相關聯。 CPOR 關聯宣告流程會識別在獎勵計畫中註冊哪個 MPNs，但不會告訴您它是否為特定的夥伴類型 MPN。 請務必選取正確的 MPN，以避免未來需要回收。 宣告不正確的 MPN 可能會導致缺少資格和獎勵收益。

如果您不知道要使用哪個 MPN，請洽詢您的全域管理員。

如果您想要使用的 MPN 尚未註冊，您可以在 [[獎勵總覽]](https://partner.microsoft.com/dashboard/incentives/enrollment/summary)索引標籤中進行管理。

## <a name="choosing-a-product-vs-entering-a-subscription"></a>選擇產品與輸入訂用帳戶的比較

當 Dynamics 產品已領取並核准時，合作夥伴可以在 CPOR association 宣告本身中查看訂用帳戶識別碼。 當此訂用帳戶被宣告時，它會處於作用中或處於寬限狀態，但可能會有一段時間結束訂用帳戶，而且必須在個別的 CPOR 關聯宣告中領取新的訂閱。

## <a name="competing-claims"></a>競爭宣告

如果您要為客戶建立 CPOR 關聯宣告，而其產品已與另一個合作夥伴相關聯，您的宣告將會通過仲裁：

1. 在您建立新的客戶關聯後，Microsoft 將會驗證所提供關聯和執行證明的詳細資料，以確保其正確性。

2. 如果您和其他合作夥伴宣告相同的客戶和產品/工作負載，Microsoft 將會回顧每個合作夥伴的執行證明檔，以決定要核准哪一個夥伴。

3. 可能會從兩個夥伴要求其他資訊，這可能會導致處理您的關聯要求延遲。

4. 您的 CPOR 關聯宣告仍然會在五個工作天內進行檢查，但其狀態可能_會在較_長的時間內保持不變。 當 Microsoft 與目前擁有產品/工作負載的合作夥伴合作時，就可能發生這種情況。 如果是這種情況，您將會在宣告的 [批註] 區段中收到通知。 

>[!IMPORTANT]
>如果我們需要其他資訊來驗證您的 CPOR association PoE，我們會透過 CPOR 關聯宣告批註一節來聯絡您。
