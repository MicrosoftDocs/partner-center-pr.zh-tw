---
title: 讓客戶在 CSP 中購買自己的服務
description: 瞭解 CSP 方案合作夥伴如何讓客戶為在合作夥伴中心中購買的訂用帳戶購買自己的服務（例如 Azure 保留）。
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19f86ec5353abc21e14a3a8ac2ef17dd17924cfe
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000462"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>提供客戶合作夥伴中心的許可權，以購買自己的產品或服務

**適用於**

- 合作夥伴中心
- 雲端解決方案提供者方案中的合作夥伴

**適當的角色**

- 系統管理代理人
- 銷售代理人

本文說明雲端解決方案提供者 (CSP) 方案中的合作夥伴如何為客戶提供購買某些服務或資源的許可權。

CSP 方案中的合作夥伴通常會使用合作夥伴中心及其商業市場，為其客戶購買解決方案和服務。 合作夥伴接著會讓某些客戶直接從 Azure 入口網站自行布建這些服務。

以下為範例。 假設您在合作夥伴中心中為客戶購買 Azure 方案訂用帳戶。 然後，您決定將其他資源或服務代表客戶新增至該訂用帳戶。 在此情況下，您可以將 Azure 保留新增至客戶的訂用帳戶， (例如新增保留的虛擬機器實例) 。 然後，您可以讓客戶在 Azure 入口網站中進一步布建 Azure 保留資源。

現在，有了 **客戶許可權** 功能，您可以為客戶提供更多使用 Azure 資源的自助服務選項。 藉由開啟客戶的許可權，您可讓客戶購買自己的資源 (例如，購買自己的 Azure 保留) 。  

## <a name="overview-of-customer-permissions-in-partner-center"></a>合作夥伴中心中的客戶許可權總覽

您可以使用 [客戶 **帳戶** ] 頁面來開啟 (，或關閉) 的客戶許可權。 目前，這項功能支援：

- **Azure 保留：** 開啟此許可權可讓客戶針對您為其購買的特定 Azure 訂用帳戶購買自己的 Azure 保留。

在您開啟客戶許可權之前，請注意下列重點：

- 根據預設，客戶許可權會自動停用 (關閉合作夥伴中心中的) 。

- 您必須在合作夥伴中心中指派系統管理員代理程式角色，才能開啟 (或關閉客戶) 許可權。

  獲指派銷售專員或服務中心代理程式角色的夥伴擁有唯讀存取權，無法開啟或關閉客戶許可權。

- 您可以開啟 (針對您選擇的任何客戶啟用) 許可權。

- 您可以使用合作夥伴中心儀表板或 [合作夥伴中心 api](/partner-center/develop/manage-customers)來開啟 (或關閉) 的客戶許可權。

- 當您開啟 (啟用特定客戶的) 許可權之後，您將負責支付該客戶的任何後續購買款項。 如果客戶想要交換、取消或更新購買 (或想要變更保留) 的初始範圍，他們本身將無法執行此作業。 他們需要以合作夥伴的身份要求您，以協助他們交換、取消和續約購買專案，或在日後變更保留範圍。  

- 當您開啟特定客戶的許可權之後，系統將 **不會** 通知您任何稍後由客戶進行的購買。

- 客戶的後續購買將會隨您在合作夥伴中心中顯示。 您可以在客戶的 **訂單歷程記錄** 頁面、其 **保留** 頁面或 [**活動記錄**](activity-logs.md)中找到這些購買專案。

