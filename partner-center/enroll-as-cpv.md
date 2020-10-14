---
title: 註冊為控制台廠商
description: 瞭解如何在合作夥伴中心中註冊為主控台廠商 (CPV) ，讓您可以更妥善地整合 CSP 合作夥伴系統與合作夥伴中心 Api。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/20/2020
ms.openlocfilehash: 1bfcb4de27233283b6188903b3e1f6bbdf67698c
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031891"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="e3a88-103">註冊為控制台廠商，以協助整合 CSP 合作夥伴系統與合作夥伴中心 API</span><span class="sxs-lookup"><span data-stu-id="e3a88-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>

<span data-ttu-id="e3a88-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="e3a88-104">**Applies to**</span></span>

- <span data-ttu-id="e3a88-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="e3a88-105">Partner Center</span></span>

<span data-ttu-id="e3a88-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="e3a88-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e3a88-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="e3a88-107">Global admin</span></span>

<span data-ttu-id="e3a88-108">主控台廠商 (CPV) 是獨立軟體廠商，可開發應用程式供雲端解決方案提供者 (CSP) 合作夥伴使用，讓他們能夠將其系統與合作夥伴中心 Api 整合。</span><span class="sxs-lookup"><span data-stu-id="e3a88-108">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="e3a88-109">主控台廠商不是可直接存取合作夥伴中心儀表板或合作夥伴中心 Api 的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="e3a88-109">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="e3a88-110">無論您是目前的主控台廠商 (CPV) 或想要與 Microsoft 合作夥伴合作的新 CPV，Microsoft 現在都需要您註冊合作夥伴中心，才能註冊您的應用程式，並支援雲端解決方案提供者合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="e3a88-110">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="e3a88-111">若要建立帳戶，CPV 夥伴可以使用現有的 CSP 合作夥伴租使用者或現有的 CPV 租使用者，或在上線過程中建立新的租使用者。</span><span class="sxs-lookup"><span data-stu-id="e3a88-111">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="e3a88-112">如果 CPV 合作夥伴選擇使用現有的 CSP 租使用者，則他們必須建立個別的多租使用者應用程式，並在適用于 CPV 活動的合作夥伴中心中註冊它們。</span><span class="sxs-lookup"><span data-stu-id="e3a88-112">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="e3a88-113">應用程式無法同時註冊為 CSP 和 CPV 應用程式。</span><span class="sxs-lookup"><span data-stu-id="e3a88-113">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="e3a88-114">在您註冊合作夥伴中心並註冊您的應用程式之後，您就可以存取合作夥伴中心 Api。</span><span class="sxs-lookup"><span data-stu-id="e3a88-114">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="e3a88-115">Microsoft 會透過合作夥伴中心通知，與您的沙箱資訊聯繫。</span><span class="sxs-lookup"><span data-stu-id="e3a88-115">Microsoft will contact you via a Partner Center notification with your sandbox information.</span></span> <span data-ttu-id="e3a88-116">如果您已經有沙箱帳戶，請繼續使用。</span><span class="sxs-lookup"><span data-stu-id="e3a88-116">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="e3a88-117">您將不需要新的沙箱。</span><span class="sxs-lookup"><span data-stu-id="e3a88-117">You won't need a new sandbox.</span></span>

<span data-ttu-id="e3a88-118">複習 [Microsoft 主控台廠商合約](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="e3a88-118">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="e3a88-119">合作夥伴中心內的工作</span><span class="sxs-lookup"><span data-stu-id="e3a88-119">Working in Partner Center</span></span>
<span data-ttu-id="e3a88-120">在您註冊合作夥伴中心 CPV 經驗並接受 CPV 合約之後，您可以：</span><span class="sxs-lookup"><span data-stu-id="e3a88-120">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="e3a88-121">管理多租使用者應用程式 (將應用程式新增至合作夥伴中心) 中 Azure 入口網站、註冊及取消註冊應用程式。</span><span class="sxs-lookup"><span data-stu-id="e3a88-121">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="e3a88-122">CPVs 必須在合作夥伴中心中註冊其應用程式，才能取得合作夥伴中心 Api 的授權。</span><span class="sxs-lookup"><span data-stu-id="e3a88-122">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="e3a88-123">單純將應用程式加入 Azure 入口網站，並無法授權 CPV 應用程式使用合作夥伴中心 API。</span><span class="sxs-lookup"><span data-stu-id="e3a88-123">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="e3a88-124">檢視及管理您的 CPV 設定檔</span><span class="sxs-lookup"><span data-stu-id="e3a88-124">View and manage your CPV profile</span></span> 

- <span data-ttu-id="e3a88-125">檢視及管理您需要存取 CPV 功能的使用者。</span><span class="sxs-lookup"><span data-stu-id="e3a88-125">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="e3a88-126">全域管理員是 CPV 可以擁有的唯一角色。</span><span class="sxs-lookup"><span data-stu-id="e3a88-126">Global admin is the only role a CPV can have.</span></span>


