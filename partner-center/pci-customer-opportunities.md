---
title: パートナーセンターの洞察-CloudAscent 傾向レポート
description: パートナーセンターの CloudAscent 傾向レポートについて説明します。 Microsoft 製品を購入する顧客の傾向に関する情報が含まれています。
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 91f64faeec0b97be2797d489e152cb84cbb2e192
ms.sourcegitcommit: 8bd2e2f2f0f6bcd0fa202787df5b3c1f786f88f9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/29/2021
ms.locfileid: "108213452"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a><span data-ttu-id="627a4-104">パートナーセンターダッシュボードから使用可能な CloudAscent 傾向レポート</span><span class="sxs-lookup"><span data-stu-id="627a4-104">CloudAscent Propensity reports available from Partner Center dashboard</span></span>

<span data-ttu-id="627a4-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="627a4-105">**Appropriate roles**</span></span>

- <span data-ttu-id="627a4-106">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="627a4-106">Executive report viewer</span></span>
- <span data-ttu-id="627a4-107">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="627a4-107">Report viewer</span></span>

<span data-ttu-id="627a4-108">パートナーセンターダッシュボードは、CloudAscent プログラムからダウンロード可能な傾向データを提供します。</span><span class="sxs-lookup"><span data-stu-id="627a4-108">The Partner Center dashboard provides downloadable propensity data from the CloudAscent program.</span></span> <span data-ttu-id="627a4-109">データは、顧客が Microsoft 製品を購入する可能性を示しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-109">The data shows the customers' likelihood to purchase Microsoft products.</span></span>  <span data-ttu-id="627a4-110">この記事では、このデータの内訳、スコアリングの使用方法、およびその意味について説明します。</span><span class="sxs-lookup"><span data-stu-id="627a4-110">This article describes the breakdown of this data, how to use the scoring, and what it means.</span></span>

## <a name="summary-definitions"></a><span data-ttu-id="627a4-111">概要定義</span><span class="sxs-lookup"><span data-stu-id="627a4-111">Summary definitions</span></span>

- <span data-ttu-id="627a4-112">**SMC のお客様**–傾向のダウンロードにおける顧客の合計数です。</span><span class="sxs-lookup"><span data-stu-id="627a4-112">**SMC Customers**– This is the total number of customers in the propensity downloads.</span></span>  <span data-ttu-id="627a4-113">顧客は、レコードのパートナーによって識別されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-113">Customers are identified by partner of record.</span></span>
- <span data-ttu-id="627a4-114">**契約期限切れ**–現在の会計年度内で、期限切れになった契約の数を提供しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-114">**Expire Agreements**– Within the current fiscal year, we're providing the number of expiring agreements.</span></span>
- <span data-ttu-id="627a4-115">**[有効期限** が迫っている収益] –オープン期限が切れた契約に関連付けられている収益。</span><span class="sxs-lookup"><span data-stu-id="627a4-115">**Open Expiring Revenue**– The revenue associated to the open expiring agreements.</span></span>

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Customers 営業案件の概要ダッシュボードのスクリーンショット。":::

## <a name="cloudascent-smb-segmentation"></a><span data-ttu-id="627a4-117">CloudAscent SMB セグメンテーション</span><span class="sxs-lookup"><span data-stu-id="627a4-117">CloudAscent SMB segmentation</span></span>

<span data-ttu-id="627a4-118">中小企業 (SMB) セグメントは、3つの異なるサブセグメントに分割されています。</span><span class="sxs-lookup"><span data-stu-id="627a4-118">The small to medium business (SMB) segment is divided into three distinct sub segments.</span></span>

