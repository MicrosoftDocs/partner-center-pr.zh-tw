---
title: 授予合作夥伴的客戶代理人系統管理權限 | 合作夥伴中心
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何要求客戶委派系統管理員許可權給轉銷商，或移除相同的許可權，以及如何使用這些許可權。
author: LauraBrenner
ms.author: labrenne
keywords: 委派的系統管理員許可權、代表的系統管理員、移除許可權、AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253477"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>授予合作夥伴的客戶代理人系統管理權限

**適用於**

-  合作夥伴中心

若要代表客戶管理客戶的服務或訂閱，客戶必須授與您該服務的系統管理員權限。 若要從客戶取得系統管理員權限，請透過電子郵件傳送建立經銷商關係要求給他們。 客戶核准您的要求後，您就能登入服務的系統管理員入口網站及代表客戶管理服務。 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>邀請客戶與您建立經銷商關係

1.  選取 [**客戶**]，然後選取 [**要求轉銷商關係**]。

2.  在下一頁，複查草稿電子郵件訊息。 您可以在預設電子郵件應用程式中開啟草稿訊息，或您可以將訊息複製到您的剪貼簿，並將它貼到電子郵件。 

    >[!IMPORTANT]
    >您可以在電子郵件中編輯文字，但是請務必包含連結，因為它已個人化，用來將客戶直接連結至您的帳戶。 
    
3.  當您完成此步驟時，請選取 [**完成**]。

4.  將電子郵件傳送給您的客戶。

5.  客戶接受邀請之後，他們將會出現在您的 **\[客戶\]** 頁面，而且您將能從該處佈建客戶及管理其服務。

6.  若要管理客戶的帳戶、服務、使用者和授權，請選取名稱附近的向下箭號，然後選取您想要管理之服務的系統管理入口網站，以展開客戶的記錄。

>[!IMPORTANT]  
>客戶可以在服務的管理員入口網站中重新指派或移除系統管理員許可權。 不過，除非並直到您與客戶重新協商合約，您繼續負責提供客戶支援和遵守雲端轉銷商合約，即使客戶重新指派或移除系統管理員權限。 在此情況下，如果客戶需要協助，請洽詢 Microsoft 支援服務以代表客戶開啟服務要求。

您的客戶可以從 Office 365 系統管理員入口網站中，找出其合作夥伴具有其租使用者的系統管理員許可權。 請這樣做：

1. 客戶必須以全域管理員身分登入 Office 365 管理員入口網站。

2. 選取 [**設定**] > [**合作夥伴關聯**性]。

3. 在 [**合作夥伴關係**] 頁面上，客戶會看到與其合作的合作夥伴清單，以及已授與其租使用者之委派系統管理許可權的夥伴。

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>客戶可以管理合作夥伴的委派系統管理員許可權 

您的客戶可能會決定從其租使用者中移除您的委派系統管理員許可權，但保留與您的關係，以供訂閱和授權更新之用。 客戶在 Office 365 系統管理中心的 **\[合作夥伴關係\]** 頁面上管理其 Office 365 帳戶的權利和權限。 在這個頁面上，客戶可以：

- 查看他們與哪些合作夥伴擁有合作關係，以及哪些合作夥伴具有委派的系統管理員權限

- 從租使用者移除合作夥伴的委派系統管理許可權

若要移除合作夥伴的委派系統管理權限：

1. 在 **\[合作夥伴關係\]** 頁面下，選取感興趣的合作夥伴。
2. 在詳細資料窗格中，選取 **\[移除委派的管理員\]** 。
3. 在確認窗格中，選取 **\[移除\]** 。

>[!IMPORTANT]  
>指派給合作夥伴的 Azure AD 角色是隱含的。 如果您嘗試使用 Azure AD 入口網站/PowerShell/Graph 列出 Azure AD 角色成員，不會傳回合作夥伴。 若要了解合作夥伴是否獲指派 Azure AD 角色，您必須參考 Office 365 系統管理員入口網站中的合作夥伴關係頁面，查看是否將委派系統管理權限授與給合作夥伴。

## <a name="delegated-admin-privileges-in-azure-ad"></a>Azure AD 中委派的系統管理員權限 

合作夥伴的 Azure AD 租使用者中有兩個安全性群組 [管理員代理程式] 和 [技術服務人員]，用於委派系統管理。 當客戶授予委派的系統管理權限給合作夥伴：

- 系統管理員代理程式群組會指派給客戶的 Azure AD 租使用者中的全域管理員角色。

- 技術服務人員代理程式群組會指派給客戶的 Azure AD 租使用者中的技術支援中心系統管理員角色。

根據指派的目錄角色，這兩個群組的成員可以使用其合作夥伴認證和系統管理員代表客戶登入客戶的 Azure AD 租使用者和 O365 服務。

如果您的客戶移除委派的系統管理員許可權，則會移除 Azure AD 角色指派，而且您將無法再管理客戶的 Azure AD 租使用者。

### <a name="azure-subscriptions-and-resource-management"></a>Azure 訂閱和資源管理

每個 Azure 訂閱都有它自己的一組資源管理角色。 在 CSP 合作夥伴可以管理客戶的 Azure 訂用帳戶之前，必須將合作夥伴指派給 Azure 訂用帳戶底下的一或多個角色。 具體而言：

- 當客戶接受經銷商邀請並授予委派的系統管理權限給合作夥伴，合作夥伴不會自動取得客戶租用戶底下現有 Azure 訂閱的存取權。

- 當雲端解決方案提供者合作夥伴為客戶佈建新的 Azure 訂閱，雲端解決方案提供者合作夥伴租用戶底下的系統管理代理人群組會自動獲指派訂閱的擁有者角色。 根據此角色指派，群組成員可以存取及管理訂閱的資源。

- 當客戶使用 Office 365 入口網站移除合作夥伴的委派系統管理許可權時，只要合作夥伴仍然指派給訂用帳戶下的一個或多個角色，合作夥伴仍然可以管理客戶的 Azure 訂用帳戶。 若要停止合作夥伴管理 Azure 訂閱，客戶必須移除角色指派。

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

在合作夥伴中心，CSP 合作夥伴可以在這些情況下，不需委派系統管理員許可權，即可管理其客戶的 Autopilot 設定檔： 

- 如果客戶移除委派的系統管理許可權，但與您保持轉銷商關係，您可以繼續管理他們的 Autopilot 設定檔。

- 您可以管理您或其他合作夥伴新增的客戶裝置。 

- 您無法管理客戶透過商務用 Microsoft Store、教育 Microsoft Store 或 Microsoft Intune 入口網站新增的裝置。

如需 Autopilot 的詳細資訊，請參閱[使用 Windows Autopilot 簡化裝置設定](https://docs.microsoft.com/partner-center/autopilot)。

>[!IMPORTANT]  
>合作夥伴中心目前的 Autopilot 管理體驗可能會持續改變。 發行本文時，會考慮下列變更：

- 合作夥伴必須由客戶授予委派的系統管理權限，合作夥伴才能新增/更新/移除設定檔以及從客戶租用戶中的任何裝置套用/移除設定檔。

- 合作夥伴必須被授與客戶的委派系統管理許可權，合作夥伴才能移除其他合作夥伴或客戶在客戶租使用者中新增的裝置。 否則，合作夥伴只能移除相同合作夥伴先前加入的裝置。
