---
title: 確認客戶接受 Microsoft Cloud 合約 | 合作夥伴中心
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何確認客戶接受 Microsoft Cloud 合約。 這可能需要為客戶訂購 Microsoft 產品和服務。
author: LauraBrenner
ms.author: labrenne
keywords: 客戶、客戶、同意、MCA、Microsoft Cloud 合約、客戶合約範本
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252584"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>確認客戶接受 Microsoft Cloud 合約

**適用於**
-  合作夥伴中心

> [!NOTE]
> 合約資源目前僅由 Microsoft 公用雲端中的合作夥伴中心支援。 不適用於：
> * 由 21Vianet 營運的合作夥伴中心
> * Microsoft Cloud 德國合作夥伴中心
> * Microsoft Cloud for US Government 適用的合作夥伴中心

>[!NOTE]
>此合約會在2020年1月31日前生效。 在該日期之後，所有客戶（現有和新的）都必須簽署新的 Microsoft 客戶合約。 若要深入瞭解，請閱讀[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)。

身為合作夥伴，您必須先取得客戶的 Microsoft Cloud 合約接受者，才能訂購該客戶的 Microsoft 產品和服務。 為了更妥善協助合作夥伴符合合規需求，Microsoft 會要求合作夥伴提供接受合約者的下列相關詳細資料，以確認接受： 

-   名字

-   姓氏

-   電子郵件地址

-   電話號碼 (選用)

-   接受日期

若要深入瞭解，請參閱 Microsoft Cloud 合約客戶接受確認[常見問題](https://docs.microsoft.com/partner-center/confirm-consent-faq)。

直接帳單合作夥伴和間接提供者必須在透過合作夥伴中心或合作夥伴中心 API 交易時，確認客戶接受 Microsoft Cloud 合約。 確認是*必要*的。

如果未為指定客戶提供確認：

-   您將無法為此客戶建立新訂單。

-   您將無法變更此客戶現有以基座為基礎之訂用帳戶的基座數目。

您可以透過合作夥伴中心或合作夥伴中心 API 來確認客戶接受。 若要透過合作夥伴中心 API 來執行這項操作，請參閱下列主題： 

-   [取得客戶同意的確認](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [取得合約中繼資料](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [確認客戶同意](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


這同時適用于生產和沙箱環境。

## <a name="confirming-customer-acceptance-in-partner-center"></a>確認合作夥伴中心的客戶接受度

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>確認新客戶的客戶接受

當您在合作夥伴中心建立新的客戶租使用者時，請使用下列程式來確認客戶接受度。 請注意，您必須是系統管理代理人或銷售代理人，才能執行此動作。

1. 依序選取 [**客戶**] 和 [**新客戶**]，然後選取 [**帳戶資訊**]。
2. 輸入 **\[公司\]** 和 **\[主要連絡人\]** 的相關資訊。

![公司資訊](images/mca/mca1.png)

3. 在 **\[Microsoft Cloud 合約\]** 中，選取 **\[客戶已接受最新的 Microsoft cloud 合約\]** 。
4. 在 [合約接受日期] 下方，輸入適當的日期。 您不能將此設定為未來日期。
5. 輸入提供接受的使用者詳細資料。

![新增接受日期](images/mca/MCA3.png)

根據預設，會顯示主要連絡人使用者資訊。 如果不正確，請選取 [**更新**]，然後輸入接受合約之人員的 [**名字**]、[**姓氏**]、[**電子郵件地址**] 和 [*電話號碼*（選擇性）]。

6. 選取 [下一步] 以繼續建立客戶租用戶的其餘步驟。

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>確認現有客戶的客戶接受

您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 **\[客戶\]** ，然後尋找並選取您想要查看的客戶。
2. 選取 [帳戶資訊]。
3. 在 **\[Microsoft Cloud 合約\]** 下方，選取 **\[更新\]** 。

![更新](images/mca/mca4.png)

4. 輸入接受合約之使用者的 **\[名字\]** 、 **\[姓氏\]** 、 **\[電子郵件地址\]** 和 **\[電話號碼\]** (選用)。
5. 在 [合約接受日期] 下方，輸入適當的日期。 您不能將此設定為未來日期。
6. 選取 **\[儲存並繼續\]** 。

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>為現有客戶建立新訂單時確認客戶接受

如果您嘗試為尚未確認的現有客戶建立新訂單，您會收到完成確認的提示。 請使用下列程序來執行此動作。

1. 輸入接受合約之使用者的 **\[名字\]** 、 **\[姓氏\]** 、 **\[電子郵件地址\]** 和 **\[電話號碼\]** (選用)。
2. 在 [合約接受日期] 下方，輸入適當的日期。 您不能將此設定為未來日期。
3. 選取 **\[儲存並繼續\]** 。

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>擷取現有客戶的客戶接受確認

您可以使用下列程序，擷取您先前提供過的現有客戶的客戶接受確認。 您必須是系統管理員代理人或銷售代理人，才能執行此動作。

1. 選取 **\[客戶\]** ，然後尋找並選取您想要查看的客戶。
2. 選取 [帳戶資訊]。
3. 在 [ **Microsoft cloud 合約**] 底下，您會看到是否已為此客戶提供確認。
