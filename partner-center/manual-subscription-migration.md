---
title: 遷移合格的 Dynamics 365 訂閱
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何從合格的基本 Dynamics 365 訂閱遷移至新的訂用帳戶，然後再讓現有的訂閱過期。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 優惠，續約優惠，新的 Dynamics 365 Sku
ms.openlocfilehash: 5225ff60399cd491009ecb16e4c17b4fc05c0052
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949641"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>將 Dynamics 365 和 Customer Engagement Plan 從基本 （合格的供應項目） 移轉至較新版本

**適用於**

-  合作夥伴中心

**適當的角色**
-   全域系統管理員
-   使用者系統管理員
-   系統管理代理人
-   銷售代理人

自2019年1月1日起，從基本（合格供應專案）訂用帳戶使用 Dynamics 365 for Sales/Customer Engagement 方案的客戶，已無法再續約這些舊供應專案;現有的訂閱將不會在過期時自動更新。 在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為「從 [日期] 自動續約于 [日期] 的到期日]。 

為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。 我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。

如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。 有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。 您可以隨時將客戶移轉至新的方案。 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 提供淘汰

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic （限定供應專案）教職員版
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic （合格供應專案）適用于學生
- Dynamics 365 for Sales Enterprise Edition （政府定價） CRMOL Basic （合格供應專案）
- 來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （合格供應專案）
- 適用于教職員的 Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （限定供應專案））
- Dynamics 365 for Sales Enterprise Edition （從 SA for CRM Basic （合格供應專案）適用于學生）
- 來自 SA for CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）（合格供應專案）
- 適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）
- 適用于教職員的 Dynamics 365 for Sales Enterprise Edition 附加元件
- 適用于學生的 Dynamics 365 for Sales Enterprise Edition 附加元件（合格供應專案）
- 適用于 CRM Basic 的 Dynamics 365 for Sales Enterprise Edition （政府定價）附加元件（合格供應專案）
- Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）
- Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價） CRMOL Basic （合格優惠）
- 適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL 基本（合格供應專案）
- Dynamics 365 Customer Engagement 方案 Enterprise Edition CRMOL Basic （合格供應專案）教職員版
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic （合格供應專案）
- Dynamics 365 Customer Engagement Plan Enterprise Edition （政府定價），適用于 CRM Basic 的 SA （合格供應專案）
- Dynamics 365 Customer Engagement 方案 Enterprise Edition （從 SA for CRM Basic （合格供應專案））學生專用
- Dynamics 365 Customer Engagement 方案 Enterprise Edition，適用于教職員的 SA for CRM Basic （合格供應專案）
- 適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）
- 適用于 CRM Basic 的 Dynamics 365 Customer Engagement 方案 Enterprise Edition （政府定價）附加元件（合格供應專案）
- 適用于學生的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件（合格供應專案）
- 適用于教職員的 Dynamics 365 Customer Engagement 方案 Enterprise Edition 附加元件



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>來自基本（合格供應專案）替代方案的 Dynamics 365 for Sales/Customer Engagement 方案

**淘汰的優惠**   

- 來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 for Sales （合格供應專案）
- 來自 CRM Basic 或 CRMOL Basic 的 Dynamics 365 Customer Engagement 方案（合格供應專案）

**取代選項**
- Dynamics 365 for Sales 專業版（新）
- Dynamics 365 for Sales 專業版（新）
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement 方案或
- Dynamics 365 團隊成員



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
5. 選取 [提交]。 您將針對需要新授權的每位使用者執行此動作。 

將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。 

1. 從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。
2. 在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。

舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。 暫停的訂閱將在 120 天後自動解除佈建。 您的客戶將不會產生舊訂用帳戶的額外費用。
 

 



