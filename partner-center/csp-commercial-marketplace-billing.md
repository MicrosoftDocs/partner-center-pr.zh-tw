---
title: 商業 marketplace 產品的帳單
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心中從商用 marketplace 購買 ISV SaaS 產品或訂用帳戶的計費方式。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c03ab358b8fb6ab0f23ea5f42b9d35c6f6c2b80c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000422"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>合作夥伴中心中的商業 marketplace 產品和訂閱帳單

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 帳單系統管理員

作為 CSP 方案中的合作夥伴，您可以使用合作夥伴中心，從商業市集中的 ISV 發行者購買以授權為基礎的 SaaS 產品。 這麼做之後，您就可以存取這些購買類型的帳單。 計費週期會在行事曆月份的第一天開始，並于日曆月份的最後一天結束。 發票會在下個月的第8天提供使用。

您可以從合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard/) 或使用 [合作夥伴中心 api](/partner-center/develop/)存取發票。

CSP 方案中的合作夥伴會在購買這些產品時，向客戶購買的 ISV 商用 marketplace 解決方案計費，方法是使用客戶先前購買的 Azure 租使用者) 合作夥伴中心或 Azure 入口網站 (。

>[!NOTE]
>如果客戶使用自己的 Azure AD 租使用者 (而不是從 CSP 方案) 中的合作夥伴購買，客戶也可以選擇直接從 ([Microsoft AppSource](https://appsource.microsoft.com/) 或 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) 購買自己的 ISV SaaS 解決方案。 如果有，則會直接從 Microsoft 收到自己的帳單。 同樣地，如果 CSP 方案中的合作夥伴將 Azure 訂用帳戶或新的 Azure 方案銷售給客戶，並將該租使用者的角色型存取權授與客戶 (或間接轉銷商) 該租使用者的以 [角色為基礎的存取權](/azure/role-based-access-control/built-in-roles) (將任何角色指派 **給) 客戶** (，而不需事先核准或向 CSP 合作夥伴提出通知。 在這些情況下，Microsoft 不會直接通知 CSP 方案中的合作夥伴購買客戶的情況。 不過，Microsoft 提供了選用的 [Azure 監視器](/azure/azure-monitor/platform/alerts-activity-log) 機制，可讓您用來設定 Azure 訂用帳戶上的活動警示或通知。

## <a name="access-billing-information-for-commercial-marketplace-products"></a>存取商用 marketplace 產品的帳單資訊

貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。 若要存取最新的發票和對帳檔案以進行商業 marketplace 產品購買：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)。

2. 從 [合作夥伴中心] 功能表中，選取 [計費]。 

    您會在 [帳單] 頁面頂端看到兩個索引標籤： **週期性** 和 **週期性和一次性購買**。 每個索引標籤可讓您存取不同 marketplace 產品的發票和對帳 (偵察) 檔案：

    - **週期性** 索引標籤：顯示與 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、Power BI Pro 和 Microsoft Azure 相關之訂閱的發票和對帳檔案。

    - **週期性和單次購買** 索引標籤：顯示 azure 方案、azure 保留、軟體和商用 marketplace 產品的發票和對帳檔案。
  
3. 選取 [ **週期性和一次性購買** ] 索引標籤。如果您以不同的貨幣購買客戶的訂用帳戶，您會看到每個貨幣的索引標籤。 您可以執行下列工作： om 這個頁面：

    - 若要查看最新的發票和對帳檔案，請選取 **發票** 或 **對帳**檔案。  (如果您想要的話，也可以使用 [合作夥伴中心 api](/partner-center/develop/)來存取最新的發票和偵察檔案資料。

    - 若要查看先前的發票和偵察檔，請展開下方的 **計費記錄** 資料列。

    - 若要根據最新的帳戶活動隨時檢查估計的帳戶餘額或帳單，請選取 [ **估價** ] 標題下的連結。  

    >[!NOTE]
    > 當我們在每個月的第8天張貼帳單時，會包含稅金及任何其他適用的費用和信用額度。 這表示最終到期金額可能與您在計費期間所看到的數量不同。

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>深入瞭解商用 marketplace 產品的發票和偵察檔案

本節針對從協力廠商 ISV 發行者購買給客戶的商業 marketplace SaaS 訂用帳戶，提供發票和對帳檔案的詳細資訊。

當您從 [合作夥伴中心] 功能表的 [**計費**] 選項中選取 [**週期性和一次性購買**] 時，您可以存取發票和對帳檔案，以取得與 Microsoft (第一方) 和 ISV (協力廠商) 購買相關的費用。 這些購買專案可能與下列專案相關：

- 從 Microsoft 或 ISV 發行者 (的 SaaS 訂閱) 

- Azure 方案

- Azure 保留

- 其他以訂用帳戶為基礎的軟體 (從 Microsoft 或 ISV 發行者) 

這些購買的範例可能包括 SUSE Linux 軟體 (軟體訂用帳戶) 或 Azure ISV SaaS 產品訂用帳戶。

>[!NOTE]
> 如需有關如何讀取發票和偵察檔案的詳細資訊，請參閱 [帳單總覽](billing.md)。

### <a name="tips-on-reading-your-invoice"></a>讀取發票的秘訣

當您從協力廠商 ISV 發行者購買以授權為基礎的 SaaS 產品時，您只會看到發票上的授權費用費用。 即使 ISV 的 SaaS 產品使用 (或取用) 基礎的 Azure 基礎結構資源，也是如此。 這是因為您客戶對 ISV SaaS 產品的 Azure 基礎結構使用費用，會直接向 ISV 收費。  (Isv 會在其各自的 Azure 使用量每日分級的發票對帳檔案中看到相關聯的 Azure 使用量費用。 ) 

您的發票將包含數個頁面：

- **發票的第1頁：** 包含 CSP 方案夥伴帳單詳細資料的摘要總覽。 這包括計費週期的費用摘要、發票號碼、付款條款 (淨60天) ，以及透過網路付款或依檢查付款的計費方法。

- **第2頁 (以及發票的任何後續頁面) ：** 針對第一方的 Microsoft 購買和協力廠商 ISV (以授權為基礎的) 從商用 marketplace 購買的費用詳細資料。 您可以根據每個產品名稱底下的 **發行者** 行，識別 ISV 授權型購買。 相關聯的對帳檔案會針對特定發票費用提供更多帳單詳細資料。

- **發票的最終頁面：** 如果您向 ISV 收取以授權為基礎的 marketplace 產品的費用，此最終頁面將會顯示 ISV 發行者的名稱和位址的更多詳細資料。

### <a name="tips-on-reading-your-reconciliation-file"></a>讀取對帳檔案的秘訣

**週期性和單次採購**對帳檔案包含數個數據行，其中包含對應至發票費用的額外詳細資料。 [ **PublisherName** ] 欄會顯示購買是來自 Microsoft 或協力廠商 ISV 發行者。

對帳檔案中的某些費用可能會以 $0 的成本顯示。 這可能是因為 ISV 「免費試用」供應專案， (通常是30或60天) 或自備授權供應專案。

在免費試用 ISV 提供的案例中：

- 免費試用期涵蓋了 ISV 以授權為基礎的 SaaS 產品在這段時間的成本。 您也不需要支付該 SaaS 產品的相關 Azure 基礎結構使用費用。  但是，如果您使用以使用量為基礎的 ISV 供應專案，則免費試用版不包含基礎 Azure 基礎結構使用量的成本。 在此情況下，Azure 基礎結構使用量費用會出現在個別的 Azure 對帳檔案中。

- 當您為客戶購買並部署 ISV 的免費試用版產品時，ISV 發行者會自動在免費試用版中註冊客戶。 免費試用期間會在 ISV 發行者所定義的期間後自動結束。 在該期間結束之後，將會向客戶收取費用。 這表示，對帳檔案可能會針對符合試用資格的產品顯示兩個數據列：一個會追蹤試用期間，另一個則會追蹤付費供應專案 (這會顯示 $0，直到試用期結束) 為止。 試用期結束後，顯示付費供應專案的資料列就會開始顯示費用。 

如需每個資料行代表什麼的詳細資訊，請參閱 [使用您的對帳](use-the-reconciliation-files.md)檔案。 另請參閱 [合作夥伴中心中的計費類型](billing-different-types.md)

## <a name="next-steps"></a>下一步

- [管理客戶的商業 marketplace 產品](csp-commercial-marketplace-manage.md)
- [瞭解商業 marketplace 產品的支援](csp-commercial-marketplace-support.md)