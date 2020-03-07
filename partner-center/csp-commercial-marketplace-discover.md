---
title: 探索商業 marketplace 中的供應專案 |合作夥伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解 CSP 合作夥伴如何使用合作夥伴中心，從獨立軟體廠商（Isv）查看或搜尋 marketplace 提供的 SaaS 供應專案或定價。
author: MicheleHope
ms.author: v-mihope
keywords: 訂用帳戶，marketplace，商業 marketplace，協力廠商，ISV，SaaS 優惠，雲端解決方案提供者方案，CSP 計畫，CSP 合作夥伴
ms.localizationpriority: medium
ms.openlocfilehash: 23a31646165576842b625ec4f05a8da404fae01d
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340143"
---
# <a name="discover-offers-and-pricing-in-the-commercial-marketplace"></a>探索商業 marketplace 中的供應專案和定價

**適用於**

- 夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 全域系統管理員
- 系統管理代理人

當獨立軟體廠商（Isv）選擇在商業 marketplace 發佈供應專案時，他們也可以決定是否要在 CSP 計畫中提供供應專案。 如果他們選擇透過 CSP 方案銷售供應專案，CSP 合作夥伴應該會在合作夥伴中心的 Marketplace 區域看到該供應專案。 

如果 ISV 供應專案未如預期般出現在合作夥伴中心，可能是因為：

- ISV 決定不透過 CSP 計畫銷售供應專案。 例如，某些 ISV 產品可能已在商用 marketplace 的其他區域提供（例如[Microsoft AppSource](https://appsource.microsoft.com/)和[Azure Marketplace](https://azuremarketplace.microsoft.com/)），但可能不會顯示在合作夥伴中心 marketplace 中的 csp。

- ISV 決定讓供應專案僅限於所選的 CSP 合作夥伴數目。 如需專屬供應專案的詳細資訊，請參閱本說明主題稍後的。

- 供應專案類型可能無法透過合作夥伴中心或 Azure 入口網站 transactable （例如容器或某些以使用方式為基礎的優惠）。

- 此 ISV 供應專案可能不支援相關聯客戶的帳單國家/地區。

## <a name="view-marketplace-offers-in-partner-center"></a>在合作夥伴中心觀看 Marketplace 優惠

若要在 CSP 計畫中查看可用的商用 marketplace 優惠： 

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **CSP** ]。

2. 依序選取 [**銷售**] 和 [ **Marketplace**]。 根據預設，您會看到所有類型和類別目錄的產品。

3. 依類型或類別選取篩選。 您也可以使用 [**搜尋**] 來尋找特定關鍵字、供應專案名稱或 ISV 發行者的名稱。

4. 從清單中選取特定的產品供應專案。 這會帶您前往 [產品總覽] 索引標籤，您可以在其中深入瞭解供應專案。 此索引標籤上的資訊可能包括： 

    - 產品或供應專案的描述

    - ISV 發行者的詳細資訊

    - ISV 發行者所上傳之檔或行銷資料的連結

    - 適用于客戶支援、工程或 CSP 計畫連絡人的其他可能 ISV 連絡人

5. 若要查看供應專案可用方案、Sku 或價格的詳細資訊，請選取 [**方案 + 定價**] 索引標籤。此索引標籤會顯示：

    - 此供應專案可供您使用的市場

    - 適用于供應專案的 Sku 或方案清單

    - 每個可用 SKU 或方案的定價

## <a name="view-marketplace-offers-via-partner-center-apis"></a>透過合作夥伴中心 Api 來觀看 Marketplace 優惠

CSP 方案合作夥伴也可以使用 Api 來傳回合格供應專案的清單。 符合資格的供應專案只會提供給合作夥伴透過合作夥伴中心 marketplace 銷售的 SaaS ISV 優惠。 如需使用 Api 來識別目錄中供應專案的合作夥伴，請參閱指引以[取得市場](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)供應專案的清單。

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>在合作夥伴中心內查看最新的 Marketplace 供應專案定價

請遵循下列步驟，以取得與供應專案相關聯的最新定價詳細資料：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)，然後從左側導覽功能表中選取 [ **CSP** ]。

2. 依序選取 [**銷售**] 和 [ **Marketplace**]。 Marketplace 供應專案的清單隨即出現。

3. 向下流覽至 [ **Marketplace** ] 區段（在 [ **Azure 方案定價**] 底下），然後從右上角選取 [**匯出價格清單**]。 這會產生試算表，其中包含可從 ISV 發行者取得的 SaaS、授權型供應專案的最新定價資料。 某些 Azure 應用程式價格可能也會出現在這裡。 這是每日更新的資訊，因此您可以依自己的選擇，隨時檢查最新價格。

4. 如果 ISV 產品包含免費試用期，此試算表會顯示該產品的兩個數據列：

    - 一個資料列顯示免費試用價格為零。 這表示可以使用免費試用期間。

    - 另一個資料列顯示免費試用期結束後，將會套用的價格和條款。

身為 CSP 方案合作夥伴，您可能符合與特定商業 marketplace 供應專案相關聯的其他獎勵。 如需其他獎勵的詳細資訊，請參閱[csp 獎勵指南](https://aka.ms/partnerincentives)（需要 csp 登入）。

## <a name="learn-about-marketplace-exclusive-offers"></a>瞭解 marketplace 專屬優惠

Isv 可以選擇僅將其供應專案提供給 CSP 方案中的特定合作夥伴。 這就是所謂的專屬供應專案。 CSP 方案中的所有合作夥伴仍然可以在合作夥伴中心的商業市場中，看到所有 ISV 供應專案，包括標示為「獨家」的產品。

如果供應專案**未**標示為專屬，所有合作夥伴都可以購買該供應專案（假設所選客戶的計費國家/地區符合 ISV 供應專案的國家/地區可用性）。

不過，針對任何標示為「專屬」的供應專案，只有 ISV 所選取的合作夥伴才能購買該供應專案。

> [!NOTE]
> 如果您看到標示為「專屬」的供應專案，而您想要向客戶銷售，請直接與 ISV 聯繫，並要求取得銷售專屬供應專案的許可權。 當您查看專屬供應專案的詳細資料時，您可能會看到可供您選取的**連絡人 ISV**連結。

若要深入瞭解商業 marketplace 中的 ISV 體驗，請參閱[雲端解決方案提供者](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers)。

如需有關在 marketplace 中 CSP 體驗的詳細資訊，請參閱[商業 marketplace 總覽](csp-commercial-marketplace-overview.md)。

## <a name="next-steps"></a>後續步驟

- [購買商用 marketplace 優惠](csp-commercial-marketplace-purchase.md)