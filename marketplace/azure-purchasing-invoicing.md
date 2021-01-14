---
title: 從 Azure Marketplace 購買軟體和解決方案
description: 瞭解在 Azure Marketplace 中簡化和簡化軟體購買與管理的工具。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 8f7962b1b040be90f7dc1b2696a2ced3830d25b9
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182472"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace 購買

Azure Marketplace 有許多工具和功能，可簡化和簡化購買原則的購買、發票和管理程式。

## <a name="simplified-procurement"></a>簡化的採購

Azure Marketplace 可透過不同的購買選項協助簡化採購程序。 如果您使用與您的 Azure 帳戶相關聯的信用卡來購買產品，則所有購買專案都會合並為單一發票並以選擇的信用卡計費。 如果您是大型客戶，可以使用 Enterprise 合約來購買。 使用 EA 時，任何軟體購買都會自動包含在您的 Azure 發票中。 發票將會先包含 Azure 使用量費用，之後才是 Azure Marketplace 費用。

當您透過 Azure Marketplace 購買時，您可以消除管理個別廠商關聯性和發票的複雜度。 您可以從 Microsoft 取得單一合併的每月帳單，其中包含您的 Azure Marketplace 購買和您的 Azure 費用。

## <a name="permission-to-purchase"></a>購買的許可權

找到正確的軟體應用程式之後，就可以輕鬆完成購買。 不過，您將需要 Azure 訂用帳戶內的適當許可權。 因為 Azure 會在 [角色型存取控制](/azure/role-based-access-control/overview) 上運作 (RBAC) 模型，所以您的帳戶需要訂用帳戶 **擁有** 者或 **參與者** 許可權才能進行購買。

完成購買之前，請確定使用者在 Azure 租使用者中具有正確的設定。 這將有助於防止在購買期間發生錯誤。

在 Azure 入口網站的 Azure Marketplace 體驗中，尋找您想要購買的應用程式，然後 **選取 [建立]** 或 [ **設定 + 訂閱**]。 系統會提示您先完成一些資訊，才能使用新的解決方案。

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="供應專案建立按鈕。":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="[設定 + 訂閱] 按鈕。":::

如果您想要從 Azure Marketplace online store 部署解決方案，請在 [產品描述] 頁面上選取 [ **立即取得** ]，然後使用您的 Azure 帳號憑證登入。

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Azure Marketplace 登入] 對話方塊。":::

登入後，系統會將您重新導向至 Azure 入口網站中的產品以完成購買。

## <a name="purchase-policy-management"></a>購買原則管理

Microsoft 可讓您以 Azure 訂用帳戶管理員的身分，使用帳單設定檔來管理使用者購買。 從三個選項中選擇：

- **免費 + 付費** –可讓使用者取得任何 Azure Marketplace 軟體應用程式。
- **免費** -可讓使用者只部署 Azure Marketplace 的免費軟體。
- **否** -防止使用者從 Azure Marketplace 部署任何軟體。

這些設定會套用至所有可存取您 Azure 訂用帳戶的使用者，讓您能夠透過 Azure 入口網站來控制其採購。

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="透過 Azure 入口網站控制 IT 採購":::

## <a name="cost-management"></a>成本管理

當您從 Azure Marketplace 購買產品時，您想要取得可協助您管理成本的見解。 Azure 成本管理是一項免費的工具，可供您用來查看您所購買之產品的相關資訊。 您可以使用成本管理來查看您要在一段時間內花費多少服務的詳細資料，以及這些成本如何針對您所設定的預算進行追蹤。 除了設定預算之外，您還可以排程報表並分析訂用帳戶成本。 藉由 [使用 Azure 成本管理來完成分析成本和建立預算](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)的 Microsoft Learn 課程模組，以深入瞭解 Azure 成本管理。

您可在 Azure 成本管理底下的成本分析工具上檢視 Azure Marketplace 費用及發票。

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="使用 Azure 成本管理可深入瞭解您購買的產品。":::

## <a name="next-steps"></a>後續步驟

- [計費與發票開立](billing-invoicing.md)