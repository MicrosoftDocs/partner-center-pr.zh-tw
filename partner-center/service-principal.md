---
title: Azure AD 服務主體
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何將服務主體新增至您的 Azure AD 租用戶。 這樣做就等於在合作夥伴中心新增 Azure AD 應用程式 (服務主體)。
author: LauraBrenner
ms.author: labrenne
Keywords: Azure、Azure 方案、服務主體、Azure AD 應用程式
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 76a65cd824c7c1af5242bea3af6069a466c9fa1c
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425997"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="d7e4a-105">在合作夥伴中心新增 Azure AD 應用程式 (服務主體)</span><span class="sxs-lookup"><span data-stu-id="d7e4a-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="d7e4a-106">在合作夥伴中心的商務 Marketplace 計畫中，您現在可以將 Azure AD 應用程式 (服務主體) 新增為合作夥伴中心帳戶中的使用者。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="d7e4a-107">(先前，您可以在 Cloud Partner 入口網站或 CPP 帳戶中這麼做。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="d7e4a-108">但現在您已移轉至合作夥伴中心，所以 CPP 帳戶為唯讀狀態。)請注意，服務主體與 Azure AD 應用程式是同義。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-108">Now that you have migrated to Partner Center, the CPP account is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="d7e4a-109">新增 Azure AD 應用程式 (服務主體)</span><span class="sxs-lookup"><span data-stu-id="d7e4a-109">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="d7e4a-110">在合作夥伴中心儀表板，選取 [設定]，然後選取 [開發人員設定]。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-110">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="d7e4a-111">選取 [使用者]，然後選取 [新增 Azure AD 應用程式]。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-111">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="d7e4a-112">選取現有的 Azure AD 應用程式，或建立新的應用程式。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-112">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="d7e4a-113">如果建立新的 Azure AD 應用程式，請包含下列資訊：</span><span class="sxs-lookup"><span data-stu-id="d7e4a-113">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="d7e4a-114">**回覆 URL**：使用者用於登入以使用您 Azure AD 應用程式的 URL。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-114">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="d7e4a-115">**應用程式識別碼 URI**：Azure AD 應用程式的邏輯識別碼，會在向 Azure AD 傳送單一登入要求時顯示。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-115">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="d7e4a-116">**安全性角色**：**管理員** (與 CPP 中的「擁有者」角色相同) 和**開發人員** (與 CPP 中的「參與者」角色相同) 角色適用於合作夥伴中心內的商務 Marketplace 計畫，而且可與此 Azure AD 應用程式相關聯。</span><span class="sxs-lookup"><span data-stu-id="d7e4a-116">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
