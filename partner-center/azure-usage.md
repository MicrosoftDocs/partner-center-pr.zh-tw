---
title: 適用于保留使用量上限的 Microsoft Azure VM 大小 |合作夥伴中心
ms.topic: article
ms.date: 04/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何在為虛擬機器（VM）購買 Microsoft Azure 保留時，將其調整為您客戶的運算需求。
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, vm, 管理, 使用率, 調整大小
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 05a041ae794270430b6e2ed7b72ff48b04018601
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453275"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="fed03-104">調整 Microsoft Azure VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="fed03-104">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="fed03-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="fed03-105">**Applies to**</span></span>

- <span data-ttu-id="fed03-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="fed03-106">Partner Center</span></span>
- <span data-ttu-id="fed03-107">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="fed03-107">Azure portal</span></span>
- <span data-ttu-id="fed03-108">雲端解決方案提供者中的合作夥伴</span><span class="sxs-lookup"><span data-stu-id="fed03-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="fed03-109">判斷客戶的 Azure 保留專案的 VM 大小</span><span class="sxs-lookup"><span data-stu-id="fed03-109">Determine the VM size for a customer's Azure reservation</span></span> 

<span data-ttu-id="fed03-110">代表您的客戶購買 Microsoft Azure 保留時，您必須選擇虛擬機器（VM）大小，以符合客戶的運算需求。</span><span class="sxs-lookup"><span data-stu-id="fed03-110">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="fed03-111">您可以使用下列其中一個方法來找到此項資訊：</span><span class="sxs-lookup"><span data-stu-id="fed03-111">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="fed03-112">Azure 使用量 API</span><span class="sxs-lookup"><span data-stu-id="fed03-112">Azure utilization API</span></span>
- <span data-ttu-id="fed03-113">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="fed03-113">The Azure portal</span></span>
- <span data-ttu-id="fed03-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="fed03-114">Azure PowerShell</span></span>
- <span data-ttu-id="fed03-115">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="fed03-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="fed03-116">以下列出使用每種方法的指示。</span><span class="sxs-lookup"><span data-stu-id="fed03-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="fed03-117">購買保留區之後，保留區折扣會自動套用到符合保留區屬性和數量的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="fed03-118">您不需要將保留指派給 VM。</span><span class="sxs-lookup"><span data-stu-id="fed03-118">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="fed03-119">保留折扣不適用於傳統或促銷 Vm。</span><span class="sxs-lookup"><span data-stu-id="fed03-119">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="fed03-120">若要正確找出代表您客戶購買的 VM 大小和類型，您必須使用以下所述的其中一種方法，因為合作夥伴中心對帳檔案不會正確顯示 VM 系列類型。</span><span class="sxs-lookup"><span data-stu-id="fed03-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

<span data-ttu-id="fed03-121">**使用 Azure 使用量 API，取得 VM 大小調整資訊**</span><span class="sxs-lookup"><span data-stu-id="fed03-121">**Get VM sizing information using the Azure utilization API**</span></span>

