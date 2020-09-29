---
title: 將 azure 訂用帳戶的 azure 訂用帳戶轉移給另一個 CSP 合作夥伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在 Azure 方案下變更與客戶的 Azure 訂用帳戶相關聯的雲端解決方案提供者方案合作夥伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e1b70f26dc146507ac3764ae223ca27915162f0c
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422552"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>將客戶的 Azure 方案訂用帳戶轉移至不同的合作夥伴

## <a name="applies-to"></a>適用於

- 雲端解決方案提供者 (CSP) 計畫中的合作夥伴

本文說明客戶如何將 Azure 方案下的 azure 訂用帳戶從一個雲端解決方案提供者 (CSP) 切換至另一個。

若要從不同的夥伴切換客戶的 Azure 訂用帳戶，請遵循下列步驟。 夥伴和客戶都有完成的步驟。

>[!Note]  
>只有與 Microsoft 具有直接計費關係的合作夥伴可以存取轉換工具。 間接轉銷商必須與間接提供者合作，以利用這種轉換工具。

客戶必須與這兩個夥伴交談 (目前和未來的) ，才能運用這項工具。 離線對話必須能夠避免混淆和流失。 此外，合作夥伴和客戶應該在起始轉換之前，先瞭解這些考慮和必要條件：

**重要考慮：**

- Azure 保留專案不會隨訂用帳戶移至未來合作夥伴
- 目前合作夥伴下的 Azure 服務 CSP 定價不會轉換  
- 客戶的支援責任將移至未來的合作夥伴
- 計費和發票開立將在傳輸時移至未來合作夥伴
- Azure 角色型存取控制 (RBAC) 不受傳輸影響
- 系統管理員代表 (AOBO) 預設不會授與未來合作夥伴
- 只要產品通過 Marketplace 資格檢查，就會傳輸協力廠商 marketplace 產品。
    - 沒有特殊的折扣或區域限制
    - 非訂用帳戶為基礎的產品
    - 未來的夥伴應與發行者合作，以確保他們位於產品部署的允許清單中
    - 如果未符合上述所有條件，則必須取消 Azure 訂用帳戶，然後再以新的合作夥伴重新購買 Marketplace 產品的傳送

**必要條件：**

- 客戶參與目前的 CSP 合作夥伴，以進行轉換
- 未來的 CSP 合作夥伴會與客戶合作，以確保符合客戶需求
- 未來的 CSP 合作夥伴會在轉換開始前與客戶建立關聯性  
- 客戶必須使用未來的 CSP 合作夥伴簽署 Microsoft 客戶合約
- 未來的 CSP 合作夥伴必須已簽署 Microsoft 合作夥伴合約才能使用此工具

## <a name="customer-tasks-to-be-completed"></a>要完成的客戶工作

若要轉移 azure 訂用帳戶下的 Azure 訂用帳戶，客戶必須聯絡其目前的合作夥伴來開始此程式。 他們應該收集其目前合作夥伴的公司名稱和網域，讓其未來的合作夥伴可以代表他們完成傳送申請表單。

客戶也必須識別他們想要從目前合作夥伴轉移的訂用帳戶。 您無法變更 Office 365、Enterprise 行動套件或 Microsoft Dynamics CRM 訂閱的合作夥伴。

>[!Note]  
>未來的合作夥伴必須負責完成傳送要求表單，以起始傳輸程式。 Microsoft 無法代表客戶或目前的夥伴介入。 客戶應該規劃與其未來和目前的合作夥伴密切合作，以順利進行轉換。

## <a name="future-partner-tasks-to-be-completed"></a>未來要完成的夥伴工作

訂用帳戶的未來夥伴需要從合作夥伴中心完成傳送要求表單，以要求訂用帳戶轉移：

1.  從 [合作夥伴中心] 功能表選取 [ **客戶**]，然後選取您想要代表的客戶完成傳送申請表單。
2.  從 [客戶] 功能表選取 [ **訂閱**]。
3.  選取 [ **轉移要求** ] 區段。
4.  從 [ **轉移要求] 區段**中，選取 [ **加入新要求**]。

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="傳輸區段":::

5.  完成 **新的傳送要求** 表單。

6.  選取 [傳送**轉移要求**  >  **傳送]**。

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="完成轉移要求表單":::

