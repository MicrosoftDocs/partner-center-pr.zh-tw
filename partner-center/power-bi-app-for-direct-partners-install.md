---
title: 安裝適用于 Power BI 的合作夥伴中心分析
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 請遵循本文中的步驟，安裝及預覽適用于 Power BI 的合作夥伴中心分析應用程式（適用于 CSP 中的直接合作夥伴）。
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 36efc58198be67181ed448d90db505889c3070d4
ms.sourcegitcommit: b81cde2d62e096e58ac3ce12fc9c35a97d10d51f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/18/2020
ms.locfileid: "85072414"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="01695-103">安裝和預覽適用於 Microsoft Power BI 的合作夥伴中心分析應用程式</span><span class="sxs-lookup"><span data-stu-id="01695-103">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="01695-104">**適用於**</span><span class="sxs-lookup"><span data-stu-id="01695-104">**Applies to**</span></span>

- <span data-ttu-id="01695-105">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="01695-105">Partner Center</span></span>

<span data-ttu-id="01695-106">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="01695-106">**Appropriate roles**</span></span>
-   <span data-ttu-id="01695-107">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="01695-107">Global admin</span></span>
-   <span data-ttu-id="01695-108">使用者系統管理員</span><span class="sxs-lookup"><span data-stu-id="01695-108">User admin</span></span>
-   <span data-ttu-id="01695-109">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="01695-109">Sales agent</span></span>
-   <span data-ttu-id="01695-110">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="01695-110">Admin agent</span></span>

## <a name="before-you-begin"></a><span data-ttu-id="01695-111">開始之前</span><span class="sxs-lookup"><span data-stu-id="01695-111">Before you begin</span></span>

