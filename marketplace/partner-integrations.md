---
title: Azure Marketplace 合作夥伴整合
description: 瞭解與 Azure 環境整合 Azure Marketplace 的解決方案，並取得 Microsoft 合作夥伴提供的部署指南連結。
ms.service: partner-services
ms.topic: conceptual
author: dsindona
ms.author: dsindona
ms.date: 11/16/2020
ms.openlocfilehash: 7c97936e7764361c21503eca174433029707cf69
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691647"
---
# <a name="azure-marketplace-partner-integrations"></a>Azure Marketplace 合作夥伴整合

瞭解如何將合作夥伴解決方案整合到您的 Azure 環境。 本文提供每個解決方案的總覽，以及詳細部署指南的連結。 解決方案會依字母順序列出。 

## <a name="apache-kafka-on-confluent-cloud"></a>Confluent 雲端上的 Apache Kafka

![Confluent 雲端](./media/partners/confluent-cloud.png)

除了您的雲端應用程式之外，Azure 還可讓您與 Confluent Cloud 整合。 Confluent 客戶通常會在 Azure 入口網站與 Confluent 雲端之間流覽。 例如，使用者在 Azure Marketplace 購買 Confluent 雲端供應專案之後，他們就必須設定 Confluent Cloud 的帳戶。 此程式增加了複雜性和時間，而且需要使用者管理兩個入口網站之間的設定和資源。 為了降低跨平臺管理的負擔，Microsoft 與 Confluent Cloud 合作，建立了從 Azure 到 Confluent Cloud 的整合布建層。 解決方案可在 Azure Marketplace 中取得，並提供在 Azure 上使用 Confluent 雲端供應專案的無縫體驗

解決方案會使用在 Azure 中啟用的資源提供者來布建 Confluent 雲端資源。 這可讓使用者透過 Azure 入口網站、Azure CLI 和 Azure Sdk 來存取即時事件串流。 Confluent Cloud 擁有並執行 SaaS 應用程式，其中包括環境、叢集、主題、API 金鑰和受控連接器。

與 Confluent Cloud 的深度整合可提供下列功能：

- 使用完全受控的基礎結構，從 Azure 入口網站布建新的 Confluent Cloud 組織資源。
- 使用 Azure Active Directory，簡化從 Azure 到 Confluent Cloud 的單一登入;Confluent Cloud 入口網站不需要個別的驗證。
- 透過 Azure 訂用帳戶發票來取得 Confluent 雲端耗用量費用的統一帳單。
- 從 Azure 入口網站管理 Confluent 雲端資源，並在 [ **所有資源** ] 頁面中，連同您的 Azure 資源一起追蹤它們。

[Confluent 雲端部署指南](https://docs.confluent.io/current/cloud/marketplace/index.html)

關於 Confluent on Azure 的相關問題，請移至 [https://support.confluent.io](https://support.confluent.io) 。 如果您是第一次使用者，請先重設您的密碼，然後再登入 Confluent 支援入口網站。 如果您沒有包含 Confluent 的帳戶，請傳送電子郵件至 [cloud-support@confluent.io](mailto:cloud-support@confluent.io) 。

## <a name="datadog"></a>Datadog

![DataDog 標誌](./media/partners/datadog.png)

Datadog 為 Azure 使用者提供可檢視性和安全性工具，以瞭解應用程式在混合式和多重雲端環境中的健全狀況和效能。 但是，設定所需的整合通常需要在 Azure 入口網站和 Datadog 之間流覽。 為了簡化跨入口網站的設定和資源管理，Microsoft 與 Datadog 合作，在 Azure 上建立整合式 Datadog 解決方案。 此解決方案可透過 Azure Marketplace 提供順暢的體驗，讓 Azure 客戶能夠使用 Datadog 的雲端監視解決方案。

請參閱 [Azure 監視器檔](/azure/azure-monitor/platform/partners#datadog) ，以深入瞭解此解決方案並註冊公開預覽。

## <a name="next-steps"></a>後續步驟

- [Azure Marketplace 線上商店](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn：建立 Azure 帳戶](/learn/modules/create-an-azure-account/)
