---
title: 受限制的直接計費功能
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 直接帳單合作夥伴的需求，以及如何避免受限制的功能。 找出您的功能是否受到限制。
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38fe5d03784d0fcf0796545d31e8272f316d2878
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/06/2021
ms.locfileid: "99623978"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>受限制的直接帳單功能，以及 CSP 直接帳單合作夥伴所需的需求  

## <a name="overview"></a>概觀

直接帳單合作夥伴必須符合新的 [需求](direct-partner-new-requirements.md) ，才能保留在 CSP 直接帳單合作夥伴計畫中。 否則，其對直接計費功能的存取權最終將會受到限制，且可能無法再執行特定工作，例如為客戶進行新的購買。

> [!Note]
> 不符合 CSP 直接帳單合作夥伴方案新需求的直接帳單合作夥伴，將會在其直接帳單功能受到限制時收到通知。 這適用于所有直接帳單合作夥伴，無論他們是否選擇 [從直接帳單合作夥伴轉換為間接轉銷商](transition-direct-to-indirect.md) 。  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>如何判斷您的直接帳單功能是否受到限制

若要確認直接帳單合作夥伴租使用者的存取是否受到限制，請遵循下列步驟。

1. 登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。

2. 移至 **帳戶設定**  ->  **法律聲明設定檔**。

3. 在 [ **程式資訊**] 底下，尋找 **Microsoft 雲端解決方案提供者狀態**。

4. 如果程式狀態的值 **受限制**，這表示您的直接帳單合作夥伴租使用者的直接帳單功能存取權已受限制。

## <a name="affected-direct-bill-capabilities"></a>受影響的直接帳單功能

如果您的直接帳單功能受到限制，您將無法再于合作夥伴中心中為客戶購買新的產品。 這種限制包括：

- Azure 訂用帳戶

- 以授權為基礎的訂用帳戶

- 將新的附加元件加入至現有的授權型訂閱。

- 進行一次性的軟體和保留產品購買 (例如，軟體訂用帳戶、永久軟體和 Azure 保留的虛擬機器實例) 。

您也無法使用 CSP 方案下的 [azure 合作夥伴共用服務供應](shared-services.md) 專案來購買新的 azure 訂用帳戶，以供您自己使用。

現有的直接帳單訂用帳戶不會受到影響。 它們仍然有效，而且會自動更新。 您將繼續由 Microsoft 直接向您收取費用，直到取消為止。 您仍然可以透過下列方式管理現有的訂閱：

- 暫止現有的訂閱

- 調整現有授權型訂用帳戶的授權計數

- 將現有附加元件的授權計數調整至訂用帳戶。 
 
    >[!Note] 
    >您無法將新的附加元件加入至現有的訂用帳戶，因為它會被視為新的購買訂閱。

- 部署新的 Azure 資源，並在現有的 Azure 訂用帳戶下管理現有的 Azure 資源。 這包括可透過 Azure Marketplace 和 Visual Studio 訂閱取得的資源。

除了新的購買，您也無法在合作夥伴中心中存取下列直接帳單功能：

- 您無法建立新的客戶租使用者。 合作夥伴中心中的 [**客戶**] 頁面下的 [**建立客戶**] 選項將無法使用。

- 您無法對要求直接轉銷商關係的客戶產生邀請。 合作夥伴中心中的 [**客戶**] 頁面下的 [**要求轉售商關聯** 性] 選項將無法使用。

    >[!NOTE]
    >從直接帳單夥伴轉換為間接轉銷商的過程中，如果您已經將直接帳單合作夥伴租使用者註冊為間接轉銷商，您可以改為向要求間接轉銷商關係的客戶產生邀請。

- 您無法建立新的沙箱租使用者。 每個直接帳單合作夥伴租使用者都可以建立一個沙箱租使用者，以供直接帳單 API 整合之用。 如果您先前未建立，則不允許您在直接帳單夥伴功能受到限制之後進行。  

## <a name="next-steps"></a>接下來的步驟

- [關於成為間接轉銷商的其他資訊](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [雲端解決方案提供者直接合作夥伴的新需求](direct-partner-new-requirements.md)
