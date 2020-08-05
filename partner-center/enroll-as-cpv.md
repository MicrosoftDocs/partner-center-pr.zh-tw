---
title: 註冊為控制台廠商
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何在合作夥伴中心 (CPV) 註冊為「控制台」廠商。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b6258f54120e0a40f94ad74a76821c4222eb0ef4
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/04/2020
ms.locfileid: "87545889"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="673d6-103">註冊為控制台廠商，協助整合 CSP 合作夥伴系統與合作夥伴中心 Api</span><span class="sxs-lookup"><span data-stu-id="673d6-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="673d6-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="673d6-104">**Applies to**</span></span>

- <span data-ttu-id="673d6-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="673d6-105">Partner Center</span></span>

<span data-ttu-id="673d6-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="673d6-106">**Appropriate roles**</span></span>

- <span data-ttu-id="673d6-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="673d6-107">Global admin</span></span>

<span data-ttu-id="673d6-108"> (CPV) 的控制台廠商是獨立軟體廠商，其會開發應用程式供雲端解決方案提供者 (CSP) 合作夥伴使用，讓他們能夠整合其系統與合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="673d6-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="673d6-109">控制台廠商不是可直接存取合作夥伴中心儀表板或合作夥伴中心 Api 的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="673d6-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="673d6-110">無論您是目前的控制台廠商 (CPV) 或想要與 Microsoft 合作夥伴合作的新 CPV，Microsoft 現在都要求您在合作夥伴中心註冊，才能註冊您的應用程式並支援雲端解決方案提供者合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="673d6-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="673d6-111">若要建立帳戶，CPV 合作夥伴可以使用現有的 CSP 合作夥伴租使用者，或現有的 CPV 租使用者，或可在上架程式中建立新的租使用者。</span><span class="sxs-lookup"><span data-stu-id="673d6-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="673d6-112">如果 CPV 合作夥伴選擇使用現有的 CSP 租使用者，則他們必須建立個別的多租使用者應用程式，並在合作夥伴中心註冊以進行 CPV 活動。</span><span class="sxs-lookup"><span data-stu-id="673d6-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="673d6-113">應用程式無法同時註冊為 CSP 和 CPV 應用程式。</span><span class="sxs-lookup"><span data-stu-id="673d6-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="673d6-114">在合作夥伴中心註冊並註冊您的應用程式之後，您就可以存取合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="673d6-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="673d6-115">Microsoft 會透過您的沙箱資訊，透過合作夥伴中心通知來聯絡您。</span><span class="sxs-lookup"><span data-stu-id="673d6-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="673d6-116">如果您已經有沙箱帳戶，請繼續使用它。</span><span class="sxs-lookup"><span data-stu-id="673d6-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="673d6-117">您不需要新的沙箱。</span><span class="sxs-lookup"><span data-stu-id="673d6-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="673d6-118">審查[Microsoft 控制台廠商合約](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="673d6-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="673d6-119">合作夥伴中心內的工作</span><span class="sxs-lookup"><span data-stu-id="673d6-119">Working in Partner Center</span></span>
<span data-ttu-id="673d6-120">在您註冊合作夥伴中心的 CPV 體驗並接受 CPV 合約後，您就可以：</span><span class="sxs-lookup"><span data-stu-id="673d6-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="673d6-121">管理多租使用者應用程式 (新增應用程式，以在合作夥伴中心) 中 Azure 入口網站、註冊及取消註冊應用程式。</span><span class="sxs-lookup"><span data-stu-id="673d6-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="673d6-122">CPVs 必須在合作夥伴中心註冊其應用程式，才能獲得合作夥伴中心 Api 的授權。</span><span class="sxs-lookup"><span data-stu-id="673d6-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="673d6-123">單純將應用程式加入 Azure 入口網站，並無法授權 CPV 應用程式使用合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="673d6-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="673d6-124">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="673d6-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="673d6-125">檢視及管理您需要存取 CPV 功能的使用者。</span><span class="sxs-lookup"><span data-stu-id="673d6-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="673d6-126">全域管理員是 CPV 可以擁有的唯一角色。</span><span class="sxs-lookup"><span data-stu-id="673d6-126">Global admin is the only role a CPV can have.</span></span>


