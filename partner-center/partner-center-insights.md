---
title: 合作夥伴中心深入解析
description: 探索此合作夥伴中心整合報表儀表板。 瞭解您要如何在 Kpi 中進行銷售和部署、客戶開發等等。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI，效能，客戶成功，測量，報告資料
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: c9a80519ab418c0b0c52bbf7e0224e439b4f672e
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467528"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a>合作夥伴中心深入解析-顯示 Microsoft 商業夥伴如何執行的儀表板

**適當的角色**
- 全域系統管理員
- 帳戶管理員
- 高階報告檢視人員
- 報告檢視人員

## <a name="introduction"></a>簡介

深入解析是合作夥伴中心的整合報表儀表板，適用于在 Microsoft 合作夥伴網路（MPN）方案中註冊的 Microsoft 商業合作夥伴。 深入解析儀表板會針對雲端產品（例如 Office、Azure、Dynamics 和授權模型，如 CSP 和 EA）提供360度的關鍵效能指標（KPI）觀點。 它會公開一組豐富的 KPI 報表，可協助您為組織做出資料驅動的決策。 

## <a name="role-based-access-control-to-the-insights-dashboard"></a>深入解析儀表板的角色型存取控制

合作夥伴中心有兩個特別針對存取見解而設計的新角色： [**報表檢視器**] 和 [**執行報表檢視器]**。 執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取機密資料集，例如收益和客戶/員工個人資料。 

全域管理員或帳戶管理員可以將這些角色指派給使用者，並且指派給整個公司或特定 MPN 位置。  

>[!Note] 
>從2019年12月2日起 MPN 系統管理員的使用者，會自動新增至全公司的報表檢視器角色。 他們能夠以報表檢視器的形式存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員或帳戶管理員可以視需要覆寫這些指派。 

## <a name="reports-available"></a>可用的報表

下列報表可作為 Insights 儀表板的一部分。

**總覽**：總覽報表會提供您感的各種不同 kpi 的快照集，例如客戶計數、使用中訂用帳戶計數、Azure 耗用量收益、作用中授權等等。

**客戶**：客戶報表會向您的客戶呈現分析，例如客戶取得資料、作用中客戶等。

**產品-** 訂用帳戶：訂用帳戶報表會針對您的雲端訂用帳戶（例如 O365、Azure、Dynamics 等）顯示取得和使用方式分析。

**產品授權**： [授權] 儀表板會針對以授權為基礎的雲端產品（例如 O365、Dynamics、Power BI 等）提供授權分析。

**產品-azure 使用方式**： azure 使用量報表會顯示與您客戶的 azure 訂用帳戶相關的計量，包括依計量分類的 azure 耗用量收益和使用量。

專長**認證：職稱**報表會針對您的使用中、合格和有風險的專長呈現計量。

**優點**： [權益] 報表會針對您已獲得與取用的合作夥伴權益提供分析。

## <a name="navigating-the-insights-reports"></a>導覽見解報告

**日期範圍篩選**：您可以在每個頁面的右上角找到日期範圍選取專案。 您可以選取以過去3、6或12個月為基礎的日期範圍，或選取自訂的日期範圍，以自訂 [總覽] 頁面圖形的輸出。 預設的日期範圍選取為12個月。 

:::image type="content" source="images/pci/intro1.png" alt-text="簡介地圖":::

**意見反應按鈕**：所有 Insights 報告中的每個圖表/控制項都會加上 [意見反應] 按鈕，讓您提供報表功能的實例意見反應。 

 
**頁面層級篩選**：除了 [總覽]、[權益] 和 [專長認證] 報表以外，所有 Insights 報表都可讓您套用頁面層級篩選。 

- 選取的篩選準則將適用于頁面上的所有圖表和計量，包括 [摘要] 區段。 如果您在該篩選準則中有任何資料，就可以使用篩選項目。 

- 每個篩選器清單的預設選取專案為 [**全部**]。 例如，如果您尚未選取 [產品] 篩選中的特定產品，預設選項會是 [所有產品]。

- 選取的篩選器會顯示在頁面頂端。 

:::image type="content" source="images/pci/filters.png" alt-text="濾波器":::

### <a name="filters-definitions"></a>篩選定義：

- 產品：您的組織所銷售/管理的所有 Microsoft Cloud 產品清單，例如 O365、Azure、D365 移轉、EMS、PowerBI 等等。
- 客戶市場：客戶國家/地區清單
- 合作夥伴歸屬：您與您的客戶訂用帳戶相關聯的關聯類型，例如，數位合作夥伴記錄（DPOR）、委派的系統管理員許可權（聯盟）、合作夥伴系統管理員連結（PAL）等。 
- 合作夥伴位置：所有組織的 MPN 位置清單。
- 銷售通路：您用來購買/布建產品和服務的所有銷售通路/定價，亦即 CSP、EA、CSP 間接、Direct、Advisor、Open、其他
- 客戶區段：合作夥伴客戶群之間的客戶區段清單。

## <a name="read-about-each-of-the-dashboards-and-reports"></a>閱讀每個儀表板和報表：

- [合作夥伴中心深入解析-總覽儀表板](pci-overview-report.md)

- [合作夥伴中心深入解析 - 客戶儀表板](pci-customer-report.md)

- [合作夥伴中心深入解析-訂閱報表](pci-product-subscriptions-report.md)

- [合作夥伴中心深入解析-授權報表](pci-product-licenses-report.md)

- [合作夥伴中心深入解析-Azure 使用方式報表](pci-azure-usage-report.md)

- [合作夥伴中心深入解析 - 專長認證報表](pci-competencies-report.md)

- [合作夥伴中心深入解析 - 權益報表](pci-benefits-report.md)
