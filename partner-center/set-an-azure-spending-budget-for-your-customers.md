---
title: 為客戶設定 Azure 費用預算
ms.topic: how-to
ms.date: 06/03/2020
description: 瞭解如何為您的客戶設定或移除每月 Azure 費用預算，以及查看 Azure 費用資料並設定預算相關的通知。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438989"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>在合作夥伴中心中設定、檢查或移除客戶的每月 Azure 費用預算

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

您可以在合作夥伴中心中 [為您的客戶設定每月的 Azure 支出預算](#set-azure-spending-budget) 。 這可協助您的客戶管理其 Azure 費用。 此選項可讓您比較客戶的 Azure 費用與該月的預算。 它也可協助您的客戶為其 Azure 費用編制預算，讓其每月帳單不會高於預期。

> [!NOTE]  
> 這項功能不適用於沙箱或在生產環境中測試 (提示) 帳戶。

[為客戶 (的) 設定 Azure 費用預算](#set-azure-spending-budget)之後，您也可以透過下列方式來檢查客戶的使用方式。 這些選項可協助您找出設定錯誤的服務或可能會建議詐騙的不尋常趨勢。 然後，您可以與客戶 (的) ，以找出根本原因和管理成本。 如有必要，您也可以 [將客戶的預算變更](#set-azure-spending-budget) 為較高的金額。

- [檢查目前的 Azure 費用](#check-current-azure-spending)

- [當客戶的支出接近預算限制時，開啟電子郵件通知](#notifications-for-budget-limits)

- [依使用量的訂用帳戶來查看依服務區分的成本](#itemized-costs-by-service)

您也可以隨時移除客戶 () 的 [Azure 消費預算](#remove-azure-spending-budget) 。

## <a name="azure-spending-data"></a>Azure 費用資料

Azure 費用資料是 *估計值* ，而 *實際計費金額可能會有所不同*。 資料的值 *不會反映* 可能適用的稅金、信用額度、調整或其他費用。

消費資料每天重新整理 *一次*。 除非您在 Azure 入口網站中變更其帳戶設定，否則您的客戶可以繼續使用 (並向) 的 Azure 服務和資源收費。

## <a name="set-azure-spending-budget"></a>設定 Azure 費用預算

您可以在合作夥伴中心中為多個客戶 *設定每月 Azure 消費預算* ：

1. 登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 費用** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，選取您要設定預算的客戶 () 。

4. 輸入 **每月預算** 的值。

5. 選擇 [套用] 以儲存 **您的變更** 。

您也可以在訂用帳戶設定中 *設定個別客戶的預算* ：

1. 登入合作夥伴中心儀表板。

2. 在 [ **CSP**] 下的左側功能表中，選擇 [ **客戶**]。

3. 在 [ **客戶** ] 頁面上，選取客戶的 **公司名稱**。

4. 在 [客戶的訂用帳戶 **] 頁面的** [ **基於使用方式的訂** 用帳戶] 下，選擇 [ **變更預算**]

5. 輸入預算的值。

6. 選擇 [套用] 以儲存 **您的變更** 。

## <a name="remove-azure-spending-budget"></a>移除 Azure 費用預算

您可以在合作夥伴中心中移除客戶 () 的 *每月 Azure 費用預算* ：

1. 登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 費用** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，選取您要移除其預算的客戶 (s) 。

4. 選擇 [ **移除預算**]。

## <a name="check-current-azure-spending"></a>檢查目前的 Azure 費用

您可以隨時 *追蹤客戶目前的 Azure 費用和每月預算* ：

1. 登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/)。

2. 在 [ **CSP**] 下的左側功能表中，選擇 [ **Azure 費用**]。

3. 在 [ **Azure 消費** ] 頁面的 [ **具有 Microsoft Azure 訂用** 帳戶的客戶] 下，您可以看到客戶的每月預算、目前的費用預估，以及使用的預算百分比。

## <a name="notifications-for-budget-limits"></a>預算限制的通知

當客戶的每月費用接近預算限制時，您可以 *開啟電子郵件通知* 。 當您開啟此選項時，當客戶使用80% 或更多的每月預算時，系統會通知您。 此選項可協助您隨時留意 Azure 帳單。 若要設定電子郵件通知：

1. 登入合作夥伴中心。

2. 移至 [設定]  。

3. 選取 [ **我的喜好** 設定]。

4. 如果沒有，請設定慣用的電子郵件地址。

5. 設定通知的慣用語言。

6. [**通知喜好** 設定] 區段底下的 [選取 **CSP** ] 索引標籤

7. 檢查 **Azure 消費** 通知的電子郵件選項，並 **儲存**。


## <a name="itemized-costs-by-service"></a>依服務的詳細成本

您可以 *針對以使用量為基礎的訂用帳戶，查看服務的詳細成本 (和預估使用量)*：

1. 登入合作夥伴中心。

2. 在 [ **CSP**] 下的左側功能表中，選擇 [ **客戶**]。

3. 在 [ **客戶** ] 頁面上，選取客戶的 **公司名稱**。

4. 在 [客戶的訂用帳戶 **] 頁面的** [ **基於使用方式的訂閱**] 下，選取 **訂** 用帳戶的名稱。

5. 在訂用帳戶的頁面上，您可以依服務查看 **詳細的成本** ，以及當月的 **預估使用量** 。
