---
title: Power BI 用パートナー センター分析アプリ | パートナー センター
ms.topic: article
ms.date: 03/15/2019
description: Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) の使用方法を説明します。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 085fcb059a11b487c69ba64d9c411b173ed48c6b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134572"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="e9e74-103">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="e9e74-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

<span data-ttu-id="e9e74-104">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="e9e74-104">**Applies to**</span></span>

-   <span data-ttu-id="e9e74-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="e9e74-105">Partner Center</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="e9e74-106">ビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="e9e74-106">View your business data</span></span>

<span data-ttu-id="e9e74-107">Power BI 用パートナー センター分析アプリでは、ビジネス データの視覚表現を利用できます。以下に例を示します。</span><span class="sxs-lookup"><span data-stu-id="e9e74-107">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="e9e74-108">顧客数、サブスクリプション数、ライセンス数の増加</span><span class="sxs-lookup"><span data-stu-id="e9e74-108">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="e9e74-109">Office 365、Microsoft Dynamics、Microsoft Azure の製品の使用量</span><span class="sxs-lookup"><span data-stu-id="e9e74-109">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="e9e74-110">過去 60 日間の各 Azure サブスクリプションにおける従量制課金リソースごとの 1 日当たりの消費単位</span><span class="sxs-lookup"><span data-stu-id="e9e74-110">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="e9e74-111">(最新の価格カードに基づく) 推定コスト</span><span class="sxs-lookup"><span data-stu-id="e9e74-111">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="e9e74-112">データセットのエクスポートおよびカスタム レポート作成 (顧客別など) の機能</span><span class="sxs-lookup"><span data-stu-id="e9e74-112">Ability to export datasets and create custom reports, including per customer</span></span> 

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="e9e74-113">パートナー センターの分析のアプリのプレビュー リリースについて</span><span class="sxs-lookup"><span data-stu-id="e9e74-113">About the Partner Center Analytics app preview release</span></span>

 - <span data-ttu-id="e9e74-114">このアプリは、クラウド ソリューション プロバイダー プログラムの直接パートナーのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="e9e74-114">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="e9e74-115">CSP の他のパートナー (間接リセラーなど) はログインできません。</span><span class="sxs-lookup"><span data-stu-id="e9e74-115">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="e9e74-116">見積もりコストはすべて税抜きの請求データであり、法的拘束力を持ちません。</span><span class="sxs-lookup"><span data-stu-id="e9e74-116">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="e9e74-117">推定コストは、データ インサイトの目的のみで使用することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="e9e74-117">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="e9e74-118">顧客情報は、サブスクリプションに基づきます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-118">Customer information is based on subscriptions.</span></span> <span data-ttu-id="e9e74-119">最近、アカウントを作成し、まだサブスクリプションがない顧客はカウントされません。</span><span class="sxs-lookup"><span data-stu-id="e9e74-119">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span> 

- <span data-ttu-id="e9e74-120">推定コストは、最新の価格カード (CSP 価格に基づく) を使って算出されます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-120">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span> 

- <span data-ttu-id="e9e74-121">日数は暦日です。</span><span class="sxs-lookup"><span data-stu-id="e9e74-121">Days are calendar days.</span></span> 


### <a name="business-insights-report"></a><span data-ttu-id="e9e74-122">ビジネス インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="e9e74-122">Business Insights report</span></span>

-  <span data-ttu-id="e9e74-123">**顧客テナント**:個別の Azure のサブスクリプションを購入した顧客の AD テナント</span><span class="sxs-lookup"><span data-stu-id="e9e74-123">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

-  <span data-ttu-id="e9e74-124">**新しい (過去 30 日)**:新しい顧客が過去 30 日間に少なくとも 1 つのサブスクリプションの購入</span><span class="sxs-lookup"><span data-stu-id="e9e74-124">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

-  <span data-ttu-id="e9e74-125">**(過去 30 日間) のチャーン**:お客様を"active"、"で猶予"または"disabled"サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-125">**Churn (last 30 days)**: Customers without any “active”, “in grace” or “disabled” subscriptions</span></span>

