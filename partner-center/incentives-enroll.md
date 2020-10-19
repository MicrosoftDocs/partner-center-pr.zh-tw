---
title: 獎勵註冊
ms.topic: how-to
ms.date: 09/25/2020
description: 註冊獎勵方案，並為使用者管理指派必要的角色。 本文說明註冊程式。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 067ad9370da6a6deeaeac7b24e606fe0bcd555a9
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175194"
---
# <a name="enrollment-and-user-management-in-the-incentives-program"></a><span data-ttu-id="4e010-104">獎勵計畫中的註冊和使用者管理</span><span class="sxs-lookup"><span data-stu-id="4e010-104">Enrollment and user management in the incentives program</span></span>

<span data-ttu-id="4e010-105">**適用於：**</span><span class="sxs-lookup"><span data-stu-id="4e010-105">**Applies to:**</span></span>

- <span data-ttu-id="4e010-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="4e010-106">Partner Center</span></span>

<span data-ttu-id="4e010-107">**適當的角色：**</span><span class="sxs-lookup"><span data-stu-id="4e010-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="4e010-108">獎勵管理員</span><span class="sxs-lookup"><span data-stu-id="4e010-108">Incentives admin</span></span>

>[!NOTE]
><span data-ttu-id="4e010-109">在您可以註冊獎勵計畫之前，您必須先完成合作夥伴中心 [遷移](prepare-pmc-pc-migration.md)的 Partner Membership Center。</span><span class="sxs-lookup"><span data-stu-id="4e010-109">Before you can enroll in the incentives program you must have completed the Partner Membership Center to Partner Center [migration](prepare-pmc-pc-migration.md).</span></span>

<span data-ttu-id="4e010-110">註冊程式是由兩個步驟所組成。</span><span class="sxs-lookup"><span data-stu-id="4e010-110">The enrollment process consists of two steps.</span></span>

<span data-ttu-id="4e010-111">**步驟1。使用者管理：** 此步驟牽涉到在合作夥伴中心中建立獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4e010-111">**Step 1. User management:** This step involves establishing the Incentive Administrator in Partner Center.</span></span>

<span data-ttu-id="4e010-112">**步驟2。註冊：** Microsoft 會將邀請傳送給您，以在您的獎勵計畫中註冊。</span><span class="sxs-lookup"><span data-stu-id="4e010-112">**Step 2. Enrollment:** Microsoft sends you an invitation to enroll in your incentive program.</span></span>

## <a name="user-management"></a><span data-ttu-id="4e010-113">使用者管理</span><span class="sxs-lookup"><span data-stu-id="4e010-113">User Management</span></span>

<span data-ttu-id="4e010-114">若要註冊合作夥伴中心獎勵方案，全域管理員或帳戶管理員必須將您的公司使用者設定為獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4e010-114">To enroll in a Partner Center incentive program, the Global Administrator or Account Administrator needs to set up your company users as Incentive Administrators.</span></span> <span data-ttu-id="4e010-115">如需夥伴帳戶、角色和許可權的相關資訊，請參閱 [管理您的合作夥伴中心帳戶](partner-center-account-setup.md)。</span><span class="sxs-lookup"><span data-stu-id="4e010-115">For information on partner accounts, roles, and permissions, see [Manage your Partner Center account](partner-center-account-setup.md).</span></span> <span data-ttu-id="4e010-116">全域管理員也可以透過 Azure Active Directory (Azure AD) 來設定您的公司使用者。</span><span class="sxs-lookup"><span data-stu-id="4e010-116">The Global Administrator can also set up your company users through the Azure Active Directory (Azure AD).</span></span>

<span data-ttu-id="4e010-117">當您的組織符合獎勵資格之後，Microsoft 會將邀請傳送給帳戶管理員和獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4e010-117">Once your organization is eligible for incentives, Microsoft will send invitations to the Account Administrator and the Incentive Administrator.</span></span>

>[!NOTE]
><span data-ttu-id="4e010-118">只有獎勵系統管理員可以在獎勵計畫中註冊。</span><span class="sxs-lookup"><span data-stu-id="4e010-118">Only the Incentive Administrator can enroll in incentive programs.</span></span> <span data-ttu-id="4e010-119">如果您的地點沒有任何獎勵系統管理員，則全域管理員和帳戶管理員必須指派一個。</span><span class="sxs-lookup"><span data-stu-id="4e010-119">If there is no Incentive Administrator for your location, the Global Administrator and Account Administrator must assign one.</span></span> <span data-ttu-id="4e010-120">您必須為位置 MPN 識別碼指派獎勵系統管理員。</span><span class="sxs-lookup"><span data-stu-id="4e010-120">The Incentive Administrator must be assigned for the location MPN IDs.</span></span> <span data-ttu-id="4e010-121">全域管理員或帳戶管理員也可以指派為「獎勵管理員」。</span><span class="sxs-lookup"><span data-stu-id="4e010-121">The Global Administrator or Account Administrator can also be assigned as the Incentive Administrator.</span></span>

