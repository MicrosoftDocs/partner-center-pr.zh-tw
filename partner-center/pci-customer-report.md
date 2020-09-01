---
title: 合作夥伴中心 Insights-客戶報表
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 探索改善業務的方式。 依地理位置、產品和其他屬性查看您的特定客戶趨勢。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 30032a9b396a82f530c9497f96e4a9b1f6b46e00
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220496"
---
# <a name="customers-dashboard-reports-from-partner-center-insights"></a>來自合作夥伴中心見解的客戶儀表板報告

客戶儀表板會顯示客戶的資料，這些客戶已透過您取得 Office、Azure、Dynamics 等雲端產品，或使用您在其租使用者中部署及管理這些產品。 
 
[客戶] 儀表板包含下列區段： 

- [摘要]  
- 客戶的地理散佈 
- 客戶新增/流失趨勢 
- 依合作夥伴地點、客戶區段、銷售通路、合作夥伴屬性類型分配的客戶 
- 依產品的客戶分佈 
- 依合作夥伴地點、客戶區段、計價模式、合作夥伴屬性類型的客戶分佈趨勢 
- 活躍客戶趨勢 

## <a name="summary"></a>[摘要]

[摘要] 區段會顯示與您的客戶相關的各種 Kpi 的快照集，例如客戶、使用中客戶、訂用帳戶、新增的客戶、客戶流失，以及每個產品的客戶。 頁面層級篩選適用于每個區段。

:::image type="content" source="images/pci/customerproduct.png" alt-text="[客戶摘要] 儀表板的螢幕擷取畫面會顯示橫條圖，以及使用中、最近新增、遺失/流失或特定產品的客戶數目。":::

### <a name="customers"></a>客戶

- 您組織中所有雲端產品（例如 Office、Azure、Dynamics 等）之不同屬性類型的所有客戶目前的計數。如果客戶至少有一個具有作用中狀態的訂用帳戶，則會進行計算。  
- 在選取的日期範圍內拒絕客戶的% 
- 微型圖顯示所選日期範圍內客戶計數的月數趨勢

### <a name="active-customers"></a>活動客戶

- 目前具有任何使用中產品使用量的客戶計數，例如任何雲端產品上的使用中。
- 在選取的時間週期內，使用中客戶的成長或拒絕百分比
- 微型圖顯示所選日期範圍內的作用中客戶計數的月數趨勢。

### <a name="customers-added"></a>新增的客戶

- 在所選時段內新增的所有客戶計數。
- 在選取的不良範圍內新增的客戶成長或拒絕%。
- 微型圖顯示在選取的日期範圍內，客戶所新增的月趨勢。

### <a name="customers-churned"></a>客戶流失
- 在所選時段內每個月流失的所有客戶計數。 如果客戶沒有處於作用中狀態的單一訂用帳戶，則會將客戶視為遺失。 
- 在選取的日期範圍內流失的客戶% 
- 微型圖提供在所選時間週期內流失客戶的月趨勢 
 
### <a name="customers-by-products"></a>依產品的客戶

- 在各種雲端產品（例如 O365、Azure、Dynamics 等）上散發的客戶目前計數。  

## <a name="geographical-spread-of-your-customers"></a>客戶的地理散佈

目前客戶的計數、目前作用中的客戶，以及在選取的日期範圍內新增的客戶，都會使用客戶的國家（地區）進行地理對應。 度量下方顯示的百分比表示該國家/地區的總計占該國家/地區總計的百分比。 您可以將滑鼠停留在地圖上，以查看該國家/地區的總計、使用中的新客戶。 您可以搜尋並選取方格中的國家/地區，以縮放至地圖中的位置。 選取地圖上的 [ **首頁** ] 按鈕，還原為原始的視圖。 方格中的所有資料行都可以排序。  

:::image type="content" source="images/pci/customersgeo.png" alt-text="依地理位置顯示的合作夥伴中心 Insights 客戶報表的螢幕擷取畫面，會顯示世界地圖以及依區域的總計、新增及新客戶的清單。":::

## <a name="customer-adds-and-churns"></a>客戶新增和變換

客戶的趨勢，並在選取的日期範圍內細分為新的、現有的流失。 X 軸代表所選日期範圍的月份，而 Y 軸代表客戶計數。 流失客戶會以 Y 軸的負向比例表示。 堆疊直條圖提供本月新的、現有的流失客戶並劃分。 您可以選取圖例中的特定堆疊專案來重建直條圖。 您可以利用圖表頂端的滑杆來放大特定期間。 

:::image type="content" source="images/pci/customerslost.png" alt-text="具有橫條圖的合作夥伴中心 Insights 客戶報表的螢幕擷取畫面，顯示在一段特定時間內新增和遺失或流失的客戶數目。":::

## <a name="customer-distribution"></a>客戶分佈

依您的 MPN 地點、客戶區段、銷售通路/Azure 定價模型和屬性類型 (的明細，例如 DPOR、等 ) 。 按一下圖表上方的個別索引標籤，以依這些分類來查看細目。 您可以藉由選取 [圖例] 專案來選取/取消選取特定的維度來重建圖表。 

## <a name="customers-by-products"></a>依產品的客戶

您目前客戶的明細依產品和 Sku/方案計算。 在 product 並劃分圓形圖中選取產品，以依下圖中的 Sku/方案來查看並劃分。

:::image type="content" source="images/pci/customerbyprod.png" alt-text="依產品顯示的客戶螢幕擷取畫面會顯示兩個放射圖：一個具有依產品分類的客戶明細，另一個則包含客戶明細（依 SKU）。":::

## <a name="customer-distribution-trend"></a>客戶分佈趨勢 

在選取的日期範圍內，您的客戶在選取的日期範圍內的每月分佈趨勢（依市場、區段、MPN 地點和他們所取得的產品）。 按一下圖表中的個別索引標籤，以依這些分類來查看趨勢。 X 軸代表您所選日期範圍的月份，而 Y 軸則是所選類別的客戶計數， (索引標籤選取範圍) 。 您可以將滑鼠停留在圖表資料行上，以查看每個堆疊的值並劃分。 您可以利用圖表頂端的滑杆來放大特定期間。   

:::image type="content" source="images/pci/customerdistri.png" alt-text="客戶分佈趨勢報表的螢幕擷取畫面，其中顯示可依市場、部門、合作夥伴地點或產品查看的橫條圖。":::

## <a name="active-customers"></a>活動客戶

比較所選日期範圍內的作用中與客戶總計的每月趨勢圖。 資料行代表每個月的使用中客戶計數，每月代表客戶總數。 

:::image type="content" source="images/pci/activecustomer.png" alt-text="顯示作用中客戶一段時間之橫條圖的合作夥伴中心見解作用中客戶報表的螢幕擷取畫面。":::

## <a name="next-steps"></a>後續步驟

如需詳細報表，請參閱 [合作夥伴中心 Insights](partner-center-insights.md)。

>[!NOTE]
> 您可以從 [見解] 儀表板的 [下載報告] 區段中，下載開啟此報表的原始資料。 [深入了解](pci-download-reports.md) 
