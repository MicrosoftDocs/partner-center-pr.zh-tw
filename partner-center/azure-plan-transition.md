---
title: 將客戶從目前的 Azure 供應項目移至 Azure 方案
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解 CSP 合作夥伴如何使用合作夥伴中心，將客戶從現有的 CSP Azure 供應項目移至 Azure 方案下的 Azure 服務。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 05/04/2020
ms.openlocfilehash: 073ee1a3f0cd90d3b10493a989d00dc1594505d6
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84452585"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>將客戶從現有 CSP Azure 供應項目轉換至 Azure 方案

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員
- 技術服務代理人
- 銷售代理人
- 使用者管理系統管理員

間接提供者和直接帳單合作夥伴可以轉換為適用於 Azure 的 Microsoft 雲端服務提供者計畫 (CSP) 中所提供的新商務體驗。 (間接經銷商必須透過其間接提供者來運作)。客戶可以透過簡化的方式購買雲端服務，無論是向合作夥伴、Microsoft 賣方或直接在網路上購買。

轉換功能僅適用於轉換至適用於 Azure 新商務經驗的客戶，以及已簽署 Microsoft 客戶合約的使用者，而不是針對 CSP 中的其他供應項目，例如 Office 365 或 Dynamics 365。

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>將現有的 CSP 供應項目轉換為 Azure 方案

您可以透過合作夥伴中心內 CSP 計畫中的新商務體驗，將客戶從他們的現有 CSP Azure 供應項目轉換到 Azure 方案下的 Azure 服務。 若要這麼做，合作夥伴和客戶必須透過合作夥伴中心建立轉售商關係，而且客戶必須已簽署 Microsoft 客戶合約。

### <a name="select-transition-to-azure-plan"></a>選取轉換至 Azure 方案

1. 為您的客戶選取 Azure 方案。

2. 選取 [將計費轉換為 Azure 方案]。

   :::image type="content" source="images/azure/transition1.png" alt-text="轉換":::

3. 選取 [繼續]

   :::image type="content" source="images/azure/transition2.png" alt-text="轉換":::

   您的客戶將會轉換為 Azure 方案。

   **轉換工作流程會自動執行必要的步驟**：

   - 購買 Azure 方案
   - 在直接 CSP 案例中，每位客戶一個方案  
   - 每個轉售商一個方案  

   例如，合作夥伴購買了兩個 Microsoft Azure 供應項目，並在購買中包含兩個不同的 POR。 在此情況下，轉換工作流程會購買兩個 Azure 方案 (每個轉銷商一個)，並自動對應 Azure 方案底下的個別 Azure 訂用帳戶。  

   **將 Azure 訂用帳戶對應至 Azure 方案**

   購買 Azure 方案之後，我們的系統會將現有的 Azure 訂用帳戶對應至 Azure 方案。 您可以在 Azure 入口網站和合作夥伴中心檢視進度。

4. 返回客戶的合作夥伴中心 [訂用帳戶] 頁面，使用他們的當地貨幣更新其預算限制。

   :::image type="content" source="images/azure/transition3.png" alt-text="轉換":::

   >[!NOTE]
   >您在合作夥伴中心設定的預算不會帶到 Azure 入口網站。 您也應該在 Azure 入口網站中設定預算和警示。

   當您移至 Azure 方案時，您無法再為此客戶購買 Azure 訂用帳戶。 您會在 Azure 入口網站中建立 Azure 方案底下的訂用帳戶。

   >[!NOTE]
   > 所有 Azure 方案底下透過 RBAC 購買的 Azure 訂用帳戶，都會以當地貨幣計價和計費。 將不會使用 FX 費率。

### <a name="track-your-transition-details"></a>追蹤您的轉換詳細資料

在 Azure 入口網站和合作夥伴中心追蹤進度。

:::image type="content" source="images/azure/details1.png" alt-text="顯示詳細資料":::

### <a name="billing-impact-to-partners"></a>對合作夥伴的計費影響

如果您從現有的 CSP Azure 供應項目轉換客戶，將會有下列計費影響：

- 您將需支付截至結束原始 CSP Azure 訂用帳戶時間點，所有使用量的現有 CSP 發票費用。

- 如果您擁有現有 CSP 訂用帳戶的系統管理員存取權限，則在遷移該訂用帳戶時，您將會繼續擁有存取權。

若要將 CSP 和伺服器和雲端註冊的直接 Enterprise 合約轉換至Azure 服務，請參閱[取得 Microsoft 合作夥伴合約 Azure 訂用帳戶的計費擁有權](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>稽核記錄

若要調解計費，請在 [訂用帳戶] 頁面上，檢視您的 "Microsoft Azure" (0145P) 訂用帳戶的歷程記錄。

"Microsoft Azure" (0145P) 訂用帳戶由兩個部分組成：

1. 商務訂用帳戶
2. Azure 訂用帳戶 (權利)

轉換完成時，會將 Azure 訂用帳戶移至新的 Azure 方案底下，並暫停商務訂用帳戶，這樣就不會再報告有使用量。  

>[!Note]
>當 Microsoft Azure (0145P) 訂用帳戶是在 CSP 中購買時，商務訂用帳戶和 Azure 訂用帳戶 (權利) 會具有相同值。 只有在計費擁有權變更或傳輸的情況下，這些值才會有所不同。

### <a name="transition-issues"></a>轉換問題

轉換期間發生任何問題並不在預料之中。 如果發生失敗情況，我們會在轉換工作流程本身中為您更新。 Azure 使用量不會受到干擾。  

## <a name="next-steps"></a>接下來的步驟

- [管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)

- [合作夥伴所獲得信用點數 - 概觀](partner-earned-credit.md)