1. <span data-ttu-id="627a4-119">**上位の非管理** 対象には、Microsoft の最も多くの機会を持つ最大規模の SMB 顧客が含まれます。</span><span class="sxs-lookup"><span data-stu-id="627a4-119">**Top Unmanaged** includes the largest SMB customers with the most opportunity for Microsoft.</span></span> <span data-ttu-id="627a4-120">一般的な上位の管理されていないお客様は、多数の従業員、大量の IT 予算および支出、Microsoft の収益の可能性を持つ、管理アカウントに類似した特性を共有します。</span><span class="sxs-lookup"><span data-stu-id="627a4-120">Typical Top Unmanaged customers share similar characteristics to Managed accounts, with large number of employees, large IT budgets and spend, and large amounts of potential revenue for Microsoft.</span></span>

   <span data-ttu-id="627a4-121">上位のアンマネージは、次の2つの方法で定義されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-121">We define Top Unmanaged in two ways:</span></span>

   - <span data-ttu-id="627a4-122">上位の管理されていない **ユーザーベース**–300以上の従業員を含むアカウントを含みます。</span><span class="sxs-lookup"><span data-stu-id="627a4-122">**Top Unmanaged User Based**– includes accounts with 300 or more employees.</span></span> <span data-ttu-id="627a4-123">User-Based アカウントは、初回購入の場合は優れたターゲット、Microsoft 365、Dynamics 365、Surface などのユーザーベースのサブスクリプション製品を展開する場合に適しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-123">User-Based accounts are great targets for first-time purchase, or expansion of user-based subscription products such as Microsoft 365, Dynamics 365, or Surface.</span></span>
   - <span data-ttu-id="627a4-124">管理されていない **計算ベースの上位**– Azure が $ 10k を超える可能性のあるアカウントを含みます。</span><span class="sxs-lookup"><span data-stu-id="627a4-124">**Top Unmanaged Compute Based** – includes accounts with Azure potential greater than $10k.</span></span> <span data-ttu-id="627a4-125">コンピューティングベースのアカウントには、既存の Azure が含まれます。</span><span class="sxs-lookup"><span data-stu-id="627a4-125">Compute based accounts include existing Azure.</span></span> <span data-ttu-id="627a4-126">将来、Azure をまだ購入していても、Azure では $ 10k を超える可能性のある azure をまだ購入していない、未来の年の可能性があるアカウントとアカウント。</span><span class="sxs-lookup"><span data-stu-id="627a4-126">accounts with significant future year potential and accounts who have yet to purchase Azure yet but have potential for Azure greater than $10k.</span></span>

2. <span data-ttu-id="627a4-127">**中規模ビジネス** には、既存の顧客と、25 ~ 300 人の従業員を持つ見込み客アカウントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="627a4-127">**Medium Business** includes existing customers and prospect accounts with 25 to 300 employees.</span></span>

3. <span data-ttu-id="627a4-128">**スモールビジネス** には、10-25 人の従業員を抱える企業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="627a4-128">**Small Business** includes businesses with 10-25 employees.</span></span>

4. <span data-ttu-id="627a4-129">**非常に小規模なビジネス** には、従業員が1-9 の企業が含まれています。</span><span class="sxs-lookup"><span data-stu-id="627a4-129">**Very Small Business** includes businesses with 1-9 employees.</span></span>

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="SMC によるお客様の種類。":::

<span data-ttu-id="627a4-131">**上位の管理対象外** および **中規模のビジネス** subsegments は、microsoft および microsoft パートナー向けの高ライフタイム値 (ltv) のお客様を表します。</span><span class="sxs-lookup"><span data-stu-id="627a4-131">**Top Unmanaged** and **Medium Business** subsegments represent high life-time value (LTV) customers for Microsoft, and Microsoft Partners.</span></span> <span data-ttu-id="627a4-132">このため、it 部門は、このセグメントの成長に焦点を当てています。</span><span class="sxs-lookup"><span data-stu-id="627a4-132">Because of this, they're the lead areas of focus for driving growth in this segment.</span></span> <span data-ttu-id="627a4-133">この2つの subsegments では、D365/Azure 基幹業務 (LOB) アプリを使用して、さらに収益化で Microsoft 365 ソケットを取得し、Microsoft 向けの高機能を実現することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="627a4-133">In these two subsegments, we're better positioned to acquire the socket with Microsoft 365, monetize further with D365/Azure line of business (LOB) apps, and realize a high LTV for Microsoft.</span></span>

