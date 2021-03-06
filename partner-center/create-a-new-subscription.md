---
title: 在合作夥伴中心中建立客戶訂用帳戶
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將您的客戶訂用帳戶銷售給 Microsoft 所發行的產品，以及由協力廠商 Isv 發佈的 SaaS 產品。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 85a40974557817825d58246c2c010c7cf8a6a5e1
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038875"
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

當您在合作夥伴中心中建立客戶的記錄之後，您便可以向他們銷售型錄中產品的訂閱。 這包括 Microsoft 所發佈的產品，以及軟體即服務 (SaaS) 產品，由協力廠商獨立軟體廠商發佈， (Isv) 到 [商用 marketplace](https://azuremarketplace.microsoft.com/marketplace)。

某些供應專案僅限每個客戶一個訂用帳戶。 若要查看受限制的供應項目清單，請造訪合作夥伴中心 [定價與方案] 頁面。

>[!IMPORTANT]
> 作為 CSP 方案中的合作夥伴，您可以從合作夥伴中心中的 ISV 發行者購買 **授權型** 或 **計量** 付費的 SaaS 訂用帳戶。 這表示您可以購買 ISV 發行者提供給您的任何 **授權型** 或 **計量** 付費 SaaS 供應專案，包括您有權存取的 [專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 。 若要購買或管理來自 Isv (的商用 marketplace 供應專案，例如涉及 Azure 應用程式、容器或 Vm 的使用量型供應專案) ，您必須移至 [Azure 入口網站](https://portal.azure.com/)。

## <a name="create-a-new-subscription"></a>建立新的訂用帳戶

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 選取 [訂用帳戶]。 [ **線上服務** ] 索引標籤會顯示所有可用的 Marketplace SaaS 供應專案。

4. 若只要查看特定類型的訂用帳戶，請在可用的篩選中進行選取：
   - **發行者**：選擇 **Microsoft** 以查看 microsoft 提供的供應專案，或查看 isv 所發佈之商業 marketplace 產品的 **合作夥伴** 。
   - **計費類型**：選取您想要使用的訂用帳戶計費類型： **授權** 或 **使用** 方式。 請參閱以 [授權為基礎的帳單](license-based-billing.md) ，以取得可協助您決定每月和每年計費頻率的資訊。
   - **類別**：選擇 [ **企業**]、[ **小型企業**] 或 [ **試用**]。 如需試用訂用帳戶的相關資訊，請參閱[為您的客戶提供 Microsoft 產品試用版](offer-your-customers-trials-of-microsoft-products.md)。

5. 選取您要為客戶購買的產品訂閱。 您看到的產品取決於客戶區段的類型 (教育版、政府版等 ) 和您已套用的篩選。 Marketplace 中顯示的某些供應專案可能不一定會提供給特定的客戶或特定的 CSP 合作夥伴。 這可能是因為：

   - 客戶已經有該產品的訂用帳戶，只允許一個

   - 客戶的訂用帳戶可能已暫止 (在此情況下，您可以重新啟用訂用帳戶，而不是購買新的訂用帳戶。 ) 

   - 針對 ISV SaaS 供應專案，可能有幾個原因無法購買供應專案： ISV 可能不支援客戶的計費國家或地區;ISV 可能選擇不讓供應專案透過 CSP 方案提供;或者，ISV 可能只對特定 CSP 合作夥伴提供 [專屬](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 供應專案。 ISV 供應專案也可能無法透過合作夥伴中心 (例如容器或某些以使用量為基礎的供應專案) 來可交易。  

6. 針對您要新增的每個訂用帳戶，視需要輸入 (的授權數目) 然後選取 [ **新增至購物車**]。

7. 當您完成新增訂用帳戶時，請選取 [ **審核** ] 並檢查您的訂單。

8. 在您審核訂單並準備好購買這些訂用帳戶之後，請選取 [ **購買**]。

9. 購買客戶的訂用帳戶之後，將會發生下列情況：

    - 您可以從該客戶的 [訂用帳戶 **] 頁面選取** 訂用帳戶名稱，以檢查或編輯訂用帳戶。 從這裡開始，您可以選取附加元件授權 (如果有的話)、變更授權數量，或暫停訂用帳戶。

    **ISV SaaS (授權型和計量付費) 訂用帳戶：**
    - 您將會收到 ISV 發行者網站的連結。 此連結應可協助您完成客戶訂用帳戶的部署或帳戶設定。
      
    >[!NOTE]
    > 您或您的客戶都不會收到一封電子郵件，說明如何完成此類型 ISV 訂用帳戶的帳戶設定/布建。 ) 

    - 如果您的訂用帳戶隨附30天的免費試用版，則會自動套用免費試用期限。 作為 CSP 方案中的合作夥伴，您不能在購買給客戶的供應專案上豁免免費試用期。 當免費試用期結束後，訂用帳戶期限將會開始，且訂用帳戶將會轉換為付費狀態。 然後，訂用帳戶會根據相同的排程自動續約。
   
## <a name="update-subscriptions-with-add-ons"></a>更新具有附加元件的訂用帳戶 

若要購買附加元件，客戶必須先具備作用中的基本訂用帳戶。  您無法透過類別目錄來購買附加元件。

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 選擇您要管理的訂閱。

4. 在 [ **狀態** ] 區段下方，是訂用帳戶的可用附加元件清單。  

5. 更新每個必要附加元件的授權數量。 然後，**提交** 您的變更。

透過合作夥伴中心購買附加元件的能力僅適用于直接帳單和間接提供者。
根據基本需求和區域可用性，只會顯示合格的附加元件。 如需定價和供應項目的詳細資訊，請參閱雲端轉銷商供應項目矩陣。  暫止基本訂用帳戶，也會暫止任何相關聯的附加元件。

附加元件的開始日期會與基本訂用帳戶一致，費用會根據收費開始日期和收費結束日期計算，並在第一張發票中按比例收費。 如需其他資訊，請參閱以 [授權為基礎的計費](license-based-billing.md)。


## <a name="suspend-or-cancel-a-subscription"></a>暫停或取消訂用帳戶

如果客戶要求，或是發生未付款或詐騙等情形，合作夥伴可以暫停或取消訂閱。

### <a name="suspend-a-subscription"></a>暫停訂閱

當您將訂閱的狀態變更為 **\[已暫停\]** 時，使用者就無法登入或存取服務。

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 選擇您要管理的訂閱。

4. 在 [狀態]  區段中，選擇 [暫止]  。 然後，**提交** 您的變更。

5. 所有的資料將被刪除，除非訂用帳戶在 90 日内重新啟用，或 90 天加上開啟帳戶的時間和第一個計費期間之間的天數 (最多 120 天)。

當您在暫停訂用帳戶時，您在 [已暫停] 按鈕下方看到的日期會顯示該訂用帳戶何時會自動到期 (如果您沒有重新啟用的話)。 

### <a name="cancel-a-subscription"></a>取消訂用帳戶

您可以選擇從合作夥伴中心 [商用 marketplace](csp-commercial-marketplace-overview.md)中的協力廠商 ISV 發行者，取消以授權為基礎的 SaaS 訂閱。 只要您在取消期間內取消，就會收到完整退款。

針對 ISV 優惠，每月計費：

- 如果您在下訂單後取消了24小時以外的時間，您將會在下一張發票上收到完整的信用額度。

- 如果您在下一次訂單之後取消超過24小時，則會排程在續約時進行取消。

針對每年計費的優惠：

- 如果您在下訂單後取消了14天，您將會在下一張發票上收到完整的信用額度。

- 如果您在下一次訂單後取消超過14天，取消將會排定在續約時進行。

在這些期間結束之後，您就不會再看到取消訂用帳戶的選項。

> [!NOTE]
> 使用虛擬機器或容器的使用量型和計量付費、協力廠商 ISV 服務 (，例如) 不符合退貨資格。 以使用量為基礎的服務可以取消布建為取消方法。 由於費用是在使用之後計費，因此這些服務不符合退款資格。

若要取消 ISV 發行者提供的授權型 SaaS 訂用帳戶，請執行下列動作：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 找出您要取消的訂用帳戶。

4. 在 [ **狀態** ] 資料行中，選取 [ **取消**]。 然後，**提交** 您的變更。

5. 如果出現對話方塊，請填寫任何相關的詳細資料，然後選取 [ **提交**]。

6. 若要確認取消，請選取 **[是，取消]**。

> [!NOTE]
> 您也可以選擇使用 Api 取消 Azure Marketplace 的訂用帳戶。 若要這樣做，請參閱 [取消 Azure Marketplace 訂](/partner-center/develop/cancel-an-azure-marketplace-subscription)用帳戶。

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>選擇是否要自動續訂商業市集訂用帳戶

根據預設，使用中的訂閱會設定為在訂閱期間到期時自動續訂。 針對 [商用 marketplace 產品的訂閱](csp-commercial-marketplace-overview.md)，您可以選擇性地選擇不自動更新訂用帳戶。

若要停止有效的商業 marketplace 訂用帳戶，使其無法自動更新：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。

3. 選取 **訂用帳戶** 。 這會列出您為客戶購買的任何授權型訂閱。

4. 在 [ **訂** 用帳戶] 資料行中，選取您要修改的訂用帳戶。

5. 在 [訂閱詳細資料] 頁面中，找出 [ **狀態** ] 區段，並取消核取 [ **自動更新** ] 方塊。

6. 選取 [提交]。

## <a name="next-steps"></a>後續步驟

- [為您的客戶購買商業市集產品](csp-commercial-marketplace-purchase.md)

- [為您的客戶管理商業 marketplace 產品](csp-commercial-marketplace-manage.md)

- [商務 Marketplace 概觀](csp-commercial-marketplace-overview.md)