---
title: Azure 方案計費 - 發票和對帳檔案
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何存取及了解與 Azure 方案計費相關的發票和對帳檔案結構。
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: fa1d1298f0fd3650bdaa4e6fc6b602844ac199c4
ms.sourcegitcommit: 83f9c114910282dc87b3ec22d59a8b24b1d6b368
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/01/2020
ms.locfileid: "84262872"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>CSP 中的新商務體驗 - Azure 計費 

**適當的角色：**

- 系統管理代理人
- 帳單系統管理員
- 全域系統管理員

Azure 方案下的計費，是藉由使用一致的單一計費日期和以行事曆月份為基礎的計費期間，簡化的計費體驗。

## <a name="summary-of-billing-essentials"></a>計費基本資訊摘要

- **發票日期**：發票和對帳檔案在合作夥伴中心儀表板/API 中將於 8 日 (午夜 UTC) 提供。

- **發票計費期間**：發票計費期間會對應到行事曆月份，例如，10/1-10/31、11/1-11/30。

- **收費服務期間**：收費將會與行事曆月份一致。 例如，如果計費合作夥伴在 10/15 透過 Azure 方案新增 Azure 服務，而客戶在 10/15 開始使用 Azure 服務，則計費合作夥伴會在 11/8 收到 10/15 - 10/31 服務期間客戶使用的發票/對帳檔案。 下一個月份的發票會在 12/8 產生，其中包含 11/1- 11/31 服務期間的所有費用。

- **發票付款期限**：淨 60 天。

- **發票貨幣**：合作夥伴會繼續以客戶國家/地區的指派貨幣來計費。 例如，如果計費合作夥伴是在愛爾蘭，而客戶是在英國、挪威和德國，則計費合作夥伴將會收到 GBP、NOK 和 EUR 發票/對帳檔案。

- **合作夥伴獎勵**：從發票月份結束起算 45 天支付。

## <a name="access-your-invoices-and-reconciliation-files"></a>存取您的發票和對帳檔案

貴公司的全域管理員或計費管理員將會在發票已準備好可供檢視時，收到電子郵件。 

**若要存取發票和對帳檔案**

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/en-us/dashboard/)。

2. 從 [合作夥伴中心] 功能表中，選取 [計費]。

3. 選取 [週期性] 和 [一次性] 的索引標籤，以及您感興趣的貨幣。

![計費](images/azure/billing3.png)

4. 選取 [發票] 或 [對帳檔案]。  

若要檢視歷程記錄發票和對帳檔案，請展開下方的計費歷程記錄資料列。


## <a name="understanding-usage-data"></a>瞭解使用量資料 

1. Azure 方案是使用量的根或最上層容器。 所有使用量都會繫結回單一 Azure 方案。

2. 在方案中，將會有一或多個 Azure 訂用帳戶。 這些是用於資源管理和部署的容器。 

3. 在訂用帳戶內，資源群組會新增至群組資源。 每個資源都會部署到一個資源群組。 

4. 資源的範例包括虛擬機器和儲存體帳戶。 

5. 資源發出計量：計量是資源耗用量的度量，一個資源可能會發出多個計量的使用量。 計量是以 ProductID、SKUID 和 AvailabilityID 識別。 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>訂用帳戶資源群組和計量的階層

**Azure 帳戶 (租用戶)**

- 訂用帳戶 A
    - 資源群組 1
        - 虛擬機器 (資源)
            - 計算計量
        - 虛擬網路 (資源)
            - 沒有計費計量

    - 資源群組 2
        - 虛擬機器 (資源)
            - 電腦計量
        - 進階 SSD 受控磁碟 (資源)
            - 儲存體容量計量
            - 儲存體作業計量

- 訂用帳戶 B - 資源群組 1 - Azure SQL (資源) - DTU 計量 - VPN 閘道 (資源) - VPN 閘道計量

    - 資源群組 2
        - 虛擬網路介面 (資源)
            - 沒有計費計量

## <a name="read-the-invoice"></a>讀取發票

1. 發票在每個月的第八天之後才可取得。

2. 合作夥伴有 60 天的時間匯款。

3. 計費期間會涵蓋指定的行事曆月份，例如，10/1-10/31。