<span data-ttu-id="627a4-134">現在、2つの主要な領域があります。 1.</span><span class="sxs-lookup"><span data-stu-id="627a4-134">Today we have two key areas of opportunity – 1.</span></span> <span data-ttu-id="627a4-135">お客様は成長を促進します。3.</span><span class="sxs-lookup"><span data-stu-id="627a4-135">our customer adds growth; 2.</span></span> <span data-ttu-id="627a4-136">Microsoft 365 を使用してクラウドソケットを取得していますが、Dynamics 365 と Azure には大きなチャンスがあります。</span><span class="sxs-lookup"><span data-stu-id="627a4-136">while we do well acquiring cloud sockets leading with Microsoft 365, we have a large opportunity in Dynamics 365 and Azure.</span></span>

<span data-ttu-id="627a4-137">次のスクリーンショットは、4つの SMB Subsegments を表しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-137">The following screenshot represents the four SMB Subsegments.</span></span> <span data-ttu-id="627a4-138">CloudAscent は、すべての管理対象外および中規模のビジネスアカウントのプロファイル、スコアリング、およびモデリングに優先順位を付けます。</span><span class="sxs-lookup"><span data-stu-id="627a4-138">CloudAscent prioritize the profiling, scoring, and modeling of all Top Unmanaged and Medium Business accounts.</span></span>

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="SMB subsegments のスクリーンショット。":::

## <a name="cloudascent-machine-learning"></a><span data-ttu-id="627a4-140">CloudAscent Machine Learning</span><span class="sxs-lookup"><span data-stu-id="627a4-140">CloudAscent Machine Learning</span></span>

<span data-ttu-id="627a4-141">SMB では、機械学習テクノロジを使用して、上位のアンマネージおよび中規模のビジネスセグメント内の売上およびマーケティング顧客の予測を促進します。</span><span class="sxs-lookup"><span data-stu-id="627a4-141">SMB uses machine learning technology to drive sales and marketing customer predictions within the Top Unmanaged and Medium Business segments.</span></span> <span data-ttu-id="627a4-142">シグナルはどのように収集され、傾向推奨事項に分類されますか。</span><span class="sxs-lookup"><span data-stu-id="627a4-142">How are signals collected and turned into propensity recommendations?</span></span>

- <span data-ttu-id="627a4-143">**データ収集**: Web クローラーは、会社のドメインに ping を実行し、ブログの投稿、プレスリリース、ソーシャルストリーム、および技術フォーラムを監視して、数十億の顧客信号をスキャンおよび収集します。</span><span class="sxs-lookup"><span data-stu-id="627a4-143">**Data Collection**: Web crawlers scan and collect billions of customer signals by pinging the company domains, and monitoring blog posts, press releases, social streams, and technical forums.</span></span>  <span data-ttu-id="627a4-144">収集されたシグナルに加えて、c&B、Microsoft 内部サブスクリプション、トランザクションデータなどの内部ソースと外部ソースの両方から、のグラフィック情報が収集されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-144">In addition to the collected signals, firmographics information is collected from both internal and external sources such as D&B, Microsoft Internal subscription and transactional data.</span></span>

- <span data-ttu-id="627a4-145">**Machine Learning**: これらの信号は、クラウド製品とクラスターによって各顧客の売上およびマーケティング予測の構造化データセットを出力する機械学習モデルに取り込まれます。</span><span class="sxs-lookup"><span data-stu-id="627a4-145">**Machine Learning**: The signals are fed into the machine learning model that outputs a structured data set of Sales and Marketing predictions for each customer by cloud product and cluster.</span></span>  <span data-ttu-id="627a4-146">各顧客は、お客様の適合性を判断する Microsoft の上位 SMB と、お客様のオンライン行動を意図したとおりに定義する機械学習アルゴリズムを使用して、お客様にスコアを付けます。</span><span class="sxs-lookup"><span data-stu-id="627a4-146">Each customer is scored using a look alike model to Microsoft's top SMB that determines the customer's Fit, and machine learning algorithms that integrate the customer's online behavior define as Intent.</span></span> <span data-ttu-id="627a4-147">スコアリングは、Microsoft Cloud 製品を購入する顧客の傾向を示すクラスターにマージされます。</span><span class="sxs-lookup"><span data-stu-id="627a4-147">The scoring is merged into clusters that show a customer's propensity to purchase Microsoft Cloud Products.</span></span>

