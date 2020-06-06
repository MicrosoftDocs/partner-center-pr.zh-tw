---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在合作夥伴中心與您的 Salesforce CRM 同步處理您的參考
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 2e2cbe4b6f5418cea4d992b9e68daa7e0ed3ec09
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453255"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM 的共同銷售連接器 – 概觀

### <a name="appropriate-roles"></a>適當的角色

- 推薦管理員
- CRM 上的系統管理員或系統自訂者

合作夥伴中心共同銷售連接器可讓您的銷售人員從您的 CRM 系統內與 Microsoft 共同合作。 他們不需要經過訓練，就能使用合作夥伴中心來管理共同銷售交易。 使用共同銷售連接器，您可以建立新的共同銷售參照來與 Microsoft 賣方互動、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料，例如交易價值和結束日期。  您也可以在這些共同銷售交易上，收到 Microsoft 賣方的任何更新。 在您選擇的 CRM 中工作時（而不是在合作夥伴中心），您可以執行所有的參考工作。 

解決方案是以 Microsoft 電源自動化解決方案為基礎，並使用合作夥伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安裝之前的必要條件

|**主題**   |**詳細資料**   |**連結**   |
|--------------|--------------------|------|
|Microsoft 合作夥伴網路識別碼 |您需要有效的 MPN 識別碼|加入[MPN](https://partner.microsoft.com/)|
|共同銷售準備就緒|您的 IP/服務解決方案必須共同銷售。|[與 Microsoft 一起銷售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作夥伴中心帳戶|與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您的共同銷售解決方案相關聯的 MPN 識別碼相同。 在部署連接器之前，請確認您可以在合作夥伴中心入口網站中看到您的共同銷售參照。|[管理您的帳戶](create-user-accounts-and-set-permissions.md)|
|合作夥伴中心使用者角色|將安裝和使用連接器的員工必須是推薦管理員|[指派使用者角色和權限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 使用者角色是系統管理員或系統自訂者|[在 Salesforce CRM 中指派角色](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Power 自動化 Flow 帳戶|適用于 CRM 系統管理員或系統自訂者的主動式[電源自動化](https://flow.microsoft.com)帳戶。 該使用者應該在安裝之前至少登入一次[電源](https://flow.microsoft.com)。|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>安裝 Salesforce CRM 的合作夥伴中心推薦同步處理

1. 移至 [[電源自動化](https://flow.microsoft.com)]，並選取右上角的 [**環境**]。 這會顯示可用的 CRM 實例。

2. 從右上角的下拉式選單中，選取適當的 CRM 實例。

3. 選取左側導覽列上的 [**方案**]。

4. 按一下上方功能表上的 [**開啟 AppSource** ] 連結。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. 在彈出畫面中搜尋**Salesforce 的合作夥伴中心參照連接器**。  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. 按一下 [**立即取得**] 按鈕，然後按 [**繼續**]。

7. 這會開啟頁面，您可以在其中選取要安裝應用程式的 Salesforce CRM 環境。  同意條款及條件。

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="可用的 CRM":::

8. 接著，您會被導向至 [**管理您的解決方案**] 頁面。  使用頁面底部的箭號按鈕，流覽至 [合作夥伴中心的參考]。 已**排程的安裝**應該會出現在合作夥伴中心的 [參考解決方案] 旁。 安裝需要10-15 分鐘的時間。

9. 安裝完成後，流覽回到 [[電源自動化](https://flow.microsoft.com)]，然後從左側導覽區域選取 [**解決方案**]。 請注意，解決方案清單中提供**Salesforce 的合作夥伴中心參照同步**處理。

10. 選取**Salesforce 的 [合作夥伴中心參考同步**處理]。 下列電源可自動執行流程和實體：

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Salesforce 流程":::

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在您上線之前進行測試

在您安裝、設定及自訂生產環境的電源自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。

- 在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。

- 建立解決方案的複本，並執行您的設定，並在預備環境中自動執行流程自訂。

- 在預備/CRM 實例上測試解決方案。

- 成功時，將匯入為生產實例的受控解決方案。

## <a name="configure-the-solution"></a>設定解決方案

1. 在您的 CRM 實例中安裝解決方案之後，請流覽回到 [[電源自動化](https://flow.microsoft.com/)]。

2. 從右上角的 [**環境**] 下拉式選，選取您已安裝電源自動化解決方案的 CRM 實例。

3. 您將需要建立與三個使用者帳戶建立關聯的連接：

   - 具有參考系統管理員認證的合作夥伴中心使用者
   - 合作夥伴中心事件
   - CRM 系統管理員，具備在解決方案中自動化流程的能力。

   1. 從左側導覽列選取 [連線]，**然後從清單**中選取 [合作夥伴中心參照] 解決方案。

   2. 按一下 [**建立連接**] 來建立連線。

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="建立連線":::

   3. 在右上角的搜尋列中搜尋**合作夥伴中心參照（預覽）** 。

   4. 使用 [參考管理員] 的認證角色建立合作夥伴中心使用者的連線。

   5. 接下來，使用 [參考管理員] 的認證為合作夥伴中心使用者建立合作夥伴中心的事件連線。

   6. 為 CRM 系統管理員使用者建立 Common Data Service （目前的環境）的連接。

4. 若要讓電源自動化流程與連線產生關聯，請編輯每個電源自動化流程，以連線至 Common Data Service 和合作夥伴中心的參照。 儲存變更。

5. **開啟**電源自動化流程。

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook Api 註冊資源變更事件

合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。 這些變更事件會當做 HTTP post 傳送至您的 url。

1. 若要註冊您的 url，請選取 **[合作夥伴中心 Webhook 註冊（Insider preview）** 電源自動化流程]。

2. 新增（a）的連接。具有參照系統管理員認證的合作夥伴中心使用者（b.）以下反白顯示合作夥伴中心事件

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. 當您進行這些更新時，您會看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 儲存您的變更，然後選取 [**開啟**]。

   若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：

5. 選取 **[合作夥伴中心至 SALESFORCE CRM （Insider preview）**]。

6. 選取 [**編輯**] 圖示，然後選取 [**收到 HTTP 要求時**]。

7. 選取**複製**圖示以複製提供的 HTTP POST URL。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="複製 URL":::

8. 現在選取 [合作夥伴中心 Webhook 註冊（Insider Preview）] 電源自動化流程，然後選取 [**執行**]。

9. 確定 [執行流程] 視窗在右側窗格中開啟，然後按一下 [**繼續**]。

10. 輸入下列詳細資料：

    1. **Http 觸發程式端點**：從先前步驟複製的 URL

    2. **要註冊的事件**：「參考建立」和「參考更新」

    3. **覆寫現有的觸發程式端點（如果有的話**）：是（這會覆寫任何現有的端點）。

11. 選取 [**執行**]，然後選取 [**完成]。**

Webhook 現在可以接聽建立和更新事件。

## <a name="customize-synchronization-steps"></a>自訂同步處理步驟

在合作夥伴中心與您的 CRM 系統之間同步共同銷售參照時，會在此列出合作夥伴中心電腦上同步處理的欄位。

通常 CRM 系統是高度自訂的。 您可以自訂電源自動化流程。 遵循欄位對應指南，如有必要，請在電源自動化流程的步驟中進行適當的變更。  系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。

每個電源自動化流程的多個步驟可以根據您的需求自訂。 以下是可用自訂的範例：

1. 若要在合作夥伴中心內自訂建立或更新事件的欄位以進行 CRM 參考同步處理：

   1. 選取 [合作夥伴中心至 Salesforce CRM （Insider Preview）]。

   2. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   3. 選取 **[（範圍）]，同步處理潛在客戶或商機**。

2. 若要自訂建立事件的 CRM 欄位對應，請選取 [**如果是新的共用機會]，然後**。 **如果是**，請選取子步驟，然後**在 CRM 中展開 [建立新商機**]。 您可以使用欄位對應指南來編輯本節中的對應。

   1. 若要自訂更新事件的 CRM 欄位對應，請按一下步驟「（範圍）同步處理潛在客戶或商機」。

   2. **如果它是商機的更新，請選取此**方式。 **若為 [是]** ，請選取 [子步驟]，然後展開 **[合作夥伴中心與 CRM 中的商機物件之間的差異**]。  

   3. 選取 **[如果是]** ，然後按一下 [**更新現有商機**]

3. 若要針對 update 事件自訂 CRM 至電腦參照同步處理的欄位：

   1. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   2. 選取 **[（範圍）] 以同步處理商機**。

   3. 針對 [更新事件] 的自訂 CRM 欄位對應（根據欄位對應指南），選取 **[合作夥伴中心和 CRM 中的潛在客戶] 物件之間是否有差異，然後**。

   4. 選取子步驟（**如果是**），然後展開 [**以商機資料更新參考**] 步驟。

   您可以根據欄位對應指南，編輯本節中的對應。

4. 若要針對建立事件自訂 CRM 至電腦參照同步處理的欄位嗎？

   1. 選取 [**編輯**] 以編輯/自訂電源自動化流程。

   2. 選取 **[同步處理參考] （範圍）。**

   3. 如需自訂建立事件的 CRM 欄位對應（根據欄位對應指南），請選取 [**建立 Microsoft 參考**]。

您可以根據欄位對應指南，編輯本節中的對應。

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>在 Salesforce CRM 商機版面配置中建立個別的區段

若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，電源自動化解決方案必須清楚地區分 Microsoft 特定的參考欄位。 這讓您的賣方小組能夠決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。

一組自訂欄位可作為 Salesforce CRM**商機**實體的合作夥伴中心參考同步處理的一部分。 CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。
Salesforce CRM 系統管理員使用者將需要建立個別的 CRM 區段。

下列自訂欄位應為 CRM 區段的一部分：

- **與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機

- **參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位

- **參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結

- **Microsoft 如何提供協助？** Microsoft 針對此參考所需的協助

- **產品**：與此商機相關聯的產品清單

- **Audit**：與 Microsoft 合作夥伴中心參考同步的唯讀審核記錄

### <a name="set-up-fields-and-relationships"></a>設定欄位和關聯性

1. 登入您的 Salesforce 帳戶，並移至 [**商機**]。

2. 按一下 [**設定**] 和 [**編輯物件**] 選項，以加入必要的欄位。

3. 從左側導覽中選取**欄位 & 關聯**性

   :::image type="content" source="images/salesforce/fields1.png" alt-text="欄位":::

4. 在 [**欄位 & 關聯**性] 資料表中新增下欄欄位：

   |**欄位標籤**   |**欄位名稱**|**Data type**|**編制**|
   |---------------------|:-------------------|:--------------|:----------------|
   |稽核|  Audit__c|長文字區域（100000）（顯示行4）||
   |Microsoft 如何提供協助？|H ow_can_Microsoft_help__c|清單|
   |產品|產品-c|文字（255）||
   |轉介 |  Referral_Identi fier__c|文字（100）（外部識別碼）|是|
   |參考連結|   Referral_Link__c_|URL （255）||
   |與合作夥伴的 & 同步|同步處理-合作夥伴-中心-c|核取方塊（預設為未核取）||

   * 挑選清單值：

   - 工作負載特定價值主張
   - 客戶技術架構
   - 概念證明或示範
   - 報價或授權
   - 將銷售客戶成功後置
   - 一般或其他

5. 欄位會在 [欄位] **& [關聯**性] 底下建立

   :::image type="content" source="images/salesforce/fields2.png" alt-text="建立的欄位":::

6. 在 [商機配置] 中，以上欄欄位建立個別的區段。

   - 此章節應適用于商機配置中的銷售人員

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="合作夥伴中心欄位版面配置":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端對端雙向共同銷售參考同步處理

當您安裝、設定並自訂電源自動化解決方案之後，您可以測試 Salesforce CRM 和合作夥伴中心之間的共同銷售參考同步處理。

### <a name="pre-requisites"></a>必要條件

若要同步處理合作夥伴中心和 Salesforce CRM 之間的參考，電源自動化解決方案必須清楚地區分 Microsoft 特定的參考欄位。 此識別可讓您的賣方小組決定他們想要與 Microsoft 共用哪些參照，以進行共同銷售。

一組自訂欄位可作為 Salesforce CRM 解決方案**商機**實體的合作夥伴中心參考同步處理的一部分。 CRM 系統管理員使用者必須建立具有**商機**自訂欄位的個別 crm 區段。

下列自訂欄位應為 CRM 區段的一部分：

- **與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機

- **參考識別碼**： Microsoft 合作夥伴中心參照的唯讀識別碼欄位

- **參考連結**： Microsoft 合作夥伴中心中的參考的唯讀連結

- **Microsoft 說明如何**： microsoft 針對此參考所需的協助

- **產品**：與此商機相關聯的產品清單

- **Audit**：與合作夥伴中心參考同步的唯讀審核記錄

### <a name="scenarios"></a>場景

1. 在 CRM 中建立或更新參照並在合作夥伴中心同步處理時的參考同步處理：

   1. 以在 CRM 的 [**商機**] 區段中可見的使用者身分，登入您的 Salesforce CRM 環境。

   2. 當您在 Salesforce CRM 環境中建立「新商機」時，請確定下列區段存在

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. 若要與 Microsoft 合作夥伴中心同步處理此機會，請確定您已在卡片視圖中設定下欄欄位：

       - 「與合作夥伴中心同步」：是
       - 「Microsoft 如何協助？」：從下列選項中選取：
       - 產品：產品的解決方案識別碼

   4. 將 [商機**與合作夥伴中心同步**] 選項設定為 **[是]** 之後，請等候10分鐘，然後登入您的合作夥伴中心帳戶。 您的參考將與 Salesforce CRM 同步處理。

   5. 當 [與合作夥伴中心同步] 選項設定為 [是] 時，如果您更新 Salesforce CRM 中的機會，這些變更將會與您的合作夥伴中心帳戶同步處理。

   6. 與合作夥伴中心成功同步處理的機會，將會使用 Salesforce CRM 中的✔圖示來識別。

2. 在 Microsoft 合作夥伴中心內建立或更新參照時的參考同步處理，並在 Salesforce CRM 環境中同步處理：

    1. 登入您的合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/home)。

    2. 從左側功能表中選取 [**參考**]。

    3. 按一下 [新交易] 選項，從合作夥伴中心建立新的共同銷售參照。

    4. 登入您的 Salesforce CRM 環境。

    5. 流覽至 [**開啟商機**]。 在 Microsoft 合作夥伴中心建立的參考現在已在 Salesforce CRM 中同步處理。

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce 商機畫面":::

    6. 當您選取同步處理的參考時，會填入卡片視圖詳細資料。

## <a name="next-steps"></a>後續步驟

- [深入瞭解 Microsoft Power 自動化平臺？](https://docs.microsoft.com/-automate/)

- [管理潛在客戶](manage-leads.md)

- [管理共同銷售商機](manage-co-sell-opportunities.md)

- [合作夥伴中心 Webhook](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)