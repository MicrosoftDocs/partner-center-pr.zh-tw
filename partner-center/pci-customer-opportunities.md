---
title: 合作夥伴中心 Insights-CloudAscent 傾向報告
description: 瞭解合作夥伴中心中的 CloudAscent 傾向報告。 包含客戶傾向購買 Microsoft 產品的相關資訊。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175282"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="04cb9-104">CloudAscent 可從合作夥伴中心儀表板取得的傾向報表</span><span class="sxs-lookup"><span data-stu-id="04cb9-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="04cb9-105">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="04cb9-105">**Appropriate roles**</span></span>
- <span data-ttu-id="04cb9-106">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="04cb9-106">Executive report viewer</span></span>
- <span data-ttu-id="04cb9-107">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="04cb9-107">Report viewer</span></span>

<span data-ttu-id="04cb9-108">合作夥伴中心儀表板會從 CloudAscent 程式提供可下載的傾向資料。</span><span class="sxs-lookup"><span data-stu-id="04cb9-108">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="04cb9-109">此資料會顯示客戶購買 Microsoft 產品的傾向。</span><span class="sxs-lookup"><span data-stu-id="04cb9-109">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="04cb9-110">本文說明這項資料的細目、如何運用評分，以及其意義。</span><span class="sxs-lookup"><span data-stu-id="04cb9-110">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="04cb9-111">摘要定義</span><span class="sxs-lookup"><span data-stu-id="04cb9-111">Summary definitions</span></span>

- <span data-ttu-id="04cb9-112">**SMC 客戶**–這是傾向下載中的客戶總數。</span><span class="sxs-lookup"><span data-stu-id="04cb9-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="04cb9-113">客戶是由記錄的夥伴所識別。</span><span class="sxs-lookup"><span data-stu-id="04cb9-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="04cb9-114">**過期協定**-在目前會計年度內，我們會提供過期協定的數目。</span><span class="sxs-lookup"><span data-stu-id="04cb9-114">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="04cb9-115">**過期的收入**–與過期合約相關聯的收入。</span><span class="sxs-lookup"><span data-stu-id="04cb9-115">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="04cb9-116">**開啟過期的收入**–與開放式過期合約相關聯的收入。</span><span class="sxs-lookup"><span data-stu-id="04cb9-116">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="04cb9-118">CloudAscent SMB 分割</span><span class="sxs-lookup"><span data-stu-id="04cb9-118">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="04cb9-119">小型至中型企業 (SMB) 區段會進一步分成三個不同的子區段。</span><span class="sxs-lookup"><span data-stu-id="04cb9-119">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="04cb9-120">**頂級非受控** 包括最大的 SMB 客戶，最具 Microsoft 的商機。</span><span class="sxs-lookup"><span data-stu-id="04cb9-120">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="04cb9-121">一般未受管理的客戶與受管理的帳戶共用類似的特性，有大量員工、大量的 IT 預算和支出，以及 Microsoft 的大量潛在收入。</span><span class="sxs-lookup"><span data-stu-id="04cb9-121">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="04cb9-122">我們定義了最常見的雙重非受控方法：</span><span class="sxs-lookup"><span data-stu-id="04cb9-122">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="04cb9-123">**最常見的非受控使用者**-包含具有300或更多員工的帳戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-123">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="04cb9-124">User-Based 帳戶是首次購買或擴充以使用者為基礎的訂閱產品（例如 M365、D365 或 Surface）的絕佳目標。</span><span class="sxs-lookup"><span data-stu-id="04cb9-124">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="04cb9-125">以**最上層非受控計算為基礎**–包括 Azure 可能大於 $ 10k 的帳戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-125">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="04cb9-126">以計算為基礎的帳戶包括現有的 Azure。</span><span class="sxs-lookup"><span data-stu-id="04cb9-126">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="04cb9-127">有多年來的帳戶，以及尚未購買 Azure 的帳戶，但 Azure 可能大於 $ 10k 的帳戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-127">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="04cb9-128">**中型企業** 包含擁有25至300員工的現有客戶和潛在客戶帳戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-128">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="04cb9-129">**Small Business** 包含擁有25位以上員工的所有剩餘企業。</span><span class="sxs-lookup"><span data-stu-id="04cb9-129">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

