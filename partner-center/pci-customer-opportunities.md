---
title: パートナー センター Insights - CloudAscent の傾向レポート
description: CloudAscent の傾向レポートについては、パートナー センター。 Microsoft 製品を購入する顧客の傾向に関する情報が含まれます。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153040"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="06fe3-104">CloudAscent の傾向レポートは、ダッシュボードからパートナー センターできます</span><span class="sxs-lookup"><span data-stu-id="06fe3-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="06fe3-105">**適切なロール**: エグゼクティブ レポート ビューアー |レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="06fe3-105">**Appropriate roles**: Executive report viewer | Report viewer</span></span>

<span data-ttu-id="06fe3-106">[パートナー センターダッシュボードには、CloudAscent プログラムからダウンロード可能な傾向データが表示されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-106">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="06fe3-107">このデータは、顧客が Microsoft 製品を購入する可能性を示しています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-107">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="06fe3-108">この記事では、このデータの内訳、スコアリングの使い方、および意味について説明します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-108">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="06fe3-109">概要の定義</span><span class="sxs-lookup"><span data-stu-id="06fe3-109">Summary definitions</span></span>

- <span data-ttu-id="06fe3-110">**SMC のお** 客様 – これは、傾向のダウンロードに含まれる顧客の総数です。</span><span class="sxs-lookup"><span data-stu-id="06fe3-110">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="06fe3-111">顧客はレコードのパートナーによって識別されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-111">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="06fe3-112">**契約の期限切** れ – 現在の会計年度内に、期限切れの契約の数を提供しています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-112">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="06fe3-113">**Open Expiring Revenue**– オープン期限切れの契約に関連付けられている収益。</span><span class="sxs-lookup"><span data-stu-id="06fe3-113">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Customers Opportunities Summary ダッシュボードのスクリーンショット。":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="06fe3-115">CloudAscent SMB のセグメント化</span><span class="sxs-lookup"><span data-stu-id="06fe3-115">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="06fe3-116">中小企業 (SMB) セグメントは、3 つの異なるサブセグメントに分割されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-116">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="06fe3-117">**管理されていない上位には** 、Microsoft にとって最も多くの機会を持つ最大の SMB 顧客が含まれています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-117">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="06fe3-118">一般的なトップ アンマネージドのお客様は、マネージド アカウントと同様の特性を共有しています。従業員の数が多く、IT の予算と支出が多く、Microsoft の収益が多い可能性があります。</span><span class="sxs-lookup"><span data-stu-id="06fe3-118">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="06fe3-119">Top Unmanaged は、次の 2 つの方法で定義します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-119">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="06fe3-120">**上位のアンマネージド ユーザー ベース**– 300 人以上の従業員を持つアカウントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-120">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="06fe3-121">User-Based アカウントは、初回購入の場合は優れたターゲット、Microsoft 365、Dynamics 365、Surface などのユーザーベースのサブスクリプション製品を展開する場合に適しています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-121">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="06fe3-122">管理されていない **計算ベースの上位**– Azure が $ 10k を超える可能性のあるアカウントを含みます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-122">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="06fe3-123">コンピューティングベースのアカウントには、既存の Azure が含まれます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-123">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="06fe3-124">将来、Azure をまだ購入していても、Azure では $ 10k を超える可能性のある azure をまだ購入していない、未来の年の可能性があるアカウントとアカウント。</span><span class="sxs-lookup"><span data-stu-id="06fe3-124">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="06fe3-125">**中規模ビジネス** には、既存の顧客と、25 ~ 300 人の従業員を持つ見込み客アカウントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-125">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="06fe3-126">**スモールビジネス** には、10-25 人の従業員を抱える企業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-126">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="06fe3-127">**非常に小規模なビジネス** には、従業員が1-9 の企業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-127">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC によるお客様の種類。":::

<span data-ttu-id="06fe3-129">**上位の管理対象外** および **中規模のビジネス** subsegments は、microsoft および microsoft パートナー向けの高ライフタイム値 (ltv) のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-129">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="06fe3-130">このため、it 部門は、このセグメントの成長に焦点を当てています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-130">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="06fe3-131">この2つの subsegments では、D365/Azure 基幹業務 (LOB) アプリを使用して、さらに収益化で Microsoft 365 ソケットを取得し、Microsoft 向けの高機能を実現することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="06fe3-131">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="06fe3-132">現在、2つの主要な領域があります。 1.</span><span class="sxs-lookup"><span data-stu-id="06fe3-132">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="06fe3-133">お客様は成長を促進します。3.</span><span class="sxs-lookup"><span data-stu-id="06fe3-133">our customer adds growth; 2.</span></span> <span data-ttu-id="06fe3-134">Microsoft 365 を使用してクラウドソケットを取得していますが、Dynamics 365 と Azure には大きなチャンスがあります。</span><span class="sxs-lookup"><span data-stu-id="06fe3-134">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="06fe3-135">次のスクリーンショットは、4つの SMB Subsegments を表しています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-135">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="06fe3-136">CloudAscent は、すべての管理対象外および中規模のビジネスアカウントのプロファイル、スコアリング、およびモデリングに優先順位を付けます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-136">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB subsegments のスクリーンショット。":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="06fe3-138">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="06fe3-138">CloudAscent Machine Learning</span></span>

<span data-ttu-id="06fe3-139">SMB では、機械学習テクノロジを使用して、上位のアンマネージおよび中規模のビジネスセグメント内の売上およびマーケティング顧客の予測を促進します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-139">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="06fe3-140">シグナルはどのように収集され、傾向推奨事項に分類されますか。</span><span class="sxs-lookup"><span data-stu-id="06fe3-140">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="06fe3-141">**データ収集**: Web クローラーは、会社のドメインに ping を実行し、ブログの投稿、ニュース リリース、ソーシャル ストリーム、技術フォーラムを監視することで、数十億の顧客シグナルをスキャンして収集します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-141">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="06fe3-142">収集されたシグナルに加えて、企業情報は、D&B、Microsoft 内部サブスクリプション、トランザクション データなどの内部ソースと外部ソースの両方から収集されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-142">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="06fe3-143">**Machine Learning:** シグナルは機械学習モデルに送り込まれており、クラウド製品とクラスターによって顧客ごとに売上とマーケティングの予測の構造化されたデータ セットが出力されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-143">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="06fe3-144">各顧客は、顧客の適合を決定する Microsoft の上位 SMB に似たモデルを使用してスコア付けされ、顧客のオンライン動作を統合する機械学習アルゴリズムは意図として定義されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-144">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="06fe3-145">スコアリングは、Microsoft Cloud Products を購入する顧客の傾向を示すクラスターにマージされます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-145">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="06fe3-146">**最適化**: Machine Learningトランザクション データとサブスクリプション データを四半期ごとに使用することで、モデルを最適化します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-146">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="06fe3-147">Machine Learning は、win/loss データを使用してアルゴリズムを調整し、クラスターの推奨事項と MSX で動作する機会を比較することで、モデルが期待通り動作している検証を行います。</span><span class="sxs-lookup"><span data-stu-id="06fe3-147">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB 機械学習のスクリーンショット。":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="06fe3-149">CloudAscent の傾向</span><span class="sxs-lookup"><span data-stu-id="06fe3-149">CloudAscent Propensity</span></span>

<span data-ttu-id="06fe3-150">傾向に関する推奨事項の作成方法</span><span class="sxs-lookup"><span data-stu-id="06fe3-150">How are propensity recommendations created?</span></span>

<span data-ttu-id="06fe3-151">Web クローラーを介して収集された信号とさまざまなソースから提供されるデータを使用して、企業データと顧客のソーシャル メディアシグナルを統合します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-151">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="06fe3-152">スコアリングでは、インテントの適合モデルとスコア付けモデルに対して、これらのシグナルとデータが比較モデルで使用されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-152">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="06fe3-153">顧客アカウントの適合</span><span class="sxs-lookup"><span data-stu-id="06fe3-153">Customer Account Fit</span></span>

   - <span data-ttu-id="06fe3-154">企業図を定義する内部データ ポイントと外部データ ポイント。</span><span class="sxs-lookup"><span data-stu-id="06fe3-154">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="06fe3-155">適合スコアリングでは、Microsoft の最適な SMB に似たモデルを使用して、顧客を比較し、Microsoft Cloud Products に適合する可能性がある場合を確認します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-155">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="06fe3-156">Fit スコアリングが四半期ごとに更新される</span><span class="sxs-lookup"><span data-stu-id="06fe3-156">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="06fe3-157">顧客アカウントの意図</span><span class="sxs-lookup"><span data-stu-id="06fe3-157">Customer Account Intent</span></span>

   - <span data-ttu-id="06fe3-158">ソーシャル メディアと顧客のオンライン動作に関連するシグナルは、意図を定義します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-158">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="06fe3-159">インテントのスコアリングは、クラスターを定義するために、適合の一番上に重なっています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-159">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="06fe3-160">インテントスコアリングは毎月更新されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-160">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 予測モデル。":::

3. <span data-ttu-id="06fe3-162">クラスタリング</span><span class="sxs-lookup"><span data-stu-id="06fe3-162">Clustering</span></span>

   <span data-ttu-id="06fe3-163">適合とインテントのための信号は、クラスタリングスコアに統合されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-163">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="06fe3-164">CloudAscent には、次の4つのクラスターがあります。</span><span class="sxs-lookup"><span data-stu-id="06fe3-164">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="06fe3-165">Now-販売準備ができているお客様</span><span class="sxs-lookup"><span data-stu-id="06fe3-165">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="06fe3-166">評価-マーケティングの準備ができている顧客</span><span class="sxs-lookup"><span data-stu-id="06fe3-166">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="06fe3-167">育成-ドライブ認識キャンペーン</span><span class="sxs-lookup"><span data-stu-id="06fe3-167">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="06fe3-168">教育-目的を教育および監視する</span><span class="sxs-lookup"><span data-stu-id="06fe3-168">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="06fe3-169">クラスターを使用すると、製品、geo、業界、および垂直などのセグメント要因に基づいて、顧客が販売およびマーケティングのイニシアチブをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-169">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="06fe3-170">CloudAscent ブックの [ **傾向 model** ] タブには、傾向と推定の空白の収益が共有されています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-170">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="06fe3-171">適合とインテントのクラスタリングを定義するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-171">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="06fe3-172">ML モデルを使用して、最初に100のスケールでカスタマーフィットスコアとインテントスコアを計算します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-172">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="06fe3-173">正確なスコアは、ML モデルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="06fe3-173">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="06fe3-174">次のスコアの例:</span><span class="sxs-lookup"><span data-stu-id="06fe3-174">Example Scores Below:</span></span>

         |<span data-ttu-id="06fe3-175">**分類**</span><span class="sxs-lookup"><span data-stu-id="06fe3-175">**Classification**</span></span>|<span data-ttu-id="06fe3-176">**スコア**</span><span class="sxs-lookup"><span data-stu-id="06fe3-176">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="06fe3-177">高</span><span class="sxs-lookup"><span data-stu-id="06fe3-177">High</span></span>|<span data-ttu-id="06fe3-178">75 ~ 100</span><span class="sxs-lookup"><span data-stu-id="06fe3-178">75 - 100</span></span>|
         |<span data-ttu-id="06fe3-179">Medium</span><span class="sxs-lookup"><span data-stu-id="06fe3-179">Medium</span></span>|<span data-ttu-id="06fe3-180">55 ~ 74</span><span class="sxs-lookup"><span data-stu-id="06fe3-180">55 - 74</span></span>|
         |<span data-ttu-id="06fe3-181">低</span><span class="sxs-lookup"><span data-stu-id="06fe3-181">Low</span></span>|<span data-ttu-id="06fe3-182">30 - 54</span><span class="sxs-lookup"><span data-stu-id="06fe3-182">30 - 54</span></span>|
         |<span data-ttu-id="06fe3-183">非常に低い</span><span class="sxs-lookup"><span data-stu-id="06fe3-183">Very Low</span></span>|<span data-ttu-id="06fe3-184">0 - 29</span><span class="sxs-lookup"><span data-stu-id="06fe3-184">0 - 29</span></span>|

      2. <span data-ttu-id="06fe3-185">上記のルールを使用して、Customer Fit シグナルと Intent Signals の両方で、企業を High、Medium、Low、Very Low に分類します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-185">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="06fe3-186">顧客の適合と意図のシグナルを 2D マトリックスにプロットし、各交差部分が傾向を表します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-186">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="06fe3-187">たとえば、最も高い傾向を表す高適合 + 高意図 = A1 です。</span><span class="sxs-lookup"><span data-stu-id="06fe3-187">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="06fe3-188">最後に、これらのセグメントはクラスターを形成するためにグループ化されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-188">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="06fe3-189">たとえば、A1、A2、A3、A4 は Act Now クラスターを形成します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-189">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent モデル。":::

   <span data-ttu-id="06fe3-191">これらのお客様には、Act Now と Evaluate customers をターゲットにすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="06fe3-191">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="06fe3-192">CloudAscent Products & モデル</span><span class="sxs-lookup"><span data-stu-id="06fe3-192">CloudAscent Products & Models</span></span>

<span data-ttu-id="06fe3-193">次の図は、CloudAscent 内の各傾向モデルのビューを示しています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-193">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向モデル。":::

<span data-ttu-id="06fe3-195">空白モデルは、製品を持っなかったり、新規の見込み客である既存の Microsoft 顧客の予測で構成されています。</span><span class="sxs-lookup"><span data-stu-id="06fe3-195">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="06fe3-196">アップセル モデルでは、トランザクション データを使用して、Azure でのアップセルの可能性を予測し、SKU Microsoft 365します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-196">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="06fe3-197">これらの顧客は既に Azure と Microsoft 365 の両方を持っています。アップセル モデルでは、既存の SKU の購入が多い可能性が高いという結果が示されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-197">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="06fe3-198">EOS は、Win 7、Office 2010、SQL Server、Windows Server のサービス終了 (EOS) のお客様を共有します。</span><span class="sxs-lookup"><span data-stu-id="06fe3-198">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="06fe3-199">EOS データは MS Sales からプルされ、使用可能な場合は CloudAscent 傾向モデリングでオーバーレイされます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-199">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="06fe3-200">EOS データは Modern Work に保存され、Azure Sales が再生されます。</span><span class="sxs-lookup"><span data-stu-id="06fe3-200">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
