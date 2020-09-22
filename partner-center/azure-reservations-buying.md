---
title: 為客戶購買 Microsoft Azure 保留
description: 瞭解如何在合作夥伴中心中代表您的客戶購買或購買 Azure 保留。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 655bd48df616b26b842d5f99960d6b6ad2e75f1f
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000262"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>在合作夥伴中心中代表客戶購買 Microsoft Azure 保留

**適用於**

- 合作夥伴中心
- Microsoft Azure 入口網站
- 雲端解決方案提供者中的合作夥伴

**適當的角色**

- 系統管理代理人
- 全域系統管理員
- 技術服務代理人
- 銷售代理人
- 使用者管理系統管理員
 
> [!NOTE]
> 本文僅適用于雲端解決方案提供者 (CSP) 計畫中的合作夥伴。 使用其他類型訂用帳戶的客戶 (例如隨用隨付、個別、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀 [此 Azure 保留檔](/azure/cost-management-billing/reservations)。

## <a name="before-you-begin"></a>開始之前

請先參閱下列重要資訊，再代表客戶購買 Azure 保留。  (您想要讓客戶能夠從您購買的先前 Azure 訂用帳戶購買自己的 Azure 保留嗎？ 請參閱 [授與客戶購買自己的 Azure 保留的許可權](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)。 ) 

- 如果您的客戶登入新的 Microsoft 客戶合約， (請 [確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)) ，您必須在 azure 方案下購買 azure 保留。 如需詳細資訊，請參閱 [購買 Azure 方案](purchase-azure-plan.md)。

- 在您代表客戶購買保留區之前，客戶必須已擁有有效的 Azure 訂閱
  
- 軟體訂用帳戶成本（例如 SQL Database 或 SUSE Linux 軟體）不包含在 Azure 保留價格中

- 除非您的地點是巴西，否則 Microsoft 的商業價格不包含稅金。 如果您的地點是巴西，則商業價格會包含適當的稅額

- 銷售人員和技術支援中心需能代表客戶明確的存取 Azure 訂閱，以便在 Azure 入口網站與檔案支援要求中購買或管理訂閱，包括換貨與退款  

- 如果您是間接提供者，而且您透過 Azure 入口網站購買 Azure 保留專案，則會從您選取的 Azure CSP 訂用帳戶繼承記錄 (間接轉銷商) 的夥伴。

- Azure 保留的記錄夥伴無法在購買後變更。 您可以取消現有的保留，並向新的記錄夥伴購買新的保留。

- 如果客戶想將 Azure 訂閱從直接或 EA 轉移至雲端解決方案提供者，保留區無法轉移。

## <a name="azure-reservations-unavailable-markets"></a>未提供 Azure 保留的市場

> [!IMPORTANT]
> 以下是**未提供** Azure 保留的市場：  
>  
> **不適用的市場 (以字母順序排序)**
>
> |A 到 Gi   | Gr 到 Pal  | Pap 到 Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | 奧蘭島     | 格陵蘭     | 巴布亞紐幾內亞     |
> | 美屬薩摩亞     | 格瑞那達     | 皮特康群島     |
> | 安道爾     | 哥德普洛     | 留尼旺     |
> | 安圭拉     | 關島     | 沙巴   |
> | 南極大陸     | 根息     | 聖巴瑟米   |
> | 安地卡及巴布達       | 幾內亞     | 聖露西亞   |
> | 阿路巴       | 幾內亞比索     | 聖馬丁   |
> | 亞塞拜然       | 蓋亞納     | 聖匹島   |
> | 貝南     | 海地       | 聖文森及格瑞那丁     |
> | 不丹     | 赫德島及麥當勞群島       | 薩摩亞獨立國     |
> | 波奈     | 曼城島     | 聖馬利諾     |
> | 布威島     | 尖棉     | 聖多美普林西比   |
> | 英屬印度洋領土       | 澤西島     | 塞席爾   |
> | 英屬維爾京群島     | 吉里巴斯       | 獅子山   |
> | 布吉納法索     | 科索沃     | 聖佑達修斯     |
> | 蒲隆地     | 寮國     | 荷屬聖馬丁     |
> | 柬埔寨     | 賴索托     | 索羅門群島     |
> | 中非共和國     | 賴比瑞亞     | 索馬利亞     |
> | 查德     | 馬達加斯加     | 南喬治亞與南三明治群島     |
> | 中國     | 馬拉威     | 南蘇丹     |
> | 聖誕島     | 馬爾地夫     | 聖赫勒拿、阿森松、特里斯坦達庫尼亞群島     |
> | 可可斯群島     | 馬利     | 蘇利南     |
> | 葛摩     | 馬紹爾群島     | 冷岸     |
> | 剛果共和國     | 馬丁尼克     | 史瓦濟蘭     |
> | 剛果民主共和國 (DRC)     | 茅利塔尼亞     | 東帝汶   |
> | 柯克群島     | 馬約特島     | 多哥   |
> | 吉布地     | 密克羅尼西亞     | 托克勞群島   |
> | 多米尼克     | 蒙特色拉特島     | 東加   |
> | 赤道幾內亞     | 莫三比克     | 土克斯及開科斯群島   |
> | 厄利垂亞     | 緬甸     | 吐瓦魯   |
> | 福克蘭群島     | 諾魯     | 美國外島   |
> | 法屬圭亞那     | 新喀里多尼亞群島     | 萬那杜   |
> | 法屬玻里尼西亞     | 尼日     | 梵蒂岡   |
> | 法屬南半球領土     | 紐威島     | 瓦利斯及福杜納   |
> | 加彭     | 諾福克島     | 葉門   |
> | 甘比亞     | 北馬里安納群島     |    |
> | 直布羅陀     | 帛琉       |    |

## <a name="purchase-azure-reservations"></a>購買 Azure 保留

請遵循下列步驟，代表您的客戶在合作夥伴中心購買 Microsoft Azure 的保留。  (您想要讓客戶能夠從您購買的先前 Azure 訂用帳戶購買自己的 Azure 保留嗎？ 請參閱 [授與客戶購買自己的 Azure 保留的許可權](give-customers-permission.md)。 ) 

1. 從合作夥伴中心] 功能表中選取 [ **客戶** ]。  

