---
title: Power BI にパートナーセンター分析を使用する
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Power BI 用のパートナーセンター分析アプリ (CSP のダイレクトパートナー向け) を使用してビジネスデータを表示する方法について説明します。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f5bdb166562593b970f40c23921dc80b2a1cb8ad
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633864"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="0d3cc-103">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="0d3cc-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="0d3cc-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="0d3cc-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0d3cc-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="0d3cc-105">Global admin</span></span>
- <span data-ttu-id="0d3cc-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="0d3cc-106">User management admin</span></span>
- <span data-ttu-id="0d3cc-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="0d3cc-107">Sales agent</span></span>
- <span data-ttu-id="0d3cc-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="0d3cc-108">Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="0d3cc-109">ビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="0d3cc-109">View your business data</span></span>

<span data-ttu-id="0d3cc-110">Power BI 用パートナー センター分析アプリでは、ビジネス データの視覚表現を利用できます。以下に例を示します。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-110">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="0d3cc-111">顧客数、サブスクリプション数、ライセンス数の増加</span><span class="sxs-lookup"><span data-stu-id="0d3cc-111">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="0d3cc-112">Office 365、Microsoft Dynamics、Microsoft Azure の製品の使用量</span><span class="sxs-lookup"><span data-stu-id="0d3cc-112">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="0d3cc-113">過去 60 日間の各 Azure サブスクリプションにおける従量制課金リソースごとの 1 日当たりの消費単位</span><span class="sxs-lookup"><span data-stu-id="0d3cc-113">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="0d3cc-114">(最新の価格カードに基づく) 推定コスト</span><span class="sxs-lookup"><span data-stu-id="0d3cc-114">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="0d3cc-115">顧客ごとなど、データセットをエクスポートしてカスタムレポートを作成する機能。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-115">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="0d3cc-116">パートナー センターの分析のアプリのプレビュー リリースについて</span><span class="sxs-lookup"><span data-stu-id="0d3cc-116">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="0d3cc-117">このアプリは、クラウド ソリューション プロバイダー プログラムの直接パートナーのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-117">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="0d3cc-118">CSP の他のパートナー (間接リセラーなど) はログインできません。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-118">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="0d3cc-119">見積もりコストはすべて税抜きの請求データであり、法的拘束力を持ちません。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-119">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="0d3cc-120">推定コストは、データ インサイトの目的のみで使用することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-120">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="0d3cc-121">顧客情報は、サブスクリプションに基づきます。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-121">Customer information is based on subscriptions.</span></span> <span data-ttu-id="0d3cc-122">最近アカウントを作成したが、まだサブスクリプションを持っていないお客様は、カウントに含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-122">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="0d3cc-123">推定コストは、最新の価格カード (CSP 価格に基づく) を使って算出されます。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-123">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="0d3cc-124">日数は暦日です。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-124">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="0d3cc-125">ビジネス インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="0d3cc-125">Business Insights report</span></span>

- <span data-ttu-id="0d3cc-126">**Customer tenants** (顧客のテナント): サブスクリプションを購入した顧客の個別の Azure AD テナント数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-126">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="0d3cc-127">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="0d3cc-127">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="0d3cc-128">**チャーン (過去30日間)**: "アクティブ"、"猶予"、"無効" の各サブスクリプションを持たないお客様</span><span class="sxs-lookup"><span data-stu-id="0d3cc-128">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="0d3cc-129">**New (last 24 hours)**: (新規 (過去 24 時間)) 過去 24 時間以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="0d3cc-129">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="0d3cc-130">**Estimated monthly cost over last 12 months** (過去 12 か月間の月間推定コスト): 過去 12 か月間にわたって月単位で集計された税抜き推定コスト (単位: ドル) の月別推移</span><span class="sxs-lookup"><span data-stu-id="0d3cc-130">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0d3cc-131">**Estimated cost by product over last 12 months** (過去 12 か月間の製品別推定コスト): 販売された製品を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-131">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="0d3cc-132">この状態は、売上が最も多い上位製品を示します。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-132">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="0d3cc-133">**Customers over last 12 months** (過去 12 か月間の顧客): 過去 12 か月間にわたって月単位で集計された新規顧客とチャーン顧客の月別推移</span><span class="sxs-lookup"><span data-stu-id="0d3cc-133">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0d3cc-134">**Estimated cost by customer over last 12 months** (過去 12 か月間の顧客別推定コスト): 顧客を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-134">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="0d3cc-135">この状態は、上位の顧客が最も収益を上げていることを示します。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-135">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="0d3cc-136">**Customer count by product** (製品別顧客数): 製品をそれに関連付けられている顧客数の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-136">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="0d3cc-137">この状態は、ほとんどの顧客に販売されている上位の製品を示します。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-137">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="0d3cc-138">サブスクリプション インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="0d3cc-138">Subscription Insights report</span></span>

