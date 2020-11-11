---
title: 使用您的對帳檔案
ms.topic: article
ms.date: 06/08/2020
description: 瞭解合作夥伴中心中的對帳檔案，以及如何針對指定的計費週期，解讀詳細的明細專案查看費用。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d09c1e57d16937c5656579f3932e9c8feb3ecf24
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/11/2020
ms.locfileid: "94488074"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>瞭解如何讀取您合作夥伴中心對帳檔案中的明細專案

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

您可以從合作夥伴中心下載您的對帳檔案，以取得計費週期中每個費用的詳細、明細專案視圖。 明細專案詳細資料包含每個客戶訂用帳戶的費用，以及詳細的事件 (例如，將授權新增至訂用帳戶) 。

適當的角色：

- 帳單系統管理員
- 全域系統管理員

如需有關如何讀取 **發票** 的詳細資訊，請參閱 [閱讀帳單](read-your-bill.md)。

## <a name="understand-reconciliation-file-fields"></a>瞭解對帳檔案欄位

- [以授權為基礎的對帳檔案欄位](license-based-recon-files.md)
- [以使用量為基礎的對帳檔案欄位](usage-based-recon-files.md)
- [每日評分的使用量對帳檔案欄位](daily-rated-usage-recon-files.md)
- [一次性購買 CSP 對帳檔案欄位](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>瞭解對帳檔案中的費用類型

若要瞭解對帳檔案中的費用類型 ( **ChargeType** 資料行) ，請參閱 [對帳檔案費用類型](recon-file-charge-types.md)。

## <a name="fix-formatting-issues"></a>修正格式化問題

有時，對帳檔案可能會包含格式化問題。 例如，如果未使用 en-us 地區設定，就可能發生此問題。

請遵循下列步驟來修正對帳檔案中的任何格式問題：

1. 在 Microsoft Excel 中，以 .csv 格式) 開啟對帳檔案 (。
2. 選取檔案中的第一個資料行。
3. 開啟 [ **將文字轉換成資料行] Wizard** 。 在功能區上，選取 [ **資料** ]，然後選取 [ **文字至資料行** ]。
4. 在嚮導中，選取 [ **分隔檔案類型** ]。 然後，選取 [下一步]。
5. 在 [ **分隔符號** ] 欄位中，選取 [ **逗號** ]。  (如果 **已** 選取索引標籤，您可以將此選項保留為已選取狀態。 ) 然後選取 **[下一步** ]。
6. 在 [ **資料行資料格式** ] 欄位中，選取 [ **日期： MDY** ]。 然後，選取 [下一步]。
7. 在 [ **資料行資料格式** ] 欄位中，選取 [所有數量] 資料行的 [ **文字** ]。 然後選取 [完成]。

## <a name="download-reconciliation-files-programmatically"></a>以程式設計方式下載對帳檔案

對帳檔案可能很大，有時很難下載。 若要以程式設計方式下載對帳檔案，請參閱 [取得發票明細專案](/partner-center/develop/get-invoiceline-items)。

## <a name="map-taxes-or-vat"></a>地圖稅或 加值稅

若要將稅金或加值稅 (加值稅) 對應至您的發票：

- 以授權為基礎的檔案加總 **稅額** 資料行。
- 加總以使用量為基礎之檔案中的 **TaxAmount** 資料行。

## <a name="itemize-reconciliation-files-by-partner"></a>依夥伴進行對帳檔案的匯總

**間接模型** 中的合作夥伴可以在以授權為基礎和以使用量為基礎的對帳檔案中使用這些額外欄位，以依轉銷商將檔案加上詳細資訊。

| MPN 識別碼 | 描述 |
| ------ | ----------- |
| MPN 識別碼 | Microsoft 合作夥伴網路 () MPN 雲端解決方案提供者 (的)  (直接或間接) 。 |
| [經銷商 MPN 識別碼](#reseller-mpn-id) | 訂用帳戶 [之記錄轉銷商的 MPN 識別碼](#reseller-mpn-id)。 此欄位會對應至合作夥伴中心中特定訂用帳戶所列出的轉售商識別碼。 只會出現在間接模型合作夥伴的對帳檔案上。 |

### <a name="reseller-mpn-id"></a>經銷商 MPN 識別碼

如果 CSP 合作夥伴將訂用帳戶直接銷售給客戶，則會將其 **MPN 識別碼** 列為 **MPN 識別碼** 和 **轉售商 MPN 識別碼** 兩次。

如果 CSP 合作夥伴的轉銷商沒有 **MPN 識別碼** ，此值會改為設定為夥伴的 **MPN 識別碼** 。

如果 CSP 合作夥伴移除 **轉售商 MPN 識別碼** ，此值會設定為 *-1* 。

若要查看或更新 **轉售商 MPN 識別碼** ：

1. 登入合作夥伴中心。
2. 在 [合作夥伴中心] 功能表中，選取 [ **客戶** ]。
3. 從清單中選擇客戶。
4. 在 [客戶] 功能表中，選取 [ **訂閱** ]。
5. 從清單中選擇訂用帳戶。
6. 選取 \[更新\] 以變更 \[經銷商 (MPN 識別碼)\]。