- <span data-ttu-id="627a4-148">**最適化**: Machine Learning システムは、1か月ごとにトランザクションデータを使用し、四半期ごとにサブスクリプションデータを消費することにより、モデルを最適化します。</span><span class="sxs-lookup"><span data-stu-id="627a4-148">**Optimization**: The Machine Learning system optimizes the models by consuming the transaction data monthly and the subscription data quarterly.</span></span>  <span data-ttu-id="627a4-149">Machine Learning は、win/差損データを使用して、アルゴリズムを調整し、クラスターの推奨事項を MSX で動作する機会と比較することによってモデルが想定どおりに機能していることを検証します。</span><span class="sxs-lookup"><span data-stu-id="627a4-149">Using the win/loss data, the Machine Learning adjusts the algorithms and validates that the models are working as expected by comparing cluster recommendations to opportunities acted upon in MSX.</span></span>

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="SMB machine learning のスクリーンショット。":::

## <a name="cloudascent-propensity"></a><span data-ttu-id="627a4-151">CloudAscent 傾向</span><span class="sxs-lookup"><span data-stu-id="627a4-151">CloudAscent Propensity</span></span>

<span data-ttu-id="627a4-152">傾向の推奨事項はどのように作成されますか。</span><span class="sxs-lookup"><span data-stu-id="627a4-152">How are propensity recommendations created?</span></span>

<span data-ttu-id="627a4-153">Web クローラーを介して収集されたシグナルとさまざまなソースから提供されるデータを使用して、紹介しているのは、のグラフィックスデータと顧客のソーシャルメディア信号を統合します。</span><span class="sxs-lookup"><span data-stu-id="627a4-153">Using signals collected via web crawlers and data provided from various sources, we consolidate the firmographics data and customer's social media signals.</span></span>  <span data-ttu-id="627a4-154">スコアリングでは、これらのシグナルとデータを比較モデルとして使用して、目的のモデルに適合とスコアリングを行います。</span><span class="sxs-lookup"><span data-stu-id="627a4-154">The scoring uses these signals and data in comparison models for fit and scoring models for Intent.</span></span>

1. <span data-ttu-id="627a4-155">お客様のアカウントの適合性</span><span class="sxs-lookup"><span data-stu-id="627a4-155">Customer Account Fit</span></span>

   - <span data-ttu-id="627a4-156">ファイヤグラフィックを定義する内部および外部のデータポイント。</span><span class="sxs-lookup"><span data-stu-id="627a4-156">Internal and External data points that define firmographics.</span></span>

   - <span data-ttu-id="627a4-157">スコアリングでは、顧客を比較して Microsoft Cloud 製品に適合するかどうかを確認するために、最適な SMB をモデルとして考えることができます。</span><span class="sxs-lookup"><span data-stu-id="627a4-157">Fit scoring uses a look alike model to our best SMB to compare customers and see if they're a potential  fit for Microsoft Cloud Products.</span></span>

   - <span data-ttu-id="627a4-158">スコア付けの調整は四半期ごとに更新されます</span><span class="sxs-lookup"><span data-stu-id="627a4-158">Fit scoring is updated quarterly</span></span>

2. <span data-ttu-id="627a4-159">顧客アカウントの目的</span><span class="sxs-lookup"><span data-stu-id="627a4-159">Customer Account Intent</span></span>

   - <span data-ttu-id="627a4-160">ソーシャルメディアに関連するシグナルと、顧客のオンライン動作によってインテントが定義されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-160">Signals related to Social media and a customer's online behavior define Intent.</span></span>

   - <span data-ttu-id="627a4-161">インテントのスコアリングは、クラスターを定義するために、適合の一番上に重なっています。</span><span class="sxs-lookup"><span data-stu-id="627a4-161">Intent scoring is overlaid on top of fit to define the clusters.</span></span>

   - <span data-ttu-id="627a4-162">インテントスコアリングは毎月更新されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-162">Intent scoring is updated monthly.</span></span>

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="CloudAscent SMB 予測モデル。":::

