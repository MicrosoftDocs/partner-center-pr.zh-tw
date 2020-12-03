---
title: Cloudyn 提供適用於 CSP 的 Azure 成本管理
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心中註冊 Cloudyn web 應用程式並使用其秘密金鑰，讓您可以使用應用程式來追蹤客戶的 Azure 使用量和成本。
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534978"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="efe42-103">使用適用于 CSP 合作夥伴的 Azure 成本管理應用程式來追蹤客戶的 Azure 使用量和成本</span><span class="sxs-lookup"><span data-stu-id="efe42-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="efe42-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="efe42-104">**Appropriate roles**</span></span>

- <span data-ttu-id="efe42-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="efe42-105">Global admin</span></span>
- <span data-ttu-id="efe42-106">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="efe42-106">Admin agent</span></span>

[<span data-ttu-id="efe42-107">取得有關 Azure 成本管理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="efe42-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="efe42-108">開始之前</span><span class="sxs-lookup"><span data-stu-id="efe42-108">Before you begin</span></span>
<span data-ttu-id="efe42-109">在可以使用 Azure 成本管理之前，請先確定您符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="efe42-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="efe42-110">您是雲端解決方案提供者計畫的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="efe42-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="efe42-111">您有能力建立 Partner Center API Web 應用程式。</span><span class="sxs-lookup"><span data-stu-id="efe42-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="efe42-112">概觀</span><span class="sxs-lookup"><span data-stu-id="efe42-112">Overview</span></span>

<span data-ttu-id="efe42-113">Cloudyn 是一個 web 應用程式，可讓您追蹤和管理客戶使用 Azure 的數量，以及該使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="efe42-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="efe42-114">您是透過合作夥伴中心 API 使用此應用程式。</span><span class="sxs-lookup"><span data-stu-id="efe42-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="efe42-115">在合作夥伴中心註冊您的 Web 應用程式</span><span class="sxs-lookup"><span data-stu-id="efe42-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="efe42-116">當您在合作夥伴中心註冊 Azure Active Directory Web 應用程式，您就啟用對 Partner Center API 的存取權。</span><span class="sxs-lookup"><span data-stu-id="efe42-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="efe42-117">使用[全域系統管理員或系統管理代理人帳戶](create-user-accounts-and-set-permissions.md)登入[合作夥伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="efe42-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="efe42-118">從 **合作夥伴中心** 中，選取 [ **帳戶設定**] &gt; **[應用程式管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**。</span><span class="sxs-lookup"><span data-stu-id="efe42-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="efe42-119">在 **\[Web 應用程式\]** 區段中，按一下 **\[新增 Web 應用程式\]**。</span><span class="sxs-lookup"><span data-stu-id="efe42-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="efe42-120">**注意**：如果您先前已建立 Web 應用程式，可以略過步驟 3。</span><span class="sxs-lookup"><span data-stu-id="efe42-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="efe42-121">複製並儲存您 Web 應用程式的 **商務識別碼** GUID 和 **應用程式識別碼** GUID。</span><span class="sxs-lookup"><span data-stu-id="efe42-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="efe42-122">您將需要這兩個識別碼，才能使用 30 天免費試用版的 Azure 成本管理應用程式。</span><span class="sxs-lookup"><span data-stu-id="efe42-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="efe42-123">將秘密金鑰新增到您的應用程式。</span><span class="sxs-lookup"><span data-stu-id="efe42-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="efe42-124">在 **\[新增金鑰\]** 按鈕旁邊的下拉式清單中，選取 1 或 2 年期間。</span><span class="sxs-lookup"><span data-stu-id="efe42-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="efe42-125">按一下 [ **新增金鑰**]。</span><span class="sxs-lookup"><span data-stu-id="efe42-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="efe42-126">複製並儲存秘密金鑰值。</span><span class="sxs-lookup"><span data-stu-id="efe42-126">Copy and save the secret key value.</span></span> <span data-ttu-id="efe42-127">您將需要此值，以便使用 30 天免費試用版。</span><span class="sxs-lookup"><span data-stu-id="efe42-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="efe42-128">應用程式秘密金鑰類似于到期日較長的密碼。</span><span class="sxs-lookup"><span data-stu-id="efe42-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="efe42-129">請將金鑰值儲存在安全的位置，以供未來使用。</span><span class="sxs-lookup"><span data-stu-id="efe42-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="efe42-130">後續步驟</span><span class="sxs-lookup"><span data-stu-id="efe42-130">Next steps</span></span>
<span data-ttu-id="efe42-131">啟動 [30 天免費試用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="efe42-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="efe42-132">若要啟動試用版，您需要下列資訊：</span><span class="sxs-lookup"><span data-stu-id="efe42-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="efe42-133">合作夥伴中心登入憑證</span><span class="sxs-lookup"><span data-stu-id="efe42-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="efe42-134">商務識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="efe42-134">Commerce ID GUID</span></span>
- <span data-ttu-id="efe42-135">應用程式識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="efe42-135">App ID GUID</span></span>
- <span data-ttu-id="efe42-136">應用程式秘密金鑰值</span><span class="sxs-lookup"><span data-stu-id="efe42-136">Application secret key value</span></span>
