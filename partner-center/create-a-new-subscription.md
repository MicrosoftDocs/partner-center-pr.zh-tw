---
title: 在合作夥伴中心建立客戶訂用帳戶
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何向 Microsoft 所發佈的產品以及由協力廠商 Isv 發佈的 SaaS 產品，銷售您的客戶訂用帳戶。
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: 訂用帳戶，建立新的訂用帳戶，暫停，取消，暫停，暫停，SaaS，授權，ISV，協力廠商
ms.localizationpriority: medium
ms.openlocfilehash: 3588fb8408ef3c190813691d42331753ac531a8f
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991490"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a><span data-ttu-id="367e9-104">建立、暫停或取消客戶訂閱</span><span class="sxs-lookup"><span data-stu-id="367e9-104">Create, suspend, or cancel customer subscriptions</span></span>

<span data-ttu-id="367e9-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="367e9-105">**Applies to**</span></span>

- <span data-ttu-id="367e9-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="367e9-106">Partner Center</span></span>
- <span data-ttu-id="367e9-107">Microsoft Cloud for US Government 適用的合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="367e9-107">Partner Center for Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="367e9-108">雲端解決方案提供者合作夥伴</span><span class="sxs-lookup"><span data-stu-id="367e9-108">CSP partners</span></span>

<span data-ttu-id="367e9-109">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="367e9-109">**Appropriate roles**</span></span>

- <span data-ttu-id="367e9-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="367e9-110">Admin agent</span></span>
- <span data-ttu-id="367e9-111">帳單系統管理員</span><span class="sxs-lookup"><span data-stu-id="367e9-111">Billing admin</span></span>
- <span data-ttu-id="367e9-112">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="367e9-112">Global admin</span></span>
- <span data-ttu-id="367e9-113">技術服務代理人</span><span class="sxs-lookup"><span data-stu-id="367e9-113">Helpdesk agent</span></span>
- <span data-ttu-id="367e9-114">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="367e9-114">Sales agent</span></span>

<span data-ttu-id="367e9-115">當您在合作夥伴中心中建立客戶的記錄之後，您便可以向他們銷售型錄中產品的訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-115">After you've created a record of your customer in the Partner Center, you can sell them subscriptions to products in the catalog.</span></span> <span data-ttu-id="367e9-116">這包括由 Microsoft 發佈的產品，以及由協力廠商獨立軟體廠商（Isv）發佈到[商業 marketplace](https://azuremarketplace.microsoft.com/marketplace)的軟體即服務（SaaS）產品。</span><span class="sxs-lookup"><span data-stu-id="367e9-116">This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace).</span></span>

<span data-ttu-id="367e9-117">某些供應專案僅限每個客戶有一個訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-117">Some offers are limited to one subscription per customer.</span></span> <span data-ttu-id="367e9-118">若要查看受限制的供應項目清單，請造訪合作夥伴中心 [定價與方案] 頁面。</span><span class="sxs-lookup"><span data-stu-id="367e9-118">To see a list of which offers are restricted, visit the Partner Center Pricing and Offers page.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="367e9-119">身為 CSP 計畫的合作夥伴，您只能從合作夥伴中心內的 ISV 發行者購買以**授權為基礎**的 SaaS 訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-119">As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center.</span></span> <span data-ttu-id="367e9-120">這表示您可以購買 ISV 發行者已提供給您的任何**授權型**SaaS 供應專案，包括您有權存取的[專屬優惠](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)。</span><span class="sxs-lookup"><span data-stu-id="367e9-120">This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access.</span></span> <span data-ttu-id="367e9-121">若要向 Isv 購買或管理其他的商業 marketplace 供應專案（例如，以**使用量為基礎**、計量付費或涉及 Azure 應用程式、容器或 vm 的耗用量型供應專案），您必須移至[azure 管理入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="367e9-121">To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered, or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/).</span></span> <span data-ttu-id="367e9-122">如需詳細資訊，請參閱[購買商用 marketplace 產品](csp-commercial-marketplace-purchase.md)。</span><span class="sxs-lookup"><span data-stu-id="367e9-122">For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).</span></span>

## <a name="create-a-new-subscription"></a><span data-ttu-id="367e9-123">建立新的訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="367e9-123">Create a new subscription</span></span>

