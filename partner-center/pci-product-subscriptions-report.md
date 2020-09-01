---
title: 合作夥伴中心 Insights 訂閱報表
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解您的表現如何，以及您可以針對客戶銷售或管理的雲端訂用帳戶改進。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8df91ec4072b1873a240d42fa2382ebcc00b9bc5
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220326"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>可從合作夥伴中心 Insights 儀表板取得的產品訂閱報表

**適當的角色**
- 全域系統管理員
- 系統管理代理人
- 報表檢視器
- 執行報表檢視器

產品訂用帳戶報表會針對您已銷售或為客戶管理的雲端訂用帳戶提供分析。 這是產品專屬的報表，其中包含與雲端產品（例如 Office 365、Azure、Dynamics 等）相關聯的訂閱效能。

您可以從產品訂用帳戶報表中查看下列章節。

- [摘要]
- 訂用帳戶的地理散佈
- 訂用帳戶新增/流失趨勢
- 依合作夥伴位置、銷售通路、Sku、合作夥伴附加類型、區段的訂用帳戶散發
- 依訂用帳戶狀態的趨勢
- 產品趨勢

 > [!NOTE]
 > 您可以從見解儀表板取得此報表。 若要查看此報表，您必須在合作夥伴中心中指派特定角色，例如全域管理員、帳戶管理員、報表檢視器或執行報表檢視器。 如需詳細資訊，請參閱貴公司的全域管理員。這份報表中的特定資料類型，可能也只適用于具有主管報表檢視器許可權的使用者。

## <a name="summary"></a>[摘要]

[摘要] 區段會顯示「關鍵效能指標」的快照集觀點， (Kpi) 與您為客戶銷售或管理的訂用帳戶相關的訂用帳戶。  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="訂閱報表摘要":::

如需摘要各區段的詳細資訊，請參閱下文。

- 訂用帳戶:
  - 您目前銷售或管理的雲端產品訂用帳戶計數。
  - 在您選取的日期範圍內，訂用帳戶的成長百分比或拒絕。
  - 微圖表會顯示所選日期範圍內的每月訂用帳戶計數趨勢。

- 有效訂閱：
  - 目前的雲端產品訂用帳戶計數，使用以產品遙測為基礎的有效使用量。 這會排除 Azure 訂用帳戶的所有試用版訂閱。
  - 所選時段內的作用中訂用帳戶成長或拒絕百分比。
  - 微圖表會在您選取的日期範圍內，顯示使用中訂用帳戶的月數趨勢。

- 新增的訂閱：
  - 在選取的日期範圍內，新增 (銷售或受控) 的客戶訂用帳戶總計。 具有作用中或已**更新****狀態的新**訂用帳戶會視為新增訂閱。
  - 在上個月中，相較于第一個完整月份，增加或拒絕訂用帳戶的成長百分比。
  - 微型圖會顯示在您選取的日期範圍內所新增之訂用帳戶的每月趨勢。

- 訂閱流失：
  - 在您選取的日期範圍內流失的客戶訂用帳戶總計。 狀態為 **取消布建** 或在該月份 **暫停** 的訂用帳戶，會計算為流失訂用帳戶。  
  - 在選取的日期範圍內流失的訂閱百分比。
  - 微圖表會顯示流失在選取的日期範圍內的每月訂閱趨勢。

- 依產品的訂用帳戶：依雲端產品的目前訂用帳戶計數明細。

## <a name="geographical-spread-of-subscriptions"></a>訂用帳戶的地理散佈

**依地理位置**的訂用帳戶會依客戶市場顯示訂用帳戶總計的地理分佈。 訂用帳戶總計數量包括銷售的訂閱和使用中的訂用帳戶。

[ **國家/地區** ] 資料表會顯示您有訂用帳戶的所有國家/地區，以及總和使用中訂用帳戶的每個國家/地區數量。

您可以搜尋並選取方格中的國家/地區，以縮放至地圖中的位置。 在地圖上按 **Home** 選項，以還原為原始視圖。 將滑鼠停留在地圖上，以依國家/地區查看所有訂閱和使用中的訂閱。 方格上的這兩個欄位都可以排序。

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="依地理位置的訂閱":::

## <a name="subscription-addschurns"></a>訂用帳戶新增/變換

此視圖顯示訂閱的趨勢。 這些會細分成不同的類別 (新的、現有的流失) 選取的日期範圍。 X 軸代表所選日期範圍的月份。 Y 軸代表訂用帳戶計數。 流失訂用帳戶會以 Y 軸的負位數表示。 

堆疊直條圖會顯示當月新的、現有的和流失的訂閱明細。 您可以重建直條圖，並將其與特定的堆疊專案分開。 若要這樣做，請選取圖例中的特定專案。 您也可以利用圖表頂端的滑杆來放大特定的期間。

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="訂用帳戶新增和變換":::

## <a name="subscription-distribution"></a>訂用帳戶散發

此視圖會依您的 MPN 位置、客戶區段、銷售通路/Azure 定價模型和屬性 (類型（例如 DPOR、) 等），提供您目前訂用帳戶的明細。 按一下個別的索引標籤，以依這些分類來查看細目。 若要使用特定專案類別的明細來建立圓形圖，請在 [圖例] 中選取這些專案類別。

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="訂用帳戶散發":::

## <a name="subscription-state-distribution"></a>訂用帳戶狀態分佈

此視圖會依訂用帳戶狀態或狀態，顯示目前客戶訂用帳戶的散發。 這包括下列訂用帳戶狀態： **Active**、 **Disabled**、 **取消布建**、 **Open**、 **InGracePeriod**、 **Closed**和 **其他**。

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="訂用帳戶狀態分佈":::

## <a name="products-trend"></a>產品趨勢

這個視圖會顯示橫條圖和兩張圓形圖。 橫條圖顯示依商業產品細分的每月訂用帳戶趨勢，例如 Azure、Office、Dynamics 等等。

這兩個圓形圖會顯示您目前客戶訂用帳戶的明細。 第一個圓形圖會依產品細分訂閱。 第二個圓形圖會依 Sku 或方案細分訂用帳戶。 當您選取 [ **依產品** 劃分的明細] 圓形圖中的產品時，連續的圓形圖會顯示該產品的訂用帳戶依據 sku 的明細。

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="產品趨勢":::

> [!NOTE]
 > 依 Sku 細分的訂用帳戶計數可能不一定會符合該產品的總訂用帳戶計數。 如果客戶已在相同的產品訂用帳戶下購買多個 Sku，就可能發生這種情況。

## <a name="next-steps"></a>後續步驟

- 如需詳細報表，請參閱 [合作夥伴中心 Insights](partner-center-insights.md)。

>[!NOTE] 
> 您可以從 [見解] 儀表板的 [下載報告] 區段中，下載開啟此報表的原始資料。 [深入了解](pci-download-reports.md) 
