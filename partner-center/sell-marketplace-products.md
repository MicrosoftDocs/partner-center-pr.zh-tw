---
title: 銷售商業市集產品的訂用帳戶 | 合作夥伴中心
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 您可以使用合作夥伴中心，向您的客戶銷售由獨立軟體廠商 (ISV) 發佈到商業市集的軟體即服務 (SaaS) 產品訂用帳戶。
author: JnHs
ms.author: jenhayes
keywords: 訂閱, Marketplace, 協力廠商, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651641"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>銷售商業市集產品的訂用帳戶

**適用於**

- 合作夥伴中心

您可以使用合作夥伴中心，向您的客戶銷售由獨立軟體廠商 (ISV) 發佈到商業市集 ([Microsoft AppSource](https://appsource.microsoft.com/) 和 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) 的軟體即服務 (SaaS) 產品訂用帳戶。 這有助於讓您的業務差異化，還能為客戶提供滿足其特定商務需求的產品搭售方案。 您可以管理這些 Marketplace SaaS 產品的授權和訂用帳戶，就像 Microsoft 產品一樣。

如需商業市集的詳細資訊，請參閱 [Marketplace 常見問題集](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)。

> [!IMPORTANT]
> 只有軟體即服務 (SaaS) 商業市集訂用帳戶可在合作夥伴中心購買。 其他商業市集供應項目類型 (例如 Azure 應用程式、容器或虛擬機器) 則是透過 Azure 入口網站進行管理，並根據耗用量計費。 需要現有的 Azure 訂閱，才能透過 Azure 入口網站啟用隨用隨付解決方案。

## <a name="view-marketplace-offers-and-pricing"></a>檢視 Marketplace 供應項目和定價

若要檢視所有可用的商業市集供應項目，請從左側導覽功能表中選取 [Marketplace]。 根據預設，您會看到所有類型和類別目錄的產品。 您可以依類型和/或類別篩選，或使用搜尋方塊來搜尋特定關鍵字。 選取產品以查看發行者和可用 SKU 的相關資訊，包括是否提供免費試用期。

> [!NOTE]
> 商業市集中提供的某些產品可能不會在這裡顯示。 ISV 可以決定是否要在合作夥伴中心將其產品提供給雲端解決方案提供者 (CSP) 合作夥伴。 如果您在商業市場中看到您想要透過合作夥伴中心提供給客戶的產品，請在產品清單中尋找發行者的連絡人資訊，並讓他們知道您有興趣。

商業市集產品的價格可能經常變更。 若要取得所有商業市集產品的最新定價資訊，請選取 [Marketplace] 頁面右上角的 [匯出價格清單]。 這會產生包含所有定價資料的試算表。 此定價資訊每天都會更新，因此您可以依您想要的頻率來查看，以取得最新價格。

> [!TIP]
> 如果此清單中的產品提供免費試用版，試算表中會針對該產品包含兩個資料列。 一個資料列會顯示零的價格，表示有可用的免費試用版。 另一個資料列將包含試用期結束後將套用的價格和期間。
>
> 如果此清單中的產品使用[計量付費](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing)計費，期間欄位將是空白。

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>為您的客戶購買商業市集產品

購買商業市集 SaaS 產品訂用帳戶的程序與購買 Microsoft 產品訂用帳戶相同。 購買訂用帳戶之前，您必須先選取客戶或加入新的客戶。

為客戶新增訂閱時，您可以選取 [發行者] 篩選器中的 [合作夥伴]，以選擇僅查看 ISV 提供的 Marketplace 供應項目。 如需詳細資訊，請參閱[建立新的訂閱](create-a-new-subscription.md)。

請注意，您在 **Marketplace** 頁面中看到的某些供應項目可能無法供特定客戶使用。 可用性可能會受到一些因素的影響，包括 ISV 是否支援客戶的帳單國家/地區。

> [!TIP]
> 您也可以使用[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/) 來為您的客戶建立商業市集訂用帳戶。 如需詳細資訊，請參閱[建立商業市集產品的訂用帳戶](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。

針對商業市集產品的訂用帳戶，您可以在取消期間內 (每月訂用帳戶為 24 小時，每年訂用帳戶為 14天) 選擇[取消訂用帳戶](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription)。 您也可以[選擇是否要自動更新訂閱](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription)。

## <a name="license-activation-for-commercial-marketplace-products"></a>商業市集產品的授權啟用

對於軟體即服務 (SaaS) 供應項目類型，授權指派和啟用是透過發行產品的獨立軟體廠商 (ISV) 來管理。 若要完成此程式，您必須造訪發行者的網站，搭配授權碼使用個人化連結，讓發行者能夠識別您的特定購買。 您可以在購買 SaaS 供應項目之後出現的 [確認] 頁面上以及在 [訂閱] 頁面上 (在該供應項目的資料列中) 找到此連結。 您也可以[使用合作夥伴中心 API 來擷取此連結](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)。

當您使用此連結流覽發行者的網站時，您會看到布建和指派授權或完成安裝程式所需的其他資訊或動作。 所需的步驟可能會根據發行者和供應項目而有所不同。 您必須負責提交任何必要的資訊 (或將 URL 傳送給您的客戶，以直接提供此資訊)。 提供必要資訊之後，發行者將會佈建並指派適當的授權。 只有在成功指派授權之後，才會對訂閱開始計費。

## <a name="access-billing-info-for-commercial-marketplace-products"></a>存取商業市集產品的帳單資訊

若為商業市集產品，計費期間會從日曆月份的第一天開始，並在日曆月份的最後一天結束。 我們會讓您的發票在下個月的第8天提供。 您可以在合作夥伴中心或使用合作夥伴中心 API 來存取這些發票。

如需詳細資訊，請參閱[了解合作夥伴中心的帳單類型](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges)。

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>為使用商業市集產品的客戶提供支援

就像 Microsoft 產品一樣，您應該是客戶洽詢帳單及訂閱管理相關問題的第一個連絡窗口。 如需技術支援，您必須連絡發行者。 Microsoft 不供應商業 marketplace 產品的支援，但會將發行者的支援連絡人資訊提供給您。

如需詳細資訊，請參閱[支援商業市集產品](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products)和[為您的客戶提供支援](https://docs.microsoft.com/partner-center/customer-support)。

## <a name="manage-subscriptions-using-partner-center-apis"></a>使用合作夥伴中心 API 管理訂閱

您可以使用合作夥伴中心 API 來建立商業市集產品的訂用帳戶。 若要這樣做，您必須先取得市場供應項目的清單，然後建立並提交特定商業市集訂用帳戶的訂單。 最後，您會取得訂用帳戶的啟用連結。

您也可以使用合作夥伴中心 API 來執行生命週期管理，並管理這些訂閱的發票。

如需詳細資訊，請參閱[建立商業市集產品的訂用帳戶](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)。