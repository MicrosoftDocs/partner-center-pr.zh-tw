---
title: 為您的客戶購買商用 marketplace 產品或優惠 |合作夥伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 方案合作夥伴如何使用合作夥伴中心 marketplace，讓客戶能夠從獨立軟體廠商（Isv）購買 SaaS 優惠。
author: MicheleHope
ms.author: v-mihope
keywords: 訂用帳戶，marketplace，商業 marketplace，協力廠商，ISV，SaaS 優惠，雲端解決方案提供者方案，購買供應專案，購買訂閱
ms.localizationpriority: medium
ms.openlocfilehash: 3dd3facf79e0e33a6dfc35a162c444a13a19b256
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253796"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>在合作夥伴中心為您的客戶購買商用 marketplace 產品

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

身為雲端解決方案提供者（CSP）方案的合作夥伴，您可以使用商業 marketplace，向獨立軟體廠商（Isv）所提供的特定軟體即服務（SaaS）產品購買客戶訂閱。 

藉由為您的客戶提供 ISV SaaS 訂用帳戶，您可以協助區分您的企業。 您也可以讓客戶存取軟體配套，以解決其特定的商務需求。 您可以從 ISV 發行者管理這些 marketplace SaaS 產品的授權和訂用帳戶，就像管理 Microsoft 產品的授權和訂閱一樣。

您可以購買以**授權為基礎**的 SaaS 訂用帳戶或以**使用量為基礎的**訂用帳戶。 若要深入瞭解授權型和以使用量為基礎的計費差異，請參閱[計費基本概念](billing-basics.md)。

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>在合作夥伴中心購買以授權為基礎的 SaaS 訂用帳戶

您可以使用您用來購買 Microsoft 產品訂閱的相同程式，來購買 ISV 發行者所提供之授權型 SaaS 產品的訂閱。

若要在合作夥伴中心購買以授權為基礎的 SaaS 訂用帳戶，請參閱[建立、暫停或取消客戶訂閱](create-a-new-subscription.md#create-a-new-subscription)。

您也可以使用[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/) 來為您的客戶建立商業市集訂用帳戶。 （如需使用合作夥伴中心 Api 的詳細資訊，請參閱[建立商業 marketplace 產品的訂](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)用帳戶）。

>[!IMPORTANT]
> 身為 CSP 計畫的合作夥伴，您只能從合作夥伴中心內的 ISV 發行者購買以**授權為基礎**的 SaaS 訂閱。 這表示您可以購買 ISV 發行者已提供給您的任何**授權型**SaaS 供應專案，包括您有權存取的[專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。 若要向 Isv 購買或管理其他的商用 marketplace 供應專案（例如，以**使用量為基礎**、計量付費或以耗用量為基礎的優惠，涉及 Azure 應用程式、容器或 vm），您必須移至[azure 管理入口網站](https://portal.azure.com/)。 如需詳細資訊，請參閱下列主題。

## <a name="purchase-usage-based-subscriptions-in-the-azure-management-portal"></a>在 Azure 管理入口網站中購買以使用量為基礎的訂用帳戶

相較于協力廠商 ISV 發行者的授權型 SaaS 訂用帳戶，以使用方式為基礎的訂用帳戶會先要求客戶擁有 Azure 訂用帳戶。 以使用方式為基礎的資源會在客戶的 Azure 訂用帳戶下計費，適用于商業 marketplace。 一旦您的客戶擁有 Azure 訂用帳戶，CSP 方案中的合作夥伴就可以依照下列步驟，為他們購買商業 marketplace 訂用帳戶：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)，然後從左側功能表中選取 [**客戶**]。

2. 選取特定的客戶，然後選取 [訂用帳戶 **]。**  

3. 在 [以**使用量為基礎**的訂用帳戶] 下，選取 [**所有資源**]。 這會帶您前往 Azure 管理入口網站。

4. 在 Azure 管理入口網站中，從左側功能表中選取 [**建立資源**]。

5. 選取 [Azure Marketplace] 清單頂端的 [**查看全部**]。

6. 若要縮小清單範圍，請使用 Marketplace 清單頂端的篩選器。 例如，您可以從 [發行者] 下拉式清單中選取 [ **Microsoft** **]** 或 [**合作夥伴**]，只查看 microsoft 或 ISV 發行者的供應專案。

7. 選擇特定的供應專案，然後選取 [**建立**]。

## <a name="next-steps"></a>後續步驟

- [管理商用 marketplace 優惠](csp-commercial-marketplace-purchase.md)