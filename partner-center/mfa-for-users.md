---
title: 使用多重要素驗證來設定您的使用者
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何使用 MFA 為員工進行設定
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578283"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="bffb5-103">使用多重要素驗證來設定您的使用者</span><span class="sxs-lookup"><span data-stu-id="bffb5-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="bffb5-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="bffb5-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bffb5-105">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="bffb5-105">Global admin</span></span>

<span data-ttu-id="bffb5-106">較高的隱私權保護和安全性是我們最優先的考量。</span><span class="sxs-lookup"><span data-stu-id="bffb5-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="bffb5-107">我們知道最佳的防禦是預防，而且我們只與最弱的連結一樣強大。</span><span class="sxs-lookup"><span data-stu-id="bffb5-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="bffb5-108">這就是為什麼我們需要生態系統中的每個人都採取行動，並確保具備適當的安全性保護。</span><span class="sxs-lookup"><span data-stu-id="bffb5-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="bffb5-109">我們強烈建議所有合作夥伴在其合作夥伴租用戶中為其使用者啟用多重要素驗證 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="bffb5-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="bffb5-110">為使用者新增多重要素驗證</span><span class="sxs-lookup"><span data-stu-id="bffb5-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="bffb5-111">您必須是公司的全域管理員才能完成這項工作。</span><span class="sxs-lookup"><span data-stu-id="bffb5-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="bffb5-112">若要為使用者啟用 MFA，最簡單的方法是在將使用者新增至 Azure AD 租用戶時進行。</span><span class="sxs-lookup"><span data-stu-id="bffb5-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="bffb5-113">登入 [Azure 入口網站](https://portal.azure.com)，然後移至 [使用者管理]。</span><span class="sxs-lookup"><span data-stu-id="bffb5-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="bffb5-114">選取 [多重要素驗證]。</span><span class="sxs-lookup"><span data-stu-id="bffb5-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="bffb5-115">選取您想要啟用的使用者，然後選取 [啟用]。</span><span class="sxs-lookup"><span data-stu-id="bffb5-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="bffb5-116">這會為這名使用者啟用 MFA。</span><span class="sxs-lookup"><span data-stu-id="bffb5-116">This will enable MFA for this user.</span></span> <span data-ttu-id="bffb5-117">[已啟用] 表示系統會要求使用者在第一次登入時設定其 MFA 驗證。</span><span class="sxs-lookup"><span data-stu-id="bffb5-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="bffb5-118">之後在登入時，系統就會要求其提供透過電子郵件或簡訊 (視其設定而定) 所收到的驗證碼。</span><span class="sxs-lookup"><span data-stu-id="bffb5-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何驗證":::

>[!NOTE]
><span data-ttu-id="bffb5-120">您可以使用上述相同步驟，並選取 [強制執行] 來 **強制** 使用者使用 MFA。</span><span class="sxs-lookup"><span data-stu-id="bffb5-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="bffb5-121">若要深入了解，請閱讀[啟用每一使用者 Azure Multi-Factor Authentication 以保護登入事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)。</span><span class="sxs-lookup"><span data-stu-id="bffb5-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="bffb5-122">所有使用者都會從 [已停用] \*\*\*\* 開始。</span><span class="sxs-lookup"><span data-stu-id="bffb5-122">All users start out **Disabled**.</span></span> <span data-ttu-id="bffb5-123">當您以每一使用者 Azure Multi-Factor Authentication 註冊使用者時，其狀態會變更為 [已啟用] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="bffb5-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="bffb5-124">當已啟用的使用者登入並完成註冊程序時，其狀態會變更為 [強制執行] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="bffb5-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="bffb5-125">後續步驟</span><span class="sxs-lookup"><span data-stu-id="bffb5-125">Next steps</span></span>

- [<span data-ttu-id="bffb5-126">將角色和權限指派給使用者</span><span class="sxs-lookup"><span data-stu-id="bffb5-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

