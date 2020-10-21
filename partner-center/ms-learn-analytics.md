---
title: 合作夥伴中心見解 Microsoft Learn 分析
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 利用個別定型、完成的課程模組、完成的學習路徑等資料，來追蹤公司的學習人員。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 42c7af80ab49cee6e7043587207e553d2ffaa3ac
ms.sourcegitcommit: a7376c0ba8f4f3d01361bc227640311b486b3b6e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/21/2020
ms.locfileid: "92333810"
---
# <a name="the-microsoft-learn-analytics-report-shows-the-status-of-learners-in-your-company"></a>Microsoft Learn 分析報表會顯示您公司中的學習者狀態

**適當的角色**
-   全域系統管理員
-   MPN 合作夥伴系統管理員

Microsoft Learn 報表會提供您公司中的學習工具的相關資訊，包括已完成的模組，以及它們所在的學習路徑。 報表會顯示每個個別學習模組的狀態。 您公司的全域管理員和 MPN 管理員可以查看資料。

## <a name="how-to-read-the-report"></a>如何讀取報表

### <a name="summary-charts"></a>摘要圖表

這些圖表摘要說明已定型個人、模組完成和學習路徑的計數和每月累計趨勢。


**定型的個人計數**：已在選取的日期範圍內至少完成一個模組的所有不同學習者計數 

**定型的個人趨勢走勢圖**：使用中學習的每月月累計計數 

**模組完成計數**：在選取的日期範圍內，由合作夥伴公司的學習人員所完成的模組完成計數。
例如，如果 "Module 1" 是由15個人完成，而且 "Module 2" 是由相同的15個人完成，則模組完成計數將會是30。 模組完成日期應該落在選取的日期範圍內。

**模組完成趨勢走勢圖**：模組完成的月數累計計數 

**學習路徑完成計數**：在選取的日期範圍期間，合作夥伴公司中的學習程式完成學習路徑的計數。
例如，如果學習路徑 "Path 1" 是由20個人完成，而且學習路徑 "path 2" 已由相同20個人完成，則學習路徑完成計數將會是40。 學習路徑完成日期應該落在選取的日期範圍內。

**學習路徑完成趨勢走勢圖**：學習路徑完成的每月月累積計數 

### <a name="trained-individuals-monthly-trend"></a>定型的個人每月趨勢

這項資料是您公司的使用者在該月第一次完成課程模組的趨勢。 

**X 軸** 是所選時間篩選準則的月份。 

**Y 軸** 是使用中的學習者計數，已在該月) 註冊 (首次完成模組。 這不是累計的。

### <a name="module-completions-monthly-trend"></a>模組完成每月趨勢

這項資料是您所有公司的使用者在該月完成的模組趨勢。  (非累計)  

**X 軸** 是所選時間篩選準則的月份。 

**Y 軸** 是該月份的模組完成計數。 這不是累計的。

### <a name="learning-path-completions-monthly-trend"></a>學習路徑完成每月趨勢

這項資料是您公司的使用者在該月份完成學習路徑的趨勢。  (非累計)  

**X 軸** 是所選時間篩選準則的月份。 

**Y 軸** 是該月份中的模組完成計數。 這不是累計的。

### <a name="learning-path-completion-tabs"></a>學習路徑完成索引標籤 

**模組索引標籤**

此索引標籤包含您公司中依前5個模組名稱完成的模組細分;與模組相關聯的產品;以及與模組相關的使用者角色。  

- 模組完成環圈圖：模組名稱的明細) 摘要區段中顯示的「模組完成」 (計數。

圖表中央顯示的數位是完成的總模組

- 依角色的完成：依模組的角色完成模組的明細。 如果模組與多個角色相關聯，則會將每個角色新增至模組完成的計數。

圖表中央顯示的數位是模組完成的相異角色數目。 

- 依產品的完成：由模組所對應的產品完成模組完成的明細。 如果模組與多項產品相關聯，則會將每個產品新增至模組完成的計數。    

圖表中央顯示的數位是模組完成的相異產品數目。  

**學習路徑索引標籤**   

此索引標籤包含在您公司中依前5個模組名稱完成的學習路徑細目;學習路徑所對應的產品;以及與此學習路徑相關的角色。  

- 學習路徑完成環圈圖：學習路徑完成的明細：依名稱) 的摘要區段中顯示的「學習路徑完成」 (計數。

- 依角色的完成：依角色的學習路徑完成明細。 如果模組與多個角色相關聯，則會將每個角色新增至模組完成的計數。

- 依產品的完成：將學習路徑對應到的產品完成學習路徑的明細。 如果模組與多項產品相關聯，則會將每個產品新增至模組完成的計數。

### <a name="completions-by-learning-individuals"></a>學習個人的完成

這會列出您公司中已定型的使用者，以及其完成的模組與學習路徑的詳細資料。

Microsoft Learn 識別具有使用者物件識別碼的學習工具。 在 [ **模組]** 索引標籤下，所有學習工具都會依模組完成排序。 它們會顯示 Microsoft Learn 使用者名稱、物件識別碼和模組計數。 您可以使用使用者名稱進行搜尋。 

在 [ **學習路徑]** 索引標籤下，[完成學習路徑] 所排序的所有學習工具都會以學習模組顯示名稱、物件識別碼和模組計數來顯示。

若要使用使用者物件識別碼來取得學習模組的詳細資料： 

1. 登入 [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer )。  (您必須是公司 Azure AD 租使用者的全域管理員。 ) 

2. 將使用者物件識別碼複製到 [Graph Explorer] 中反 [白顯示的區域](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) 。 

## <a name="faq"></a>常見問題集

1. 我看不到我公司的學習詳細資料。

這份報告適用于在合作夥伴中心中具有帳戶的合作夥伴。 如果您仍在 Partner Membership Center 中，您將看不到這份報表。

2.  公司中的誰可以查看這份報表？ 

全域管理員和 MPN 管理員可以查看報表。

3. 如何確定所有的使用者都將他們的 Microsoft Learn 帳戶與其合作夥伴中心帳戶建立關聯？

全域系統管理員新增使用者之後，該使用者必須移至他們的 **我的設定檔** ，才能將其 Microsoft Learn 帳戶相關聯。

- 選取儀表板右上角的 **您的帳戶** 圖示，然後選取 [ **我的設定檔**]。 

-  在 **您的學習** 下，使用者將能夠建立其 Microsoft Learning 帳戶的關聯，並將其 Microsoft 帳戶連接到合作夥伴大學。

3. 我是否可以看到在此報表中使用 MSA 帳戶登入 Microsoft Learn 的所有公司使用者？

目前，執行這項作業的最佳方式是將這些使用者新增至您的 Azure AD 租使用者，並將其新增至合作夥伴中心，讓他們可以透過合作夥伴中心中的 **我的設定檔** 來建立其 Microsoft Learn 帳戶的關聯。 

對於僅使用其 MSA 帳戶進行訓練的使用者，在不久的未來，Microsoft Learn 團隊將可讓他們將其工作電子郵件與其 Microsoft Learn 設定檔產生關聯。 

## <a name="next-steps"></a>後續步驟

如需詳細報表，請參閱 [合作夥伴中心 Insights](partner-center-insights.md)。

>[!NOTE] 
> 您可以從 [見解] 儀表板的 [下載報告] 區段中，下載開啟此報表的原始資料。 [深入了解](pci-download-reports.md) 