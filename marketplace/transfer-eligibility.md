---
title: 轉移資格-在計費帳戶之間傳輸訂用帳戶的指導方針，Azure Marketplace
description: 在 Azure 入口網站的計費帳戶之間轉移訂用帳戶之前的商業檢查指導方針。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007154"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>在計費帳戶之間轉移訂用帳戶的資格

您可以在 Azure 入口網站的計費區段中，將 [訂用](/azure/cost-management-billing/understand/subscription-transfer) 帳戶從一個計費帳戶轉移到另一個帳單帳戶。 在傳輸之前，會掃描訂用帳戶中的協力廠商產品。 只有在 *所有* 產品都已清除以進行傳輸時，才允許傳輸 (請參閱下面的 [準則](#criteria-for-transfer-approval-or-denial)) 。 系統會為無法清除的應用程式產生相關的錯誤訊息，以協助您判斷後續步驟。

> [!NOTE]
> 本文不適用於 SaaS 供應專案，因為 SaaS 資源會附加至租使用者，而不是訂用帳戶。 SaaS 資源可以從一個計費帳戶轉移到另一個計費帳戶，但這是依資源和依 Azure 支援的支援要求來完成。

## <a name="criteria-for-transfer-approval-or-denial"></a>傳輸核准或拒絕的準則

如果任何協力廠商應用程式符合下列任何一個條件，您就無法轉移訂用帳戶：

- 目標帳戶是商業的，且應用程式會退出宣告以透過合作夥伴銷售。
- 應用程式為選取的夥伴加入，且目標帳戶不在允許清單中。
- 這項供應專案是過去針對所選訂用帳戶的預覽供應專案，也是私人供應專案，且訂用帳戶已不再位於允許清單中。
- 新的計費帳戶位於與供應專案銷售位置不同的區域，而供應專案則不會在該區域中銷售。

封鎖的傳輸會維持有效，直到您從訂用帳戶中移除資源為止，之後您可以再次嘗試傳送。

## <a name="next-steps"></a>下一步

[取得 Microsoft AppSource 和 Azure Marketplace 的支援](get-support.md)

