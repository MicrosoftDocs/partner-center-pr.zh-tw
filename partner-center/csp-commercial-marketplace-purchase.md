---
title: 購買商用 marketplace 優惠
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 方案合作夥伴如何使用合作夥伴中心 marketplace，讓客戶從獨立軟體廠商 (Isv) 購買 SaaS 供應專案。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7533b0791ec8760c6223d6af59c2b7995b34a7bc
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000502"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>在合作夥伴中心中為您的客戶購買商用 marketplace 產品

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

在雲端解決方案提供者 (CSP) 計畫中的合作夥伴，您可以使用商用 marketplace 為客戶購買特定軟體即服務的訂用帳戶， (SaaS) 獨立軟體廠商 (Isv 所提供的產品。 

藉由為您的客戶提供 ISV SaaS 訂用帳戶，您可以協助您區分企業。 您也可以讓客戶存取軟體組合，以解決其特定的商務需求。 您可以從 ISV 發行者管理這些 marketplace SaaS 產品的授權和訂用帳戶，就像您管理 Microsoft 產品的授權和訂閱一樣。

您可以購買以 **授權為基礎** 的 SaaS 訂用帳戶或以 **使用量為基礎的** 訂用帳戶。 若要深入瞭解以授權為基礎和以使用量為基礎的計費之間的差異，請參閱 [計費基本概念](billing-basics.md)。

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>在合作夥伴中心中購買以授權為基礎的 SaaS 訂閱

您可以使用您用來購買 Microsoft 產品訂閱的相同程式，購買 ISV 發行者所提供的授權型 SaaS 產品訂用帳戶。

若要購買合作夥伴中心中以授權為基礎的 SaaS 訂用帳戶，請參閱 [建立、暫停或取消客戶訂閱](create-a-new-subscription.md#create-a-new-subscription)。

您也可以使用[合作夥伴中心 API](/partner-center/develop/) 來為您的客戶建立商業市集訂用帳戶。  (如需有關使用合作夥伴中心 Api 的詳細資訊，請參閱 [建立商用 marketplace 產品的訂用](/partner-center/develop/create-subscription-azure-marketplace-products)帳戶。 ) 

>[!IMPORTANT]
> 作為 CSP 方案中的合作夥伴，您只能從合作夥伴中心內的 ISV 發行者購買以 **授權為基礎** 的 SaaS 訂閱。 這表示您可以購買 ISV 發行者提供給您的任何 **授權型** SaaS 供應專案，包括您有權存取的 [專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 。 若要購買或管理來自 Isv (（例如以 **使用量為基礎**、計量付費或取用型供應專案，包括 Azure 應用程式、容器或 vm) 的優惠），您必須移至 [Azure 入口網站](https://portal.azure.com/)。 如需詳細資訊，請參閱下列主題。

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>在 Azure 入口網站中購買以使用量為基礎的訂用帳戶

相較于協力廠商 ISV 發行者的授權型 SaaS 訂用帳戶，以使用量為基礎的訂用帳戶首先需要客戶擁有 Azure 訂用帳戶。 商業 marketplace 的計費，以使用量為基礎的資源會落在客戶的 Azure 訂用帳戶底下。 當您的客戶擁有 Azure 訂用帳戶之後，CSP 方案中的合作夥伴就可以依照下列步驟，為他們購買商用 marketplace 訂用帳戶：

1. 登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)，然後從左側功能表中選取 [ **客戶** ]。

2. 選取特定的客戶，然後選取 [ **訂閱**]。  

3. 在以 **使用量為基礎**的訂用帳戶底下，選取 [ **所有資源**]。 這會帶您前往 Azure 管理入口網站。

4. 在 Azure 入口網站中，從左側功能表中選取 [ **建立資源** ]。

5. 選取 Azure Marketplace 清單頂端的 [ **查看全部** ]。

6. 若要縮小清單的範圍，請使用 Marketplace 清單頂端的篩選準則。 例如，您可以從 [發行者] 下拉式清單中選取 [ **Microsoft** **]** 或 [**夥伴**]，以僅查看 microsoft 或來自 ISV 發行者的供應專案。

7. 選擇特定的供應專案，然後選取 [ **建立**]。

## <a name="next-steps"></a>下一步

- [管理商業 marketplace 優惠](csp-commercial-marketplace-purchase.md)