<span data-ttu-id="04cb9-131">**最常見的非受控** 和 **中型企業** e1edp01 子代表高生命時間價值 (LTV) 客戶給 microsoft 和 microsoft 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="04cb9-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="04cb9-132">因此，它們是在此區段中推動成長的潛在客戶領域。</span><span class="sxs-lookup"><span data-stu-id="04cb9-132">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="04cb9-133">在這兩個 e1edp01 子中，我們最好是使用 M365 取得通訊端，再銷售 D365/Azure 企業營運 (LOB) 應用程式，並實現 Microsoft 的高 LTV。</span><span class="sxs-lookup"><span data-stu-id="04cb9-133">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="04cb9-134">今天，我們有兩個主要的商機範圍–1。</span><span class="sxs-lookup"><span data-stu-id="04cb9-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="04cb9-135">我們的客戶增加了成長;二級.</span><span class="sxs-lookup"><span data-stu-id="04cb9-135">our customer adds growth; 2.</span></span> <span data-ttu-id="04cb9-136">雖然我們可以取得 M365 的雲端通訊端，但我們在 D365 和 Azure 中有很大的機會。</span><span class="sxs-lookup"><span data-stu-id="04cb9-136">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="04cb9-137">下列螢幕擷取畫面顯示三個 SMB E1edp01 子與市場的優化路由。</span><span class="sxs-lookup"><span data-stu-id="04cb9-137">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="04cb9-138">CloudAscent 會優先處理所有最上層非受控與中型企業帳戶的分析、評分和模型化。</span><span class="sxs-lookup"><span data-stu-id="04cb9-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="04cb9-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="04cb9-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="04cb9-141">SMB 使用機器學習技術，在最上層非受控和中業務區段內推動銷售和行銷客戶預測。</span><span class="sxs-lookup"><span data-stu-id="04cb9-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="04cb9-142">如何收集信號並將其轉換為傾向建議？</span><span class="sxs-lookup"><span data-stu-id="04cb9-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="04cb9-143">**資料收集**： Web 編目程式會藉由 ping 公司網域來掃描及收集數十億個客戶信號，並監視： blog 文章、電子報、社交串流和技術論壇。</span><span class="sxs-lookup"><span data-stu-id="04cb9-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="04cb9-144">除了收集到的信號之外，也會從內部和外部來源（例如 D&B、Microsoft 內部訂用帳戶和交易資料）收集 firmographics 資訊。</span><span class="sxs-lookup"><span data-stu-id="04cb9-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="04cb9-145">**Machine Learning**：會將信號送入機器學習模型，以針對每個客戶依雲端產品和叢集輸出一組結構化的銷售和行銷預測資料集。</span><span class="sxs-lookup"><span data-stu-id="04cb9-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="04cb9-146">每個客戶都會使用外觀類似的模型來評分，以決定客戶的適合程度，並使用機器學習演算法來將客戶的線上行為定義整合為意圖。</span><span class="sxs-lookup"><span data-stu-id="04cb9-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="04cb9-147">評分會合並到叢集，以顯示客戶的傾向以購買 Microsoft 雲端產品。</span><span class="sxs-lookup"><span data-stu-id="04cb9-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="04cb9-148">**優化**： Machine Learning 系統會每季取用交易資料和訂用帳戶資料，以優化模型。</span><span class="sxs-lookup"><span data-stu-id="04cb9-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="04cb9-149">Machine Learning 會使用 win/遺失資料來調整演算法，並藉由比較叢集建議與在 MSX 中處理的商機，來驗證模型是否如預期般運作。</span><span class="sxs-lookup"><span data-stu-id="04cb9-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="04cb9-151">CloudAscent 傾向</span><span class="sxs-lookup"><span data-stu-id="04cb9-151">CloudAscent Propensity</span></span>

<span data-ttu-id="04cb9-152">如何建立傾向建議？</span><span class="sxs-lookup"><span data-stu-id="04cb9-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="04cb9-153">使用透過 web 編目程式所收集的信號和來自各種來源的資料，我們會合並 firmographics 資料和客戶的社交媒體信號。</span><span class="sxs-lookup"><span data-stu-id="04cb9-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="04cb9-154">評分會在比較模型中使用這些信號和資料，以配合意圖的模型並進行評分。</span><span class="sxs-lookup"><span data-stu-id="04cb9-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="04cb9-155">符合客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="04cb9-155">Customer Account Fit</span></span>

   - <span data-ttu-id="04cb9-156">定義 firmographics 的內部和外部資料點。</span><span class="sxs-lookup"><span data-stu-id="04cb9-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="04cb9-157">[符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。</span><span class="sxs-lookup"><span data-stu-id="04cb9-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="04cb9-158">每季更新評分比例</span><span class="sxs-lookup"><span data-stu-id="04cb9-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="04cb9-159">客戶帳戶意圖</span><span class="sxs-lookup"><span data-stu-id="04cb9-159">Customer Account Intent</span></span>

   - <span data-ttu-id="04cb9-160">社交媒體和客戶的線上行為定義意圖的相關信號。</span><span class="sxs-lookup"><span data-stu-id="04cb9-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="04cb9-161">意圖評分會重迭在適合定義叢集的最上層。</span><span class="sxs-lookup"><span data-stu-id="04cb9-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="04cb9-162">意圖評分會每月更新。</span><span class="sxs-lookup"><span data-stu-id="04cb9-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

