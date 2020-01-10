---
title: 確認客戶接受 Microsoft 客戶合約 | 合作夥伴中心
ms.topic: article
ms.date: 01/07/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何確認客戶接受 Microsoft 客戶合約。 這可能需要為客戶訂購 Microsoft 產品和服務。
author: LauraBrenner
ms.author: labrenne
keywords: 客戶, 客戶, 同意, MCA, Microsoft Cloud 合約, Microsoft 客戶合約, 客戶合約範本
ms.localizationpriority: medium
ms.openlocfilehash: 33eddc437360cb80071bf98187a7d4e23b820fb9
ms.sourcegitcommit: 99a8b2daf52d455d33f15945d52efbcc8ff551c8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/08/2020
ms.locfileid: "75752566"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>確認客戶接受 Microsoft 客戶合約

**適當的角色**

- 系統管理代理人
- 銷售代理人

目前，客戶必須接受並簽署適用的**Microsoft Cloud 合約**，CSP 合作夥伴才能代表客戶下訂單。 然後，合作夥伴必須提供簽署者的相關資訊給 Microsoft，以確認客戶接受。 如果未提供確認：
- 您將無法為此客戶建立新訂單。
- 您將無法變更此客戶現有以基座為基礎之訂用帳戶的基座數目。

如需如何使用合作夥伴中心儀表板或 API 來確認客戶接受 Microsoft Cloud 合約的詳細資訊，請參閱[確認客戶接受 Microsoft Cloud 合約](confirm-consent.md)。

Microsoft 將在 2019 年 10 月 1 日把 **Microsoft 客戶合約**引進 CSP 計畫，以取代 Microsoft Cloud 合約。 為了協助合作夥伴遷移至新的合約，在 2020 年 1 月 31 日前，CSP 計畫中將支援目前的 Microsoft Cloud 合約。 如需更多時間軸詳細資料，請參閱下表：

| 日期 | 里程碑 | 詳細資料 |
|------------|------------|--------------------------------|
|2019 年 8 月 1 日|沙箱中提供 UX 預覽|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心儀表板，確認客戶接受 Microsoft 客戶合約。 具有 CSP 沙箱環境存取權的合作夥伴可預覽使用者體驗變更。 沒有沙箱存取權的合作夥伴可以深入了解本主題中的變更。|
|2019 年 9 月 3 日|沙箱中提供 API 預覽。|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 API 來確認客戶接受 Microsoft 客戶合約。 API 合作夥伴可以使用此機會預覽 API 變更，並開始處理 API 整合以支援新的合約。|
|2019年9月20日|沙箱中提供 .NET SDK 預覽。|合作夥伴可以在 CSP 沙箱環境中使用合作夥伴中心 .NET SDK 來確認客戶接受 Microsoft 客戶合約。 API 合作夥伴可以使用此機會預覽 .NET SDK 變更，並開始處理 API 整合以支援新的合約。|
|2019 年 10 月 1 日|可在生產環境中使用的 Microsoft 客戶合約|Microsoft 會將 Microsoft 客戶合約引進 CSP 計畫，以取代 Microsoft Cloud 合約。 合作夥伴可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。 CSP 合作夥伴計畫中仍支援 Microsoft Cloud 合約。 不過，建議合作夥伴開始遷移至 Microsoft 客戶合約。 現有訂用帳戶的新購買和基座計數變更將需要 Microsoft 客戶合約或 Microsoft Cloud 合約的合作夥伴確認。 某些新供應項目 (例如新的 Azure 方案) 將需要確認 Microsoft 客戶合約。|
|2020 年 1 月 31 日|已從生產環境中移除 Microsoft Cloud 合約|CSP 合作夥伴計畫中不再接受 Microsoft Cloud 合約。 現有訂用帳戶的新購買和基座計數變更將需要合作夥伴提供 Microsoft 客戶合約的確認。 這項需求適用於新客戶及先前可能已接受 Microsoft Cloud 合約的現有客戶。|

## <a name="access-microsoft-customer-agreement-template"></a>存取 Microsoft 客戶合約範本
合作夥伴可以從[這裡](https://aka.ms/customeragreement)手動下載最新版本的 Microsoft 客戶合約範本。 請注意，Microsoft 客戶合約是國家/地區特有的。 當要求 Microsoft 客戶合約範本時，請務必根據客戶的位置選取正確的國家/地區。 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>使用合作夥伴中心 API/SDK 確認客戶接受
合作夥伴可以使用合作夥伴中心 API/SDK 來確認客戶接受 Microsoft 客戶合約。 如需 API/SDK 的詳細資訊，請參閱：

- [取得 Microsoft 客戶合約的合約中繼資料](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [確認客戶接受 Microsoft 客戶合約](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [取得客戶接受 Microsoft 客戶合約的確認](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [取得 Microsoft 客戶合約範本的下載連結](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>在合作夥伴中心確認客戶接受
合作夥伴可以在合作夥伴中心針對新客戶和現有客戶，確認客戶接受 Microsoft 客戶合約。 轉銷商無法代表其客戶進行證明，而且必須與間接提供者合作，才能完成證明。

### <a name="confirm-customer-acceptance-for-new-customers"></a>確認新客戶的客戶接受

當您在合作夥伴中心建立新的客戶租用戶時，請使用下列步驟來確認客戶是否接受 Microsoft 客戶合約。 您必須是系統管理員代理人或銷售代理人，才能執行這些步驟。

1. 選取 [客戶]，然後選取 [新客戶]。

2. 在 [帳戶資訊] 底下，輸入公司及其主要連絡人的資訊。

3. 在 [Microsoft 合約] 底下，選取 [Microsoft 客戶合約]。

4. 在 [合約接受日期] 下方，輸入適當的日期。 您不能將此日期設定為未來日期。

5. 請確定顯示的主要使用者連絡人資訊正確。 如果此資訊不正確，請選取 [更新]，然後輸入接受合約人員的 [名字]、[姓氏]、[電子郵件地址] 和 [電話號碼] (選用)。

6. 選取 [下一步] 以繼續建立客戶租用戶的其餘步驟。

![新客戶](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>確認現有客戶的客戶接受

您必須是系統管理員代理人或銷售代理人，才能執行此動作：

1. 選取 [客戶]。 尋找並選取客戶。

2. 選取 [帳戶資訊]。

3. 在 [Microsoft 客戶合約] 下方，選取 [更新]。

4. 輸入接受合約人員的 [名字]、[姓氏]、[電子郵件地址] 和 [電話號碼] (選用)。 在 [合約接受日期] 下方，輸入適當的日期。 您不能將此日期設定為未來日期。

5. 選取 [儲存] 並繼續作業。

![現有客戶](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>取得客戶接受的確認

您可以使用下列步驟來取得現有客戶已接受 Microsoft 客戶合約的確認。 您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 [客戶]，然後尋找並選取您想要查看的客戶。

2. 選取 [帳戶資訊]。

3. 在 [Microsoft 客戶合約] 底下，檢視此客戶是否已提供確認。