- <span data-ttu-id="e9e74-126">**新しい (過去 24 時間)**:新しい顧客が過去 24 時間に少なくとも 1 つのサブスクリプションの購入</span><span class="sxs-lookup"><span data-stu-id="e9e74-126">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="e9e74-127">**過去 12 か月間の推定月間コスト**:推定税引き前の請求金額の傾向を 1 か月の前月が過去 12 か月間の期間の月単位で集計</span><span class="sxs-lookup"><span data-stu-id="e9e74-127">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e9e74-128">**製品で過去 12 か月間の推定コスト**:推定税引き前の請求金額を並べ替えて販売されている製品は、過去 12 か月間の期間にわたって集計されます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-128">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="e9e74-129">これにより、収益性の高い主力製品が明確になります。</span><span class="sxs-lookup"><span data-stu-id="e9e74-129">This will indicate top products bringing most revenue.</span></span>

- <span data-ttu-id="e9e74-130">**過去 12 か月間以上の顧客**:過去 12 か月間の期間の月単位の新規の顧客や顧客のチャーンか月ごとの傾向を 1 か月の集計</span><span class="sxs-lookup"><span data-stu-id="e9e74-130">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e9e74-131">**過去 12 か月間の推定コストを顧客が**:顧客の過去 12 か月間の期間にわたって集計された推定税引き前の請求金額で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-131">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="e9e74-132">これにより、収益性の高い主要顧客が明確になります。</span><span class="sxs-lookup"><span data-stu-id="e9e74-132">This will indicate top customers bringing most revenue.</span></span>

- <span data-ttu-id="e9e74-133">**製品別の顧客数**:製品は販売関連付けられている顧客によって並べ替えられています。</span><span class="sxs-lookup"><span data-stu-id="e9e74-133">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="e9e74-134">これにより、多くの顧客が購入した主力製品が明らかになります。</span><span class="sxs-lookup"><span data-stu-id="e9e74-134">This will indicate top products sold to most customers.</span></span> 


### <a name="subscription-insights-report"></a><span data-ttu-id="e9e74-135">サブスクリプション インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="e9e74-135">Subscription Insights report</span></span> 

- <span data-ttu-id="e9e74-136">**Subscription status** (サブスクリプションの状態): </span><span class="sxs-lookup"><span data-stu-id="e9e74-136">**Subscription status**:</span></span>

    - <span data-ttu-id="e9e74-137">アクティブ:サブスクリプションの"猶予"または「アクティブ」に属する状態</span><span class="sxs-lookup"><span data-stu-id="e9e74-137">Active: Subscriptions belonging to either “active” or “in grace” state</span></span>

    - <span data-ttu-id="e9e74-138">中断。「無効」状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-138">Suspended: Subscriptions belonging to “disabled” state</span></span>

    - <span data-ttu-id="e9e74-139">プロビジョニング解除します。属するサブスクリプションが「プロビジョニング解除」または「期限切れ」の状態</span><span class="sxs-lookup"><span data-stu-id="e9e74-139">De-provisioned: Subscriptions belonging to “de-provisioned” or “expired” status</span></span>

- <span data-ttu-id="e9e74-140">**Expiry status** (有効期限の状態): </span><span class="sxs-lookup"><span data-stu-id="e9e74-140">**Expiry status**:</span></span>

    - <span data-ttu-id="e9e74-141">［有効期限切れ］:既に有効期限の切れたサブスクリプション (サブスクリプションの終了日が、これまで)</span><span class="sxs-lookup"><span data-stu-id="e9e74-141">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

    - <span data-ttu-id="e9e74-142">30 日後に期限切れになりません。(サブスクリプションの終了日は、次の 30 日後に)、30 日後に期限切れサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-142">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

    - <span data-ttu-id="e9e74-143">30 日以内に期限切れになりません。サブスクリプション (サブスクリプションの終了日は現在および今後 30 日間)、[次へ] の 30 日以内に切れる</span><span class="sxs-lookup"><span data-stu-id="e9e74-143">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

-  <span data-ttu-id="e9e74-144">**サブスクリプションの合計**:「アクティブ」でのサブスクリプションの"猶予"または「無効」の状態</span><span class="sxs-lookup"><span data-stu-id="e9e74-144">**Total subscriptions**: Subscriptions in “active,” “in grace” or “disabled” status</span></span>

