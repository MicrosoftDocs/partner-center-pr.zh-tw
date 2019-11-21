---
title: Microsoft Azure VM sizing for maximum reservation usage  | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.
author: LauraBrenner
ms.author: labrenne
keywords: azure, 保留區, vm, 管理, 使用率, 調整大小
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2b8148d66be8a439056efa41eccb60cbc3e4274b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253253"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>調整 Microsoft Azure VM 大小以提供最大保留區使用率

**適用於**

- 合作夥伴中心
- Azure 入口網站
- 雲端解決方案提供者中的合作夥伴

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determine the VM size for a customer's Azure reservation 

When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs. 您可以使用下列其中一個方法來找到此項資訊：

- Azure 使用量 API
- Azure 入口網站
- Azure PowerShell
- Azure Resource Manager (ARM) API

以下列出使用每種方法的指示。 購買保留區之後，保留區折扣會自動套用到符合保留區屬性和數量的虛擬機器。 You don't need to assign the reservation to a VM.

>[!NOTE]
>Reservation discounts don't apply to classic or promotional VMs.

>[!IMPORTANT]
>若要正確找出代表您客戶購買的 VM 大小和類型，您必須使用以下所述的其中一種方法，因為合作夥伴中心對帳檔案不會正確顯示 VM 系列類型。

**Get VM sizing information using the Azure utilization API**

1. 使用 API 回應中 additionalInfo 的 ServiceType 屬性值，找出要購買的 VM 大小。
2. For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

**Get VM sizing information using the Microsoft Azure portal**

1. In Partner Center, go to your **Customers** page.
2. Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 從入口網站功能表選取 **\[虛擬機器\]** ，然後選取您要購買保留區的 VM。
4. On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.  

    ![Size and region information on detail page](images/usage1.png)

**Get VM sizing information using Microsoft Azure PowerShell**

使用下列影像中的資訊，取得您要購買保留區的 VM 大小與位置。 

![VM location and size](images/usage2.png)

**Get VM sizing information using the Azure Resource Manager (ARM) API**

1. 使用 ARMClient 或 ARM API，呼叫您要購買保留區之 VM 的 ARM 用戶端。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 呼叫會傳回 **vmSize** 和 **location** 的值，如下所示。

    ![vmSize value](images/usage3.png) ![location value](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>確認 Azure VM 使用率與保留區折扣

After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.

You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:

- Azure 入口網站
- Azure 使用量 API

以下列出使用每種方法的指示。

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Verify the customer's reservation usage in the Microsoft Azure portal

1. In Partner Center, go to your **Customers** page.

2. Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information. Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.
3. 從入口網站功能表選取 **\[保留區\]** ，然後選取您要查看其使用率的保留區。
4. On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.

    >[!NOTE]
    >使用率資料可能會延遲最多 8 小時。

    a. If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.
    b。 If the reservation's usage is 0%, the discount is not being applied to any virtual machine.
    c. If the reservation's usage is between 1% and 99%, there are unused benefits.

5. To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Verify the customer's reservation usage with the Azure utilization API

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

您可以使用 Azure 使用量 API 取得保留區使用率資料，來確認客戶獲得保留區折扣，並查看折扣套用到那些 VM (虛擬機器)。 Compare Example A to Example B to see how to verify a customer's reservation usage.

![Reservation usage examples](images/usage5.png)

- ReservationId 可識別用於套用折扣至 VM 的 Azure 保留區。
- consumptionMeter 是已套用保留區折扣之 VM 的 MeterId。
- 由於已套用保留區折扣，所以 ReservationMeter 會顯示 $0 費用。

For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>軟體成本 (例如 Microsoft Windows Server) 目前不包含在 VM 保留區的價格中，並會在訂單記錄和發票中顯示為不同的一行項目。 不過，如果客戶擁有 Azure Hybrid Use Benefit，將不會套用軟體成本。 如需詳細資訊，請參閱 [Windows 軟體的成本不包括在保留執行個體內](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure Reservations 資源

|**For information about**   |**請閱讀本文**    |
|:-----------------------------|:-----------------|
|雲端解決方案提供者中的 Azure Reservations 概觀  | [Sell Microsoft Azure Reserved VM Instances](azure-reservations.md)
|Purchasing Azure reservations for your customers in Partner Center   |[Buy Azure reservations](azure-reservations-buying.md)
|Managing Azure reservations in Partner Center | [Managing Azure reservations in Partner Center](azure-reservations-manage.md)
|在 Azure 入口網站中購買 Azure Reservations | Azure 說明中的[預付具有 Azure 保留的 VM 執行個體的虛擬機器](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 入口網站中管理 Azure Reservations   |Azure 說明中的[管理保留的 VM 執行個體](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作夥伴中心 API 購買 Azure Reservations | 合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)
