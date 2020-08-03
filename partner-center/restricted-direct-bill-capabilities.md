---
title: 受限制的直接計費功能
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 直接帳單合作夥伴需求，以及如何避免受到限制的功能。 瞭解您的功能是否受到限制。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 46506548ec1848c983bfeabf44be74018e80be5e
ms.sourcegitcommit: e1c8bea4aaf807aebe99c125cb1fb6dc8fdfa210
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/30/2020
ms.locfileid: "87444770"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>受限制的直接帳單功能和 CSP 直接帳單合作夥伴所需的需求  

## <a name="overview"></a>概觀

直接帳單合作夥伴必須符合新的[需求](direct-partner-new-requirements.md)，才能繼續進行 CSP 直接帳單合作夥伴計畫。 否則，其對直接計費功能的存取權最終將會受到限制，且可能無法再執行特定工作，例如為客戶進行新的購買。

> [!Note]
> 不符合 CSP 直接帳單合作夥伴計畫新需求的直接帳單合作夥伴，將會在其直接帳單功能受到限制時通知 Microsoft。 這適用于所有的直接帳單合作夥伴，無論他們是否選擇[從直接帳單合作夥伴轉換為間接轉銷商](transition-direct-to-indirect.md)。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>如何判斷您的直接帳單功能是否受到限制

若要確認是否已限制從直接帳單合作夥伴租使用者到直接帳單功能的存取權，請遵循下列步驟。

1. 登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。

2. 移至 [**合作夥伴設定**] [  ->  **合作夥伴設定檔**]。

3. 在 [**程式資訊**] 下，尋找 [ **Microsoft Cloud 解決方案提供者狀態**]。

4. 如果程式狀態的值為 [**受限制**]，表示您的直接帳單合作夥伴租使用者對直接帳單功能的存取已受到限制。

## <a name="affected-direct-bill-capabilities"></a>受影響的直接帳單功能

如果您的直接帳單功能已受到限制，您就無法再于合作夥伴中心為您的客戶購買新的產品。 這種限制包括：

- Azure 訂用帳戶

- 以授權為基礎的訂閱

- 將新的附加元件新增至現有的授權型訂閱。

- 進行一次性購買的軟體和保留產品（例如，軟體訂閱、永久軟體和 Azure 保留的虛擬機器實例）。

您也不能使用 CSP 計畫下的[azure 合作夥伴共用服務供應](shared-services.md)專案來購買新的 azure 訂用帳戶供您自己使用。

現有的直接帳單訂閱不會受到影響。 它們仍然有效，而且是 autorenewed。 您將繼續直接向 Microsoft 收取費用，直到取消為止。 您仍然可以透過下列方式來管理現有的訂閱：

- 暫止現有的訂閱

- 調整現有授權型訂閱的授權計數

- 調整現有附加元件在訂用帳戶中的授權計數。 
 
    >[!Note] 
    >您無法將新的附加元件加入現有的訂用帳戶，因為它被視為新購買的訂閱。

- 部署新的 Azure 資源，並在現有的 Azure 訂用帳戶下管理現有的 Azure 資源。 這包括可透過 Azure marketplace 和 Visual Studio 訂用帳戶取得的資源。

除了新購買專案以外，您也無法在合作夥伴中心存取下列直接帳單功能：

- 您無法建立新的客戶租使用者。 合作夥伴中心的 [**客戶**] 頁面下的 [**建立客戶**] 選項將無法使用。

- 您無法對要求直接轉銷商關係的客戶產生邀請。 [合作夥伴中心] 的 [**客戶**] 頁面下的 [**要求轉售商關係**] 選項將無法使用。

    >[!NOTE]
    >在從直接帳單合作夥伴轉移至間接轉銷商的過程中，如果您已將您的直接帳單合作夥伴租使用者註冊為間接轉銷商，您可以改為向要求間接轉銷商關聯性的客戶產生邀請。

- 您無法建立新的沙箱租使用者。 每個直接帳單合作夥伴租使用者都可以建立一個沙箱租使用者，以供直接帳單 API 整合之用。 如果您先前尚未建立，則不允許您在直接帳單合作夥伴功能受到限制之後執行這項操作。  

## <a name="next-steps"></a>接下來的步驟

- [關於成為間接轉銷商的其他資訊](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [雲端解決方案提供者直接合作夥伴的新需求](direct-partner-new-requirements.md)