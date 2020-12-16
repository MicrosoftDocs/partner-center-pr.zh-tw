---
title: 確認客戶接受 Microsoft 客戶合約
description: 了解如何確認客戶接受 Microsoft 客戶合約。 這可能需要為客戶訂購 Microsoft 產品和服務。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: f2513213bff38a6296832253a13725ff2508f1f8
ms.sourcegitcommit: 22d79fb31cce852ae809078ea2310ebc80030739
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/12/2020
ms.locfileid: "97354605"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>用來確認客戶是否已接受 Microsoft 客戶合約的更新後方法


**適當的角色**

- 系統管理代理人
- 銷售代理人

> [!NOTE]
> 目前只有 Microsoft 公用雲端中的合作夥伴中心支援合約資源。 合約資源不適用於：
> * 由 21Vianet 營運的合作夥伴中心
> * Microsoft Cloud 德國合作夥伴中心
> * Microsoft Cloud for US Government 適用的合作夥伴中心

>[!NOTE]
>自 2020 年 1 月 31 日起，所有客戶 (包括現有和新的客戶) 都必須簽署新的 Microsoft 客戶合約。 如需詳細資訊，請閱讀[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)。

身為合作夥伴，您必須先讓您的客戶接受 Microsoft 客戶合約，才能為該客戶訂購 Microsoft 產品和服務。 為了更妥善協助合作夥伴符合合規需求，Microsoft 會要求合作夥伴提供接受合約者的下列相關詳細資料，以確認接受：

- 名字

- 姓氏

- 電子郵件地址

- 電話號碼 (選用)

- 接受日期

直接帳單合作夥伴和間接提供者透過合作夥伴中心或合作夥伴中心 API 交易時，必須確認客戶已接受 Microsoft 客戶合約。 確認是「強制性」  的。

如未提供客戶確認：

- 您將無法為此客戶建立新訂單。

- 您將無法變更此客戶現有授權型訂閱的授權數目。

確認客戶接受可以透過合作夥伴中心或合作夥伴中心 API 來完成。 若要透過合作夥伴中心 API 執行這項操作，請參閱下列主題：

- [取得客戶同意的確認](/partner-center/develop/get-confirmation-of-customer-consent)

- [取得合約中繼資料](/partner-center/develop/get-agreement-metadata)

- [確認客戶同意](/partner-center/develop/confirm-customer-consent)

這同時適用于生產和沙箱環境。

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>確認新客戶的客戶接受

當您在合作夥伴中心建立新的客戶租用戶，請使用下列程序來確認客戶接受。 您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 [客戶]  ，選取 [新客戶]  ，然後選取 [帳戶資訊]  。

2. 輸入[公司]  和 [主要連絡人]  資訊。

   :::image type="content" source="images/mca/mca1.png" alt-text="公司資訊":::

3. 在 [Microsoft 客戶合約]  底下，選取 [客戶已接受最新的 Microsoft 客戶合約]  。

4. 在 [合約接受日期]  下方，輸入適當的日期。 您不能將此日期設定為未來日期。

5. 輸入提供接受的使用者詳細資料。

   :::image type="content" source="images/mca/MCA3.png" alt-text="新增接受日期":::

   根據預設，會顯示主要連絡人的使用者資訊。 如果此資訊不正確，請選取 [更新]  ，然後輸入接受合約之人員的 [名字]  、[姓氏]  、[電子郵件地址]  、*[電話號碼]  (選用)。

6. 選取 [下一步]  以繼續建立客戶租用戶的其餘步驟。

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>確認現有客戶的客戶接受

您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 [客戶]，然後尋找並選取您想要查看的客戶。

2. 選取 [帳戶資訊]  。

3. 在 [Microsoft 客戶合約]  下方，選取 [更新]  。

   :::image type="content" source="images/mca/mca4.png" alt-text="更新":::

4. 輸入接受合約之使用者的[名字]  、[姓氏]  、[電子郵件地址]  、[電話號碼]  (選用)。

5. 在 [合約接受日期]  下方，輸入適當的日期。 您不能將此日期設定為未來日期。

6. 選取 [儲存並繼續]  。

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>為現有客戶建立新訂單時確認客戶接受

如果您嘗試為以前沒有確認過的現有客戶建立新訂單，您會收到完成確認的提示。 使用下列程序來執行此動作。

1. 輸入接受合約之使用者的[名字]  、[姓氏]  、[電子郵件地址]  、[電話號碼]  (選用)。

2. 在 [合約接受日期]  下方，輸入適當的日期。 您不能將此日期設定為未來日期。

3. 選取 [儲存並繼續]  。

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>擷取現有客戶的客戶接受確認

您可以使用下列程序，擷取您先前提供過的現有客戶的客戶接受確認。 您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 [客戶]，然後尋找並選取您想要查看的客戶。

2. 選取 [帳戶資訊]  。

3. 在[Microsoft 客戶合約]  下方，您會看到是否已為這個客戶提供確認。

## <a name="next-steps"></a>後續步驟

- [確認客戶接受 CSP 合作夥伴方案中的 Microsoft 客戶合約](confirm-customer-agreement.md)

- [代表客戶證明接受 Microsoft 客戶合約](attest-acceptance-customer-agreement.md)