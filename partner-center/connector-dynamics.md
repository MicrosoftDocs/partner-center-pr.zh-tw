---
title: Dynamics 365 CRM 的共同銷售連接器合作夥伴中心
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 將合作夥伴中心中的推薦與 Dynamics 365 CRM 的共同銷售連接器同步處理。 然後，銷售人員可以從您的 CRM 系統內與 Microsoft 共同銷售。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947738"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM 的共同銷售連接器–總覽

### <a name="appropriate-roles"></a>適當的角色

- 推薦管理員
- CRM 上的系統管理員或系統自訂員

合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。 他們不需要訓練以使用合作夥伴中心來管理共同銷售交易。 使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。 您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。 您可以在您選擇的 CRM 中，而不是在合作夥伴中心中，執行所有的參考工作。 

解決方案是以 Microsoft Power Automate 解決方案為基礎，並使用合作夥伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安裝之前的先決條件

|**主題**   |**詳細資料**   |**連結**   |
|--------------|--------------------|------|
|Microsoft 合作夥伴網路識別碼 |您需要有效的 MPN 識別碼|加入 [MPN](https://partner.microsoft.com/)|
|共同銷售解決方案就緒|您的 IP/服務解決方案必須已準備好共同銷售。|[與 Microsoft 銷售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作夥伴中心帳戶|與合作夥伴中心租使用者相關聯的 MPN 識別碼必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。 先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。|[管理您的帳戶](create-user-accounts-and-set-permissions.md)|
|合作夥伴中心使用者角色|將安裝並使用連接器的員工必須是推薦系統管理員|[指派使用者角色和權限](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|CRM 使用者角色是系統管理員或系統自訂員|[在 Dynamics 365 中指派角色](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate Flow 帳戶|適用于 CRM 系統管理員或系統自訂員的 active [Power Automate](https://flow.microsoft.com) 帳戶。 在安裝之前，該使用者至少應登入 [Power Automate](https://flow.microsoft.com) 一次。|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>為 Dynamics 365 (Power Automate 解決方案) 安裝合作夥伴中心的推薦同步處理

1. 移至 [Power Automate](https://flow.microsoft.com) ，然後在右上角選取 [ **環境** ]。 此步驟會顯示可用的 CRM 實例。

2. 從右上角的下拉式清單中選取適當的 CRM 實例。

3. 選取左側導覽列上的 [ **方案** ]。

4. 按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. 在快顯視窗中搜尋 **合作夥伴中心的 Dynamics365 參考連接器以進行** 。  

6. 按一下 [ **立即取得** ] 按鈕，然後 **繼續** 進行。

7. 這會開啟頁面，您可以在其中選取 CRM (Dynamics 365) 環境以安裝應用程式。  同意條款及條件。

8. 然後，系統會將您導向至 [ **管理您的解決方案** ] 頁面。  使用頁面底部的箭號按鈕，流覽至「合作夥伴中心的推薦」。 已 **排程的安裝** 應該會出現在合作夥伴中心的推薦解決方案旁邊。 安裝將需要10-15 分鐘的時間。 

9. 安裝完成之後，請流覽回到 [Power Automate](https://flow.microsoft.com) ，然後從左側導覽區域選取 **解決方案** 。 請注意，您可以在 [方案] 清單中找到 **Dynamics 365 的合作夥伴中心推薦同步** 處理。

10. 選取 **合作夥伴中心 Dynamics 365 的推薦同步** 處理。 以下是可用的流程和實體 Power Automate：

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用的 CRM":::

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：上線之前先進行測試

在生產環境中安裝、設定和自訂 Power Automate 解決方案之前，請務必在預備 CRM 實例上測試解決方案。

- 在預備環境/CRM 實例上安裝 Microsoft Power Automate 的解決方案。
- 製作解決方案的複本，並在預備環境中執行設定和 Power Automate 流程自訂。
- 測試預備/CRM 實例上的方案。 
- 成功時，請將受控解決方案匯入至生產環境實例。 

## <a name="configure-the-solution"></a>設定解決方案

1. 在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power Automate](https://flow.microsoft.com/)。


2. 從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power Automate 解決方案的 CRM 實例。

3. 您將需要建立與三個使用者帳戶建立關聯的連接：

   - 具有推薦系統管理員認證的合作夥伴中心使用者

   - 合作夥伴中心事件

   - CRM 管理員與解決方案中的 Power Automate 流程。

      1. 從左側導覽列選取 [ **連接** ]，然後從清單中選取 [合作夥伴中心的參考] 解決方案。

      2. 按一下 [ **建立連接**] 來建立連接。

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="建立連線":::

      3. 在右上角的搜尋列中搜尋 **合作夥伴中心參考 (預覽)** 。

      4. 使用「參考系統管理員」的認證角色建立合作夥伴中心使用者的連接。

      5. 接下來，使用推薦的系統管理員認證來為您的合作夥伴中心使用者建立合作夥伴中心事件連接。

      6. 為 CRM 系統管理員使用者建立 Common Data Service (目前環境) 的連接。
       
     
      7. 新增所有連線之後，您應該會在您的環境中看到下列連接：

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="連線":::
   
## <a name="edit-the-connections"></a>編輯連接

1. 返回 [ **方案** ] 頁面，然後選取 [ **預設方案**]。 按一下 [**全部**]，以選取 [ **(預覽) 的連接參考**。

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="[連接]":::

2. 選取三個點圖示，逐一編輯每一個連接。 新增相關的連接。

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="列出的連接"::: 

3.  依下列順序開啟流程：
- 合作夥伴中心 Webhook 註冊 (Insider Preview) 
- 建立共同銷售參考– Dynamics 365 至合作夥伴中心 (Insider Preview) 
- 合作夥伴中心 Microsoft 共同銷售參考更新至 Dynamics 365 (Insider preview) 
- 合作夥伴中心至 Dynamics 365 (Insider Preview) 
- Dynamics 365 至合作夥伴中心 (Insider Preview) 
- Dynamics 365 (Insider preview 的合作夥伴中心機會) 
- 可合作夥伴中心 (Insider Preview) 的 Dynamics 365 Microsoft 解決方案
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook Api 來註冊資源變更事件

合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。 這些變更事件會以 HTTP 文章的形式傳送至您的 url。

1. 若要註冊您的 url，請選取 **合作夥伴中心 Webhook 註冊 (Insider preview)** Power Automate flow。

2. 新增 (的連接。 ) 合作夥伴中心具有推薦的系統管理員認證的使用者 (b. ) 合作夥伴中心事件，如下所強調

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="觸發程序":::

3. 當您進行這些更新時，您會看到

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 儲存您的變更，然後選取 [ **開啟**]。

   若要讓合作夥伴中心 webhook 接聽事件變更，請執行下列步驟：

5. 選取 **合作夥伴中心至 Dynamics 365 (Insider preview)**。

6. 選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。

7. 選取 **複製** 圖示來複製提供的 HTTP POST URL。

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="複製 URL":::

8. 現在，選取 [合作夥伴中心 Webhook 註冊 (Insider Preview) ] Power Automate 流程，然後選取 [ **執行**]。

9. 確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。

10. 輸入下列詳細資料：

    1. **Http 觸發程式端點**：從先前步驟複製的 URL

    2. **要註冊的事件**：「參考建立」和「參考更新」

    3. **覆寫現有的觸發程式端點（如果有的話**）：是 (這會覆寫任何現有的端點。 ) 

11. 選取 [ **執行** ]，然後選取 [ **完成]。**

Webhook 現在可以接聽建立和更新事件。

## <a name="customize-synchronization-steps"></a>自訂同步處理步驟

當共同銷售的參考在合作夥伴中心與您的 CRM 系統之間進行同步處理時，在合作夥伴中心電腦上同步的欄位會列在此處。

通常會高度自訂 CRM 系統。 您可以自訂 Power Automate 流程。 依照欄位對應指南操作，如有必要，請在 Power Automate 流程的步驟中進行適當的變更。  系統會提供 Microsoft 合作夥伴中心對 CRM 的對應，但根據您的 CRM 環境，您可以選擇進一步自訂欄位。

您可以根據自己的需求自訂每個 Power Automate 流程的多個步驟。 以下是可用自訂的範例：

1. 若要自訂合作夥伴中心中的建立或更新事件的欄位以進行 CRM 推薦同步處理： 

    a. 選取合作夥伴中心至 Dynamics 365 (Insider preview) 或合作夥伴中心至 Salesforce (Insider preview) 。

    b. 選取 [ **編輯** ] 以編輯/自訂 Power Automate 流程。

    c. 選取 **(範圍) 同步處理潛在客戶或商機**。

2. 若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 **它是否為新的共用商機，然後**。 若為 [ **是]** ，請選取子步驟，然後 **在 CRM 中展開 [建立新商機**]。 您可以使用欄位對應指南來編輯本節中的對應。

    d. 若要根據 [更新事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請按一下 [ (範圍) 同步處理潛在客戶或商機] 步驟。

    e. **如果這是商機的更新，請選取它**。 **如果 [是]** ，請選取 [子步驟]，然後展開 [**合作夥伴中心和 CRM 中商機物件之間的差異]，然後再** 展開。  

    f. 選取 **[是]** ，然後選取 [**更新現有的商機**]

3. 若要自訂更新事件的 CRM 對電腦推薦同步處理的欄位：

    a. 選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。

    b. 選取 **(範圍) 同步處理商機**。

    c. 若要自訂 update 事件的 CRM 欄位對應，請選取 **合作夥伴中心和 CRM 中的潛在客戶物件之間是否有差異**。 

    d. **若為 [是]** ，請選取子步驟，然後展開 [**使用商機資料更新參考**] 步驟。

   您可以根據欄位對應指南編輯本節中的對應。

4. 針對建立事件自訂 CRM 對電腦推薦同步處理的欄位嗎？

   a. 選取 [ **編輯**  ] 以編輯/自訂 Power Automate 流程。

   b. 選取 **(範圍) 同步處理參考。**

   c. 若要根據 [建立事件] 的欄位對應指南) 自訂 CRM 欄位對應 (，請選取 [ **建立 Microsoft 參考**]。

   您可以根據欄位對應指南編輯本節中的對應。

已建立兩個環境變數：

- 核取記號：表示除了在合作夥伴中心與 Dynamics 365 CRM 之間雙向同步處理的商機之外，是否還需要核取記號圖示。

- 僅同步共同銷售商機：表示您是否只要同步處理共同銷售商機。

您可以選擇編輯環境變數的預設值。

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="預設值的編輯方塊":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>端對端雙向共同銷售推薦同步處理

安裝、設定和自訂 Power Automate 解決方案之後，您可以測試 Dynamics 365 和合作夥伴中心之間的共同銷售參照同步處理。

### <a name="pre-requisites"></a>必要條件

為了同步處理合作夥伴中心與 Dynamics 365 CRM 之間的參考，Power Automate 解決方案清楚標示 Microsoft 特定的參考欄位。 此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。

一組自訂欄位可作為 **商機** 實體的一部分。 CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。

下列自訂欄位應該是 CRM 區段的一部分：

- **與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步處理商機

- **參考識別碼**： Microsoft 合作夥伴中心推薦的唯讀識別碼欄位

- **參考連結**： Microsoft 合作夥伴中心中參考的唯讀連結

- **Microsoft 如何協助？**： microsoft 針對此推薦提供的協助

- **產品**：與此商機相關聯的產品清單

- **Audit**：使用合作夥伴中心參考進行同步處理的唯讀審核記錄

更新 Dynamics 365 CRM 中的商機表單，以包含 Products 欄位的解決方案。

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="商機表單":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{替代文字}":::

### <a name="scenarios"></a>場景：

1. 參考在 CRM 中建立或更新時的參考同步處理，並在合作夥伴中心中同步處理：

   1. 登入您的 Dynamics 365 CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。

   2. 當您在 Dynamics 365 環境中建立「新商機」時，請確定下列區段存在

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="顯示 Dynamics 365 中 Microsoft 合作夥伴中心資訊的 [範例商機] 區段。":::

   3. 若要與 Microsoft 合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：

      - **與合作夥伴中心同步**：是

      - **Microsoft 如何協助？**：請從下列專案進行選取：

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 中的 [範例商機] 區段，會顯示名為「Microsoft 如何協助」之欄位旁的 Microsoft 合作夥伴中心說明選項？":::

      - **產品**：產品的解決方案識別碼

   4. 一旦在 Dynamics 365 中建立商機，並將 [ **同步處理合作夥伴中心** ] 選項設為 **[是]**，請等候10分鐘，然後登入您的合作夥伴中心帳戶。 您的參考會與 Dynamics 365 進行同步處理。

   5. 同樣地，如果有 [同步處理合作夥伴中心] 選項設定為 [是] 的商機，如果您更新 Dynamics 365 CRM 的商機，這些變更將會在您的合作夥伴中心帳戶中同步處理。

   6. 使用合作夥伴中心成功同步處理的商機將會以 Dynamics 365 中的✔圖示來識別。

2. 在 Microsoft 合作夥伴中心中建立或更新參考時的參考同步處理，並在 Dynamics 365 環境中同步處理：

   1. 登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。

   2. 從左側功能表中選取 [ **參考** ]。

   3. 按一下 [新增交易] 選項，從合作夥伴中心建立新的共同銷售推薦。

   4. 登入您的 Dynamics 365 CRM 環境。

   5. 流覽至 **開啟的商機**。 在 Microsoft 合作夥伴中心中建立的參照現在已在 Dynamics 365 CRM 中同步處理。

   6. 當您選取同步處理的參考時，就會填入卡片視圖詳細資料。

## <a name="next-steps"></a>後續步驟

- [管理潛在客戶](manage-leads.md)

- [管理共同銷售商機](manage-co-sell-opportunities.md)

- [深入瞭解 Microsoft Power Automate platform？](/power-automate/)

- [合作夥伴中心 Webhook](/partner-center/develop/partner-center-webhooks)