---
title: 合作夥伴中心 Insights-CloudAscent 傾向報告
description: 瞭解合作夥伴中心儀表板中的 CloudAscent 傾向報告。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 510f85b053ec17fa0a2a66217a19c006e7ca2bc9
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811332"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent 可從合作夥伴中心儀表板取得的傾向報表

**適當的角色**
- 高階報告檢視人員
- 報告檢視人員

合作夥伴中心儀表板會從 CloudAscent 程式提供可下載的傾向資料。 此資料會顯示客戶購買 Microsoft 產品的傾向。  本文說明這項資料的細目、如何運用評分，以及其意義。

## <a name="summary-definitions"></a>摘要定義

- **SMC 客戶**–這是傾向下載中的客戶總數。  客戶是由記錄的夥伴所識別。
- **過期協定**-在目前會計年度內，我們會提供過期協定的數目。
- **過期的收入**–與過期合約相關聯的收入。
- **開啟過期的收入**–與開放式過期合約相關聯的收入。

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB 分割

小型至中型企業 (SMB) 區段會進一步分成三個不同的子區段。

1. **頂級非受控** 包括最大的 SMB 客戶，最具 Microsoft 的商機。 一般未受管理的客戶與受管理的帳戶共用類似的特性，有大量員工、大量的 IT 預算和支出，以及 Microsoft 的大量潛在收入。

   我們定義了最常見的雙重非受控方法：

   - **最常見的非受控使用者**-包含具有300或更多員工的帳戶。 以使用者為基礎的帳戶是首次購買或擴充以使用者為基礎的訂閱產品（例如 M365、D365 或 Surface）的絕佳目標。
   - 以**最上層非受控計算為基礎**–包括 Azure 可能大於 $ 10k 的帳戶。 以計算為基礎的帳戶包括現有的 Azure。 有多年來的帳戶，以及尚未購買 Azure 的帳戶，但 Azure 可能大於 $ 10k 的帳戶。

2. **中型企業** 包含擁有25至300員工的現有客戶和潛在客戶帳戶。

3. **Small Business** 包含擁有25位以上員工的所有剩餘企業。

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="依 SMC 類型的客戶。":::

**最常見的非受控** 和 **中型企業** e1edp01 子代表高生命時間價值 (LTV) 客戶給 microsoft 和 microsoft 合作夥伴。 因此，它們是在此區段中推動成長的潛在客戶領域。 在這兩個 e1edp01 子中，我們最好是使用 M365 取得通訊端，再銷售 D365/Azure 企業營運 (LOB) 應用程式，並實現 Microsoft 的高 LTV。

今天，我們有兩個主要的商機範圍–1。 我們的客戶增加了成長;二級. 雖然我們可以取得 M365 的雲端通訊端，但我們在 D365 和 Azure 中有很大的機會。

下列螢幕擷取畫面顯示三個 SMB E1edp01 子與市場的優化路由。 CloudAscent 會優先處理所有最上層非受控與中型企業帳戶的分析、評分和模型化。

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="SMB e1edp01 子的螢幕擷取畫面。":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB 使用機器學習技術，在最上層非受控和中業務區段內推動銷售和行銷客戶預測。 如何收集信號並將其轉換為傾向建議？

- **資料收集**： Web 編目程式會藉由 ping 公司網域來掃描及收集數十億個客戶信號，並監視： blog 文章、電子報、社交串流和技術論壇。  除了收集到的信號之外，也會從內部和外部來源（例如 D&B、Microsoft 內部訂用帳戶和交易資料）收集 firmographics 資訊。

- **Machine Learning**：會將信號送入機器學習模型，以針對每個客戶依雲端產品和叢集輸出一組結構化的銷售和行銷預測資料集。  每個客戶都會使用外觀類似的模型來評分，以決定客戶的適合程度，並使用機器學習演算法來將客戶的線上行為定義整合為意圖。 評分會合並到叢集，以顯示客戶的傾向以購買 Microsoft 雲端產品。

- **優化**： Machine Learning 系統會每季取用交易資料和訂用帳戶資料，以優化模型。  Machine Learning 會使用 win/遺失資料來調整演算法，並藉由比較叢集建議與在 MSX 中處理的商機，來驗證模型是否如預期般運作。

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 機器學習的螢幕擷取畫面。":::

## <a name="cloudascent-propensity"></a>CloudAscent 傾向

如何建立傾向建議？

使用透過 web 編目程式所收集的信號和來自各種來源的資料，我們會合並 firmographics 資料和客戶的社交媒體信號。  評分會在比較模型中使用這些信號和資料，以配合意圖的模型並進行評分。

1. 符合客戶帳戶

   - 定義 firmographics 的內部和外部資料點。

   - [符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。

   - 每季更新評分比例

2. 客戶帳戶意圖

   - 社交媒體和客戶的線上行為定義意圖的相關信號。

   - 意圖評分會重迭在適合定義叢集的最上層。

   - 意圖評分會每月更新。

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 預測模型。":::

3. 叢集

   符合和意圖的信號會合並成群集分數。 CloudAscent 有四個群集：

      - 立即行動-銷售就緒客戶
      - 評估-行銷就緒的客戶
      - 培養-磁片磁碟機認知活動
      - 教育教育和監視意圖

   群集可讓使用者根據區段因素（例如：產品、地理、產業和垂直），以特定客戶的銷售和行銷計畫為目標。

   CloudAscent 活頁簿中的 [ **傾向模型** ] 索引標籤會共用傾向和預估的空白字元收入。 若要定義符合和意圖的叢集，請執行下列步驟：

      1. 使用 ML 模型時，我們會先計算規模為100的客戶符合分數和意圖分數。  確切分數會根據 ML 模型而有所不同。  下列範例分數：

         |**分類**|**分數**|
         |---------|:---------|
         |高|75-100|
         |中|55-74|
         |低|30 - 54|
         |非常低|0 - 29|

      2. 使用上述規則，我們會將企業分類為高、中、低，並在客戶的配合和意圖信號之間非常低。

      3. 我們會將每個代表傾向的交集，繪製在2D 矩陣上的客戶擬合和意圖信號。     例如，高尺寸 + 高意圖 = A1，代表最高的傾向。

      4. 最後，這些區段會組成叢集。  例如，A1、A2、A3、A4 形成「立即行動」叢集。

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent 模型。":::

   針對這些客戶，建議您將目標設為「立即行動」並評估客戶。

## <a name="cloudascent-products--models"></a>CloudAscent 產品 & 模型

下圖提供 CloudAscent 內每個傾向模型的觀點：

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向模型。":::

空白模型是由現有 Microsoft 客戶的預測所組成，其中沒有產品及/或是新的潛在客戶。

追加銷售模型會使用交易資料來預測 Azure 和 M365 Sku 中的追加銷售潛力。

EOS 共用 Win 7、Office 2010、SQL Server 和 Windows Server 的服務客戶結束。 使用 CloudAscent 傾向模型時，會從 MS Sales 提取 EOS 資料並與之重迭。 EOS 資料存留在新式工作和 Azure 銷售的生活中。
