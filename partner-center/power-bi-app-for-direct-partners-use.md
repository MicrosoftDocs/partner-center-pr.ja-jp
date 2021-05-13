---
title: パートナー センター Analytics を使用Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: (CSP の直接パートナー向け) Power BI 用パートナー センター分析アプリを使用してビジネス データを表示する方法について説明します。
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855031"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="08f23-103">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="08f23-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="08f23-104">**適切なロール**: グローバル管理者|ユーザー管理管理者|Sales Agent |管理エージェント</span><span class="sxs-lookup"><span data-stu-id="08f23-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="08f23-105">ビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="08f23-105">View your business data</span></span>

<span data-ttu-id="08f23-106">Power BI 用パートナー センター分析アプリでは、ビジネス データの視覚表現を利用できます。以下に例を示します。</span><span class="sxs-lookup"><span data-stu-id="08f23-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="08f23-107">顧客数、サブスクリプション数、ライセンス数の増加</span><span class="sxs-lookup"><span data-stu-id="08f23-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="08f23-108">Office 365、Microsoft Dynamics、Microsoft Azure の製品の使用量</span><span class="sxs-lookup"><span data-stu-id="08f23-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="08f23-109">過去 60 日間の各 Azure サブスクリプションにおける従量制課金リソースごとの 1 日当たりの消費単位</span><span class="sxs-lookup"><span data-stu-id="08f23-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="08f23-110">(最新の価格カードに基づく) 推定コスト</span><span class="sxs-lookup"><span data-stu-id="08f23-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="08f23-111">データセットをエクスポートし、顧客ごとにを含むカスタム レポートを作成する機能。</span><span class="sxs-lookup"><span data-stu-id="08f23-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="08f23-112">パートナー センターの分析のアプリのプレビュー リリースについて</span><span class="sxs-lookup"><span data-stu-id="08f23-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="08f23-113">このアプリは、クラウド ソリューション プロバイダー プログラムの直接パートナーのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="08f23-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="08f23-114">CSP の他のパートナー (間接リセラーなど) はログインできません。</span><span class="sxs-lookup"><span data-stu-id="08f23-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="08f23-115">見積もりコストはすべて税抜きの請求データであり、法的拘束力を持ちません。</span><span class="sxs-lookup"><span data-stu-id="08f23-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="08f23-116">推定コストは、データ インサイトの目的のみで使用することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="08f23-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="08f23-117">顧客情報は、サブスクリプションに基づきます。</span><span class="sxs-lookup"><span data-stu-id="08f23-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="08f23-118">最近アカウントを作成したが、まだサブスクリプションを持っていない顧客は、カウントに含まれません。</span><span class="sxs-lookup"><span data-stu-id="08f23-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="08f23-119">推定コストは、最新の価格カード (CSP 価格に基づく) を使って算出されます。</span><span class="sxs-lookup"><span data-stu-id="08f23-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="08f23-120">日数は暦日です。</span><span class="sxs-lookup"><span data-stu-id="08f23-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="08f23-121">ビジネス インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="08f23-121">Business Insights report</span></span>

- <span data-ttu-id="08f23-122">**Customer tenants** (顧客のテナント): サブスクリプションを購入した顧客の個別の Azure AD テナント数</span><span class="sxs-lookup"><span data-stu-id="08f23-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="08f23-123">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="08f23-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="08f23-124">**チャーン (過去 30 日間)**: "アクティブ"、"猶予中"、または "無効" サブスクリプションがないお客様</span><span class="sxs-lookup"><span data-stu-id="08f23-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="08f23-125">**New (last 24 hours)**: (新規 (過去 24 時間)) 過去 24 時間以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="08f23-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="08f23-126">**Estimated monthly cost over last 12 months** (過去 12 か月間の月間推定コスト): 過去 12 か月間にわたって月単位で集計された税抜き推定コスト (単位: ドル) の月別推移</span><span class="sxs-lookup"><span data-stu-id="08f23-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08f23-127">**Estimated cost by product over last 12 months** (過去 12 か月間の製品別推定コスト): 販売された製品を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="08f23-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="08f23-128">この状態は、上位の製品がほとんどの収益を生み出す状態を示します。</span><span class="sxs-lookup"><span data-stu-id="08f23-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="08f23-129">**Customers over last 12 months** (過去 12 か月間の顧客): 過去 12 か月間にわたって月単位で集計された新規顧客とチャーン顧客の月別推移</span><span class="sxs-lookup"><span data-stu-id="08f23-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08f23-130">**Estimated cost by customer over last 12 months** (過去 12 か月間の顧客別推定コスト): 顧客を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="08f23-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="08f23-131">この状態は、上位の顧客がほとんどの収益を得たかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f23-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="08f23-132">**Customer count by product** (製品別顧客数): 製品をそれに関連付けられている顧客数の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="08f23-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="08f23-133">この状態は、ほとんどの顧客に販売された上位の製品を示します。</span><span class="sxs-lookup"><span data-stu-id="08f23-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="08f23-134">サブスクリプション インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="08f23-134">Subscription Insights report</span></span>

