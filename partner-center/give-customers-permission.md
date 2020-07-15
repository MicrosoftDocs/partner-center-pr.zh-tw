---
title: 讓客戶在 CSP 中購買自己的服務
description: 瞭解 CSP 方案合作夥伴如何讓客戶針對在合作夥伴中心購買的訂用帳戶購買自己的服務（例如 Azure 保留）。
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
Keywords: 訂用帳戶，自助式購買，自助 RI，啟用 RI，停用 RI，自助，客戶購買，客戶許可權，客戶購買保留實例，客戶購買 Azure 保留，開啟自助服務，關閉自助服務
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62447e284ce35b414594031c590110cedc5a59ab
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377452"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>授與客戶合作夥伴中心的許可權，以購買自己的產品或服務

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 系統管理代理人
- 銷售代理人

本文說明雲端解決方案提供者（CSP）方案中的合作夥伴如何提供客戶購買部分自己的服務或資源的許可權。

CSP 方案中的合作夥伴通常會使用合作夥伴中心和其商業 marketplace，為客戶購買解決方案和服務。 然後，合作夥伴可以讓某些客戶直接從 Azure 入口網站布建這些服務。

以下為範例。 假設您在合作夥伴中心購買客戶的 Azure 方案訂用帳戶。 接著，您決定將其他資源或服務新增至該訂用帳戶（代表客戶）。 在此情況下，您可以將 Azure 保留專案新增至客戶的訂用帳戶（例如，新增保留的虛擬機器實例）。 接著，您可以允許客戶進一步在 Azure 入口網站中布建 Azure 保留資源本身。

現在，透過**客戶**權力功能，您可以使用 Azure 資源為客戶提供更多的自助選項。 藉由開啟客戶的許可權，您可以讓客戶購買自己的資源（例如購買自己的 Azure 保留）。  

## <a name="overview-of-customer-permissions-in-partner-center"></a>合作夥伴中心的客戶許可權總覽

使用 [客戶**帳戶**] 頁面，即可開啟（或關閉）客戶的許可權。 目前，這項功能支援：

- **Azure 保留：** 開啟此許可權可讓客戶為您購買的特定 Azure 訂用帳戶購買自己的 Azure 保留專案。

在您開啟客戶許可權之前，請注意下列重點：

- 根據預設，合作夥伴中心內的客戶許可權會自動停用（關閉）。

- 您必須先將 [合作夥伴中心] 中的 [系統管理員] 角色指派給您，才可以開啟或關閉客戶的許可權。

  獲派「銷售代理程式」或「服務台」代理程式角色具有唯讀存取權，且無法開啟或關閉客戶許可權的夥伴。

- 您可以為您選擇的任何客戶開啟（啟用）許可權。

- 您可以使用合作夥伴中心儀表板或[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/manage-customers)來開啟（或關閉）客戶的許可權。

- 在您開啟（啟用）特定客戶的許可權之後，您會負責支付該客戶所做的任何後續購買。 若客戶想要交換、取消或續訂已進行的購買（或他們想要變更保留的初始範圍），他們將無法自行執行。 他們需要以合作夥伴的身分詢問您，以協助他們交換、取消和續約購買，或對保留範圍進行變更。  

- 開啟特定客戶的許可權之後，您將**不會**收到任何稍後的客戶購買通知。

- 客戶日後購買的內容將會顯示在合作夥伴中心，以及您所做的任何購買。 您可以在客戶的 [**訂單歷程記錄**] 頁面、[**保留**] 頁面或 [[**活動記錄**](activity-logs.md)] 中找到這些購買專案。

