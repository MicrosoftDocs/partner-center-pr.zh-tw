---
title: 實作合作夥伴安全性需求
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何為您的使用者實作必要的安全性需求
author: LauraBrenner
ms.author: labrenne
keywords: 安全性
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133261"
---
# <a name="implement-the-partner-security-requirements"></a><span data-ttu-id="f59db-104">實作合作夥伴安全性需求</span><span class="sxs-lookup"><span data-stu-id="f59db-104">Implement the partner security requirements</span></span>

<span data-ttu-id="f59db-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="f59db-105">**Appropriate roles**</span></span>

- <span data-ttu-id="f59db-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-106">Global admin</span></span>

<span data-ttu-id="f59db-107">確保客戶及合作夥伴的安全性和隱私權是 Microsoft 最為優先的工作。</span><span class="sxs-lookup"><span data-stu-id="f59db-107">Security and privacy of customers and partners are top priorities for Microsoft.</span></span> <span data-ttu-id="f59db-108">我們持續看到更多更為複雜的安全性攻擊，這些攻擊主要與身分識別遭到入侵有關。</span><span class="sxs-lookup"><span data-stu-id="f59db-108">We continue to see an increasing number of more sophisticated security attacks, primarily related to compromised identities.</span></span> <span data-ttu-id="f59db-109">由於預防性控制項在對抗安全性攻擊的整體防禦策略中扮演重要角色，我們將會開始強制執行一組強制的安全性需求，以協助保護合作夥伴與其客戶。</span><span class="sxs-lookup"><span data-stu-id="f59db-109">As preventive controls play a key role in an overall defense strategy to thwart security attacks, we will start enforcing a set of mandatory security requirements to help protect partners and their customers.</span></span>

<span data-ttu-id="f59db-110">在本教學課程中，您將深入了解合作夥伴的安全性需求、如何滿足這些需求，以及對合作夥伴目錄中的使用者所造成的影響。</span><span class="sxs-lookup"><span data-stu-id="f59db-110">Through this tutorial you will learn more about the partner security requirements, how to fulfill them, and the impact to users in your partner directory.</span></span>

<span data-ttu-id="f59db-111">所有參與雲端解決方案提供者方案的合作夥伴、控制台廠商和 Advisor 合作夥伴，都必須針對其合作夥伴租用戶中的每位使用者強制執行多重要素驗證 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="f59db-111">All partners who are participating in the Cloud Solution Provider program, Control Panel Vendors, and Advisor partners are required to enforce Multi-Factor Authentication (MFA) for each user in their partner tenant.</span></span> <span data-ttu-id="f59db-112">這項強制執行的驗證可藉由啟用兩個 [Azure Active Directory 基準原則](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)來完成。</span><span class="sxs-lookup"><span data-stu-id="f59db-112">This enforcement can be done by enabling two [Azure Active Directory baseline policies](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).</span></span> <span data-ttu-id="f59db-113">基準原則是一組預先定義的原則，可協助組織抵禦許多常見的攻擊。</span><span class="sxs-lookup"><span data-stu-id="f59db-113">Baseline policies are a set of predefined policies that help protect organizations against many common attacks.</span></span> <span data-ttu-id="f59db-114">這些常見的攻擊可能包括密碼噴灑、重播和網路釣魚。</span><span class="sxs-lookup"><span data-stu-id="f59db-114">These common attacks can include password spray, replay, and phishing.</span></span> <span data-ttu-id="f59db-115">基準保護原則適用於所有版本的 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="f59db-115">Baseline policies are available in all editions of Azure Active Directory.</span></span> <span data-ttu-id="f59db-116">Microsoft 將這些基準保護原則提供給所有人使用的原因，是因為以身分識別為基礎的攻擊在過去幾年一直持續攀升。</span><span class="sxs-lookup"><span data-stu-id="f59db-116">Microsoft is making these baseline protection policies available to everyone because identity-based attacks have been on the rise over the last few years.</span></span>

<span data-ttu-id="f59db-117">下列程序描述啟用兩個必要基準原則的程序：</span><span class="sxs-lookup"><span data-stu-id="f59db-117">The procedures below describe the process of enabling the two necessary baseline policies:</span></span>

