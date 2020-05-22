---
title: 遷移 Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將合格的 Dynamics 365 Business Edition 供應專案在到期前遷移至較新的版本。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 優惠，續約優惠，新的 Dynamics 365 Sku
ms.openlocfilehash: d49966db4a2c9de50b0723abf9ccd0fe589a442a
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795973"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>將 Dynamics 365 商務版提供移轉至較新版本

**適用於**

- 合作夥伴中心

**適當的角色**
- 全域系統管理員
- 使用者系統管理員
- 系統管理代理人
- 銷售代理人

自2019年1月1日起，使用 Dynamics 365 Business Edition 訂用帳戶的客戶將無法再續約這些舊版供應專案;現有的訂閱將不會在過期時自動更新。 在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日]。

為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。 我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。

如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。 有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。 您可以隨時將客戶移轉至新的方案。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>即將淘汰的 Dynamics 365 Business Edition

- Dynamics 365 for Finance and Operations，Business edition
- Dynamics 365 的商務小組成員版本

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-Dynamics 365 Business Edition 的新優惠

透過新的 Dynamics Business Central 供應專案，您的客戶可以連接其財務、銷售、服務和營運，以簡化商務程式、改善客戶互動，並做出更好的決策。 Dynamics 365 Business Central 是以雲端為基礎，僅供雲端解決方案提供者（CSP）方案合作夥伴使用。
Dynamics 365 Business Edition 客戶有資格在2020年6月30日前獲得新的商業中心優惠折扣轉換定價。

## <a name="transition-customers-to-new-product-plans"></a>將客戶轉換到新產品方案

 將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：

- 購買新訂閱
- 重新指派目前的使用者授權
- 取消舊訂閱

## <a name="purchase-the-new-plan-for-your-customer"></a>為您的客戶購買新方案

1. 從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。
2. 選取 [**新增訂**用帳戶]。
3. 選取您要從型錄購買的訂閱 (在此案例中為以上其中一個選項)，輸入授權數量，然後選取 **\[提交\]**。 

您的客戶現在會有舊的訂閱和新的訂用帳戶。 下一個步驟是將授權重新指派給客戶的使用者。

1. 從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。
2. 選取 [**使用者和授權**]。
3. 若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。 
4. 在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。 
5. 選取 [提交]  。 您將針對需要新授權的每位使用者執行此動作。 

將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。 

1. 從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。
2. 在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。

舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。 暫停的訂閱將在 120 天後自動解除佈建。 您的客戶將不會產生舊訂用帳戶的額外費用。