>[!NOTE]
> 如需客戶將支付的價格以及如何協助客戶管理其購買的相關資訊，請參閱 [協助客戶管理購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>提供客戶購買自己的 Azure 保留的許可權

Azure 保留是以折扣價購買 Azure 服務的絕佳方式。 若要深入瞭解 Azure 保留的優點，請參閱 [什麼是 Azure 保留專案？](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

現在您可以選擇代表客戶購買 Azure 保留，因為您可能已經完成。 或者，您可以授與客戶購買自己的 Azure 保留的許可權。

>[!NOTE]
> 在您授與客戶購買自己的 Azure 保留的許可權之後，請協助他們管理任何購買的保留。 如需詳細資訊，請參閱 [協助客戶管理購買的保留](give-customers-permission.md#help-customers-manage-reservations-they-purchase)。

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>讓客戶購買自己的 Azure 保留

1. 確認客戶有您購買的現有 Azure 方案或 Azure 全域訂用帳戶。

2. 確認客戶已獲指派此訂用帳戶的 **擁有** 者角色。

3. 啟用客戶許可權 (**在) 上** 開啟此功能，以購買自己的 Azure 保留。

每個步驟都會顯示在下方。

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>確認客戶擁有現有的 Azure 訂用帳戶

在您授與客戶購買自己的 Azure 保留的許可權之前，您必須確認客戶已有現有的 Azure 方案或 Azure 全域訂用帳戶。 如果客戶未在合作夥伴中心中顯示目前的 Azure 訂用帳戶，您必須先為他們購買訂用帳戶，才能開啟其客戶許可權。

- 若要查看客戶是否已有 Azure 訂用帳戶，請登入合作夥伴中心儀表板，然後選取 [ **CSP** ]，再選取 [ **客戶**]。 從清單中選取特定的客戶。 **然後選取訂**用帳戶，並尋找 azure 方案或 azure Global 的任何以使用量為基礎的訂用帳戶。

- 如果客戶沒有現有的 Azure 訂用帳戶，您可以為他們購買訂用帳戶。 請參閱 [購買 Azure 方案](purchase-azure-plan.md)。

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>確認已在 Azure 中將正確的角色指派給客戶

在您確認客戶擁有現有的 Azure 訂用帳戶之後，您也需要確認與客戶相關聯的金鑰使用者已獲指派該 Azure 訂用帳戶的正確 **擁有** 者角色。 這是以角色為基礎的存取 (RBAC) 客戶必須為您購買的 Azure 訂用帳戶購買 Azure 保留。

某些夥伴可能已將 **擁有** 者角色指派給想要主動管理及布建自己的 Azure 資源的客戶。 如果您已將 **擁有** 者狀態指派給客戶，以管理您為其購買的先前訂用帳戶，您可以略過此步驟。  

> [!IMPORTANT]
> 如果客戶未獲指派 **擁有** 者角色，他們將會在 Azure 入口網站中收到錯誤，使其無法購買 Azure 保留。

若要確認客戶已獲指派 Azure 訂用帳戶的 **擁有** 者角色：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 選取 [ **CSP**]，然後選取 [ **客戶** ]，然後選取特定的客戶。

3. 選取 **該客戶的訂** 用帳戶，並找出特定的 Azure 訂用帳戶。

4. 選取該客戶訂用帳戶旁邊的 [ **管理** ] 按鈕。 這麼做會開啟 [Azure 入口網站](https://portal.azure.com/)。

5. 若要將 **擁有** 者角色指派給特定使用者，請遵循下列步驟， [將使用者指派為系統管理員](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)。

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>開啟或關閉客戶許可權以購買自己的 Azure 保留

在您確認客戶擁有現有的 Azure 訂用帳戶，且已將該訂用帳戶的 **擁有** 者角色指派給使用者之後，您就可以開啟 (啟用) 的客戶許可權。 您也可以使用這些步驟關閉 (停用) 客戶許可權。 您可以使用合作夥伴中心儀表板或 [合作夥伴中心 api](/partner-center/develop/manage-customers)來啟用或停用客戶許可權。

若要開啟 (或關閉合作夥伴中心中的) 客戶許可權：

1. 登入合作夥伴中心[儀表板](https://partner.microsoft.com/dashboard)。

2. 從左側導覽功能表中，選取 [ **CSP**]，然後選取 [ **客戶**]。 客戶清單隨即出現。

3. 選取特定的客戶名稱。

4. 從 [客戶] 功能表中選取 [ **帳戶** ]。 [客戶 **帳戶** ] 頁面隨即出現。

5. 在頁面底部找出 [ **客戶許可權** ] 區域。

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="帳戶頁面上的客戶許可權。" border="true":::

6. 在 [ **Azure 保留**] 底下，找出 [ **允許客戶購買** ] 選項。

7. 若要開啟客戶許可權，請將此選項旁邊的開關移至 [ **開啟** ] 位置。 若要關閉客戶許可權，請將開關移至 [ **關閉** ] 位置。

>[!NOTE]
> 若要瞭解當您開啟客戶的許可權來購買自己的 Azure 保留時，會發生什麼情況，請參閱 [合作夥伴中心中的客戶許可權總覽](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)。
>
>當您開啟 (或關閉) 客戶許可權時，活動記錄會記錄每個動作。 當您選取合作夥伴中心儀表板) 頂端的齒輪圖示時， (可以存取此記錄檔。 當您開啟或關閉客戶許可權時，此動作會顯示為 [ **建立客戶購買許可權** ] 或 [ **刪除客戶購買許可權** ] 活動記錄。

## <a name="help-customers-manage-reservations-they-purchase"></a>協助客戶管理他們購買的保留

一旦您授與客戶購買自己的 Azure 保留的許可權，您可以協助他們更妥善地管理購買的任何資源。 客戶可以直接從 [Azure 入口網站](https://portal.azure.com/)管理 Azure 保留的許多層面。 在您的 CSP 訂用帳戶內購買 Azure 保留專案的其他部分時，他們將需要您的協助。  

協助客戶深入瞭解如何管理 Azure 保留的下列各方面：

- 客戶將支付 Azure 保留費用
- 客戶如何優化 Azure 保留的使用
- 當客戶購買具有共用範圍的保留時，會發生什麼事？
- 如果客戶想要變更、取消和更新保留，或變更其範圍，會發生什麼事？

**客戶的價格將支付其保留費用。** 您的客戶將會根據您先前在 CSP 合作夥伴計費帳戶中購買的訂用帳戶來購買 Azure 保留。 客戶根據此訂用帳戶購買之任何 Azure 保留的價格也是由您所設定。 此價格可能與客戶在 Azure 入口網站中看到的 Web Direct 價格不同。

**客戶可如何將保留的使用優化。** 某些客戶可能會受益于深入瞭解如何將保留的使用優化，或如何在購買期間指派保留的初始範圍。 如需詳細資訊，請要求客戶閱讀 [Azure 資源的管理保留](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)。

**當客戶購買具有共用範圍的保留時，會發生什麼事？** 當客戶購買以先前的 CSP 訂用帳戶為基礎的保留，並將共用範圍指派給該保留時，由 CSP 提供給該客戶的所有訂用帳戶折扣將會套用至 CSP 合作夥伴為該客戶購買之所有訂用帳戶的相符使用量。

**如果客戶想要交換、取消或續約他們所做的購買，或變更保留的初始範圍，該怎麼辦？** 客戶必須要求合作夥伴協助他們變更保留的初始範圍。 他們也需要合作夥伴的協助，以交換、取消或更新保留。 他們無法以 CSP 合作夥伴購買的訂用帳戶為基礎，執行這些工作本身的保留。

## <a name="next-steps"></a>下一步

- [代表您的客戶購買 Azure 保留](azure-reservations-buying.md)

- [合作夥伴中心-銷售 Microsoft 保留專案](azure-reservations.md)

- [代表您的客戶管理 Azure Reservations](azure-reservations-manage.md)