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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="45cde-103">在新裝置上使用 Windows Autopilot 設定檔，以自訂客戶的全新體驗</span><span class="sxs-lookup"><span data-stu-id="45cde-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="45cde-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="45cde-104">**Appropriate roles**</span></span>

- <span data-ttu-id="45cde-105">系統管理代理人</span><span class="sxs-lookup"><span data-stu-id="45cde-105">Admin agent</span></span>
- <span data-ttu-id="45cde-106">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="45cde-106">Global admin</span></span>
- <span data-ttu-id="45cde-107">銷售代理人</span><span class="sxs-lookup"><span data-stu-id="45cde-107">Sales agent</span></span>
- <span data-ttu-id="45cde-108">使用者管理系統管理員</span><span class="sxs-lookup"><span data-stu-id="45cde-108">User management admin</span></span>

<span data-ttu-id="45cde-109">如果您管理客戶裝置，您可能需要為客戶的使用者自訂現成體驗 (OOBE) 。</span><span class="sxs-lookup"><span data-stu-id="45cde-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="45cde-110">您可以先使用 Windows Autopilot 設定檔預先設定新的裝置，再將裝置傳遞給客戶，並將新的設定檔套用至客戶已購買的裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="45cde-111">請注意，Oem 已開始將出貨標籤包含在 Autopilot 裝置的外部，以顯示裝置的 **產品金鑰識別碼 (PKID)**。</span><span class="sxs-lookup"><span data-stu-id="45cde-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="45cde-112">這一維、可讀取的條碼可為下游合作夥伴提供註冊裝置以進行 Autopilot 的方式，而不需要將裝置 () ，而是透過替代方式來收集裝置識別碼。</span><span class="sxs-lookup"><span data-stu-id="45cde-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="45cde-113">本文說明如何在合作夥伴中心中建立 Autopilot 設定檔，並將其套用至裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="45cde-114">如果您還不熟悉 Autopilot，請參閱下列文章中的資訊：</span><span class="sxs-lookup"><span data-stu-id="45cde-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="45cde-115">Windows Autopilot 概觀</span><span class="sxs-lookup"><span data-stu-id="45cde-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="45cde-116">Autopilot 部署參考指南</span><span class="sxs-lookup"><span data-stu-id="45cde-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="45cde-117">概觀</span><span class="sxs-lookup"><span data-stu-id="45cde-117">Overview</span></span>