>[!NOTE]
> 如需客戶將支付的價格，以及如何協助客戶管理其購買的相關資訊，請參閱[協助客戶管理他們所購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>授與客戶購買自己的 Azure 保留的許可權

Azure 保留是以折扣價購買 Azure 服務的絕佳方式。 若要深入瞭解 Azure 保留的優點，請參閱[什麼是 Azure 保留專案？](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

現在您可以選擇代表您的客戶購買 Azure 保留，因為您可能已經完成。 或者，您可以授與客戶購買自己的 Azure 保留區的許可權。

>[!NOTE]
> 在您授與客戶購買自己的 Azure 保留的許可權之後，請協助他們管理所購買的任何保留。 如需詳細資訊，請參閱[協助客戶管理他們所購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>讓客戶購買自己的 Azure 保留專案

1. 確認客戶已有您購買的現有 Azure 方案或 Azure 全域訂用帳戶。

2. 確認客戶已獲指派此訂用帳戶的**擁有**者角色。

3. 啟用客戶權力 **（開啟此功能）** 來購買自己的 Azure 保留。

每個步驟如下所示。

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>確認客戶有現有的 Azure 訂用帳戶

在您授與客戶購買自己的 Azure 保留專案的許可權之前，您必須確認客戶有現有的 Azure 方案或 Azure 全域訂用帳戶。 如果客戶在合作夥伴中心沒有顯示目前的 Azure 訂用帳戶，您必須先為他們購買訂用帳戶，然後再開啟其客戶許可權。

- 若要查看客戶是否已有 Azure 訂用帳戶，請登入 [合作夥伴中心] 儀表板，然後選取 [ **CSP** ] 和 [**客戶**]。 從清單中選取特定的客戶。 **然後選取 [** 訂用帳戶]，然後尋找 azure 方案或 azure Global 的任何以使用量為基礎的訂用帳戶。

- 如果客戶沒有現有的 Azure 訂用帳戶，您可以為他們購買訂用帳戶。 請參閱[購買 Azure 方案](purchase-azure-plan.md)。

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>確認已在 Azure 中為客戶指派正確的角色

在您確認客戶擁有現有的 Azure 訂用帳戶之後，您也需要確認與您的客戶相關聯的金鑰使用者已獲指派該 Azure 訂用帳戶的正確**擁有**者角色。 這是客戶需要為您購買的 Azure 訂用帳戶購買 Azure 保留的角色型存取（RBAC）。

某些合作夥伴可能已將「**擁有**者」角色指派給想要主動管理和布建自己的 Azure 資源的客戶。 如果您已將 [**擁有**者] 狀態指派給客戶，以管理您為其購買的先前訂用帳戶，則可以略過此步驟。  

> [!IMPORTANT]
> 如果尚未將「**擁有**者」角色指派給客戶，他們會在 Azure 入口網站中收到錯誤，使其無法購買 Azure 保留。

若要確認客戶已獲指派 Azure 訂用帳戶的**擁有**者角色：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 依序選取 [ **CSP**] 和 [**客戶**]，然後選取特定的客戶。

3. 選取**該客戶的 [** 訂用帳戶]，並找出特定的 Azure 訂用帳戶。

4. 選取該客戶訂用帳戶旁的 [**管理**] 按鈕。 這麼做會開啟[Azure 入口網站](https://portal.azure.com/)。

5. 若要將**擁有**者角色指派給特定使用者，請遵循下列步驟，[將使用者指派為系統管理員](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>開啟或關閉客戶的許可權以購買自己的 Azure 保留專案

在您確認客戶具有現有的 Azure 訂用帳戶，而且已將該訂用帳戶的**擁有**者角色指派給使用者之後，您就可以開啟（啟用）客戶的許可權。 您也可以使用這些步驟來關閉（停用）客戶的許可權。 您可以使用合作夥伴中心儀表板或[合作夥伴中心 api](https://docs.microsoft.com/partner-center/develop/manage-customers)來啟用或停用客戶許可權。

若要在合作夥伴中心開啟（或關閉）客戶的許可權：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從左側導覽功能表中，依序選取 [ **CSP**] 和 [**客戶**]。 客戶清單隨即出現。

3. 選取特定的客戶名稱。

4. 從 [客戶] 功能表中選取 [**帳戶**]。 [客戶**帳戶**] 頁面隨即出現。

5. 找出頁面底部的 [**客戶許可權**] 區域。

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="客戶在帳戶頁面上的許可權。" border="true":::

6. 在 [ **Azure 保留**] 底下，找出 [**允許客戶購買**] 選項。

7. 若要開啟客戶許可權，請將此選項旁邊的切換開關移至 [**開啟**] 位置。 若要關閉客戶權力，請將切換開關移至 [**關閉**] 位置。

>[!NOTE]
> 若要瞭解當您開啟客戶的許可權來購買自己的 Azure 保留時，會發生什麼事，請參閱[合作夥伴中心的客戶許可權總覽](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。
>
>當您開啟（或關閉）客戶許可權時，活動記錄會記錄每個動作。 （當您選取 [合作夥伴中心] 儀表板頂端的齒輪圖示時，就可以存取此記錄）。 當您開啟或關閉客戶權力時，此動作將會顯示為 [在活動記錄中**建立客戶購買許可權**或**刪除客戶購買許可權**]。

## <a name="help-customers-manage-reservations-they-purchase"></a>協助客戶管理他們所購買的保留

一旦授與客戶購買自己的 Azure 保留的許可權，您就可以協助他們更有效地管理他們所購買的任何資源。 客戶可以直接從[Azure 入口網站](https://portal.azure.com/)管理 Azure 保留專案的許多層面。 在您的 CSP 訂用帳戶中，他們將需要協助您管理 Azure 保留專案的一些其他層面。  

協助客戶深入瞭解如何管理 Azure 保留專案的下列各方面：

- 客戶將支付 Azure 保留費用
- 客戶可以如何將 Azure 保留專案優化
- 當客戶購買具有共用範圍的保留時，會發生什麼事？
- 若客戶想要變更、取消和更新保留，或變更其範圍，會發生什麼事？

**客戶會支付其保留費用。** 您的客戶將會根據您先前在 CSP 合作夥伴帳單帳戶中購買的訂用帳戶來購買 Azure 保留。 根據此訂用帳戶購買之任何 Azure 保留的客戶價格也會由您設定。 此價格可能與客戶在 Azure 入口網站中看到的 Web Direct 價格不同。

**客戶可以如何將保留的使用優化。** 某些客戶可能會受益于深入瞭解如何優化保留的使用方式，或如何在購買期間指派保留的初始範圍。 如需詳細資訊，請要求客戶閱讀[管理 Azure 資源的保留](https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。

**當客戶購買具有共用範圍的保留時，會發生什麼事？** 當客戶根據先前的 CSP 訂用帳戶購買保留區，並將共用範圍指派給該保留時，CSP 提供給客戶的任何折扣將會套用至 CSP 合作夥伴為該客戶購買之所有訂用帳戶的相符使用量。

**如果他們想要交換、取消或續訂已進行的購買，或變更保留的初始範圍，客戶該怎麼做？** 客戶必須要求合作夥伴協助他們變更保留的初始範圍。 他們也需要合作夥伴的協助，以交換、取消或更新保留。 他們無法根據 CSP 合作夥伴為其購買的訂閱，自行執行這些工作。

## <a name="next-steps"></a>後續步驟

- [代表您的客戶購買 Azure 保留專案](azure-reservations-buying.md)

- [合作夥伴中心-銷售 Microsoft 預約](azure-reservations.md)

- [代表您的客戶管理 Azure Reservations](azure-reservations-manage.md)
