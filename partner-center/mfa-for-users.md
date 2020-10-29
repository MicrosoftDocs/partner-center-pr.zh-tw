---
title: 使用多重要素驗證來設定您的使用者
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何使用 MFA 為員工進行設定
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526002"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="0c665-103">使用多重要素驗證來設定您的使用者</span><span class="sxs-lookup"><span data-stu-id="0c665-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="0c665-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="0c665-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0c665-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="0c665-105">Global admin</span></span>

<span data-ttu-id="0c665-106">較高的隱私權保護和安全性是我們最優先的考量。</span><span class="sxs-lookup"><span data-stu-id="0c665-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="0c665-107">我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。</span><span class="sxs-lookup"><span data-stu-id="0c665-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="0c665-108">這就是為什麼我們需要生態系統中的每個人都採取行動，並確保具備適當的安全性保護。</span><span class="sxs-lookup"><span data-stu-id="0c665-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="0c665-109">為了協助保護合作夥伴和客戶，我們針對參與雲端解決方案提供者計畫的顧問、控制台廠商和合作夥伴推出一組強制性的安全性需求。</span><span class="sxs-lookup"><span data-stu-id="0c665-109">To help safeguard partners and customers, we are introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="0c665-110">合作夥伴都必須針對其合作夥伴租用戶的所有使用者帳戶強制執行多重要素驗證 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="0c665-110">Partners are required to enforce multi-factor authentication (MFA) for all user accounts in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="0c665-111">為使用者新增多重要素驗證</span><span class="sxs-lookup"><span data-stu-id="0c665-111">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="0c665-112">您必須是公司的全域管理員才能完成這項工作。</span><span class="sxs-lookup"><span data-stu-id="0c665-112">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="0c665-113">若要為使用者啟用 MFA，最簡單的方法是在將使用者新增至 Azure AD 租用戶時進行。</span><span class="sxs-lookup"><span data-stu-id="0c665-113">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="0c665-114">登入 [Azure 入口網站](https://portal.azure.com)，然後移至 [使用者管理]。</span><span class="sxs-lookup"><span data-stu-id="0c665-114">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management** .</span></span>
1. <span data-ttu-id="0c665-115">選取 [多重要素驗證]。</span><span class="sxs-lookup"><span data-stu-id="0c665-115">Select **Multi-factor authentication** .</span></span>
1. <span data-ttu-id="0c665-116">選取您想要啟用的使用者，然後選取 [啟用]。</span><span class="sxs-lookup"><span data-stu-id="0c665-116">Select the user you want to enable and then select **Enable** .</span></span>

<span data-ttu-id="0c665-117">這會為這名使用者啟用 MFA。</span><span class="sxs-lookup"><span data-stu-id="0c665-117">This will enable MFA for this user.</span></span> <span data-ttu-id="0c665-118">[已啟用] 表示系統會要求使用者在第一次登入時設定其 MFA 驗證。</span><span class="sxs-lookup"><span data-stu-id="0c665-118">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="0c665-119">之後在登入時，系統就會要求其提供透過電子郵件或簡訊所收到的驗證碼。</span><span class="sxs-lookup"><span data-stu-id="0c665-119">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message.</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何驗證":::

<span data-ttu-id="0c665-121">若要強制使用者使用 MFA，您可以使用上述相同步驟，並選取 [強制執行] 來 **強制執行** 。</span><span class="sxs-lookup"><span data-stu-id="0c665-121">To force users to use MFA, you can **Enforce** using same steps as above and selecting **Enforce** .</span></span> <span data-ttu-id="0c665-122">請深入了解，閱讀[啟用每一使用者 Azure Multi-Factor Authentication 以保護登入事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)。</span><span class="sxs-lookup"><span data-stu-id="0c665-122">Learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="0c665-123">所有使用者都會從 [已停用] \*\*\*\* 開始。</span><span class="sxs-lookup"><span data-stu-id="0c665-123">All users start out **Disabled** .</span></span> <span data-ttu-id="0c665-124">當您以每一使用者 Azure Multi-Factor Authentication 註冊使用者時，其狀態會變更為 [已啟用] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="0c665-124">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled** .</span></span> <span data-ttu-id="0c665-125">當已啟用的使用者登入並完成註冊程序時，其狀態會變更為 [強制執行] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="0c665-125">When enabled users sign in and complete the registration process, their state changes to **Enforced** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0c665-126">後續步驟</span><span class="sxs-lookup"><span data-stu-id="0c665-126">Next steps</span></span>

- [<span data-ttu-id="0c665-127">將角色和權限指派給使用者</span><span class="sxs-lookup"><span data-stu-id="0c665-127">Assign roles and permissions to users</span></span>](permissions-overview.md)