- <span data-ttu-id="08f23-135">**サブスクリプションの状態**:</span><span class="sxs-lookup"><span data-stu-id="08f23-135">**Subscription status**:</span></span>

- <span data-ttu-id="08f23-136">アクティブ: "アクティブ" または "猶予期間" 状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="08f23-137">中断: "無効" 状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="08f23-138">プロビジョニングの取り下し: "プロビジョニングの取り下がり" または "期限切れ" 状態に属するサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="08f23-139">**Expiry status** (有効期限の状態): </span><span class="sxs-lookup"><span data-stu-id="08f23-139">**Expiry status**:</span></span>

  - <span data-ttu-id="08f23-140">Expired (期限切れ): 既に有効期限が切れてた状態のサブスクリプション (サブスクリプションの終了日が過去の日付)</span><span class="sxs-lookup"><span data-stu-id="08f23-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="08f23-141">Expiring after 30 days (30 日後に期限切れ): 今後 30 日後に期限切れとなるサブスクリプション (サブスクリプションの終了日が 30 日後)</span><span class="sxs-lookup"><span data-stu-id="08f23-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="08f23-142">Expiring in 30 days (30 日以内に期限切れ): 今後 30 日以内に期限切れとなるサブスクリプション (サブスクリプションの終了日が今日から 30 日後までの間)</span><span class="sxs-lookup"><span data-stu-id="08f23-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="08f23-143">**サブスクリプションの合計**: "アクティブ"、"猶予中"、または "無効" 状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="08f23-144">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="08f23-145">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="08f23-146">**30 日以内に期限切れ**: 今後 30 日以内に期限切れとなるサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="08f23-147">**Churn (last 30 days)** (チャーン (過去 30 日)) : 過去 30 日以内にプロビジョニング解除または中断 (無効) となったサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="08f23-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="08f23-148">**サブスクリプションの種類別の配布**: ライセンス ベースおよび使用量ベースのサブスクリプションの種類別のサブスクリプションの合計の % 分布</span><span class="sxs-lookup"><span data-stu-id="08f23-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="08f23-149">**Active subscription count by product** (製品別アクティブなサブスクリプション数): 製品をアクティブなサブスクリプション数の順に表示</span><span class="sxs-lookup"><span data-stu-id="08f23-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="08f23-150">**Subscriptions over last 12 months** (過去 12 か月間のサブスクリプション): 過去 12 か月間にわたって月単位で集計された新規サブスクリプションとチャーン サブスクリプションの月別推移</span><span class="sxs-lookup"><span data-stu-id="08f23-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08f23-151">**顧客サブスクリプションの** 詳細: 顧客、サブスクリプション、オファーの詳細なビュー</span><span class="sxs-lookup"><span data-stu-id="08f23-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="08f23-152">ライセンス インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="08f23-152">License Insights report:</span></span>

- <span data-ttu-id="08f23-153">**合計ライセンス** 数: すべてのライセンス ベースのサブスクリプションで集計されたライセンスの総数</span><span class="sxs-lookup"><span data-stu-id="08f23-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="08f23-154">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="08f23-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="08f23-155">**Churn (last 30 days)**: (チャーン (過去 30 日)): 過去 30 日以内のライセンス減少数</span><span class="sxs-lookup"><span data-stu-id="08f23-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="08f23-156">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="08f23-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="08f23-157">**Licenses over last 90 days** (過去 90 日間のライセンス): 過去 90 日間にわたって月単位で集計されたライセンス増減の月別推移</span><span class="sxs-lookup"><span data-stu-id="08f23-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="08f23-158">**Active license count by product** (製品別アクティブなライセンス数): 製品をアクティブなライセンス数の順に表示</span><span class="sxs-lookup"><span data-stu-id="08f23-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="08f23-159">**顧客別のアクティブなライセンス数**: アクティブなライセンス数で並べ替えた顧客</span><span class="sxs-lookup"><span data-stu-id="08f23-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="08f23-160">**過去 90** 日間の顧客ライセンス イベントの詳細: イベントの日付、イベント名、数量、数量の変更など、顧客、サブスクリプション、サブスクリプション イベントの詳細なビュー。</span><span class="sxs-lookup"><span data-stu-id="08f23-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="08f23-161">ライセンス使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="08f23-161">Licenses Usage report:</span></span>

