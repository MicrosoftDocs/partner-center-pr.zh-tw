---
title: Csp 的 Cloudyn Azure 成本管理
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在合作夥伴中心註冊 Cloudyn web 應用程式並使用它的秘密金鑰，讓您可以使用應用程式來追蹤客戶的 Azure 使用量和成本。
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435907"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="f525a-103">使用適用于 CSP 合作夥伴的 Azure 成本管理應用程式來追蹤客戶的 Azure 使用量和成本</span><span class="sxs-lookup"><span data-stu-id="f525a-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="f525a-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="f525a-104">**Applies to**</span></span>

- <span data-ttu-id="f525a-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="f525a-105">Partner Center</span></span>
- <span data-ttu-id="f525a-106">雲端解決方案提供者計畫合作夥伴</span><span class="sxs-lookup"><span data-stu-id="f525a-106">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="f525a-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="f525a-107">**Appropriate roles**</span></span>

- <span data-ttu-id="f525a-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="f525a-108">Global admin</span></span>
- <span data-ttu-id="f525a-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="f525a-109">Admin agent</span></span>

[<span data-ttu-id="f525a-110">取得有關 Azure 成本管理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="f525a-110">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="f525a-111">開始之前</span><span class="sxs-lookup"><span data-stu-id="f525a-111">Before you begin</span></span>
<span data-ttu-id="f525a-112">在可以使用 Azure 成本管理之前，請先確定您符合下列需求：</span><span class="sxs-lookup"><span data-stu-id="f525a-112">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="f525a-113">您是雲端解決方案提供者計畫的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="f525a-113">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="f525a-114">您有能力建立 Partner Center API Web 應用程式。</span><span class="sxs-lookup"><span data-stu-id="f525a-114">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="f525a-115">概觀</span><span class="sxs-lookup"><span data-stu-id="f525a-115">Overview</span></span>

<span data-ttu-id="f525a-116">Cloudyn 是一個 web 應用程式，可讓您追蹤及管理客戶使用 Azure 的程度，以及該使用量的成本。</span><span class="sxs-lookup"><span data-stu-id="f525a-116">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="f525a-117">您是透過合作夥伴中心 API 使用此應用程式。</span><span class="sxs-lookup"><span data-stu-id="f525a-117">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="f525a-118">在合作夥伴中心註冊您的 Web 應用程式</span><span class="sxs-lookup"><span data-stu-id="f525a-118">Register your web app in the Partner Center</span></span>
<span data-ttu-id="f525a-119">當您在合作夥伴中心註冊 Azure Active Directory Web 應用程式，您就啟用對 Partner Center API 的存取權。</span><span class="sxs-lookup"><span data-stu-id="f525a-119">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="f525a-120">使用[全域系統管理員或系統管理代理人帳戶](create-user-accounts-and-set-permissions.md)登入[合作夥伴中心](https://partnercenter.microsoft.com/pcv/dashboard/overview)。</span><span class="sxs-lookup"><span data-stu-id="f525a-120">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="f525a-121">從**合作夥伴中心**，選取 [**帳戶設定**] [ &gt; **[應用程式管理](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**]。</span><span class="sxs-lookup"><span data-stu-id="f525a-121">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="f525a-122">在 **\[Web 應用程式\]** 區段中，按一下 **\[新增 Web 應用程式\]**。</span><span class="sxs-lookup"><span data-stu-id="f525a-122">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="f525a-123">**注意**：如果您先前已建立 Web 應用程式，可以略過步驟 3。</span><span class="sxs-lookup"><span data-stu-id="f525a-123">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="f525a-124">複製並儲存您 Web 應用程式的**商務識別碼** GUID 和**應用程式識別碼** GUID。</span><span class="sxs-lookup"><span data-stu-id="f525a-124">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="f525a-125">您將需要這兩個識別碼，才能使用 30 天免費試用版的 Azure 成本管理應用程式。</span><span class="sxs-lookup"><span data-stu-id="f525a-125">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="f525a-126">將秘密金鑰新增到您的應用程式。</span><span class="sxs-lookup"><span data-stu-id="f525a-126">Add a secret key to your app</span></span>
1. <span data-ttu-id="f525a-127">在 **\[新增金鑰\]** 按鈕旁邊的下拉式清單中，選取 1 或 2 年期間。</span><span class="sxs-lookup"><span data-stu-id="f525a-127">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="f525a-128">按一下 [**新增金鑰**]。</span><span class="sxs-lookup"><span data-stu-id="f525a-128">Click **Add key**.</span></span> 
3. <span data-ttu-id="f525a-129">複製並儲存秘密金鑰值。</span><span class="sxs-lookup"><span data-stu-id="f525a-129">Copy and save the secret key value.</span></span> <span data-ttu-id="f525a-130">您將需要此值，以便使用 30 天免費試用版。</span><span class="sxs-lookup"><span data-stu-id="f525a-130">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="f525a-131">應用程式秘密金鑰就像是具有較長到期日的密碼。</span><span class="sxs-lookup"><span data-stu-id="f525a-131">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="f525a-132">請將金鑰值儲存在安全的位置，以供未來使用。</span><span class="sxs-lookup"><span data-stu-id="f525a-132">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f525a-133">後續步驟</span><span class="sxs-lookup"><span data-stu-id="f525a-133">Next steps</span></span>
<span data-ttu-id="f525a-134">啟動 [30 天免費試用版](https://go.microsoft.com/fwlink/?linkid=857895)。</span><span class="sxs-lookup"><span data-stu-id="f525a-134">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="f525a-135">若要啟動試用版，您需要下列資訊：</span><span class="sxs-lookup"><span data-stu-id="f525a-135">You need the following details to start the trial:</span></span>
- <span data-ttu-id="f525a-136">合作夥伴中心登入憑證</span><span class="sxs-lookup"><span data-stu-id="f525a-136">Partner Center sign in credentials</span></span>
- <span data-ttu-id="f525a-137">商務識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="f525a-137">Commerce ID GUID</span></span>
- <span data-ttu-id="f525a-138">應用程式識別碼 GUID</span><span class="sxs-lookup"><span data-stu-id="f525a-138">App ID GUID</span></span>
- <span data-ttu-id="f525a-139">應用程式秘密金鑰值</span><span class="sxs-lookup"><span data-stu-id="f525a-139">Application secret key value</span></span>
