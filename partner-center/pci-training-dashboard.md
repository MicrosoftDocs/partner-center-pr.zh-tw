---
title: 深入解析訓練儀表板。
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 探索合作夥伴中心訓練儀表板。 訓練是合作夥伴中心 Insights (PCI) 區域中可用的其中一個報表。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10646cb4ecc6c48c5187c96740a2c05610c9d3cc
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175259"
---
# <a name="trainings-dashboard"></a>訓練儀表板

**適當的角色**
- 高階報告檢視人員
- 報告檢視人員

訓練儀表板提供公司員工公司所採取之認證、評量及考試的見解。 定型儀表板包含下列各節：

- 總結
- 依認證、評量、測驗來分割的定型效能
- 憑證、評量、測驗等認證的個人
- 活動詳細資料

>[!NOTE] 
>這份報告可在合作夥伴中心的 Insights 中樞底下取得。 若要查看這份報表，您應該將報表檢視器或執行報表檢視器的角色指派給您。 只有執行報表檢視器的使用者可以看到此報表的一些區段。 如需深入解析報表存取控制的相關資訊，請參閱 [PCI 角色](pci-roles.md)。

## <a name="summary"></a>總結

[摘要] 區段會顯示與您的訓練相關的各種效能指標的數值快照集。 各種效能指標是經過認證的個人、認證、具有測驗認證的個人、測驗認證、具有評量認證和評量認證的個人。 此區段中的資料會根據選取的日期範圍重新整理，這可能是三個月 (3M) 、六個月 (>6 分鐘) & 12 個月 (1Y) 或自訂資料範圍 (自訂) 。 

:::image type="content" source="images/pci/td-summary.png" alt-text="總結":::

- **具有認證的個人**：代表公司中具有認證的不同個人人數。
- 憑證**計數**：代表公司中的個人所採用的認證總數。
- **具有評**量的個人：代表您公司中具有評量認證的不同個人數目。 
- **評量計數**：代表公司的個人所採取的評定總數。
- **具有**檢查功能的個人：代表您公司中具有檢查認證的相異個人數目。 
- **檢查計數**：代表公司中的個人所採取的檢查總數。

## <a name="training-performance"></a>定型效能

定型效能會顯示每月的個人人數，以及貴公司的個人所完成的訓練。 它會依認證、評量及測驗，以圖表的形式針對選取的日期範圍進行分割。 X 軸代表所選日期範圍的月份。 Y 軸代表所選定型類型的個人和所採用訓練數目的相異計數。 按一下圖表上方的個別索引標籤，以依訓練類型來查看細目。 您可以透過下載圖示，以 tsv 格式下載所選取日期範圍的圖表資料。

:::image type="content" source="images/pci/td-training-performance.png" alt-text="總結":::

## <a name="individuals-performance"></a>個人效能

[個人] 的 [效能] 區段會針對選取的日期範圍，顯示貴公司的個人所採取之定型的詳細資料。 在區段的左面板中搜尋並選取個人的名稱。 所選人員的定型詳細資料會顯示在區段的右面板上。

:::image type="content" source="images/pci/td-indiviual-performance.png" alt-text="總結":::

>[!NOTE] 
> [個人] 效能區段僅適用于執行報表檢視器的使用者。 

## <a name="next-steps"></a>後續步驟

[合作夥伴中心 Insights 中的報表](partner-center-insights.md)

>[!NOTE] 
> 您可以從 [見解] 儀表板的 [下載報告] 區段中，下載開啟此報表的原始資料。 [深入了解](pci-download-reports.md)