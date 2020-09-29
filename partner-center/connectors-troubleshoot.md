---
title: 對共同銷售推薦連接器進行疑難排解
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有關如何針對共同銷售連接器進行疑難排解的常見問題。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: d34a13a6789f3bd712d2cec3a594b8e407f7449d
ms.sourcegitcommit: 3329fd120d8d49a4831412b79e044678ec71b84c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/29/2020
ms.locfileid: "91422334"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>對共同銷售推薦連接器進行疑難排解

**適用於：**

- 合作夥伴中心
- Dynamics 365 CRM
- Salesforce CRM

**適當的角色**

- 推薦管理員
- CRM 上的系統管理員或系統自訂員

 ## <a name="questions-and-answers-about-pre-requisites"></a>先決條件的相關問題和解答

1. 您可以針對您的環境使用試用共同銷售推薦連接器解決方案嗎？

如果您是在測試/預備環境中，您可以選擇試用版解決方案。 付費版本的連接器可在 AppSource 中使用，每月 $ 15/月。 使用付費連線時，您每天會收到10K 的 API 呼叫。 連接器是合作夥伴中心參考 Api 之上的包裝函式。 每當連接器解決方案針對合作夥伴中心或 CRM 端的商機執行 **建立** 或 **更新** 事件時，就會進行 API 呼叫。

2. 您需要在 CRM 環境中建立區段的角色為何？

身為系統管理員或系統自訂員的使用者，可以為所有人套用變更。 不過，所有的應用程式使用者都可以個人化系統，甚至與其他人共用部分自訂。 

3. 合作夥伴銷售人員是否需要特殊角色才能處理合作夥伴中心？
 
合作夥伴賣方必須獲派「推薦系統管理員」角色。 如需詳細資訊，請參閱下列 [許可權總覽) # B1 建立-使用者-帳戶-和設定許可權) 。

4. 您需要在 CRM 環境中先設定哪些欄位？ 

•確定您的貨幣適用于您的位置，並且正確地放在您的 CRM 環境中。 •您的銷售小組應以 crm 使用者的形式列在您的 CRM 環境中。

5.  Power Automate 環境建立需要哪些必要條件？

若要使用 Power Automate 環境，您需要：

- 需要 Power Automate 授權。
- 至少需要 1 GB 的儲存體。

6.  您需要 Dynamics 365 訂用帳戶才能使用 Salesforce 連接器解決方案嗎？

Salesforce 連接器解決方案的類型為「Dynamics Flow」，可支援與其他 CRM 系統進行同步處理。 解決方案不需要您擁有 Dynamics 365 實例或訂用帳戶。 安裝 Salesforce 解決方案時，可能會出現您公司中現有 CD 環境的下拉式清單。 您必須選取該環境。 此外，如果您收到錯誤，表示找不到連線到已登入使用者的 Dynamics 365 組織，則您必須為連接器建立新的環境。

## <a name="questions-and-answers-about-configuration"></a>關於設定的問題和解答

1. 如果您在 Power Automate 平臺中啟動流程時遇到下列錯誤，該怎麼辦？

錯誤： Azure Resource Manager 的要求失敗，錯誤為： ' {"error"： {"code"： "WorkflowTriggerNotFound"，"message"： "找不到工作流程 ' e14d00f1-1fdf-4b1b-aaac-54a5064093d3 ' 觸發程式 ' manual '。"}} '。 

遵循下列疑難排解步驟：

- 刪除 CD 連線，然後重新建立 CD 連線。
- 關閉和開啟子流程 
- 刪除解決方案，然後重新安裝解決方案。 

2.  如果您在 Power Automate 平臺中新增合作夥伴中心連接器時遇到下列錯誤，該怎麼辦？

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="要求登入的錯誤訊息":::

遵循下列疑難排解步驟：

- 使用合作夥伴中心登入 (flow.microsoft.com) 登入流程環境。


3. 如果您在 Power Automate 平臺中啟用 CRM 流程的合作夥伴中心時收到下列錯誤，該怎麼辦？
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="需要更新的錯誤訊息":::

遵循下列疑難排解步驟：

- 先啟用下列兩個子流程，再啟用合作夥伴中心至 CRM flow。
      - 合作夥伴中心至 CRM-Helper (Insider Preview) 
      - 合作夥伴中心 Microsoft 共同銷售參考更新至 CRM (Insider preview) 

4. 當您嘗試編輯流程時，當您無法將連接新增至流程時，該怎麼辦？

當流程正在執行時，您會在流程中加入流程的連接，而且您會分別新增至每個流程。  如果在編輯流程時，新增連接的對話方塊未自動開啟，則您可以編輯流程的每個步驟和子步驟，以新增連接。

- 選取每個流程，並個別加以編輯。
- 展開流程中的所有步驟 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="需要連接的步驟":::

- 選取您會在其中看到警告圖示的步驟，要求關聯連接，以及新增連接。 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="逐步編輯流程":::


5. 如果共同銷售推薦連接器解決方案的流程未啟用 (開啟) ，您該怎麼做？

