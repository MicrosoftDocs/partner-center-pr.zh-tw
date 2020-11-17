---
title: '從合作夥伴銷售 Connect 遷移 (PSC) '
description: 瞭解 Microsoft 合作夥伴如何可以從合作夥伴銷售 Connect (PSC) 遷移至合作夥伴中心，以及建立或管理 Microsoft 銷售人員所傳送的交易。
ms.topic: article
author: vikramb
ms.author: vikramb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/06/2020
ms.openlocfilehash: 34a18e4a4bf4d5c29265fdf76fae05b4ba16a3bc
ms.sourcegitcommit: 445c7b70943f71cc4b2cb48a327b9dcc1814974d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "94670162"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>合作夥伴中心 (電腦) 共同銷售的指南，適用于從合作夥伴銷售 Connect (PSC 進行遷移的合作夥伴) 

**適用於**

- 合作夥伴中心

**適當的角色**

- 帳戶管理員
- 推薦管理員
- 合作夥伴銷售 Connect (PSC) 賣方
- 合作夥伴銷售 Connect (PSC) 管理員
- 合作夥伴銷售 Connect (PSC) 交易經理

如您所知，在2021年3月31日之後，您的公司將無法存取 PSC。 不過，您可以在合作夥伴中心中找到您想要建立共同銷售交易、管理交易，以及處理由 Microsoft 賣方傳送給您的交易。 不過，也會有一些差異，而下列指引將有助於讓您的轉換合作夥伴中心更順暢且更簡單的進展。

>[!Important]
> 如果您在這裡看到關於遷移的資訊，您就是在正確的位置。 本指南不適用於解決方案評估 (SA) 和 OEM IOT 合作夥伴管理其在 PSC 的交易。

## <a name="before-you-move-things-you-need-to-know"></a>移動之前，您必須知道的事項

### <a name="if-you-are-psc-admin"></a>如果您是 PSC 系統管理員

