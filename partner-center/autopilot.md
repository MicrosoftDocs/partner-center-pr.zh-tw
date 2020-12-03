---
title: 自訂裝置的全新體驗
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在傳遞客戶的新裝置之前，您可以使用 Windows Autopilot 設定檔，自訂或預先設定裝置的全新體驗 (OOBE) 。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534979"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>在新裝置上使用 Windows Autopilot 設定檔，以自訂客戶的全新體驗

**適當的角色**

- 系統管理代理人
- 全域系統管理員
- 銷售代理人
- 使用者管理系統管理員

如果您管理客戶裝置，您可能需要為客戶的使用者自訂現成體驗 (OOBE) 。 您可以先使用 Windows Autopilot 設定檔預先設定新的裝置，再將裝置傳遞給客戶，並將新的設定檔套用至客戶已購買的裝置。 

請注意，Oem 已開始將出貨標籤包含在 Autopilot 裝置的外部，以顯示裝置的 **產品金鑰識別碼 (PKID)**。  這一維、可讀取的條碼可為下游合作夥伴提供註冊裝置以進行 Autopilot 的方式，而不需要將裝置 () ，而是透過替代方式來收集裝置識別碼。

本文說明如何在合作夥伴中心中建立 Autopilot 設定檔，並將其套用至裝置。

如果您還不熟悉 Autopilot，請參閱下列文章中的資訊：

