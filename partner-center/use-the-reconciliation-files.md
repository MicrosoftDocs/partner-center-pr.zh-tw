---
title: 使用您的對帳檔案
ms.topic: article
ms.date: 06/08/2020
description: 瞭解合作夥伴中心的對帳檔案，以及如何解讀特定計費週期的詳細、明細專案的費用觀點。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f52c0b3d53fde6d5b5f68c54f8967e26a33b8c76
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991772"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>瞭解如何讀取合作夥伴中心對帳檔案中的明細專案

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

您可以從合作夥伴中心下載您的對帳檔案，以取得計費週期中每個費用的詳細明細專案。 明細專案詳細資料包括每個客戶的訂用帳戶的費用，以及詳細的事件（例如，將基座加入訂用帳戶中）。

適當的角色：

- 帳單系統管理員
- 全域系統管理員

如需有關如何讀取**發票**的詳細資訊，請參閱[閱讀您的帳單](read-your-bill.md)。

## <a name="understand-reconciliation-file-fields"></a>瞭解對帳檔案欄位

- [以授權為基礎的對帳檔案欄位](license-based-recon-files.md)
- [基於使用方式的對帳檔案欄位](usage-based-recon-files.md)
- [一次性和週期性的對帳檔案欄位](one-time-recurring-recon-files.md)
- [每日評分的使用量對帳檔案欄位](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>瞭解對帳檔案中的收費類型

若要瞭解對帳檔案中的費用類型（ **ChargeType**資料行），請參閱[對帳檔案費用類型](recon-file-charge-types.md)。

## <a name="fix-formatting-issues"></a>修正格式問題

對帳檔案有時可能會包含格式問題。 例如，如果未使用 en-us 地區設定，則可能會發生此問題。

請遵循下列步驟來修正對帳檔案中的任何格式設定問題：

1. 在 Microsoft Excel 中開啟對帳檔案（格式為 .csv）。
2. 選取檔案中的第一個資料行。
3. 開啟 [**將文字轉換成資料行] Wizard**。 在功能區上，選取 [**資料**]，然後選取 [**文字到資料行**]。
4. 在嚮導中，選取 [**分隔檔案類型**]。 然後，選取 [下一步]。
5. 在 [**分隔符號**] 欄位中，選取 [**逗號**]。 （如果已選取索引標籤，您可以將此選項保留為 [已選取 **]** ）。然後選取 **[下一步]**。
6. 在 [**資料行資料格式**] 欄位中，選取 [**日期： MDY**]。 然後，選取 [下一步]。
7. 在 [**資料行資料格式**] 欄位中，針對 [所有數量] 資料行選取 [**文字**]。 然後，選取 [完成]。

## <a name="download-reconciliation-files-programmatically"></a>以程式設計方式下載對帳檔案

對帳檔案可能非常大，有時很難以下載。 若要以程式設計方式下載對帳檔案，請參閱[取得發票明細專案](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)。

## <a name="map-taxes-or-vat"></a>地圖稅額或 加值稅

若要將稅金或加值稅（加值稅）對應到您的發票：

- 加總以授權為基礎的檔案中的**稅務**資料行。
- 加總以使用方式為基礎之檔案中的**TaxAmount**資料行。

## <a name="itemize-reconciliation-files-by-partner"></a>依合作夥伴的逐條對帳檔案

**間接模型**中的合作夥伴可以在以授權為基礎和以使用量為基礎的對帳檔案中使用這些額外的欄位，以根據轉售商將檔案加上。

| MPN 識別碼 | 描述 |
| ------ | ----------- |
| MPN 識別碼 | 雲端解決方案提供者（CSP）合作夥伴（直接或間接）的 Microsoft 合作夥伴網路（MPN）識別碼。 |
| [經銷商 MPN 識別碼](#reseller-mpn-id) | 訂用帳戶[之記錄轉銷商的 MPN 識別碼](#reseller-mpn-id)。 此欄位對應至合作夥伴中心內的特定訂用帳戶所列的轉售商識別碼。 只會出現在間接模型合作夥伴的對帳檔案上。 |

### <a name="reseller-mpn-id"></a>經銷商 MPN 識別碼

如果 CSP 合作夥伴直接將訂用帳戶銷售給客戶，其**MPN 識別碼**會列出兩次，同時做為**MPN 識別碼**和**轉售商 MPN 識別碼**。

如果 CSP 合作夥伴具有沒有**MPN 識別碼**的轉銷商，此值會改為設定為合作夥伴的**MPN 識別碼**。

如果 CSP 合作夥伴移除**轉售商 MPN 識別碼**，此值將會設定為 *-1*。

若要查看或更新**轉售商 MPN 識別碼**：

1. 登入合作夥伴中心。
2. 在 [合作夥伴中心] 功能表中，選取 [**客戶**]。
3. 從清單中選擇客戶。
4. 在 [客戶] 功能表中，選取 [**訂閱**]。
5. 從清單中選擇訂用帳戶。
6. 選取 \[更新\]**** 以變更 \[經銷商 (MPN 識別碼)\]****。
