---
title: 商業 marketplace 產品的帳單
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解在合作夥伴中心內從商業 marketplace 購買客戶的 ISV SaaS 產品或訂用帳戶的計費方式。
author: LauraBrenner
ms.author: labrenne
keywords: 訂用帳戶，產品，採購，Marketplace，協力廠商，ISV，帳單，發票，調整，偵察檔案
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ee8b7850708d5e04f07ab41965b4c4659b377ba
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908117"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>合作夥伴中心內的商業 marketplace 產品和訂用帳戶計費

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 帳單系統管理員

身為 CSP 計畫的合作夥伴，您可以使用合作夥伴中心，從商用 marketplace 中的 ISV 發行者購買授權型 SaaS 產品。 這麼做之後，您就可以存取這些購買類型的帳單。 計費週期會在日曆月份的第一天開始，並在日曆月份的最後一天結束。 在下個月的第8天可取得發票。

您可以從合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)或使用[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/)來存取發票。

CSP 計畫中的合作夥伴會針對客戶購買的 ISV 商業 marketplace 解決方案計費，其方式是從合作夥伴中心或 Azure 入口網站購買這些產品（使用客戶先前的 CSP 購買 Azure 租使用者）。

>[!NOTE]
>如果客戶使用自己的 Azure AD 租使用者（而不是從 CSP 方案中的合作夥伴購買），客戶也可以選擇直接從（[Microsoft AppSource](https://appsource.microsoft.com/)或[Azure Marketplace](https://azuremarketplace.microsoft.com/)）購買自己的 ISV SaaS 解決方案。 如果他們這麼做，他們會直接從 Microsoft 收到自己的帳單。 同樣地，如果 CSP 方案中的合作夥伴將 Azure 訂用帳戶或新的 Azure 方案銷售給客戶，並將該租使用者的[角色型存取權](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)授與客戶（或間接轉銷**商），** 則該客戶（或間接轉銷商）也可以購買商業 marketplace 供應專案，而不需要事先核准或通知給 CSP 合作夥伴。 在這些情況下，Microsoft 不會直接向 CSP 計畫中的合作夥伴通知其客戶所進行的購買。 不過，Microsoft 會提供選擇性的[Azure 監視器](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log)機制，讓您可以用來設定 Azure 訂用帳戶上活動的警示或通知。

## <a name="access-billing-information-for-commercial-marketplace-products"></a>存取商業 marketplace 產品的帳單資訊

貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。 若要存取商業 marketplace 產品購買的最新發票和對帳檔案：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard/)。

2. 從 [合作夥伴中心] 功能表中，選取 [計費]  。 

    您會在 [帳單] 頁面頂端看到兩個索引標籤： [**週期性**] 和 [**週期性] 和**[單次購買]。 每個索引標籤都可讓您存取不同 marketplace 產品的發票和對帳（偵察）檔案：

    - **週期性**索引標籤：顯示與 Office 365、Microsoft 365、Dynamics 365、Azure Active Directory、PowerBI Pro 和 Microsoft Azure 相關之訂閱的發票和對帳檔案。

    - **週期性和一次性購買**索引標籤：顯示 azure 方案、azure 保留、軟體和商用 marketplace 產品的發票和對帳檔案。
  
3. 選取 [**週期性和一次性購買**] 索引標籤。如果您以不同的貨幣購買客戶的訂用帳戶，您會看到每個貨幣的索引標籤。 您可以進行一些 fr： om 這個頁面：

    - 若要查看最新的發票和對帳檔案，請選取 [**發票**或**對帳**檔案]。 （如果您想要的話，也可以使用[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/)來存取最新的發票和偵察檔案資料。

    - 若要查看先前的發票和偵察檔案，請展開下方的 [**帳單記錄**] 列。

    - 若要根據最新的帳戶活動，隨時檢查預估的帳戶餘額或帳單，請選取 [**估價**] 標題下方的連結。  

    >[!NOTE]
    > 當我們在當月第8天張貼帳單時，將會包含稅金和任何其他適用的費用和信用額度。 這表示最終到期金額可能與您在計費期間所看到的數量不同。

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>深入瞭解商業 marketplace 產品的發票和偵察檔

本節針對向協力廠商 ISV 發行者購買的客戶提供的商用 marketplace SaaS 訂閱的發票和對帳檔案的詳細資訊。