- 您需要有工作電子郵件才能登入 [合作夥伴中心](https://partner.microsoft.com/)。
- 使用合作夥伴中心 [帳戶管理員](permissions-overview.md)的協助來設定您的帳戶。
- 閱讀這份檔，瞭解如何在合作夥伴中心中共同銷售。
- 在合作夥伴中心中為所有您的 PSC 使用者 (系統管理員、交易管理員和賣方) 角色設定使用者帳戶，並為其指派 [參考系統管理員角色](permissions-overview.md)。

>[!Important]
> 請確定在合作夥伴中心的 MPN 位置清單中有提供 PSC 橫幅中顯示的 MPN 識別碼。 您可以前往中的 [帳戶設定] 和 [[位置](manage-locations.md)] 來確認合作夥伴中心，以尋找與合作夥伴中心帳戶相關聯的所有 MPNs 清單。

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="此圖顯示可供合作夥伴尋找 MPN 識別碼的 PSC 橫幅。":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>如果您是 PSC 交易經理或賣方

- 您需要工作電子郵件才能登入 [合作夥伴中心](https://partner.microsoft.com/)。
- 如果您在 PSC 中使用非工作帳戶，或您的公司電子郵件與合作夥伴公司不同，請洽詢您的 PSC 系統管理員，以取得帳戶設定的說明。
- 如果您的合作夥伴中心帳戶設定已完成，不論您用來登入 PSC 的帳戶是否完整，請洽詢您的 PSC 系統管理員。
- 確認您是否有合作夥伴中心和 [參考] 區段的存取權。
- 閱讀這份檔，瞭解合作夥伴中心中的工作流程和變更。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>作為 PSC 的系統管理員，這些是您的後續步驟

如果您沒有看到 [參考] 索引標籤：

- 貴公司的 [全域管理員](permissions-overview.md) 可以授與您存取 [參考] 索引標籤的許可權。若要尋找您的全域管理員，請從合作夥伴中心右上方的齒輪圖示移至 [夥伴設定]。 在左側導覽列的第二個層級中選取 [使用者管理] 頁面。 在頁面右上方的 [所有使用者] 下拉式清單中按一下，並變更為 [全域管理員]。 該頁面接著會顯示所有全域管理員及其各自的電子郵件識別碼。 請聯絡他們來取得您工作帳戶的「推薦系統管理員」存取權。

  >[!Important]
  > 如果您的角色只管理 PSC 中的使用者，您可以在合作夥伴中心中取得 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company) 角色。 如果您的角色也包含管理共同銷售機會，您應該取得 [推薦系統管理員](permissions-overview.md#manage-referrals) 角色。 此外，請在 PSC 系統管理員中提名一個變更管理領導人，以與合作夥伴中心帳戶管理員合作，而不是由所有 PSC 系統管理員來個別向電腦上的帳戶管理員進行處理。

  :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="顯示 [夥伴設定] 使用者管理頁面中帳戶管理員的影像。":::

- 移至左側流覽窗格中的 [參考] 索引標籤，並檢查您是否可以存取這些頁面。

  >[!Note]
  > 您可能必須登出合作夥伴中心並重新登入，以重新整理您的認證以存取 [參考] 頁面。

## <a name="user-migration"></a>使用者移轉

在合作夥伴中心中設定您的帳戶之後，請使用 [共同銷售商機] 頁面中的 [使用者遷移嚮導]，自動將合作夥伴中心角色指派給公司員工。

>[!Note]
> 使用者遷移只能由公司的 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company) 執行。 如果您沒有帳戶管理員角色，請尋找可協助您使用使用者遷移嚮導來設定使用者帳戶的帳戶管理員。 使用者遷移功能將于2020年11月18日起提供。

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="顯示使用者遷移嚮導的影像。":::

帳戶管理員將會在《推薦指南》旁的 [共同銷售商機] 頁面中，取得 PSC 使用者遷移嚮導連結。 他們可以按一下連結來起始使用者遷移。 這個動作可以執行多次，直到該公司想要遷移的所有使用者都已在合作夥伴中心中指派適當的角色。

使用者遷移表具有下列詳細資料

- 使用者帳戶-員工的電子郵件識別碼
- PSC 合作夥伴帳戶-與 PSC 相關聯的員工帳戶
- PSC 使用者角色-指派給 PSC 的三個角色之一。
- 電腦 MPN 位置-將相關電腦角色提供給使用者的位置。 PSC partner account MPN 可用來在合作夥伴中心中尋找對等的 MPN 位置以指派許可權。 整個組織代表 vOrg MPN 識別碼。
- 電腦使用者角色-員工會根據其 PSC 使用者角色指派角色。 PSC 中的系統管理員將會被指派電腦的推薦系統管理員角色。 賣方將會被指派電腦中的推薦使用者角色。 若要深入瞭解電腦角色以及這些角色的使用者可以在[合作夥伴中心進行](permissions-overview.md#manage-referrals)的動作，請參閱
- 電腦 AAD 租使用者-使用者指派至其中的租使用者合作夥伴中心
- 狀態-遷移狀態有三個可能的狀態
    - 未遷移-使用者未指派任何電腦參考角色
    - 已遷移-使用者已成功遷移，並已指派相關角色，如下表所示
    - 錯誤-因某些錯誤而無法完成遷移

在以下提供解決方案的某些情況下，遷移可能會失敗並導致錯誤

1. PSC 使用者可能使用非工作帳戶。

2. PSC 使用者可能會使用不同于您在合作夥伴中心中所使用之網域的帳戶。

   - 若要解決與案例1和2相關的錯誤，所有這類使用者都必須使用附加至您 Azure AD 租使用者的工作帳戶登入合作夥伴中心。 您的 [全域管理員](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) 可以提供協助。 若要尋找您的全域管理員，請從合作夥伴中心右上方的齒輪圖示移至 [夥伴設定]。 在左側導覽列的第二個層級中，按一下 [使用者管理] 頁面。 在頁面右上方的 [所有使用者] 下拉式清單中按一下，並變更為 [全域管理員]。 全域管理員可以在您的 Azure AD 租使用者中建立新的使用者帳戶，或將來賓使用者存取權指派給其他網域帳戶使用者。 一旦為所有 PSC 交易管理員和使用者設定帳戶之後，他們必須登入合作夥伴中心，移至左側導覽中的 [參考] 索引標籤，然後檢查以確定他們可以看到 [參考] 頁面。

3. 使用者已在合作夥伴中心中指派了參考角色。
    - 您可以從帳戶設定中的 [使用者管理] 頁面，確認使用者的現有角色，並視需要修改相同的角色。

完成使用者遷移之後，請使用下列指導方針來決定遷移策略： 

如果您的公司有 PDM （當您的合作夥伴中心帳戶已設定，而且您的使用者已移動並具有角色和許可權）時，您可以將共同銷售活動移至合作夥伴中心。 通知 PDM 進行切換，而不是等到您的遷移完成期限，讓您的所有新交易都流入合作夥伴中心。

>[!Note]
>一旦您進行此切換之後，您就只能針對 PSC 中現有的主動式交易採取行動。 您不能建立新交易，也不會收到來自 PSC 的 Microsoft 賣方的任何交易。

如果您的公司沒有 PDM，請確定所有使用者都已設定並驗證所有的使用者帳戶。 當您在合作夥伴中心中開始共同銷售時，將會透過電子郵件和 PSC 中的橫幅通知您。 請記住，您仍然需要管理 PSC 中現有的主動式交易。

>[!Important]
>使用中交易不會遷移至電腦。 您必須在2020年12月31日前關閉並註冊交易。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>適用于 PSC 管理員、PSC 交易經理和 PSC 賣方的後續步驟

瞭解如何在合作夥伴中心中共同銷售。
這是很重要的步驟，可協助您準備合作夥伴中心中的共同銷售。 瞭解工作流程和合作夥伴中心中的變更，讓您可以有效地從第一天共同銷售。 一開始請完整閱讀這份檔。 [共同銷售體驗資源庫](https://aka.ms/cosellexperience)也提供一組良好的資源。

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

## <a name="psc-and-partner-center-field-mapping"></a>PSC 和合作夥伴中心欄位對應

本章節會提供 PSC 與合作夥伴中心之間的確切屬性對應。 PSC 中的每個畫面都會與合作夥伴中心共同銷售商機一節中的相關觀點進行比較。 

>[!Note]
>遵循 PSC 螢幕擷取畫面中的黃色氣泡上的數位，在合作夥伴中心中尋找對等的屬性。 紅色的氣泡表示合作夥伴中心中未提供該欄位。

**合作夥伴中心中共同銷售商機的 PSC 首頁和預設觀點**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="顯示夥伴銷售 Connect 首頁之間的欄位對應，以及合作夥伴中心中共同銷售商機的預設觀點的影像。":::

**PSC 格線視圖和合作夥伴中心交易視圖**

- 合作夥伴中心中沒有任何清單視圖，如同 PSC 一樣。  所有交易都會依據客戶資訊和交易類型，以最新的接收或建立日期列出。 預設會選取 view 中的第一筆交易。 以 PSC 資料表格式顯示的大部分值都可在電腦的詳細資料檢視中取得。
- 交易角色不是電腦中的必要欄位。 它不會顯示，也不會在任何工作流程中加以捕捉。 它會根據新增至交易的解決方案，在 Microsoft 賣方端自動衍生。
- 上次修改日期不會顯示在 PC 的 [推薦詳細資料] 頁面上。 夥伴可以使用排序功能，根據上次更新日期來排序交易。

:::image type="content" source="images/pscmigration/gridview.png" alt-text="顯示夥伴銷售 Connect (PSC) 方格視圖與合作夥伴中心交易視圖之間的欄位對應影像。":::

**PSC 和合作夥伴中心的交易詳細資料檢視**

- 合作夥伴可以按一下夥伴交易詳細資料檢視上的 [編輯] 按鈕， (6) 來編輯交易。 一旦按一下 [編輯] 按鈕，所有欄位都會變成可編輯的選項，可以儲存或取消對交易所做的編輯。
- 在合作夥伴中心中，沒有任何選項可關閉重複的交易。
- 合作夥伴中心未提供客戶成果。 所有與客戶互動相關的詳細資料都可以在 PC 的 Notes 區段中更新。
- 預估的解決方案關閉日期僅適用于合作夥伴中心中的 OEM IOT 交易。 任何其他交易類型都不會顯示。
- 電腦不需要授權方案。 它會根據交易中選取的解決方案自動推斷。

>[!Note]
>任何標示為「成功」或「遺失」的交易都無法在 post 之後進行編輯。 將交易移至這些終端機狀態的其中一個時，請務必小心。

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="此圖顯示 Partner Sales Connect (PSC 之間的欄位對應) 交易詳細資料檢視和合作夥伴中心的交易詳細資料檢視。":::

**PSC 的 [新增產品] 視圖和 [新增解決方案] 合作夥伴中心**

:::image type="content" source="images/pscmigration/products.png" alt-text="此圖顯示 Partner Sales Connect (PSC 之間的欄位對應) 新增產品視圖和合作夥伴中心新增方案視圖。":::

**PSC 和合作夥伴中心中的使用者管理**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="此圖顯示 Partner Sales Connect (PSC 之間的欄位對應) 使用者管理首頁和 [帳戶設定] 中的 [合作夥伴中心使用者管理]。":::

**PSC 和合作夥伴中心中的使用者角色指派**

- 與 PSC 管理員同等的角色是合作夥伴中心中的帳戶管理員角色。
- 在共同銷售交易管理的合作夥伴中心中，只有一個角色是參考管理員角色。

:::image type="content" source="images/pscmigration/roles.png" alt-text="顯示夥伴銷售 Connect (PSC) 角色指派視圖和合作夥伴中心角色指派視圖之間的欄位對應影像。":::

**PSC 和合作夥伴中心中的通知**

:::image type="content" source="images/pscmigration/notifications.png" alt-text="顯示夥伴銷售 Connect (PSC) 通知和合作夥伴中心通知觀點之間對應的影像。":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>從 PSC 移至合作夥伴中心常見問題

**季.如果我沒有合作夥伴中心存取權，該怎麼辦？**

您可以聯絡您在 [沒有存取權] 頁面上列出的系統管理員，以取得指派的角色。 在 [參考] 區段下，您將需要「[參考系統管理員](permissions-overview.md#manage-referrals)」角色才能讀取和寫入權限。 如果您只管理商務設定檔，則您需要合作夥伴中心內的「商務設定檔系統管理員」角色。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="顯示合作夥伴中心中無存取體驗的影像。":::

**同比.誰可以授與我合作夥伴中心中 [參考] 區段的存取權？**

您的 [帳戶管理員](permissions-overview.md#manage-mpn-membership-and-your-company) 可以授與您存取 [參考] 索引標籤。若要尋找您的帳戶管理員，請從合作夥伴中心右上方的齒輪圖示移至 [夥伴設定]。 在左側導覽列的第二個層級中，按一下 [使用者管理] 頁面。 按一下頁面右上方的 [所有使用者] 下拉式清單，並變更為 [帳戶管理員]。 頁面接著會顯示所有的帳戶管理員及其各自的電子郵件識別碼。 請聯絡他們來取得您工作帳戶的「推薦系統管理員」存取權。

**三.我們的帳戶的 [+ 新增交易] 按鈕會呈現灰色。我該怎麼做才能開始建立交易？**

只有當您在合作夥伴中心中使用的 MPN 組織未附加共同銷售就緒的解決方案時，才會發生這種情況。 請洽詢您的 PDM 以取得解決方案的 MPN 識別碼，或建立支援票證，其中提及問題「新的交易按鈕在 PSC 遷移後呈現灰色」。

**Q4.我可以將交易指派給組織中的特定人員，例如 PSC 嗎？**

您可以將小組成員指派給特定的交易。 它不會封鎖其他的參考管理員來進行流覽或處理這些交易。 

**Q5.是否有所有指派給我的交易的觀點？**

您可以使用 [我的最愛] 功能，也就是使用者層級索引標籤。您可以將指派給您的所有交易都標示為 [我的最愛]，以快速存取交易。

**Q6.交易是否有唯讀的查看？**

否，在 [參考] 區段中不會顯示交易的唯讀狀態。 所有的參考系統管理員都將擁有所有交易的完整讀取和寫入存取權。

**Q7.如何在將交易變成獲勝之後進行註冊？**

如果交易符合下列準則，我們將會顯示一個快顯視窗，以開始進行 [交易註冊](./register-deals.md)。

- 有一項獎勵符合資格的解決方案附加至交易。
- Microsoft 賣方已獲邀參與交易，或已邀請您進行交易。
- Microsoft 卡片處於合作夥伴中心中的「接受」或「成功」狀態。

**Q8.當我按一下交易登記區段中的 [+ 新增交易註冊] 按鈕時，我收到錯誤訊息。如何註冊我的交易？**

「+ 新交易註冊」僅供在 ISV connect 計畫中註冊的合作夥伴使用，在合作夥伴中心中沒有對應的共同銷售商機來註冊交易。 若要註冊具有共同銷售商機的交易，當交易被標示為「成功」且符合交易註冊的準則時，就會顯示快顯視窗。

**Q9.是否要新增客戶組織的必要專案？**

是的，合作夥伴中心中必須加入 [客戶組織](./manage-co-sell-opportunities.md#select-your-customer) 。 首先，請先搜尋客戶的位置。 根據您擁有的詳細資料;您可以指定特定的組建名稱，或只提供城市詳細資料。 組織搜尋將會提取所有符合您輸入名稱的法律實體，如此您就不需要輸入任何位址詳細資料。 系統會根據選取的組織自動填入所有詳細資料。

**Q10.客戶連絡人詳細資料是否為必要？**

取決於您所建立的 [交易類型](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) 。 如果您只是共用您的管線，而不需要 Microsoft 銷售組織提供任何協助，您可以選擇不提供客戶連絡人詳細資料。 如果您正在共同銷售，而您積極尋求 Microsoft 賣方的協助，則必須提供客戶連絡人詳細資料。 在合作夥伴中心內建立共同銷售要求之前，您應該先明確同意客戶。

**Q11.我可以將多少解決方案新增到交易中？**

您最多可以新增50個解決方案 (類似于 PSC 中的「產品」) 進行交易。 與 PSC 不同的是，您可以將解決方案與您自己的共同銷售合格解決方案、Microsoft 第一方 Sku 和其他協力廠商共同銷售合格的解決方案混合。 在合作夥伴中心內，不需要選取或提供任何交易角色。 針對 Microsoft Sku，您可以選擇性地為每個新增至交易的 SKU 新增數量和價格。

**十二 題。何時會在建立交易之後得知 Microsoft 賣方詳細資料？**

只有在符合 Microsoft 端上相關賣方角色時所述的確切說明需求之後，才會指派 microsoft 銷售人員。 即使是在指派之後，Microsoft 銷售人員都可以選擇接受或拒絕共同銷售邀請。 只有當賣方接受共同銷售邀請時，才會將交易更新為 Microsoft 賣方連絡人的詳細資料。 用於處理交易的 Microsoft 賣方 SLA 為14天。 這是合作夥伴在交易進入到期狀態之前必須採取的相同 SLA。

**Q13.我可以在哪裡找到商機識別碼？**

PSC 的商機識別碼與 PC 中的交易識別碼相同。 當您開啟任何交易時，您可以在交易名稱旁邊找到交易識別碼。

**Q14.我的 PDM 如何取得電腦的存取權？**

您的 Pdm 小組無法直接存取與 PSC 不同的合作夥伴中心。 有多個選項可啟用這項功能，如下所述。

- OCP 見解-如果 Pdm 小組只是要查看與其相關的交易 & 進度，他們可以使用 OCP 見解入口網站來取得您的組織觀點。 這是內部工具，僅適用于 Pdm 小組。 請注意，您的公司使用者無法使用 OCP 見解。
- 合作夥伴中心中的來賓使用者-您可以 @microsoft.com 在合作夥伴中心內將您的 PDM 帳戶新增為來賓使用者，並指派參考系統管理員角色給他們，讓他們可以根據參考來查看和採取行動。
- 在您的租使用者中建立 [新的使用者](./create-user-accounts-and-set-permissions.md#add-a-new-user) -您可以在自己的租使用者中建立新的使用者，並與 PDM 共用這些詳細資料，讓他們可以在您的帳戶中使用與其他推薦使用者類似的參考來進行流覽和操作。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>協助您在合作夥伴中心中建立及管理交易的資源

如果您尚未閱讀共同銷售說明主題，下列資源將協助您在合作夥伴中心管理交易。

|**進行此動作**   |**請閱讀本文**   |
|-----------------------|:-----------------------|
|瞭解共同銷售商機頁面中的索引標籤和導覽|[導覽共同銷售區段](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|從 D&B 清單中選取客戶組織 |[選取您的客戶](./manage-co-sell-opportunities.md#select-your-customer)|
|修改 [交易詳細資料] 區段中的欄位|[交易詳細資料](./manage-co-sell-opportunities.md#deal-details)|
|將小組成員新增至交易小組|[新增您的員工](./manage-co-sell-opportunities.md#add-team-members)|
|回應共同銷售交易|[管理共同銷售交易](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|註冊您在合作夥伴中心中贏得的交易 |[註冊新交易](./register-deals.md)
|取得參考見解，並瞭解您的參考如何進行 |[推薦深入解析](./referral-insights.md)
|建立和管理商務設定檔|[管理商務設定檔](./create-a-marketing-profile.md)
|管理商務設定檔的潛在客戶 |[管理潛在客戶](./manage-leads.md)|

## <a name="next-steps"></a>後續步驟

請遵循下列其他資源：

- [合作夥伴銷售會連接到合作夥伴中心活頁簿](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -活頁簿，以透過合作夥伴中心與合作夥伴銷售連接來將夥伴的銷售流程和角色與新的銷售程式保持一致。
- [合作夥伴中心共同銷售操作指南](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -透過合作夥伴中心來識別作業模型的指引，以管理潛在客戶或共同銷售商機並註冊交易。
- [參考管理](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) 的簡報：透過合作夥伴中心來視覺化管理潛在客戶和共同銷售商機的逐步指示。
- [在商業 marketplace 中發佈和管理的](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) 逐步解說逐步指示，可讓您透過商用市集中的合作夥伴中心來建立、管理及發佈優惠。