- <span data-ttu-id="e9e74-145">**新しい (過去 30 日)**:過去 30 日以内に顧客が購入した新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-145">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="e9e74-146">**新しい (過去 24 時間)**:過去 24 時間以内に顧客が購入した新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-146">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="e9e74-147">**30 日以内に期限切れにならない**:次の 30 日以内の有効期限のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e9e74-147">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="e9e74-148">**(過去 30 日間) のチャーン**:逆にプロビジョニングされたサブスクリプションまたは Suspended の過去 30 日以内には、(無効)</span><span class="sxs-lookup"><span data-stu-id="e9e74-148">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="e9e74-149">**Distribution by subscription types** (サブスクリプションの種類別分布率): 全サブスクリプションのライセンス ベースと利用量ベースのサブスクリプションの種類別分布率</span><span class="sxs-lookup"><span data-stu-id="e9e74-149">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage based subscription type</span></span>

- <span data-ttu-id="e9e74-150">**製品別のアクティブなサブスクリプション数**:アクティブなサブスクリプションの数によって並べ替えられて販売されている製品</span><span class="sxs-lookup"><span data-stu-id="e9e74-150">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="e9e74-151">**過去 12 か月間のサブスクリプション**:過去 12 か月間の期間の月単位の新規のサブスクリプションとサブスクリプションの変更頻度か月ごとの傾向を 1 か月の集計</span><span class="sxs-lookup"><span data-stu-id="e9e74-151">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e9e74-152">**顧客サブスクリプションの詳細**:顧客、サブスクリプション プランの詳細の表示</span><span class="sxs-lookup"><span data-stu-id="e9e74-152">**Customer subscription details**: Detailed view of the customers, subscriptions and offers</span></span> 


### <a name="license-insights-report"></a><span data-ttu-id="e9e74-153">ライセンス インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="e9e74-153">License Insights report:</span></span>

- <span data-ttu-id="e9e74-154">**ライセンスの合計**:ライセンス ベースのライセンスのすべてのサブスクリプションにわたって集計の合計数</span><span class="sxs-lookup"><span data-stu-id="e9e74-154">**Total licenses**: Total number of licenses aggregated across all license based subscriptions</span></span>

- <span data-ttu-id="e9e74-155">**新しい (過去 30 日)**:過去 30 日以内のライセンスの追加</span><span class="sxs-lookup"><span data-stu-id="e9e74-155">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="e9e74-156">**(過去 30 日間) のチャーン**:過去 30 日間でのライセンスの削減</span><span class="sxs-lookup"><span data-stu-id="e9e74-156">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="e9e74-157">**新しい (過去 24 時間)**:過去 24 時間以内にライセンスの追加</span><span class="sxs-lookup"><span data-stu-id="e9e74-157">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="e9e74-158">**過去 90 日間ライセンス**:前月のライセンスの追加や過去 90 日間の期間の月単位で集計の削減か月ごとの傾向</span><span class="sxs-lookup"><span data-stu-id="e9e74-158">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="e9e74-159">**製品別のアクティブなライセンス数**:アクティブなライセンスの数によって並べ替えられて販売されている製品</span><span class="sxs-lookup"><span data-stu-id="e9e74-159">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="e9e74-160">**お客様によってアクティブなライセンス数**:アクティブなライセンス数の順で顧客が並べ替えられます</span><span class="sxs-lookup"><span data-stu-id="e9e74-160">**Active license count by customer**: Customers sorted by sorted by active license count</span></span>

- <span data-ttu-id="e9e74-161">**過去 90 日間ライセンスのイベントの詳細を顧客**:サブスクリプション イベントのイベントなどの日付、イベント名、数量と数量の変更および顧客のサブスクリプション ビューの詳細。</span><span class="sxs-lookup"><span data-stu-id="e9e74-161">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions and subscription events including event date, event name, quantity and change in quantity.</span></span>


### <a name="licenses-usage-report"></a><span data-ttu-id="e9e74-162">ライセンス使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="e9e74-162">Licenses Usage report:</span></span>