<span data-ttu-id="45cde-118">利用合作夥伴中心中的 Windows Autopilot 功能，您可以建立自訂設定檔以套用至客戶裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="45cde-119">下列設定檔設定已在發行本文時提供：</span><span class="sxs-lookup"><span data-stu-id="45cde-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="45cde-120">略過隱私權設定。</span><span class="sxs-lookup"><span data-stu-id="45cde-120">Skip privacy settings.</span></span> <span data-ttu-id="45cde-121">此選用的 Autopilot 設定檔設定可讓組織在 OOBE 程式期間不詢問隱私權設定。</span><span class="sxs-lookup"><span data-stu-id="45cde-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="45cde-122">停用裝置上的本機系統管理員帳戶建立。</span><span class="sxs-lookup"><span data-stu-id="45cde-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="45cde-123">組織可以決定在程式完成之後，使用者設定裝置是否應該具有系統管理員存取權。</span><span class="sxs-lookup"><span data-stu-id="45cde-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="45cde-124">自動設定公司或學校裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="45cde-125">所有向 Autopilot 註冊的裝置都會自動被視為公司或學校裝置，因此在 OOBE 程式期間不會詢問此問題。</span><span class="sxs-lookup"><span data-stu-id="45cde-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="45cde-126">略過 Cortana、OneDrive 和 OEM 註冊設定頁面。</span><span class="sxs-lookup"><span data-stu-id="45cde-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="45cde-127">所有向 Autopilot 註冊的裝置，會在) 程式 (OOBE 的全新體驗期間自動略過這些頁面。</span><span class="sxs-lookup"><span data-stu-id="45cde-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="45cde-128">略過使用者授權合約 (EULA) 。</span><span class="sxs-lookup"><span data-stu-id="45cde-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="45cde-129">從 Windows 10 版本1709開始，組織可以決定略過 OOBE 程式期間所呈現的 EULA 頁面。</span><span class="sxs-lookup"><span data-stu-id="45cde-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="45cde-130">如需有關在 Windows 安裝期間略過 EULA 頁面的重要資訊，請參閱以下 [WINDOWS AUTOPILOT eula 關閉](#windows-autopilot-eula-dismissal) 。</span><span class="sxs-lookup"><span data-stu-id="45cde-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="45cde-131">以下是適用的設定檔和裝置管理權限和限制：</span><span class="sxs-lookup"><span data-stu-id="45cde-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="45cde-132">CSP 合作夥伴可以針對具有轉售商關係的現有客戶繼續管理 Autopilot 設定檔，即使客戶已移除合作夥伴的委派系統管理權限也一樣。</span><span class="sxs-lookup"><span data-stu-id="45cde-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="45cde-133">您可以為已新增的客戶管理現有裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="45cde-134">您無法管理客戶上傳至商務用 Microsoft Store 或 Microsoft Intune 入口網站的裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="45cde-135">在合作夥伴中心中建立和管理 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="45cde-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="45cde-136">在合作夥伴中心中，您可以建立 Windows Autopilot 部署設定檔，並將其套用至裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="45cde-137">只有系統管理員代理程式可以建立及套用設定檔。</span><span class="sxs-lookup"><span data-stu-id="45cde-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="45cde-138">建立新的 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="45cde-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="45cde-139">從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取要為其建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="45cde-140">在客戶的詳細資料頁面上，選取 [ **裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="45cde-141">在 [ **Windows Autopilot 設定檔** ] 下，選取 [ **新增設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="45cde-142">輸入設定檔的名稱和描述，然後設定 OOBE 設定。</span><span class="sxs-lookup"><span data-stu-id="45cde-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="45cde-143">從下列選項進行選擇：</span><span class="sxs-lookup"><span data-stu-id="45cde-143">Choose from:</span></span>  

   - <span data-ttu-id="45cde-144">在安裝程式中略過隱私權設定</span><span class="sxs-lookup"><span data-stu-id="45cde-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="45cde-145">停用設定中的本機系統管理員帳戶</span><span class="sxs-lookup"><span data-stu-id="45cde-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="45cde-146">自動略過設定中的頁面</span><span class="sxs-lookup"><span data-stu-id="45cde-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="45cde-147"> (包括 *自動選取公司或學校的設定* ，以及 *略過 Cortana、OneDrive 和 OEM 註冊設定頁面*) </span><span class="sxs-lookup"><span data-stu-id="45cde-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="45cde-148">略過使用者授權合約 (EULA) </span><span class="sxs-lookup"><span data-stu-id="45cde-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="45cde-149">如需有關在 Windows 安裝期間略過 EULA 頁面的重要資訊，請參閱以下 [WINDOWS AUTOPILOT eula 關閉](#windows-autopilot-eula-dismissal) 。</span><span class="sxs-lookup"><span data-stu-id="45cde-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="45cde-150">完成時選取 **\[提交\]**。</span><span class="sxs-lookup"><span data-stu-id="45cde-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="45cde-151">將 Autopilot 設定檔套用至客戶裝置</span><span class="sxs-lookup"><span data-stu-id="45cde-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="45cde-152">下列指示假設您已將客戶的裝置新增至合作夥伴中心，且您可以存取其裝置清單。</span><span class="sxs-lookup"><span data-stu-id="45cde-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="45cde-153">如果您尚未新增客戶的裝置，請遵循 [將裝置新增至客戶帳戶](#add-devices-to-a-customers-account) 中的指示，然後遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="45cde-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="45cde-154">為客戶建立 Autopilot 設定檔之後，您可以將其套用至客戶的裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="45cde-155">從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取您為其建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="45cde-156">在客戶的詳細資料頁面上，選取 [ **裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="45cde-157">在 [ **將設定檔套用至裝置** ] 下，選取您要新增設定檔的裝置或裝置群組，然後選取 [套用 **設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="45cde-158">您剛剛套用的設定檔會出現在 [ **設定檔** ] 欄位中。</span><span class="sxs-lookup"><span data-stu-id="45cde-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="45cde-159">遵循下列步驟來確認設定檔將會成功套用至裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="45cde-160">a.</span><span class="sxs-lookup"><span data-stu-id="45cde-160">a.</span></span>  <span data-ttu-id="45cde-161">將裝置連線到網路，並將它開啟。</span><span class="sxs-lookup"><span data-stu-id="45cde-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="45cde-162">b.</span><span class="sxs-lookup"><span data-stu-id="45cde-162">b.</span></span>  <span data-ttu-id="45cde-163">確認是否會顯示適當的 OOBE 畫面 (如果有的話)。</span><span class="sxs-lookup"><span data-stu-id="45cde-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="45cde-164">c.</span><span class="sxs-lookup"><span data-stu-id="45cde-164">c.</span></span>  <span data-ttu-id="45cde-165">當 OOBE 程式停止時，請將裝置重設為其原廠預設值，為新的使用者準備該裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="45cde-166">從客戶的裝置移除 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="45cde-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="45cde-167">從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取您為其建立 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="45cde-168">在客戶的詳細資料頁面上，選取 [ **裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="45cde-169">在 [ **將設定檔套用至裝置** ] 下，選取您要從中移除設定檔的裝置，然後選取 [ **移除設定檔**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="45cde-170">從裝置移除設定檔並不會從您的清單中刪除設定檔。</span><span class="sxs-lookup"><span data-stu-id="45cde-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="45cde-171">如果您想要刪除設定檔，請依照 [更新或刪除 Autopilot 設定檔](#update-or-delete-an-autopilot-profile)中的指示進行。</span><span class="sxs-lookup"><span data-stu-id="45cde-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="45cde-172">更新或刪除 Autopilot 設定檔</span><span class="sxs-lookup"><span data-stu-id="45cde-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="45cde-173">如果客戶想要在您將裝置寄送至裝置之後變更現成體驗，您可以在合作夥伴中心中變更設定檔。</span><span class="sxs-lookup"><span data-stu-id="45cde-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="45cde-174">當客戶的裝置連線到網際網路時，它會在 OOBE 程式期間下載最新的設定檔版本。</span><span class="sxs-lookup"><span data-stu-id="45cde-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="45cde-175">此外，當客戶將裝置還原為其原廠預設設定時，裝置會在 OOBE 程式期間再次下載最新的設定檔版本。</span><span class="sxs-lookup"><span data-stu-id="45cde-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="45cde-176">從合作夥伴中心] 功能表選取 [ **客戶** ]，然後選取想要變更 Autopilot 設定檔的客戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="45cde-177">在客戶的詳細資料頁面上，選取 [ **裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="45cde-178">在 [ **Windows Autopilot 設定檔** ] 下，選取您需要更新的設定檔。</span><span class="sxs-lookup"><span data-stu-id="45cde-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="45cde-179">進行必要的變更，然後選取 [ **提交**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="45cde-180">若要刪除此設定檔，請選取頁面右上角的 [ **刪除設定檔** ]。</span><span class="sxs-lookup"><span data-stu-id="45cde-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="45cde-181">將裝置新增至客戶的帳戶</span><span class="sxs-lookup"><span data-stu-id="45cde-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="45cde-182">銷售專員和系統管理員代理程式可以將裝置新增至客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="45cde-183">您必須能夠存取客戶的裝置清單，才能將自訂 Autopilot 設定檔套用至客戶裝置。</span><span class="sxs-lookup"><span data-stu-id="45cde-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="45cde-184">如果您打算使用 OEM 名稱、序號和模型組合，請注意下列限制：</span><span class="sxs-lookup"><span data-stu-id="45cde-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="45cde-185">此元組僅適用于較新的裝置 (4k 雜湊，例如) ，而且不支援 (RS2 和先前裝置) 的128b 雜湊。</span><span class="sxs-lookup"><span data-stu-id="45cde-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="45cde-186">元組註冊會區分大小寫，因此檔案中的資料必須與 OEM 提供者所提供的模型和製造商名稱 \**_完全_* 相符， (硬體提供者) 。</span><span class="sxs-lookup"><span data-stu-id="45cde-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="45cde-187">依照下列指示，在合作夥伴中心中將裝置新增至客戶的帳戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="45cde-188">從合作夥伴中心] 功能表中選取 [_ \*客戶\*\*]，然後選取您要管理其裝置的客戶。</span><span class="sxs-lookup"><span data-stu-id="45cde-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="45cde-189">在客戶的詳細資料頁面上，選取 [ **裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="45cde-190">在 [ **將設定檔套用至裝置** ] 下方，選取 [ **新增裝置**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="45cde-191">輸入裝置清單的名稱，然後選取 **[流覽]** ，以 .csv 檔案格式將客戶的清單 (上傳) 至合作夥伴中心。</span><span class="sxs-lookup"><span data-stu-id="45cde-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="45cde-192">您應該已在購買裝置時收到此 .csv 檔案。</span><span class="sxs-lookup"><span data-stu-id="45cde-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="45cde-193">如果您未收到 .csv 檔案，您可以依照 [將裝置新增至 Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步驟自行建立。</span><span class="sxs-lookup"><span data-stu-id="45cde-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="45cde-194">上傳 .csv 檔案，然後選取 [ **儲存**]。</span><span class="sxs-lookup"><span data-stu-id="45cde-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="45cde-195">如果您在嘗試上傳 .csv 檔案時收到錯誤訊息，請檢查檔案的格式。</span><span class="sxs-lookup"><span data-stu-id="45cde-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="45cde-196">您只能使用硬體雜湊，或 OEM 名稱、序號和型號 (依該資料行順序)，或 Windows 產品識別碼。</span><span class="sxs-lookup"><span data-stu-id="45cde-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="45cde-197">您也可以使用 [ **新增裝置** ] 旁的連結所提供的範例 .csv 檔案來建立裝置清單。</span><span class="sxs-lookup"><span data-stu-id="45cde-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="45cde-198">您的 .csv 檔案看起來應該像這樣：</span><span class="sxs-lookup"><span data-stu-id="45cde-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="45cde-199">**裝置序號、Windows 產品識別碼、硬體雜湊、製造商名稱、裝置型號**</span><span class="sxs-lookup"><span data-stu-id="45cde-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="45cde-200">**{serialNumber},,, Microsoft Corporation，Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="45cde-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="45cde-201">「製造商名稱」和「裝置型號」會區分大小寫。</span><span class="sxs-lookup"><span data-stu-id="45cde-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="45cde-202">如果您不知道要為製造商名稱和裝置型號放置哪些值，您可以在裝置上執行，以收集正確的值：</span><span class="sxs-lookup"><span data-stu-id="45cde-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="45cde-203">Windows Autopilot EULA 關閉</span><span class="sxs-lookup"><span data-stu-id="45cde-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="45cde-204">重要資訊</span><span class="sxs-lookup"><span data-stu-id="45cde-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="45cde-205">Windows Autopilot 可讓您在為客戶管理的裝置上設定 Windows 的自訂安裝。</span><span class="sxs-lookup"><span data-stu-id="45cde-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="45cde-206">如果客戶已獲授權，您可以隱藏或隱藏設定 Windows 時通常會向使用者呈現的特定設定畫面，包括 EULA (使用者授權合約) 接受畫面。</span><span class="sxs-lookup"><span data-stu-id="45cde-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="45cde-207">藉由使用此函數，您同意隱藏或隱藏任何設計來提供使用者通知或接受條款的畫面，表示您已從客戶取得足夠的同意與授權來隱藏條款，而您代表客戶 (是否可以) 組織或個別使用者，或同意任何通知，並接受任何適用于您客戶的條款。</span><span class="sxs-lookup"><span data-stu-id="45cde-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="45cde-208">這包括同意授權條款和條件，或若未使用此工具抑制或隱藏時會對使用者顯示的通知。</span><span class="sxs-lookup"><span data-stu-id="45cde-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="45cde-209">您的客戶不可在這些裝置上使用 Windows 軟體，如果他們未向 Microsoft 或其授權經銷商有效取得軟體授權。</span><span class="sxs-lookup"><span data-stu-id="45cde-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>