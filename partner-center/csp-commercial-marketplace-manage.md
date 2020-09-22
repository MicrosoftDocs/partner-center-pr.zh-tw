---
title: 管理 marketplace 產品 & 優惠
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作夥伴中心，瞭解雲端解決方案提供者如何管理從商業市場為客戶購買的協力廠商 ISV 優惠。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d32f42b2c4bd8e4ec6c659326d1a21385c0642f
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000512"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>管理客戶的商業 marketplace 產品和優惠

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

雲端解決方案提供者 (CSP) 計畫中的合作夥伴，可以使用合作夥伴中心入口網站，向商業市場購買客戶的許多 ISV SaaS 供應專案或訂用帳戶。 購買供應專案後，您就有各種方式可以進行管理。

## <a name="view-or-edit-a-subscription"></a>查看或編輯訂用帳戶

從協力廠商 ISV 發行者購買訂用帳戶之後，您可以如下所示進行審核或編輯：

1. 登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **客戶** ]。

2. 選取適當的客戶，然後選取 [ **訂閱**]。 這會列出您為客戶購買的任何授權型訂閱。

3. 在 [ **訂** 用帳戶] 資料行中，選取您要查看或編輯的訂用帳戶。 這會提供您設定或布建供應專案的詳細資訊。  (如果供應專案需要更多動作，您可能也會在 [狀態] 資料行中看到 [需要採取動作] 狀態。 這也可能伴隨著 ISV 發行者網站的連結。 ) 

4. 當您選取要查看或編輯的訂用帳戶之後，[訂用帳戶詳細資料] 頁面可讓您編輯訂用帳戶，並執行如下的動作：

    - 變更訂用帳戶昵稱

    - 新增/減少訂用帳戶中的授權數目

    - 取消訂用帳戶

    - [關閉自動續約]

    - 新增間接轉銷商 MPN 識別碼（如果適用）

> [!NOTE]
> 您可能需要完成 ISV 發行者所定義的特定步驟，才能對訂用帳戶執行某些變更，例如取消訂用帳戶。

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>指派授權並代表客戶啟動訂用帳戶

當您購買軟體即服務 (SaaS) 供應專案由獨立軟體廠商 (ISV) publisher 在商用市集中提供，ISV 發行者可協助管理指派授權的程式，並代表您的客戶啟用訂用帳戶。

發行者應該提供個人化的連結，以及識別特定購買的授權碼。

1. 您可以透過下列幾種方式，從 ISV 發行者找到這個個人化連結：

   - 您可以在購買 ISV SaaS 供應專案之後，看到出現在 [確認] 頁面的連結。 若要在頁面上尋找此連結，請尋找並選取 [ **移至發行者的網站]**。

   - 您可以在特定客戶的 [訂用帳戶] 頁面中看到連結。 此發行者連結會出現在與客戶購買的 ISV 供應專案或訂用帳戶相關聯的資料列上。

   - 您可以 [使用合作夥伴中心 api 來取得連結](/partner-center/develop/get-activation-link-by-order-line-item)。

   > [!NOTE]
   > 若要代表您的客戶執行這項作業，您可能需要複製個人化連結、將它貼入私用瀏覽器，然後輸入客戶的認證。

2. 當您在 ISV 發行者的網站或系統中，發行者會讓您知道完成客戶安裝程式和布建或指派授權所需採取的任何額外步驟。

3. 身為代表您客戶工作之 CSP 方案中的合作夥伴，您必須負責執行下列工作：

    - 將任何必要的資訊提交給發行者。

    - 將任何必要的 URL 直接傳送給客戶 (，或直接將此訂用帳戶的詳細資料傳達給您的客戶) 

4. 一旦您提供必要資訊給發行者，發行者就會布建並指派適當的授權。 訂用帳戶只會在發生下列事件之後才開始計費：

    - ISV 發行者已成功指派適當的授權

    - ISV 發行者已透過個別的 SaaS 履行 API 確認了 Microsoft (，) 帳戶設定已成功完成

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>從 ISV 發行者取消以授權為基礎的 SaaS 訂用帳戶

當您訂閱「商業市場」內 ISV 發行者所提供的授權型 SaaS 產品時，您可以選擇在其指定的取消期間內取消訂用帳戶。 此取消期間會根據您是否有每月或每年訂閱而變更。 您也可以選擇是否要自動更新訂閱。

如需有關套用的取消期間、如何取消或如何自動更新訂用帳戶的詳細資訊，請參閱：

- [取消訂用帳戶](create-a-new-subscription.md#cancel-a-subscription)

- [自動更新商業 marketplace 訂用帳戶](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>新增或移除 SaaS 訂用帳戶的授權

針對 SaaS 商業市場優惠，您可以新增或移除客戶訂用帳戶的使用者授權。

1. 登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **客戶** ]。

2. 選取適當的客戶，然後選取 [ **訂閱**]。 這會列出您為客戶購買的任何授權型訂閱。

3. 在 [ **訂** 用帳戶] 資料行中，選取您要修改的訂用帳戶。

4. 在 [訂閱詳細資料] 頁面中，找出 [ **Quantity** ] 欄位。 您可以在這裡增加或減少授權數目。

5. 變更數量，然後選取 [ **提交**]。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作夥伴中心 API 管理訂閱

您也可以使用合作夥伴中心 Api 來執行生命週期管理及管理訂用帳戶的發票。 如需詳細資訊，請參閱 [建立商業 marketplace 產品的訂用](/partner-center/develop/create-subscription-azure-marketplace-products)帳戶。

## <a name="next-steps"></a>下一步

- [購買商用 marketplace 優惠](csp-commercial-marketplace-purchase.md)
- [瞭解商業 marketplace 中的帳單](csp-commercial-marketplace-billing.md)