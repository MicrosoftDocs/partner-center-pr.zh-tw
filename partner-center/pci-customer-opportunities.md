---
title: 合作夥伴中心 Insights-CloudAscent 傾向報告
description: 瞭解合作夥伴中心儀表板中的 CloudAscent 傾向報告。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: 510f85b053ec17fa0a2a66217a19c006e7ca2bc9
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811332"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="fdd2b-103">CloudAscent 可從合作夥伴中心儀表板取得的傾向報表</span><span class="sxs-lookup"><span data-stu-id="fdd2b-103">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="fdd2b-104">**適當的角色**</span><span class="sxs-lookup"><span data-stu-id="fdd2b-104">**Appropriate roles**</span></span>
- <span data-ttu-id="fdd2b-105">高階報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="fdd2b-105">Executive report viewer</span></span>
- <span data-ttu-id="fdd2b-106">報告檢視人員</span><span class="sxs-lookup"><span data-stu-id="fdd2b-106">Report viewer</span></span>

<span data-ttu-id="fdd2b-107">合作夥伴中心儀表板會從 CloudAscent 程式提供可下載的傾向資料。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-107">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="fdd2b-108">此資料會顯示客戶購買 Microsoft 產品的傾向。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-108">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="fdd2b-109">本文說明這項資料的細目、如何運用評分，以及其意義。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-109">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="fdd2b-110">摘要定義</span><span class="sxs-lookup"><span data-stu-id="fdd2b-110">Summary definitions</span></span>

- <span data-ttu-id="fdd2b-111">**SMC 客戶**–這是傾向下載中的客戶總數。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-111">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="fdd2b-112">客戶是由記錄的夥伴所識別。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-112">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="fdd2b-113">**過期協定**-在目前會計年度內，我們會提供過期協定的數目。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-113">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="fdd2b-114">**過期的收入**–與過期合約相關聯的收入。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-114">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="fdd2b-115">**開啟過期的收入**–與開放式過期合約相關聯的收入。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="客戶商機摘要儀表板的螢幕擷取畫面。":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="fdd2b-117">CloudAscent SMB 分割</span><span class="sxs-lookup"><span data-stu-id="fdd2b-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="fdd2b-118">小型至中型企業 (SMB) 區段會進一步分成三個不同的子區段。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-118">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="fdd2b-119">**頂級非受控** 包括最大的 SMB 客戶，最具 Microsoft 的商機。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="fdd2b-120">一般未受管理的客戶與受管理的帳戶共用類似的特性，有大量員工、大量的 IT 預算和支出，以及 Microsoft 的大量潛在收入。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-120">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="fdd2b-121">我們定義了最常見的雙重非受控方法：</span><span class="sxs-lookup"><span data-stu-id="fdd2b-121">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="fdd2b-122">**最常見的非受控使用者**-包含具有300或更多員工的帳戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="fdd2b-123">以使用者為基礎的帳戶是首次購買或擴充以使用者為基礎的訂閱產品（例如 M365、D365 或 Surface）的絕佳目標。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="fdd2b-124">以**最上層非受控計算為基礎**–包括 Azure 可能大於 $ 10k 的帳戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="fdd2b-125">以計算為基礎的帳戶包括現有的 Azure。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="fdd2b-126">有多年來的帳戶，以及尚未購買 Azure 的帳戶，但 Azure 可能大於 $ 10k 的帳戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="fdd2b-127">**中型企業** 包含擁有25至300員工的現有客戶和潛在客戶帳戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="fdd2b-128">**Small Business** 包含擁有25位以上員工的所有剩餘企業。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-128">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="依 SMC 類型的客戶。":::

<span data-ttu-id="fdd2b-130">**最常見的非受控** 和 **中型企業** e1edp01 子代表高生命時間價值 (LTV) 客戶給 microsoft 和 microsoft 合作夥伴。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-130">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="fdd2b-131">因此，它們是在此區段中推動成長的潛在客戶領域。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-131">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="fdd2b-132">在這兩個 e1edp01 子中，我們最好是使用 M365 取得通訊端，再銷售 D365/Azure 企業營運 (LOB) 應用程式，並實現 Microsoft 的高 LTV。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-132">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="fdd2b-133">今天，我們有兩個主要的商機範圍–1。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-133">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="fdd2b-134">我們的客戶增加了成長;二級.</span><span class="sxs-lookup"><span data-stu-id="fdd2b-134">our customer adds growth; 2.</span></span> <span data-ttu-id="fdd2b-135">雖然我們可以取得 M365 的雲端通訊端，但我們在 D365 和 Azure 中有很大的機會。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-135">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="fdd2b-136">下列螢幕擷取畫面顯示三個 SMB E1edp01 子與市場的優化路由。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-136">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="fdd2b-137">CloudAscent 會優先處理所有最上層非受控與中型企業帳戶的分析、評分和模型化。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-137">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="SMB e1edp01 子的螢幕擷取畫面。":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="fdd2b-139">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="fdd2b-139">CloudAscent Machine Learning</span></span>