- <span data-ttu-id="f59db-118">**要求系統管理員使用 MFA**  啟用 [要求系統管理員使用 MFA] 原則時，將要求系統管理員角色中的使用者使用 Authenticator 應用程式來註冊使用 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-118">**Require MFA for admins**  Enabling the Require MFA for admins policy will require users in the administrator roles to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="f59db-119">完成 MFA 註冊後，管理員每次登入時都必須執行 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-119">Once MFA registration is complete, administrators will need to perform MFA every time they sign-in.</span></span>

- <span data-ttu-id="f59db-120">**使用者保護**  使用者保護是以風險為基礎的 MFA 基準原則，可保護目錄中的所有使用者。</span><span class="sxs-lookup"><span data-stu-id="f59db-120">**End user protection**  End user protection is a risk-based MFA baseline policy that protects all users in a directory.</span></span> <span data-ttu-id="f59db-121">啟用此原則會要求所有使用者都必須使用驗證器應用程式註冊 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-121">Enabling this policy requires all users to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="f59db-122">使用者可以略過 MFA 註冊提示 14 天，在這之後，他們將會遭到封鎖而無法登入，直到他們註冊 MFA 為止。</span><span class="sxs-lookup"><span data-stu-id="f59db-122">Users can ignore the MFA registration prompt for 14 days, after which they will be blocked from signing in until they register for MFA.</span></span> <span data-ttu-id="f59db-123">註冊 MFA 之後，只有在有風險的登入嘗試時，才會提示使用者進行 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-123">Once registered for MFA, users will be prompted for MFA only during risky sign-in attempts.</span></span> <span data-ttu-id="f59db-124">遭盜用的使用者帳戶會遭到封鎖，直到重設其密碼且風險事件已解除為止。</span><span class="sxs-lookup"><span data-stu-id="f59db-124">Compromised user accounts are blocked until their password is reset and risk events have been dismissed.</span></span>

<span data-ttu-id="f59db-125">啟用這些原則之後，每個使用者都能夠利用 Azure MFA 來進行驗證，而不需要額外付費。</span><span class="sxs-lookup"><span data-stu-id="f59db-125">Once these policies are enabled, each user will be able to utilize Azure MFA at no additional cost.</span></span> <span data-ttu-id="f59db-126">如果您使用第三方解決方案，則在存取 Microsoft 商業雲端服務時，您必須為每位使用者強制執行 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-126">If you are using a third-party solution, then you are required to enforce MFA for each user when accessing Microsoft Commercial cloud services.</span></span>

>[!NOTE]
><span data-ttu-id="f59db-127">由於會針對合作夥伴目錄中的每個使用者強制執行 MFA，因此會影響任何利用使用者認證的自動化或整合作業。</span><span class="sxs-lookup"><span data-stu-id="f59db-127">Since MFA will be enforced for every user in the partner directory, there will be an impact to any automation or integration that utilizes user credentials.</span></span> <span data-ttu-id="f59db-128">若要解決這種影響，您必須修改自動化或整合連線到 Microsoft 商業雲端服務的方式。</span><span class="sxs-lookup"><span data-stu-id="f59db-128">To address this impact, you will need to modify the way your automation or integration connects to Microsoft commercial cloud services.</span></span> <span data-ttu-id="f59db-129">如果您要連線的服務支援以權杖為基礎的驗證，則建議您實作[安全的應用程式模型架構](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)。</span><span class="sxs-lookup"><span data-stu-id="f59db-129">If the service you are connecting to supports token-based authentication, then it is recommended that you implement the [Secure Application Model framework](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).</span></span>

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a><span data-ttu-id="f59db-130">步驟一：封鎖任何現有的舊版驗證通訊協定</span><span class="sxs-lookup"><span data-stu-id="f59db-130">Step one: Block any existing legacy authentication protocols</span></span>