<span data-ttu-id="01695-112">從下列可用的 Power BI 應用程式清單中，選取與您的公司最相關的應用程式：</span><span class="sxs-lookup"><span data-stu-id="01695-112">Select the application that is most relevant to your business from the following list of available Power BI apps:</span></span>
- [<span data-ttu-id="01695-113">直接提供者</span><span class="sxs-lookup"><span data-stu-id="01695-113">Direct Provider</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [<span data-ttu-id="01695-114">間接提供者</span><span class="sxs-lookup"><span data-stu-id="01695-114">Indirect Provider</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [<span data-ttu-id="01695-115">間接轉銷商</span><span class="sxs-lookup"><span data-stu-id="01695-115">Indirect Reseller</span></span>](https://appsource.microsoft.com/en-us/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

<span data-ttu-id="01695-116">安裝合作夥伴中心分析應用程式預覽版之前，請先確定您符合下列需求。</span><span class="sxs-lookup"><span data-stu-id="01695-116">Before you install the Partner Center Analytics app preview version, be sure that you meet the following requirements.</span></span>

- <span data-ttu-id="01695-117">您可以為您的企業挑選正確的 Power BI 應用程式。</span><span class="sxs-lookup"><span data-stu-id="01695-117">You pick the correct Power BI app for your business.</span></span>

- <span data-ttu-id="01695-118">您有 Power BI pro 授權。</span><span class="sxs-lookup"><span data-stu-id="01695-118">You have a Power BI pro license.</span></span>

- <span data-ttu-id="01695-119">您有權在您的租使用者上安裝範本應用程式。</span><span class="sxs-lookup"><span data-stu-id="01695-119">You have permissions to install template apps on your tenant.</span></span>

- <span data-ttu-id="01695-120">您可以登入 Power BI。</span><span class="sxs-lookup"><span data-stu-id="01695-120">You can sign in to Power BI.</span></span>

- <span data-ttu-id="01695-121">您可以在[公司的 Azure Active Directory （Azure AD）租](azure-active-directory-tenants-and-partner-center.md)使用者中，以全域管理員、系統管理員代理程式或計費管理員身分登入。</span><span class="sxs-lookup"><span data-stu-id="01695-121">You can sign in as a global admin, admin agent, or billing admin to [your company's Azure Active Directory (Azure AD) tenant](azure-active-directory-tenants-and-partner-center.md).</span></span>

## <a name="to-install-the-app"></a><span data-ttu-id="01695-122">若要安裝應用程式</span><span class="sxs-lookup"><span data-stu-id="01695-122">To install the app</span></span>

1. <span data-ttu-id="01695-123">在上一節中，按一下指定的應用程式來源連結（直接提供者/間接提供者/間接轉銷商）。</span><span class="sxs-lookup"><span data-stu-id="01695-123">Click on the app source link given (Direct Provider/Indirect Provider/Indirect Reseller) in the above section.</span></span>

2. <span data-ttu-id="01695-124">按一下 [**立即取得**]。</span><span class="sxs-lookup"><span data-stu-id="01695-124">Click on **GET IT NOW**.</span></span> 

3. <span data-ttu-id="01695-125">按一下 [**繼續**] 以同意條款及條件。</span><span class="sxs-lookup"><span data-stu-id="01695-125">Agree terms and conditions by clicking **Continue**.</span></span>

4. <span data-ttu-id="01695-126">在 \[已經有帳戶名稱了嗎?\] 下方選取 **\[登入\]**。</span><span class="sxs-lookup"><span data-stu-id="01695-126">Under Already have an account? select **Sign In**.</span></span>

5. <span data-ttu-id="01695-127">在下一個頁面上，輸入您的 Power BI 的使用者名稱和密碼，然後選取 \[登入\]。</span><span class="sxs-lookup"><span data-stu-id="01695-127">On the next page, enter your Power BI user name and password and then select Sign In.</span></span>

6. <span data-ttu-id="01695-128">藉由提供工作區名稱來安裝工作區。</span><span class="sxs-lookup"><span data-stu-id="01695-128">Install the workspace by providing the workspace name.</span></span>

7. <span data-ttu-id="01695-129">您可以在 [應用程式] 區段中找到已安裝的範本應用程式。</span><span class="sxs-lookup"><span data-stu-id="01695-129">You can find the template apps installed under Apps Section.</span></span>

8. <span data-ttu-id="01695-130">按一下 [應用程式]，然後選擇已安裝的應用程式。</span><span class="sxs-lookup"><span data-stu-id="01695-130">Click on Apps and choose the installed apps.</span></span>

9. <span data-ttu-id="01695-131">開始使用新的應用程式畫面隨即開啟。</span><span class="sxs-lookup"><span data-stu-id="01695-131">Get Started with your new app screen opens.</span></span>

10. <span data-ttu-id="01695-132">若要連接到資料，請按一下 **[連接]**。</span><span class="sxs-lookup"><span data-stu-id="01695-132">To connect to the data Click **Connect**.</span></span>

11. <span data-ttu-id="01695-133">在 [連線**到合作夥伴中心分析**] 快顯視窗中，確認 [**驗證方法**] 已設定為 [ **oAuth2** ]，或從清單中選取 [ **oAuth2** ] （如果不是）。</span><span class="sxs-lookup"><span data-stu-id="01695-133">On the **Connect to Partner Center Analytics** pop-up window, verify that the **Authentication method** is set to **oAuth2** or select **oAuth2** from the list if it's not.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="01695-134">這個視窗可能需要幾分鐘才會出現。</span><span class="sxs-lookup"><span data-stu-id="01695-134">This window may take a few minutes to appear.</span></span>

12. <span data-ttu-id="01695-135">在 [**合作夥伴中心分析連接器**] 頁面上，使用全域管理員、系統管理員代理程式或貴公司 Azure AD 租使用者的計費管理員認證登入，然後選取 [登**入**]。</span><span class="sxs-lookup"><span data-stu-id="01695-135">On the **Partner Center Analytics Connector** page, sign in with global admin, admin agent, or billing admin credentials for your company's Azure AD tenant, and then select **Sign In**.</span></span>
 
13. <span data-ttu-id="01695-136">出現存取權提示時，選取 **\[接受\]**。</span><span class="sxs-lookup"><span data-stu-id="01695-136">When prompted for access, select **Accept**.</span></span> 

<span data-ttu-id="01695-137">將合作夥伴中心分析服務連線到 Power BI 後，資料將會開始載入。</span><span class="sxs-lookup"><span data-stu-id="01695-137">Once the Partner Center Analytics service is connected to Power BI, data will begin to load.</span></span> <span data-ttu-id="01695-138">視資料數量而定，這最多可能需要花費 10 分鐘。</span><span class="sxs-lookup"><span data-stu-id="01695-138">Depending on the amount of data, this can take up to 10 minutes.</span></span> 

<span data-ttu-id="01695-139">資料完成載入後，您可以開始在 Power BI 中使用合作夥伴中心分析應用程式儀表板和報告。</span><span class="sxs-lookup"><span data-stu-id="01695-139">After the data finishes loading, you can start using the Partner Center Analytics app dashboard and reports in Power BI.</span></span>

## <a name="next-steps"></a><span data-ttu-id="01695-140">後續步驟</span><span class="sxs-lookup"><span data-stu-id="01695-140">Next steps</span></span>

[<span data-ttu-id="01695-141">使用適用於 Microsoft Power BI 的合作夥伴中心分析應用程式來檢視業務資料</span><span class="sxs-lookup"><span data-stu-id="01695-141">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-use.md)
