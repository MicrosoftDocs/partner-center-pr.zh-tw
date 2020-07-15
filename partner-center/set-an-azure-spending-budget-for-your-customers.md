---
title: 為客戶設定 Azure 消費預算
ms.topic: article
ms.date: 06/03/2020
description: 瞭解如何為您的客戶設定或移除每月的 Azure 費用預算，同時也可查看 Azure 費用資料並設定預算相關通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a52fa8d490ad43cc1e4f331b1a335004a07c83bd
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377732"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>在合作夥伴中心內設定、檢查或移除客戶的每月 Azure 費用預算

適用於︰

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

您可以在合作夥伴中心[為您的客戶設定每月的 Azure 費用預算](#set-azure-spending-budget)。 這可協助您的客戶管理其 Azure 費用。 此選項可讓您將客戶的 Azure 費用與當月的預算進行比較。 它也可協助您的客戶預算其 Azure 費用，使其每月帳單不會高於預期。

> [!NOTE]  
> 這項功能無法在沙箱中使用，或在生產（TIP）帳戶中測試。

[為客戶設定 Azure 消費預算](#set-azure-spending-budget)之後，您也可以透過下列方式來審查客戶的使用量。 這些選項可協助您找出設定錯誤的服務或可能會建議詐騙的異常趨勢。 接著，您可以與您的客戶合作，找出根本原因並管理成本。 如有必要，您也可以[將客戶的預算變更](#set-azure-spending-budget)為較高的金額。

- [檢查目前的 Azure 費用](#check-current-azure-spending)

- [當客戶的支出接近預算限制時，開啟電子郵件通知](#notifications-for-budget-limits)

- [依據依使用量的訂用帳戶，查看服務的明細成本](#itemized-costs-by-service)

您也可以隨時[移除客戶的 Azure 消費預算](#remove-azure-spending-budget)。

## <a name="azure-spending-data"></a>Azure 費用資料

Azure 消費資料是*估計值*，而*實際的計費金額可能會有所不同*。 資料的值*不會反映*可能適用的稅金、信用額度、調整或其他費用。

消費資料每天會重新整理*一次*。 除非您變更 Azure 入口網站中的帳戶設定，否則您的客戶可以繼續使用（並收取） Azure 服務和資源。

## <a name="set-azure-spending-budget"></a>設定 Azure 消費預算

您可以為合作夥伴中心內的多個客戶*設定每月 Azure 費用預算*：

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用**帳戶的客戶] 底下，選取您想要設定預算的客戶。

4. 輸入 [**每月預算**] 的值。

5. 選擇 **[** 套用] 以儲存變更。

您也可以在其訂用帳戶設定中*為個別客戶設定預算*：

1. 登入合作夥伴中心儀表板。

2. 在左側功能表中，選擇 [ **CSP**] 底下的 [**客戶**]。

3. 在 [**客戶**] 頁面上，選取客戶的**公司名稱**。

4. 在 [客戶的訂用帳戶 **] 頁面的**[**使用量型訂閱**] 底下，選擇 [**變更預算**]。

5. 輸入預算的值。

6. 選擇 **[** 套用] 以儲存變更。

## <a name="remove-azure-spending-budget"></a>移除 Azure 費用預算

您可以在合作夥伴中心移除客戶的*每月 Azure 費用預算*：

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用帳戶的客戶**] 底下，選取您想要移除其預算的客戶。

4. 選擇 [**移除預算**]。

## <a name="check-current-azure-spending"></a>檢查目前的 Azure 費用

您可以隨時*追蹤客戶目前的 Azure 支出和每月預算*：

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 消費**] 頁面的 [**具有 Microsoft Azure 訂用帳戶的客戶**] 底下，您可以看到客戶的每月預算、目前的支出預估和所用預算百分比的總覽。

## <a name="notifications-for-budget-limits"></a>預算限制的通知

當客戶的每月費用接近其預算限制時，您可以*開啟電子郵件通知*。 當您開啟此選項時，當客戶使用80% 或以上的每月預算時，系統會通知您。 此選項可協助您隨時留意 Azure 帳單。 若要設定電子郵件通知：

1. 登入合作夥伴中心。

2. 在左側功能表的 [ **CSP**] 底下，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 消費**] 頁面的 [**電子郵件通知**] 下，將 [**取得電子郵件**] 設定切換為 [**開啟**]。

4. 選擇 [**變更電子郵件地址**] 以查看通知的電子郵件地址。

5. 如果電子郵件地址*不正確*，請輸入正確的電子郵件地址，然後選擇 [**更新**]。 如果電子郵件地址*正確無誤*，請選擇 [**取消**]。

## <a name="itemized-costs-by-service"></a>依服務的明細成本

您可以*針對使用量型訂用帳戶，根據服務來查看明細成本（和預估使用量）*：

1. 登入合作夥伴中心。

2. 在左側功能表中，選擇 [ **CSP**] 底下的 [**客戶**]。

3. 在 [**客戶**] 頁面上，選取客戶的**公司名稱**。

4. 在 [客戶的**訂閱**] 頁面的 [**使用量型訂閱**] 底下，選取**訂**用帳戶的名稱。

5. 在訂用帳戶的頁面上，您可以查看服務的**明細成本**，以及當月的**預估使用量**。
