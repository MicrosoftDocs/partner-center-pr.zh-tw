---
title: 確認客戶接受 Microsoft 客戶合約 | 合作夥伴中心
ms.topic: article
ms.date: 02/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 了解如何確認客戶接受 Microsoft 客戶合約。 這可能需要為客戶訂購 Microsoft 產品和服務。
author: LauraBrenner
ms.author: labrenne
keywords: 客戶, 客戶, 同意, MCA, Microsoft Cloud 合約, Microsoft 客戶合約, 客戶合約範本
ms.localizationpriority: high
ms.openlocfilehash: a40d5fa1d737dd679699db467ce8b3b1be81f84b
ms.sourcegitcommit: 1125391fd9a1ded2a051968b3a280a10676ed8bb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/04/2020
ms.locfileid: "82741049"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>確認客戶接受 Microsoft 客戶合約

**適用於**

- 合作夥伴中心
- Microsoft 365 系統管理中心

**適當的角色**

- 系統管理代理人
- 銷售代理人

**適當的合作夥伴類型**

- 間接轉銷商、直接帳單、間接提供者


Microsoft 在 2019 年 10 月 1 日把 **Microsoft 客戶合約**引進 CSP 計畫，以取代 Microsoft Cloud 合約。 若為間接轉銷商，請參閱其他[指引](indirect-reseller-tasks-in-partner-center.md)。 為了協助合作夥伴遷移至新的合約，在 2020 年 1 月 31 日前，此兩個合約會並存在 CSP 計畫中。 從 2020 年 2 月 1 日開始，Microsoft 客戶合約會取代 Microsoft Cloud 合約。

客戶有兩個選項可以接受 Microsoft 客戶合約。 

**選項 1**：合作夥伴證明客戶接受 - 合作夥伴可以使用合作夥伴中心 API/SDK 或透過合作夥伴中心儀表板來確認客戶接受。

**選項 2**：客戶直接接受 - 合作夥伴可以透過 URL 邀請客戶，在 Microsoft 365 系統管理中心檢閱及接受合約。

## <a name="access-microsoft-customer-agreement-template"></a>存取 Microsoft 客戶合約範本

