---
title: 受控服務的合作夥伴所獲得信用點數
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 深入了解受控服務的 Microsoft 合作夥伴所獲得信用點數 (PEC) 如何計算及支付，以及如何確保您符合資格。
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f274103feeadfa6fd135f99632f3013c29601972
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182404"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>合作夥伴所獲得信用點數如何計算及付費

**適當的角色**

- 全域系統管理員
- 使用者系統管理員
- 系統管理代理人
- 帳單系統管理員
- 銷售代理人

針對受控服務 (PEC) 取得的合作夥伴所獲得信用點數，可辨識和獎勵合作夥伴，其擁有全天候 IT 營運控制及管理其客戶的部分或全部 Azure 環境。 根據預設，在 CSP 中，合作夥伴會被授與客戶訂用帳戶的必要存取權，讓他們能夠執行全天候的作業管理，並控制訂用帳戶上的資源。 下一節將說明客戶可以為交易合作夥伴佈建存取權的其他方式。 每月發票金額為合作夥伴所獲得信用點數的淨額。 合作夥伴可以在他們的每月對帳檔案上查看 PEC 詳細資料。 如需客戶可以為交易合作夥伴佈建存取權的其他方式，請參閱[管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)。

另請參閱[恢復 Azure CSP 訂用帳戶的系統管理員權限](revoke-reinstate-csp.md)

## <a name="eligibility"></a>資格

若要接收合夥點數 (PEC)，必須滿足下列需求： 

- 您應具備作用中的 MPN 合約和有效的角色型存取控制 (RBAC) 角色，才能接收所管理之 Azure 資產的所獲得信用點數。

- 您必須具有在 CSP 中客戶 Azure 資源的全天候營運控制和管理。 這表示您必須在客戶的 Azure 訂用帳戶、Azure 資源群組、Azure 資源上擁有系統管理員權限。 在間接提供者及其間接經銷商的案例中，如果間接提供者或間接經銷商或雙方都有此營運控制和管理，間接提供者就有資格使用 PEC。 若要深入了解，請參閱[恢復 Azure CSP 訂用帳戶的系統管理員權限](./revoke-reinstate-csp.md)。

- 除了以上要求，PEC 僅適用於 Azure 方案耗用量價格中所列的服務，您可以從 [Azure 方案價格](https://partner.microsoft.com/commerce/sales)頁面匯出這些資訊。

- PEC **不** 適用於下列服務：
    - Azure 方案保留
    - 在 Azure 方案耗用量價格的標記資料行中，識別為「第三方」的第三方產品
    - Marketplace 價目表中的產品
    - [Azure Spot 虛擬機器](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC 會向下獲得至 Azure 資源層級。 如果您在訂用帳戶或資源群組層級上具有有效存取權，每個具有較高實體的資源可以獲得 PEC。

- 您也可以在 [Azure 成本管理](/azure/cost-management-billing/costs/get-started-partners)頁面上取得 PEC 的詳細資料。

### <a name="calculation"></a>計算

PEC 會每日計算，並可在每日使用量檔案和每月發票對帳檔案中檢視。 合作夥伴 (間接提供者或間接經銷商) 必須具有整天 (全天候) 的存取權，以確保他們獲得 PEC。 系統會在受控 Azure 資產上每日計算 PEC。 指定計費週期 (月) 的最大 PEC 為 15%。 在整個月 (存取跨度) 和所有合格資源 (存取範圍) 內保留永續性特殊權限存取的合作夥伴，將獲得 15% 的完整 PEC。 範圍和跨度縮減會導致該月的 PEC 率降低。 每日評等使用量檔案會每日顯示是否在 Azure 資產上套用 PEC。 合作夥伴還可以註冊警示，以監視永續性特殊權限存取是否發生變更。

## <a name="azure-cost-management"></a>Azure 成本管理

使用成本分析的 Azure 成本管理 (ACM) 可讓您成為合作夥伴，查看已獲得 PEC 優勢的成本。  

1. 在 [Azure 入口網站](https://portal.azure.com)中，登入您的合作夥伴租用戶，然後選取 [成本管理 + 帳單]。

2. 選取 [Azure 成本管理]

3. 選取 [成本分析]

   [成本分析] 視圖會顯示您計費帳戶的成本，適用於以您支付 Microsoft 的價格所購買及使用的所有服務。

4. 在樞紐分析表的下拉式清單中選取 **PartnerEarnedCreditApplied**，以查看已套用 PEC 的成本。 當 **PartnerEarnedCreditApplied** 屬性為 True 時，相關聯的成本就會享有合作夥伴所取得信用額度的權益。 

   當 PartnerEarnedCreditApplied 屬性為 False 時，相關聯的成本尚不符合所需的信用額度資格，或所購買的服務不符合合作夥伴所取得的信用額度。

   >[!NOTE] 
   >一般而言，服務的使用量需要8-24 小時才會出現在 [成本管理] 中，而 PEC 信用額度會在 Azure 成本管理的存取時間起 48 小時內出現。

5. 您也可以使用 [分組依據及新增] 篩選功能，依據 PartnerEarnedCreditApplied 屬性分組及篩選，以深入瞭解具有 PEC 的成本，以及未套用任何 PEC 的成本。

## <a name="next-steps"></a>接下來的步驟

- [合作夥伴所獲得信用點數 - 概觀](partner-earned-credit.md)

- 合作夥伴所獲得信用點數計算的詳細範例在價目表上，您可以透過合作夥伴中心儀表板取得 (需要登入)。

- [移至 Azure 方案 - 開始使用](azure-plan-get-started.md)

- [管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)

- [撤銷或恢復 Azure CSP 訂用帳戶的系統管理員權限](revoke-reinstate-csp.md)