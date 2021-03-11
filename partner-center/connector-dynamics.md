---
title: Dynamics 365 CRM 合作夥伴中心的共同銷售連接器
description: 使用 Dynamics 365 CRM 的共同銷售連接器，同步處理合作夥伴中心內的推薦。 然後，銷售人員可以從您的 CRM 系統內與 Microsoft 共同銷售。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 1b0f8f12cf60db0dcc03aae24316e869cbf34376
ms.sourcegitcommit: d7fbaff51c7ac29fbf700d7f7fdef798fd97c6fa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "102619404"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM 的共同銷售連接器–總覽

### <a name="appropriate-roles"></a>適當的角色

- 推薦管理員
- CRM 上的系統管理員或系統自訂員

合作夥伴中心共同銷售連接器可讓您的銷售人員在您的 CRM 系統內與 Microsoft 共同銷售。 他們不必經過訓練，就能使用合作夥伴中心來管理共同銷售交易。 使用共同銷售連接器來建立新的共同銷售參考，以與 Microsoft 賣方交流、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值）和結束日期。 您也可以從 Microsoft 銷售人員收到這些共同銷售交易的任何更新。 您可以在您選擇的 CRM 中管理所有的參考工作，而不是在合作夥伴中心內。 

解決方案是以 Microsoft Power 自動化解決方案為基礎，並使用合作夥伴中心 Api。

## <a name="before-you-install---pre-requisites"></a>安裝之前的先決條件