您可以從[這裡](https://aka.ms/customeragreement)手動下載最新版本的 Microsoft 客戶合約範本。 Microsoft 客戶合約是國家/地區特定。 當要求 Microsoft 客戶合約範本時，請務必根據客戶的位置選取正確的國家/地區。 

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>選項 1：在合作夥伴中心確認客戶接受

合作夥伴可以在合作夥伴中心針對新的和現有的客戶，確認客戶接受 Microsoft 客戶合約。 轉銷商無法代表其客戶進行證明，而且必須與間接提供者合作，才能完成證明。

### <a name="confirm-customer-acceptance-for-new-customers"></a>確認新客戶的客戶接受

當您在合作夥伴中心建立新的客戶租用戶時，請使用下列步驟來確認客戶是否接受 Microsoft 客戶合約。 您必須是系統管理員代理人或銷售代理人，才能執行這些步驟。

1. 選取 [客戶]  ，然後選取 [新客戶]  。

2. 在 [帳戶資訊]  底下，輸入公司及其主要連絡人的資訊。

3. 在 [Microsoft 合約]  底下，選取方塊以證明客戶已接受 Microsoft 客戶合約。 

4. 在 [合約接受日期]  下方，輸入適當的日期。 您不能將此日期設定為未來日期。

5. 請確定顯示的主要使用者連絡人資訊正確。 如果資訊不正確，請選取 [更新]  ，然後輸入接受合約人員的正確資訊。

6. 選取 [下一個]  ，繼續建立客戶租用戶。

![新客戶](images/mca/newcustomeragreement.jpg)  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>確認現有客戶的客戶接受

您必須是系統管理員代理人或銷售代理人，才能執行此動作：

1. 選取 [客戶]  。 尋找並選取客戶。

2. 選取 [帳戶資訊]  。

3. 在 [Microsoft 客戶合約]  下方，選取 [更新]  。

4. 輸入接受合約人員的 [名字]  、[姓氏]  、[電子郵件地址]  和 [電話號碼]  (選用)。 在 [合約接受日期]  下方，輸入適當的日期。 您不能將此日期設定為未來日期。

5. 選取 [儲存]  並繼續作業。

![現有客戶](images/mcua2-update2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>取得客戶接受的確認

您可以使用下列步驟來取得現有客戶已接受 Microsoft 客戶合約的確認。 您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 [客戶]  ，然後尋找並選取您想要查看的客戶。

2. 選取 [帳戶資訊]  。

3. 在 [Microsoft 客戶合約]  底下，檢視此客戶是否已提供確認。

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>使用合作夥伴中心 API/SDK 確認客戶接受

您可以使用合作夥伴中心 API/SDK 來確認客戶接受 Microsoft 客戶合約。 如需 API/SDK 的詳細資訊，請參閱：

- [取得 Microsoft 客戶合約的合約中繼資料](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [確認客戶接受 Microsoft 客戶合約](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [取得客戶接受 Microsoft 客戶合約的確認](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [取得 Microsoft 客戶合約範本的下載連結](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>選項 2：Microsoft 365 系統管理中心的客戶接受

合作夥伴可以透過 URL 邀請新的和現有的客戶，在 Microsoft 365 系統管理中心內檢閱及接受合約。 接下來幾節將示範如何：

- 建立全新的客戶，並邀請客戶檢閱及接受合約。

- 邀請新客戶檢閱及接受轉銷商關係和合約。

- 邀請現有的客戶檢閱及接受合約。

>[!NOTE]
> 您可以使用[合作夥伴中心 API/SDK](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement)，取得客戶直接接受 Microsoft 客戶合約的狀態。  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>建立全新的客戶，並邀請客戶檢閱及接受合約

使用下列步驟在合作夥伴中心建立新的客戶，然後邀請他們在 Microsoft 365 系統管理中心內檢閱及接受 Microsoft 客戶合約。

1. 從合作夥伴中心的 [客戶]  索引標籤中，選取 [新增客戶]  。

2. 在 [帳戶資訊]  底下的所有必要欄位中，輸入新客戶的相關資訊，包括客戶的公司名稱和主要連絡人。

3. 在 [客戶合約]  中，選取第一個選項 [要求客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約]  。 完成頁面上其他任何必要欄位。

4. 選取 **[下一步：檢閱]** ，然後繼續建立客戶租用戶的步驟。 (注意：新客戶在接受 Microsoft 客戶合約之前，無法進行新的購買。)  

![建立新客戶](images/mca/create-new-customer.jpg)

5. 當您到達新客戶工作流程中的 [確認]  畫面時，請儲存客戶認證。 您稍後必須將這些認證提供給您的客戶。

6. 在合作夥伴中心外，建立並傳送電子郵件，邀請客戶在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。 請務必在電子郵件中包含下列項目：

   - 此 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) 的連結 (需要登入)

   - 您在步驟 5 中儲存的客戶認證。

7. 客戶接著會收到來自合作夥伴的電子郵件邀請，然後選取 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。

8. 客戶使用先前所收到來自合作夥伴的客戶認證，來登入 Microsoft 365 系統管理中心。

9. 客戶接著勾選方塊來接受 Microsoft 客戶合約。

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約 

使用下列步驟來邀請新客戶檢閱及接受轉銷商關係和 Microsoft 客戶合約。 

1. 從合作夥伴中心的 [客戶]  索引標籤中，選取 [要求建立轉銷商關係]  連結。 

2. 系統會產生自動電子郵件範本，包括文字和參數化 URL，以將客戶引導至 Microsoft 365 系統管理中心。

3. 您可以自訂自動產生的電子郵件範本，然後選取 [複製到剪貼簿]  或 [在電子郵件中開啟]  。

4. 使用此電子郵件範本來邀請客戶接受**轉銷商關係**要求和 **Microsoft 客戶合約**。 (注意：在電子郵件邀請中，請確定合作夥伴也包含自動提供的 URL，以及最近建立的客戶認證)。

![建立關係](images/mca/createrelationship.png)

5. 客戶透過電子郵件接收邀請，然後按一下參數化 URL。 

6. 客戶使用合作夥伴在電子郵件內提供的認證來登入 Microsoft 365 系統管理中心。

7. 客戶勾選方塊以接受**轉銷商關係**和 **Microsoft 客戶合約**。 

8. 在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。 他們可以選取合作夥伴來查看詳細資料。

![接受合約](images/mca/accept.jpg)


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>邀請現有的客戶檢閱及接受合約 

使用下列步驟來邀請現有的客戶檢閱及接受 Microsoft 客戶合約。 

1. 建立具有內嵌 URL 的客戶電子郵件，邀請您的客戶接受 Microsoft 客戶合約。

2. 您的客戶透過電子郵件收到邀請，然後按一下 [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement)。 

3. 客戶將其認證輸入 Microsoft 365 系統管理中心。

4. 您的客戶勾選方塊來接受 Microsoft 客戶合約。 

5. 在相同的 URL 中，客戶可以看到他們正在合作的不同合作夥伴合併清單。 他們可以選取合作夥伴來查看詳細資料。

![客戶](images/mca/customeraccept.png)

>[!NOTE]
>在某些情況下，客戶可能無法直接接受 Microsoft 客戶合約。 若要深入了解這些情況，請參閱[您需要代表客戶進行證明的兩個案例](attest-acceptance-customer-agreement.md)。

### <a name="historical-timeline-details"></a>歷程記錄時間軸詳細資料

| 日期 | 里程碑 | 詳細資料 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|沙箱中提供 UX 預覽|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心儀表板，確認客戶接受 Microsoft 客戶合約。 具有 CSP 沙箱環境存取權的合作夥伴可預覽使用者體驗變更。 沒有沙箱存取權的合作夥伴可以深入了解本主題中的變更。|
|2019 年 9 月 3 日|沙箱中提供 API 預覽。|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 API 來確認客戶接受 Microsoft 客戶合約。 API 合作夥伴可以使用此機會預覽 API 變更，並開始處理 API 整合以支援新的合約。|
|2019 年 9 月 20 日|沙箱中提供 .NET SDK 預覽。|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 .NET SDK 來確認客戶接受 Microsoft 客戶合約。 API 合作夥伴可以使用此機會預覽 .NET SDK 變更，並開始處理 API 整合以支援新的合約。|
|2019 年 10 月 1 日|可在生產環境中使用的 Microsoft 客戶合約|Microsoft 會將 Microsoft 客戶合約引進 CSP 計畫，以取代 Microsoft Cloud 合約。 合作夥伴可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。 CSP 合作夥伴計畫中仍支援 Microsoft Cloud 合約。 不過，建議合作夥伴開始遷移至 Microsoft 客戶合約。 現有訂用帳戶的新購買和基座計數變更將需要 Microsoft 客戶合約或 Microsoft Cloud 合約的合作夥伴確認。 某些新供應項目 (例如新的 Azure 方案) 將需要確認 Microsoft 客戶合約。|
|2020 年 1 月 31 日|已從生產環境中移除 Microsoft Cloud 合約|CSP 合作夥伴計畫中不再接受 Microsoft Cloud 合約。 現有訂用帳戶的新購買和基座計數變更將需要合作夥伴提供 Microsoft 客戶合約的確認。 這項需求適用於新客戶及先前可能已接受 Microsoft Cloud 合約的現有客戶。|
|2020 年 2 月 3 日|合作夥伴現在可以選擇透過 URL 來邀請客戶，在已驗證的 Microsoft 365 系統管理中心檢閱及接受合約。 | 客戶可以在 Microsoft 365 系統管理中心接受 Microsoft 客戶合約。 客戶在 Microsoft 365 系統管理中心直接接受合約即會確認條款核准。 
