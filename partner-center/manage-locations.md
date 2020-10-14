---
title: 管理合作夥伴帳戶中的位置
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何新增位置，以及如何在獎勵計畫、雲端解決方案提供者業務、訂閱和其他交易中使用 MPN 識別碼。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c4435227cdd5d777d11c79bf4adc63471ad925e9
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006854"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>管理您的 MPN 帳戶位置並新增位置

**適用於**

- 合作夥伴中心

**適當的角色**

- 全域系統管理員
- 帳戶管理員

位置 MPN 識別碼可識別公司的每個特定位置。 您可以使用位置 MPN 識別碼來註冊獎勵計畫、交易雲端解決方案提供者 (CSP) 業務以及其他商業交易。 全域 MPN 識別碼可用於非交易式活動，例如支援要求。

## <a name="the-following-is-a-typical-scenario"></a>以下為典型的案例：

Contoso 在英國有其合作夥伴通用帳戶 (PGA)。 這是其已註冊的合法公司，而且有一個用於管理所有非交易業務的全域 MPN 識別碼。 Contoso 在英國、法國和美國的其他位置也有相當於分公司或部門的合作夥伴位置帳戶 (PLA)。 在 MPN 帳戶結構中，這些 PLA 會以唯一的位置 MPN 識別碼來表示。 PLA 可用於交易業務，例如 CSP 或獎勵計畫。 支出會繫結至特定位置。 

>[!NOTE]
>CSP 租用戶與 MPN 位置識別碼之間有 1 對 1 的關聯性。

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 位置的結構":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>為 CSP 業務新增位置的必要條件

若要新增 CSP 業務位置，有幾個必要條件：

1. 您必須在想要執行業務的國家/地區中擁有位置 MPN 識別碼。

1. 您在尚未註冊 CSP 的[業務區域](regional-authorization-overview.md)中需要新的 Azure AD 租用戶。 當您註冊 CSP 時，請建立此項目。
 
3. 使用新的 AAD 租用戶在區域中註冊 CSP 計畫。
提供合法公司的詳細資料，包括合法公司名稱、地址、主要連絡人詳細資料。 此帳戶會進行驗證，因此請務必新增有效的資訊。

>[!NOTE] 
 >請記得使用**新的** Azure AD 租用戶的**新**認證來登入。 請不要使用現有認證，因為合作夥伴中心會將您識別為已擁有帳戶。

4. 接受 Microsoft 合作夥伴合約並啟用帳戶。

## <a name="add-a-location"></a>新增位置

1. 在合作夥伴中心使用 MPN 帳戶登入。 MPN 帳戶應具備全域管理員或帳戶系統管理員權限。 

1. 從 [設定] 圖示選取 [合作夥伴設定]。

2. 選取 [位置]。

3. 選取 [新增位置]，然後插入要新增至公司位置的地址詳細資料，以及該位置的主要連絡人。

> [!NOTE]
> 在合作夥伴中心新增位置後，即無法將其移除。 如果您已使用正確的 MPN 識別碼來登入，您會在合作夥伴中心的左側功能表中看到 **MPN**。

## <a name="change-global-partner-account-location"></a>變更全球合作夥伴帳戶位置

1. 在 [[位置]](https://partner.microsoft.com/pcv/accountsettings/locationsprofile) 頁面上檢查位置清單，來確定已列出您要作為法律實體的位置。 如果沒有，請新增它。

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="MPN 位置的結構":::

2. 選取 [合作夥伴設定檔]，然後選取 [更新法定公司設定檔]。

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="MPN 位置的結構":::

3. 選取區域和法律實體，然後加以**提交**。

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="MPN 位置的結構":::

## <a name="next-steps"></a>後續步驟

- 了解[驗證程序](verification-responses.md)。