3. <span data-ttu-id="627a4-164">クラスタリング</span><span class="sxs-lookup"><span data-stu-id="627a4-164">Clustering</span></span>

   <span data-ttu-id="627a4-165">適合とインテントのための信号は、クラスタリングスコアに統合されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-165">The Signals for fit and intent are consolidated into a clustering score.</span></span> <span data-ttu-id="627a4-166">CloudAscent には、次の4つのクラスターがあります。</span><span class="sxs-lookup"><span data-stu-id="627a4-166">CloudAscent has four clusters:</span></span>

      - <span data-ttu-id="627a4-167">Now-販売準備ができているお客様</span><span class="sxs-lookup"><span data-stu-id="627a4-167">Act Now - sales ready customers</span></span>
      - <span data-ttu-id="627a4-168">評価-マーケティングの準備ができている顧客</span><span class="sxs-lookup"><span data-stu-id="627a4-168">Evaluate - marketing ready customers</span></span>
      - <span data-ttu-id="627a4-169">育成-ドライブ認識キャンペーン</span><span class="sxs-lookup"><span data-stu-id="627a4-169">Nurture - drive awareness campaigns</span></span>
      - <span data-ttu-id="627a4-170">教育-目的を教育および監視する</span><span class="sxs-lookup"><span data-stu-id="627a4-170">Educate - educate and monitor for intent</span></span>

   <span data-ttu-id="627a4-171">クラスターを使用すると、製品、geo、業界、および垂直などのセグメント要因に基づいて、顧客が販売およびマーケティングのイニシアチブをターゲットにすることができます。</span><span class="sxs-lookup"><span data-stu-id="627a4-171">The clustering allows users to target specific customers for sales and marketing initiatives based on segment factors, for example: product, geo, industry and vertical.</span></span>

   <span data-ttu-id="627a4-172">CloudAscent ブックの [ **傾向 model** ] タブには、傾向と推定の空白の収益が共有されています。</span><span class="sxs-lookup"><span data-stu-id="627a4-172">The **Propensity model** tab in the CloudAscent Workbooks shares the propensity and the estimated whitespace revenue.</span></span> <span data-ttu-id="627a4-173">適合とインテントのクラスタリングを定義するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="627a4-173">To define the clustering of Fit and Intent, we go through the following steps:</span></span>

      1. <span data-ttu-id="627a4-174">ML モデルを使用して、最初に100のスケールでカスタマーフィットスコアとインテントスコアを計算します。</span><span class="sxs-lookup"><span data-stu-id="627a4-174">Using ML Models, we first calculate Customer Fit Score and intent Score on a scale of 100.</span></span>  <span data-ttu-id="627a4-175">正確なスコアは、ML モデルによって異なります。</span><span class="sxs-lookup"><span data-stu-id="627a4-175">Exact Scores will vary based on ML Models.</span></span>  <span data-ttu-id="627a4-176">次のスコアの例:</span><span class="sxs-lookup"><span data-stu-id="627a4-176">Example Scores Below:</span></span>

         |<span data-ttu-id="627a4-177">**分類**</span><span class="sxs-lookup"><span data-stu-id="627a4-177">**Classification**</span></span>|<span data-ttu-id="627a4-178">**スコア**</span><span class="sxs-lookup"><span data-stu-id="627a4-178">**Score**</span></span>|
         |---------|:---------|
         |<span data-ttu-id="627a4-179">高</span><span class="sxs-lookup"><span data-stu-id="627a4-179">High</span></span>|<span data-ttu-id="627a4-180">75 ~ 100</span><span class="sxs-lookup"><span data-stu-id="627a4-180">75 - 100</span></span>|
         |<span data-ttu-id="627a4-181">Medium</span><span class="sxs-lookup"><span data-stu-id="627a4-181">Medium</span></span>|<span data-ttu-id="627a4-182">55 ~ 74</span><span class="sxs-lookup"><span data-stu-id="627a4-182">55 - 74</span></span>|
         |<span data-ttu-id="627a4-183">低</span><span class="sxs-lookup"><span data-stu-id="627a4-183">Low</span></span>|<span data-ttu-id="627a4-184">30 - 54</span><span class="sxs-lookup"><span data-stu-id="627a4-184">30 - 54</span></span>|
         |<span data-ttu-id="627a4-185">非常に低い</span><span class="sxs-lookup"><span data-stu-id="627a4-185">Very Low</span></span>|<span data-ttu-id="627a4-186">0 - 29</span><span class="sxs-lookup"><span data-stu-id="627a4-186">0 - 29</span></span>|

      2. <span data-ttu-id="627a4-187">上記のルールを使用して、お客様の適合性と目的の信号の両方で、企業を高、中、低、および非常に低いものとして分類しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-187">Using the rule above, we classify companies to be High, Medium, Low, and Very Low across both Customer Fit and Intent Signals.</span></span>

      3. <span data-ttu-id="627a4-188">傾向を表す各交差部分を含む2D マトリックスに、顧客の適合性とインテントの信号をプロットします。</span><span class="sxs-lookup"><span data-stu-id="627a4-188">We plot customer fit and intent signals on a 2D matrix with each intersection representing the propensity.</span></span> <span data-ttu-id="627a4-189">たとえば、High Fit + High インテント = A1 は最高の傾向を表します。</span><span class="sxs-lookup"><span data-stu-id="627a4-189">For Example, High Fit + High Intent = A1, representing the highest propensity.</span></span>

      4. <span data-ttu-id="627a4-190">最後に、これらのセグメントグループによってクラスターが形成されます。</span><span class="sxs-lookup"><span data-stu-id="627a4-190">Finally, these segments group to form clusters.</span></span>  <span data-ttu-id="627a4-191">たとえば、A1、A2、A3、A4 は、Act クラスターを形成します。</span><span class="sxs-lookup"><span data-stu-id="627a4-191">For Example, A1, A2, A3, A4 form the Act Now cluster.</span></span>

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="CloudAscent モデル。":::

   <span data-ttu-id="627a4-193">これらのお客様には、現在、Act をターゲットにして、顧客を評価することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="627a4-193">For these customers, we recommend targeting Act Now and Evaluate customers.</span></span>

