---
title: パートナーセンターの洞察-CloudAscent 傾向レポート
description: パートナーセンターダッシュボードの CloudAscent 傾向レポートについて説明します。
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
ms.contentlocale: ja-JP
ms.lasthandoff: 09/19/2020
ms.locfileid: "90811352"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="92799-103">パートナーセンターダッシュボードから使用可能な CloudAscent 傾向レポート</span><span class="sxs-lookup"><span data-stu-id="92799-103">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="92799-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="92799-104">**Appropriate roles**</span></span>
- <span data-ttu-id="92799-105">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="92799-105">Executive report viewer</span></span>
- <span data-ttu-id="92799-106">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="92799-106">Report viewer</span></span>

<span data-ttu-id="92799-107">パートナーセンターダッシュボードは、CloudAscent プログラムからダウンロード可能な傾向データを提供します。</span><span class="sxs-lookup"><span data-stu-id="92799-107">The Partner Center Dashboard provides downloadable propensity data from the CloudAscent Program.</span></span> <span data-ttu-id="92799-108">このデータは、Microsoft 製品を購入する顧客の傾向を示しています。</span><span class="sxs-lookup"><span data-stu-id="92799-108">The data shows the customers' propensity to purchase Microsoft products.</span></span>  <span data-ttu-id="92799-109">この記事では、このデータの内訳、スコアリングを利用する方法、およびその意味について説明します。</span><span class="sxs-lookup"><span data-stu-id="92799-109">This articles describes the breakdown of this data, how to utilize the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="92799-110">概要定義</span><span class="sxs-lookup"><span data-stu-id="92799-110">Summary definitions</span></span>

- <span data-ttu-id="92799-111">**SMC のお客様**–傾向のダウンロードにおける顧客の合計数です。</span><span class="sxs-lookup"><span data-stu-id="92799-111">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="92799-112">顧客は、レコードのパートナーによって識別されます。</span><span class="sxs-lookup"><span data-stu-id="92799-112">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="92799-113">**契約期限切れ**–現在の会計年度内で、期限切れになった契約の数を提供しています。</span><span class="sxs-lookup"><span data-stu-id="92799-113">**Expire Agreements**– within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="92799-114">**期限**切れの収益–期限切れになった契約に関連付けられている収益。</span><span class="sxs-lookup"><span data-stu-id="92799-114">**Expiring Revenue**– the revenue associated to the expiring agreements.</span></span>
- <span data-ttu-id="92799-115">**[有効期限**が迫っている収益] –オープン期限が切れた契約に関連付けられている収益。</span><span class="sxs-lookup"><span data-stu-id="92799-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Customers 営業案件の概要ダッシュボードのスクリーンショット。":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="92799-117">CloudAscent SMB セグメンテーション</span><span class="sxs-lookup"><span data-stu-id="92799-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="92799-118">小規模から中規模のビジネス (SMB) セグメントは、さらに3つの個別のサブセグメントに分割されます。</span><span class="sxs-lookup"><span data-stu-id="92799-118">The small to medium business (SMB) segment is further divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="92799-119">**上位の非管理** 対象には、Microsoft の最も多くの機会を持つ最大規模の SMB 顧客が含まれます。</span><span class="sxs-lookup"><span data-stu-id="92799-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="92799-120">一般的な上位の管理されていないお客様は、多数の従業員、大量の IT 予算および支出、Microsoft の収益の可能性を持つ、管理アカウントと同様の特性を共有します。</span><span class="sxs-lookup"><span data-stu-id="92799-120">Typical Top Unmanaged customers share similar characteristics as Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="92799-121">上位のアンマネージ2つの方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="92799-121">We define Top Unmanaged two ways:</span></span>

   - <span data-ttu-id="92799-122">上位の管理されていない**ユーザーベース**–300以上の従業員を含むアカウントを含みます。</span><span class="sxs-lookup"><span data-stu-id="92799-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="92799-123">ユーザーベースのアカウントは、初めて購入する場合、または M365、D365、Surface などのユーザーベースのサブスクリプション製品を展開する場合に適しています。</span><span class="sxs-lookup"><span data-stu-id="92799-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as M365, D365, or Surface.</span></span>
   - <span data-ttu-id="92799-124">管理されていない**計算ベースの上位**– Azure が $ 10k を超える可能性のあるアカウントを含みます。</span><span class="sxs-lookup"><span data-stu-id="92799-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="92799-125">コンピューティングベースのアカウントには、既存の Azure が含まれます。</span><span class="sxs-lookup"><span data-stu-id="92799-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="92799-126">将来、Azure をまだ購入していても、Azure では $ 10k を超える可能性のある azure をまだ購入していない、未来の年の可能性があるアカウントとアカウント。</span><span class="sxs-lookup"><span data-stu-id="92799-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="92799-127">**中規模ビジネス** には、既存の顧客と、25 ~ 300 人の従業員を持つ見込み客アカウントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="92799-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="92799-128">**スモールビジネス** には、従業員が25人未満の残りの企業がすべて含まれます。</span><span class="sxs-lookup"><span data-stu-id="92799-128">**Small Business** includes all remaining businesses with fewer than 25 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC によるお客様の種類。":::