- <span data-ttu-id="0d3cc-139">**サブスクリプションの状態**:</span><span class="sxs-lookup"><span data-stu-id="0d3cc-139">**Subscription status**:</span></span>

- <span data-ttu-id="0d3cc-140">アクティブ: "アクティブ" または "猶予中" のいずれかの状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-140">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="0d3cc-141">中断: "無効" 状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-141">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="0d3cc-142">プロビジョニング解除: "プロビジョニング解除" または "期限切れ" の状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-142">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="0d3cc-143">**Expiry status** (有効期限の状態): </span><span class="sxs-lookup"><span data-stu-id="0d3cc-143">**Expiry status**:</span></span>

  - <span data-ttu-id="0d3cc-144">Expired (期限切れ): 既に有効期限が切れてた状態のサブスクリプション (サブスクリプションの終了日が過去の日付)</span><span class="sxs-lookup"><span data-stu-id="0d3cc-144">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="0d3cc-145">Expiring after 30 days (30 日後に期限切れ): 今後 30 日後に期限切れとなるサブスクリプション (サブスクリプションの終了日が 30 日後)</span><span class="sxs-lookup"><span data-stu-id="0d3cc-145">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="0d3cc-146">Expiring in 30 days (30 日以内に期限切れ): 今後 30 日以内に期限切れとなるサブスクリプション (サブスクリプションの終了日が今日から 30 日後までの間)</span><span class="sxs-lookup"><span data-stu-id="0d3cc-146">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="0d3cc-147">**サブスクリプションの合計**: "アクティブ"、"猶予"、"無効" の状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-147">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="0d3cc-148">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-148">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="0d3cc-149">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-149">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="0d3cc-150">**30 日以内に期限切れ**: 今後 30 日以内に期限切れとなるサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-150">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="0d3cc-151">**Churn (last 30 days)** (チャーン (過去 30 日)) : 過去 30 日以内にプロビジョニング解除または中断 (無効) となったサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="0d3cc-151">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="0d3cc-152">**サブスクリプションの種類別の分布**: ライセンスベースのサブスクリプションと使用状況に基づくサブスクリプションの種類別のサブスクリプションの合計数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-152">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="0d3cc-153">**Active subscription count by product** (製品別アクティブなサブスクリプション数): 製品をアクティブなサブスクリプション数の順に表示</span><span class="sxs-lookup"><span data-stu-id="0d3cc-153">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="0d3cc-154">**Subscriptions over last 12 months** (過去 12 か月間のサブスクリプション): 過去 12 か月間にわたって月単位で集計された新規サブスクリプションとチャーン サブスクリプションの月別推移</span><span class="sxs-lookup"><span data-stu-id="0d3cc-154">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0d3cc-155">**顧客サブスクリプションの詳細**: 顧客、サブスクリプション、およびプランの詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="0d3cc-155">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="0d3cc-156">ライセンス インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="0d3cc-156">License Insights report:</span></span>

- <span data-ttu-id="0d3cc-157">**合計ライセンス** 数: ライセンスベースのサブスクリプション全体で集計されたライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-157">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="0d3cc-158">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-158">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="0d3cc-159">**Churn (last 30 days)**: (チャーン (過去 30 日)): 過去 30 日以内のライセンス減少数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-159">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="0d3cc-160">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="0d3cc-160">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="0d3cc-161">**Licenses over last 90 days** (過去 90 日間のライセンス): 過去 90 日間にわたって月単位で集計されたライセンス増減の月別推移</span><span class="sxs-lookup"><span data-stu-id="0d3cc-161">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="0d3cc-162">**Active license count by product** (製品別アクティブなライセンス数): 製品をアクティブなライセンス数の順に表示</span><span class="sxs-lookup"><span data-stu-id="0d3cc-162">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="0d3cc-163">**顧客別アクティブライセンス数**: アクティブなライセンス数で並べ替えられた顧客</span><span class="sxs-lookup"><span data-stu-id="0d3cc-163">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="0d3cc-164">**過去90日間のカスタマーライセンスイベントの詳細**: イベント日、イベント名、数量、数量の変化など、顧客、サブスクリプション、サブスクリプションイベントの詳細なビュー。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-164">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="0d3cc-165">ライセンス使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="0d3cc-165">Licenses Usage report:</span></span>

