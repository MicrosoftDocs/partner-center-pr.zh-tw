---
title: 管理合作夥伴帳戶中的位置
ms.topic: how-to
ms.date: 02/05/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何新增位置，以及如何在獎勵計畫、雲端解決方案提供者業務、訂閱和其他交易中使用 MPN 識別碼。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c5ac31b772c6757468c5ea9d463643731571b31f
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624267"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>管理您的 MPN 帳戶位置並新增位置


**適當的角色**

- 全域系統管理員
- 帳戶管理員

位置 MPN 識別碼可識別公司的每個特定位置。 您可以使用位置 MPN 識別碼來註冊獎勵計畫、交易雲端解決方案提供者 (CSP) 業務以及其他商業交易。 全域 MPN 識別碼可用於非交易式活動，例如支援要求。

## <a name="the-following-is-a-typical-scenario"></a>以下為典型的案例：

Contoso 在英國有其合作夥伴通用帳戶 (PGA)。 這是其已註冊的合法公司，而且有一個用於管理所有非交易業務的全域 MPN 識別碼。 Contoso 在英國、法國和美國的其他位置也有相當於分公司或部門的合作夥伴位置帳戶 (PLA)。 在 MPN 帳戶結構中，這些 PLA 會以唯一的位置 MPN 識別碼來表示。 PLA 可用於交易業務，例如 CSP 或獎勵計畫。 支出會繫結至特定位置。 

>[!NOTE]
>CSP 租用戶與 MPN 位置識別碼之間有 1 對 1 的關聯性。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的結構":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>為 CSP 商務新增帳戶的必要條件

若要加入新的 CSP 商務帳戶，請先確定您已滿足必要條件。

1. 您的國家/地區必須要有一個位置 MPN 識別碼。 若要建立新的 MPN 位置，請閱讀下方的「新增 MPN 位置」。
  
1. 若要建立新的 CSP 間接轉銷商註冊，請參閱 [使用間接提供者的工作](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >請記得 **使用新的 CSP 帳戶****新** 的認證登入。 請不要使用現有認證，因為合作夥伴中心會將您識別為已擁有帳戶。

2. 接受 Microsoft 合作夥伴合約並啟用帳戶。

1. 如果您想要註冊為直接帳單合作夥伴，請閱讀 [直接帳單合作夥伴的需求](direct-partner-new-requirements.md)

## <a name="view-your-mpn-locations"></a>查看您的 MPN 位置

1. 使用您的 MPN 帳號憑證登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home) 。  (您的 MPN 認證可能與您的 CSP 認證不同)  
 
1. 從 [ **設定** ] 圖示，選取 [ **帳戶設定**]、[ **組織設定檔**]、[ **法律**]。 

1. 在 [ **夥伴** ] 索引標籤上，確認沒有橫幅錯誤訊息要求您修正從 PMC 遷移的位置。 如果有，請遵循指示並修正這些位置。 

3. 如果沒有錯誤訊息，請從 [  **設定**] 中選取 [  **帳戶設定**]、[ **組織設定檔**]、[ **識別碼**]。

4. 找出類型為 "Location" 的 MPN 識別碼，此識別碼符合此 CSP 帳戶的國家/地區，並使用它來搜尋下列專案並完成關聯。

5. 如果找不到符合您想要使用之 CSP 帳戶的位置 MPN 識別碼，您可以新增新的位置，以建立新的 MPN 識別碼。 請參閱下方 **的新增 MPN 位置** 。

## <a name="add-an-mpn-location"></a>新增 MPN 位置

1. 使用合作夥伴中心中的 MPN 帳戶登入。  (您的 MPN 認證可能與您) 的 CSP 認證不同。 MPN 帳戶應具備全域管理員或帳戶系統管理員權限。 

1. 從 [ **設定] 圖示** 選取 **帳戶設定** ，然後選取 [ **組織設定檔**]。

2. 選取 [ **法律聲明** ]，然後在 [ **夥伴** ] 索引標籤上，選取 [ **商務位置]，** 然後按一下 [ **新增位置]。**

3. 提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和連絡人。
 
1. 按一下 [ **新增位置**]。 這會為新的位置建立新的 MPN 識別碼，您可以將其用於 CSP 交易和獎勵。

:::image type="content" source="images/legal-biz.png" alt-text="新增法律聲明企業":::

> [!NOTE]
> 在合作夥伴中心新增位置後，即無法將其移除。 如果您已使用正確的 MPN 識別碼來登入，您會在合作夥伴中心的左側功能表中看到 **MPN**。

## <a name="change-country-of-partner-global-account"></a>變更合作夥伴通用帳戶的國家/地區 

1. 使用合作夥伴中心中的 MPN 帳戶登入。  (您的 MPN 認證可能與您) 的 CSP 認證不同。 MPN 帳戶應具備全域管理員或帳戶系統管理員權限。 

2. 在 [ **夥伴** ] 索引標籤上，移至 [ **商務位置** ] 並檢查位置清單，以確保列出您想要的位置，以列出您的法律實體。 
 
1. 若要新增位置，請按一下 [ **新增位置**]，然後在 [飛出] 中提供所需的詳細資料，包括您想要新增至公司之位置的公司名稱、位址和主要連絡人。 
 
1. 選取 [**國家/地區**] 下拉式清單旁的 [**變更您的國家**/地區]，然後依照步驟執行。 

:::image type="content" source="images/lbp.png" alt-text="法律聲明商務設定檔資料飛出":::

5. 按一下 [儲存]。

6. MPN global account country 將會變更為新的法律國家/地區。
  
## <a name="next-steps"></a>後續步驟

- 了解[驗證程序](verification-responses.md)。
