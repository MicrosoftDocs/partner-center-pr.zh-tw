---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389806"
---
# <a name="understand-charge-types"></a>Understand charge types

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file. Your invoice provides a summary of charges. Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types. For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).

Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).

> [!NOTE]
> One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.

## <a name="map-charge-types-to-invoice-charges"></a>Map charge types to invoice charges

To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel. Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.

## <a name="license-based-charges"></a>授權型費用

To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| 啟用費用 | The amount charged to the customer when they use the subscription after purchase. |
| 取消費用 | Prorated charges refunded to the customer when associated seats are changed. |
| 循環費用 | Periodic charges for a subscription. |
| 循環執行個體 (依比例計算) | Prorated charges assessed from the customer when associated seats are changed. |
| 取消時按比例計算費用 | Prorated refund for unused portion of service upon cancellation. |
| 購買時按比例計算之費用 | The charge type for a subscription when using annual billing. |
| 購買費用 | The charge type for a subscription when using monthly billing. |
| 續約時按比例計算費用 | Prorated fees upon subscription renewal. |
| 續約費用 | 訂閱續約時的費用 |
| 啟用時按比例計算費用 | >Prorated fees from activation until end of billing period. |

## <a name="one-time-charges"></a>One-time charges

To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| 新的 | Used when a new purchase is created. |
| addQuantity | Used in both the refund of the original purchase and the new quantity after an increase. |
| removeQuantity | Used in both the refund of the original purchase and the new quantity after a decrease. |
| [取消] | Used when a subscription is cancelled. |
| 轉換 | Used when a license is upgraded but the number of seats remains unchanged. |

## <a name="usage-charges"></a>使用量費用

To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| 取消時的存取用量費用 | Access usage fee upon cancellation for unpaid usage during the current billing period. |
| 目前週期的存取用量費用 | Access usage fee for the current billing period. |

### <a name="credits"></a>點數

To map these credits to your invoice:

- Sum the **TotalForCustomer** from the license-based file.
- Sum the **PostTaxTotal** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| 明細項目位移 | Partial or whole refund to a line item, including taxes. |

### <a name="usage-based-discounts"></a>用量型折扣

To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.

| Charge description (ChargeType column in reconciliation file) | Charge explanation |
| ------------------------------------------------------------- | ------------------ |
| 啟用折扣 | Discount applied when subscription activated. |
| 循環折扣 | Discount applied on periodic charges. |
| 續約折扣 | Discount applied when subscription renewed. |
| 取消折扣 | Charges applied when discounts cancelled. |

### <a name="license-based-discounts"></a>授權型折扣

To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.

*License-based discounts may be applied to multiple charge types.*
