---
title: 註冊為控制台廠商
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何在合作夥伴中心 (CPV) 註冊為「控制台」廠商。
author: parthpandyaMSFT
ms.author: parthp
keywords: 控制台廠商，註冊 CPV 應用程式，管理 CPV 應用程式
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 503bbb6d1c083337dc9bad9cc469c43d614eb5a3
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302365"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="9e652-104">註冊為控制台廠商，協助整合 CSP 合作夥伴系統與合作夥伴中心 Api</span><span class="sxs-lookup"><span data-stu-id="9e652-104">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="9e652-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="9e652-105">**Applies to**</span></span>

- <span data-ttu-id="9e652-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="9e652-106">Partner Center</span></span>

<span data-ttu-id="9e652-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="9e652-107">**Appropriate roles**</span></span>

- <span data-ttu-id="9e652-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="9e652-108">Global admin</span></span>

<span data-ttu-id="9e652-109"> (CPV) 的控制台廠商是獨立軟體廠商，其會開發應用程式供雲端解決方案提供者 (CSP) 合作夥伴使用，讓他們能夠整合其系統與合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="9e652-109">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="9e652-110">控制台廠商不是可直接存取合作夥伴中心儀表板或合作夥伴中心 Api 的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="9e652-110">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="9e652-111">無論您是目前的控制台廠商 (CPV) 或想要與 Microsoft 合作夥伴合作的新 CPV，Microsoft 現在都要求您在合作夥伴中心註冊，才能註冊您的應用程式並支援雲端解決方案提供者合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="9e652-111">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="9e652-112">若要建立帳戶，CPV 合作夥伴可以使用現有的 CSP 合作夥伴租使用者，或現有的 CPV 租使用者，或可在上架程式中建立新的租使用者。</span><span class="sxs-lookup"><span data-stu-id="9e652-112">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="9e652-113">如果 CPV 合作夥伴選擇使用現有的 CSP 租使用者，則他們必須建立個別的多租使用者應用程式，並在合作夥伴中心註冊以進行 CPV 活動。</span><span class="sxs-lookup"><span data-stu-id="9e652-113">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="9e652-114">應用程式無法同時註冊為 CSP 和 CPV 應用程式。</span><span class="sxs-lookup"><span data-stu-id="9e652-114">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="9e652-115">在合作夥伴中心註冊並註冊您的應用程式之後，您就可以存取合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="9e652-115">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="9e652-116">Microsoft 會透過您的沙箱資訊，透過合作夥伴中心通知來聯絡您。</span><span class="sxs-lookup"><span data-stu-id="9e652-116">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="9e652-117">如果您已經有沙箱帳戶，請繼續使用它。</span><span class="sxs-lookup"><span data-stu-id="9e652-117">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="9e652-118">您不需要新的沙箱。</span><span class="sxs-lookup"><span data-stu-id="9e652-118">You won't need a new sandbox.</span></span>

<span data-ttu-id="9e652-119">審查[Microsoft 控制台廠商合約](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="9e652-119">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="9e652-120">合作夥伴中心內的工作</span><span class="sxs-lookup"><span data-stu-id="9e652-120">Working in Partner Center</span></span>
<span data-ttu-id="9e652-121">在您註冊合作夥伴中心的 CPV 體驗並接受 CPV 合約後，您就可以：</span><span class="sxs-lookup"><span data-stu-id="9e652-121">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="9e652-122">管理多租使用者應用程式 (新增應用程式，以在合作夥伴中心) 中 Azure 入口網站、註冊及取消註冊應用程式。</span><span class="sxs-lookup"><span data-stu-id="9e652-122">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

>[!Note] 
><span data-ttu-id="9e652-123">CPVs 必須在合作夥伴中心註冊其應用程式，才能獲得合作夥伴中心 Api 的授權。</span><span class="sxs-lookup"><span data-stu-id="9e652-123">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="9e652-124">單純將應用程式加入 Azure 入口網站，並無法授權 CPV 應用程式使用合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="9e652-124">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="9e652-125">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="9e652-125">View and manage your CPV profile</span></span> 

- <span data-ttu-id="9e652-126">檢視及管理您需要存取 CPV 功能的使用者。</span><span class="sxs-lookup"><span data-stu-id="9e652-126">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="9e652-127">全域管理員是 CPV 可以擁有的唯一角色。</span><span class="sxs-lookup"><span data-stu-id="9e652-127">Global admin is the only role a CPV can have.</span></span>


