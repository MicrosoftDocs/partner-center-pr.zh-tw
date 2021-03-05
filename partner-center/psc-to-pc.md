---
title: '從合作夥伴銷售 Connect 遷移 (PSC) '
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 Microsoft 合作夥伴如何可以從合作夥伴銷售 Connect (PSC) 遷移至合作夥伴中心，並建立或管理 Microsoft 銷售人員所傳送的交易。
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 495d9899db36d0e4911647b337a99105a063236c
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124817"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>合作夥伴中心內的共同銷售指南 (電腦) ，適用于從合作夥伴銷售 Connect (PSC 進行遷移的合作夥伴) 

**適當的角色**

- 帳戶管理員
- 推薦管理員
- 合作夥伴銷售 Connect (PSC) 賣方
- 合作夥伴銷售 Connect (PSC) 管理員
- 合作夥伴銷售 Connect (PSC) 交易經理

本文提供從合作夥伴銷售 Connect 遷移至合作夥伴中心的合作夥伴指引，讓他們可以在合作夥伴中心內繼續建立及管理共同銷售交易。

>[!Note]
> 如果您在這裡看到關於遷移的資訊，您就是在正確的位置。 本指南不適用於解決方案評估 (SA) 和 OEM 授權商務合作夥伴管理其在 PSC 的交易。