<span data-ttu-id="fdd2b-140">SMB 使用機器學習技術，在最上層非受控和中業務區段內推動銷售和行銷客戶預測。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-140">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="fdd2b-141">如何收集信號並將其轉換為傾向建議？</span><span class="sxs-lookup"><span data-stu-id="fdd2b-141">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="fdd2b-142">**資料收集**： Web 編目程式會藉由 ping 公司網域來掃描及收集數十億個客戶信號，並監視： blog 文章、電子報、社交串流和技術論壇。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-142">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="fdd2b-143">除了收集到的信號之外，也會從內部和外部來源（例如 D&B、Microsoft 內部訂用帳戶和交易資料）收集 firmographics 資訊。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-143">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="fdd2b-144">**Machine Learning**：會將信號送入機器學習模型，以針對每個客戶依雲端產品和叢集輸出一組結構化的銷售和行銷預測資料集。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-144">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="fdd2b-145">每個客戶都會使用外觀類似的模型來評分，以決定客戶的適合程度，並使用機器學習演算法來將客戶的線上行為定義整合為意圖。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-145">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="fdd2b-146">評分會合並到叢集，以顯示客戶的傾向以購買 Microsoft 雲端產品。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-146">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="fdd2b-147">**優化**： Machine Learning 系統會每季取用交易資料和訂用帳戶資料，以優化模型。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-147">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="fdd2b-148">Machine Learning 會使用 win/遺失資料來調整演算法，並藉由比較叢集建議與在 MSX 中處理的商機，來驗證模型是否如預期般運作。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-148">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 機器學習的螢幕擷取畫面。":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="fdd2b-150">CloudAscent 傾向</span><span class="sxs-lookup"><span data-stu-id="fdd2b-150">CloudAscent Propensity</span></span>

<span data-ttu-id="fdd2b-151">如何建立傾向建議？</span><span class="sxs-lookup"><span data-stu-id="fdd2b-151">How are propensity recommendations created?</span></span>

<span data-ttu-id="fdd2b-152">使用透過 web 編目程式所收集的信號和來自各種來源的資料，我們會合並 firmographics 資料和客戶的社交媒體信號。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-152">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="fdd2b-153">評分會在比較模型中使用這些信號和資料，以配合意圖的模型並進行評分。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-153">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="fdd2b-154">符合客戶帳戶</span><span class="sxs-lookup"><span data-stu-id="fdd2b-154">Customer Account Fit</span></span>

   - <span data-ttu-id="fdd2b-155">定義 firmographics 的內部和外部資料點。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-155">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="fdd2b-156">[符合評分] 會使用外觀類似的模型來比較客戶，並查看它們是否為 Microsoft 雲端產品的最適合。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-156">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="fdd2b-157">每季更新評分比例</span><span class="sxs-lookup"><span data-stu-id="fdd2b-157">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="fdd2b-158">客戶帳戶意圖</span><span class="sxs-lookup"><span data-stu-id="fdd2b-158">Customer Account Intent</span></span>

   - <span data-ttu-id="fdd2b-159">社交媒體和客戶的線上行為定義意圖的相關信號。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-159">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="fdd2b-160">意圖評分會重迭在適合定義叢集的最上層。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-160">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="fdd2b-161">意圖評分會每月更新。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-161">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 預測模型。":::

