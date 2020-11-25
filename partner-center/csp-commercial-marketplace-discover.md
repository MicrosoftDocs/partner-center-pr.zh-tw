---
title: 探索優惠-商業市場
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 合作夥伴如何使用合作夥伴中心來查看或搜尋 marketplace 中的 SaaS 供應專案，以及獨立軟體廠商 (Isv) 的定價。
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e89473cf095be4cc87c96f1c2a6d0da224eccedd
ms.sourcegitcommit: f34f2f69e6df4f260479a205d94010cf47987ff2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/25/2020
ms.locfileid: "96038842"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>探索合作夥伴中心商用 marketplace 中的優惠和定價

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

當獨立軟體廠商 (Isv) 選擇在商業 marketplace 中發佈供應專案時，他們也可以決定是否要讓供應專案可在 CSP 方案中使用。 如果他們選擇透過 CSP 方案銷售供應專案，CSP 合作夥伴應該會在合作夥伴中心 Marketplace 區域中看到該供應專案。

如果 ISV 供應專案未如預期般出現在合作夥伴中心中，可能是因為：

- ISV 決定不透過 CSP 方案銷售供應專案。 例如，某些 ISV 產品可能已在商用 marketplace 的其他區域中提供 (例如 [Microsoft AppSource](https://appsource.microsoft.com/) 和 [Azure Marketplace](https://azuremarketplace.microsoft.com/)) ，但可能不會針對合作夥伴中心 marketplace 中的 CSP 方案中的合作夥伴所顯示。

- ISV 決定將供應專案僅提供給一系列精選的 CSP 合作夥伴。 如需專屬優惠的詳細資訊，請參閱本說明主題稍後的。

- 供應專案類型可能無法透過合作夥伴中心或 Azure 入口網站 (例如容器或某些以使用量為基礎的供應專案) 進行可交易。

- 此 ISV 供應專案可能不支援相關客戶 () 的計費國家/地區。

## <a name="view-marketplace-offers-in-partner-center"></a>在合作夥伴中心中查看 Marketplace 供應專案

若要在 CSP 方案中查看可用的商業 marketplace 供應專案：

1. 登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **CSP** ]。

2. 選取 [ **銷售**]，然後選取 [ **Marketplace**]。 根據預設，您會看到所有類型和類別目錄的產品。

3. 依類型或類別選取篩選。 您也可以使用 **搜尋** 來尋找特定關鍵字、供應專案名稱或 ISV 發行者的名稱。

4. 從清單中選取特定的產品供應專案。 這會將您帶到 [產品總覽] 索引標籤，您可以在其中深入瞭解供應專案。 此索引標籤上的資訊可能包括： 

    - 產品或供應專案的描述

    - ISV 發行者的詳細資訊

    - ISV 發行者所上傳之檔或行銷資料的連結

    - 客戶支援、工程或 CSP 方案連絡人的其他可能 ISV 連絡人

5. 若要查看供應專案的可用方案、Sku 或價格的詳細資訊，請選取 [ **方案 + 定價** ] 索引標籤。此索引標籤會顯示您：

    - 您可以使用這項供應專案的市場

    - 適用于供應專案的 Sku 或方案清單

    - 每個可用 SKU 或方案的定價

## <a name="view-marketplace-offers-via-partner-center-apis"></a>透過合作夥伴中心 Api 觀看 Marketplace 優惠

CSP 方案合作夥伴也可以使用 Api 來傳回合格供應專案的清單。 合格供應專案只會提供給合作夥伴透過合作夥伴中心 marketplace 銷售的 SaaS ISV 供應專案。 針對使用 Api 來識別目錄中供應專案的合作夥伴，請參閱指導方針以 [取得市場](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)供應專案清單。

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>在合作夥伴中心中查看最新的 Marketplace 供應專案定價

請依照下列步驟取得與供應專案相關聯的最新定價詳細資料：

1. 登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **CSP** ]。

2. 選取 [ **銷售**]，然後選取 [ **定價和** 供應專案]。

3. 向下滾動至 **marketplace** 區段，選取位置並下載 **Marketplace 定價**。 這會產生一份試算表，其中包含適用于 SaaS 的最新定價資料、授權型供應專案，以及 ISV 發行者所提供的計量付費供應專案。 某些 Azure 應用程式定價可能也會出現在這裡。 這項資訊會每日更新，因此您可以在選擇的時候，檢查其是否有最新的價格。

4. 如果 ISV 產品包含免費的試用期間，試算表會顯示該產品的兩個數據列：

    - 一個資料列會顯示零的免費試用價格。 這表示可以使用免費試用期間。

    - 另一列則顯示免費試用期結束後將套用的價格和條款。

作為 CSP 方案合作夥伴，您可能有資格獲得與特定商業 marketplace 供應專案相關聯的其他獎勵。 如需其他獎勵的詳細資訊，請參閱 [csp 獎勵指南](https://aka.ms/partnerincentives) (需要 csp 登入) 。

## <a name="learn-about-marketplace-exclusive-offers"></a>瞭解 marketplace 專屬優惠

Isv 可以選擇讓其供應專案僅適用于 CSP 方案中的特定合作夥伴。 這就是所謂的專屬供應專案。 CSP 方案中的所有合作夥伴仍然可以在合作夥伴中心商用 marketplace 中查看所有 ISV 供應專案，包括標示為專屬的供應專案。

如果供應專案 **未** 標示為專屬，則所有合作夥伴都可以購買該供應專案 (假設所選客戶的計費國家/地區符合 ISV 供應專案的國家/地區可用性) 。

不過，針對任何標記為專屬的供應專案，只有 ISV 所選取的合作夥伴才能購買該供應專案。

> [!NOTE]
> 如果您看到您想要銷售給客戶的供應專案，請直接與 ISV 聯繫，並要求銷售專屬供應專案的許可權。 當您查看專屬供應專案的詳細資料時，您可能會看到可供您選取的 **連絡人 ISV** 連結。

若要深入瞭解商用 marketplace 中的 ISV 體驗，請閱讀 [雲端解決方案提供者](/azure/marketplace/cloud-solution-providers)。

如需 marketplace 中 CSP 體驗的詳細資訊，請參閱 [商業 marketplace 總覽](csp-commercial-marketplace-overview.md)。

## <a name="next-steps"></a>後續步驟

- [購買商用 marketplace 優惠](csp-commercial-marketplace-purchase.md)