---
title: 使用 Windows Autopilot 設定檔自訂裝置的全新體驗 |合作夥伴中心
description: 使用 Autopilot 設定檔預先設定裝置的全新體驗。
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: autopilot，windows autopilot，microsoft autopilot，零接觸部署，oobe，登入畫面，現成的
ms.localizationpriority: medium
ms.openlocfilehash: 7861efa8c0fd7e03488ba3f222fcb3a476c06cc2
ms.sourcegitcommit: 76c34fd8dc544cea93496079df68759a1da9098c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/04/2019
ms.locfileid: "73544046"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>使用 Windows Autopilot 設定檔自訂裝置的全新體驗

**適用於**

- CSP 直接帳單合作夥伴、間接提供者和間接轉銷商

如果您管理客戶裝置，您可能需要針對客戶的使用者自訂全新體驗（OOBE）。 您可以先使用 Windows Autopilot 設定檔預先設定新的裝置，再將裝置傳遞給客戶，並將新的設定檔套用至客戶已購買的裝置。 

請注意，Oem 已開始在 [Autopilot 裝置] 方塊外部加入出貨標籤，以顯示裝置的**產品金鑰識別碼（PKID）** 。  這個一維、可讀取的條碼提供下游合作夥伴一種方式來註冊裝置以進行 Autopilot，而不需要將裝置取消裝箱，並以替代方式收集裝置識別碼。

本文說明如何建立 Autopilot 設定檔，並將其套用至合作夥伴中心內的裝置。

如果您還不熟悉 Autopilot，請參閱下列文章中的資訊：

