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
# <a name="roles-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="64754-104">深入解析儀表板的角色型存取控制</span><span class="sxs-lookup"><span data-stu-id="64754-104">Roles-based access control to the Insights dashboard</span></span>

<span data-ttu-id="64754-105">Insights 儀表板會在合作夥伴中心使用兩個新角色，來管理員工對報表的存取權-主管報表檢視器和報表檢視器。</span><span class="sxs-lookup"><span data-stu-id="64754-105">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="64754-106">執行報表檢視器角色中的使用者可以存取所有報表資料集，而報表檢視器角色中的使用者將無法存取機密資料集，例如收益和客戶/員工個人資料。</span><span class="sxs-lookup"><span data-stu-id="64754-106">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="64754-107">如同其他合作夥伴中心角色，全域管理員或帳戶管理員將能夠在使用者管理頁面上，將使用者指派給這些角色。</span><span class="sxs-lookup"><span data-stu-id="64754-107">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="64754-108">這些角色可能適用于整個公司或特定 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="64754-108">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="64754-109">針對特定 MPN 位置指派的角色，會限制使用者只能查看與所選 MPN 位置相關聯的報告資料。</span><span class="sxs-lookup"><span data-stu-id="64754-109">Roles assigned for specific MPN location(s) limits the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="64754-110">合作夥伴可以從下面的觀點選取一個或多個位置。</span><span class="sxs-lookup"><span data-stu-id="64754-110">Partner can select one or multiple locations from the below view.</span></span>

![角色](images/pci/roles.png)

><span data-ttu-id="64754-112">下從2020年1月20日 MPN 系統管理員的使用者，會自動新增至該租使用者所有位置的全公司「主管報表檢視器」角色。</span><span class="sxs-lookup"><span data-stu-id="64754-112">[Note] Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide ‘Executive Report Viewer’ role for all locations for that tenant.</span></span> <span data-ttu-id="64754-113">如此一來，這些使用者就能夠以執行報表檢視器的身分存取報表，而不需要全域管理員或帳戶管理員所需的任何明確動作。全域管理員和帳戶管理員可以覆寫這些使用者的自動指派角色，以進一步增加或限制其功能。</span><span class="sxs-lookup"><span data-stu-id="64754-113">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>