<span data-ttu-id="92799-130">**上位の管理対象外** および **中規模のビジネス** subsegments は、microsoft および microsoft パートナー向けの高ライフタイム値 (ltv) のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="92799-130">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="92799-131">そのため、このセグメントの成長に焦点を当てています。</span><span class="sxs-lookup"><span data-stu-id="92799-131">Hence they are the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="92799-132">この2つの subsegments では、D365/Azure 基幹業務 (LOB) アプリを使用して、M365 でソケットを入手し、さらに収益化を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="92799-132">In these two subsegments, we are better positioned to acquire the socket with M365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="92799-133">現在、2つの主要な領域があります。 1.</span><span class="sxs-lookup"><span data-stu-id="92799-133">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="92799-134">お客様は成長を促進します。3.</span><span class="sxs-lookup"><span data-stu-id="92799-134">our customer adds growth; 2.</span></span> <span data-ttu-id="92799-135">M365 を使用してクラウドソケットを取得していますが、D365 と Azure には大きなチャンスがあります。</span><span class="sxs-lookup"><span data-stu-id="92799-135">while we do well acquiring cloud sockets leading with M365, we have a large opportunity in D365 and Azure.</span></span>

<span data-ttu-id="92799-136">次のスクリーンショットは、3つの SMB Subsegments と、市場に合わせて最適化されたルートを示しています。</span><span class="sxs-lookup"><span data-stu-id="92799-136">The following screenshot represents the three SMB Subsegments and optimized routes to market.</span></span> <span data-ttu-id="92799-137">CloudAscent は、すべての管理対象外および中規模のビジネスアカウントのプロファイル、スコアリング、およびモデリングに優先順位を付けます。</span><span class="sxs-lookup"><span data-stu-id="92799-137">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="SMB subsegments のスクリーンショット。":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="92799-139">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="92799-139">CloudAscent Machine Learning</span></span>

<span data-ttu-id="92799-140">SMB では、機械学習テクノロジを使用して、上位のアンマネージおよび中規模のビジネスセグメント内の売上およびマーケティング顧客の予測を促進します。</span><span class="sxs-lookup"><span data-stu-id="92799-140">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="92799-141">シグナルはどのように収集され、傾向推奨事項に分類されますか。</span><span class="sxs-lookup"><span data-stu-id="92799-141">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="92799-142">**データ収集**: Web クローラーは、会社のドメインに ping を実行して数十億の顧客信号をスキャンおよび収集し、ブログの投稿、プレスリリース、ソーシャルストリーム、および技術フォーラムを監視します。</span><span class="sxs-lookup"><span data-stu-id="92799-142">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring: blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="92799-143">収集されたシグナルに加えて、c&B、Microsoft 内部サブスクリプション、トランザクションデータなどの内部ソースと外部ソースの両方から、のグラフィック情報が収集されます。</span><span class="sxs-lookup"><span data-stu-id="92799-143">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="92799-144">**Machine Learning**: これらの信号は、クラウド製品とクラスターによって各顧客の売上およびマーケティング予測の構造化データセットを出力する機械学習モデルに取り込まれます。</span><span class="sxs-lookup"><span data-stu-id="92799-144">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="92799-145">各顧客は、お客様の適合性を判断する Microsoft の上位 SMB と、お客様のオンライン行動を意図したとおりに定義する機械学習アルゴリズムを使用して、お客様にスコアを付けます。</span><span class="sxs-lookup"><span data-stu-id="92799-145">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="92799-146">スコアリングは、Microsoft Cloud 製品を購入する顧客の傾向を示すクラスターにマージされます。</span><span class="sxs-lookup"><span data-stu-id="92799-146">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="92799-147">**最適化**: Machine Learning システムは、1か月ごとにトランザクションデータを使用し、四半期ごとにサブスクリプションデータを消費することにより、モデルを最適化します。</span><span class="sxs-lookup"><span data-stu-id="92799-147">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="92799-148">Machine Learning は、win/差損データを使用して、アルゴリズムを調整し、クラスターの推奨事項を MSX で動作する機会と比較することによってモデルが想定どおりに機能していることを検証します。</span><span class="sxs-lookup"><span data-stu-id="92799-148">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB machine learning のスクリーンショット。":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="92799-150">CloudAscent 傾向</span><span class="sxs-lookup"><span data-stu-id="92799-150">CloudAscent Propensity</span></span>