>[!Important]
> 自2021年4月1日起，您的公司將無法建立或編輯 PSC 的交易。 **您仍然可以使用 PSC 的大量匯出功能來下載現有交易資料。您也可以在此日期之後，將 [open 交易](psc-to-pc.md#psc-deals-migration) 從 PSC 遷移到合作夥伴中心。** <br><br> 如果您正在積極處理的交易包含 IP 共同銷售激勵符合資格的解決方案，您有兩個選擇： <br><br> 1. 在2021年3月31日前，于 PSC 中將交易標示為贏及完成交易註冊。 <br> 2. [將交易遷移](psc-to-pc.md#psc-deals-migration) 至合作夥伴中心，讓您有更多時間處理並開始交易註冊。

如您所知， **公司將在2021年4月30日之後失去對 PSC 的存取權**。 不過，您仍然可以在合作夥伴中心內找到您想要進行的所有作業，例如建立共同銷售交易、管理交易，以及採取 Microsoft 銷售人員傳送給您的交易。

不過，會有一些差異。 下列指導方針可協助您將轉換至合作夥伴中心的工作更順暢、更簡單。

## <a name="before-you-move-things-you-need-to-know"></a>移動之前，您必須知道的事項

### <a name="if-you-are-a-psc-admin"></a>如果您是 PSC 系統管理員

- 您需要使用工作電子郵件來登入 [合作夥伴中心](https://partner.microsoft.com/)。
- 使用合作夥伴中心 [帳戶管理員](permissions-overview.md)來設定您的帳戶。
- 閱讀這份檔，瞭解如何在合作夥伴中心共同銷售。
- 為您所有的 PSC 使用者，設定合作夥伴中心內的使用者帳戶， (系統管理員、交易管理員和賣方角色) 並指派給他們 [參考系統管理員角色](permissions-overview.md)。

>[!IMPORTANT]
> 請確定 [合作夥伴中心] 的 MPN 位置清單中有提供 [PSC] 橫幅中顯示的 MPN 識別碼。

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="此圖顯示可供合作夥伴尋找 MPN 識別碼的 PSC 橫幅。":::

 若要確認 MPN 識別碼會顯示為合作夥伴中心的 MPN 位置，請登入 [合作夥伴中心] [儀表板](https://partner.microsoft.com/dashboard)，然後選取畫面右上方的齒輪圖示) 的 [ (**設定** ]，接著選取 [ **帳戶設定**]。 在第二層的左側導覽功能表中，選取 [ **位置** ]，以查看與合作夥伴中心帳戶相關聯的所有 MPN 識別碼和位置的清單。

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>如果您是 PSC 交易經理或賣方

- 您需要使用工作電子郵件來登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)。
- 如果您在 PSC 中使用非工作帳戶，或您的公司電子郵件與合作夥伴公司不同，請洽詢您的 PSC 系統管理員，以取得帳戶設定的說明。
- 如果您的合作夥伴中心帳戶設定已完成，不論您用來登入 PSC 的帳戶是否完整，請洽詢您的 PSC 系統管理員。
- 確認您是否有合作夥伴中心和 [參考] 區段的存取權。
- 閱讀這份檔，瞭解合作夥伴中心內的工作流程和變更。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>作為 PSC 的系統管理員，這些是您的後續步驟

從 [合作夥伴中心] 左側導覽功能表中，選取 [ **參考** ] 選項。 確認您可以存取 [參考] 頁面。

  >[!Note]
  > 您可能必須登出合作夥伴中心並重新登入，以重新整理您的認證以存取 [參考] 頁面。

如果您在 [合作夥伴中心] 功能表或 [參考] 相關頁面上看不到 [ **參考** ] 選項，請洽詢貴公司的 [帳戶管理員](permissions-overview.md) ，並要求他們提供您存取 [ **參考** ] 選項和相關區域。

若要尋找您公司的帳戶管理員：

1. 從 [合作夥伴中心] 儀表板右上角的齒輪圖示，選取 [ **帳戶設定** ]。

1. 從第二層、左側導覽功能表選取 [ **使用者管理** ]。

1. 在 [使用者] 清單的頂端，選取 [ **篩選** ] 下拉式功能表。 將選項變更為 [ **帳戶管理員**]。

   頁面會顯示所有的帳戶管理員及其各自的電子郵件地址。 傳送電子郵件給其中一封電子郵件，要求他們為您的工作帳戶指派「參考管理員」角色。

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="顯示 [夥伴設定] 使用者管理頁面中帳戶管理員的影像。":::

>[!Important]
>- 如果您的角色只牽涉到管理 PSC 中的使用者，請要求貴公司的帳戶管理員將「合作夥伴中心」的 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company) 角色指派給您。 
>- 如果您的角色也包含管理共同銷售機會，請要求獲派「 [推薦系統管理員](permissions-overview.md#manage-referrals) 」角色。
> - 建議您也在 PSC 系統管理員中提名一個變更管理領導人。 這樣做會讓所有的 PSC 系統管理員都不需要個別接觸到合作夥伴中心帳戶管理員。 相反地，變更管理潛在客戶可以是與合作夥伴中心帳戶管理員合作的主要人員。

## <a name="user-migration"></a>使用者移轉

在合作夥伴中心設定您的帳戶之後，請使用 [共同銷售商機] 頁面中的 [使用者遷移嚮導]，將合作夥伴中心角色自動指派給公司的員工。

>[!Note]
> 使用者遷移只能由公司的 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company) 執行。 如果您沒有帳戶管理員角色，請尋找可協助您使用「使用者遷移嚮導」來設定使用者帳戶的帳戶管理員。

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="顯示使用者遷移嚮導的影像。":::

帳戶管理員會在「參考指南」旁的 [共同銷售商機] 頁面中，看到 [PSC 使用者遷移嚮導] 連結。 他們可以藉由選取連結來起始使用者遷移。 若要起始使用者遷移，系統管理員可以選取連結。 他們可以多次執行此使用者遷移步驟，直到所有使用者都已在合作夥伴中心指派適當的角色。

使用者遷移表具有下列詳細資料：

- 使用者帳戶-員工的電子郵件識別碼
- PSC 合作夥伴帳戶-與 PSC 相關聯的員工帳戶
- PSC 使用者角色-指派給 PSC 的三個角色之一。
- 電腦 MPN 位置-將相關電腦角色提供給使用者的位置。 PSC partner account MPN 可用來在合作夥伴中心尋找對等的 MPN 位置以指派許可權。 整個組織代表 vOrg MPN 識別碼。
- 電腦使用者角色-員工會根據其 PSC 使用者角色指派角色。 PSC 中的系統管理員將會被指派電腦的推薦系統管理員角色。 賣方將會被指派電腦中的推薦使用者角色。 若要深入瞭解電腦角色以及這些角色的使用者可以在[合作夥伴中心進行](permissions-overview.md#manage-referrals)的動作，請參閱
- 電腦 AAD 租使用者-在合作夥伴中心將使用者指派至其中的租使用者
- 狀態-遷移狀態有三個可能的狀態
    - **未遷移** -使用者未指派任何電腦參考角色
    - 已 **遷移**-使用者已成功遷移，並已指派相關角色，如下表所示
    - **錯誤** -因某些錯誤而無法完成遷移

有時候，遷移可能會失敗，並導致錯誤。 以下是一些可能會造成錯誤的原因，以及解決問題的一些方法：

1. PSC 使用者可能使用非工作帳戶。

2. PSC 使用者可能會使用不同于您在合作夥伴中心所使用之網域的帳戶。

   若要解決案例1和2的相關錯誤，請要求使用者使用附加至您 Azure AD 租使用者的工作帳戶登入合作夥伴中心。 您的 [全域管理員](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) 可以提供協助。
   
   若要尋找您的全域管理員： 
   - 登入 [合作夥伴中心] [儀表板](https://partner.microsoft.com/dashboard) ，並從右上角的齒輪圖示選取 [ **帳戶設定** ]。
   - 從第二層、左方導覽列選取 [ **使用者管理** ]。
   - 在 [使用者] 清單的頂端，選取 [ **篩選** ] 下拉式功能表，然後將選項變更為 [ **全域管理員**]。頁面接著會顯示所有全域管理員及其各自的電子郵件地址。 要求其中一個使用者為您的工作帳戶指派參考系統管理員角色。
   
      全域管理員可以在您的 Azure AD 租使用者中建立新的使用者帳戶，或將來賓使用者存取權指派給其他網域帳戶使用者。 一旦為所有 PSC 交易管理員和使用者設定帳戶之後，他們必須登入合作夥伴中心，從左側導覽功能表中選取 [ **參考** ]，然後確認他們可以看到 [參考] 頁面。

3. 使用者已在合作夥伴中心內有指派的參考角色。
    - 您可以驗證使用者的現有角色。 在合作夥伴中心的右上角，選取齒輪圖示) 的 **設定** (，然後選取 [ **帳戶設定**]。 當您看到第二個左導覽功能表時，請選取 [ **使用者管理** ]，並搜尋使用者。

## <a name="psc-deals-migration"></a>PSC 交易遷移

完成使用者遷移之後，請使用 [共同銷售商機] 頁面中的 [交易遷移嚮導]，將所有符合資格的 open 交易從 PSC 帶入電腦。 **交易遷移連結將只會顯示在合作夥伴中心內整個組織範圍的推薦系統管理員。** 在共同銷售商機頁面的右上方會有稱為「 **PSC 交易遷移** 」的連結，該頁面將會開啟「交易遷移嚮導」。

開始進行交易遷移之前，請先閱讀本節。

**適用于遷移**

只有部分交易才有資格從 PSC 遷移至電腦。 這個遷移嚮導的設計，是為了協助合作夥伴將交易移至合作夥伴中心，讓他們仍在主動與客戶合作，以達成交易。 **只有在2020年1月1日的開啟狀態下，使用有效的合作夥伴帳戶詳細資料來建立的交易 (有效的 MPN 識別碼) ，而不會進行交易註冊則適合進行遷移。**

**不適合進行遷移**

- 解決方案評估交易不符合交易遷移的資格
- OEM 授權商務交易不符合交易遷移的資格
- 所有已在 PSC 中標示為獲勝的交易都不適合進行遷移。 如果有資格參加標示為「成功」的交易，請務必在 PSC 中完成註冊。

## <a name="pre-requisites-for-deal-migration"></a>交易遷移的先決條件

開始從電腦進行交易遷移之前，請遵循下列指示來設定 PSC 中的交易，以順利進行遷移。

1. 您公司中從事 open 交易的所有銷售團隊成員都有關于這項遷移的通知。
2. 銷售團隊成員會經過定型，以使用合作夥伴中心進行交易管理。
3. 交易具有所有必要的資訊，如下所述。
    - 客戶公司詳細資料，包括名稱和位址
    - 客戶連絡人詳細資料（如果是共同銷售交易）
    - 至少一個解決方案
    - 至少一個具有所有詳細資料的小組成員-名字、姓氏、電子郵件識別碼及電話號碼
    - 交易價值
    - 預估的交易關閉日期
    - 合作夥伴注意事項

您可以使用 PSC 的大量下載和上傳功能，在所有符合資格的交易中加入所有遺漏的詳細資料。

>[!Note]
> 即使不符合上述先決條件，交易遷移也會成功。 但是，如果合作夥伴中心內有任何上述必要欄位無法使用，您就無法變更交易的狀態。 然後，您必須在合作夥伴中心的交易中輸入所有缺少的必要資訊，才能開始處理。 **強烈建議您先清除 PSC 中符合資格的交易，再將其遷移至合作夥伴中心。**

合作夥伴中心內的交易遷移已建立為單鍵體驗。 只要您的公司準備好遷移符合資格的交易，您只需要按一下 [ **遷移交易]** 按鈕即可。 **您無法選擇要從 PSC 遷移的交易。如果您不想要將任何交易遷移至合作夥伴中心，請在開始進行遷移之前，將其移到 PSC 的「已關閉」狀態。**

>[!Note]
> 開始遷移之後， **最多可能需要24小時的時間，才會遷移交易**。

完成遷移後，橫幅訊息的狀態將會變更為 [完成]，並包含遷移報表的連結。 下載報表以查看從 PSC 遷移至 PC 的交易詳細資料。

報表包含下列詳細資料。

1. **合作夥伴中心參與識別碼** -合作夥伴中心內的唯一識別碼，適用于參與專案中的所有交易。 有兩個交易：一個適用于合作夥伴，另一個則用於合作夥伴中心的共同銷售合作。
2. **合作夥伴中心的參考** 識別碼-合作夥伴中心內屬於夥伴之交易的唯一識別碼。
3. **交易名稱** -提供給 PSC 的交易識別碼。
4. **Psc 交易識別碼** -此交易的 psc 中的唯一識別碼。
5. **錯誤** -指出遷移特定交易時是否有任何錯誤。

所有已成功遷移的交易將不會顯示在 PSC 中。 您可以繼續處理電腦上已遷移的交易，包括在 PC 中完成交易註冊。 共同銷售交易的 Microsoft 銷售人員的互動不會有任何變更。

從 PSC 遷移的交易將會根據交易來源，在輸入和輸出索引標籤中提供。 您公司所共用的所有交易都將可在 [輸出] 索引標籤中取得，而 Microsoft 起始的交易將會出現在合作夥伴中心的 [輸入] 索引標籤中。 遷移後將會建立兩種類型的交易。

1. **共同銷售交易** （標示為共同銷售的 PSC）將在合作夥伴中心內建立為共同銷售交易。
2. **夥伴主導的交易** （未標示為共同銷售的交易）將在合作夥伴中心內建立為合作夥伴主導的交易。 Microsoft 銷售人員可以看到合作夥伴主導的交易，而且可以在達到終止狀態 (贏得、遺失) 之前，升級為共同銷售交易。 此外，如果交易中有獎勵符合資格的解決方案，夥伴主導的交易就有資格進行交易註冊。

>[!Important]
> 如果因為某些交易無法遷移而發生任何錯誤， **您可以按一下 [遷移交易] 按鈕來重新起始交易遷移**。 只有有一些符合資格的交易還在進行遷移時，才會啟用此功能。 如果您在轉換階段中，在開始進行交易遷移之後，某些新交易會在 PSC 中建立，這也會很有説明。

所有交易都成功遷移後，會有橫幅顯示「**沒有交易可供遷移**」，並 **停** 用 [**遷移交易]** 按鈕。

完成使用者遷移及/或交易遷移之後，請使用下列指導方針來決定遷移策略：

如果您的公司有合作夥伴開發經理 (PDM) -當您的合作夥伴中心帳戶已設定，而且您的使用者已移動並具有角色和許可權時，您可以將共同銷售活動移至合作夥伴中心。 通知 PDM 進行切換，而不是等到您的遷移完成期限，讓您所有的新交易都流動到合作夥伴中心。

>[!Note]
>一旦您進行此切換之後，您就只能針對 PSC 中現有的主動式交易採取行動。 您不能建立新交易，也不會收到來自 PSC 的 Microsoft 賣方的任何交易。

如果您的公司沒有 PDM，請確定所有使用者都已設定並驗證所有的使用者帳戶。 當您在合作夥伴中心內開始共同銷售時，將會透過電子郵件和 PSC 中的橫幅來通知您。 請記住，您仍然需要管理 PSC 中現有的主動式交易。

>[!Important]
> 您可以在2021年4月30日前註冊標示為贏的交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>適用于 PSC 管理員、PSC 交易經理和 PSC 賣方的後續步驟

瞭解如何在合作夥伴中心共同銷售。
這是很重要的步驟，可協助您為合作夥伴中心內的共同銷售做好準備。 瞭解合作夥伴中心內的工作流程和變更，讓您可以有效地立即共同銷售。 一開始請完整閱讀這份檔。 [共同銷售體驗資源庫](https://aka.ms/cosellexperience)也提供一組良好的資源。

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC 與 PC 工作流程之間的主要差異

|**案例**|**合作夥伴銷售連接**|**合作夥伴中心**|
|-----|:-----|:-----|
|使用者角色|PSC 具有系統管理員、交易經理和賣方角色。|電腦只有 [參考系統管理員](permissions-overview.md#manage-referrals) 角色，可提供所有交易的讀取和寫入權限。|
|邀請 Microsoft 共同銷售交易|由 Microsoft 賣方起始，沒有合作夥伴的明確要求。|如果需要 Microsoft 銷售人員協助，合作夥伴將必須提出 [明確的要求](manage-co-sell-opportunities.md#add-solutions) 。 Microsoft 賣方有一個拒絕要求的選項。|
|Expiry|交易到期沒有任何概念。|夥伴輸入交易如果夥伴不接受，則會在14天內到期。 如果 Microsoft 銷售人員在14天內未採取任何動作，就會發生這種情況：夥伴輸出交易可進入已過期狀態。|
|Microsoft 賣方詳細資料|在交易建立後立即顯示。|只有當賣方明確接受合作夥伴的共同銷售邀請時，才會與合作夥伴共用 Microsoft 賣方詳細資料。|
|[私人管線](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|不適用。|合作夥伴可以共用其管道，而不會提供 Microsoft 銷售人員的可見度。|
|方案|只有一個價位清單的解決方案可以新增到交易中。|夥伴可以加入屬於下列清單的 [解決方案](manage-co-sell-opportunities.md#add-solutions) 。 答) 自己的解決方案 b) Microsoft 第一方目錄的解決方案 (類似于) PSC 的交易交易角色與其他協力廠商合作夥伴的 c) 共同銷售解決方案 (類似于 PSC) 中的 ISV 交易角色。|
|交易指派|只有指派的賣方才能查看交易並採取行動。|您可以將小組成員新增到交易中，以指定處理工作的人員，而不會封鎖其他的推薦系統管理員來觀看或處理這些交易。|
|客戶組織|自由格式文字專案。|只要輸入幾個字元，就可以針對[D&B 資料庫](https://www.dnb.com/)搜尋[客戶組織](manage-co-sell-opportunities.md#select-your-customer)。 合法的名稱和位址會根據選擇自動填入。|
|客戶連絡人|不是必要的。|私人管線共用不是必要的。 如果 Microsoft 賣方受邀參與共同銷售要求，則為必要項。|
|公用 API|不適用。|[公用 API](/partner/develop/referrals) ，以程式設計方式管理合作夥伴中心的參考。|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>將 PSC 的欄位對應至合作夥伴中心的對應欄位

本節會針對針對「合作夥伴中心共同銷售商機」一節中的對應視圖，為 PSC 顯示的 (或「對應」 ) 選取的螢幕擷取畫面。

您會在每一對螢幕擷取畫面上看到編號、黃色或紅色圓圈：

- **黃色圓圈是什麼意思？** 編號的黃色圓圈會先出現在每個 PSC 螢幕擷取畫面上。 然後，您會在其下找到內含許多相同數位的隨附合作夥伴中心螢幕擷取畫面。

   若要查看 PSC 中的每個欄位或屬性如何對應至合作夥伴中心內的對應項，請在兩個相關的螢幕擷取畫面中，將編號的圓形一起配對。 例如，在第一個中比對編號、黃色 "1"，而在第二個的第二個中，第二個則是合作夥伴中心螢幕擷取畫面。

- **紅色圓圈代表什麼意思？** 如果您在一個螢幕擷取畫面上看到紅色圓圈，表示 [合作夥伴中心] 中未提供 [PSC] 欄位。

以下區域會顯示 PSC 與合作夥伴中心的欄位對應：

1. 與合作夥伴中心共同銷售商機預設視圖對應的 PSC 首頁
1. 對應至合作夥伴中心交易視圖的 PSC 方格視圖
1. 與合作夥伴中心交易詳細資料檢視對應的 PSC 交易詳細資料檢視
1. PSC 新增產品視圖對應到合作夥伴中心新增解決方案視圖
1. 與合作夥伴中心使用者管理檢視對應的 PSC 使用者管理檢視
1. 對應至合作夥伴中心角色指派視圖的 PSC 使用者角色指派視圖
1. 對應至合作夥伴中心通知視圖的 PSC 通知視圖

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-與合作夥伴中心共同銷售商機預設視圖對應的 PSC 首頁

比較最上層的 PSC 螢幕擷取畫面與其下的合作夥伴中心螢幕擷取畫面之間相符、編號的圓形。 相符的數位會顯示您可以在合作夥伴中心找到 PSC 相關功能或屬性的位置。 紅色圓圈表示沒有相符的合作夥伴中心欄位。  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="顯示夥伴銷售 Connect 首頁與合作夥伴中心內共同銷售商機之預設觀點之間的欄位對應影像。" lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-與合作夥伴中心交易視圖對應的 PSC 方格視圖

比較最上層的 PSC 螢幕擷取畫面與其下的合作夥伴中心螢幕擷取畫面之間相符、編號的圓形。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示沒有相符的合作夥伴中心欄位。  

> [!NOTE]
> 其他考慮會顯示在螢幕擷取畫面下方。

:::image type="content" source="images/pscmigration/gridview.png" alt-text="顯示夥伴銷售 Connect (PSC 之間的欄位對應的影像) 格線視圖和合作夥伴中心交易觀點。" lightbox="images/pscmigration/grid-view-expanded.png":::

**特殊考慮事項：**

- 合作夥伴中心沒有任何清單視圖，如同 PSC 一樣。  所有交易都會依據客戶資訊和交易類型，以最新的接收或建立日期列出。 預設會選取 view 中的第一筆交易。 以 PSC 資料表格式顯示的大部分值都可在電腦的詳細資料檢視中取得。
- 交易角色不是電腦中的必要欄位。 它不會在任何工作流程中顯示或捕捉。 它會根據新增至交易的解決方案，在 Microsoft 賣方端自動衍生。
- 上次修改日期不會顯示在 PC 的 [推薦詳細資料] 頁面上。 夥伴可以使用排序功能，根據上次更新日期來排序交易。

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-與合作夥伴中心對應的 PSC 交易詳細資料檢視

比較頂端 (PSC 的相符、已編號的圓形) 螢幕擷取畫面，以及其下的合作夥伴中心螢幕擷取畫面。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示合作夥伴中心沒有相符的欄位或區域。

> [!NOTE]
> 其他考慮會顯示在螢幕擷取畫面下方。

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="顯示夥伴銷售 Connect (PSC 之間的欄位對應的影像) 交易詳細資料檢視和合作夥伴中心的交易詳細資料檢視。" lightbox="images/pscmigration/deal-details-expanded.png":::

**特殊考慮事項：**

- 合作夥伴可以選取夥伴交易詳細資料檢視上的 [編輯] 按鈕 (6) 來編輯交易。 選取 [編輯] 按鈕之後，所有欄位都將變成可編輯。 然後，您可以選擇儲存或取消對交易進行的編輯。
- 在合作夥伴中心內沒有任何選項可關閉重複的交易。
- 合作夥伴中心未提供客戶成果。 所有與客戶互動相關的詳細資料都可以在 PC 的 Notes 區段中更新。
- 預估的解決方案結束日期僅適用于合作夥伴中心的 OEM IOT 交易。 任何其他交易類型都不會顯示這項資訊。
- 電腦不需要授權方案。 這項資訊會根據在交易中選取的解決方案自動推斷。

>[!Note]
>任何標示為「成功」或「遺失」的交易，之後都無法編輯。 將交易移至這些終端機狀態的其中一個時，請務必小心。

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-PSC 的 [新增產品] 視圖對應到合作夥伴中心的 [新增解決方案] 視圖

比較頂端 (PSC 的相符、已編號的圓形) 螢幕擷取畫面，以及其下的合作夥伴中心螢幕擷取畫面。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示合作夥伴中心沒有相符的欄位或區域。
  
:::image type="content" source="images/pscmigration/products.png" alt-text="顯示 Partner Sales Connect (PSC 之間的欄位對應影像) 新增產品視圖和合作夥伴中心新增解決方案觀點。" lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-PSC 與合作夥伴中心的使用者管理

比較頂端 (PSC 的相符、已編號的圓形) 螢幕擷取畫面，以及其下的合作夥伴中心螢幕擷取畫面。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示合作夥伴中心沒有相符的欄位或區域。  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="顯示合作夥伴銷售 Connect (PSC 之間的欄位對應影像) 使用者管理首頁和 [合作夥伴中心] 使用者管理頁面在 [帳戶設定] 區域內的頁面。"  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-在 PSC 與合作夥伴中心的使用者角色指派

比較頂端 (PSC 的相符、已編號的圓形) 螢幕擷取畫面，以及其下的合作夥伴中心螢幕擷取畫面。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示合作夥伴中心沒有相符的欄位或區域。  

:::image type="content" source="images/pscmigration/roles.png" alt-text="顯示夥伴銷售 Connect (PSC) 角色指派視圖和合作夥伴中心角色指派視圖之間的欄位對應影像。" lightbox="images/pscmigration/roles-expanded.png":::

**特殊考慮事項：**

- 與 PSC 管理員同等的角色是合作夥伴中心內的帳戶管理員角色。
- 合作夥伴中心內只有一個角色可進行共同銷售交易管理。 此角色是參考管理員角色。

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-PSC 與合作夥伴中心的通知

比較頂端 (PSC 的相符、已編號的圓形) 螢幕擷取畫面，以及其下的合作夥伴中心螢幕擷取畫面。 相符的數位會顯示您可以在合作夥伴中心尋找與 PSC 相關的功能或屬性。 紅色圓圈表示合作夥伴中心沒有相符的欄位或區域。  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="顯示合作夥伴銷售 Connect (PSC) 通知和合作夥伴中心通知觀點之間對應的影像。"  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>從 PSC 移至合作夥伴中心-常見問題

下列各節會回答有關遷移的常見問題。

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-如果我沒有合作夥伴中心的存取權，該怎麼辦？

您可以聯絡您在 [沒有存取權] 頁面上列出的系統管理員，以取得指派的角色。 在 [參考] 區段下，您將需要「讀取」和「寫入」許可權的「 [參考管理員](permissions-overview.md#manage-referrals) 」角色。 如果您只管理商務設定檔，則您需要合作夥伴中心內的商務設定檔系統管理員角色。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="顯示合作夥伴中心內無存取體驗的影像。":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-誰可以授與我合作夥伴中心內 [參考] 區段的存取權？

您的 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company)可以授與您存取 [參考] 索引標籤。若要尋找您的帳戶管理員，請從 [合作夥伴中心][儀表板](https://partner.microsoft.com/dashboard)右上角的齒輪圖示中選取 [**帳戶設定**]。 然後，從第二層、左側導覽列選取 [ **使用者管理** ]。 在 [使用者] 清單的頂端，選取 [ **篩選** ] 下拉式功能表，然後將選項變更為 [ **帳戶管理**]。頁面會顯示所有的帳戶管理員及其各自的電子郵件地址。 要求其中一個使用者為您的工作帳戶指派參考系統管理員角色。

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-我們的帳戶的 [+ 新增交易] 按鈕呈現灰色。 我該怎麼做才能開始建立交易？

只有在沒有共同銷售就緒的解決方案附加至您在合作夥伴中心使用的 MPN 組織時，才會發生這種情況。 請洽詢您的 PDM 以取得解決方案的 MPN 識別碼，或建立一個提及問題的支援票證：「在 PSC 遷移後新的交易按鈕呈現灰色」。

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-我可以將交易指派給組織中的特定人員，例如 PSC 嗎？

您可以將小組成員指派給特定的交易。 它不會封鎖其他的參考管理員來進行流覽或處理這些交易。

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-是否有所有指派給我的交易觀看？

您可以使用 [我的最愛] 功能，也就是使用者層級索引標籤。您可以將指派給您的所有交易都標示為 [我的最愛]，以快速存取交易。

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-是否有交易的唯讀視圖？

否，在 [參考] 區段中不會顯示交易的唯讀狀態。 所有的參考系統管理員都將擁有所有交易的完整讀取和寫入存取權。

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-如何在將交易標示為贏後進行註冊？

如果交易符合下列準則，我們將會顯示一個快顯視窗，以開始進行 [交易註冊](./register-deals.md)。

- 有一項獎勵符合資格的解決方案附加至交易。
- Microsoft 賣方已獲邀參與交易，或已邀請您進行交易。
- Microsoft 卡片處於合作夥伴中心的「接受」或「成功」狀態。

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-當我在交易註冊區段中選取 [+ 新增交易註冊] 按鈕時，收到錯誤訊息。 如何註冊我的交易？

[ **+ 新增交易註冊** ] 按鈕只適用于在 ISV connect 方案中註冊的合作夥伴，在合作夥伴中心內註冊交易，而沒有對應的共同銷售機會。 若要註冊具有共同銷售商機的交易，當交易被標示為「成功」且符合交易註冊的準則時，就會顯示快顯視窗。

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-新增客戶組織是否為必要？

是的，合作夥伴中心內必須加入 [客戶組織](./manage-co-sell-opportunities.md#select-your-customer) 。 首先，請先搜尋客戶的位置。 根據您擁有的詳細資料;您可以指定特定的組建名稱，或只提供城市詳細資料。 組織搜尋將會提取所有符合您輸入名稱的法律實體，如此您就不需要輸入任何位址詳細資料。 系統會根據選取的組織自動填入所有詳細資料。

### <a name="10---are-customer-contact-details-mandatory"></a>10-客戶連絡人詳細資料是否為必要？

取決於您所建立的 [交易類型](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 。 如果您只是共用您的管線，而不需要 Microsoft 銷售組織提供任何協助，您可以選擇不提供客戶連絡人詳細資料。 如果您正在共同銷售，而您積極尋求 Microsoft 賣方的協助，則必須提供客戶連絡人詳細資料。 在合作夥伴中心內建立共同銷售要求之前，您應該先明確同意客戶。

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-我可以在交易中加入多少解決方案？

您最多可以新增50個解決方案 (類似于 PSC 中的「產品」) 進行交易。 與 PSC 不同的是，您可以將解決方案與您自己的共同銷售合格解決方案、Microsoft 第一方 Sku 和其他協力廠商共同銷售合格的解決方案混合。 在合作夥伴中心內，不需要選取或提供任何交易角色。 針對 Microsoft Sku，您可以選擇性地為每個新增至交易的 SKU 新增數量和價格。

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-在建立交易之後，何時會收到 Microsoft 賣方詳細資料的通知？

只有在符合 Microsoft 端上相關賣方角色時所述的確切說明需求之後，才會指派 microsoft 銷售人員。 即使是在指派之後，Microsoft 銷售人員都可以選擇接受或拒絕共同銷售邀請。 只有當賣方接受共同銷售邀請時，才會將交易更新為 Microsoft 賣方連絡人的詳細資料。 用於處理交易的 Microsoft 賣方 SLA 為14天。 這是合作夥伴在交易進入到期狀態之前必須採取的相同 SLA。

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-我可以在哪裡找到商機識別碼？

PSC 的商機識別碼與 PC 中的交易識別碼相同。 當您開啟任何交易時，您可以在交易名稱旁邊找到交易識別碼。

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-我的 PDM 如何取得電腦的存取權？

與 PSC 不同的是，您的 Pdm 小組無法直接存取合作夥伴中心。 有多個選項可啟用這項功能，如下所述。

- OCP 見解-如果 Pdm 小組只是要查看與其相關的交易和進度，則可以使用 OCP 見解入口網站來取得您的組織視圖。 這是內部工具，僅適用于 Pdm 小組。 請注意，您的公司使用者無法使用 OCP 見解。
- 合作夥伴中心內的來賓使用者-您可以 @microsoft.com 在合作夥伴中心內將您的 PDM 帳戶新增為來賓使用者，並指派參考系統管理員角色給他們，讓他們可以根據參考來查看和採取行動。
- 在您的租使用者中建立 [新的使用者](./create-user-accounts-and-set-permissions.md#add-a-new-user) -您可以在自己的租使用者中建立新的使用者，並與 PDM 共用這些詳細資料，讓他們可以在您的帳戶中使用與其他推薦使用者類似的參考來進行流覽和操作。

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>如果您的 PSC 帳戶未與有效的 MPN 相關聯，請尋找正確的 MPN 識別碼

如果您在這裡看到的是「PSC 不正確 MPN 識別碼關聯問題」，則您在正確的位置。 因為下列原因，所以您的帳戶可能已連結至不正確 MPN 識別碼

- 您的公司沒有合作夥伴中心帳戶。
- 當您在內部系統中輸入帳戶的 MPN 識別碼時，您的 PDM 發生錯誤，這些系統會將您的 PSC 帳戶連結至您的合作夥伴中心帳戶， (MPNID) 。
- 您的公司未完成從夥伴成員中心 (PMC) 到 PC 的遷移。

首先，請遵循下列步驟來尋找正確的 MPN 識別碼

- 登入您的合作夥伴中心帳戶
- 使用 [帳戶設定檔](./partner-center-account-setup.md#locate-your-mpn-id) 中提供的指引來找出 MPN 識別碼。

以下螢幕擷取畫面顯示您可以在其中找到合作夥伴中心 MPN 識別碼的確切位置

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="顯示夥伴可在其中找到其 MPN 識別碼之帳戶設定的影像。"  lightbox="images/pscmigration/findingMPNID.png":::

接下來，

- 如果您有 PDM，請要求他們使用來自合作夥伴中心帳戶的正確 MPN 識別碼來修正您的 MPN 識別碼。
- 如果您沒有 PDM，請傳送電子郵件給 PSC 橫幅中提供的電子郵件，其中包含 psc 橫幅中顯示的 PSC 帳戶資訊，以及來自合作夥伴中心帳戶的正確 MPN 識別碼。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>協助您在合作夥伴中心建立和管理交易的資源

如果您尚未閱讀共同銷售說明主題，下列資源將協助您在合作夥伴中心管理交易。

|**進行此動作**   |**請閱讀本文**   |
|-----------------------|:-----------------------|
|瞭解共同銷售商機頁面中的索引標籤和導覽|[導覽共同銷售區段](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|從 D&B 清單中選取客戶組織 |[選取您的客戶](./manage-co-sell-opportunities.md#select-your-customer)|
|修改 [交易詳細資料] 區段中的欄位|[交易詳細資料](./manage-co-sell-opportunities.md#deal-details)|
|將小組成員新增至交易小組|[新增您的員工](./manage-co-sell-opportunities.md#add-team-members)|
|回應共同銷售交易|[管理共同銷售交易](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|註冊您在合作夥伴中心所贏得的交易 |[註冊新交易](./register-deals.md)
|取得參考見解，並瞭解您的參考如何進行 |[推薦深入解析](./referral-insights.md)
|建立和管理商務設定檔|[管理商務設定檔](./create-a-marketing-profile.md)
|管理商務設定檔的潛在客戶 |[管理潛在客戶](./manage-leads.md)|

## <a name="next-steps"></a>下一步


- [合作夥伴銷售可連接至合作夥伴中心活頁簿](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -活頁簿，以透過合作夥伴中心與合作夥伴銷售 Connect 來調整合作夥伴的銷售程式和角色與新的銷售流程。
- [合作夥伴中心共同銷售操作指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -透過合作夥伴中心識別作業模型以管理潛在客戶或共同銷售商機並註冊交易的指引。
- [推薦管理](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) 的簡報：透過合作夥伴中心來視覺化管理潛在客戶和共同銷售商機的逐步指示。
- [在商業 marketplace 中發佈和管理的](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) 逐步解說逐步指示，可讓您透過合作夥伴中心在商用市集中建立、管理及發佈供應專案。