3. <span data-ttu-id="fdd2b-163">叢集</span><span class="sxs-lookup"><span data-stu-id="fdd2b-163">Clustering</span></span>

   <span data-ttu-id="fdd2b-164">符合和意圖的信號會合並成群集分數。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-164">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="fdd2b-165">CloudAscent 有四個群集：</span><span class="sxs-lookup"><span data-stu-id="fdd2b-165">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="fdd2b-166">立即行動-銷售就緒客戶</span><span class="sxs-lookup"><span data-stu-id="fdd2b-166">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="fdd2b-167">評估-行銷就緒的客戶</span><span class="sxs-lookup"><span data-stu-id="fdd2b-167">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="fdd2b-168">培養-磁片磁碟機認知活動</span><span class="sxs-lookup"><span data-stu-id="fdd2b-168">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="fdd2b-169">教育教育和監視意圖</span><span class="sxs-lookup"><span data-stu-id="fdd2b-169">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="fdd2b-170">群集可讓使用者根據區段因素（例如：產品、地理、產業和垂直），以特定客戶的銷售和行銷計畫為目標。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-170">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="fdd2b-171">CloudAscent 活頁簿中的 [ **傾向模型** ] 索引標籤會共用傾向和預估的空白字元收入。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-171">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="fdd2b-172">若要定義符合和意圖的叢集，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="fdd2b-172">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="fdd2b-173">使用 ML 模型時，我們會先計算規模為100的客戶符合分數和意圖分數。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-173">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="fdd2b-174">確切分數會根據 ML 模型而有所不同。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-174">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="fdd2b-175">下列範例分數：</span><span class="sxs-lookup"><span data-stu-id="fdd2b-175">Example Scores Below:</span></span>

         |<span data-ttu-id="fdd2b-176">**分類**</span><span class="sxs-lookup"><span data-stu-id="fdd2b-176">**Classification**</span></span>|<span data-ttu-id="fdd2b-177">**分數**</span><span class="sxs-lookup"><span data-stu-id="fdd2b-177">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="fdd2b-178">高</span><span class="sxs-lookup"><span data-stu-id="fdd2b-178">High</span></span>|<span data-ttu-id="fdd2b-179">75-100</span><span class="sxs-lookup"><span data-stu-id="fdd2b-179">75 - 100</span></span>|
         |<span data-ttu-id="fdd2b-180">中</span><span class="sxs-lookup"><span data-stu-id="fdd2b-180">Medium</span></span>|<span data-ttu-id="fdd2b-181">55-74</span><span class="sxs-lookup"><span data-stu-id="fdd2b-181">55 - 74</span></span>|
         |<span data-ttu-id="fdd2b-182">低</span><span class="sxs-lookup"><span data-stu-id="fdd2b-182">Low</span></span>|<span data-ttu-id="fdd2b-183">30 - 54</span><span class="sxs-lookup"><span data-stu-id="fdd2b-183">30 - 54</span></span>|
         |<span data-ttu-id="fdd2b-184">非常低</span><span class="sxs-lookup"><span data-stu-id="fdd2b-184">Very Low</span></span>|<span data-ttu-id="fdd2b-185">0 - 29</span><span class="sxs-lookup"><span data-stu-id="fdd2b-185">0 - 29</span></span>|

      2. <span data-ttu-id="fdd2b-186">使用上述規則，我們會將企業分類為高、中、低，並在客戶的配合和意圖信號之間非常低。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-186">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="fdd2b-187">我們會將每個代表傾向的交集，繪製在2D 矩陣上的客戶擬合和意圖信號。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-187">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="fdd2b-188">例如，高尺寸 + 高意圖 = A1，代表最高的傾向。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-188">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="fdd2b-189">最後，這些區段會組成叢集。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-189">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="fdd2b-190">例如，A1、A2、A3、A4 形成「立即行動」叢集。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-190">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent 模型。":::

   <span data-ttu-id="fdd2b-192">針對這些客戶，建議您將目標設為「立即行動」並評估客戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-192">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="fdd2b-193">CloudAscent 產品 & 模型</span><span class="sxs-lookup"><span data-stu-id="fdd2b-193">CloudAscent Products & Models</span></span>

<span data-ttu-id="fdd2b-194">下圖提供 CloudAscent 內每個傾向模型的觀點：</span><span class="sxs-lookup"><span data-stu-id="fdd2b-194">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向模型。":::

<span data-ttu-id="fdd2b-196">空白模型是由現有 Microsoft 客戶的預測所組成，其中沒有產品及/或是新的潛在客戶。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-196">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="fdd2b-197">追加銷售模型會使用交易資料來預測 Azure 和 M365 Sku 中的追加銷售潛力。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-197">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="fdd2b-198">EOS 共用 Win 7、Office 2010、SQL Server 和 Windows Server 的服務客戶結束。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-198">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="fdd2b-199">使用 CloudAscent 傾向模型時，會從 MS Sales 提取 EOS 資料並與之重迭。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="fdd2b-200">EOS 資料存留在新式工作和 Azure 銷售的生活中。</span><span class="sxs-lookup"><span data-stu-id="fdd2b-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