1. <span data-ttu-id="367e9-124">登入[合作夥伴中心儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="367e9-124">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="367e9-125">從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="367e9-126">選取 [訂用帳戶]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="367e9-126">Select **Add subscription**.</span></span> <span data-ttu-id="367e9-127">[**線上服務**] 索引標籤會顯示所有可用的 Marketplace SaaS 供應專案。</span><span class="sxs-lookup"><span data-stu-id="367e9-127">The **Online Services** tab will show all available Marketplace SaaS offers.</span></span>

4. <span data-ttu-id="367e9-128">若只要查看特定類型的訂用帳戶，請在可用的篩選中進行選取：</span><span class="sxs-lookup"><span data-stu-id="367e9-128">To see only certain types of subscriptions, make selections in the available filters:</span></span>
   - <span data-ttu-id="367e9-129">**發行者**：選擇 [ **microsoft** ] 僅查看 microsoft 或**合作夥伴**提供的供應專案，以查看 isv 所發佈的商業 marketplace 產品。</span><span class="sxs-lookup"><span data-stu-id="367e9-129">**Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.</span></span>
   - <span data-ttu-id="367e9-130">**計費類型**：選取您想要使用的訂用帳戶計費類型： [**授權**] 或 [**使用**方式]。</span><span class="sxs-lookup"><span data-stu-id="367e9-130">**Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**.</span></span> <span data-ttu-id="367e9-131">如需可協助您在每月與年度計費頻率之間做選擇的詳細資訊，請參閱[新計費功能的常見問題集](faq-about-new-billing-features.md)。</span><span class="sxs-lookup"><span data-stu-id="367e9-131">See [FAQ about new billing features](faq-about-new-billing-features.md) for information that will help you decide between the monthly and annual billing frequency.</span></span>
   - <span data-ttu-id="367e9-132">**類別**：選擇 [**企業**]、[**小型企業**] 或 [**試用**]。</span><span class="sxs-lookup"><span data-stu-id="367e9-132">**Category**: Choose **Enterprise**, **Small business**, or **Trial**.</span></span> <span data-ttu-id="367e9-133">如需試用訂用帳戶的相關資訊，請參閱[為您的客戶提供 Microsoft 產品試用版](offer-your-customers-trials-of-microsoft-products.md)。</span><span class="sxs-lookup"><span data-stu-id="367e9-133">For info about trial subscriptions, see [Offer your customers trials of Microsoft products](offer-your-customers-trials-of-microsoft-products.md).</span></span>

5. <span data-ttu-id="367e9-134">選取您想要為客戶購買的產品訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-134">Select the product subscriptions you want to purchase for your customer.</span></span> <span data-ttu-id="367e9-135">您看到的產品取決於客戶區段的類型（教育、政府等），以及您已套用的篩選。</span><span class="sxs-lookup"><span data-stu-id="367e9-135">The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied.</span></span> <span data-ttu-id="367e9-136">Marketplace 上顯示的某些供應專案可能不一定會提供給特定的客戶或特定的 CSP 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="367e9-136">Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner.</span></span> <span data-ttu-id="367e9-137">這可能是因為：</span><span class="sxs-lookup"><span data-stu-id="367e9-137">This can be because:</span></span>

   - <span data-ttu-id="367e9-138">客戶已有該產品的訂用帳戶，且只允許一個</span><span class="sxs-lookup"><span data-stu-id="367e9-138">The customer already has a subscription to that product and is only allowed one</span></span>

   - <span data-ttu-id="367e9-139">客戶的訂用帳戶可能已暫停（在此情況下，您可以重新啟用訂用帳戶，而不是購買新的）。</span><span class="sxs-lookup"><span data-stu-id="367e9-139">The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)</span></span>

   - <span data-ttu-id="367e9-140">針對 ISV SaaS 供應專案，可能有幾個原因導致無法購買供應專案： ISV 可能不支援客戶的帳單國家或地區;ISV 可能選擇不透過 CSP 計畫提供供應專案;或者，ISV 可能只對特定 CSP 合作夥伴提供[專屬](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers)供應專案。</span><span class="sxs-lookup"><span data-stu-id="367e9-140">For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners.</span></span> <span data-ttu-id="367e9-141">ISV 供應專案可能也不會透過合作夥伴中心 transactable （例如，容器或某些以使用量為基礎的優惠）。</span><span class="sxs-lookup"><span data-stu-id="367e9-141">The ISV offer may also not be transactable through the Partner Center (for example, containers or some usage-based offers).</span></span>  

6. <span data-ttu-id="367e9-142">針對您想要新增的每個訂用帳戶，輸入授權數目（如有需要），然後選取 [**新增至購物車**]。</span><span class="sxs-lookup"><span data-stu-id="367e9-142">For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.</span></span>

