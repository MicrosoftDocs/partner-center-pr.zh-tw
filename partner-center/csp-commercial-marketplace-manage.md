---
title: 為您的客戶管理商用 marketplace 產品或供應專案 |合作夥伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 使用合作夥伴中心，瞭解雲端解決方案提供者如何管理為來自商用 marketplace 的客戶購買的不同協力廠商 ISV 優惠。
author: MicheleHope
ms.author: v-mihope
keywords: 訂用帳戶，Marketplace，協力廠商，ISV，SaaS 優惠，雲端解決方案提供者方案，管理供應專案，管理訂用帳戶，授權，取消訂用帳戶，基座，關閉自動續訂，間接轉售商 MPN 識別碼
ms.localizationpriority: medium
ms.openlocfilehash: 7dbcc978340240175d2c03a5ba1e9312b48d7bdc
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/21/2020
ms.locfileid: "80114950"
---
# <a name="manage-commercial-marketplace-products-for-your-customers"></a>為您的客戶管理商業 marketplace 產品

**適用於**

- 夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

雲端解決方案提供者（CSP）方案中的合作夥伴可以使用合作夥伴中心入口網站，為客戶從商業 marketplace 購買許多 ISV SaaS 供應專案或訂閱。 購買供應專案之後，您可以使用各種方式來進行管理。

## <a name="view-or-edit-a-subscription"></a>查看或編輯訂用帳戶

向協力廠商 ISV 發行者購買訂閱之後，您可以如下所示加以檢查或編輯：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [**客戶**]。

2. 選取適當的客戶，然後選取 [訂用帳戶 **]。** 這會列出您已為客戶購買的任何授權型訂閱。

3. 在 [**訂**用帳戶] 資料行中，選取您想要查看或編輯的訂用帳戶。 這會提供您設定或布建供應專案的詳細資訊。 （如果供應專案需要執行更多動作，您可能也會看到 [狀態] 欄中顯示 [需要動作] 狀態。 這也可能伴隨著 ISV 發行者網站的連結）。

4. 選取您想要查看或編輯的訂用帳戶之後，[訂閱詳細資料] 頁面可讓您編輯訂用帳戶，並執行以下動作：

    - 變更訂用帳戶昵稱

    - 新增/減少訂用帳戶中的基座數目（授權）

    - 取消訂用帳戶

    - [關閉自動續約]

    - 新增間接轉銷商 MPN 識別碼（如果適用）

> [!NOTE]
> 您可能需要先完成 ISV 發行者所定義的特定步驟，才能對訂用帳戶執行某些變更，例如取消訂用帳戶。

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>指派授權並代表客戶啟動訂用帳戶

當您購買商業 marketplace 中的獨立軟體廠商（ISV）發行者所提供的「軟體即服務」（SaaS）供應專案時，ISV 發行者會協助管理指派授權的程式，並代表您的「啟用」訂用帳戶顧客.

發行者應該提供個人化的連結，以及識別您特定購買的授權碼。

1. 您可以透過幾種方式，從 ISV 發行者找到這項個人化連結：

    - 在您購買 ISV SaaS 供應專案之後，您可以在 [確認] 頁面中看到連結。

    - 您可以從特定客戶的 [訂閱] 頁面看到連結。 此發行者連結會出現在與客戶購買的 ISV 供應專案或訂用帳戶相關聯的資料列上。

    - 您可以[使用合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)來抓取連結。

2. 一旦您在 ISV 發行者的網站或系統中，發行者就會讓您知道完成客戶設定程式以及布建或指派授權時所需採取的任何額外步驟。

3. 身為代表您客戶工作之 CSP 計畫的合作夥伴，您必須負責執行下列工作：

    - 將任何必要的資訊提交給發行者。

    - 將任何必要的 URL 直接傳送給您的客戶（或直接將此訂用帳戶的詳細資料傳達給您的客戶）

4. 一旦您將必要的資訊提供給發行者，發行者就會布建並指派適當的授權。 只有在發生下列事件之後，訂用帳戶才會開始計費：

    - ISV 發行者已成功指派適當的授權

    - ISV 發行者已確認 Microsoft （透過個別的 SaaS 履行 API）已成功完成帳戶設定

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>從 ISV 發行者取消以授權為基礎的 SaaS 訂用帳戶

當您訂閱商業 marketplace 中 ISV 發行者所提供的授權型 SaaS 產品時，您可以選擇在其指定的取消期間內取消訂用帳戶。 此取消期間會根據您是否有每月或年度訂閱而變更。 您也可以選擇是否要自動更新訂用帳戶。

如需有關取消期間、如何取消或如何自動更新訂閱的詳細資訊，請參閱：

- [取消訂用帳戶](create-a-new-subscription.md#cancel-a-subscription)

- [自動續訂商業 marketplace 訂用帳戶](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>新增或移除 SaaS 訂用帳戶的授權

針對 SaaS 商業 marketplace 供應專案，您可以新增或移除客戶訂用帳戶的使用者授權。

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [**客戶**]。

2. 選取適當的客戶，然後選取 [訂用帳戶 **]。** 這會列出您已為客戶購買的任何授權型訂閱。

3. 在 [**訂**用帳戶] 欄位中，選取您想要修改的訂用帳戶。

4. 在 [訂閱詳細資料] 頁面中，找出 [ **Quantity** ] 欄位。 這是您可以增加或減少授權數目的地方。

5. 變更數量，然後選取 [**提交**]。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作夥伴中心 API 管理訂閱

您也可以使用合作夥伴中心 Api 來執行生命週期管理，並管理您訂用帳戶的發票。 如需詳細資訊，請參閱[建立商業 marketplace 產品的訂用](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)帳戶。

## <a name="next-steps"></a>後續步驟

- [購買商用 marketplace 優惠](csp-commercial-marketplace-purchase.md)
- [瞭解商業 marketplace 中的帳單](csp-commercial-marketplace-billing.md)