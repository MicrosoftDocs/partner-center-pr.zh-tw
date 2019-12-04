---
title: 使用 Windows Autopilot 設定檔自訂裝置的全新體驗 |合作夥伴中心
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 瞭解如何在您將裝置傳遞給客戶之前，使用 Autopilot 設定檔自訂或預先設定新裝置的全新體驗。
author: maggiepuccievans
ms.author: evansma
keywords: autopilot，windows autopilot，microsoft autopilot，零接觸部署，oobe，登入畫面，現成的
ms.localizationpriority: medium
ms.openlocfilehash: 16653865ff251bcf73dcd79c4948d3326bcc0fab
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721430"
---
# <a name="customize-the-out-of-box-experience-for-a-device-with-windows-autopilot-profiles"></a><span data-ttu-id="18059-104">使用 Windows Autopilot 設定檔自訂裝置的全新體驗</span><span class="sxs-lookup"><span data-stu-id="18059-104">Customize the out-of-box experience for a device with Windows Autopilot profiles</span></span>

<span data-ttu-id="18059-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="18059-105">**Applies to**</span></span>

- <span data-ttu-id="18059-106">CSP 直接帳單合作夥伴、間接提供者和間接轉銷商</span><span class="sxs-lookup"><span data-stu-id="18059-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="18059-107">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="18059-107">**Appropriate roles**</span></span>

- <span data-ttu-id="18059-108">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="18059-108">Admin agent</span></span>
- <span data-ttu-id="18059-109">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="18059-109">Global admin</span></span>
- <span data-ttu-id="18059-110">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="18059-110">Sales agent</span></span>
- <span data-ttu-id="18059-111">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="18059-111">User management admin</span></span>

<span data-ttu-id="18059-112">如果您管理客戶裝置，您可能需要針對客戶的使用者自訂全新體驗（OOBE）。</span><span class="sxs-lookup"><span data-stu-id="18059-112">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="18059-113">您可以先使用 Windows Autopilot 設定檔預先設定新的裝置，再將裝置傳遞給客戶，並將新的設定檔套用至客戶已購買的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-113">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="18059-114">請注意，Oem 已開始在 [Autopilot 裝置] 方塊外部加入出貨標籤，以顯示裝置的**產品金鑰識別碼（PKID）** 。</span><span class="sxs-lookup"><span data-stu-id="18059-114">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="18059-115">這個一維、可讀取的條碼提供下游合作夥伴一種方式來註冊裝置以進行 Autopilot，而不需要將裝置取消裝箱，並以替代方式收集裝置識別碼。</span><span class="sxs-lookup"><span data-stu-id="18059-115">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="18059-116">本文說明如何建立 Autopilot 設定檔，並將其套用至合作夥伴中心內的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-116">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="18059-117">如果您還不熟悉 Autopilot，請參閱下列文章中的資訊：</span><span class="sxs-lookup"><span data-stu-id="18059-117">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="18059-118">Windows Autopilot 概觀</span><span class="sxs-lookup"><span data-stu-id="18059-118">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="18059-119">Autopilot 部署參考指南</span><span class="sxs-lookup"><span data-stu-id="18059-119">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="18059-120">概觀</span><span class="sxs-lookup"><span data-stu-id="18059-120">Overview</span></span>

