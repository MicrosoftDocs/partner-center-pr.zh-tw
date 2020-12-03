---
title: 調整 Azure VM 大小以提供最大保留區使用率
description: 瞭解如何將虛擬機器 (VM 的大小調整為您為客戶購買 Microsoft Azure 保留時的計算需求) 。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534942"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="006bb-103">調整 Microsoft Azure VM 大小以提供最大保留區使用率</span><span class="sxs-lookup"><span data-stu-id="006bb-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="006bb-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="006bb-104">**Appropriate roles**</span></span>

- <span data-ttu-id="006bb-105">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="006bb-105">Admin agent</span></span>
- <span data-ttu-id="006bb-106">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="006bb-106">Sales agent</span></span>

<span data-ttu-id="006bb-107">本文說明如何將虛擬機器 (VM) 的大小調整為您為客戶購買 Microsoft Azure 保留時的計算需求。</span><span class="sxs-lookup"><span data-stu-id="006bb-107">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="006bb-108">本文僅適用于雲端解決方案提供者 (CSP) 計畫中的合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="006bb-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="006bb-109">使用其他類型訂用帳戶的客戶 (例如隨用隨付、個別、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀 [此 Azure 保留檔](/azure/cost-management-billing/reservations)。</span><span class="sxs-lookup"><span data-stu-id="006bb-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="006bb-110">判斷客戶的 Azure 保留的 VM 大小</span><span class="sxs-lookup"><span data-stu-id="006bb-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="006bb-111">代表客戶購買 Microsoft Azure 的保留時，您必須選擇 (VM 的虛擬機器) 調整大小，以符合客戶的計算需求。</span><span class="sxs-lookup"><span data-stu-id="006bb-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="006bb-112">您可以使用下列其中一個方法來找到此項資訊：</span><span class="sxs-lookup"><span data-stu-id="006bb-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="006bb-113">Azure 使用量 API</span><span class="sxs-lookup"><span data-stu-id="006bb-113">Azure utilization API</span></span>
- <span data-ttu-id="006bb-114">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="006bb-114">The Azure portal</span></span>
- <span data-ttu-id="006bb-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="006bb-115">Azure PowerShell</span></span>
- <span data-ttu-id="006bb-116">Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="006bb-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="006bb-117">以下列出使用每種方法的指示。</span><span class="sxs-lookup"><span data-stu-id="006bb-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="006bb-118">購買保留區之後，保留區折扣會自動套用到符合保留區屬性和數量的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="006bb-119">您不需要將保留指派給 VM。</span><span class="sxs-lookup"><span data-stu-id="006bb-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="006bb-120">保留折扣不適用於傳統或促銷 Vm。</span><span class="sxs-lookup"><span data-stu-id="006bb-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="006bb-121">若要正確找出代表您客戶購買的 VM 大小和類型，您必須使用以下所述的其中一種方法，因為合作夥伴中心對帳檔案不會正確顯示 VM 系列類型。</span><span class="sxs-lookup"><span data-stu-id="006bb-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="006bb-122">使用 Azure 使用量 API，取得 VM 大小調整資訊</span><span class="sxs-lookup"><span data-stu-id="006bb-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="006bb-123">使用 API 回應中 additionalInfo 的 ServiceType 屬性值，找出要購買的 VM 大小。</span><span class="sxs-lookup"><span data-stu-id="006bb-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="006bb-124">如需詳細資訊，請參閱在[合作夥伴中心 API](/partner-center/develop/)[取得客戶的 Azure 使用量記錄](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="006bb-124">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="006bb-125">使用 Microsoft Azure 入口網站，取得 VM 大小調整資訊</span><span class="sxs-lookup"><span data-stu-id="006bb-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="006bb-126">在合作夥伴中心中，移至 [ **客戶** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="006bb-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="006bb-127">尋找想要購買 Azure VM 保留的客戶，然後選取向下箭號來展開客戶的資訊。</span><span class="sxs-lookup"><span data-stu-id="006bb-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="006bb-128">選取 **Microsoft Azure 管理入口網站** ，在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="006bb-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="006bb-129">從入口網站功能表選取 **\[虛擬機器\]**，然後選取您要購買保留區的 VM。</span><span class="sxs-lookup"><span data-stu-id="006bb-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="006bb-130">在 VM 的詳細資料頁面上，找到大小和區域資訊（如下所示），並使用此資訊來購買合作夥伴中心中的保留。</span><span class="sxs-lookup"><span data-stu-id="006bb-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="詳細資料頁面上的大小和區域資訊":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="006bb-132">使用 Microsoft Azure PowerShell 取得 VM 大小調整資訊</span><span class="sxs-lookup"><span data-stu-id="006bb-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="006bb-133">使用下列影像中的資訊，取得您要購買保留區的 VM 大小與位置。</span><span class="sxs-lookup"><span data-stu-id="006bb-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="VM 位置和大小":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="006bb-135">使用 Azure Resource Manager (ARM) API 取得 VM 大小調整資訊</span><span class="sxs-lookup"><span data-stu-id="006bb-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="006bb-136">使用 ARMClient 或 ARM API，呼叫您要購買保留區之 VM 的 ARM 用戶端。</span><span class="sxs-lookup"><span data-stu-id="006bb-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="006bb-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="006bb-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="006bb-138">呼叫會傳回 **vmSize** 和 **location** 的值，如下所示。</span><span class="sxs-lookup"><span data-stu-id="006bb-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="vmSize 值":::
    :::image type="content" source="images/usage4.png" alt-text="位置值":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="006bb-141">確認 Azure VM 使用率與保留區折扣</span><span class="sxs-lookup"><span data-stu-id="006bb-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="006bb-142">代表客戶購買 Azure 保留的 VM 實例之後，預先支付 VM 空間的折扣會自動套用至符合客戶保留的屬性和數量的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="006bb-143">您可以使用下列其中一種方法來確認客戶的保留使用量，並查看要套用保留折扣的虛擬機器：</span><span class="sxs-lookup"><span data-stu-id="006bb-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="006bb-144">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="006bb-144">The Azure portal</span></span>
- <span data-ttu-id="006bb-145">Azure 使用量 API</span><span class="sxs-lookup"><span data-stu-id="006bb-145">Azure utilization API</span></span>

<span data-ttu-id="006bb-146">以下列出使用每種方法的指示。</span><span class="sxs-lookup"><span data-stu-id="006bb-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="006bb-147">只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="006bb-148">確認 Microsoft Azure 入口網站中客戶的保留使用量</span><span class="sxs-lookup"><span data-stu-id="006bb-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="006bb-149">在合作夥伴中心中，移至 [ **客戶** ] 頁面。</span><span class="sxs-lookup"><span data-stu-id="006bb-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="006bb-150">尋找您想要確認其保留折扣和使用量的客戶，然後選取向下箭號以展開客戶的資訊。</span><span class="sxs-lookup"><span data-stu-id="006bb-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="006bb-151">選取 **Microsoft Azure 管理入口網站** ，在 Azure 入口網站中開啟客戶的記錄。</span><span class="sxs-lookup"><span data-stu-id="006bb-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="006bb-152">從入口網站功能表選取 **\[保留區\]**，然後選取您要查看其使用率的保留區。</span><span class="sxs-lookup"><span data-stu-id="006bb-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="006bb-153">在 [ **總覽** ] 頁面上，檢查保留的使用率圖表，其中顯示多少保留已套用至虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="006bb-154">使用率資料可能會延遲最多 8 小時。</span><span class="sxs-lookup"><span data-stu-id="006bb-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="006bb-155">a.</span><span class="sxs-lookup"><span data-stu-id="006bb-155">a.</span></span> <span data-ttu-id="006bb-156">如果保留的使用率是100%，則客戶會取得保留購買所能提供的所有可能省下的費用。</span><span class="sxs-lookup"><span data-stu-id="006bb-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="006bb-157">b.</span><span class="sxs-lookup"><span data-stu-id="006bb-157">b.</span></span> <span data-ttu-id="006bb-158">如果保留的使用量為0%，則折扣不會套用至任何虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="006bb-159">c.</span><span class="sxs-lookup"><span data-stu-id="006bb-159">c.</span></span> <span data-ttu-id="006bb-160">如果保留的使用量介於1% 到99% 之間，則有未使用的權益。</span><span class="sxs-lookup"><span data-stu-id="006bb-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="006bb-161">若要避免這種情況，請先決定正確的 VM 大小，以支援客戶的計算需求，然後再進行購買。</span><span class="sxs-lookup"><span data-stu-id="006bb-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="006bb-162">使用 Azure 使用量 API 來確認客戶的保留使用量</span><span class="sxs-lookup"><span data-stu-id="006bb-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="006bb-163">只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。</span><span class="sxs-lookup"><span data-stu-id="006bb-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="006bb-164">您可以使用 Azure 使用量 API 取得保留區使用率資料，來確認客戶獲得保留區折扣，並查看折扣套用到那些 VM (虛擬機器)。</span><span class="sxs-lookup"><span data-stu-id="006bb-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="006bb-165">比較範例 A 與範例 B，以瞭解如何確認客戶的保留使用量。</span><span class="sxs-lookup"><span data-stu-id="006bb-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="保留使用範例":::

- <span data-ttu-id="006bb-167">ReservationId 可識別用於套用折扣至 VM 的 Azure 保留區。</span><span class="sxs-lookup"><span data-stu-id="006bb-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="006bb-168">consumptionMeter 是已套用保留區折扣之 VM 的 MeterId。</span><span class="sxs-lookup"><span data-stu-id="006bb-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="006bb-169">由於已套用保留區折扣，所以 ReservationMeter 會顯示 $0 費用。</span><span class="sxs-lookup"><span data-stu-id="006bb-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="006bb-170">如需詳細資訊，請參閱在[合作夥伴中心 API](/partner-center/develop/)[取得客戶的 Azure 使用量記錄](/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。</span><span class="sxs-lookup"><span data-stu-id="006bb-170">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="006bb-171">軟體成本 (例如 Microsoft Windows Server) 目前不包含在 VM 保留區的價格中，並會在訂單記錄和發票中顯示為不同的一行項目。</span><span class="sxs-lookup"><span data-stu-id="006bb-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="006bb-172">不過，如果客戶擁有 Azure Hybrid Use Benefit，將不會套用軟體成本。</span><span class="sxs-lookup"><span data-stu-id="006bb-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="006bb-173">如需詳細資訊，請參閱 [Windows 軟體的成本不包括在保留執行個體內](/azure/billing/billing-reserved-instance-windows-software-costs)。</span><span class="sxs-lookup"><span data-stu-id="006bb-173">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="006bb-174">後續步驟</span><span class="sxs-lookup"><span data-stu-id="006bb-174">Next steps</span></span>

|<span data-ttu-id="006bb-175">**如需下列資訊**</span><span class="sxs-lookup"><span data-stu-id="006bb-175">**For information about**</span></span>   |<span data-ttu-id="006bb-176">**請閱讀本文**</span><span class="sxs-lookup"><span data-stu-id="006bb-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="006bb-177">雲端解決方案提供者中的 Azure Reservations 概觀</span><span class="sxs-lookup"><span data-stu-id="006bb-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="006bb-178">銷售 Microsoft Azure 保留的 VM 執行個體</span><span class="sxs-lookup"><span data-stu-id="006bb-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="006bb-179">在合作夥伴中心中為您的客戶購買 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="006bb-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="006bb-180">購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="006bb-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="006bb-181">在合作夥伴中心中管理 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="006bb-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="006bb-182">在合作夥伴中心中管理 Azure 保留</span><span class="sxs-lookup"><span data-stu-id="006bb-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="006bb-183">在 Azure 入口網站中購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="006bb-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="006bb-184">Azure 說明中的[預付具有 Azure 保留的 VM 執行個體的虛擬機器](/azure/virtual-machines/windows/prepay-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="006bb-184">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="006bb-185">在 Azure 入口網站中管理 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="006bb-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="006bb-186">Azure 說明中的[管理保留的 VM 執行個體](/azure/billing/billing-manage-reserved-vm-instance)</span><span class="sxs-lookup"><span data-stu-id="006bb-186">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="006bb-187">使用合作夥伴中心 API 購買 Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="006bb-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="006bb-188">合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](/partner-center/develop/purchase-azure-reservations)</span><span class="sxs-lookup"><span data-stu-id="006bb-188">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="006bb-189">提供客戶從您購買的訂用帳戶購買自己的 Azure 保留的許可權。</span><span class="sxs-lookup"><span data-stu-id="006bb-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="006bb-190">提供客戶購買自己的 Azure 保留的許可權</span><span class="sxs-lookup"><span data-stu-id="006bb-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |