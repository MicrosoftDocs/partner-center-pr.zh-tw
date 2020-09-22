---
title: 在合作夥伴中心中建立客戶訂用帳戶
ms.topic: how-to
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何將您的客戶訂用帳戶銷售給 Microsoft 所發行的產品，以及由協力廠商 Isv 發佈的 SaaS 產品。
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 8c3cfc2a6576029a8fdfb902a7b3889b4ea6c628
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000522"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="a990d-103">建立、暫停或取消客戶訂閱</span><span class="sxs-lookup"><span data-stu-id="a990d-103">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="a990d-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="a990d-104">**Applies to**</span></span>

- <span data-ttu-id="a990d-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a990d-105">Partner Center</span></span>
- <span data-ttu-id="a990d-106">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="a990d-106">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="a990d-107">雲端解決方案提供者合作夥伴</span><span class="sxs-lookup"><span data-stu-id="a990d-107">CSP partners</span></span>

<span data-ttu-id="a990d-108">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="a990d-108">**Appropriate roles**</span></span>

- <span data-ttu-id="a990d-109">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="a990d-109">Admin agent</span></span>
- <span data-ttu-id="a990d-110">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="a990d-110">Billing admin</span></span>
- <span data-ttu-id="a990d-111">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="a990d-111">Global admin</span></span>
- <span data-ttu-id="a990d-112">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="a990d-112">Helpdesk agent</span></span>
- <span data-ttu-id="a990d-113">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="a990d-113">Sales agent</span></span>

