---
title: 稅務原則如何影響 Azure Marketplace 的支出
description: 瞭解稅務原則如何影響 Azure Marketplace 的支出。
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758454"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="57f55-103">稅務原則如何影響 Azure Marketplace 的支出</span><span class="sxs-lookup"><span data-stu-id="57f55-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="57f55-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="57f55-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="57f55-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="57f55-105">Global admin</span></span>
-    <span data-ttu-id="57f55-106">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="57f55-106">User admin</span></span>
-    <span data-ttu-id="57f55-107">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="57f55-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="57f55-108">簡介</span><span class="sxs-lookup"><span data-stu-id="57f55-108">Introduction</span></span>

<span data-ttu-id="57f55-109">Microsoft 商用 marketplace 的範圍遍及全球。</span><span class="sxs-lookup"><span data-stu-id="57f55-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="57f55-110">交易會跨框線進行，視 ISV 和客戶所在的位置而定，稅金影響可能會有所不同。</span><span class="sxs-lookup"><span data-stu-id="57f55-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="57f55-111">Microsoft AppSource 和 Azure Marketplace 會使用合作夥伴中心稅務設定檔資訊來判斷 ISV 的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="57f55-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="57f55-112">若要判斷客戶的國家/地區，請使用客戶的帳單資訊，或者，如果客戶是在歐盟，我們會使用兩個不同的資訊片段。</span><span class="sxs-lookup"><span data-stu-id="57f55-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="57f55-113">若要進一步瞭解下列案例，請參閱 [稅務詳細資料](tax-details-marketplace.md) 表格，其中會顯示 Microsoft 是否代表發行者收取和支付稅金，或者該責任是否屬於發行者。</span><span class="sxs-lookup"><span data-stu-id="57f55-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="57f55-114">本主題中的所有範例銷售值和稅額百分比僅供說明之用，而非精確的數位。</span><span class="sxs-lookup"><span data-stu-id="57f55-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="57f55-115">Microsoft 管理的國家/地區的發行者交易</span><span class="sxs-lookup"><span data-stu-id="57f55-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="57f55-116">**案例 A** -在 [Microsoft 管理的國家/地區](tax-details-marketplace.md#microsoft-managed-countries)的發行者與客戶之間進行的交易。</span><span class="sxs-lookup"><span data-stu-id="57f55-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="57f55-117">在銷售時，這些交易將會加上適用的稅額，而 Microsoft 會將該稅金傳送到適用的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="57f55-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="57f55-118">付款和付款計算不會收取稅金。</span><span class="sxs-lookup"><span data-stu-id="57f55-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="57f55-119">請參閱 [案例 D](#foreign-publisher-transacts-with-us-customer) ，以瞭解非 US 發行者與美國客戶之間的交易。</span><span class="sxs-lookup"><span data-stu-id="57f55-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="顯示支付進程案例 A 的工作流程。":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="57f55-121">發行者交易在 Microsoft 管理的國家/地區，其中 Marketplace 費用是可免稅服務</span><span class="sxs-lookup"><span data-stu-id="57f55-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="57f55-122">**案例 B** -在以美國為基礎的發行者之間進行的交易 (如合作夥伴中心的稅務設定檔資訊所定義) 給以 Microsoft 管理的國家/地區為客戶提供的 Marketplace 費用 (的可計費服務) 的稅。</span><span class="sxs-lookup"><span data-stu-id="57f55-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="57f55-123">在此案例中，商店服務費用的稅額會從發行者的付款扣除。</span><span class="sxs-lookup"><span data-stu-id="57f55-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="顯示付款流程案例 B 的工作流程。":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="57f55-125">發行者管理的稅務國家/地區交易</span><span class="sxs-lookup"><span data-stu-id="57f55-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="57f55-126">**案例 C** -在發行者和客戶之間發生的交易，該國家/地區不會在客戶上強加扣繳稅。</span><span class="sxs-lookup"><span data-stu-id="57f55-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="57f55-127">客戶不需要支付任何費用，而是發行者的義務來支付所有適用的稅金。</span><span class="sxs-lookup"><span data-stu-id="57f55-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="57f55-128">如需特定國家（地區）定價 (的詳細資訊，例如，若要抵消即將推出的稅務) 請參閱 [商用 marketplace 供應專案的方案和定價](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices)。</span><span class="sxs-lookup"><span data-stu-id="57f55-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="顯示支付進程案例 C 的工作流程。":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="57f55-130">與 US 客戶的外部發行者交易</span><span class="sxs-lookup"><span data-stu-id="57f55-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="57f55-131">**案例 D** -所有外部發行者都 (如其合作夥伴中心稅務設定檔資訊) 在不含美國條約的國家/地區所定義 (請參閱 [案例 E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) 向以美國為基礎的客戶 (（如其客戶帳戶位址) 所定義）進行銷售。</span><span class="sxs-lookup"><span data-stu-id="57f55-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="57f55-132">美國政府需要代表發行者進行 Microsoft 預繳稅。</span><span class="sxs-lookup"><span data-stu-id="57f55-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="57f55-133">從付款支付至發行者的稅金是根據供應專案價格來計算。</span><span class="sxs-lookup"><span data-stu-id="57f55-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="顯示付款流程案例 D 的工作流程。":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="57f55-135">具有美國客戶的條約交易的外部發行者</span><span class="sxs-lookup"><span data-stu-id="57f55-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="57f55-136">**案例 E** -所有外部發行者都 (如其合作夥伴中心稅務設定檔資訊所定義) 在具有美國條約的國家/地區中，以美國條約的國家/地區提供銷售給美國客戶 () 的客戶帳戶位址定義。</span><span class="sxs-lookup"><span data-stu-id="57f55-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="57f55-137">美國政府不需要代表發行者來進行 Microsoft 的扣稅。</span><span class="sxs-lookup"><span data-stu-id="57f55-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="顯示支付進程案例 E 的工作流程。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="57f55-139">外部發行者在 Microsoft 管理的國家/地區銷售給歐盟 加值稅 註冊的客戶 (愛爾蘭以外的國家) </span><span class="sxs-lookup"><span data-stu-id="57f55-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="57f55-140">**案例 F** –外部發行者與歐盟 加值稅 註冊客戶之間的所有交易， (在 Microsoft-Managed 國家/地區的愛爾蘭) 以外的國家/地區。</span><span class="sxs-lookup"><span data-stu-id="57f55-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="57f55-141">客戶不會在銷售時支付稅款。</span><span class="sxs-lookup"><span data-stu-id="57f55-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="顯示付款流程案例 F 的工作流程。":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="57f55-143">外部發行者會在愛爾蘭于 Microsoft 管理的國家/地區 (銷售給歐盟 加值稅 註冊的客戶) </span><span class="sxs-lookup"><span data-stu-id="57f55-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="57f55-144">**案例 G** -外部發行者與歐盟 加值稅 註冊客戶之間的所有交易， (在 Microsoft-Managed 國家/地區的愛爾蘭) 內。</span><span class="sxs-lookup"><span data-stu-id="57f55-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="57f55-145">客戶會支付愛爾蘭加值稅，Microsoft 會向愛爾蘭政府支付這款稅額。</span><span class="sxs-lookup"><span data-stu-id="57f55-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="顯示付款流程案例 G 的工作流程。":::

## <a name="next-steps"></a><span data-ttu-id="57f55-147">下一步</span><span class="sxs-lookup"><span data-stu-id="57f55-147">Next steps</span></span>

- [<span data-ttu-id="57f55-148">發行者常見問題</span><span class="sxs-lookup"><span data-stu-id="57f55-148">Publisher FAQ</span></span>](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="57f55-149">建立付款和稅務設定檔的指示</span><span class="sxs-lookup"><span data-stu-id="57f55-149">Instructions to create payment and tax profiles</span></span>](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
