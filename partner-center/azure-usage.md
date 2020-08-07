---
title: 調整 Azure VM 大小以提供最大保留區使用率
ms.topic: how-to
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 瞭解如何在您購買 Microsoft Azure 保留時，將虛擬機器 (VM) 大小調整為客戶的計算需求。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: bc9fc14598e7c96f9cc1b55eba7c59af68ad84a9
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900112"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>調整 Microsoft Azure VM 大小以提供最大保留區使用率

**適用於**

- 合作夥伴中心
- Azure 入口網站
- 雲端解決方案提供者方案中的合作夥伴
 
> [!NOTE]
> 本文僅適用于雲端解決方案提供者 (CSP) 方案中的合作夥伴。 使用其他類型之訂用帳戶的客戶 (例如，隨用隨付、個人、Microsoft 客戶合約或 Enterprise 合約訂用帳戶) 應改為閱讀[此 Azure 保留檔](https://docs.microsoft.com/azure/cost-management-billing/reservations)。

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>判斷客戶的 Azure 保留專案的 VM 大小

代表您的客戶購買 Microsoft Azure 保留時，您必須選擇虛擬機器 (VM) 大小，以符合客戶的運算需求。 您可以使用下列其中一個方法來找到此項資訊：

- Azure 使用量 API
- Azure 入口網站
- Azure PowerShell
- Azure Resource Manager (ARM) API

以下列出使用每種方法的指示。 購買保留區之後，保留區折扣會自動套用到符合保留區屬性和數量的虛擬機器。 您不需要將保留指派給 VM。

>[!NOTE]
>保留折扣不適用於傳統或促銷 Vm。

>[!IMPORTANT]
>若要正確找出代表您客戶購買的 VM 大小和類型，您必須使用以下所述的其中一種方法，因為合作夥伴中心對帳檔案不會正確顯示 VM 系列類型。

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>使用 Azure 使用量 API，取得 VM 大小調整資訊

1. 使用 API 回應中 additionalInfo 的 ServiceType 屬性值，找出要購買的 VM 大小。

2. 如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/)中的[取得 Azure 的客戶使用量記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>使用 Microsoft Azure 入口網站，取得 VM 大小調整資訊

1. 在合作夥伴中心，移至您的 [**客戶**] 頁面。

2. 尋找想要購買 Azure VM 保留的客戶，然後選取向下箭號以展開客戶的資訊。 選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。

3. 從入口網站功能表選取 **\[虛擬機器\]**，然後選取您要購買保留區的 VM。

4. 在 VM 的詳細資料頁面上，尋找大小和區域資訊（如下所示），並使用此資訊在合作夥伴中心購買保留。  

   :::image type="content" source="images/usage1.png" alt-text="詳細資料頁面上的大小和區域資訊":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>使用 Microsoft Azure PowerShell 取得 VM 大小調整資訊

使用下列影像中的資訊，取得您要購買保留區的 VM 大小與位置。 

:::image type="content" source="images/usage2.png" alt-text="VM 位置和大小":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>使用 Azure Resource Manager (ARM) API 取得 VM 大小調整資訊

1. 使用 ARMClient 或 ARM API，呼叫您要購買保留區之 VM 的 ARM 用戶端。

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. 呼叫會傳回 **vmSize** 和 **location** 的值，如下所示。

    :::image type="content" source="images/usage3.png" alt-text="vmSize 值":::
    :::image type="content" source="images/usage4.png" alt-text="位置值":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>確認 Azure VM 使用率與保留區折扣

代表客戶購買 Azure 保留的 VM 實例之後，預先支付 VM 空間的折扣會自動套用至符合客戶保留之屬性和數量的虛擬機器。

您可以使用下列其中一種方法來驗證客戶的保留使用量，並查看要套用保留折扣的虛擬機器：

- Azure 入口網站
- Azure 使用量 API

以下列出使用每種方法的指示。

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>確認客戶在 Microsoft Azure 入口網站中的保留使用量

1. 在合作夥伴中心，移至您的 [**客戶**] 頁面。

2. 尋找您要驗證其保留折扣和使用量的客戶，然後選取向下箭號以展開客戶的資訊。 選取 [ **Microsoft Azure 管理入口網站**] 以在 Azure 入口網站中開啟客戶的記錄。
3. 從入口網站功能表選取 **\[保留區\]**，然後選取您要查看其使用率的保留區。
4. 在 [**總覽**] 頁面上，檢查保留的 [使用率] 圖形，其中會顯示已將多少保留套用至虛擬機器。

    >[!NOTE]
    >使用率資料可能會延遲最多 8 小時。

    a. 如果保留的使用率是100%，表示您的客戶正在取得保留購買可提供的所有可能的節約。
    b. 如果保留的使用量為0%，則不會將折扣套用至任何虛擬機器。
    c. 如果保留的使用量介於1% 到99% 之間，則會有未使用的權益。

5. 若要避免這種情況，請在進行購買之前，先決定正確的 VM 大小以支援客戶的運算需求。

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>使用 Azure 使用率 API 驗證客戶的保留使用量

>[!NOTE]
>只有 Azure 使用量 API 會顯示折扣套用的虛擬機器。  

您可以使用 Azure 使用量 API 取得保留區使用率資料，來確認客戶獲得保留區折扣，並查看折扣套用到那些 VM (虛擬機器)。 將範例 A 與範例 B 進行比較，以瞭解如何驗證客戶的保留使用量。

:::image type="content" source="images/usage5.png" alt-text="保留使用範例":::

- ReservationId 可識別用於套用折扣至 VM 的 Azure 保留區。
- consumptionMeter 是已套用保留區折扣之 VM 的 MeterId。
- 由於已套用保留區折扣，所以 ReservationMeter 會顯示 $0 費用。

如需詳細資訊，請參閱[合作夥伴中心 API](https://docs.microsoft.com/partner-center/develop/)中的[取得 Azure 的客戶使用量記錄](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure)。

>[!IMPORTANT]
>軟體成本 (例如 Microsoft Windows Server) 目前不包含在 VM 保留區的價格中，並會在訂單記錄和發票中顯示為不同的一行項目。 不過，如果客戶擁有 Azure Hybrid Use Benefit，將不會套用軟體成本。 如需詳細資訊，請參閱 [Windows 軟體的成本不包括在保留執行個體內](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs)。  

## <a name="azure-reservations-resources"></a>Azure Reservations 資源

|**如需下列資訊**   |**請閱讀本文**    |
|:-----------------------------|:-----------------|
|雲端解決方案提供者中的 Azure Reservations 概觀  | [銷售 Microsoft Azure 保留的 VM 執行個體](azure-reservations.md)
|在合作夥伴中心為您的客戶購買 Azure 保留   | [購買 Azure Reservations](azure-reservations-buying.md)
|在合作夥伴中心管理 Azure 保留專案 | [在合作夥伴中心管理 Azure 保留專案](azure-reservations-manage.md)
|在 Azure 入口網站中購買 Azure Reservations | Azure 說明中的[預付具有 Azure 保留的 VM 執行個體的虛擬機器](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) |
|在 Azure 入口網站中管理 Azure Reservations   | Azure 說明中的[管理保留的 VM 執行個體](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance)  |
|使用合作夥伴中心 API 購買 Azure Reservations | 合作夥伴中心開發人員文件中的[購買 Azure 保留的 VM 執行個體](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations)   |
|提供客戶從您購買的訂用帳戶購買自己的 Azure 保留的許可權。 | [授與客戶購買自己的 Azure 保留的許可權](give-customers-permission.md)   |
