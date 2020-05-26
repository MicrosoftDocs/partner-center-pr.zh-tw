---
title: Salesforce CRM 合作夥伴中心的共同銷售連接器
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用 Salesforce CRM 連接器，取得 Microsoft 的參考
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825695"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM 的共同銷售連接器-總覽

### <a name="appropriate-roles"></a>適當的角色

- 推薦管理員
- CRM 上的系統管理員或系統自訂者

合作夥伴中心共同銷售連接器可讓您的銷售人員從您的 CRM 系統內與 Microsoft 共同合作。 他們不需要經過訓練，就能使用合作夥伴中心來管理共同銷售交易。 使用共同銷售連接器，您將能夠建立新的共同銷售諮詢，以參與 Microsoft 賣方、接收來自 Microsoft 賣方的參考、接受/拒絕參考、修改交易資料（例如交易價值、結束日期等），以及接收來自 Microsoft 賣方的任何更新，以進行這些共同銷售交易。 您可以在您選擇的 CRM 中工作，而不是在合作夥伴中心內執行所有動作。 

解決方案是以 Microsoft 電源自動化解決方案為基礎，並使用 Microsoft 合作夥伴中心 Api。


## <a name="before-you-install---pre-requisites"></a>安裝之前的必要條件

|**主題**   |**詳細資料**   |**連結**   |
|--------------|--------------------|------|
|Microsoft 合作夥伴網路識別碼 |您需要有效的 MPN 識別碼|加入[MPN](https://partner.microsoft.com/)|
|共同銷售準備就緒|您的 IP/服務解決方案必須共同銷售。|[與 Microsoft 一起銷售](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|合作夥伴中心帳戶|與合作夥伴中心租使用者相關聯的 MPN 識別碼，必須與您的共同銷售解決方案相關聯的 MPN 識別碼相同。 在部署連接器之前，請確認您可以在合作夥伴中心入口網站中看到您的共同銷售參照。|[管理您的帳戶](create-user-accounts-and-set-permissions.md)|
|合作夥伴中心使用者角色|將安裝和使用連接器的員工必須是推薦管理員|[指派使用者角色和權限](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM 使用者角色是系統管理員或系統自訂者|[指派 Dynamics 365 中的角色](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power 自動化 Flow 帳戶|適用于 CRM 系統管理員或系統自訂者的主動式[電源自動化](https://flow.microsoft.com)帳戶。 該使用者應該在安裝之前至少登入一次[電源](https://flow.microsoft.com)。|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>安裝 Salesforce CRM 的合作夥伴中心推薦同步處理

1. 移至 [[電源自動化](https://flow.microsoft.com)]，並選取右上角的 [**環境**]。 這會顯示可用的 CRM 實例。

2. 從右上角的下拉式選單中，選取適當的 CRM 實例。 

3. 選取左側導覽列上的 [**方案**]。

4. 按一下上方功能表上的 [**開啟 AppSource** ] 連結。

![開啟 AppSource](images/cosellconnectors/openappsource.png)

5. 在彈出畫面中搜尋**Salesforce 的合作夥伴中心參照連接器**。  

6. 按一下 [**立即取得**] 按鈕，然後按 [**繼續**]。 

7. 這會開啟頁面，您可以在其中選取要安裝應用程式的 CRM （Dynamics 365）環境。  同意條款及條件。 

8. 接著，您會被導向至 [**管理您的解決方案**] 頁面。  使用頁面底部的箭號按鈕，流覽至 [合作夥伴中心的參考]。 已**排程的安裝**應該會出現在合作夥伴中心的 [參考解決方案] 旁。 安裝需要10-15 分鐘的時間。 

9. 安裝完成後，流覽回到 [[電源自動化](https://flow.microsoft.com)]，然後從左側導覽區域選取 [**解決方案**]。 請注意，解決方案清單中提供**Salesforce 的合作夥伴中心參照同步**處理。

10. 選取**Dynamics 365 的合作夥伴中心參照同步**處理。 下列電源可自動執行流程和實體：

![可用的 CRM](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>最佳做法：在您上線之前進行測試

在您安裝、設定及自訂生產環境的電源自動化解決方案之前，請務必在預備 CRM 實例上測試解決方案。

- 在預備環境/CRM 實例上安裝 Microsoft Power 自動化解決方案。
- 建立解決方案的複本並執行設定，並在預備環境上自動化流程自訂。
- 在預備/CRM 實例上測試解決方案。 
- 成功時，將匯入為生產實例的受控解決方案。 

## <a name="configure-the-solution"></a>設定解決方案

1. 在您的 CRM 實例中安裝解決方案之後，請流覽回到 [[電源自動化](https://flow.microsoft.com/)]。

2. 從右上角的 [**環境**] 下拉式選，選取您已安裝電源自動化解決方案的 CRM 實例。

3. 您將需要建立與三個使用者帳戶建立關聯的連接： 

- 具有參考系統管理員認證的合作夥伴中心使用者 
- 合作夥伴中心事件
- CRM 系統管理員，具備在解決方案中自動化流程的能力。 

    a. 從左側導覽列選取 [連線]，**然後從清單**中選取 [合作夥伴中心參照] 解決方案。
    b. 按一下 [**建立連接**] 來建立連線。 

    ![建立連線](images/cosellconnectors/createconnection.png)

    c. 在右上角的搜尋列中搜尋**合作夥伴中心參照（預覽）** 。
    d. 使用 [參考管理員] 的認證角色建立合作夥伴中心使用者的連線。版. 接下來，使用 [參考管理員] 的認證為合作夥伴中心使用者建立合作夥伴中心的事件連線。f. 為 CRM 系統管理員使用者建立 Common Data Service （目前的環境）的連接。

4. 若要讓電源自動化流程與連線產生關聯，請編輯每個電源自動化流程，以連線至 Common Data Service 和合作夥伴中心的參照。 儲存變更。

5. **開啟**電源自動化流程。

## <a name="next-steps"></a>後續步驟

- [使用 Webhook 取得資源變更事件](referral-connector-webhooks.md)

- [深入瞭解 Microsoft Power 自動化平臺？](https://docs.microsoft.com/power-automate/)

- [管理潛在客戶](manage-leads.md)

- [管理共同銷售商機](manage-co-sell-opportunities.md)