## <a name="enrollment-process"></a><span data-ttu-id="4e010-122">註冊程式</span><span class="sxs-lookup"><span data-stu-id="4e010-122">Enrollment Process</span></span>

<span data-ttu-id="4e010-123">當您的組織符合獎勵資格之後，Microsoft 會將邀請傳送給合格 MPNLocationID 的獎勵系統管理員，以開始進行註冊程式。</span><span class="sxs-lookup"><span data-stu-id="4e010-123">Once your organization is eligible for incentives, Microsoft will send an invitation to the Incentives Administrator of the eligible MPNLocationID to begin the enrollment process.</span></span> <span data-ttu-id="4e010-124">這封電子郵件將會從 **Microsoft 合作夥伴中心**傳送，且將會有主旨 **合作夥伴獎勵註冊邀請**。</span><span class="sxs-lookup"><span data-stu-id="4e010-124">This email will be sent from **Microsoft Partner Center**, and will have the subject **Partner Incentive Enrollment Invitation**.</span></span> <span data-ttu-id="4e010-125">開啟邀請，然後選取 [ **開始**]。</span><span class="sxs-lookup"><span data-stu-id="4e010-125">Open the invitation and select **Get Started**.</span></span>

<span data-ttu-id="4e010-126">您也會在合作夥伴中心首頁上看到邀請。</span><span class="sxs-lookup"><span data-stu-id="4e010-126">You’ll also see an invitation on the Partner Center home page.</span></span> <span data-ttu-id="4e010-127">一旦您選取該訊息之後，就無法再看到它。</span><span class="sxs-lookup"><span data-stu-id="4e010-127">Once you select that message, you won’t be able to see it again.</span></span> <span data-ttu-id="4e010-128">不過，獎勵系統管理員仍可登入 [合作夥伴中心儀表板](https://partner.microsoft.com/dashboard/) ，並選取 [ **使用者管理**]，以啟動此程式。</span><span class="sxs-lookup"><span data-stu-id="4e010-128">However, the Incentives Administrator can still start the process by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) and selecting **User Management**.</span></span>

<span data-ttu-id="4e010-129">某些獎勵方案沒有任何符合資格的條件，而且會開放給所有合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="4e010-129">Certain incentive programs have no eligibility criteria, and are open to all partners.</span></span> <span data-ttu-id="4e010-130">獎勵系統管理員會在 [獎勵總覽] 頁面上看到這些計畫的邀請，前提是他們有相關獎勵計畫和 MPN 的許可權。</span><span class="sxs-lookup"><span data-stu-id="4e010-130">The Incentive Administrator will see invitations for these programs on the incentive overview page, provided they have permissions for the relevant incentive program and MPN.</span></span> <span data-ttu-id="4e010-131">Microsoft 不會為這些程式傳送電子郵件邀請。</span><span class="sxs-lookup"><span data-stu-id="4e010-131">Microsoft does not send email invitations for these programs.</span></span>

<span data-ttu-id="4e010-132">如需註冊程式的詳細資訊，請下載 [獎勵註冊指南](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) ， (登入所需的) 。</span><span class="sxs-lookup"><span data-stu-id="4e010-132">For more information on the enrollment process, download the [Incentives Enrollment Guide](https://partner.microsoft.com/resources/detail/partner-center-incentives-enrollment-pdf) (sign-in required).</span></span>

## <a name="expiration-and-renewal"></a><span data-ttu-id="4e010-133">到期和續約</span><span class="sxs-lookup"><span data-stu-id="4e010-133">Expiration and renewal</span></span>

<span data-ttu-id="4e010-134">獎勵註冊會在會計年度結束時到期。</span><span class="sxs-lookup"><span data-stu-id="4e010-134">Incentives enrollment expires at the end of the fiscal year.</span></span> <span data-ttu-id="4e010-135">不過，只要您保持具有有效合約的合格合作夥伴，Microsoft 就會將您的獎勵註冊向前復原到下一個會計年度。</span><span class="sxs-lookup"><span data-stu-id="4e010-135">However, as long as you remain an eligible partner with an active agreement, Microsoft will roll forward your incentives enrollment into the next fiscal year.</span></span> <span data-ttu-id="4e010-136">您不需要採取任何動作。</span><span class="sxs-lookup"><span data-stu-id="4e010-136">You don't need to take any action.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4e010-137">後續步驟</span><span class="sxs-lookup"><span data-stu-id="4e010-137">Next steps</span></span>

- [<span data-ttu-id="4e010-138">判斷您的計劃資格</span><span class="sxs-lookup"><span data-stu-id="4e010-138">Determine your program eligibility</span></span>](incentives-determined-your-program-eligibility.md)
