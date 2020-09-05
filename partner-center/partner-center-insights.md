---
title: 合作夥伴中心深入解析
description: 探索此合作夥伴中心統一的報告儀表板。 瞭解您如何在 Kpi 中進行銷售和部署、客戶開發等等。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: 2b1a09253b7a9e9c8863f07b729ad116689a4642
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490626"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>合作夥伴中心 Insights-顯示 Microsoft 商業夥伴如何執行的儀表板

**適當的角色**
- 全域系統管理員
- 帳戶管理員
- 高階報告檢視人員
- 報告檢視人員

## <a name="introduction"></a>簡介

深入解析是合作夥伴中心中的整合報告儀表板，已在 Microsoft 合作夥伴網路 (MPN) 計畫中註冊的 Microsoft 商業合作夥伴。 深入解析儀表板可讓您在各種雲端產品（例如 Office、Azure、Dynamics 及授權模型，例如 CSP 和 EA）之間， (KPI) 的關鍵效能指標的360度觀點。 它會公開一組豐富的 KPI 報告，協助您為組織做出資料驅動的決策。 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>深入解析儀表板的角色型存取控制

合作夥伴中心有兩個新的角色專門設計來存取見解： **報表檢視器** 和 **執行報表檢視器**。 執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取敏感資料集，例如收益和客戶/員工的個人資料。 

全域管理員或帳戶管理員可以指派這些角色給使用者，或指派給整個公司或特定的 MPN 位置。  

>[!Note] 
>從2020年1月20日 MPN 系統管理員的使用者，會自動新增至全公司的報表檢視器角色。 他們能夠以報表檢視器的形式存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員或帳戶管理員可以視需要覆寫這些指派。 

## <a name="reports-available"></a>可用的報表

下列報告可作為見解儀表板的一部分。

**總覽**：總覽報表會呈現您感興趣的各種 kpi 的快照集觀點，例如客戶計數、使用中的訂用帳戶計數、Azure 耗用量收入、使用中的授權等。

**客戶**：客戶報表提供客戶的分析，例如客戶取得資料、主動式客戶等。

**產品-** 訂用帳戶：訂用帳戶報表會針對您的雲端訂用帳戶提供取得和流量分析 (例如 O365、Azure、Dynamics 等 ) 

**產品授權**：授權儀表板會針對以授權為基礎的雲端產品（例如 O365、Dynamics、Power BI 等）提供授權分析。

**產品-azure**使用量： azure 使用量報表會呈現與您客戶的 azure 訂用帳戶相關的計量，包括 azure 使用量收益和依計量類別的使用量。

專長**認證：專長**認證報告會針對您的主動式、合格及具風險的專長認證提供度量。

**優點**：權益報表針對您已獲得和取用的合作夥伴權益提供分析。

## <a name="navigating-the-insights-reports"></a>流覽見解報表

**日期範圍篩選器**：您可以在每個頁面的右上角找到日期範圍選取範圍。 您可以選取以過去3、6或12個月為基礎的日期範圍，或選取自訂日期範圍，來自訂總覽頁面圖形的輸出。 預設的日期範圍選項為12個月。 

:::image type="content" source="images/pci/intro1.png" alt-text="簡介地圖":::

**意見反應按鈕**：所有深入解析報表中的每個圖表/控制項都會與意見反應按鈕合併，讓您針對報表功能提供實例意見反應。 

 
**頁面層級篩選**：除了總覽、權益和專長認證報表之外，所有深入解析報表都可讓您套用頁面層級篩選。 

- 選取的篩選準則將適用于頁面上的所有圖表和計量，包括 [摘要] 區段。 如果您在該篩選準則中有任何資料，則可以使用篩選項目。 

- 每個篩選清單的預設選項為 [ **全部**]。 例如，如果您尚未在 [產品] 篩選中選取特定產品，預設選取專案將會是 [所有產品]。

- 選取的篩選器會顯示在頁面頂端。 

:::image type="content" source="images/pci/filters.png" alt-text="顯示已套用篩選準則列的部分螢幕擷取畫面，其中包含產品、客戶市場、合作夥伴歸屬和銷售通路的篩選選取專案。":::

### <a name="filters-definitions"></a>篩選定義：

- 產品：您的組織所銷售/管理的所有 Microsoft 雲端產品的清單，例如 O365、Azure、D365、EMS、Power BI 等等。
- 客戶市場：客戶國家/地區清單
- 合作夥伴歸屬：您的客戶訂用帳戶的關聯類型，例如記錄的數位夥伴 (DPOR) 、委派的系統管理員許可權 (聯合) 、合作夥伴系統管理員連結 (PAL) 等。 
- 合作夥伴位置：所有組織的 MPN 位置清單。
- 銷售通路：您購買/布建產品和服務的所有銷售通路/定價，亦即 CSP、EA、CSP 間接、Direct、Advisor、Open、其他
- 客戶區段：各合作夥伴客戶群的客戶區段清單。

## <a name="read-about-each-of-the-dashboards-and-reports"></a>閱讀每個儀表板和報表的相關資訊：

- [合作夥伴中心 Insights-總覽儀表板](pci-overview-report.md)

- [合作夥伴中心深入解析 - 客戶儀表板](pci-customer-report.md)

- [合作夥伴中心 Insights-訂閱報表](pci-product-subscriptions-report.md)

- [合作夥伴中心 Insights-授權報表](pci-product-licenses-report.md)

- [合作夥伴中心 Insights-Azure 使用量報表](pci-azure-usage-report.md)

- [合作夥伴中心深入解析 - 專長認證報表](pci-competencies-report.md)

- [合作夥伴中心深入解析 - 權益報表](pci-benefits-report.md)
