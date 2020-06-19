---
title: 在合作夥伴中心建立客戶訂用帳戶
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何向 Microsoft 所發佈的產品以及由協力廠商 Isv 發佈的 SaaS 產品，銷售您的客戶訂用帳戶。
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 訂用帳戶，建立新的訂用帳戶，暫停，取消，暫停，暫停，SaaS，授權，ISV，協力廠商
ms.localizationpriority: medium
ms.openlocfilehash: 3588fb8408ef3c190813691d42331753ac531a8f
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991490"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>建立、暫停或取消客戶訂閱

**適用於**

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心
- 雲端解決方案提供者合作夥伴

**適當的角色**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員
- 技術服務代理人
- 銷售代理人

當您在合作夥伴中心中建立客戶的記錄之後，您便可以向他們銷售型錄中產品的訂閱。 這包括由 Microsoft 發佈的產品，以及由協力廠商獨立軟體廠商（Isv）發佈到[商業 marketplace](https://azuremarketplace.microsoft.com/marketplace)的軟體即服務（SaaS）產品。

某些供應專案僅限每個客戶有一個訂用帳戶。 若要查看受限制的供應項目清單，請造訪合作夥伴中心 [定價與方案] 頁面。

> [!IMPORTANT]
> 身為 CSP 計畫的合作夥伴，您只能從合作夥伴中心內的 ISV 發行者購買以**授權為基礎**的 SaaS 訂閱。 這表示您可以購買 ISV 發行者已提供給您的任何**授權型**SaaS 供應專案，包括您有權存取的[專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。 若要向 Isv 購買或管理其他的商業 marketplace 供應專案（例如，以**使用量為基礎**、計量付費或涉及 Azure 應用程式、容器或 vm 的耗用量型供應專案），您必須移至[azure 管理入口網站](https://portal.azure.com/)。 如需詳細資訊，請參閱[購買商用 marketplace 產品](csp-commercial-marketplace-purchase.md)。

## <a name="create-a-new-subscription"></a>建立新的訂用帳戶

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。

3. 選取 [訂用帳戶]****。 [**線上服務**] 索引標籤會顯示所有可用的 Marketplace SaaS 供應專案。

4. 若只要查看特定類型的訂用帳戶，請在可用的篩選中進行選取：
   - **發行者**：選擇 [ **microsoft** ] 僅查看 microsoft 或**合作夥伴**提供的供應專案，以查看 isv 所發佈的商業 marketplace 產品。
   - **計費類型**：選取您想要使用的訂用帳戶計費類型： [**授權**] 或 [**使用**方式]。 如需可協助您在每月與年度計費頻率之間做選擇的詳細資訊，請參閱[新計費功能的常見問題集](faq-about-new-billing-features.md)。
   - **類別**：選擇 [**企業**]、[**小型企業**] 或 [**試用**]。 如需試用訂用帳戶的相關資訊，請參閱[為您的客戶提供 Microsoft 產品試用版](offer-your-customers-trials-of-microsoft-products.md)。

5. 選取您想要為客戶購買的產品訂閱。 您看到的產品取決於客戶區段的類型（教育、政府等），以及您已套用的篩選。 Marketplace 上顯示的某些供應專案可能不一定會提供給特定的客戶或特定的 CSP 合作夥伴。 這可能是因為：

   - 客戶已有該產品的訂用帳戶，且只允許一個

   - 客戶的訂用帳戶可能已暫停（在此情況下，您可以重新啟用訂用帳戶，而不是購買新的）。

   - 針對 ISV SaaS 供應專案，可能有幾個原因導致無法購買供應專案： ISV 可能不支援客戶的帳單國家或地區;ISV 可能選擇不透過 CSP 計畫提供供應專案;或者，ISV 可能只對特定 CSP 合作夥伴提供[專屬](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)供應專案。 ISV 供應專案可能也不會透過合作夥伴中心 transactable （例如，容器或某些以使用量為基礎的優惠）。  

6. 針對您想要新增的每個訂用帳戶，輸入授權數目（如有需要），然後選取 [**新增至購物車**]。

7. 當您完成新增訂閱之後，請選取 [**審查**]，並檢查您的訂單。

8. 當您已審核訂單並準備好購買這些訂閱之後，請選取 [**購買**]。

9. 購買客戶的訂用帳戶之後，將會發生下列情況：

    - 您可以從該客戶的**訂閱**頁面中選取訂用帳戶名稱，以檢查或編輯訂閱。 從這裡開始，您可以選取附加元件授權 (如果有的話)、變更授權數量，或暫停訂用帳戶。

    **針對 ISV SaaS （以授權為基礎）的訂用帳戶：**
    - 您會收到「ISV 發行者」網站的連結。 此連結應該可協助您完成客戶訂閱的部署或帳戶設定。
      
    >[!NOTE]
    > 您或您的客戶都不會收到一封電子郵件，說明如何針對此類型的 ISV 訂閱完成帳戶設定/布建。）

    - 如果您的訂用帳戶隨附30天免費試用版，將會自動套用免費試用期限。 身為 CSP 計畫的合作夥伴，您無法在購買給客戶的供應專案上放棄免費試用期。 一旦免費試用期結束後，訂用帳戶期限就會開始，且訂用帳戶將會轉換成付費狀態。 然後，訂用帳戶會根據相同的排程進行 autorenew。

## <a name="suspend-or-cancel-a-subscription"></a>暫停或取消訂用帳戶

如果客戶要求，或是發生未付款或詐騙等情形，合作夥伴可以暫停或取消訂閱。

### <a name="suspend-a-subscription"></a>暫停訂閱

當您將訂閱的狀態變更為 **\[已暫停\]** 時，使用者就無法登入或存取服務。

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。

3. 選擇您要管理的訂閱。

4. 在 [狀態]  區段中，選擇 [暫止]  。 然後，**提交**您的變更。

5. 所有的資料將被刪除，除非訂用帳戶在 90 日内重新啟用，或 90 天加上開啟帳戶的時間和第一個計費期間之間的天數 (最多 120 天)。

當您在暫停訂用帳戶時，您在 [已暫停]**** 按鈕下方看到的日期會顯示該訂用帳戶何時會自動到期 (如果您沒有重新啟用的話)。 如需詳細資訊，請參閱[關於新帳單功能的常見問題](faq-about-new-billing-features.md)。

### <a name="cancel-a-subscription"></a>取消訂用帳戶

您可以選擇在合作夥伴中心的[商業市場](csp-commercial-marketplace-overview.md)中，取消協力廠商 ISV 發行者的授權型 SaaS 訂閱。 只要您在取消期間取消，您就會收到完整退款。

針對每月計費的 ISV 優惠：

- 如果您在下一次訂單後取消少於24小時，您會在下一張發票上收到完整的點數。

- 如果您在下一次訂單後於24小時後取消，則會排程在續約時進行取消。

針對每年計費的優惠：

- 如果您在下一次訂單後取消少於14天，您將會在下一張發票上收到完整的點數。

- 如果您在下一次訂單後的14天后取消，將會排定在續約時進行取消。

在這些期間結束之後，您就不會再看到取消訂用帳戶的選項。

> [!NOTE]
> 以使用量為基礎和計量付費，協力廠商 ISV 服務（例如，使用虛擬機器或容器）並不符合退貨資格。 以使用方式為基礎的服務可以解除布建為取消方法。 因為費用會在使用後計費，所以這些服務不符合退款資格。

若要取消 ISV 發行者提供的授權型 SaaS 訂用帳戶，請執行下列動作：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。

3. 找出您想要取消的訂用帳戶。

4. 在 [**狀態**] 欄中，選取 [**取消**]。 然後，**提交**您的變更。

5. 如果出現對話方塊，請填寫任何相關的詳細資料，然後選取 [**提交**]。

6. 若要確認取消，請選取 **[是，取消]**。

> [!NOTE]
> 您也可以選擇使用 Api 取消 Azure Marketplace 訂用帳戶。 若要這麼做，請參閱[取消 Azure Marketplace 訂](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)用帳戶。

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>選擇是否要自動續訂商業市集訂用帳戶

根據預設，使用中的訂用帳戶會設定為在訂用帳戶期間到期時自動續訂。 對於[商業市集產品的訂用帳戶](csp-commercial-marketplace-overview.md)，您可以選擇不自動更新訂用帳戶。

若要停止有效的商用 marketplace 訂用帳戶，使其無法自動續約：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。

3. 選取 **訂用帳戶** 。 這會列出您已為客戶購買的任何授權型訂閱。

4. 在 [**訂**用帳戶] 欄位中，選取您想要修改的訂用帳戶。

5. 在 [訂閱詳細資料] 頁面中，找出 [**狀態**] 區段，然後取消核取 [**自動續約**] 方塊。

6. 選取 [提交]。

## <a name="next-steps"></a>後續步驟

- [為您的客戶購買商業市集產品](csp-commercial-marketplace-purchase.md)

- [為您的客戶管理商業 marketplace 產品](csp-commercial-marketplace-manage.md)

- [商務 Marketplace 概觀](csp-commercial-marketplace-overview.md)