- <span data-ttu-id="0d3cc-166">**Licenses assigned by product**(製品別割り当て済みライセンス): 販売された製品をライセンス割り当て数の順に表示</span><span class="sxs-lookup"><span data-stu-id="0d3cc-166">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="0d3cc-167">**Licenses in use by product**(製品別使用中ライセンス): 販売された製品をライセンス使用数の順に表示</span><span class="sxs-lookup"><span data-stu-id="0d3cc-167">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="0d3cc-168">**Customer distribution of licenses assigned** (割り当て済みライセンスの顧客分布): 全顧客を 20% 刻みのライセンス割り当て率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="0d3cc-168">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="0d3cc-169">**Customer distribution of licenses in use** (使用中ライセンスの顧客分布): すべての顧客を 20% 刻みの使用中ライセンス率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="0d3cc-169">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="0d3cc-170">**Licenses assigned by customer** (顧客別割り当て済みライセンス): 販売されたライセンスと割り当てられたライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="0d3cc-170">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="0d3cc-171">**Licenses in use by customer** (顧客別使用中ライセンス): 販売されたライセンスと使用中ライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="0d3cc-171">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="0d3cc-172">Azure インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="0d3cc-172">Azure Insights report:</span></span>

- <span data-ttu-id="0d3cc-173">**過去12か月間の使用量ベースのお客様**: 過去12か月間、新しい使用量ベースのお客様と頻繁の使用量ベースのお客様の傾向を月単位で集計</span><span class="sxs-lookup"><span data-stu-id="0d3cc-173">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0d3cc-174">**過去12か月間の使用量ベースのサブスクリプション**: 過去1か月の新しい使用状況ベースのサブスクリプションと頻繁の使用量ベースのサブスクリプションの傾向 (過去12か月の期間にわたって毎月集計)</span><span class="sxs-lookup"><span data-stu-id="0d3cc-174">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="0d3cc-175">**過去60日間のお客様による使用量の推定コスト**: 過去60日間に集計された課税前請求書の金額で並べ替えられた使用量ベースの顧客。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-175">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="0d3cc-176">この状態は、最も多くの収益をもたらす、使用量ベースの上位の顧客を示します。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-176">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="0d3cc-177">**過去60日間のカテゴリ別の使用量の推定コスト**: 過去60日の期間に集計された課税前請求書の金額で並べ替えられた、使用量ベースのサブスクリプションのメーターカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-177">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="0d3cc-178">**過去60日間のサブスクリプションによる使用量の推定コスト**: 過去60日の期間に集計された課税前請求書の金額に基づく使用量ベースのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-178">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="0d3cc-179">**Customer estimated usage cost by spending budget** (予算支出別顧客推定使用コスト): 顧客を、現在の使用量予算支出のしきい値 (100%) を超えた部分のパーセント率の順に表示。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-179">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="0d3cc-180">Azure リソース使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="0d3cc-180">Azure Resource Usage report:</span></span>

- <span data-ttu-id="0d3cc-181">**選択した期間の日別の Azure リソースの使用**: 過去60日以内に選択された期間の各使用量ベースのサブスクリプションでの、各従量制リソースの使用量単位。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-181">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="0d3cc-182">**選択した期間の Azure リソースの推定使用コスト**: 過去60日以内に選択された期間の各使用量ベースのサブスクリプションで、各従量制課金リソースの最新のレートカードに基づく推定コスト。</span><span class="sxs-lookup"><span data-stu-id="0d3cc-182">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0d3cc-183">次のステップ</span><span class="sxs-lookup"><span data-stu-id="0d3cc-183">Next steps</span></span>

- [<span data-ttu-id="0d3cc-184">Power BI 用パートナー センター分析アプリの概要</span><span class="sxs-lookup"><span data-stu-id="0d3cc-184">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="0d3cc-185">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="0d3cc-185">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
