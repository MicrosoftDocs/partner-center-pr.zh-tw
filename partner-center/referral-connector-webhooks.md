---
title: 使用 Webhook 取得資源變更事件
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作夥伴中心 Webhook Api 來瞭解 Dynamics 365 CRM 或 Salesforce CRM 何時會發生參考的資源變更。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2335c06d9c410d44ed5f444574d9bc8fb3e48fc0
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434017"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a>使用 Webhook Api 來註冊 Dynamics 365 CRM 和 Salesforce CRM 的資源變更事件

### <a name="appropriate-roles"></a>適當的角色

- 推薦管理員
- Dynamics 365 CRM 或 Salesforce CRM 的系統管理員或系統自訂者

合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。 這些變更事件會當做 HTTP post 傳送至您的 url。

>[!NOTE]
>本主題說明 Dynamics 365 CRM 和 Salesforce CRM 的 Webhook Api。

## <a name="configure-the-webhook"></a>設定 Webhook

1. 若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。

2. 新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. 當您進行這些更新時，您會看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 儲存您的變更，然後選取 [**開啟**]。

   若要讓合作夥伴中心 webhook 接聽合作夥伴中心和 CRM 系統中 IP 共同銷售/獨立參考物件的事件變更，請執行下列步驟：

5. 選取 [**合作夥伴中心] 至 [Dynamics 365 （Insider preview）** ] 或 **[合作夥伴中心] 至 [Salesforce （insider preview）**]。

6. 選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。

7. 選取**複製**圖示以複製提供的 HTTP POST URL。

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="複製 URL":::

8. 現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。

9. 確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。

10. 輸入下列詳細資料：

    1. **Http 觸發程式端點**：從先前步驟複製的 URL

    2. **要註冊的事件**：「參考建立」和「參考更新」

    3. **覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。

    Webhook 現在可以接聽變更（建立和更新事件）。

11. 選取 [**執行**]，然後選取 [**完成]。**

## <a name="customize-synchronization-steps"></a>自訂同步處理步驟

在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。

通常 CRM 系統是高度自訂的。 您可以自訂電源自動化流程。 遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。  系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。

每個電源自動化流程的多個步驟可以根據您的需求自訂。 以下是可用自訂的範例：

1. 若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：

   1. 選取 [合作夥伴中心] 至 [Dynamics 365 （Insider Preview）] 或 [合作夥伴中心] 至 [Salesforce （Insider Preview）]。

   2. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   3. 選取 **[（範圍）]，同步處理潛在客戶或商機**。

2. 若要自訂 [建立事件] 的 CRM 欄位對應（根據欄位對應指南），請選取 [**如果是新的共用機會]，然後**。 **如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。 您可以使用欄位對應指南來編輯本節中的對應。

   1. 如需自訂 update 事件的 CRM 欄位對應（根據欄位對應指南），請按一下「同步處理潛在客戶或商機」的步驟 [（範圍）]。

   2. **如果它是商機的更新，請選取此**方式。 **若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。  

   3. 選取 **[如果是]** ，然後按一下 [**更新現有商機**]

3. 若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：

   1. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   2. 選取 **[（範圍）] 以同步處理商機**。

   3. 針對 [更新事件] 的自訂 CRM 欄位對應（根據欄位對應指南），選取 **[合作夥伴中心和 CRM 中的潛在客戶] 物件之間是否有差異，然後**。

   4. 選取 [子步驟 **] （如果是**），然後展開 [**以商機資料更新參考**] 步驟。

   您可以根據欄位對應指南，編輯本節中的對應。

4. 若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？

   1. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   2. 選取 **[同步處理參考] （範圍）。**

   3. 如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。

您可以根據欄位對應指南，編輯本節中的對應。

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端對端雙向共同銷售參考同步處理

當您安裝、設定並自訂電源自動化解決方案之後，您可以測試 Dynamics 365 或 Salesforce 與合作夥伴中心之間的共同銷售參照同步處理。

### <a name="pre-requisites"></a>必要條件

若要在合作夥伴中心與 Dynamics 365 CRM 之間或跨合作夥伴中心和 Salesforce CRM 之間同步處理這些參考，電源自動化解決方案必須明確地區分 Microsoft 特定的參考欄位。 這讓您的賣方小組能夠決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。

一組自訂欄位可作為 Dynamics 365 解決方案**商機**實體的合作夥伴中心參考同步處理的一部分。 CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。

下列自訂欄位應為 CRM 區段的一部分：

- **與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機

- **參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位

- **參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結

- **Microsoft help？**： microsoft 針對此參考所需的協助

- **產品**：與此商機相關聯的產品清單

- **Audit**：與合作夥伴中心參考同步的唯讀審核記錄

### <a name="scenarios"></a>場景

1. 在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：

   1. 以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 DYNAMICS 365 CRM 環境。

   2. 當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="商機":::

   3. 若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：

      - **與合作夥伴中心同步**：是

      - **Microsoft help？**：請從下列專案中選取：

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="協助選取":::

      - **產品**：產品的解決方案識別碼

   4. 一旦在 Dynamics 365 中建立商機，並將 [**同步與合作夥伴中心**] 選項設定為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。 您的參考會與 Dynamics 365 進行同步處理。

   5. 因此，如果您有機會將「與合作夥伴中心同步」選項設定為「是」，則當您在 Dynamics 365 CRM 中更新商機時，變更將會在您的合作夥伴中心帳戶中同步處理。

   6. 與合作夥伴中心成功同步處理的機會，將會使用 Dynamics 365 中的✔圖示來識別。

2. 在 Microsoft 合作夥伴中心建立或更新參照時的參考同步處理，並在 Dynamics 365 環境中進行同步處理：

   1. 登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。

   2. 從左側功能表中選取 [**參考**]。

   3. 按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。

   4. 登入您的 Dynamics 365 CRM 環境。

   5. 流覽至 [**開啟商機**]。 在 Microsoft 合作夥伴中心建立的參考現在已在 Dynamics 365 CRM 中同步處理。

   6. 當您選取同步處理的參考時，會填入卡片視圖詳細資料。

## <a name="next-steps"></a>後續步驟

- [深入瞭解 Microsoft Power 自動化平臺？](https://docs.microsoft.com/power-automate/)

- [合作夥伴中心 webhook 事件](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [管理潛在客戶](manage-leads.md)

- [管理共同銷售商機](manage-co-sell-opportunities.md)