A. 在 Power Automate 中，您將需要依下列順序編輯流程，並將其更新為使用個別的連接：

- 合作夥伴中心 Webhook 註冊 (Insider Preview) 
- 建立共同銷售參考-Salesforce 至合作夥伴中心 (Insider Preview) 
- 合作夥伴中心 Microsoft 共同銷售參考更新至 Salesforce (Insider preview) 
- 合作夥伴中心至 Salesforce (Insider preview) 
- Salesforce 至合作夥伴中心 (Insider Preview) 
- 合作夥伴中心 (Insider Preview) 的 Salesforce 機會
- 合作夥伴中心 (Insider Preview) 的 Salesforce Microsoft 解決方案

 B. 針對每個流程，選取 [ **僅執行使用者** ] 選項。 選取 [ **使用連接** ，而不是 **由僅限執行的使用者提供**]。  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="啟用流程":::


C. 在下列提及的流程中啟用下列各項：

 - 合作夥伴中心 Microsoft 共同銷售參考更新至 Salesforce (Insider preview) 

- Salesforce 至合作夥伴中心 (Insider Preview) 

    
D. 啟用所有剩餘的流程。

E. 在 [flow] 合作夥伴中心 Webhook 註冊中，選取 [ **執行**]。 從合作夥伴中心中的第一個動作提供 **HTTP url** **至 Salesforce** flow。 選取 [ **要註冊的事件** ] 底下的四個選項，然後選取 **[是]** 進行覆寫。

## <a name="questions-and-answers-about-runmaintenance"></a>有關執行/維護的問題和解答

1. 當 Power Automate 流程執行期間發生失敗時，您要如何進行疑難排解？

為了確保您的 Power Automate 流程會如預期般執行，並在執行期間針對失敗進行疑難排解，請參閱 [修正流程失敗](/power-automate/fix-flow-failures)。

2. 如果您在合作夥伴中心或 CRM 環境中看到未正確同步處理的參考，該怎麼辦？
 
若要判斷參照同步處理的狀態，請選取 [ **Audit**]。 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="如何同步處理參考":::

請確定符合下列條件：

- 解決方案識別碼會作為商機的一部分來提供。

- 需要兩個字母的國家/地區代碼。

- 當您為商機選取 Microsoft 的協助時，需要客戶連絡人資訊。

3. 在哪些條件下，參考不會雙向同步處理

確認下列事項：

- 合作夥伴銷售人員必須確保他們已啟用與 CRM 區段中合作夥伴中心選項的 **同步** 。

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="確定您已啟用同步處理":::

- 銷售人員必須在符合潛在客戶時提供收入和結束日期。

- 如果在建立或更新共同銷售商機中提供 CRM 識別碼，而且在 CRM 中找不到具有該識別碼的潛在客戶/商機，則會忽略該商機的 update 或 create。

- 確定已在 Salesforce 環境上設定參考貨幣欄位。 

4. 如果連接器中斷連線，而您錯過了參考同步處理，該怎麼辦。 

以下是您可以嘗試的幾個選項：

- 使用參考系統管理員角色檢查合作夥伴中心使用者的使用者名稱或密碼是否已過期。

- 您可以移至未同步處理的商機、進行次要更新，並觀察參考是否已同步處理。

- 如果流程已執行且失敗，請選取流程，然後重新提交失敗的執行。

5. 當您收到拒絕存取的錯誤時，該怎麼辦？

請確定有適當的角色存在

- 合作夥伴中心賣方的推薦系統管理員角色 
 
- 您 CRM 實例上的系統管理員或系統自訂員角色

- 確認 Power Automate flow 帳戶使用者事先登入 https://flow.microsoft.com 至少一次

6. 如果您在建立共同銷售商機時看到 **客戶帳戶的國家/地區代碼** 遺失，該怎麼辦？

您必須將 ISO 兩個字母的國家/地區代碼新增至 CRM 中的客戶帳戶。

7. 如果您在建立共同銷售商機時看到 **解決方案識別碼所需** 的錯誤，該怎麼辦？

若要建立共同銷售的參考，您需要 Microsoft 共同銷售準備就緒的解決方案。 

8. 當您看到在合作夥伴中心中建立且未同步處理至 CRM 的共同銷售商機時，該怎麼辦，即使沒有任何流程錯誤也是一樣：

執行下列動作：

- 在合作夥伴中心中建立新的共同銷售交易之後，請檢查是否已叫用合作夥伴中心至 Dynamics 365 流程， (可能會) 叫用多次。

- 如果已叫用流程，請檢查所有叫用的流程，並識別會更新 CRM 的流程執行。 您可以遵循這些動作，並確認它是否已更新 CRM 或遇到問題。

- 檢查合作夥伴中心中的 [ *新增交易**]，查看是否已填入 CRM 識別碼。

- 確定在合作夥伴中心中，交易不會意外地關閉為「成功」或「遺失」。

## <a name="next-steps"></a>後續步驟

- [管理潛在客戶](manage-leads.md)
 
- [管理共同銷售商機](manage-co-sell-opportunities.md)