7. <span data-ttu-id="367e9-143">當您完成新增訂閱之後，請選取 [**審查**]，並檢查您的訂單。</span><span class="sxs-lookup"><span data-stu-id="367e9-143">When you are finished adding subscriptions, select **Review** and review your order.</span></span>

8. <span data-ttu-id="367e9-144">當您已審核訂單並準備好購買這些訂閱之後，請選取 [**購買**]。</span><span class="sxs-lookup"><span data-stu-id="367e9-144">Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.</span></span>

9. <span data-ttu-id="367e9-145">購買客戶的訂用帳戶之後，將會發生下列情況：</span><span class="sxs-lookup"><span data-stu-id="367e9-145">After you buy a subscription for a customer, the following will occur:</span></span>

    - <span data-ttu-id="367e9-146">您可以從該客戶的**訂閱**頁面中選取訂用帳戶名稱，以檢查或編輯訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-146">You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page.</span></span> <span data-ttu-id="367e9-147">從這裡開始，您可以選取附加元件授權 (如果有的話)、變更授權數量，或暫停訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-147">From here, you can select add-on licenses if any are available, change the quantity of licenses, or suspend the subscription.</span></span>

    <span data-ttu-id="367e9-148">**針對 ISV SaaS （以授權為基礎）的訂用帳戶：**</span><span class="sxs-lookup"><span data-stu-id="367e9-148">**For ISV SaaS (license-based) subscriptions:**</span></span>
    - <span data-ttu-id="367e9-149">您會收到「ISV 發行者」網站的連結。</span><span class="sxs-lookup"><span data-stu-id="367e9-149">You will receive a link to the ISV publisher's site.</span></span> <span data-ttu-id="367e9-150">此連結應該可協助您完成客戶訂閱的部署或帳戶設定。</span><span class="sxs-lookup"><span data-stu-id="367e9-150">This link should help you complete the deployment or account setup of the customer's subscription.</span></span>
      
    >[!NOTE]
    > <span data-ttu-id="367e9-151">您或您的客戶都不會收到一封電子郵件，說明如何針對此類型的 ISV 訂閱完成帳戶設定/布建。）</span><span class="sxs-lookup"><span data-stu-id="367e9-151">Neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)</span></span>

    - <span data-ttu-id="367e9-152">如果您的訂用帳戶隨附30天免費試用版，將會自動套用免費試用期限。</span><span class="sxs-lookup"><span data-stu-id="367e9-152">If your subscription comes with a 30-day free trial, the free trial period will be applied automatically.</span></span> <span data-ttu-id="367e9-153">身為 CSP 計畫的合作夥伴，您無法在購買給客戶的供應專案上放棄免費試用期。</span><span class="sxs-lookup"><span data-stu-id="367e9-153">As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers.</span></span> <span data-ttu-id="367e9-154">一旦免費試用期結束後，訂用帳戶期限就會開始，且訂用帳戶將會轉換成付費狀態。</span><span class="sxs-lookup"><span data-stu-id="367e9-154">Once the free trial period ends, the subscription term will begin and the subscription will convert to paid status.</span></span> <span data-ttu-id="367e9-155">然後，訂用帳戶會根據相同的排程進行 autorenew。</span><span class="sxs-lookup"><span data-stu-id="367e9-155">The subscription will then autorenew according to the same schedule.</span></span>

## <a name="suspend-or-cancel-a-subscription"></a><span data-ttu-id="367e9-156">暫停或取消訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="367e9-156">Suspend or cancel a subscription</span></span>

<span data-ttu-id="367e9-157">如果客戶要求，或是發生未付款或詐騙等情形，合作夥伴可以暫停或取消訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-157">Partners can suspend or cancel a subscription if requested by the customer, or in cases of nonpayment or fraud.</span></span>

### <a name="suspend-a-subscription"></a><span data-ttu-id="367e9-158">暫停訂閱</span><span class="sxs-lookup"><span data-stu-id="367e9-158">Suspend a subscription</span></span>

<span data-ttu-id="367e9-159">當您將訂閱的狀態變更為 **\[已暫停\]** 時，使用者就無法登入或存取服務。</span><span class="sxs-lookup"><span data-stu-id="367e9-159">When you change the status of a subscription to **Suspended**, users are not able to sign in or access services.</span></span>

1. <span data-ttu-id="367e9-160">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="367e9-160">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="367e9-161">從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-161">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="367e9-162">選擇您要管理的訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-162">Choose the subscription you want to manage.</span></span>