當您從 [合作夥伴中心] 功能表中的 [**計費**] 選項選取 [**週期性] 和**[單次購買] 時，您會取得發票和對帳檔案的存取權，以取得與 Microsoft （第一方）和 ISV （協力廠商）購買相關的費用。 這些購買專案可能會與下列專案相關聯：

- SaaS 訂閱（來自 Microsoft 或 ISV 發行者）

- Azure 方案

- Azure Reservations

- 其他以訂閱為基礎的軟體（來自 Microsoft 或 ISV 發行者）

這些購買的範例可能包括 SUSE Linux 軟體（軟體訂用帳戶）或 Azure ISV SaaS 產品訂用帳戶。

>[!NOTE]
> 如需有關如何讀取發票和偵察檔的詳細資訊，請參閱[計費總覽](billing.md)。

### <a name="tips-on-reading-your-invoice"></a>閱讀發票的秘訣

當您從協力廠商 ISV 發行者購買以授權為基礎的 SaaS 產品時，您只會看到發票上的授權費用費用。 即使 ISV 的 SaaS 產品使用（或使用）基礎 Azure 基礎結構資源，也是如此。 這是因為 ISV 的 SaaS 產品的客戶 Azure 基礎結構使用量費用，會直接向 ISV 收費。 （Isv 會在自己的 Azure 使用量每日評分的發票對帳檔案中看到相關聯的 Azure 耗用量費用。）

您的發票將包含數個頁面：

- **發票的第1頁：** 包含 CSP 計畫合作夥伴帳單詳細資料的摘要總覽。 這包括計費期間的費用摘要、發票編號、付款條款（Net 60 天），以及按網路或核取的計費付款方法。

- **發票的第2頁（以及任何後續頁面）：** 從商用 marketplace 購買第一方的 Microsoft 購買和協力廠商 ISV （以授權為基礎）的費用。 您可以根據每個產品名稱底下的**發行者**行，識別以 ISV 授權為基礎的購買專案。 相關聯的對帳檔案會針對特定發票費用提供更多計費詳細資料。

- **發票的最後一頁：** 如果您向 ISV 收取以授權為基礎的 marketplace 產品費用，此最終頁面將會顯示 ISV 發行者名稱和位址的更多詳細資料。

### <a name="tips-on-reading-your-reconciliation-file"></a>讀取對帳檔案的秘訣

**週期性和一次性採購**對帳檔案包含數個數據行，其中含有對應至發票費用的其他詳細資料。 [ **PublisherName** ] 欄會顯示購買是來自 Microsoft 或協力廠商 ISV 發行者。

您的對帳檔案中的某些費用可能會顯示為 $0 的成本。 這可能是因為 ISV 「免費試用」供應專案（通常是30或60天）或自備授權供應專案。

在免費試用 ISV 提供的案例中：

- 免費試用期間涵蓋了 ISV 以授權為基礎的 SaaS 產品在這段時間內的成本。 該 SaaS 產品的相關 Azure 基礎結構使用也不會向您收取費用。  不過，如果您使用以使用量為基礎的 ISV 供應專案，免費試用不會包含基礎 Azure 基礎結構使用量的成本。 在此情況下，Azure 基礎結構使用量費用將會出現在個別的 Azure 對帳檔案中。

- 當您為客戶購買及部署 ISV 的免費試用版合格產品時，ISV 發行者會自動在免費試用版中註冊客戶。 免費試用期間會在 ISV 發行者定義的期間之後自動結束。 一段期間結束後，就會向客戶收取費用。 這表示，對帳檔案可能會顯示兩個適用于試用版產品的資料列：一個追蹤試用期，另一個則追蹤付費供應專案（在試用期結束之前，會顯示 $0 的成本）。 試用期結束後，顯示付費供應專案的資料列就會開始顯示費用。 

如需每個資料行所代表之內容的詳細資訊，請參閱[使用您的對帳](use-the-reconciliation-files.md)檔案。 另請參閱[合作夥伴中心的帳單類型](billing-different-types.md)

## <a name="next-steps"></a>後續步驟

- [管理客戶的商業 marketplace 產品](csp-commercial-marketplace-manage.md)
- [瞭解商業 marketplace 產品的支援](csp-commercial-marketplace-support.md)