|**主題**   |**詳細資料**   |**連結**   |
|--------------|--------------------|------|
|Microsoft 合作夥伴網路識別碼 |您需要有效的 MPN 識別碼|加入 [MPN](https://partner.microsoft.com/)|
|共同銷售準備就緒|您的 IP/服務解決方案必須已準備好共同銷售。|[與 Microsoft 銷售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作夥伴中心帳戶|與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您共同銷售解決方案相關聯的 MPN 識別碼相同。 先確認您可以在合作夥伴中心入口網站中看到共同銷售的參考，然後再部署連接器。|[管理您的帳戶](create-user-accounts-and-set-permissions.md)|
|合作夥伴中心使用者角色|將安裝並使用連接器的員工必須是推薦系統管理員|[指派使用者角色和權限](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|CRM 使用者角色是系統管理員或系統自訂員|[在 Dynamics 365 中指派角色](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power 自動化流程帳戶|使用資料庫為測試/預備和生產環境建立新的生產環境。 如果您有現有的生產環境與資料庫，就可以重複使用。 即將安裝連接器解決方案的使用者必須具備 Power 自動化授權和此環境的存取權。您可以按一下 [方案] 底下的 [查看歷程記錄]，來監視進度，並在 [電源自動化](https://flow.microsoft.com/) 時取得更多詳細資料。|[建立或管理環境](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>安裝 Dynamics 365 (Power 自動化解決方案) 的合作夥伴中心推薦同步處理

1. 移至 [ [電源自動化](https://flow.microsoft.com) ]，然後在右上角選取 [ **環境** ]。 此步驟會顯示可用的 CRM 實例。

2. 從右上角的下拉式清單中選取適當的 CRM 實例。

3. 選取左側導覽列上的 [ **方案** ]。

4. 按一下頂端功能表上的 [ **開啟 AppSource** ] 連結。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="開啟 AppSource":::

5. 在快顯視窗中搜尋 **合作夥伴中心的推薦連接器以進行 Dynamics365** 。  

6. 按一下 [ **立即取得** ] 按鈕，然後 **繼續** 進行。

7. 這會開啟頁面，您可以在其中選取 CRM (Dynamics 365) 環境以安裝應用程式。  同意條款及條件。

8. 您可以按一下 [**方案**] 底下的 [**查看歷程記錄**]，來監視進度，並在電源自動化時取得更多詳細資料。
 

9. 安裝完成之後，請流覽回到 [ [電源自動化](https://flow.microsoft.com) ]，然後從左側導覽區域選取 [ **解決方案** ]。 請注意，[方案] 清單中有提供 **Dynamics 365 的合作夥伴中心推薦同步** 處理。

10. 選取 **Dynamics 365 的合作夥伴中心推薦同步** 處理。 以下是可用的 Power 自動化流程和實體：

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="可用的 CRM":::

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：上線之前先進行測試

在生產環境中安裝、設定和自訂 Power 自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。

- 在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。
- 設定和自訂預備環境中的 Microsoft Power 自動化解決方案。
- 測試預備/CRM 實例上的方案。 
- 成功時，請將受控解決方案匯入至生產環境實例。 

## <a name="configure-the-solution"></a>設定解決方案

1. 在您的 CRM 實例中安裝解決方案之後，請流覽回到 [Power 自動化](https://flow.microsoft.com/)。


2. 從右上角的 [ **環境** ] 下拉式清單中，選取您安裝 Power 自動化解決方案的 CRM 實例。

3. 您將需要建立與三個使用者帳戶建立關聯的連接：

   - 具有推薦系統管理員認證的合作夥伴中心使用者

   - 合作夥伴中心事件

   - 具有解決方案中電源自動化流程的 CRM 系統管理員。

      1. 從左側導覽列 **中選取 [** 連線]，然後從清單中選取 **合作夥伴中心的參考** 解決方案。

      2. 按一下 [ **建立連接**] 來建立連接。

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="建立連線":::

      3. 在右上角的搜尋列中搜尋 **合作夥伴中心的推薦 (預覽)** 。

      4. 為合作夥伴中心使用者建立具有「參考系統管理員」認證角色的連接。

      5. 接下來，使用推薦的系統管理員認證來建立合作夥伴中心使用者的合作夥伴中心事件連線。

      6. 為 CRM 系統管理員使用者 (目前的環境) 建立 Common Data Service 的連接。
     
      7. 新增所有連線之後，您應該會在您的環境中看到下列連接：

         :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="連線":::
   
## <a name="edit-the-connections"></a>編輯連接

1. 返回 [ **方案** ] 頁面，然後選取 [ **預設方案**]。 按一下 [**全部**]，以選取 [ **(預覽) 的連接參考**。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="編輯連接":::

2. 選取三個點圖示，逐一編輯每一個連接。 新增相關的連接。

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="列出的連接"::: 

3.  返回 [解決方案] 頁面，選取 [Dynamics 365 的合作夥伴中心推薦同步處理]，然後按一下下列順序中每個流程旁的三個點圖示，即可開啟流程。 如果您在開啟流程時遇到任何問題，請參閱 [自訂步驟](connector-dynamics.md#customize-synchronization-steps) 和 [疑難排解步驟](connectors-troubleshoot.md)。 

依下列順序開啟流程：

- 合作夥伴中心 Webhook 註冊 (Insider Preview) 
- 建立共同銷售參考– Dynamics 365 至合作夥伴中心 (Insider Preview) 
- 定制從 Dynamics 365 flow 建立或取得詳細資料 
- 合作夥伴中心至 Dynamics 365-Helper (Insider Preview) 
- 合作夥伴中心 Microsoft 共同銷售參考更新至 Dynamics 365 (Insider Preview) 
- 合作夥伴中心至 Dynamics 365 (Insider Preview) 
- Dynamics 365 至合作夥伴中心 (Insider Preview) 
- Dynamics 365 商機至合作夥伴中心 (Insider Preview) 
- Dynamics 365 Microsoft 解決方案至合作夥伴中心 (Insider Preview) 
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>使用 Webhook Api 來註冊資源變更事件

合作夥伴中心 Webhook Api 可讓您註冊資源變更事件。 這些變更事件會以 HTTP 文章的形式傳送至您的 url。

1. 選取 **合作夥伴中心至 Dynamics 365 (Insider preview)**。

2. 選取 [ **編輯** ] 圖示，然後選取 [ **收到 HTTP 要求時**]。

3. 選取 **複製** 圖示來複製提供的 HTTP POST URL。

   :::image type="content" source="images/webhook-video.gif" alt-text="使用 webhook 來註冊資源變更":::

4. 選取「合作夥伴中心 Webhook 註冊 (Insider Preview) 」電源自動化流程，然後選取 [ **執行**]。

5. 確定已在右側窗格中開啟 [執行流程] 視窗，然後按一下 [ **繼續**]。

6. 輸入下列詳細資料：

   - **Http 觸發程式端點**：從先前步驟複製的 URL

   - **要註冊的事件**：選取所有可用事件 ( 「參考建立」、「參考-已建立」、「相關-推薦」、「相關-已更新」 ) 

   -**覆寫現有的觸發程式端點（如果有的話**）：是，請務必注意，只有一個 URL 可以針對指定的 webhook 事件註冊。 請務必注意，只有一個 URL 可以針對指定的 webhook 事件註冊。 

7. 選取 [ **執行** ]，然後選取 [ **完成]。**

Webhook 現在可以接聽建立和更新事件。

## <a name="customize-synchronization-steps"></a>自訂同步處理步驟

CRM 系統經過高度自訂，而且您可以根據您的 CRM 設定自訂 Power 自動化解決方案。  當合作夥伴中心與您的 CRM 系統之間的共同銷售參照進行同步處理時，在合作夥伴中心電腦上同步處理的欄位會列在 [自訂欄位對應指南](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)中。

依照欄位對應指南操作，如有必要，請在 [自訂] 中進行適當的變更，並 **從 Dynamics 365 流程或環境變數取得詳細資料**  。 建議您不要更新 Power 自動化解決方案中的任何其他流程，因為它可能會影響未來的解決方案升級。 

可用的自訂如下：

- 核取 [商機名稱] 中的 [標記]：根據預設，[商機名稱] 旁邊會顯示核取記號，表示合作夥伴中心與 Dynamics 365 CRM 之間的同步處理已成功發生。 同樣地，如果同步處理失敗，將會顯示交叉標記。 若要避免在商機名稱中新增核取或交叉標記，請將 [商機名稱] 環境變數中 [顯示] 核取記號的目前值設定為 [否]。

- 交易價值：根據預設，合作夥伴中心的交易價值將會在 CRM 中與 **estimatedvalue** 同步處理。 如果您在 CRM 中有不同的欄位可供同步處理的價值：

  a. 使用 CRM 的功能變數名稱更新 Dynamics 365 環境變數中的交易值功能變數名稱。 請注意，您應該提供欄位的名稱，而不是其顯示名稱。

  b. 編輯 **[自訂] 建立或取得 Dynamics 365 流程的詳細資料**  ，然後流覽至在 Crm 中 **建立或更新** 商機，並更新 **新的** 商機，並 **更新現有的商機** 動作，以將 **DealValue** 值指派給 crm 中的正確欄位。 此外，請從 [**估計收益**] 欄位中移除 **DealValue 指派**。

- 客戶帳戶國家/地區代碼：在建立新的參考時，必須提供兩個字母的國家/地區代碼 (ISO 3166) 。 根據預設，國家/地區代碼會與 CRM 中的帳戶 address1_country 欄位進行同步處理。 如果您的 CRM 中有不同的欄位可供同步處理的國家/地區代碼：

   a. 針對包含雙字母代碼的帳戶中的非查閱國家/地區代碼欄位：

   - 使用 CRM 的功能變數名稱更新 Dynamics 365 環境變數中的客戶帳戶國家/地區代碼功能變數名稱。 請注意，您應該提供欄位的名稱，而不是其顯示名稱。

   - 編輯 **[自訂] 建立或取得 Dynamics 365 流程的詳細資料**  ，然後流覽至 [建立或取得 crm 中的客戶帳戶] 動作，將國家/地區值指派給 crm 中的正確欄位。 此外，請移除位址1：國家/地區欄位中的國家/地區值指派。

   b. 針對帳戶中的 [以查閱為基礎的國家/地區代碼] 欄位：

   - 在 [帳戶] 中加入新的自訂欄位，並使用兩個字母的國家/地區代碼自動填入 (ISO 3166) 根據 [查閱] 欄位中選取的值，反之亦然。

   - 遵循上述的步驟，針對非查閱國家/地區代碼欄位，將新的自訂欄位從 CRM 同步處理到合作夥伴中心。

- 商機欄位：如果商機中有必要的欄位需要擴展 **[自訂]，請從 Dynamics 365 Flow 建立或取得詳細資料**  ，並在 CRM 中流覽至 **建立或更新商機** ，並更新 **建立新的商機動作** ，根據您的業務需求將值指派給必要欄位。

- 潛在客戶欄位：如果潛在客戶中有需要填入的強制欄位： **[自訂] 建立或從 Dynamics 365 流程取得詳細資料**  ，然後流覽至 [ **建立或更新** CRM 中的潛在客戶] 和 [更新] **建立新的潛在客戶動作** ，根據您的業務需求將值指派給必要欄位。

- 客戶帳戶：當新的參考從合作夥伴中心同步處理至 CRM 時，Power 自動化解決方案會嘗試使用客戶公司名稱和郵遞區號在 CRM 中搜尋現有的帳戶。 如果找不到，則會在 CRM 中建立新的客戶帳戶。 若要更新搜尋條件和新的帳戶建立詳細資料，請編輯 **[自訂] 建立或從 Dynamics 365 流程取得詳細資料** ，然後流覽至在 CRM 中 **建立或取得客戶帳戶** ，並 **建立客戶帳戶動作**。

## <a name="update-environment-variable"></a>更新環境變數

若要更新環境變數值：

1. 移至 [ **方案** ] 頁面，然後選取 [ **預設方案**]。 按一下 [全部]，以選取 [ **環境變數** ]。

2. 針對需要更新的值選取環境變數，然後按一下 [使用三個點 **編輯** ] 圖示。

3. 更新 **目前的值** (請勿使用 [ **新值** ] 選項) 更新預設值，並提供值。 值必須符合變數的資料類型，例如 [是]/[否] 資料類型會接受 [是] 或 [否] 值。

   :::image type="content" source="images/environment-variables-video.gif" alt-text="更新環境變數":::

- 端對端雙向共同銷售推薦同步處理

安裝、設定和自訂 Power 自動化解決方案之後，您可以測試 Dynamics 365 與合作夥伴中心之間的共同銷售推薦同步處理。

### <a name="pre-requisites"></a>必要條件

若要同步處理合作夥伴中心與 Dynamics 365 CRM 之間的參考，Power 自動化解決方案會清楚標示 Microsoft 特定的參考欄位。 此識別可讓您的賣方團隊能夠決定他們想要與 Microsoft 分享哪些參考，以進行共同銷售。

在解決方案安裝過程中，會加入一組自訂欄位和物件。 CRM 系統管理員使用者必須建立具有 **商機** 自訂欄位的個別 CRM 區段。

下列自訂欄位應該是 CRM 區段的一部分：

- **與合作夥伴中心同步**：是否要與 Microsoft 合作夥伴中心同步商機。 依預設，此欄位的值為 [否]，而且您的賣方必須明確設定為 [是]，才能與 Microsoft 分享商機。 從合作夥伴中心共用的新參考會將此域值設定為 [是]。

- **參考識別碼**： Microsoft 合作夥伴中心的唯讀識別碼欄位參考

- **參考連結**： Microsoft 合作夥伴中心內的參考唯讀連結
- **Microsoft 如何協助？**： microsoft 提供的參考說明。 若要建立共同銷售的參考，請選取 Microsoft 所需的適當說明。 客戶連絡人必須與建立共同銷售參考的商機相關聯。 若要建立非共同銷售的參考，請不要選取此欄位。 您可以藉由選取適當的 [必要的說明] 選項，隨時將非共同銷售的參考轉換成共同銷售的參考。

- **Microsoft 合作夥伴中心的參考可見度**：選取 Microsoft 合作夥伴中心推薦的可見度。 藉由讓 Microsoft 銷售人員看得到，非共同銷售的參考可能會轉換成共同銷售。 當需要 Microsoft 協助時，預設會對 Microsoft 銷售者顯示推薦。 標記為可見之後，就無法還原此欄位。

- **MICROSOFT CRM 識別碼**：當共同銷售的參考是由 microsoft 所建立並接受時，此欄位將會填入 MICROSOFT 的 CRM 識別碼。

- **產品：已淘汰** –請勿使用此欄位或將它新增至 CRM 區段，只適用于回溯相容性。 改為使用 Microsoft 合作夥伴中心方案。

- **Audit**：與合作夥伴中心參考同步的唯讀審核記錄

- **Microsoft 合作夥伴中心解決方案**：自訂物件，可將共同銷售就緒解決方案或 Microsoft 解決方案與商機產生關聯。 您可以新增及/或從商機中移除一或多個解決方案。 在與 Microsoft 共用之前，您必須先將至少一個共同銷售就緒或 Microsoft 解決方案新增至商機。 若要建立此物件與商機之間的關聯，請更新 CRM 中的商機表單：

  在 [商機] 表單中選取適當的索引標籤，然後新增子方格，如下所示：

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="商機表單":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{替代文字}":::

- 新增 Microsoft 解決方案之後，您可以預先填入共同銷售就緒解決方案詳細資料，讓您的銷售人員不需要新增它們。 若要加入新的解決方案詳細資料，請移至 CRM 中的 Microsoft 解決方案詳細資料物件，然後按一下 [ **新增記錄** ] 以新增一個專案，或使用 **Excel 上傳** 來新增多個專案。

  :::image type="content" source="images/dynamic-1a.png" alt-text="解決方案詳細資料":::

### <a name="scenarios"></a>案例：

1. 在 CRM 中建立或更新參考時的參考同步處理，並在合作夥伴中心內同步處理：

   1. 登入您的 Dynamics 365 CRM 環境，讓使用者能夠看見 CRM 的 **商機** 區段。

   2. 當您在 Dynamics 365 環境中建立「新商機」時，請確定 Microsoft 合作夥伴中心區段存在

   :::image type="content" source="images/dynamic-2a.png" alt-text="新商機"::: 

   3. 若要與合作夥伴中心同步處理這個機會，請確定您已在卡片視圖中設定下欄欄位：

      - **Microsoft 如何協助？**：若要建立共同銷售的參考，請選取適當的說明選項。

         :::image type="content" source="images/dynamic-3a.png" alt-text="如何在卡片視圖中取得適當的欄位":::

      - **客戶連絡人**：若要建立共同銷售的參考，請將客戶連絡人新增至商機。

      - **與合作夥伴中心同步**：是

      - Microsoft 解決方案：若要與 Microsoft 分享參考，請將有效的共同銷售就緒或 Microsoft 解決方案新增至商機。
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="解決方案識別碼":::

   4. 一旦在 Dynamics 365 中建立商機，並將 [同步與合作夥伴中心] 選項設為 [是]，請等候10分鐘，然後登入您的合作夥伴中心帳戶。 您的參考會與 Dynamics 365 和參考識別碼進行同步處理。 將會填入參考連結。 如果發生失敗，[審核] 欄位將會填入錯誤資訊。
     
    5. 同樣地，如果有機會將 [與合作夥伴中心同步] 選項設為 [是]，則當您更新 Dynamics 365 CRM 的商機時，變更將會在您的合作夥伴中心帳戶中同步處理。

    6. 使用合作夥伴中心成功同步處理的商機將會以 Dynamics 365 中的✔圖示來識別。

2. 在 Microsoft 合作夥伴中心內建立或更新參考時的參考同步處理，並在 Dynamics 365 環境中同步處理：

   1. 登入您的合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/home)。

   2. 從左側功能表中選取 [ **參考** ]。

   3. 選取 [  **新增交易** ] 選項，從合作夥伴中心建立新的共同銷售推薦。

   4. 登入您的 Dynamics 365 CRM 環境。

   5. 流覽至 **開啟的商機**。 在 Microsoft 合作夥伴中心內建立的參考現已在 Dynamics 365 CRM 中同步處理。

   6. 當您選取同步處理的參考時，就會填入卡片視圖詳細資料。

## <a name="next-steps"></a>下一步

- [管理潛在客戶](manage-leads.md)

- [管理共同銷售商機](manage-co-sell-opportunities.md)

- [深入瞭解 Microsoft Power 自動化平臺？](/power-automate/)

- [合作夥伴中心 Webhook](/partner-center/develop/partner-center-webhooks)