<span data-ttu-id="18059-121">透過合作夥伴中心的 Windows Autopilot 功能，您可以建立自訂設定檔，以套用至客戶裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-121">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="18059-122">發行本文時，可以使用下列設定檔設定：</span><span class="sxs-lookup"><span data-stu-id="18059-122">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="18059-123">略過隱私權設定。</span><span class="sxs-lookup"><span data-stu-id="18059-123">Skip privacy settings.</span></span> <span data-ttu-id="18059-124">這個選擇性的 Autopilot 設定檔設定可讓組織不會在 OOBE 程式期間詢問隱私權設定。</span><span class="sxs-lookup"><span data-stu-id="18059-124">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="18059-125">停用裝置上的本機系統管理員帳戶建立。</span><span class="sxs-lookup"><span data-stu-id="18059-125">Disable local admin account creation on the device.</span></span> <span data-ttu-id="18059-126">組織可以決定在程式完成後，設定裝置的使用者是否應該具有系統管理員存取權。</span><span class="sxs-lookup"><span data-stu-id="18059-126">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="18059-127">自動設定適用于公司或學校的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-127">Automatically set up device for work or school.</span></span> <span data-ttu-id="18059-128">向 Autopilot 註冊的所有裝置都會自動視為公司或學校的裝置，因此不會在 OOBE 程式期間詢問此問題。</span><span class="sxs-lookup"><span data-stu-id="18059-128">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="18059-129">略過 Cortana、OneDrive 和 OEM 註冊設定頁面。</span><span class="sxs-lookup"><span data-stu-id="18059-129">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="18059-130">向 Autopilot 註冊的所有裝置都會在全新體驗（OOBE）程式期間自動略過這些頁面。</span><span class="sxs-lookup"><span data-stu-id="18059-130">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="18059-131">略過使用者授權合約（EULA）。</span><span class="sxs-lookup"><span data-stu-id="18059-131">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="18059-132">從 Windows 10 1709 版開始，組織可以決定略過在 OOBE 程式中顯示的 EULA 頁面。</span><span class="sxs-lookup"><span data-stu-id="18059-132">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="18059-133">請參閱下面的 [Windows AUTOPILOT EULA 關閉](#windows-autopilot-eula-dismissal)，以取得在 Windows 安裝期間略過 EULA 頁面的重要資訊。</span><span class="sxs-lookup"><span data-stu-id="18059-133">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="18059-134">以下是適用的設定檔和裝置管理許可權和限制：</span><span class="sxs-lookup"><span data-stu-id="18059-134">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="18059-135">CSP 合作夥伴可以繼續管理具有轉售商關係之現有客戶的 Autopilot 設定檔，即使客戶已移除合作夥伴的委派系統管理許可權也一樣。</span><span class="sxs-lookup"><span data-stu-id="18059-135">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="18059-136">您可以為已新增的客戶管理現有的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-136">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="18059-137">您無法管理客戶已上傳至 Microsoft Store for Business 或 Microsoft Intune 入口網站的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-137">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="18059-138">在合作夥伴中心建立和管理 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="18059-138">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="18059-139">在合作夥伴中心，您可以建立 Windows Autopilot 部署設定檔，並將其套用至裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-139">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="18059-140">只有系統管理員代理程式可以建立和套用設定檔。</span><span class="sxs-lookup"><span data-stu-id="18059-140">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="18059-141">建立新的 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="18059-141">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="18059-142">從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您要為其建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="18059-142">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="18059-143">在客戶的詳細資料頁面上，選取 [**裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-143">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="18059-144">在 [ **Windows Autopilot 設定檔**] 底下，選取 [**新增設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="18059-144">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="18059-145">輸入設定檔的 [名稱] 和 [描述]，然後設定 OOBE 設定。</span><span class="sxs-lookup"><span data-stu-id="18059-145">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="18059-146">選擇：</span><span class="sxs-lookup"><span data-stu-id="18059-146">Choose from:</span></span>  

   - <span data-ttu-id="18059-147">在安裝程式中略過隱私權設定</span><span class="sxs-lookup"><span data-stu-id="18059-147">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="18059-148">停用設定中的本機系統管理員帳戶</span><span class="sxs-lookup"><span data-stu-id="18059-148">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="18059-149">自動略過設定中的頁面</span><span class="sxs-lookup"><span data-stu-id="18059-149">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="18059-150">（包括*自動選取公司或學校的設定*，以及*略過 Cortana、OneDrive 和 OEM 註冊設定頁面*）</span><span class="sxs-lookup"><span data-stu-id="18059-150">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="18059-151">略過使用者授權合約（EULA）</span><span class="sxs-lookup"><span data-stu-id="18059-151">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="18059-152">請參閱下面的 [Windows AUTOPILOT EULA 關閉](#windows-autopilot-eula-dismissal)，以取得在 Windows 安裝期間略過 EULA 頁面的重要資訊。</span><span class="sxs-lookup"><span data-stu-id="18059-152">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="18059-153">完成時選取 **\[提交\]** 。</span><span class="sxs-lookup"><span data-stu-id="18059-153">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="18059-154">將 Autopilot 設定檔套用至客戶裝置</span><span class="sxs-lookup"><span data-stu-id="18059-154">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="18059-155">下列指示假設您已將客戶的裝置新增至合作夥伴中心，而且您可以存取其裝置清單。</span><span class="sxs-lookup"><span data-stu-id="18059-155">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="18059-156">如果您尚未新增客戶的裝置，請遵循[將裝置新增至客戶的帳戶](#add-devices-to-a-customers-account)中的指示，然後遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="18059-156">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="18059-157">為客戶建立 Autopilot 設定檔之後，您可以將它套用至客戶的裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-157">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="18059-158">從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="18059-158">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="18059-159">在客戶的詳細資料頁面上，選取 [**裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-159">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="18059-160">在 [**將設定檔套用至裝置**] 下，選取您想要新增設定檔的裝置或裝置群組，然後選取 [套用**設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="18059-160">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="18059-161">您剛才套用的設定檔會出現在 [**設定檔**] 資料行中。</span><span class="sxs-lookup"><span data-stu-id="18059-161">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="18059-162">請遵循下列步驟來確認設定檔將會成功套用至裝置。</span><span class="sxs-lookup"><span data-stu-id="18059-162">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="18059-163">a.</span><span class="sxs-lookup"><span data-stu-id="18059-163">a.</span></span>  <span data-ttu-id="18059-164">將裝置連線到網路，並將它開啟。</span><span class="sxs-lookup"><span data-stu-id="18059-164">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="18059-165">b。</span><span class="sxs-lookup"><span data-stu-id="18059-165">b.</span></span>  <span data-ttu-id="18059-166">確認是否會顯示適當的 OOBE 畫面 (如果有的話)。</span><span class="sxs-lookup"><span data-stu-id="18059-166">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="18059-167">c.</span><span class="sxs-lookup"><span data-stu-id="18059-167">c.</span></span>  <span data-ttu-id="18059-168">當 OOBE 程式停止時，將裝置重設為其原廠預設值，為新的使用者準備它。</span><span class="sxs-lookup"><span data-stu-id="18059-168">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="18059-169">從客戶的裝置移除 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="18059-169">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="18059-170">從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="18059-170">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="18059-171">在客戶的詳細資料頁面上，選取 [**裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-171">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="18059-172">在 [**將設定檔套用至裝置**] 下，選取您想要移除設定檔的裝置，然後選取 [**移除設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="18059-172">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="18059-173">從裝置移除設定檔並不會刪除清單中的設定檔。</span><span class="sxs-lookup"><span data-stu-id="18059-173">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="18059-174">如果您想要刪除設定檔，請依照[更新或刪除 Autopilot 設定檔](#update-or-delete-an-autopilot-profile)中的指示進行。</span><span class="sxs-lookup"><span data-stu-id="18059-174">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="18059-175">更新或刪除 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="18059-175">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="18059-176">若客戶想要在您將裝置寄送給他們之後變更全新體驗，您可以在 [合作夥伴中心] 中變更設定檔。</span><span class="sxs-lookup"><span data-stu-id="18059-176">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="18059-177">當客戶的裝置連線到網際網路時，它會在 OOBE 程式中下載最新的設定檔版本。</span><span class="sxs-lookup"><span data-stu-id="18059-177">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="18059-178">此外，當客戶將裝置還原為其出廠預設值時，裝置會在 OOBE 程式中再次下載最新的設定檔版本。</span><span class="sxs-lookup"><span data-stu-id="18059-178">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="18059-179">從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取想要變更 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="18059-179">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="18059-180">在客戶的詳細資料頁面上，選取 [**裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-180">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="18059-181">在 [ **Windows Autopilot 設定檔**] 下，選取您需要更新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="18059-181">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="18059-182">進行必要的變更，然後選取 [**提交**]。</span><span class="sxs-lookup"><span data-stu-id="18059-182">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="18059-183">若要刪除此設定檔，請選取頁面右上角的 [**刪除設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="18059-183">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="18059-184">將裝置新增至客戶的帳戶</span><span class="sxs-lookup"><span data-stu-id="18059-184">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="18059-185">「銷售代理程式」和「管理員」代理程式可以將裝置新增至客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="18059-185">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="18059-186">在您可以將自訂 Autopilot 設定檔套用至客戶裝置之前，您必須能夠存取客戶的裝置清單。</span><span class="sxs-lookup"><span data-stu-id="18059-186">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="18059-187">如果您打算使用 OEM 名稱、序號和型號組合，請注意下列限制：</span><span class="sxs-lookup"><span data-stu-id="18059-187">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="18059-188">這個元組僅適用于較新的裝置（例如4k 雜湊），不支援128b 雜湊（RS2 和先前的裝置）。</span><span class="sxs-lookup"><span data-stu-id="18059-188">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="18059-189">元組註冊會區分大小寫，因此檔案中的資料必須與 OEM 提供者（硬體提供者）所提供的***完全***相符。</span><span class="sxs-lookup"><span data-stu-id="18059-189">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="18059-190">請依照下列指示，將裝置新增至合作夥伴中心內的客戶帳戶。</span><span class="sxs-lookup"><span data-stu-id="18059-190">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="18059-191">從 [合作夥伴中心] 功能表選取 [**客戶**]，然後選取您要管理其裝置的客戶。</span><span class="sxs-lookup"><span data-stu-id="18059-191">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="18059-192">在客戶的詳細資料頁面上，選取 [**裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-192">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="18059-193">在 [**將設定檔套用至裝置**] 下，選取 [**新增裝置**]。</span><span class="sxs-lookup"><span data-stu-id="18059-193">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="18059-194">輸入裝置清單的名稱，然後選取 **[流覽]** ，將客戶的清單（以 .csv 檔案格式）上傳至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="18059-194">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="18059-195">您應該已收到您的裝置購買的此 .csv 檔案。</span><span class="sxs-lookup"><span data-stu-id="18059-195">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="18059-196">如果您未收到 .csv 檔案，您可以遵循[將裝置新增至 Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步驟，自行建立一個。</span><span class="sxs-lookup"><span data-stu-id="18059-196">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="18059-197">上傳 .csv 檔案，然後選取 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="18059-197">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="18059-198">如果您在嘗試上傳 .csv 檔案時收到錯誤訊息，請檢查檔案的格式。</span><span class="sxs-lookup"><span data-stu-id="18059-198">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="18059-199">您只能使用硬體雜湊，或 OEM 名稱、序號和型號（以該資料行順序），或 Windows 產品識別碼。</span><span class="sxs-lookup"><span data-stu-id="18059-199">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="18059-200">您也可以使用 [**新增裝置**] 旁的連結所提供的範例 .csv 檔案來建立裝置清單。</span><span class="sxs-lookup"><span data-stu-id="18059-200">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="18059-201">您的 .csv 檔案看起來應該像這樣：</span><span class="sxs-lookup"><span data-stu-id="18059-201">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="18059-202">**裝置序號、Windows 產品識別碼、硬體雜湊、製造商名稱、裝置型號**</span><span class="sxs-lookup"><span data-stu-id="18059-202">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="18059-203">**{serialNumber},,, Microsoft Corporation，Surface 膝上型電腦**</span><span class="sxs-lookup"><span data-stu-id="18059-203">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

<span data-ttu-id="18059-204">請注意，「製造商名稱」和「裝置型號」區分大小寫。</span><span class="sxs-lookup"><span data-stu-id="18059-204">Note that "Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="18059-205">如果您不知道要為製造商名稱和裝置型號放入什麼值，您可以在裝置上執行此動作，以收集正確的值：</span><span class="sxs-lookup"><span data-stu-id="18059-205">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="18059-206">Windows Autopilot EULA 關閉</span><span class="sxs-lookup"><span data-stu-id="18059-206">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="18059-207">重要資訊</span><span class="sxs-lookup"><span data-stu-id="18059-207">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="18059-208">Windows Autopilot 可讓您在為客戶管理的裝置上設定自訂的 Windows 安裝。</span><span class="sxs-lookup"><span data-stu-id="18059-208">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="18059-209">如果客戶有權執行此動作，您可以在設定 Windows 時抑制或隱藏一般會呈現給使用者的特定設定畫面，包括 EULA （使用者授權合約）接受畫面。</span><span class="sxs-lookup"><span data-stu-id="18059-209">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="18059-210">藉由使用此函式，您同意隱藏或隱藏設計為使用者提供通知或接受條款的任何畫面，這表示您已向客戶取得足夠的同意和授權，以隱藏條款，而且代表您的客戶（無論是組織或個別的使用者，也可能是），同意任何通知並接受適用于您客戶的任何條款。</span><span class="sxs-lookup"><span data-stu-id="18059-210">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="18059-211">這包括同意授權條款和條件，或若未使用此工具抑制或隱藏時會對使用者顯示的通知。</span><span class="sxs-lookup"><span data-stu-id="18059-211">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="18059-212">您的客戶不可在這些裝置上使用 Windows 軟體，如果他們未向 Microsoft 或其授權經銷商有效取得軟體授權。</span><span class="sxs-lookup"><span data-stu-id="18059-212">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
