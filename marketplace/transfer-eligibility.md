---
title: 轉移資格-在計費帳戶之間傳輸訂用帳戶的指導方針，Azure Marketplace
description: 在 Azure 入口網站的計費帳戶之間轉移訂用帳戶之前的商業檢查指導方針。
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007154"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="6bd2f-103">在計費帳戶之間轉移訂用帳戶的資格</span><span class="sxs-lookup"><span data-stu-id="6bd2f-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="6bd2f-104">您可以在 Azure 入口網站的計費區段中，將 [訂用](/azure/cost-management-billing/understand/subscription-transfer) 帳戶從一個計費帳戶轉移到另一個帳單帳戶。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="6bd2f-105">在傳輸之前，會掃描訂用帳戶中的協力廠商產品。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="6bd2f-106">只有在 *所有* 產品都已清除以進行傳輸時，才允許傳輸 (請參閱下面的 [準則](#criteria-for-transfer-approval-or-denial)) 。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="6bd2f-107">系統會為無法清除的應用程式產生相關的錯誤訊息，以協助您判斷後續步驟。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="6bd2f-108">本文不適用於 SaaS 供應專案，因為 SaaS 資源會附加至租使用者，而不是訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="6bd2f-109">SaaS 資源可以從一個計費帳戶轉移到另一個計費帳戶，但這是依資源和依 Azure 支援的支援要求來完成。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="6bd2f-110">傳輸核准或拒絕的準則</span><span class="sxs-lookup"><span data-stu-id="6bd2f-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="6bd2f-111">如果任何協力廠商應用程式符合下列任何一個條件，您就無法轉移訂用帳戶：</span><span class="sxs-lookup"><span data-stu-id="6bd2f-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="6bd2f-112">目標帳戶是商業的，且應用程式會退出宣告以透過合作夥伴銷售。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="6bd2f-113">應用程式為選取的夥伴加入，且目標帳戶不在允許清單中。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="6bd2f-114">這項供應專案是過去針對所選訂用帳戶的預覽供應專案，也是私人供應專案，且訂用帳戶已不再位於允許清單中。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="6bd2f-115">新的計費帳戶位於與供應專案銷售位置不同的區域，而供應專案則不會在該區域中銷售。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="6bd2f-116">封鎖的傳輸會維持有效，直到您從訂用帳戶中移除資源為止，之後您可以再次嘗試傳送。</span><span class="sxs-lookup"><span data-stu-id="6bd2f-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6bd2f-117">下一步</span><span class="sxs-lookup"><span data-stu-id="6bd2f-117">Next steps</span></span>

[<span data-ttu-id="6bd2f-118">取得 Microsoft AppSource 和 Azure Marketplace 的支援</span><span class="sxs-lookup"><span data-stu-id="6bd2f-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