- <span data-ttu-id="e9e74-163">**割り当てられている製品ライセンス**:ライセンス割り当ての数によって並べ替えられて販売されている製品</span><span class="sxs-lookup"><span data-stu-id="e9e74-163">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="e9e74-164">**製品で使用中のライセンス**:ライセンスの使用率カウントで並べ替えられた販売されている製品</span><span class="sxs-lookup"><span data-stu-id="e9e74-164">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="e9e74-165">**Customer distribution of licenses assigned** (割り当て済みライセンスの顧客分布): 全顧客を 20% 刻みのライセンス割り当て率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="e9e74-165">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="e9e74-166">**Customer distribution of licenses in use** (使用中ライセンスの顧客分布): すべての顧客を 20% 刻みの使用中ライセンス率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="e9e74-166">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="e9e74-167">**顧客が割り当てられているライセンス**:ライセンスの詳細ビューの販売し、顧客と製品ライセンスを割り当てる</span><span class="sxs-lookup"><span data-stu-id="e9e74-167">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="e9e74-168">**お客様が使用中のライセンス**:ライセンスの販売と顧客と製品で使用中のライセンスの詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="e9e74-168">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>


### <a name="azure-insights-report"></a><span data-ttu-id="e9e74-169">Azure インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="e9e74-169">Azure Insights report:</span></span>

- <span data-ttu-id="e9e74-170">**過去 12 か月間使用量ベースの顧客**:新しい使用状況の傾向を 1 か月の前月の顧客をベースし、過去 12 か月間の期間の月単位で集計使用法に基づく顧客を頻繁</span><span class="sxs-lookup"><span data-stu-id="e9e74-170">**Usage based customers over last 12 months**: Month over month trend of new usage based customers and churned usage based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e9e74-171">**過去 12 か月間のサブスクリプションが使用法に基づく**:新しい使用状況の傾向を 1 か月の前月のサブスクリプションをベースし、過去 12 か月間の期間の月単位で集計使用法に基づくサブスクリプションを頻繁</span><span class="sxs-lookup"><span data-stu-id="e9e74-171">**Usage based subscriptions over last 12 months**: Month over month trend of new usage based subscriptions and churned usage based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="e9e74-172">**過去 60 日間の顧客による使用量のコストの見積もり**:使用法に基づくお客様の推定税引き前の請求金額で並べ替えられますが、過去 60 日間の期間にわたって集計されます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-172">**Estimated cost of usage by customer over last 60 days**: Usage based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="e9e74-173">これにより、収益性の高い使用量ベースの主要顧客が明確になります。</span><span class="sxs-lookup"><span data-stu-id="e9e74-173">This will indicate top usage based customers bringing most revenue</span></span>

- <span data-ttu-id="e9e74-174">**カテゴリ別過去 60 日間使用量のコストの見積もり**:使用状況測定のカテゴリに分類ベースのサブスクリプションを過去 60 日間の期間にわたって集計された推定税引き前の請求金額で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-174">**Estimated cost of usage by category over last 60 days**: Meter categories of usage based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="e9e74-175">**過去 60 日間のサブスクリプションによって使用量のコストの見積もり**:推定税引き前の請求金額での使用法に基づくサブスクリプションは、過去 60 日間の期間にわたって集計されます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-175">**Estimated cost of usage by subscription over last 60 days**: Usage based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="e9e74-176">**支出予算を推定使用量のコストを顧客**:顧客の支出予算超過しきい値 (100%)、現在の使用量の割合で並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="e9e74-176">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>


### <a name="azure-resource-usage-report"></a><span data-ttu-id="e9e74-177">Azure リソース使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="e9e74-177">Azure Resource Usage report:</span></span>

- <span data-ttu-id="e9e74-178">**選択した期間の日別の Azure リソースの使用量**:過去 60 日間内で選択した期間中のサブスクリプションを従量制課金の各リソースごとの使用状況での毎日の消費量単位に基づいています。</span><span class="sxs-lookup"><span data-stu-id="e9e74-178">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="e9e74-179">**選択した期間の Azure リソースの使用量のコストの見積もり**:過去 60 日間内で選択した期間の各使用法に基づくサブスクリプションで従量制のリソースごとに最新の価格カードに基づく推定コスト。</span><span class="sxs-lookup"><span data-stu-id="e9e74-179">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span> 

## <a name="see-also"></a><span data-ttu-id="e9e74-180">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9e74-180">See also</span></span>

[<span data-ttu-id="e9e74-181">パートナー センターの Analytics の Power BI アプリの概要</span><span class="sxs-lookup"><span data-stu-id="e9e74-181">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)


[<span data-ttu-id="e9e74-182">インストールし、Microsoft Power BI 用のパートナー センターの分析アプリのプレビュー</span><span class="sxs-lookup"><span data-stu-id="e9e74-182">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
