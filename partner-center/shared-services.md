---
title: 新增 Azure 合作夥伴共用服務
description: 使用 Azure 合作夥伴共用服務購買 Azure 訂用帳戶以供您自己使用，並具有統一的方法來購買、追蹤和管理 Azure。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 93ee3e142bf11c3b329fd27ec7320b93aea780b8
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532033"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>新增 Azure 合作夥伴共用服務，讓合作夥伴可以購買 Azure 訂用帳戶以供自己使用

 
**適當的角色**

- 全域系統管理員
- 系統管理代理人
- 銷售代理人

Azure 合作夥伴共用服務是一種新的供應類型，適用於雲端解決方案提供者計畫中的合作夥伴，讓合作夥伴購買自己要使用的 Azure 訂閱。 它提供合作夥伴能夠使用統一的方式來購買、追蹤和管理 Azure 的機會，此外還能整合他們與 Microsoft 的 Azure 授權和經銷合約。 有了 Azure 合作夥伴共用服務，合作夥伴現在擁有相同的彈性，可在 CSP 中使用 Azure 訂用帳戶，就像在 Microsoft Enterprise 合約和 Web Direct 程式中一樣，開啟案例，例如：建立開發和測試環境、部署內部工作負載，以及裝載共用服務或多租使用者應用程式。  

## <a name="create-the-shared-services-tenant"></a>建立共用服務租用戶

1. 移至 [ **設定**  >  **帳戶設定**  >  **共用服務** ]。

   :::image type="content" source="images/sharedservices2.png" alt-text="帳戶設定 > 共用服務":::

2. 如果您還沒有共用服務租用戶，請按一下 **\[建立共用服務\]** 。

   :::image type="content" source="images/sharedservices3.png" alt-text="建立共用服務":::

3. 這會建立共用服務租用戶並購買 Azure 雲端解決方案提供者共用服務訂閱，以用於共用資源和內部工作負載。

   :::image type="content" source="images/sharedservices5.png" alt-text="建立租用戶並購買訂閱":::

## <a name="about-the-azure--internalshared-services-offer"></a>關於「Azure - 內部/共用服務」供應項目

- Azure 內部/共用服務訂用帳戶是 CSP 中新的 Azure 供應專案類型，可透過合作夥伴取得以供自己使用 Azure 的合作夥伴中心來存取。

- Azure-內部/共用服務供應專案符合折扣和獎勵的資格。  Azure 合作夥伴共用服務訂用帳戶符合資格，可用於購買 ri。

- 「Azure – 內部/共用服務」供應項目只適用於共用服務租用戶。

- Azure 內部/共用服務訂用帳戶的主要用途是讓您可以將 Azure 用於自己的開發用途。 您用來布建此供應專案的共用租使用者，無法用於其他服務，例如 Office 365 或 Dynamics 授權。

- 您可以取消訂閱，就如同其他訂閱一樣。 移至 [ **設定** ]  >  **視圖所有設定**  >  **共用服務** 。 選取 \[Azure – 內部/共用服務訂閱\]，然後取消它。

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>存取 Azure 合作夥伴共用服務使用詳細資料

您可在雲端解決方案提供者發票和對帳檔案上找到 Azure 使用量。 它們在發票上會當做 Microsoft Azure 明細項目的一部分。 詳細的使用資訊可在針對租用戶所記錄的對帳檔案中取得，此租用戶是專為此供應項目而建立。

## <a name="azure-partner-shared-services-pricing"></a>Azure 合作夥伴共用服務定價

若要查看 Azure 合作夥伴共用服務的新定價檔案，請前往 **銷售**  >  **定價和優惠** ，然後選取目前月份的價格清單。 在接下來幾個星期，也會發行特定的費率卡 api。

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace 優惠和 Azure 合作夥伴共用服務

從2019年3月1日起，Azure 合作夥伴共用服務 (APSS) 不再支援 Marketplace 優惠。

|**Marketplace 支援**   |**2019年3月1日前支援的 APSS**|**2019年3月1日之後**|
|---------------------------|:----------------------------|:-------------------|
|攜帶您自己的授權 (BYOL) 和免費服務   | 是   | 否|
|其他協力廠商 marketplace 優惠   | 否   |否|

使用 APSS 部署 BYOL 或免費服務的合作夥伴將不會受到影響;不過，在2019年3月1日之後，他們將無法購買新的 BYOL 或免費服務。

若要充分利用 Marketplace 供應專案的完整目錄 (而不只是 BYOL 和免費的服務) ，我們建議 CSP 合作夥伴使用 web direct Azure 訂用帳戶來部署共用服務。  我們鼓勵先前已從 Marketplace 部署協力廠商 BYOL 和免費服務資源的 CSP 合作夥伴，並想要繼續使用並部署更多協力廠商供應專案，以將 APSS 訂用帳戶遷移至 web direct [遷移現有的 Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)訂用帳戶。

在2019年3月1日之後計畫繼續使用 APSS 訂用帳戶，並想要部署新的協力廠商 [BYOL 服務](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) 或免費服務的合作夥伴，可以遵循 isv 的指示，將這些服務部署至其 APSS 訂用帳戶。

## <a name="next-steps"></a>後續步驟

- [透過雲端解決方案提供者銷售軟體訂閱](csp-software-subscriptions.md)