<span data-ttu-id="92799-151">傾向の推奨事項はどのように作成されますか。</span><span class="sxs-lookup"><span data-stu-id="92799-151">How are propensity recommendations created?</span></span>

<span data-ttu-id="92799-152">Web クローラーを介して収集されたシグナルとさまざまなソースから提供されるデータを使用して、紹介しているのは、のグラフィックスデータと顧客のソーシャルメディア信号を統合します。</span><span class="sxs-lookup"><span data-stu-id="92799-152">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="92799-153">スコアリングでは、これらのシグナルとデータを比較モデルとして使用して、目的のモデルに適合とスコアリングを行います。</span><span class="sxs-lookup"><span data-stu-id="92799-153">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="92799-154">お客様のアカウントの適合性</span><span class="sxs-lookup"><span data-stu-id="92799-154">Customer Account Fit</span></span>

   - <span data-ttu-id="92799-155">ファイヤグラフィックを定義する内部および外部のデータポイント。</span><span class="sxs-lookup"><span data-stu-id="92799-155">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="92799-156">スコアリングでは、顧客を比較して Microsoft Cloud 製品に適合するかどうかを確認するために、最適な SMB をモデルとして考えることができます。</span><span class="sxs-lookup"><span data-stu-id="92799-156">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="92799-157">スコア付けの調整は四半期ごとに更新されます</span><span class="sxs-lookup"><span data-stu-id="92799-157">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="92799-158">顧客アカウントの目的</span><span class="sxs-lookup"><span data-stu-id="92799-158">Customer Account Intent</span></span>

   - <span data-ttu-id="92799-159">ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。</span><span class="sxs-lookup"><span data-stu-id="92799-159">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="92799-160">インテントのスコアリングは、クラスターを定義するために、適合の一番上に重なっています。</span><span class="sxs-lookup"><span data-stu-id="92799-160">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="92799-161">インテントスコアリングは毎月更新されます。</span><span class="sxs-lookup"><span data-stu-id="92799-161">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 予測モデル。":::

