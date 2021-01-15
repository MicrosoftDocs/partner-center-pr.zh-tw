---
title: 安裝適用于 Power BI 的合作夥伴中心分析
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 遵循本文中的步驟，以安裝和預覽 CSP) 中直接合作夥伴的適用於 Power BI 的合作夥伴中心分析應用程式 (。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215844"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>安裝和預覽適用於 Microsoft Power BI 的合作夥伴中心分析應用程式


**適當的角色**
-   全域系統管理員
-   使用者系統管理員
-   銷售代理人
-   系統管理代理人

## <a name="before-you-begin"></a>開始之前

從下列可用的 Power BI 應用程式清單中，選取與您的業務最相關的應用程式：
- [直接提供者](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [間接提供者](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [間接轉銷商](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

安裝合作夥伴中心分析應用程式預覽版之前，請先確定您符合下列需求。

- 您可以為您的企業挑選正確的 Power BI 應用程式。

- 您有 Power BI pro 授權。

- 您有權在您的租使用者上安裝範本應用程式。

- 您可以登入 Power BI。

- 您可以使用全域管理員、系統管理員代理程式或帳單系統管理員身分登入 [公司的 Azure Active Directory (Azure AD) 租](azure-active-directory-tenants-and-partner-center.md)使用者。

## <a name="to-install-the-app"></a>若要安裝應用程式

1. 在上一節中，按一下指定 (直接提供者/間接提供者/間接轉銷商) 的應用程式來源連結。

2. 按一下 [ **立即取得**]。 

3. 按一下 [ **繼續**] 以同意條款及條件。

4. 在 \[已經有帳戶名稱了嗎?\] 下方選取 **\[登入\]**。

5. 在下一個頁面上，輸入您的 Power BI 的使用者名稱和密碼，然後選取 \[登入\]。

6. 藉由提供工作區名稱來安裝工作區。

7. 您可以在 [應用程式] 區段中找到已安裝的範本應用程式。

8. 按一下 [應用程式]，並選擇已安裝的應用程式。

9. 隨即開啟 [新增應用程式] 畫面的開始。

10. 若要連接到資料，請按一下 **[連接]**。

11. 在 [ **連接到合作夥伴中心 Analytics** ] 快顯視窗中，確認 [ **驗證方法** ] 設定為 [ **oAuth2** ]，或從清單中選取 [ **oAuth2** ] （如果沒有的話）。 

> [!NOTE]  
>  這個視窗可能需要幾分鐘才會出現。

12. 在 [ **合作夥伴中心 Analytics 連接器** ] 頁面上，使用全域管理員、系統管理員代理程式，或公司 Azure AD 租使用者的計費管理員認證登入，然後選取 [登 **入**]。
 
13. 出現存取權提示時，選取 **\[接受\]**。 

將合作夥伴中心分析服務連線到 Power BI 後，資料將會開始載入。 視資料數量而定，這最多可能需要花費 10 分鐘。 

資料完成載入後，您可以開始在 Power BI 中使用合作夥伴中心分析應用程式儀表板和報告。

## <a name="next-steps"></a>後續步驟

[使用適用於 Microsoft Power BI 的合作夥伴中心分析應用程式來檢視業務資料](power-bi-app-for-direct-partners-use.md)
