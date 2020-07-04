---
title: 合作夥伴中心深入解析以角色為基礎的存取
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解查看合作夥伴中心深入解析報告所需的特定角色。 這些包括執行報表檢視器和報表檢視器的角色。
keywords: PCI，效能，客戶成功，測量，角色
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aaa3552a7c0a3d15674ac0178fc98375b9cd1b0b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948722"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="56da6-105">合作夥伴中心深入解析儀表板的角色型存取控制</span><span class="sxs-lookup"><span data-stu-id="56da6-105">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="56da6-106">Insights 儀表板會在合作夥伴中心使用兩個新角色，來管理員工對報表的存取權-主管報表檢視器和報表檢視器。</span><span class="sxs-lookup"><span data-stu-id="56da6-106">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="56da6-107">執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取機密資料集，例如收益和客戶/員工個人資料。</span><span class="sxs-lookup"><span data-stu-id="56da6-107">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="56da6-108">如同其他合作夥伴中心角色，全域管理員或帳戶管理員將能夠在使用者管理頁面上，將使用者指派給這些角色。</span><span class="sxs-lookup"><span data-stu-id="56da6-108">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="56da6-109">這些角色可能適用于整個公司或特定 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="56da6-109">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="56da6-110">針對特定 MPN 位置指派的角色，會限制使用者只能查看與所選 MPN 位置相關聯的報告資料。</span><span class="sxs-lookup"><span data-stu-id="56da6-110">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="56da6-111">合作夥伴可以從下面的觀點選取一個或多個位置。</span><span class="sxs-lookup"><span data-stu-id="56da6-111">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="角色":::

>[!Note]
> <span data-ttu-id="56da6-113">從2020年1月20日 MPN 系統管理員的使用者，會自動新增至該租使用者所有位置的全公司**執行報告檢視器**角色。</span><span class="sxs-lookup"><span data-stu-id="56da6-113">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="56da6-114">如此一來，這些使用者就能夠以執行報表檢視器的身分存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員和帳戶管理員可以覆寫這些使用者的自動指派角色，以進一步增加或限制其功能。</span><span class="sxs-lookup"><span data-stu-id="56da6-114">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="56da6-115">後續步驟</span><span class="sxs-lookup"><span data-stu-id="56da6-115">Next steps</span></span>

- <span data-ttu-id="56da6-116">深入瞭解[合作夥伴中心深入](partner-center-insights.md)解析及其各種報告。</span><span class="sxs-lookup"><span data-stu-id="56da6-116">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
