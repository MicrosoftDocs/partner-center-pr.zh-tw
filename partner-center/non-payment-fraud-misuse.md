---
title: 管理未付款、詐騙或濫用
description: 瞭解線上交易涉及的各種風險，以及在合作夥伴中心中管理和減輕這些風險的最佳作法。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 43a35f91be9ce656157065a3d19b3643ddeff68a
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999292"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>在合作夥伴中心內管理未付款、詐騙或誤用

適用於：

- 合作夥伴中心
- Microsoft Cloud for US Government 適用的合作夥伴中心

**適當的角色**
- 全域系統管理員
- 使用者系統管理員
- 系統管理代理人
- 帳單系統管理員

您必須承擔因客戶以詐騙方式購買和/或已購買服務客戶未付款的行為而帶來的財務風險。 因此， *我們強烈建議您放置防詐騙防護和偵測風險降低控制措施*。

為了避免和/或解決詐騙活動或濫用問題，請務必了解潛在的風險，並擬定可以降低暴露於風險之機會的原則和做法。

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>強制使用 Microsoft 可接受的使用原則

如果 Microsoft 偵測到合作夥伴或客戶活動，但我們確認或懷疑違反了可接受的使用原則，我們將採取強制執行步驟。 客戶可以立即暫停。 您將會收到強制動作的通知，或由 Microsoft 對您的要求進行更新。

## <a name="abuse-of-service-risks"></a>服務風險濫用

**濫用服務** 風險表示使用雲端服務的客戶違反了 Microsoft 可接受的使用原則。

### <a name="examples-of-abuse-of-service"></a>服務濫用的範例

這些違反 Microsoft 可接受使用原則的範例可能包括：

- 垃圾郵件
- 駭客入侵
- 分散式阻斷服務 (DDoS) 攻擊
- 比特幣挖礦
- 惡意程式碼散發
- 轉售盜取的訂用帳戶

## <a name="theft-of-service-risks"></a>服務風險遭竊

**服務風險遭竊** 表示不打算支付取用服務的客戶。 這種遭竊可能牽涉到使用遭竊的付款儀器、提供錯誤的帳單資訊，以及/或預設為未付餘額。

### <a name="examples-of-service-theft"></a>服務遭竊的範例

這些線上交易風險的範例可能包括：

- 未在 person ( 「信用卡未存在」交易中發生的交易) 
- 詐稱身分
- 在收到初始付款之前布建和使用的服務
- 適用于線上詐騙的新興市場及/或高風險區域
- 由不良執行者自動建立及購買帳戶

## <a name="managing-online-risk"></a>管理線上風險

您可以使用下列建議來協助您開發原則和做法，以降低您的客戶關係生命週期中對線上交易風險的風險。

### <a name="onboarding-new-customers"></a>將新客戶上架

在新客戶上線時，降低線上風險的建議包括：

- 在可能的情況下，與客戶建立個人關係 (例如，透過電話) 聯絡客戶。
- 透過更好的方法來驗證客戶的認證和背景 (例如使用點數 bureaus 或商業商業報表機關) 。
- 在註冊期間使用多重要素驗證 (例如 SMS 驗證) ，以將建立和購買機器人帳戶的風險降至最低。
- 使用服務 (管理和追蹤身分識別，例如數位身分識別服務) 。
- 透過嚴格的信用卡詐騙偵測系統來評估客戶的財務優勢。
- 建立明確的集合原則。 詳細說明您的集合流程，以及當訂用帳戶的存取權會受到非付款的影響。  (您可以停用存取或 [暫止客戶的](create-a-new-subscription.md#suspend-a-subscription) 非付款訂用帳戶。 ) 

### <a name="managing-customer-accounts"></a>管理客戶帳戶

在購買後管理客戶帳戶的建議包括：

- 實行可快速接收、評論、處理及回應 Microsoft 通知的程式。
- 與客戶合作，瞭解其雲端使用量的商務需求，並設定適當的監視閾值。  (例如，您可以在合作夥伴中心中 [設定每月的 Azure 支出預算](set-an-azure-spending-budget-for-your-customers.md) 。 此瞭解可讓您監視每月客戶的使用方式，並在客戶接近其預算時收到通知。 ) 
- 定期監視 [客戶活動記錄](activity-logs.md) ，以協助及早偵測詐騙。
- 偵測到可疑的活動時，採取快速動作。
- 避免將訂用帳戶的完整系統管理存取權授與客戶，而不需要先履行風險降低措施

### <a name="managing-customer-billing"></a>管理客戶帳單

管理客戶帳單後購買的建議包括：

- 在初始交易與計費之前要求預付款。
- 請勿接受高風險的付款條件 (例如預付卡或預存值卡) 。
- 監視客戶款項和過時的帳戶是否應收帳款。 積極地強制執行標準欠款程式，以進行延遲的付款或非付款。

如需降低線上風險的詳細策略，請參閱[線上交易風險管理指南。](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
