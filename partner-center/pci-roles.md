---
title: 合作夥伴中心深入解析以角色為基礎的存取
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解查看合作夥伴中心深入解析報告所需的特定角色。 這些包括執行報表檢視器和報表檢視器的角色。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5a9df2b6f67ca4e825da2c273c82d7cd46763f1b
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436637"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>合作夥伴中心深入解析儀表板的角色型存取控制

Insights 儀表板會在合作夥伴中心使用兩個新角色，來管理員工對報表的存取權-主管報表檢視器和報表檢視器。  執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取機密資料集，例如收益和客戶/員工個人資料。  

如同其他合作夥伴中心角色，全域管理員或帳戶管理員將能夠在使用者管理頁面上，將使用者指派給這些角色。 這些角色可能適用于整個公司或特定 MPN 位置。 針對特定 MPN 位置指派的角色，會限制使用者只能查看與所選 MPN 位置相關聯的報告資料。 合作夥伴可以從下面的觀點選取一個或多個位置。

:::image type="content" source="images/pci/roles.png" alt-text="角色":::

>[!Note]
> 從2020年1月20日 MPN 系統管理員的使用者，會自動新增至該租使用者所有位置的全公司**執行報告檢視器**角色。 如此一來，這些使用者就能夠以執行報表檢視器的身分存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員和帳戶管理員可以覆寫這些使用者的自動指派角色，以進一步增加或限制其功能。

## <a name="next-steps"></a>後續步驟

- 深入瞭解[合作夥伴中心深入](partner-center-insights.md)解析及其各種報告。