4. 費用是調整淨額 (金額是「受控服務的合作夥伴所獲得信用點數」淨額)。

5. 如需其他計費詳細資料，請參閱發票對帳檔案和每日評等使用量檔案。

![發票](images/azure/invoice1.png)

## <a name="read-the-invoice-reconciliation-file"></a>讀取發票對帳檔案

1. 在對帳檔案中，每個 Azure 方案和計量組合最多可以有兩個計費行。

2. 如果計量符合整個行事曆月份任何類型折扣或信用點數的資格 (例如階層折扣或受控服務的合作夥伴所獲得信用點數)，則對帳檔案只會包含一個計費行。 **PriceAdjusmentDescription** 資料行會參考折扣或獲得的信用點數。

3. 如果沒有符合折扣或合作夥伴所獲得信用點數的特定計量資源，則對帳檔案只會包含一個計費行，而有效單價會是零售價格 (這就是單價)。

4. 如果計量或任何發出該計量的資源符合部分月份**受控服務的合作夥伴所獲得信用點數**的資格，則對帳檔案會包含兩個計費行。 一行代表計量合格的天數，而第二行則代表計量不合格的天數。 

## <a name="read-the-daily-usage-file"></a>讀取每日使用量檔案

- Azure 方案下的訂用帳戶計量會進行分級，並以每天為基礎進行累計。 

- **受控服務的合作夥伴所獲得信用點數**是以每天為基礎進行判斷和套用。

- 每個訂用帳戶計量都會有一個資料列，用於月份中每天的使用量。

- 在下列範例中：

  - 7/1 - 7/3 的計量符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。

  - 7/4 - 7/7 的計量不符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。

  - 7/8 - 7/31 的計量符合**受控服務的合作夥伴所獲得信用點數**的資格 (請注意，有效單價是零售價)。

![recon2](images/azure/pecfinal.png) 

## <a name="invoice-in-customer-currency"></a>以客戶貨幣表示的發票 

透過 Azure 方案的 Azure 服務會以美元計價，並以客戶國家/地區指派貨幣來計費。 如果計費貨幣不是美元，則使用的外幣匯率 (FX) 費率會顯示在發票的最後一頁。 FX 費率是每月決定，並套用至下列發票。 如需國家/地區貨幣的完整清單，請參閱[新的商務供應項目國家/地區可用性和客戶貨幣對照表](https://go.microsoft.com/fwlink/?linkid=2112354)。 

Microsoft 將使用 Thomson Reuters，來判斷用來決定定價貨幣至計費貨幣轉換的 FX 費率。 FX 費率會重新整理，並在其套用當月第一天的前一天可供使用。

**範例**：服務期間 8 月 1 日 - 8 月 31 日的使用費用，會使用在 7 月 31 日發佈的 FX 費率來計費。 這些費用會出現在 9 月發票上，而 FX 費率會在發票的最後一頁上註明。 

 
## <a name="azure-reservations"></a>Azure Reservations 

如果透過 Azure 方案購買 [Azure Reservations](https://docs.microsoft.com/partner-center/azure-reservations)，一開始就只能在合作夥伴中心選擇一次性計費。 在 Azure 入口網站上可以使用每月計費。 合作夥伴中心將於日後提供每月計費。 

## <a name="azure-spending"></a>Azure 費用 

現有的 Azure 消費經驗已更新，可支援合作夥伴中心內的新 Azure 方案計費。 這讓合作夥伴可以：

- 查看、管理及接收針對客戶層級設定的預算警示 

- 查看 Azure 方案中的預估支出總計 (依資源和計量層級細分)

因為透過 Azure 方案的 Azure 服務計費模式是後付款使用方式，所以若要避免帳單超出預期，合作夥伴可以套用每月預算，並追蹤使用量的百分比。 預算可以一次套用至一個客戶或多個客戶。 

![Azure 費用](images/azure/azurespend.png)

**詳細資訊**

-  合作夥伴所獲得信用點數 (PEC) 的計算方式，位於可透過合作夥伴中心[儀表板](https://partner.microsoft.com/en-us/dashboard/)取得的價目表 (需要登入)。 
   
-  [購買 Azure 方案](purchase-azure-plan.md)

-  [CSP 中新商務體驗的價目表](azure-plan-price-list.md)