- <span data-ttu-id="08f23-162">**Licenses assigned by product**(製品別割り当て済みライセンス): 販売された製品をライセンス割り当て数の順に表示</span><span class="sxs-lookup"><span data-stu-id="08f23-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="08f23-163">**Licenses in use by product**(製品別使用中ライセンス): 販売された製品をライセンス使用数の順に表示</span><span class="sxs-lookup"><span data-stu-id="08f23-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="08f23-164">**Customer distribution of licenses assigned** (割り当て済みライセンスの顧客分布): 全顧客を 20% 刻みのライセンス割り当て率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="08f23-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="08f23-165">**Customer distribution of licenses in use** (使用中ライセンスの顧客分布): すべての顧客を 20% 刻みの使用中ライセンス率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="08f23-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="08f23-166">**Licenses assigned by customer** (顧客別割り当て済みライセンス): 販売されたライセンスと割り当てられたライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="08f23-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="08f23-167">**Licenses in use by customer** (顧客別使用中ライセンス): 販売されたライセンスと使用中ライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="08f23-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="08f23-168">Azure インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="08f23-168">Azure Insights report:</span></span>

- <span data-ttu-id="08f23-169">**過去 12** か月間の使用量ベースの顧客: 過去 12 か月間に毎月集計された新しい使用量ベースの顧客とチャーンされた使用量ベースの顧客の月別傾向</span><span class="sxs-lookup"><span data-stu-id="08f23-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08f23-170">**過去 12** か月間の使用量ベースのサブスクリプション: 過去 12 か月間に毎月集計された新しい使用量ベースのサブスクリプションとチャーンされた使用量ベースのサブスクリプションの月別の傾向</span><span class="sxs-lookup"><span data-stu-id="08f23-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="08f23-171">**過去 60** 日間の顧客別の推定使用コスト: 過去 60 日間に集計された税引き前請求書の推定金額で並べ替えた使用量ベースの顧客。</span><span class="sxs-lookup"><span data-stu-id="08f23-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="08f23-172">この状態は、使用量ベースの上位のお客様がほとんどの収益を生み出したかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="08f23-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="08f23-173">**過去 60** 日間のカテゴリ別の使用量の推定コスト: 過去 60 日間に集計された税引き前請求書の推定金額で並べ替えた使用量ベースのサブスクリプションの測定カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="08f23-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="08f23-174">**過去 60** 日間のサブスクリプション別の使用量の推定コスト: 過去 60 日間に集計された税引き前請求書の推定金額別の使用量ベースのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="08f23-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="08f23-175">**Customer estimated usage cost by spending budget** (予算支出別顧客推定使用コスト): 顧客を、現在の使用量予算支出のしきい値 (100%) を超えた部分のパーセント率の順に表示。</span><span class="sxs-lookup"><span data-stu-id="08f23-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="08f23-176">Azure リソース使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="08f23-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="08f23-177">**選択した期間** の Azure リソースの日別の使用状況: 過去 60 日以内に選択した期間の、使用状況ベースのサブスクリプションごとに測定された各リソースの 1 日の消費量単位。</span><span class="sxs-lookup"><span data-stu-id="08f23-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="08f23-178">**[選択した期間** の Azure リソースの推定使用コスト]: 過去 60 日以内に選択した期間について、各使用量ベースのサブスクリプションの使用状況に基づく各リソースの最新のレート カードに基づく推定コスト。</span><span class="sxs-lookup"><span data-stu-id="08f23-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="08f23-179">次の手順</span><span class="sxs-lookup"><span data-stu-id="08f23-179">Next steps</span></span>

- [<span data-ttu-id="08f23-180">Power BI 用パートナー センター分析アプリの概要</span><span class="sxs-lookup"><span data-stu-id="08f23-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="08f23-181">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="08f23-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