2. 在 [ **客戶** ] 頁面上，尋找想要購買 Azure 保留的客戶，然後選取向下箭號以展開客戶的資料列。  

3. 選取 [新增產品]，然後選取 [Azure]。 

    a. 從 [區段] 清單中選擇客戶的市場區段。

    b. 從 [產品**類型**] 清單中選擇 [**保留**]。

    c. 從 [保留類型] 清單中選擇客戶想要的保留類型。

4. Azure Reservations 必須關聯至有效的 Azure 訂閱。 從 **客戶訂** 用帳戶清單中，選擇您想要新增 Azure 保留的客戶訂用帳戶。 

   >[!IMPORTANT]
   >如果客戶還沒有作用中的 Azure 訂用帳戶，請選取 **Azure** 來立即新增一個訂用帳戶。 

5. 使用篩選器來尋找符合客戶需求之虛擬機器上的 Azure 保留專案。  

6. 在您找到想要購買的保留 () 之後，請輸入客戶需要多少 **數量** 的保留實例，然後選取 [ **新增至購物車**]。  

7. 重複步驟5和6，直到您將所有必要的專案加入至訂單為止。 選取 [檢閱] 確認您的訂單正確無誤。  

8. 在 **\[檢視您的訂單\]** 頁面上，您可以： 

    - 確認或變更保留執行個體數量。

    - 選取保留區的範圍。 保留範圍可以涵蓋一個訂用帳戶或多個訂用帳戶 (共用範圍) 。 如果您將保留範圍設為單一訂用帳戶，保留折扣只會套用到此訂用帳戶。 如果您選取 [共用]，保留折扣會套用至客戶計費內容中的任何訂用帳戶。 

      >[!NOTE] 
      >如果您選擇將保留範圍限制為單一 Azure 訂用帳戶，您可能需要增加訂用帳戶的 vCPU 配額。 若要增加訂用帳戶的 vCPU 配額，您必須在 Azure 入口網站中建立支援要求。 請依照 [本主題中](/azure/azure-supportability/resource-manager-core-quotas-request) 的指示來建立要求。 

      >[!NOTE]   
      >如果您的客戶在 Azure 方案下， **範圍**  將會設定為 [ **共用**]。 

    - 如果您是提供者合作夥伴，請選取您想要與產品建立關聯的經銷商。
    
    - 如果您的 Azure 保留支援計費方案選項，您可以從下拉式功能表中選取 [每月計費頻率]。 
    - 如果您的 Azure 保留不支援帳單方案選項，您的計費頻率會預設為一次計費。 

9. 選取 **\[購買\]** 購買訂單。 您訂單的詳細資料（包括訂單號碼）會顯示在 [ **確認** ] 頁面上。 選取 [完成] 移至 [訂購記錄] 頁面。 

10. 若要在 Azure 入口網站中管理客戶的保留，請在 [ **客戶** ] 頁面上尋找 [客戶]，然後選取向下箭號展開客戶的資料列。 選取 **Microsoft Azure 管理入口網站** ，在 Azure 入口網站中開啟客戶的記錄。

## <a name="azure-reservations-resources"></a>Azure Reservations 資源
|**如需下列資訊**   |**請閱讀本文**    |
|:-----------------------------|:-----------------|
|雲端解決方案提供者中的 Azure Reservations 概觀  | [銷售 Microsoft Azure 保留的執行個體](azure-reservations.md) |
|在合作夥伴中心中管理 Azure 保留 | [在合作夥伴中心中管理 Azure 保留](azure-reservations-manage.md)
|判斷正確的 VM 大小，並確認客戶 VM 使用率   |[調整 VM 大小以提供最大 Azure Reservations 使用率](azure-usage.md)   |
|使用合作夥伴中心 API 購買 Azure Reservations | 合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](/partner-center/develop/purchase-azure-reservations)   |
|為客戶提供購買自己的 Azure 保留的許可權  | [提供客戶購買自己的 Azure 保留的許可權](give-customers-permission.md)  |