<span data-ttu-id="f59db-131">在您啟用要求系統管理員使用 MFA 和使用者保護原則之前，請確定您的使用者未使用舊版驗證通訊協定。</span><span class="sxs-lookup"><span data-stu-id="f59db-131">Before you enable the Require MFA for admins and End user protection policies, ensure that your users are not using legacy authentication protocols.</span></span> <span data-ttu-id="f59db-132">請參閱[如何：使用條件式存取封鎖 Azure AD 的舊版驗證](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use)，以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="f59db-132">See the article [How to: Block legacy authentication to Azure AD with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) for more information.</span></span>

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a><span data-ttu-id="f59db-133">步驟二：要求系統管理員使用 MFA 基準原則</span><span class="sxs-lookup"><span data-stu-id="f59db-133">Step two: Enable the Require MFA for admins baseline policy</span></span>

<span data-ttu-id="f59db-134">要求管理員使用 MFA 基準原則需要下列目錄角色的 MFA，被視為最具特殊權限的 Azure AD 角色：</span><span class="sxs-lookup"><span data-stu-id="f59db-134">The Require MFA for admin baseline policy requires MFA for the following directory roles, considered to be the most privileged Azure AD roles:</span></span>

- <span data-ttu-id="f59db-135">全域管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-135">Global administrator</span></span>
- <span data-ttu-id="f59db-136">SharePoint 管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-136">SharePoint administrator</span></span>
- <span data-ttu-id="f59db-137">Exchange 系統管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-137">Exchange administrator</span></span>
- <span data-ttu-id="f59db-138">條件式存取管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-138">Conditional access administrator</span></span>
- <span data-ttu-id="f59db-139">安全性系統管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-139">Security administrator</span></span>
- <span data-ttu-id="f59db-140">服務台管理員/密碼管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-140">Helpdesk administrator/Password administrator</span></span>
- <span data-ttu-id="f59db-141">計費管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-141">Billing administrator</span></span>
- <span data-ttu-id="f59db-142">使用者管理員</span><span class="sxs-lookup"><span data-stu-id="f59db-142">User administrator</span></span>

<span data-ttu-id="f59db-143">啟用 [要求系統管理員使用 MFA] 原則時，需要以上九個系統管理員角色，才能使用 Authenticator 應用程式來註冊使用 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-143">Upon enabling the Require MFA for admins policy, the above nine administrator roles will be required to register for MFA using the Authenticator App.</span></span> <span data-ttu-id="f59db-144">完成 MFA 註冊後，管理員每次登入時都必須執行 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-144">Once MFA registration is complete, administrators will need to perform MFA every single time they sign-in.</span></span>

<span data-ttu-id="f59db-145">如果您的組織在指令碼或程式碼中使用這些帳戶，請考慮將它們取代為 [受管理的身分識別](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)。</span><span class="sxs-lookup"><span data-stu-id="f59db-145">If your organization has these accounts in use in scripts or code, consider replacing them with [managed identities](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).</span></span>

<span data-ttu-id="f59db-146">若要啟用此原則並保護您的系統管理員：</span><span class="sxs-lookup"><span data-stu-id="f59db-146">To enable this policy and protect your administrators:</span></span>

1. <span data-ttu-id="f59db-147">以全域管理員、安全性系統管理員或條件式存取系統管理員的身分登入  **Azure 入口網站** 。</span><span class="sxs-lookup"><span data-stu-id="f59db-147">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="f59db-148">瀏覽至 [Azure Active Directory] >  [條件式存取]。</span><span class="sxs-lookup"><span data-stu-id="f59db-148">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="f59db-149">在原則清單中，選取 [基準原則:要求系統管理員使用 MFA]。</span><span class="sxs-lookup"><span data-stu-id="f59db-149">In the list of policies, select **Baseline policy: Require MFA for admins**.</span></span>

4. <span data-ttu-id="f59db-150">將 [啟用原則] 設定為 [立即使用原則]。</span><span class="sxs-lookup"><span data-stu-id="f59db-150">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="f59db-151">選取 [儲存] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="f59db-151">Select **Save**.</span></span>

<span data-ttu-id="f59db-152">當您啟用此原則之後，系統會在上述系統管理員角色的使用者登入時提示，提供額外的安全性資訊並設定行動應用程式。</span><span class="sxs-lookup"><span data-stu-id="f59db-152">Once you’ve enabled this policy, users in the above administrator roles will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="f59db-153">完成之後，他們就能夠登入適當的雲端服務。</span><span class="sxs-lookup"><span data-stu-id="f59db-153">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a><span data-ttu-id="f59db-154">步驟三：啟用使用者保護基準原則</span><span class="sxs-lookup"><span data-stu-id="f59db-154">Step three: Enable the End user protection baseline policy</span></span>