## <a name="cloudascent-products--models"></a><span data-ttu-id="627a4-194">CloudAscent 製品 & モデル</span><span class="sxs-lookup"><span data-stu-id="627a4-194">CloudAscent Products & Models</span></span>

<span data-ttu-id="627a4-195">次の図は、CloudAscent 内の各傾向モデルのビューを示しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-195">The following graphic provides a view of each propensity model within CloudAscent:</span></span>

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="CloudAscent 傾向モデル。":::

<span data-ttu-id="627a4-197">ホワイトスペースモデルは、既存の Microsoft 顧客が製品を所有していないか、または新しい見込み客となっている顧客の予測で構成されています。</span><span class="sxs-lookup"><span data-stu-id="627a4-197">Whitespace models are composed of predictions for existing Microsoft customers where they don't have a product and/or are net new prospect customers.</span></span>

<span data-ttu-id="627a4-198">アップセルモデルでは、トランザクションデータを使用して、Azure と Microsoft 365 Sku でのアップセルの可能性を予測します。</span><span class="sxs-lookup"><span data-stu-id="627a4-198">Upsell models use transaction data to predict the potential for upsell in Azure and Microsoft 365 SKUs.</span></span>

<span data-ttu-id="627a4-199">これらのお客様は既に Azure と Microsoft 365 の両方を所有しており、アップセルモデルは既存の SKU を追加購入する可能性があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-199">These customers will already have both Azure or Microsoft 365 and the upsell model shows that they’re likely to purchase more of their existing SKU.</span></span>

<span data-ttu-id="627a4-200">EOS は、Win 7、Office 2010、SQL Server、および Windows Server のサービス終了 (EOS) 顧客を共有します。</span><span class="sxs-lookup"><span data-stu-id="627a4-200">EOS shares the end of service (EOS) customers for Win 7, Office 2010, SQL Server, and Windows Server.</span></span> <span data-ttu-id="627a4-201">EOS データは MS Sales から引き出され、CloudAscent 傾向モデリング (使用可能な場合) と連携しています。</span><span class="sxs-lookup"><span data-stu-id="627a4-201">The EOS data is pulled from MS Sales and overlaid with the CloudAscent propensity modeling where available.</span></span> <span data-ttu-id="627a4-202">EOS データは、最新の作業と Azure の販売の役割を果たします。</span><span class="sxs-lookup"><span data-stu-id="627a4-202">EOS data lives in the Modern Work and Azure Sales plays.</span></span>