3. <span data-ttu-id="04cb9-164">叢集</span><span class="sxs-lookup"><span data-stu-id="04cb9-164">Clustering</span></span>

   <span data-ttu-id="04cb9-165">符合和意圖的信號會合並成群集分數。</span><span class="sxs-lookup"><span data-stu-id="04cb9-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="04cb9-166">CloudAscent 有四個群集：</span><span class="sxs-lookup"><span data-stu-id="04cb9-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="04cb9-167">立即行動-銷售就緒客戶</span><span class="sxs-lookup"><span data-stu-id="04cb9-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="04cb9-168">評估-行銷就緒的客戶</span><span class="sxs-lookup"><span data-stu-id="04cb9-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="04cb9-169">培養-磁片磁碟機認知活動</span><span class="sxs-lookup"><span data-stu-id="04cb9-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="04cb9-170">教育教育和監視意圖</span><span class="sxs-lookup"><span data-stu-id="04cb9-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="04cb9-171">群集可讓使用者根據區段因素（例如：產品、地理、產業和垂直），以特定客戶的銷售和行銷計畫為目標。</span><span class="sxs-lookup"><span data-stu-id="04cb9-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="04cb9-172">CloudAscent 活頁簿中的 [ **傾向模型** ] 索引標籤會共用傾向和預估的空白字元收入。</span><span class="sxs-lookup"><span data-stu-id="04cb9-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="04cb9-173">若要定義符合和意圖的叢集，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="04cb9-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="04cb9-174">使用 ML 模型時，我們會先計算規模為100的客戶符合分數和意圖分數。</span><span class="sxs-lookup"><span data-stu-id="04cb9-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="04cb9-175">確切分數會根據 ML 模型而有所不同。</span><span class="sxs-lookup"><span data-stu-id="04cb9-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="04cb9-176">下列範例分數：</span><span class="sxs-lookup"><span data-stu-id="04cb9-176">Example Scores Below:</span></span>

         |<span data-ttu-id="04cb9-177">**分類**</span><span class="sxs-lookup"><span data-stu-id="04cb9-177">**Classification**</span></span>|<span data-ttu-id="04cb9-178">**分數**</span><span class="sxs-lookup"><span data-stu-id="04cb9-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="04cb9-179">高</span><span class="sxs-lookup"><span data-stu-id="04cb9-179">High</span></span>|<span data-ttu-id="04cb9-180">75-100</span><span class="sxs-lookup"><span data-stu-id="04cb9-180">75 - 100</span></span>|
         |<span data-ttu-id="04cb9-181">中</span><span class="sxs-lookup"><span data-stu-id="04cb9-181">Medium</span></span>|<span data-ttu-id="04cb9-182">55-74</span><span class="sxs-lookup"><span data-stu-id="04cb9-182">55 - 74</span></span>|
         |<span data-ttu-id="04cb9-183">低</span><span class="sxs-lookup"><span data-stu-id="04cb9-183">Low</span></span>|<span data-ttu-id="04cb9-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="04cb9-184">30 - 54</span></span>|
         |<span data-ttu-id="04cb9-185">非常低</span><span class="sxs-lookup"><span data-stu-id="04cb9-185">Very Low</span></span>|<span data-ttu-id="04cb9-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="04cb9-186">0 - 29</span></span>|

      2. <span data-ttu-id="04cb9-187">使用上述規則，我們會將企業分類為高、中、低，並在客戶的配合和意圖信號之間非常低。</span><span class="sxs-lookup"><span data-stu-id="04cb9-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="04cb9-188">我們會將每個代表傾向的交集，繪製在2D 矩陣上的客戶擬合和意圖信號。</span><span class="sxs-lookup"><span data-stu-id="04cb9-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="04cb9-189">例如，高尺寸 + 高意圖 = A1，代表最高的傾向。</span><span class="sxs-lookup"><span data-stu-id="04cb9-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="04cb9-190">最後，這些區段會組成叢集。</span><span class="sxs-lookup"><span data-stu-id="04cb9-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="04cb9-191">例如，A1、A2、A3、A4 形成「立即行動」叢集。</span><span class="sxs-lookup"><span data-stu-id="04cb9-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

   <span data-ttu-id="04cb9-193">針對這些客戶，建議您將目標設為「立即行動」並評估客戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="04cb9-194">CloudAscent 產品 & 模型</span><span class="sxs-lookup"><span data-stu-id="04cb9-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="04cb9-195">下圖提供 CloudAscent 內每個傾向模型的觀點：</span><span class="sxs-lookup"><span data-stu-id="04cb9-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

<span data-ttu-id="04cb9-197">空白模型是由現有 Microsoft 客戶的預測所組成，其中沒有產品及/或是新的潛在客戶。</span><span class="sxs-lookup"><span data-stu-id="04cb9-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="04cb9-198">追加銷售模型會使用交易資料來預測 Azure 和 M365 Sku 中的追加銷售潛力。</span><span class="sxs-lookup"><span data-stu-id="04cb9-198">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="04cb9-199">EOS 共用 Win 7、Office 2010、SQL Server 和 Windows Server 的服務客戶結束。</span><span class="sxs-lookup"><span data-stu-id="04cb9-199">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="04cb9-200">使用 CloudAscent 傾向模型時，會從 MS Sales 提取 EOS 資料並與之重迭。</span><span class="sxs-lookup"><span data-stu-id="04cb9-200">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="04cb9-201">EOS 資料存留在新式工作和 Azure 銷售的生活中。</span><span class="sxs-lookup"><span data-stu-id="04cb9-201">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