4. <span data-ttu-id="367e9-163">在 [狀態]  區段中，選擇 [暫止]  。</span><span class="sxs-lookup"><span data-stu-id="367e9-163">In the **Status** section, choose **Suspended**.</span></span> <span data-ttu-id="367e9-164">然後，**提交**您的變更。</span><span class="sxs-lookup"><span data-stu-id="367e9-164">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="367e9-165">所有的資料將被刪除，除非訂用帳戶在 90 日内重新啟用，或 90 天加上開啟帳戶的時間和第一個計費期間之間的天數 (最多 120 天)。</span><span class="sxs-lookup"><span data-stu-id="367e9-165">All data will be deleted unless the subscription is reactivated within 90 days, or 90 days plus the number of days between the time the account was opened and the first billing period (maximum 120 days).</span></span>

<span data-ttu-id="367e9-166">當您在暫停訂用帳戶時，您在 [已暫停]\*\*\*\* 按鈕下方看到的日期會顯示該訂用帳戶何時會自動到期 (如果您沒有重新啟用的話)。</span><span class="sxs-lookup"><span data-stu-id="367e9-166">When you suspend a subscription, the date you see below the **Suspended** button indicates when the subscription would automatically expire if you don't reactivate it.</span></span> <span data-ttu-id="367e9-167">如需詳細資訊，請參閱[關於新帳單功能的常見問題](faq-about-new-billing-features.md)。</span><span class="sxs-lookup"><span data-stu-id="367e9-167">For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).</span></span>

### <a name="cancel-a-subscription"></a><span data-ttu-id="367e9-168">取消訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="367e9-168">Cancel a subscription</span></span>

<span data-ttu-id="367e9-169">您可以選擇在合作夥伴中心的[商業市場](csp-commercial-marketplace-overview.md)中，取消協力廠商 ISV 發行者的授權型 SaaS 訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-169">You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md).</span></span> <span data-ttu-id="367e9-170">只要您在取消期間取消，您就會收到完整退款。</span><span class="sxs-lookup"><span data-stu-id="367e9-170">As long as you cancel within the cancellation period, you will receive a full refund.</span></span>

<span data-ttu-id="367e9-171">針對每月計費的 ISV 優惠：</span><span class="sxs-lookup"><span data-stu-id="367e9-171">For ISV offers billed monthly:</span></span>

- <span data-ttu-id="367e9-172">如果您在下一次訂單後取消少於24小時，您會在下一張發票上收到完整的點數。</span><span class="sxs-lookup"><span data-stu-id="367e9-172">If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="367e9-173">如果您在下一次訂單後於24小時後取消，則會排程在續約時進行取消。</span><span class="sxs-lookup"><span data-stu-id="367e9-173">If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="367e9-174">針對每年計費的優惠：</span><span class="sxs-lookup"><span data-stu-id="367e9-174">For offers billed annually:</span></span>

- <span data-ttu-id="367e9-175">如果您在下一次訂單後取消少於14天，您將會在下一張發票上收到完整的點數。</span><span class="sxs-lookup"><span data-stu-id="367e9-175">If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.</span></span>

- <span data-ttu-id="367e9-176">如果您在下一次訂單後的14天后取消，將會排定在續約時進行取消。</span><span class="sxs-lookup"><span data-stu-id="367e9-176">If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.</span></span>

<span data-ttu-id="367e9-177">在這些期間結束之後，您就不會再看到取消訂用帳戶的選項。</span><span class="sxs-lookup"><span data-stu-id="367e9-177">After these periods are over, you will no longer see the option to cancel the subscription.</span></span>

> [!NOTE]
> <span data-ttu-id="367e9-178">以使用量為基礎和計量付費，協力廠商 ISV 服務（例如，使用虛擬機器或容器）並不符合退貨資格。</span><span class="sxs-lookup"><span data-stu-id="367e9-178">Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return.</span></span> <span data-ttu-id="367e9-179">以使用方式為基礎的服務可以解除布建為取消方法。</span><span class="sxs-lookup"><span data-stu-id="367e9-179">Usage-based services can be de-provisioned as a cancellation method.</span></span> <span data-ttu-id="367e9-180">因為費用會在使用後計費，所以這些服務不符合退款資格。</span><span class="sxs-lookup"><span data-stu-id="367e9-180">Since charges are billed after use, these services are not eligible for a refund.</span></span>

<span data-ttu-id="367e9-181">若要取消 ISV 發行者提供的授權型 SaaS 訂用帳戶，請執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="367e9-181">To cancel a license-based SaaS subscription from an ISV publisher, do the following:</span></span>

1. <span data-ttu-id="367e9-182">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="367e9-182">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="367e9-183">從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-183">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="367e9-184">找出您想要取消的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-184">Locate the subscription you want to cancel.</span></span>