1. <span data-ttu-id="fed03-122">使用 API 回應中 additionalInfo 的 ServiceType 屬性值，找出要購買的 VM 大小。</span><span class="sxs-lookup"><span data-stu-id="fed03-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>
2. <span data-ttu-id="fed03-123">如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/)中的[取得 Azure 的客戶使用量記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="fed03-123">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

<span data-ttu-id="fed03-124">**使用 Microsoft Azure 入口網站，取得 VM 大小調整資訊**</span><span class="sxs-lookup"><span data-stu-id="fed03-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1. <span data-ttu-id="fed03-125">在合作夥伴中心，移至您的 [**客戶**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="fed03-125">In Partner Center, go to your **Customers** page.</span></span>
2. <span data-ttu-id="fed03-126">尋找想要購買 Azure VM 保留的客戶，然後選取向下箭號以展開客戶的資訊。</span><span class="sxs-lookup"><span data-stu-id="fed03-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="fed03-127">選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="fed03-127">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="fed03-128">從入口網站功能表選取 **\[虛擬機器\]**，然後選取您要購買保留區的 VM。</span><span class="sxs-lookup"><span data-stu-id="fed03-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>
4. <span data-ttu-id="fed03-129">在 VM 的詳細資料頁面上，尋找大小和區域資訊（如下所示），並使用此資訊在合作夥伴中心購買保留。</span><span class="sxs-lookup"><span data-stu-id="fed03-129">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    :::image type="content" source="images/usage1.png" alt-text="詳細資料頁面上的大小和區域資訊":::

<span data-ttu-id="fed03-131">**使用 Microsoft Azure PowerShell 取得 VM 大小調整資訊**</span><span class="sxs-lookup"><span data-stu-id="fed03-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="fed03-132">使用下列影像中的資訊，取得您要購買保留區的 VM 大小與位置。</span><span class="sxs-lookup"><span data-stu-id="fed03-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 位置和大小":::

<span data-ttu-id="fed03-134">**使用 Azure Resource Manager (ARM) API 取得 VM 大小調整資訊**</span><span class="sxs-lookup"><span data-stu-id="fed03-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1. <span data-ttu-id="fed03-135">使用 ARMClient 或 ARM API，呼叫您要購買保留區之 VM 的 ARM 用戶端。</span><span class="sxs-lookup"><span data-stu-id="fed03-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="fed03-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="fed03-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="fed03-137">呼叫會傳回 **vmSize** 和 **location** 的值，如下所示。</span><span class="sxs-lookup"><span data-stu-id="fed03-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 值":::
    :::image type="content" source="images/usage4.png" alt-text="位置值":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="fed03-140">確認 Azure VM 使用率與保留區折扣</span><span class="sxs-lookup"><span data-stu-id="fed03-140">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="fed03-141">代表客戶購買 Azure 保留的 VM 實例之後，預先支付 VM 空間的折扣會自動套用至符合客戶保留之屬性和數量的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-141">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="fed03-142">您可以使用下列其中一種方法來驗證客戶的保留使用量，並查看要套用保留折扣的虛擬機器：</span><span class="sxs-lookup"><span data-stu-id="fed03-142">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="fed03-143">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="fed03-143">The Azure portal</span></span>
- <span data-ttu-id="fed03-144">Azure 使用量 API</span><span class="sxs-lookup"><span data-stu-id="fed03-144">Azure utilization API</span></span>

<span data-ttu-id="fed03-145">以下列出使用每種方法的指示。</span><span class="sxs-lookup"><span data-stu-id="fed03-145">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="fed03-146">只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-146">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="fed03-147">確認客戶在 Microsoft Azure 入口網站中的保留使用量</span><span class="sxs-lookup"><span data-stu-id="fed03-147">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="fed03-148">在合作夥伴中心，移至您的 [**客戶**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="fed03-148">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="fed03-149">尋找您要驗證其保留折扣和使用量的客戶，然後選取向下箭號以展開客戶的資訊。</span><span class="sxs-lookup"><span data-stu-id="fed03-149">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="fed03-150">選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="fed03-150">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="fed03-151">從入口網站功能表選取 **\[保留區\]**，然後選取您要查看其使用率的保留區。</span><span class="sxs-lookup"><span data-stu-id="fed03-151">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="fed03-152">在 [**總覽**] 頁面上，檢查保留的 [使用率] 圖形，其中會顯示已將多少保留套用至虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-152">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="fed03-153">使用率資料可能會延遲最多 8 小時。</span><span class="sxs-lookup"><span data-stu-id="fed03-153">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="fed03-154">a.</span><span class="sxs-lookup"><span data-stu-id="fed03-154">a.</span></span> <span data-ttu-id="fed03-155">如果保留的使用率是100%，表示您的客戶正在取得保留購買可提供的所有可能的節約。</span><span class="sxs-lookup"><span data-stu-id="fed03-155">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="fed03-156">b.</span><span class="sxs-lookup"><span data-stu-id="fed03-156">b.</span></span> <span data-ttu-id="fed03-157">如果保留的使用量為0%，則不會將折扣套用至任何虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-157">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="fed03-158">c.</span><span class="sxs-lookup"><span data-stu-id="fed03-158">c.</span></span> <span data-ttu-id="fed03-159">如果保留的使用量介於1% 到99% 之間，則會有未使用的權益。</span><span class="sxs-lookup"><span data-stu-id="fed03-159">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="fed03-160">若要避免這種情況，請在進行購買之前，先決定正確的 VM 大小以支援客戶的運算需求。</span><span class="sxs-lookup"><span data-stu-id="fed03-160">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="fed03-161">使用 Azure 使用率 API 驗證客戶的保留使用量</span><span class="sxs-lookup"><span data-stu-id="fed03-161">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="fed03-162">只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="fed03-162">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="fed03-163">您可以使用 Azure 使用量 API 取得保留區使用率資料，來確認客戶獲得保留區折扣，並查看折扣套用到那些 VM (虛擬機器)。</span><span class="sxs-lookup"><span data-stu-id="fed03-163">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="fed03-164">將範例 A 與範例 B 進行比較，以瞭解如何驗證客戶的保留使用量。</span><span class="sxs-lookup"><span data-stu-id="fed03-164">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="保留使用範例":::

- <span data-ttu-id="fed03-166">ReservationId 可識別用於套用折扣至 VM 的 Azure 保留區。</span><span class="sxs-lookup"><span data-stu-id="fed03-166">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="fed03-167">consumptionMeter 是已套用保留區折扣之 VM 的 MeterId。</span><span class="sxs-lookup"><span data-stu-id="fed03-167">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="fed03-168">由於已套用保留區折扣，所以 ReservationMeter 會顯示 $0 費用。</span><span class="sxs-lookup"><span data-stu-id="fed03-168">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="fed03-169">如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/)中的[取得 Azure 的客戶使用量記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="fed03-169">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="fed03-170">軟體成本 (例如 Microsoft Windows Server) 目前不包含在 VM 保留區的價格中，並會在訂單記錄和發票中顯示為不同的一行項目。</span><span class="sxs-lookup"><span data-stu-id="fed03-170">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="fed03-171">不過，如果客戶擁有 Azure Hybrid Use Benefit，將不會套用軟體成本。</span><span class="sxs-lookup"><span data-stu-id="fed03-171">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="fed03-172">如需詳細資訊，請參閱 [Windows 軟體的成本不包括在保留執行個體內](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。</span><span class="sxs-lookup"><span data-stu-id="fed03-172">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="fed03-173">Azure Reservations 資源</span><span class="sxs-lookup"><span data-stu-id="fed03-173">Azure reservations resources</span></span>

|<span data-ttu-id="fed03-174">**如需下列資訊**</span><span class="sxs-lookup"><span data-stu-id="fed03-174">**For information about**</span></span>   |<span data-ttu-id="fed03-175">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="fed03-175">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="fed03-176">雲端解決方案提供者中的 Azure Reservations 概觀</span><span class="sxs-lookup"><span data-stu-id="fed03-176">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="fed03-177">銷售 Microsoft Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="fed03-177">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="fed03-178">在合作夥伴中心為您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="fed03-178">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="fed03-179">購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="fed03-179">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="fed03-180">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="fed03-180">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="fed03-181">在合作夥伴中心管理 Azure 保留專案</span><span class="sxs-lookup"><span data-stu-id="fed03-181">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="fed03-182">在 Azure 入口網站中購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="fed03-182">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="fed03-183">Azure 說明中的[預付具有 Azure 保留的 VM 執行個體的虛擬機器](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="fed03-183">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="fed03-184">在 Azure 入口網站中管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="fed03-184">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="fed03-185">Azure 說明中的[管理保留的 VM 執行個體](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="fed03-185">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="fed03-186">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="fed03-186">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="fed03-187">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="fed03-187">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="fed03-188">提供客戶從您購買的訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="fed03-188">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="fed03-189">授與客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="fed03-189">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
