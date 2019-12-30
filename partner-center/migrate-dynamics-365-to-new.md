---
title: 將 Dynamics 365 Business Edition 優惠遷移至較新的版本 |合作夥伴中心
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將您的 Dynamics 365 Business Edition 優惠遷移至較新版本，然後再將其到期。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 優惠，續約優惠，新的 Dynamics 365 Sku
ms.openlocfilehash: d4efd051b4d237eac5b766ed1aedc432e8b93ecc
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005117"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="6e6ed-104">Migrar ofertas de Dynamics 365 Business Edition a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="6e6ed-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span> 

<span data-ttu-id="6e6ed-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="6e6ed-105">**Applies to**</span></span>

- <span data-ttu-id="6e6ed-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="6e6ed-106">Partner Center</span></span>

<span data-ttu-id="6e6ed-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="6e6ed-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="6e6ed-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="6e6ed-108">Global admin</span></span>
-   <span data-ttu-id="6e6ed-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="6e6ed-109">User admin</span></span>
-   <span data-ttu-id="6e6ed-110">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="6e6ed-110">Admin agent</span></span>
-   <span data-ttu-id="6e6ed-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="6e6ed-111">Sales agent</span></span>

<span data-ttu-id="6e6ed-112">自2019年1月1日起，使用 Dynamics 365 Business Edition 訂用帳戶的客戶將無法再續約這些舊版供應專案;現有的訂閱將不會在過期時自動更新。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="6e6ed-113">在訂用帳戶的詳細資料頁面上，訂用帳戶狀態會變更為從 [日期] 自動續約于 [日期] 的到期日。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="6e6ed-114">為確保客戶的持續性，您應該將具有過期訂閱的訂用帳戶轉換為支援的選項，如下所示。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="6e6ed-115">我們建議您將客戶移至訂用帳戶的年度結束日期之前的新訂閱，以避免客戶發生任何服務中斷。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="6e6ed-116">如果您使用 API （CREST 或合作夥伴中心），您可以藉由評估訂用帳戶的結束日期以及自動續約 = False 屬性，來尋找過期的訂閱。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="6e6ed-117">有問題的訂用帳戶將會在2019年1月1日設定為自動續訂 = False。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="6e6ed-118">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="6e6ed-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="6e6ed-119">即將淘汰的 Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="6e6ed-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="6e6ed-120">Dynamics 365 for Finance and Operations，Business edition</span><span class="sxs-lookup"><span data-stu-id="6e6ed-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="6e6ed-121">Dynamics 365 的商務小組成員版本</span><span class="sxs-lookup"><span data-stu-id="6e6ed-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="6e6ed-122">Dynamics Business Central-Dynamics 365 Business Edition 的新優惠</span><span class="sxs-lookup"><span data-stu-id="6e6ed-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="6e6ed-123">透過新的 Dynamics Business Central 供應專案，您的客戶可以連接其財務、銷售、服務和營運，以簡化商務程式、改善客戶互動，並做出更好的決策。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="6e6ed-124">Dynamics 365 Business Central 是以雲端為基礎，僅供雲端解決方案提供者（CSP）方案合作夥伴使用。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="6e6ed-125">Dynamics 365 Business Edition 客戶有資格在2020年6月30日前獲得新的商業中心優惠折扣轉換定價。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="6e6ed-126">Pasar a los clientes a nuevos planes de producto</span><span class="sxs-lookup"><span data-stu-id="6e6ed-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="6e6ed-127">將客戶從已淘汰的 Sku 移至更新版本，必須依照下列步驟進行：</span><span class="sxs-lookup"><span data-stu-id="6e6ed-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="6e6ed-128">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="6e6ed-128">Purchase the new subscription</span></span>
- <span data-ttu-id="6e6ed-129">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="6e6ed-129">Reassign current user licenses</span></span>
- <span data-ttu-id="6e6ed-130">Cancelar suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="6e6ed-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="6e6ed-131">為您的客戶購買新方案</span><span class="sxs-lookup"><span data-stu-id="6e6ed-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="6e6ed-132">從左側導覽中選取 [**客戶**]，然後選取您想要移至新訂用帳戶的客戶。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="6e6ed-133">選取 [**新增訂**用帳戶]。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="6e6ed-134">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="6e6ed-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="6e6ed-135">您的客戶現在會有舊的訂閱和新的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="6e6ed-136">下一個步驟是將授權重新指派給客戶的使用者。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="6e6ed-137">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="6e6ed-138">Selecciona **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="6e6ed-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="6e6ed-139">若要將授權重新指派給使用者，請選取使用者，然後選取 [**管理授權**]。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="6e6ed-140">在 [**管理授權**] 頁面上，清除 [基本（限定供應專案）授權] 核取方塊中的 [Dynamics 365 for Sales/Customer Engagement 方案]，然後為客戶即將移動的訂用帳戶選取新的服務方案。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="6e6ed-141">選取 **\[提交\]** 。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-141">Select **Submit**.</span></span> <span data-ttu-id="6e6ed-142">您將針對需要新授權的每位使用者執行此動作。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="6e6ed-143">將授權移到新的訂用帳戶之後，您就可以取消舊的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="6e6ed-144">從左側導覽中選取 [**客戶**]，然後選取您要移動的客戶。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="6e6ed-145">在 [訂閱詳細資料] 頁面上，將舊訂閱設定為 [已**暫停**]，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="6e6ed-146">舊的訂用帳戶現在已暫止，且新的訂用帳戶為作用中狀態。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="6e6ed-147">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="6e6ed-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="6e6ed-148">您的客戶將不會產生舊訂用帳戶的額外費用。</span><span class="sxs-lookup"><span data-stu-id="6e6ed-148">Your customer will incur no additional costs for the old subscription.</span></span>
