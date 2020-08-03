---
title: 提供客戶 Microsoft 產品試用
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 讓客戶試用 Microsoft 訂用帳戶產品30天。 在目錄中註冊這些免費試用，就像其他許多線上服務一樣。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecf19a5f519333e40d7f5ae8e982ac8d816e8604
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444904"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>提供客戶30天免費試用版的 Microsoft 產品

**適用於**

- 合作夥伴中心

**適當的角色**
-   全域系統管理員 
-   使用者系統管理員
-   銷售代理人

提供 30 天免費試用，讓客戶接觸全新 Microsoft 產品是個不錯的方式。 就像在許多其他線上服務一樣，您可以註冊類別目錄中的試用版。 所有合作夥伴可以都參與。

## <a name="available-trial-offers"></a>可用的試用版優惠

您可以在 [**客戶**] 頁面上找到所有未完成的試用版供應專案。 此頁面會列出所有訂閱，包括免費試用版和付費訂閱。 （這項功能目前不適用於中國）。

每位客戶都有權取得每個供應專案的免費試用版。 例如，他們可以取得 Microsoft 365 商務版 Standard 的免費試用版，以及一個 Office 365 E3 免費試用版。 不過，如果客戶已擁有該供應專案，他們就無法使用該供應專案的免費試用版。

### <a name="available-products"></a>可用的產品

免費試用版適用于更多的完整和熱門 licesen 型供應專案。 新的試用版供應專案可能會以每月為基礎引進。

合作夥伴可以在合作夥伴中心的 [**定價與**供應專案] 頁面上，找到每月價格清單中的試用版。 試用版供應專案的 [價格清單**次要授權類型**] 欄中會列出「試用版」。

目前，沒有適用于政府供應專案、教育優惠或附加元件供應專案的**免費試用**版。

## <a name="licenses-for-free-trial-offers"></a>免費試用優惠的授權

所有免費試用版都會提供25個授權。 您無法在試用期間變更此號碼。 您無法在免費試用中新增或移除授權。 將試用版轉換成付費訂用帳戶之後，您就可以將額外的授權新增至訂用帳戶。

試用版授權應指派給使用者，方法與指派付費服務授權的方式相同。

## <a name="sign-customers-up-for-trials"></a>為客戶註冊試用版

在合作夥伴中心為您的客戶取得試用版：

1. 從「合作夥伴中心」的「**銷售**」移至「**目錄**」。 
2. 在類別目錄的 **\[帳單週期\]** 中，按一下 **\[試用優惠\]**。 這樣就只允許免費試用出現，並停用其他非免費的優惠。 試用項目將會顯示在類別目錄的 **\[試用\]** 索引標籤中。
3. 選取您想要提供的免費試用，然後選取 **\[提交\]**。 所有試用版的30天內，您不需要支付費用。 您也可以隨時在試用期間將其轉換為付費訂閱。

## <a name="converting-trials-to-paid-subscriptions"></a>將試用版轉換為付費訂閱

免費試用版不會自動轉換成付費訂用帳戶。 30天后，免費試用版必須轉換成付費訂用帳戶，否則將會[過期](#expiring-offers)。 免費試用版無法擴充。

您必須自行將試用版轉換成付費訂用帳戶。 您可以[使用合作夥伴中心](#convert-trials-using-partner-center)或[透過合作夥伴中心 api](#convert-trials-using-apis)來執行此動作。

> [!NOTE]
> 雲端解決方案提供者（CSP）方案的客戶免費試用版無法轉換為另一個程式租使用者（例如 EA、Open 或 MOSP）。

### <a name="convert-trials-using-partner-center"></a>使用合作夥伴中心轉換試用版

您可以使用合作夥伴中心將試用版轉換成付費訂閱：

1. 移至客戶訂閱頁面，並選取免費試用。
2. 選取 **\[將試用版轉換成付費訂閱\]**。
3. 輸入您想要的授權數量與帳單週期，然後選取 **\[套用\]**。
4. 付費訂用帳戶的帳單會在轉換日期開始，而訂用帳戶會從轉換日期 autorenews 12 個月。 

### <a name="convert-trials-using-apis"></a>使用 Api 轉換試用版

您可能需要修改您的 Api，以配合免費試用版轉換為付費訂用帳戶。 如需詳細資訊，請參閱下列開發人員檔：

- [將試用版訂用帳戶轉換成付費版](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [取得試用版轉換方案的清單](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>沒有轉換的試用

並非所有試用版都可以轉換成付費訂閱。 合作夥伴可以使用沒有任何轉換的試用版，直到到期日為止。 合作夥伴可以購買相容的供應專案，以支援與試用版供應專案相同的服務。  這應該在試用版到期之前完成，以確保新購買的供應專案服務與試用版的服務一致。 

|**試用版**   |**相容的小型企業提供**   |**相容的企業提供**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft 小組商業雲端（使用者起始）試用版   |Microsoft 365 商務版 Basic、Microsoft 365 商務版 Standard、Microsoft 365 商務版 Premium   | F3 （先前為 F1）、Office 365 for Enterprise （E1、E3 和 E5）、M365 F1/F3、M365 Enterprise （E3）   |

>[!NOTE]
>以上的供應專案具有類似功能的類似服務方案，但供應專案之間可能會有一些差異。

### <a name="expiring-offers"></a>即將到期的優惠

您不會收到過期供應專案的通知。 您可以使用合作夥伴中心的客戶觀點或藉由查詢 API，來追蹤即將到期的日期。 我們建議您頻繁監視這些日期，以便可以針對接近決策點的客戶採取適當的行動。

試用期到期後，嘗試登入該試用版的客戶會看到到期訊息。 不過，資料會以資料保留標準來儲存。 當您使用相同的服務方案購買新的訂用帳戶之後，就可以從新啟動的訂用帳戶再次存取您的客戶資訊。

## <a name="billing"></a>計費

年度計費和免費試用版在主權雲端和公用雲端中都相同。 唯一的差異在於啟動時可用的試用 Sku。

## <a name="billing-for-free-trials"></a>免費試用的計費

免費試用版可用於每月和每年計費的訂閱。 當您將試用版轉換成付費訂用帳戶時，可以選取計費頻率。

訂用帳戶開始日期是以轉換日期為基礎。 如果將免費試用轉換為年度計費的付費方案，訂閱續約日期將是轉換日期起算的 12 個月後。 如果將免費試用轉換為每月計費的付費方案，訂閱續約日期將是轉換日期之後帳單日期起算的 12 個月後。

### <a name="invoices"></a>發票

您不會看到您的發票或以授權為基礎的對帳檔案中列出免費試用版。 將免費試用轉換成付費訂用帳戶之後，免費試用只會出現在您的發票和以授權為基礎的對帳檔案中。 轉換後的訂用帳戶將會以與任何新訂閱相同的方式來顯示。

### <a name="incentives"></a>獎勵

免費試用版不會影響獎勵。

## <a name="support"></a>支援

如需免費試用版的支援，請透過合作夥伴中心提交服務要求。