<span data-ttu-id="f59db-155">使用者保護基準原則會保護目錄中的所有使用者。</span><span class="sxs-lookup"><span data-stu-id="f59db-155">The End user protection baseline policy protects all users in a directory.</span></span> <span data-ttu-id="f59db-156">啟用此原則會要求所有使用者都必須在 14 天內註冊 Azure MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-156">Enabling this policy requires all users to register for Azure MFA within 14 days.</span></span> <span data-ttu-id="f59db-157">註冊之後，只有在有風險的登入嘗試時間，才會提示使用者進行 MFA，合作夥伴租用戶的此種行為未來將會改變。</span><span class="sxs-lookup"><span data-stu-id="f59db-157">Once registered, users will be prompted for MFA only during risky sign-in attempts, this behavior will change for partner tenants in the future.</span></span> <span data-ttu-id="f59db-158">遭盜用的使用者帳戶會遭到封鎖，直到重設密碼和風險解除為止。</span><span class="sxs-lookup"><span data-stu-id="f59db-158">Compromised user accounts are blocked until password reset and risk dismissal.</span></span>

<span data-ttu-id="f59db-159">原則 [基準原則：使用者保護] 已預先設定，當您瀏覽至 Azure 入口網站中的 [條件式存取] 刀鋒視窗時，將顯示在頂端。</span><span class="sxs-lookup"><span data-stu-id="f59db-159">The policy Baseline policy: End user protection comes pre-configured and will show up at the top when you navigate to the Conditional Access blade in Azure portal.</span></span>

<span data-ttu-id="f59db-160">若要啟用此原則並保護您的使用者：</span><span class="sxs-lookup"><span data-stu-id="f59db-160">To enable this policy and protect your users:</span></span>

1. <span data-ttu-id="f59db-161">以全域管理員、安全性系統管理員或條件式存取系統管理員的身分登入  **Azure 入口網站** 。</span><span class="sxs-lookup"><span data-stu-id="f59db-161">Sign in to the **Azure portal** as a Global Administrator, Security Administrator, or Conditional Access Administrator.</span></span>

2. <span data-ttu-id="f59db-162">瀏覽至 [Azure Active Directory] >  [條件式存取]。</span><span class="sxs-lookup"><span data-stu-id="f59db-162">Browse to **Azure Active Directory** > **Conditional Access**.</span></span>

3. <span data-ttu-id="f59db-163">在原則清單中，選取 [基準原則:終端使用者保護 (預覽)]。</span><span class="sxs-lookup"><span data-stu-id="f59db-163">In the list of policies, select **Baseline policy: End user protection (preview)**.</span></span>

4. <span data-ttu-id="f59db-164">將 [啟用原則] 設定為 [立即使用原則]。</span><span class="sxs-lookup"><span data-stu-id="f59db-164">Set **Enable policy** to **Use policy immediately**.</span></span>

5. <span data-ttu-id="f59db-165">選取 [儲存] \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="f59db-165">Select **Save**.</span></span>

<span data-ttu-id="f59db-166">當您啟用此原則之後，系統會在所有使用者登入時提示，提供額外的安全性資訊並設定行動應用程式。</span><span class="sxs-lookup"><span data-stu-id="f59db-166">Once you’ve enabled this policy, all users will be prompted on sign-in to provide additional security information and configure the mobile app.</span></span> <span data-ttu-id="f59db-167">完成之後，他們就能夠登入適當的雲端服務。</span><span class="sxs-lookup"><span data-stu-id="f59db-167">Once this is complete, they’ll be able to sign in to the appropriate cloud service.</span></span>

>[!NOTE]
><span data-ttu-id="f59db-168">在強制執行合作夥伴安全性需求之前，系統只會根據風險提示不受 [要求系統管理員使用 MFA] 基準原則限制的使用者進行 MFA。</span><span class="sxs-lookup"><span data-stu-id="f59db-168">Until the partner security requirements are enforced, users who are not covered by the Require MFA for admins baseline policy will only be prompted for MFA based on risk.</span></span>