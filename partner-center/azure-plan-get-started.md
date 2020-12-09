---
title: 開始移至 Azure 方案
description: 了解使用 Azure 隨用隨付方案時，您和您客戶需要知道的事項，包括首要步驟、安全性預防措施，以及如何開始。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: fcf75acef4afb80c5aec889911ffc2b4a53b6edd
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534908"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>開始搭配 Azure 方案使用隨用隨付費率

**適當的角色**

- 系統管理代理人
- 銷售代理人


Microsoft 在合作夥伴中心引進了新的商務體驗。  透過這種新的商務體驗，合作夥伴可在 Microsoft 客戶合約下，以隨用隨付費率為客戶取得 Azure 服務的存取權。

此方案可簡化購買體驗 - 您可以在 Azure 方案中有多個 Azure 訂用帳戶。 您不再需要針對每個 Azure 訂用帳戶提交個別訂單。 在 Azure 的這項新商務體驗中，我們已協調為單一全球定價原則，讓 CSP 合作夥伴能夠以發佈的價格提供 Azure。

合作夥伴需要有新技能，才能因應我們客戶的數位轉型需求。 許多客戶會尋求合作夥伴提供上述服務，而在交易以外，更要讓他們的雲端旅程更加順暢，並協助他們有效率地使用 Azure 服務。 Microsoft 合作夥伴在客戶生命週期的所有階段都扮演著重要的角色。 這些類型的合作夥伴服務本質上會持續進行，包括 Azure 資產監控、原則和治理管理、設定和組態微調、技術支援，以及各種其他服務。 這些服務要求合作夥伴要相當熟悉客戶的 Azure 環境，也要持續對其管理的基礎資源進行適當的治理與控制。 提供此全天候雲端作業管理的計費合作夥伴，將具有該工作 **受控服務的合作夥伴所獲得信用點數** 的資格。

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>請確定您的客戶已簽署 Microsoft 客戶合約

從 2019 年 10 月 1 日起，Microsoft 客戶合約是以完整數位程序來簡化和精簡客戶購買體驗的永久合約。 所有想要在適用於 Azure 的 CSP 中利用新商務體驗的客戶，都必須簽署 Microsoft 客戶合約。

希望根據新的 Azure 方案進行交易並下新訂單的合作夥伴，可以在生產環境中使用合作夥伴中心儀表板和 API，確認客戶接受 Microsoft 客戶合約。

從 2020 年 2 月 1 日開始，現有的 Microsoft Cloud 合約會從 CSP 方案中移除。 從那時起，所有其他供應項目 (包含 Microsoft 365、Dynamics 365 和現有的 Azure) 都需要對新的 Microsoft 客戶合約的客戶接受進行合作夥伴確認 (證明)。 CSP 中的合作夥伴將無法在未經 Microsoft 客戶合約證明的情況下，為客戶建立新訂單。

如需完整詳細資訊，請參閱[確認客戶接受 Microsoft 客戶合約](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>安全性與存取控制做法

為了協助保護合作夥伴和客戶，我們針對參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴推出一組強制性的安全性需求。

一旦強制執行這些需求，未實作強制安全性需求的合作夥伴，將無法在雲端解決方案提供者計畫中進行交易，或利用委派系統管理員權限來管理客戶租用戶。 我們正處於為需求建立技術強制執行日期的過程，並且將通知合作夥伴相關的日期與詳細資訊。

## <a name="actions-to-take-to-implement-mfa"></a>實作 MFA 所採取的動作

基於成為合作夥伴的高度特殊權限本質，我們必須確保每個使用者的每個單一驗證都有 MFA 挑戰。 您可以透過下列其中一種方式來完成這項作業：

- 實作 Azure AD Premium 並確保對每個使用者強制執行多重要素驗證 (MFA)
- 實作 [Azure AD 安全性預設值](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- 實作協力廠商解決方案，並確保對每個使用者強制執行 MFA

自 2019 年 8 月 1 日起，所有合作夥伴都必須針對其合作夥伴租用戶的所有使用者 (包括服務帳戶) 強制執行多重要素驗證。 如需這些安全性需求的詳細資訊，請參閱[合作夥伴安全性需求](partner-security-requirements.md)。

Microsoft 建議合作夥伴盡量使用 RBAC，遵循透過 [Azure Active Directory Privileged Identity Management 資源](/azure/active-directory/privileged-identity-management/pim-configure)啟用的最佳做法。

## <a name="read-more-about-the-azure-plan"></a>深入了解 Azure 方案

- [購買 Azure 方案](purchase-azure-plan.md)

- [比較 Azure 供應項目](compare-azure-offers.md)

- [合作夥伴所獲得信用點數 - 概觀](partner-earned-credit.md)

- 合作夥伴所獲得信用點數 (PEC) 計算，以及有資格獲得合作夥伴所獲得信用點數的角色和權限，可從您的合作夥伴中心儀表板價目表 (需要登入) 取得。

## <a name="next-steps"></a>接下來的步驟 

- [合作夥伴所獲得信用點數如何決定 - 詳細資料](partner-earned-credit-explanation.md)
- [Azure 方案價目表說明](azure-plan-price-list.md)
- [將您的客戶轉換為 Azure 方案](azure-plan-transition.md)
- [管理 Azure 方案下的訂用帳戶和資源](azure-plan-manage.md)
- [提供 Azure 方案的國家/地區完整清單](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)