- [Windows Autopilot 概觀](/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署參考指南](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概觀

利用合作夥伴中心中的 Windows Autopilot 功能，您可以建立自訂設定檔以套用至客戶裝置。 下列設定檔設定已在發行本文時提供：

- 略過隱私權設定。 此選用的 Autopilot 設定檔設定可讓組織在 OOBE 程式期間不詢問隱私權設定。

- 停用裝置上的本機系統管理員帳戶建立。 組織可以決定在程式完成之後，使用者設定裝置是否應該具有系統管理員存取權。

- 自動設定公司或學校裝置。 所有向 Autopilot 註冊的裝置都會自動被視為公司或學校裝置，因此在 OOBE 程式期間不會詢問此問題。

- 略過 Cortana、OneDrive 和 OEM 註冊設定頁面。 所有向 Autopilot 註冊的裝置，會在) 程式 (OOBE 的全新體驗期間自動略過這些頁面。

- 略過使用者授權合約 (EULA) 。 從 Windows 10 版本1709開始，組織可以決定略過 OOBE 程式期間所呈現的 EULA 頁面。 如需有關在 Windows 安裝期間略過 EULA 頁面的重要資訊，請參閱以下 [WINDOWS AUTOPILOT eula 關閉](#windows-autopilot-eula-dismissal) 。

以下是適用的設定檔和裝置管理權限和限制：

- CSP 合作夥伴可以針對具有轉售商關係的現有客戶繼續管理 Autopilot 設定檔，即使客戶已移除合作夥伴的委派系統管理權限也一樣。

- 您可以為已新增的客戶管理現有裝置。

- 您無法管理客戶上傳至商務用 Microsoft Store 或 Microsoft Intune 入口網站的裝置。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>在合作夥伴中心中建立和管理 Autopilot 設定檔

在合作夥伴中心中，您可以建立 Windows Autopilot 部署設定檔，並將其套用至裝置。

>[!NOTE]
>只有系統管理員代理程式可以建立及套用設定檔。

### <a name="create-a-new-autopilot-profile"></a>建立新的 Autopilot 設定檔

1. 從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取要為其建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [ **裝置**]。

3. 在 [ **Windows Autopilot 設定檔** ] 下，選取 [ **新增設定檔**]。

4. 輸入設定檔的名稱和描述，然後設定 OOBE 設定。 從下列選項進行選擇：  

   - 在安裝程式中略過隱私權設定

   - 停用設定中的本機系統管理員帳戶
  
   - 自動略過設定中的頁面<br>
         (包括 *自動選取公司或學校的設定* ，以及 *略過 Cortana、OneDrive 和 OEM 註冊設定頁面*) 
  
   - 略過使用者授權合約 (EULA) <br> 
       >[!IMPORTANT] 
       >如需有關在 Windows 安裝期間略過 EULA 頁面的重要資訊，請參閱以下 [WINDOWS AUTOPILOT eula 關閉](#windows-autopilot-eula-dismissal) 。

5. 完成時選取 **\[提交\]**。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>將 Autopilot 設定檔套用至客戶裝置

>[!NOTE]
>下列指示假設您已將客戶的裝置新增至合作夥伴中心，且您可以存取其裝置清單。 如果您尚未新增客戶的裝置，請遵循 [將裝置新增至客戶帳戶](#add-devices-to-a-customers-account) 中的指示，然後遵循下列步驟。

為客戶建立 Autopilot 設定檔之後，您可以將其套用至客戶的裝置。

1. 從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取您為其建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [ **裝置**]。

3. 在 [ **將設定檔套用至裝置** ] 下，選取您要新增設定檔的裝置或裝置群組，然後選取 [套用 **設定檔**]。 您剛剛套用的設定檔會出現在 [ **設定檔** ] 欄位中。

4. 遵循下列步驟來確認設定檔將會成功套用至裝置。

    a.  將裝置連線到網路，並將它開啟。

    b.  確認是否會顯示適當的 OOBE 畫面 (如果有的話)。

    c.  當 OOBE 程式停止時，請將裝置重設為其原廠預設值，為新的使用者準備該裝置。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>從客戶的裝置移除 Autopilot 設定檔

1. 從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取您為其建立 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [ **裝置**]。

3. 在 [ **將設定檔套用至裝置** ] 下，選取您要從中移除設定檔的裝置，然後選取 [ **移除設定檔**]。

   >[!NOTE]
   >從裝置移除設定檔並不會從您的清單中刪除設定檔。 如果您想要刪除設定檔，請依照 [更新或刪除 Autopilot 設定檔](#update-or-delete-an-autopilot-profile)中的指示進行。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或刪除 Autopilot 設定檔

如果客戶想要在您將裝置寄送至裝置之後變更現成體驗，您可以在合作夥伴中心中變更設定檔。

當客戶的裝置連線到網際網路時，它會在 OOBE 程式期間下載最新的設定檔版本。 此外，當客戶將裝置還原為其原廠預設設定時，裝置會在 OOBE 程式期間再次下載最新的設定檔版本。

1. 從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取想要變更 Autopilot 設定檔的客戶。

2. 在客戶的詳細資料頁面上，選取 [ **裝置**]。

3. 在 [ **Windows Autopilot 設定檔** ] 下，選取您需要更新的設定檔。 進行必要的變更，然後選取 [ **提交**]。

若要刪除此設定檔，請選取頁面右上角的 [ **刪除設定檔** ]。

### <a name="add-devices-to-a-customers-account"></a>將裝置新增至客戶的帳戶

>[!NOTE]
>銷售專員和系統管理員代理程式可以將裝置新增至客戶的帳戶。

您必須能夠存取客戶的裝置清單，才能將自訂 Autopilot 設定檔套用至客戶裝置。

如果您打算使用 OEM 名稱、序號和模型組合，請注意下列限制：

- 此元組僅適用于較新的裝置 (4k 雜湊，例如) ，而且不支援 (RS2 和先前裝置) 的128b 雜湊。

- 元組註冊會區分大小寫，因此檔案中的資料必須與 OEM 提供者所提供的模型和製造商名稱 **_完全_* 相符， (硬體提供者) 。

依照下列指示，在合作夥伴中心中將裝置新增至客戶的帳戶。

1. 從合作夥伴中心] 功能表中選取 [_ *客戶**]，然後選取您要管理其裝置的客戶。

2. 在客戶的詳細資料頁面上，選取 [ **裝置**]。

3. 在 [ **將設定檔套用至裝置** ] 下方，選取 [ **新增裝置**]。

4. 輸入裝置清單的名稱，然後選取 **[流覽]** ，以 .csv 檔案格式將客戶的清單 (上傳) 至合作夥伴中心。

    >[!NOTE]
    >您應該已在購買裝置時收到此 .csv 檔案。 如果您未收到 .csv 檔案，您可以依照 [將裝置新增至 Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步驟自行建立。  

5. 上傳 .csv 檔案，然後選取 [ **儲存**]。

如果您在嘗試上傳 .csv 檔案時收到錯誤訊息，請檢查檔案的格式。 您只能使用硬體雜湊，或 OEM 名稱、序號和型號 (依該資料行順序)，或 Windows 產品識別碼。 您也可以使用 [ **新增裝置** ] 旁的連結所提供的範例 .csv 檔案來建立裝置清單。

您的 .csv 檔案看起來應該像這樣：

> **裝置序號、Windows 產品識別碼、硬體雜湊、製造商名稱、裝置型號**

> **{serialNumber},,, Microsoft Corporation，Surface Laptop**

>[!NOTE]
> 「製造商名稱」和「裝置型號」會區分大小寫。

如果您不知道要為製造商名稱和裝置型號放置哪些值，您可以在裝置上執行，以收集正確的值：

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 關閉

### <a name="important-information"></a>重要資訊

Windows Autopilot 可讓您在為客戶管理的裝置上設定 Windows 的自訂安裝。 如果客戶已獲授權，您可以隱藏或隱藏設定 Windows 時通常會向使用者呈現的特定設定畫面，包括 EULA (使用者授權合約) 接受畫面。

藉由使用此函數，您同意隱藏或隱藏任何設計來提供使用者通知或接受條款的畫面，表示您已從客戶取得足夠的同意與授權來隱藏條款，而您代表客戶 (是否可以) 組織或個別使用者，或同意任何通知，並接受任何適用于您客戶的條款。 這包括同意授權條款和條件，或若未使用此工具抑制或隱藏時會對使用者顯示的通知。 您的客戶不可在這些裝置上使用 Windows 軟體，如果他們未向 Microsoft 或其授權經銷商有效取得軟體授權。