4. <span data-ttu-id="367e9-185">在 [**狀態**] 欄中，選取 [**取消**]。</span><span class="sxs-lookup"><span data-stu-id="367e9-185">In the **Status** column, select **Cancel**.</span></span> <span data-ttu-id="367e9-186">然後，**提交**您的變更。</span><span class="sxs-lookup"><span data-stu-id="367e9-186">Then **Submit** your changes.</span></span>

5. <span data-ttu-id="367e9-187">如果出現對話方塊，請填寫任何相關的詳細資料，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="367e9-187">If a dialog box appears, fill out any relevant details then select **Submit**.</span></span>

6. <span data-ttu-id="367e9-188">若要確認取消，請選取 **[是，取消]**。</span><span class="sxs-lookup"><span data-stu-id="367e9-188">To confirm the cancellation, select **Yes, cancel**.</span></span>

> [!NOTE]
> <span data-ttu-id="367e9-189">您也可以選擇使用 Api 取消 Azure Marketplace 訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-189">You can also choose to cancel an Azure Marketplace subscription using APIs.</span></span> <span data-ttu-id="367e9-190">若要這麼做，請參閱[取消 Azure Marketplace 訂](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription)用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-190">To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).</span></span>

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a><span data-ttu-id="367e9-191">選擇是否要自動續訂商業市集訂用帳戶</span><span class="sxs-lookup"><span data-stu-id="367e9-191">Choose whether to automatically renew a commercial marketplace subscription</span></span>

<span data-ttu-id="367e9-192">根據預設，使用中的訂用帳戶會設定為在訂用帳戶期間到期時自動續訂。</span><span class="sxs-lookup"><span data-stu-id="367e9-192">By default, active subscriptions are set to automatically renew when the subscription period expires.</span></span> <span data-ttu-id="367e9-193">對於[商業市集產品的訂用帳戶](csp-commercial-marketplace-overview.md)，您可以選擇不自動更新訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-193">For [subscriptions to commercial marketplace products](csp-commercial-marketplace-overview.md), you can optionally choose not to automatically renew the subscription.</span></span>

<span data-ttu-id="367e9-194">若要停止有效的商用 marketplace 訂用帳戶，使其無法自動續約：</span><span class="sxs-lookup"><span data-stu-id="367e9-194">To stop an active commercial marketplace subscription from automatically renewing:</span></span>

1. <span data-ttu-id="367e9-195">登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="367e9-195">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="367e9-196">從 [合作夥伴中心] 功能表上，選取 [客戶]  ，然後從清單中選擇客戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-196">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="367e9-197">選取 **訂用帳戶** 。</span><span class="sxs-lookup"><span data-stu-id="367e9-197">Select **Subscriptions**.</span></span> <span data-ttu-id="367e9-198">這會列出您已為客戶購買的任何授權型訂閱。</span><span class="sxs-lookup"><span data-stu-id="367e9-198">This lists any license-based subscriptions you have purchased for the customer.</span></span>

4. <span data-ttu-id="367e9-199">在 [**訂**用帳戶] 欄位中，選取您想要修改的訂用帳戶。</span><span class="sxs-lookup"><span data-stu-id="367e9-199">In the **Subscription** column, select the subscription you want to modify.</span></span>

5. <span data-ttu-id="367e9-200">在 [訂閱詳細資料] 頁面中，找出 [**狀態**] 區段，然後取消核取 [**自動續約**] 方塊。</span><span class="sxs-lookup"><span data-stu-id="367e9-200">In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box.</span></span>

6. <span data-ttu-id="367e9-201">選取 [提交]。</span><span class="sxs-lookup"><span data-stu-id="367e9-201">Select **Submit**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="367e9-202">後續步驟</span><span class="sxs-lookup"><span data-stu-id="367e9-202">Next steps</span></span>

- [<span data-ttu-id="367e9-203">為您的客戶購買商業市集產品</span><span class="sxs-lookup"><span data-stu-id="367e9-203">Purchase commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-purchase.md)

- [<span data-ttu-id="367e9-204">為您的客戶管理商業 marketplace 產品</span><span class="sxs-lookup"><span data-stu-id="367e9-204">Manage commercial marketplace products for your customers</span></span>](csp-commercial-marketplace-manage.md)

- [<span data-ttu-id="367e9-205">商務 Marketplace 概觀</span><span class="sxs-lookup"><span data-stu-id="367e9-205">Commercial marketplace overview</span></span>](csp-commercial-marketplace-overview.md)