3. <span data-ttu-id="92799-163">クラスタリング</span><span class="sxs-lookup"><span data-stu-id="92799-163">Clustering</span></span>

   <span data-ttu-id="92799-164">適合とインテントのための信号は、クラスタリングスコアに統合されます。</span><span class="sxs-lookup"><span data-stu-id="92799-164">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="92799-165">CloudAscent には、次の4つのクラスターがあります。</span><span class="sxs-lookup"><span data-stu-id="92799-165">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="92799-166">Now-販売準備ができているお客様</span><span class="sxs-lookup"><span data-stu-id="92799-166">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="92799-167">評価-マーケティングの準備ができている顧客</span><span class="sxs-lookup"><span data-stu-id="92799-167">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="92799-168">育成-ドライブ認識キャンペーン</span><span class="sxs-lookup"><span data-stu-id="92799-168">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="92799-169">教育-目的を教育および監視する</span><span class="sxs-lookup"><span data-stu-id="92799-169">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="92799-170">クラスターを使用すると、製品、geo、業界、および垂直などのセグメント要因に基づいて、顧客が販売およびマーケティングのイニシアチブをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="92799-170">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="92799-171">CloudAscent ブックの [ **傾向 model** ] タブには、傾向と推定の空白の収益が共有されています。</span><span class="sxs-lookup"><span data-stu-id="92799-171">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="92799-172">適合とインテントのクラスタリングを定義するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="92799-172">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="92799-173">ML モデルを使用して、最初に100のスケールでカスタマーフィットスコアとインテントスコアを計算します。</span><span class="sxs-lookup"><span data-stu-id="92799-173">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="92799-174">正確なスコアは、ML モデルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="92799-174">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="92799-175">次のスコアの例:</span><span class="sxs-lookup"><span data-stu-id="92799-175">Example Scores Below:</span></span>

         |<span data-ttu-id="92799-176">**分類**</span><span class="sxs-lookup"><span data-stu-id="92799-176">**Classification**</span></span>|<span data-ttu-id="92799-177">**スコア**</span><span class="sxs-lookup"><span data-stu-id="92799-177">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="92799-178">高</span><span class="sxs-lookup"><span data-stu-id="92799-178">High</span></span>|<span data-ttu-id="92799-179">75 ~ 100</span><span class="sxs-lookup"><span data-stu-id="92799-179">75 - 100</span></span>|
         |<span data-ttu-id="92799-180">Medium</span><span class="sxs-lookup"><span data-stu-id="92799-180">Medium</span></span>|<span data-ttu-id="92799-181">55 ~ 74</span><span class="sxs-lookup"><span data-stu-id="92799-181">55 - 74</span></span>|
         |<span data-ttu-id="92799-182">低</span><span class="sxs-lookup"><span data-stu-id="92799-182">Low</span></span>|<span data-ttu-id="92799-183">30 - 54</span><span class="sxs-lookup"><span data-stu-id="92799-183">30 - 54</span></span>|
         |<span data-ttu-id="92799-184">非常に低い</span><span class="sxs-lookup"><span data-stu-id="92799-184">Very Low</span></span>|<span data-ttu-id="92799-185">0 - 29</span><span class="sxs-lookup"><span data-stu-id="92799-185">0 - 29</span></span>|

      2. <span data-ttu-id="92799-186">上記のルールを使用して、お客様の適合性と目的の信号の両方で、企業を高、中、低、および非常に低いものとして分類しています。</span><span class="sxs-lookup"><span data-stu-id="92799-186">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit    and Intent Signals.</span></span>

      3. <span data-ttu-id="92799-187">傾向を表す各交差部分を含む2D マトリックスに、顧客の適合性とインテントの信号をプロットします。</span><span class="sxs-lookup"><span data-stu-id="92799-187">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span>     <span data-ttu-id="92799-188">たとえば、High Fit + High インテント = A1 は最高の傾向を表します。</span><span class="sxs-lookup"><span data-stu-id="92799-188">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="92799-189">最後に、これらのセグメントグループによってクラスターが形成されます。</span><span class="sxs-lookup"><span data-stu-id="92799-189">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="92799-190">たとえば、A1、A2、A3、A4 は、Act クラスターを形成します。</span><span class="sxs-lookup"><span data-stu-id="92799-190">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent モデル。":::

   <span data-ttu-id="92799-192">これらのお客様には、現在、Act をターゲットにして、顧客を評価することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="92799-192">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="92799-193">CloudAscent 製品 & モデル</span><span class="sxs-lookup"><span data-stu-id="92799-193">CloudAscent Products & Models</span></span>

<span data-ttu-id="92799-194">次の図は、CloudAscent 内の各傾向モデルのビューを示しています。</span><span class="sxs-lookup"><span data-stu-id="92799-194">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向モデル。":::

<span data-ttu-id="92799-196">ホワイトスペースモデルは、既存の Microsoft 顧客が製品を所有していないか、または新しい見込み客となっている顧客の予測で構成されています。</span><span class="sxs-lookup"><span data-stu-id="92799-196">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="92799-197">アップセルモデルでは、トランザクションデータを使用して、Azure と M365 Sku でのアップセルの可能性を予測します。</span><span class="sxs-lookup"><span data-stu-id="92799-197">Upsell models use transaction data to predict the potential for upsell in Azure and M365 SKUs.</span></span>

<span data-ttu-id="92799-198">EOS は、Win 7、Office 2010、SQL Server、および Windows Server のサービスエンドカスタマーを共有します。</span><span class="sxs-lookup"><span data-stu-id="92799-198">EOS shares the end of service customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="92799-199">EOS データは MS Sales から引き出され、CloudAscent 傾向モデリング (使用可能な場合) と連携しています。</span><span class="sxs-lookup"><span data-stu-id="92799-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="92799-200">EOS データは、最新の作業と Azure の販売の役割を果たします。</span><span class="sxs-lookup"><span data-stu-id="92799-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
