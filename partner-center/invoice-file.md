---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389836"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| 欄位 | 定義 |
| ----- | ---------- |
| 美國 FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| 客戶號碼 | 您的客戶號碼。 |
| 帳單地址 | 我們可寄送發票給您的收件地址。 You can change your company name and/or address in your Partner Center billing profile. |
| 授權型費用 | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| 用量型費用 | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| 折扣 | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| 點數 | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| 小計 | 稅前總計以及稅收專屬費用和點數。 |
| 稅 | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| 其他點數 | 稅收專屬點數。 |
| 目前總費用 | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| 付款指示 | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| 發票號碼 | 發票的號碼。 |
| 計費期間 | The monthly period leading up to the invoice date. This is the period during which usage-based services are consumed and license-based services are reconciled for any credit adjustments or changes in license count. |
| 發票日期 | The billing date or anniversary date on which your invoice is generated each month. |
| 付款期限 | The payment term. 對於一次性購買，這一律是 60 天。 |
| 付款截止日期 | The date by which your payment must be received. |
| 客戶採購單 | Your purchase number order. |
| 客戶服務 | The website address where you can access customer service. |
| 服務收件者 | The address where the service is being used. (This is the legal company address associated with company vetting.) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| 欄位 | 定義 |
| ----- | ---------- |
| 日期 | 購買日期。 |
| 說明 | 產品名稱。 |
| 數量 | The number of products (such as reservations) purchased. |
| 單價 | Price per product (such as a reservation). |
| 折扣 | 適用的任何折扣。 |
| 稅前金額 | 稅前購買小計。 |
| 營業稅 | 稅額。 |
| 總計 | Total amount to be paid. |