<span data-ttu-id="a990d-114">當您在合作夥伴中心中建立客戶的記錄之後，您便可以向他們銷售型錄中產品的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-114">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="a990d-115">這包括 Microsoft 所發佈的產品，以及軟體即服務 (SaaS) 產品，由協力廠商獨立軟體廠商發佈， (Isv) 到 [商用 marketplace](https://azuremarketplace.microsoft.com/marketplace)。</span><span class="sxs-lookup"><span data-stu-id="a990d-115">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="a990d-116">某些供應專案僅限每個客戶一個訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-116">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="a990d-117">若要查看受限制的供應項目清單，請造訪合作夥伴中心 [定價與方案] 頁面。</span><span class="sxs-lookup"><span data-stu-id="a990d-117">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a990d-118">作為 CSP 方案中的合作夥伴，您只能從合作夥伴中心內的 ISV 發行者購買以 **授權為基礎** 的 SaaS 訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-118">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="a990d-119">這表示您可以購買 ISV 發行者提供給您的任何 **授權型** SaaS 供應專案，包括您有權存取的 [專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 。</span><span class="sxs-lookup"><span data-stu-id="a990d-119">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="a990d-120">您必須移至[azure 入口網站](https://portal.azure.com/)，才能向 isv (（例如以**使用量為基礎**、計量付費或以耗用量為基礎的供應專案，包括 Azure 應用程式、容器或) vm）購買或管理其他商用 marketplace 供應專案。</span><span class="sxs-lookup"><span data-stu-id="a990d-120">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="a990d-121">如需詳細資訊，請參閱 [購買商用 marketplace 產品](csp-commercial-marketplace-purchase.md)。</span><span class="sxs-lookup"><span data-stu-id="a990d-121">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="a990d-122">建立新的訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a990d-122">Create a new subscription</span></span>

1. <span data-ttu-id="a990d-123">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a990d-123">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a990d-124">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-124">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a990d-125">選取 [訂用帳戶]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="a990d-125">Select **Add subscription**.</span></span> <span data-ttu-id="a990d-126">[ **線上服務** ] 索引標籤會顯示所有可用的 Marketplace SaaS 供應專案。</span><span class="sxs-lookup"><span data-stu-id="a990d-126">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="a990d-127">若只要查看特定類型的訂用帳戶，請在可用的篩選中進行選取：</span><span class="sxs-lookup"><span data-stu-id="a990d-127">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="a990d-128">**發行者**：選擇 **Microsoft** 以查看 microsoft 提供的供應專案，或查看 isv 所發佈之商業 marketplace 產品的 **合作夥伴** 。</span><span class="sxs-lookup"><span data-stu-id="a990d-128">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="a990d-129">**計費類型**：選取您想要使用的訂用帳戶計費類型： **授權** 或 **使用**方式。</span><span class="sxs-lookup"><span data-stu-id="a990d-129">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="a990d-130">請參閱以 [授權為基礎的帳單](license-based-billing.md) ，以取得可協助您決定每月和每年計費頻率的資訊。</span><span class="sxs-lookup"><span data-stu-id="a990d-130">See [License-based billing](license-based-billing.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="a990d-131">**類別**：選擇 [ **企業**]、[ **小型企業**] 或 [ **試用**]。</span><span class="sxs-lookup"><span data-stu-id="a990d-131">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="a990d-132">如需試用訂用帳戶的相關資訊，請參閱[為您的客戶提供 Microsoft 產品試用版](offer-your-customers-trials-of-microsoft-products.md)。</span><span class="sxs-lookup"><span data-stu-id="a990d-132">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="a990d-133">選取您要為客戶購買的產品訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-133">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="a990d-134">您看到的產品取決於客戶區段的類型 (教育版、政府版等 ) 和您已套用的篩選。</span><span class="sxs-lookup"><span data-stu-id="a990d-134">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="a990d-135">Marketplace 中顯示的某些供應專案可能不一定會提供給特定的客戶或特定的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="a990d-135">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="a990d-136">這可能是因為：</span><span class="sxs-lookup"><span data-stu-id="a990d-136">This can be because:</span></span>

   - <span data-ttu-id="a990d-137">客戶已經有該產品的訂用帳戶，只允許一個</span><span class="sxs-lookup"><span data-stu-id="a990d-137">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="a990d-138">客戶的訂用帳戶可能已暫止 (在此情況下，您可以重新啟用訂用帳戶，而不是購買新的訂用帳戶。 ) </span><span class="sxs-lookup"><span data-stu-id="a990d-138">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="a990d-139">針對 ISV SaaS 供應專案，可能有幾個原因無法購買供應專案： ISV 可能不支援客戶的計費國家或地區;ISV 可能選擇不讓供應專案透過 CSP 方案提供;或者，ISV 可能只對特定 CSP 合作夥伴提供 [專屬](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) 供應專案。</span><span class="sxs-lookup"><span data-stu-id="a990d-139">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="a990d-140">ISV 供應專案也可能無法透過合作夥伴中心 (例如容器或某些以使用量為基礎的供應專案) 來可交易。</span><span class="sxs-lookup"><span data-stu-id="a990d-140">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="a990d-141">針對您要新增的每個訂用帳戶，視需要輸入 (的授權數目) 然後選取 [ **新增至購物車**]。</span><span class="sxs-lookup"><span data-stu-id="a990d-141">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="a990d-142">當您完成新增訂用帳戶時，請選取 [ **審核** ] 並檢查您的訂單。</span><span class="sxs-lookup"><span data-stu-id="a990d-142">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="a990d-143">在您審核訂單並準備好購買這些訂用帳戶之後，請選取 [ **購買**]。</span><span class="sxs-lookup"><span data-stu-id="a990d-143">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="a990d-144">購買客戶的訂用帳戶之後，將會發生下列情況：</span><span class="sxs-lookup"><span data-stu-id="a990d-144">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="a990d-145">您可以從該客戶的 [訂用帳戶 **] 頁面選取** 訂用帳戶名稱，以檢查或編輯訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-145">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="a990d-146">從這裡開始，您可以選取附加元件授權 (如果有的話)、變更授權數量，或暫停訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-146">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="a990d-147">**ISV SaaS (以授權為基礎的) 訂用帳戶：**</span><span class="sxs-lookup"><span data-stu-id="a990d-147">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="a990d-148">您將會收到 ISV 發行者網站的連結。</span><span class="sxs-lookup"><span data-stu-id="a990d-148">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="a990d-149">此連結應可協助您完成客戶訂用帳戶的部署或帳戶設定。</span><span class="sxs-lookup"><span data-stu-id="a990d-149">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="a990d-150">您或您的客戶都不會收到一封電子郵件，說明如何完成此類型 ISV 訂用帳戶的帳戶設定/布建。 ) </span><span class="sxs-lookup"><span data-stu-id="a990d-150">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="a990d-151">如果您的訂用帳戶隨附30天的免費試用版，則會自動套用免費試用期限。</span><span class="sxs-lookup"><span data-stu-id="a990d-151">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="a990d-152">作為 CSP 方案中的合作夥伴，您不能在購買給客戶的供應專案上豁免免費試用期。</span><span class="sxs-lookup"><span data-stu-id="a990d-152">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="a990d-153">當免費試用期結束後，訂用帳戶期限將會開始，且訂用帳戶將會轉換為付費狀態。</span><span class="sxs-lookup"><span data-stu-id="a990d-153">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="a990d-154">然後，訂用帳戶會根據相同的排程自動續約。</span><span class="sxs-lookup"><span data-stu-id="a990d-154">The subscription will then auto-renew according to the same schedule.</span></span>
   
## <a name="update-subscriptions-with-add-ons"></a><span data-ttu-id="a990d-155">更新具有附加元件的訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a990d-155">Update subscriptions with add-ons</span></span> 

<span data-ttu-id="a990d-156">若要購買附加元件，客戶必須先具備作用中的基本訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-156">To purchase an add-on the customer must first have an active base subscription.</span></span>  <span data-ttu-id="a990d-157">您無法透過類別目錄來購買附加元件。</span><span class="sxs-lookup"><span data-stu-id="a990d-157">You can't purchase add-ons through the catalog.</span></span>

1. <span data-ttu-id="a990d-158">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a990d-158">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a990d-159">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-159">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a990d-160">選擇您要管理的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-160">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="a990d-161">在 [ **狀態** ] 區段下方，是訂用帳戶的可用附加元件清單。</span><span class="sxs-lookup"><span data-stu-id="a990d-161">Below the **Status** section, are a list of available Add-ons for the subscription.</span></span>  

5. <span data-ttu-id="a990d-162">更新每個必要附加元件的授權數量。</span><span class="sxs-lookup"><span data-stu-id="a990d-162">Update the quantity of licenses for each required Add-on.</span></span> <span data-ttu-id="a990d-163">然後，**提交**您的變更。</span><span class="sxs-lookup"><span data-stu-id="a990d-163">Then **Submit** your changes.</span></span>

<span data-ttu-id="a990d-164">透過合作夥伴中心購買附加元件的能力僅適用于直接帳單和間接提供者。</span><span class="sxs-lookup"><span data-stu-id="a990d-164">The ability to purchase add-ons through Partner Center is only available to direct bill and indirect providers.</span></span>
<span data-ttu-id="a990d-165">根據基本需求和區域可用性，只會顯示合格的附加元件。</span><span class="sxs-lookup"><span data-stu-id="a990d-165">Only eligible add-ons are displayed based on the base requirements and regional availability.</span></span> <span data-ttu-id="a990d-166">如需定價和供應項目的詳細資訊，請參閱雲端轉銷商供應項目矩陣。</span><span class="sxs-lookup"><span data-stu-id="a990d-166">Refer to the Cloud Reseller offer matrix for more information about pricing and offers.</span></span>  <span data-ttu-id="a990d-167">暫止基本訂用帳戶，也會暫止任何相關聯的附加元件。</span><span class="sxs-lookup"><span data-stu-id="a990d-167">Suspending the base subscription will also suspend any associated add-ons.</span></span>

<span data-ttu-id="a990d-168">附加元件的開始日期會與基本訂用帳戶一致，費用會根據收費開始日期和收費結束日期計算，並在第一張發票中按比例收費。</span><span class="sxs-lookup"><span data-stu-id="a990d-168">Start dates for add-ons align to the base subscription and charges are calculated from the Charge start date and Charge end date with pro-rata charges in the first invoice.</span></span> <span data-ttu-id="a990d-169">如需其他資訊，請參閱以 [授權為基礎的計費](license-based-billing.md)。</span><span class="sxs-lookup"><span data-stu-id="a990d-169">For additional information see, [License-based billing](license-based-billing.md).</span></span>


## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="a990d-170">暫停或取消訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a990d-170">Suspend or cancel a subscription</span></span>

<span data-ttu-id="a990d-171">如果客戶要求，或是發生未付款或詐騙等情形，合作夥伴可以暫停或取消訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-171">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="a990d-172">暫停訂閱</span><span class="sxs-lookup"><span data-stu-id="a990d-172">Suspend a subscription</span></span>

<span data-ttu-id="a990d-173">當您將訂閱的狀態變更為 **\[已暫停\]** 時，使用者就無法登入或存取服務。</span><span class="sxs-lookup"><span data-stu-id="a990d-173">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="a990d-174">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a990d-174">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a990d-175">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-175">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a990d-176">選擇您要管理的訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-176">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="a990d-177">在 [狀態]  區段中，選擇 [暫止]  。</span><span class="sxs-lookup"><span data-stu-id="a990d-177">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="a990d-178">然後，**提交**您的變更。</span><span class="sxs-lookup"><span data-stu-id="a990d-178">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="a990d-179">所有的資料將被刪除，除非訂用帳戶在 90 日内重新啟用，或 90 天加上開啟帳戶的時間和第一個計費期間之間的天數 (最多 120 天)。</span><span class="sxs-lookup"><span data-stu-id="a990d-179">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="a990d-180">當您在暫停訂用帳戶時，您在 [已暫停]\*\*\*\* 按鈕下方看到的日期會顯示該訂用帳戶何時會自動到期 (如果您沒有重新啟用的話)。</span><span class="sxs-lookup"><span data-stu-id="a990d-180">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> 

### <a name="cancel-a-subscription"></a><span data-ttu-id="a990d-181">取消訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a990d-181">Cancel a subscription</span></span>

<span data-ttu-id="a990d-182">您可以選擇從合作夥伴中心 [商用 marketplace](csp-commercial-marketplace-overview.md)中的協力廠商 ISV 發行者，取消以授權為基礎的 SaaS 訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-182">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="a990d-183">只要您在取消期間內取消，就會收到完整退款。</span><span class="sxs-lookup"><span data-stu-id="a990d-183">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="a990d-184">針對 ISV 優惠，每月計費：</span><span class="sxs-lookup"><span data-stu-id="a990d-184">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="a990d-185">如果您在下訂單後取消了24小時以外的時間，您將會在下一張發票上收到完整的信用額度。</span><span class="sxs-lookup"><span data-stu-id="a990d-185">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="a990d-186">如果您在下一次訂單之後取消超過24小時，則會排程在續約時進行取消。</span><span class="sxs-lookup"><span data-stu-id="a990d-186">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="a990d-187">針對每年計費的優惠：</span><span class="sxs-lookup"><span data-stu-id="a990d-187">For offers billed annually:</span></span>

- <span data-ttu-id="a990d-188">如果您在下訂單後取消了14天，您將會在下一張發票上收到完整的信用額度。</span><span class="sxs-lookup"><span data-stu-id="a990d-188">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="a990d-189">如果您在下一次訂單後取消超過14天，取消將會排定在續約時進行。</span><span class="sxs-lookup"><span data-stu-id="a990d-189">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="a990d-190">在這些期間結束之後，您就不會再看到取消訂用帳戶的選項。</span><span class="sxs-lookup"><span data-stu-id="a990d-190">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="a990d-191">使用虛擬機器或容器的使用量型和計量付費、協力廠商 ISV 服務 (，例如) 不符合退貨資格。</span><span class="sxs-lookup"><span data-stu-id="a990d-191">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="a990d-192">以使用量為基礎的服務可以取消布建為取消方法。</span><span class="sxs-lookup"><span data-stu-id="a990d-192">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="a990d-193">由於費用是在使用之後計費，因此這些服務不符合退款資格。</span><span class="sxs-lookup"><span data-stu-id="a990d-193">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="a990d-194">若要取消 ISV 發行者提供的授權型 SaaS 訂用帳戶，請執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="a990d-194">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="a990d-195">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a990d-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a990d-196">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a990d-197">找出您要取消的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-197">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="a990d-198">在 [ **狀態** ] 資料行中，選取 [ **取消**]。</span><span class="sxs-lookup"><span data-stu-id="a990d-198">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="a990d-199">然後，**提交**您的變更。</span><span class="sxs-lookup"><span data-stu-id="a990d-199">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="a990d-200">如果出現對話方塊，請填寫任何相關的詳細資料，然後選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="a990d-200">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="a990d-201">若要確認取消，請選取 **[是，取消]**。</span><span class="sxs-lookup"><span data-stu-id="a990d-201">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="a990d-202">您也可以選擇使用 Api 取消 Azure Marketplace 的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-202">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="a990d-203">若要這樣做，請參閱 [取消 Azure Marketplace 訂](/partner-center/develop/cancel-an-azure-marketplace-subscription)用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-203">To do so, see [Cancel an Azure Marketplace subscription](/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="a990d-204">選擇是否要自動續訂商業市集訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="a990d-204">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="a990d-205">根據預設，使用中的訂閱會設定為在訂閱期間到期時自動續訂。</span><span class="sxs-lookup"><span data-stu-id="a990d-205">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="a990d-206">針對 [商用 marketplace 產品的訂閱](csp-commercial-marketplace-overview.md)，您可以選擇性地選擇不自動更新訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-206">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="a990d-207">若要停止有效的商業 marketplace 訂用帳戶，使其無法自動更新：</span><span class="sxs-lookup"><span data-stu-id="a990d-207">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="a990d-208">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="a990d-208">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="a990d-209">從 [合作夥伴中心] 功能表上，選取 [客戶]，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-209">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="a990d-210">選取 **訂用帳戶** 。</span><span class="sxs-lookup"><span data-stu-id="a990d-210">Select **Subscriptions**.</span></span> <span data-ttu-id="a990d-211">這會列出您為客戶購買的任何授權型訂閱。</span><span class="sxs-lookup"><span data-stu-id="a990d-211">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="a990d-212">在 [ **訂** 用帳戶] 資料行中，選取您要修改的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="a990d-212">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="a990d-213">在 [訂閱詳細資料] 頁面中，找出 [ **狀態** ] 區段，並取消核取 [ **自動更新** ] 方塊。</span><span class="sxs-lookup"><span data-stu-id="a990d-213">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="a990d-214">選取 [提交]。</span><span class="sxs-lookup"><span data-stu-id="a990d-214">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a990d-215">下一步</span><span class="sxs-lookup"><span data-stu-id="a990d-215">Next steps</span></span>

- [<span data-ttu-id="a990d-216">為您的客戶購買商業市集產品</span><span class="sxs-lookup"><span data-stu-id="a990d-216">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="a990d-217">為您的客戶管理商業 marketplace 產品</span><span class="sxs-lookup"><span data-stu-id="a990d-217">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="a990d-218">商務 Marketplace 概觀</span><span class="sxs-lookup"><span data-stu-id="a990d-218">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)