- [Windows Autopilot 概觀](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署參考指南](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概觀

透過合作夥伴中心的 Windows Autopilot 功能，您可以建立自訂設定檔，以套用至客戶裝置。 發行本文時，可以使用下列設定檔設定：

- 略過隱私權設定。 這個選擇性的 Autopilot 設定檔設定可讓組織不會在 OOBE 程式期間詢問隱私權設定。

- 停用裝置上的本機系統管理員帳戶建立。 組織可以決定在程式完成後，設定裝置的使用者是否應該具有系統管理員存取權。

- 自動設定適用于公司或學校的裝置。 向 Autopilot 註冊的所有裝置都會自動視為公司或學校的裝置，因此不會在 OOBE 程式期間詢問此問題。

- 略過 Cortana、OneDrive 和 OEM 註冊設定頁面。 向 Autopilot 註冊的所有裝置都會在全新體驗（OOBE）程式期間自動略過這些頁面。

- 略過使用者授權合約（EULA）。 從 Windows 10 1709 版開始，組織可以決定略過在 OOBE 程式中顯示的 EULA 頁面。 請參閱下面的 [Windows AUTOPILOT EULA 關閉](#windows-autopilot-eula-dismissal)，以取得在 Windows 安裝期間略過 EULA 頁面的重要資訊。

以下是適用的設定檔和裝置管理許可權和限制：

- CSP 合作夥伴可以繼續管理具有轉售商關係之現有客戶的 Autopilot 設定檔，即使客戶已移除合作夥伴的委派系統管理許可權也一樣。

- 您可以為已新增的客戶管理現有的裝置。

- 您無法管理客戶已上傳至 Microsoft Store for Business 或 Microsoft Intune 入口網站的裝置。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>在合作夥伴中心建立和管理 Autopilot 設定檔

在合作夥伴中心，您可以建立 Windows Autopilot 部署設定檔，並將其套用至裝置。

>[!NOTE]
>只有系統管理員代理程式可以建立和套用設定檔。

### <a name="create-a-new-autopilot-profile"></a>建立新的 Autopilot 設定檔

1. 從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您要為其建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [**裝置**]。

3. 在 [ **Windows Autopilot 設定檔**] 底下，選取 [**新增設定檔**]。

4. 輸入設定檔的 [名稱] 和 [描述]，然後設定 OOBE 設定。 選擇：  

   - 在安裝程式中略過隱私權設定

   - 停用設定中的本機系統管理員帳戶
  
   - 自動略過設定中的頁面<br>
        （包括*自動選取公司或學校的設定*，以及*略過 Cortana、OneDrive 和 OEM 註冊設定頁面*）
  
   - 略過使用者授權合約（EULA）<br> 
       >[!IMPORTANT] 
       >請參閱下面的 [Windows AUTOPILOT EULA 關閉](#windows-autopilot-eula-dismissal)，以取得在 Windows 安裝期間略過 EULA 頁面的重要資訊。

5. 完成時選取 **\[提交\]** 。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>將 Autopilot 設定檔套用至客戶裝置

>[!NOTE]
>下列指示假設您已將客戶的裝置新增至合作夥伴中心，而且您可以存取其裝置清單。 如果您尚未新增客戶的裝置，請遵循[將裝置新增至客戶的帳戶](#add-devices-to-a-customers-account)中的指示，然後遵循下列步驟。

為客戶建立 Autopilot 設定檔之後，您可以將它套用至客戶的裝置。

1. 從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [**裝置**]。

3. 在 [**將設定檔套用至裝置**] 下，選取您想要新增設定檔的裝置或裝置群組，然後選取 [套用**設定檔**]。 您剛才套用的設定檔會出現在 [**設定檔**] 資料行中。

4. 請遵循下列步驟來確認設定檔將會成功套用至裝置。

    a.  將裝置連線到網路，並將它開啟。

    b。  確認是否會顯示適當的 OOBE 畫面 (如果有的話)。

    c.  當 OOBE 程式停止時，將裝置重設為其原廠預設值，為新的使用者準備它。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>從客戶的裝置移除 Autopilot 設定檔

1. 從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [**裝置**]。

3. 在 [**將設定檔套用至裝置**] 下，選取您想要移除設定檔的裝置，然後選取 [**移除設定檔**]。

   >[!NOTE]
   >從裝置移除設定檔並不會刪除清單中的設定檔。 如果您想要刪除設定檔，請依照[更新或刪除 Autopilot 設定檔](#update-or-delete-an-autopilot-profile)中的指示進行。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或刪除 Autopilot 設定檔

若客戶想要在您將裝置寄送給他們之後變更全新體驗，您可以在 [合作夥伴中心] 中變更設定檔。

當客戶的裝置連線到網際網路時，它會在 OOBE 程式中下載最新的設定檔版本。 此外，當客戶將裝置還原為其出廠預設值時，裝置會在 OOBE 程式中再次下載最新的設定檔版本。

1. 從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取想要變更 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [**裝置**]。

3. 在 [ **Windows Autopilot 設定檔**] 下，選取您需要更新的設定檔。 進行必要的變更，然後選取 [**提交**]。

若要刪除此設定檔，請選取頁面右上角的 [**刪除設定檔**]。

### <a name="add-devices-to-a-customers-account"></a>將裝置新增至客戶的帳戶

>[!NOTE]
>「銷售代理程式」和「管理員」代理程式可以將裝置新增至客戶的帳戶。

在您可以將自訂 Autopilot 設定檔套用至客戶裝置之前，您必須能夠存取客戶的裝置清單。

如果您打算使用 OEM 名稱、序號和型號組合，請注意下列限制：

- 這個元組僅適用于較新的裝置（例如4k 雜湊），不支援128b 雜湊（RS2 和先前的裝置）。

- 元組註冊會區分大小寫，因此檔案中的資料必須與 OEM 提供者（硬體提供者）所提供的***完全***相符。

請依照下列指示，將裝置新增至合作夥伴中心內的客戶帳戶。

1. 從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您要管理其裝置的客戶。

2. 在客戶的詳細資料頁面上，選取 [**裝置**]。

3. 在 [**將設定檔套用至裝置**] 下，選取 [**新增裝置**]。

4. 輸入裝置清單的名稱，然後選取 **[流覽]** ，將客戶的清單（以 .csv 檔案格式）上傳至合作夥伴中心。

    >[!NOTE]
    >您應該已收到您的裝置購買的此 .csv 檔案。 如果您未收到 .csv 檔案，您可以遵循[將裝置新增至 Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步驟，自行建立一個。  

5. 上傳 .csv 檔案，然後選取 [**儲存**]。

如果您在嘗試上傳 .csv 檔案時收到錯誤訊息，請檢查檔案的格式。 您只能使用硬體雜湊，或 OEM 名稱、序號和型號（以該資料行順序），或 Windows 產品識別碼。 您也可以使用 [**新增裝置**] 旁的連結所提供的範例 .csv 檔案來建立裝置清單。

您的 .csv 檔案看起來應該像這樣：

> **裝置序號、Windows 產品識別碼、硬體雜湊、製造商名稱、裝置型號**

> **{serialNumber},,, Microsoft Corporation，Surface 膝上型電腦**

請注意，「製造商名稱」和「裝置型號」區分大小寫。

如果您不知道要為製造商名稱和裝置型號放入什麼值，您可以在裝置上執行此動作，以收集正確的值：

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 關閉

### <a name="important-information"></a>重要資訊

Windows Autopilot 可讓您在為客戶管理的裝置上設定自訂的 Windows 安裝。 如果客戶有權執行此動作，您可以在設定 Windows 時抑制或隱藏一般會呈現給使用者的特定設定畫面，包括 EULA （使用者授權合約）接受畫面。

藉由使用此函式，您同意隱藏或隱藏設計為使用者提供通知或接受條款的任何畫面，這表示您已向客戶取得足夠的同意和授權，以隱藏條款，而且代表您的客戶（無論是組織或個別的使用者，也可能是），同意任何通知並接受適用于您客戶的任何條款。 這包括同意授權條款和條件，或若未使用此工具抑制或隱藏時會對使用者顯示的通知。 您的客戶不可在這些裝置上使用 Windows 軟體，如果他們未向 Microsoft 或其授權經銷商有效取得軟體授權。
