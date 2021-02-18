---
title: 將 Azure 訂用帳戶轉移給另一個合作夥伴
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何變更與客戶的 Azure 訂用帳戶相關聯的雲端解決方案提供者方案合作夥伴。
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: b9058b00708e0ed745c7d6343dfd9c04382cfa9e
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645651"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>了解如何將客戶的 Azure 訂用帳戶轉移給另一個合作夥伴

**適用於**

- Microsoft Cloud for US Government 適用的合作夥伴中心
- 適用于 Microsoft 全球雲端的合作夥伴中心
- 雲端解決方案提供者 (CSP) 計畫中的合作夥伴

本文說明客戶如何將其 Microsoft Azure 服務從一個雲端解決方案提供者 (CSP) 切換至另一個。

若要將客戶的 Azure 服務或訂用帳戶切換到不同的夥伴，請依照這些手動步驟進行。 夥伴和客戶都需要完成這些步驟。

>[!Note]  
>目前，只有直接或間接提供者可以傳送訂閱。
>您無法變更與 Azure 方案、Office 365、企業行動套件或 Microsoft Dynamics CRM 訂用帳戶相關聯之雲端解決方案提供者訂用帳戶的合作夥伴。

## <a name="switch-partners-for-azure-subscriptions"></a>切換 Azure 訂用帳戶的合作夥伴

1. 如果要將 Azure 訂閱轉移至新的合作夥伴，客戶必須開始該程序，並以書面方式連絡其目前記錄的合作夥伴。

   >[!Note]
   > 目前的合作夥伴必須負責建立起始移轉程序的服務票證。 Microsoft 無法代表客戶或新合作夥伴介入。 客戶應做好與目前合作夥伴密切合作的計劃，使轉移程序進行順暢。

2. 訂用帳戶的夥伴必須執行下列工作：

   從合作夥伴中心建立 Azure 服務票證以要求訂用帳戶移轉：

   1. 從 [合作夥伴中心] 功能表中，選取 [ **客戶**]，從清單中選取您的客戶，然後選取 [ **服務管理**]。 

   2. 在 **\[支援票證\]** 區段底下，選取 **\[新增票證\]** 下拉式清單並選擇 **\[Microsoft Azure\]**。
   
   3. 在 [ [Azure 入口網站](https://portal.azure.com)中，選取 [ **新增支援要求**]。
   
   4. 在步驟1中，選擇 [訂用帳戶 **管理** ] 作為 [問題類型]，指定您要傳送的訂用帳戶識別碼，然後選擇 [ **雲端解決方案提供者** ] 作為支援方案。
   
   5. 在步驟2中選取 [ **C-最不影響** ]，然後選擇 [ **其他一般問題** ] 做為問題類型。
   
   6. 下載 [CSP 訂用帳戶移轉表單](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)。

3. 訂閱的合作夥伴：請填寫[雲端解決方案提供者訂閱移轉表單](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)，簽署該表單，然後將它寄給客戶。 

   如果要填寫表單，您將會需要下列資訊：

   - 目前合作夥伴的連絡資訊和 Microsoft ID。 在 [合作夥伴中心] 功能表中，選取 [ **帳戶設定** &gt; **組織設定檔**]，並使用此處所列的 **Microsoft ID**、 **組織名稱** 和 **位址** 。

   - 客戶的 Microsoft 識別碼。 在 [合作夥伴中心] 功能表中，選取 [ **Customers**]，然後展開客戶的清單以查看其 **Microsoft ID**。

   - 要移轉的訂閱識別碼。 在展開的客戶清單中，選取 [ **View** 訂用帳戶]，然後展開選擇的訂用帳戶以查看訂用帳戶 **識別碼**。

   >[!Note]
   >轉移訂閱會產生兩個訂閱識別碼，您會在已轉移訂閱的 **\[編輯訂閱\]** 頁面上看到這兩個訂閱碼：**1**- 合作夥伴中心訂閱識別碼，用於計費目的。 **2** - 原始 Azure 訂閱識別碼也會保留並出現在合作夥伴中心，以及 Azure 管理入口網站中。 這個識別碼會出現在您的對帳檔案。  **記錄支援票證時，這兩個識別碼都要用到。**

4. 訂閱的客戶和新合作夥伴：

   檢閱表單，填寫新合作夥伴的相關資訊，然後簽署該表單。 確認新客戶已準備好合約協定。 將表單重新寄給目前記錄的合作夥伴。

   *重要* 事項：如果新的 CSP 合作夥伴與客戶之間沒有轉銷商關聯性，則必須在轉移訂用帳戶之前建立一個。 [您可以在這裡找到相關做法的資訊](request-a-relationship-with-a-customer.md)。

   >[!Note]
   >新的 CSP 合作夥伴和客戶租使用者必須位於相同的國家/地區。 

5. 目前的合作夥伴︰

   請確定表單包含兩個夥伴管理員的連絡人資訊。 Microsoft 支援服務將會聯繫這兩個系統管理員來確認傳送。 請確定您有三個簽章。 然後使用檔案 **上傳** 選項，將完成的表單附加至您現有的服務要求。 Microsoft 支援工程師將會在八個工作時間內回復您，以驗證收據和完成。

6. 新的合作夥伴：

   更新 Azure 訂用帳戶設定以將舊合作夥伴從帳戶中移除。 若要查看布建了哪些角色指派，請執行兩個 PowerShell Commandlet。

   - 在帳戶上將新合作夥伴新增為經銷商：

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > 客戶的 **租使用者識別碼** 會以客戶的 **Microsoft 識別碼** 形式出現在合作夥伴中心中。 若要尋找特定客戶的 Microsoft ID (租使用者識別碼) ，請登入合作夥伴中心 [儀表板](https://partner.microsoft.com/dashboard)。 然後從功能表中選取 [ **客戶** ]。 在清單上找出客戶。 選取向下箭號以展開客戶的清單。 您會看到客戶的 *功能變數名稱* 和客戶的 **Microsoft ID** 的相關資訊。 在 PowerShell commandlet 中使用16位數的 **MICROSOFT ID** 。

   - 在帳戶上檢視角色，包括先前的雲端解決方案提供者合作夥伴：

     ```powershell
     Get-AzRoleAssignment
     ```

7. 移除過時存取權限

   - 在 [合作夥伴中心] 功能表中，選取 [ **客戶**]。
   - 在清單上找出客戶。 選取 (按兩下) 其公司名稱。 這會開啟 [客戶 **訂閱** ] 頁面。
   - 在 [客戶詳細資料] 功能表中，選取 [ **服務管理**]。
   - 在 **\[Microsoft Azure\]** 下方，按一下連結以移至 **\[Microsoft Azure 管理入口網站\]**。

## <a name="next-steps"></a>下一步

- 下載 [CSP 訂用帳戶移轉表單](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)。

- 深入瞭解 [多合作夥伴支援](multipartner.md)。

- [多合作夥伴支援](multipartner.md)。
- [多通道支援](multichannel.md)。
- [轉移 Azure 訂閱](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)