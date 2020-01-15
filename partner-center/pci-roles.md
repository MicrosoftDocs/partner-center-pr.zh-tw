---
title: 合作夥伴中心深入解析-以角色為基礎的存取控制 |合作夥伴中心
ms.topic: article
ms.date: 01/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 需要特定角色才能查看深入解析報告
ms.assetid: 2F4B9A27-37FF-41E4-8A26-5EAE88DD8A49
keywords: PCI，效能，客戶成功，測量，角色
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e51e86ed20af16d4bc4c5d48b33eee712480bfab
ms.sourcegitcommit: 1a735003cca0bd430195ac1213bd8d77bd5063a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/14/2020
ms.locfileid: "75945860"
---
# <a name="roles-based-access-control-to-the-insights-dashboard"></a>深入解析儀表板的角色型存取控制

Insights 儀表板會在合作夥伴中心使用兩個新角色，來管理員工對報表的存取權-主管報表檢視器和報表檢視器。  執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取機密資料集，例如收益和客戶/員工個人資料。  

如同其他合作夥伴中心角色，全域管理員或帳戶管理員將能夠在使用者管理頁面上，將使用者指派給這些角色。 這些角色可能適用于整個公司或特定 MPN 位置。 針對特定 MPN 位置指派的角色，會限制使用者只能查看與所選 MPN 位置相關聯的報告資料。 合作夥伴可以從下面的觀點選取一個或多個位置。

![角色](images/pci/roles.png)

>下從2020年1月20日 MPN 系統管理員的使用者，會自動新增至該租使用者所有位置的全公司「主管報表檢視器」角色。 如此一來，這些使用者就能夠以執行報表檢視器的身分存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員和帳戶管理員可以覆寫這些使用者的自動指派角色，以進一步增加或限制其功能。