7.  檢查傳輸要求確認

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="審核暫止的傳輸":::

    >[!Note]
    >未來的夥伴只要在傳輸要求狀態為「擱置中」時，在右上角選取 [ **取消要求** ]，即可取消轉移要求。 當傳輸要求狀態為「進行中」或「完成」時，將無法取消。

## <a name="current-partner-tasks-to-be-completed"></a>目前要完成的夥伴工作

客戶目前的夥伴管理員代理程式會收到一封電子郵件，指出其客戶要求轉移其訂用帳戶：

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="檢閱":::

請檢查並接受合作夥伴中心的轉移要求表單，以完成訂用帳戶轉移。

>[!Note]  
>如果目前合作夥伴在30天內未採取任何動作，則要求將會過期，而未來的夥伴將會有一個來建立新的轉移要求。

1.  選取電子郵件中的 **審核轉移要求** 或
1.  從 [合作夥伴中心] 功能表中，選取 [ **Customers**]，然後選取代表已提交轉移要求的客戶。
2.  從 [客戶] 功能表選取 [ **訂閱**]。
3.  選取 [ **轉移要求** ] 區段。
4.  在 [**收到的要求**] 底下選取所選的**傳輸要求識別碼**，以展開 [傳送資訊]

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="來源審核傳送要求":::

5.  查看轉移要求。 選取要傳送的要求 Azure 訂用帳戶。

>[!Note]  
> 繼續進行之前，請注意：您將無法再存取選取的訂閱。
> 您將不會獲得進一步使用的發票。
> Azure 保留專案不會與訂用帳戶一起轉移。

6.  然後選取 [ **接受並傳送** ] 以完成傳送程式。

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="選取要在您的 Azure 方案下傳送的訂用帳戶":::

7.  查看傳輸接受確認。

   此時，未來的夥伴、客戶和目前的合作夥伴將會透過電子郵件通知已接受的轉移要求。

   之後，在系統更新時，傳輸狀態可能會維持暫止最多15分鐘的時間，以接受轉換。 如果需要較長的時間，系統會繼續嘗試三天。 如果傳輸狀態仍保持擱置，則夥伴應提交服務要求。

   一旦傳輸完成後，要求中所包含的訂用帳戶將會出現在未來合作夥伴的 Azure 方案中，且不再與您一起列出。

>[!Note]  
>若為間接提供者：請通知您的間接轉銷商已接受轉移要求。

### <a name="managing-your-transferred-customer-subscriptions"></a>管理您已轉移的客戶訂用帳戶
- 使用 Azure 角色型存取控制 (RBAC) 為現有使用者、群組或服務主體指派的存取權，在轉換期間不受影響。 Azure 角色型存取控制 [ (AZURE RBAC) ](/azure/role-based-access-control/overview) 協助客戶管理可存取 azure 資源的人員、這些資源的使用方式，以及他們有權存取的區域。 作為新的合作夥伴，您不會在訂用帳戶轉移之後，對客戶的資源提供任何 RBAC 存取權。 您客戶的先前合作夥伴會保留其 RBAC 存取權。 與您的客戶合作，瞭解誰有見解的訂閱，以及如何進行任何想要的變更。

- 因此，請務必讓您的客戶移除其先前合作夥伴的 Azure RBAC 存取權，並加入新夥伴的存取權。 如需提供新存取權的客戶詳細資訊，請參閱 [什麼是 AZURE RBAC)  (azure 角色型存取控制？](/azure/role-based-access-control/overview) 如需移除先前合作夥伴 RBAC 存取權的客戶詳細資訊，請參閱 [移除角色指派](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)。

- 此外，您不會自動 [代表 (AOBO ](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) 取得訂用帳戶的) 存取權。 需要 AOBO，才能代表合作夥伴管理其客戶的 Azure 訂用帳戶。 如需有關 Azure 許可權的詳細資訊，請參閱 [取得管理客戶服務或訂用帳戶的許可權。](/partner-center/customers-revoke-admin-privileges)

## <a name="next-steps"></a>後續步驟：

- [ (Azure RBAC) ](/azure/role-based-access-control/overview)
- [取得管理客戶服務或訂用帳戶的許可權。](/partner-center/customers-revoke-admin-privileges)