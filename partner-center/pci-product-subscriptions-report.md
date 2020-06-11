---
title: 合作夥伴中心深入解析訂閱報表
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解您的表現如何，以及您對客戶銷售或管理的雲端訂閱有何改進。
ms.assetid: ''
keywords: PCI，效能，度量，客戶成功，雲端訂閱，分析，報告
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d4896fbff07eebc1dd6debf6010dc3970f45a4a
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679315"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>[合作夥伴中心深入解析] 儀表板提供的產品訂閱報表

**適當的角色**
- 全域系統管理員
- 系統管理代理人
- 報表檢視器
- 執行報表檢視器

[產品訂用帳戶] 報表會針對您所銷售或您為客戶管理的雲端訂用帳戶提供分析。 這是產品特定的報告，其中包含與雲端產品（例如 Office 365、Azure、Dynamics 等）相關聯的訂閱效能。

您可以從 [產品訂閱] 報表中查看下列區段。

- 摘要
- 訂用帳戶的地理分佈
- 訂閱新增/變換趨勢
- 依合作夥伴位置、銷售通路、Sku、合作夥伴附加類型、區段的訂用帳戶散發
- 依訂用帳戶狀態的趨勢
- 產品趨勢

 > [!NOTE]
 > 您可以從 Insights 儀表板取得這份報表。 若要查看這份報告，您必須在合作夥伴中心指派特定角色，例如全域管理員、帳戶管理員、報表檢視器或執行報表檢視器。 如需詳細資訊，請參閱貴公司的全域管理員。這份報表中的特定資料類型，也只能供具備主管報表檢視器許可權的使用者使用。

**摘要**

[摘要] 區段會顯示與您為客戶銷售或管理之訂用帳戶相關之關鍵效能指標（Kpi）的快照集。  

- 訂用帳戶：您所銷售或管理的雲端產品訂用帳戶目前計數。
在您選取的日期範圍內，訂用帳戶成長或拒絕的百分比。

微圖表會在您選取的日期範圍內，顯示訂用帳戶計數的月間趨勢。

- 作用中訂用帳戶：目前的雲端產品訂用帳戶計數，並根據產品遙測測量使用中的使用量。 這會排除 Azure 訂用帳戶的所有試用訂閱。
所選時段內作用中訂閱的成長或拒絕百分比。

微圖表會在您選取的日期範圍內，顯示作用中訂用帳戶的月數月趨勢。

- 新增的訂用帳戶：您在選取的日期範圍內新增（銷售或管理）的客戶訂用帳戶總數。 具有作用中或已**更新**狀態的新訂用帳戶會計入**新增的訂閱**。
相較于第一個完整月份，過去一個月內新增的訂閱百分比成長或拒絕。

微圖表會顯示在您選取的日期範圍內新增的訂閱每月趨勢。

- 訂閱變換：在您選取的日期範圍內的客戶訂用帳戶變換總計。 在該月份中狀態為**取消布建**或已**暫停**的訂用帳戶會視為變換訂閱。  
在選取的日期範圍期間變換的訂用帳戶百分比。

微圖表會顯示在選取的日期範圍內，變換訂用帳戶的每月趨勢。

- 依產品的訂閱：依雲端產品的目前訂用帳戶計數明細。

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="訂閱報表摘要":::

**訂用帳戶的地理分佈**

[**依地理位置的訂閱**] 視圖會顯示客戶市場的總訂閱的地理分佈。 總訂用帳戶數量包含銷售的訂閱和使用中的訂閱。

[**國家/地區**] 資料表的數目會顯示您的訂用帳戶的國家/地區總計，以及總和作用中訂用帳戶的每個國家/地區數量。

您可以搜尋並選取方格中的國家/地區，以縮放至地圖中的位置。 按下地圖上的 [**首頁**] 選項，以還原成原始的視圖。 將滑鼠停留在地圖上，以依國家/地區查看所有訂閱和作用中訂閱。 格線上的兩個欄位都可以排序。

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="依地理位置的訂閱":::

**訂用帳戶新增/變換**

此視圖會顯示訂閱的趨勢。 這些會細分為所選日期範圍的不同類別（新的、現有的變換）。 X 軸代表所選日期範圍的月份。 Y 軸代表訂用帳戶計數。 變換訂用帳戶會在 Y 軸的負值尺規上表示。 

堆疊直條圖會顯示當月新的現有和變換訂閱的明細。 您可以重建直條圖，並使用特定的堆疊專案來細分。 若要這麼做，請選取圖例中的特定專案。 您也可以利用圖表頂端的滑杆來放大特定期間。

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="訂用帳戶新增和變換":::

**訂用帳戶散發**

此視圖會根據您的 MPN 位置、客戶區段、銷售通路/Azure 計價模式和屬性類型（例如 DPOR、等），顯示您目前訂用帳戶的明細。 按一下個別的索引標籤，以查看這些類別的明細。 若要使用特定專案類別的細目來建立圓形圖，請在圖例中選取這些專案類別目錄。

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="訂用帳戶散發":::

**訂用帳戶狀態散發**

此視圖會依訂用帳戶狀態或狀態顯示目前客戶訂閱的散發。 這包括下列訂用帳戶狀態： **Active**、 **Disabled**、**取消布建**、 **Open**、 **InGracePeriod**、 **Closed**和**其他**。

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="訂用帳戶狀態散發":::

**產品趨勢**

這個視圖會顯示橫條圖和兩個圓形圖。 橫條圖顯示依商業產品（例如 Azure、Office、Dynamics 等）細分的訂用帳戶每月趨勢。

這兩個圓形圖會顯示目前客戶訂用帳戶的明細。 第一個圓形圖會依產品細分訂閱。 第二個圓形圖會依 Sku 或方案細分訂閱。 當您選取 [**依產品**細分] 圓形圖中的產品時，連續的圓形圖會顯示該產品的訂用帳戶依據 sku 的明細。

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="產品趨勢":::

> [!NOTE]
 > 依 Sku 細分的訂用帳戶計數可能不一定會符合該產品的總訂用帳戶計數。 如果客戶已在相同的產品訂用帳戶下購買多個 Sku，就可能發生這種情況。

## <a name="next-steps"></a>後續步驟

- 如需更多報告，請參閱[合作夥伴中心深入](partner-center-insights.md)解析。
