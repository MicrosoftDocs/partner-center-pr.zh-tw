---
title: Azure AD 服務主體 |合作夥伴中心
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 將服務主體新增至您的 Azure AD 租用戶
author: LauraBrenner
ms.author: labrenne
Keywords: Azure、Azure 方案、服務主體、Azure AD 應用程式
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 780776ee32f20d03101a4ee39ee2dc985541d7c1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/07/2020
ms.locfileid: "75716889"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="206d2-104">在合作夥伴中心新增 Azure AD 應用程式 (服務主體)</span><span class="sxs-lookup"><span data-stu-id="206d2-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="206d2-105">在合作夥伴中心的商務 Marketplace 計畫中，您現在可以將 Azure AD 應用程式 (服務主體) 新增為合作夥伴中心帳戶中的使用者。</span><span class="sxs-lookup"><span data-stu-id="206d2-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="206d2-106">(您可以先在 Cloud Partner 入口網站 (CPP) 帳戶中執行此動作，但現在您已移轉至合作夥伴中心，而 CPP 帳戶是唯讀的)。請注意，服務主體與 Azure AD 應用程式是同義。</span><span class="sxs-lookup"><span data-stu-id="206d2-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="206d2-107">新增 Azure AD 應用程式 (服務主體)</span><span class="sxs-lookup"><span data-stu-id="206d2-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="206d2-108">在合作夥伴中心儀表板，選取 [設定]  ，然後選取 [開發人員設定]  。</span><span class="sxs-lookup"><span data-stu-id="206d2-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="206d2-109">選取 [使用者]  ，然後選取 [新增 Azure AD 應用程式]  。</span><span class="sxs-lookup"><span data-stu-id="206d2-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="206d2-110">選取現有的 Azure AD 應用程式，或建立新的應用程式。</span><span class="sxs-lookup"><span data-stu-id="206d2-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="206d2-111">如果建立新的 Azure AD 應用程式，請包含下列資訊：</span><span class="sxs-lookup"><span data-stu-id="206d2-111">If you create a new Azure AD Application, include the following information:</span></span>  

  


<span data-ttu-id="206d2-112">**回覆 URL**：這是讓使用者登入以使用您的 Azure AD 應用程式的 URL。</span><span class="sxs-lookup"><span data-stu-id="206d2-112">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="206d2-113">**應用程式識別碼 URI**：這是 Azure AD 應用程式的邏輯識別碼，是在傳送單一登入要求至 Azure AD 時提供。</span><span class="sxs-lookup"><span data-stu-id="206d2-113">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="206d2-114">**安全性角色**：**管理員** (與 CPP 中的「擁有者」角色相同) 和**開發人員** (與 CPP 中的「參與者」角色相同) 角色適用於合作夥伴中心內的商務 Marketplace 計畫，而且可與此 Azure AD 應用程式相關聯。</span><span class="sxs-lookup"><span data-stu-id="206d2-114">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

  