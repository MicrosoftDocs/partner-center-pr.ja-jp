---
title: "Power BI 用パートナー センター分析アプリ | パートナー センター"
description: "Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け) の使用方法を説明します。"
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: labrenne
ms.openlocfilehash: 3eadf41093f6d3d2ad42fecae856384800676b1a
ms.sourcegitcommit: 9183f596e81595496ae49375c116ea0f772babac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/23/2017
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="177d8-103">Microsoft Power BI 用パートナー センター分析アプリでビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="177d8-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>

**<span data-ttu-id="177d8-104">適用対象</span><span class="sxs-lookup"><span data-stu-id="177d8-104">Applies to</span></span>**

-   <span data-ttu-id="177d8-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="177d8-105">Partner Center</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="177d8-106">ビジネス データを表示する</span><span class="sxs-lookup"><span data-stu-id="177d8-106">View your business data</span></span>

<span data-ttu-id="177d8-107">Power BI 用パートナー センター分析アプリでは、ビジネス データの視覚表現を利用できます。以下に例を示します。</span><span class="sxs-lookup"><span data-stu-id="177d8-107">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="177d8-108">顧客数、サブスクリプション数、ライセンス数の増加</span><span class="sxs-lookup"><span data-stu-id="177d8-108">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="177d8-109">Office 365、Microsoft Dynamics、Microsoft Azure の製品の使用量</span><span class="sxs-lookup"><span data-stu-id="177d8-109">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="177d8-110">過去 60 日間の各 Azure サブスクリプションにおける従量制課金リソースごとの 1 日当たりの消費単位</span><span class="sxs-lookup"><span data-stu-id="177d8-110">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="177d8-111">(最新の価格カードに基づく) 推定コスト</span><span class="sxs-lookup"><span data-stu-id="177d8-111">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="177d8-112">データセットのエクスポートおよびカスタム レポート作成 (顧客別など) の機能</span><span class="sxs-lookup"><span data-stu-id="177d8-112">Ability to export datasets and create custom reports, including per customer</span></span> 

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="177d8-113">パートナー センターの分析のアプリのプレビュー リリースについて</span><span class="sxs-lookup"><span data-stu-id="177d8-113">About the Partner Center Analytics app preview release</span></span>

 - <span data-ttu-id="177d8-114">このアプリは、クラウド ソリューション プロバイダー プログラムの直接パートナーのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="177d8-114">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="177d8-115">CSP の他のパートナー (間接リセラーなど) はログインできません。</span><span class="sxs-lookup"><span data-stu-id="177d8-115">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="177d8-116">見積もりコストはすべて税抜きの請求データであり、法的拘束力を持ちません。</span><span class="sxs-lookup"><span data-stu-id="177d8-116">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="177d8-117">推定コストは、データ インサイトの目的のみで使用することを想定しています。</span><span class="sxs-lookup"><span data-stu-id="177d8-117">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="177d8-118">顧客情報は、サブスクリプションに基づきます。</span><span class="sxs-lookup"><span data-stu-id="177d8-118">Customer information is based on subscriptions.</span></span> <span data-ttu-id="177d8-119">最近、アカウントを作成し、まだサブスクリプションがない顧客はカウントされません。</span><span class="sxs-lookup"><span data-stu-id="177d8-119">Any customers that you've recently created accounts for, but who do not yet have subscriptions, are not included in counts.</span></span> 

- <span data-ttu-id="177d8-120">推定コストは、最新の価格カード (CSP 価格に基づく) を使って算出されます。</span><span class="sxs-lookup"><span data-stu-id="177d8-120">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span> 

- <span data-ttu-id="177d8-121">日数は暦日です。</span><span class="sxs-lookup"><span data-stu-id="177d8-121">Days are calendar days.</span></span> 


### <a name="business-insights-report"></a><span data-ttu-id="177d8-122">ビジネス インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="177d8-122">Business Insights report</span></span>

-  <span data-ttu-id="177d8-123">**Customer tenants** (顧客のテナント): サブスクリプションを購入した顧客の個別の Azure AD テナント数</span><span class="sxs-lookup"><span data-stu-id="177d8-123">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

-  <span data-ttu-id="177d8-124">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="177d8-124">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

-  <span data-ttu-id="177d8-125">**Churn (last 30 days)** (チャーン (過去 30 日)): "active" (アクティブ)、"in grace" (猶予期間中)、"disabled" (無効) のいずれのサブスクリプションも持たない顧客</span><span class="sxs-lookup"><span data-stu-id="177d8-125">**Churn (last 30 days)**: Customers without any “active”, “in grace” or “disabled” subscriptions</span></span>

- <span data-ttu-id="177d8-126">**New (last 24 hours)**: (新規 (過去 24 時間)) 過去 24 時間以内に 1 つ以上のサブスクリプションを購入した新規顧客</span><span class="sxs-lookup"><span data-stu-id="177d8-126">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="177d8-127">**Estimated monthly cost over last 12 months** (過去 12 か月間の月間推定コスト): 過去 12 か月間にわたって月単位で集計された税抜き推定コスト (単位: ドル) の月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-127">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="177d8-128">**Estimated cost by product over last 12 months** (過去 12 か月間の製品別推定コスト): 販売された製品を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-128">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="177d8-129">これにより、収益性の高い主力製品が明確になります。</span><span class="sxs-lookup"><span data-stu-id="177d8-129">This will indicate top products bringing most revenue.</span></span>

- <span data-ttu-id="177d8-130">**Customers over last 12 months** (過去 12 か月間の顧客): 過去 12 か月間にわたって月単位で集計された新規顧客とチャーン顧客の月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-130">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="177d8-131">**Estimated cost by customer over last 12 months** (過去 12 か月間の顧客別推定コスト): 顧客を過去 12 か月間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-131">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="177d8-132">これにより、収益性の高い主要顧客が明確になります。</span><span class="sxs-lookup"><span data-stu-id="177d8-132">This will indicate top customers bringing most revenue.</span></span>

- <span data-ttu-id="177d8-133">**Customer count by product** (製品別顧客数): 製品をそれに関連付けられている顧客数の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-133">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="177d8-134">これにより、多くの顧客が購入した主力製品が明らかになります。</span><span class="sxs-lookup"><span data-stu-id="177d8-134">This will indicate top products sold to most customers.</span></span> 


### <a name="subscription-insights-report"></a><span data-ttu-id="177d8-135">サブスクリプション インサイト レポート</span><span class="sxs-lookup"><span data-stu-id="177d8-135">Subscription Insights report</span></span> 

- <span data-ttu-id="177d8-136">**Subscription status** (サブスクリプションの状態): </span><span class="sxs-lookup"><span data-stu-id="177d8-136">**Subscription status**:</span></span>

    - <span data-ttu-id="177d8-137">Active (アクティブ): "Active" (アクティブ) 状態または "in grace" (猶予期間中) 状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-137">Active: Subscriptions belonging to either “active” or “in grace” state</span></span>

    - <span data-ttu-id="177d8-138">Suspended (中断): "disabled" (無効) 状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-138">Suspended: Subscriptions belonging to “disabled” state</span></span>

    - <span data-ttu-id="177d8-139">De-provisioned (プロビジョニング解除): "de-provisioned" (プロビジョニング解除) 状態または "expired" (期限切れ) 状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-139">De-provisioned: Subscriptions belonging to “de-provisioned” or “expired” status</span></span>

- <span data-ttu-id="177d8-140">**Expiry status** (有効期限の状態): </span><span class="sxs-lookup"><span data-stu-id="177d8-140">**Expiry status**:</span></span>

    - <span data-ttu-id="177d8-141">Expired (期限切れ): 既に有効期限が切れてた状態のサブスクリプション (サブスクリプションの終了日が過去の日付)</span><span class="sxs-lookup"><span data-stu-id="177d8-141">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

    - <span data-ttu-id="177d8-142">Expiring after 30 days (30 日後に期限切れ): 今後 30 日後に期限切れとなるサブスクリプション (サブスクリプションの終了日が 30 日後)</span><span class="sxs-lookup"><span data-stu-id="177d8-142">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

    - <span data-ttu-id="177d8-143">Expiring in 30 days (30 日以内に期限切れ): 今後 30 日以内に期限切れとなるサブスクリプション (サブスクリプションの終了日が今日から 30 日後までの間)</span><span class="sxs-lookup"><span data-stu-id="177d8-143">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

-  <span data-ttu-id="177d8-144">**Total subscriptions** (サブスクリプション合計): "active" (アクティブ)、"in grace" (猶予期間中)、"disabled" (無効) のいずれかの状態のサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-144">**Total subscriptions**: Subscriptions in “active,” “in grace” or “disabled” status</span></span>

- <span data-ttu-id="177d8-145">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-145">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="177d8-146">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内に顧客によって購入された新しいサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-146">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="177d8-147">**30 日以内に期限切れ**: 今後 30 日以内に期限切れとなるサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-147">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="177d8-148">**Churn (last 30 days)** (チャーン (過去 30 日)) : 過去 30 日以内にプロビジョニング解除または中断 (無効) となったサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="177d8-148">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="177d8-149">**Distribution by subscription types** (サブスクリプションの種類別分布率): 全サブスクリプションのライセンス ベースと利用量ベースのサブスクリプションの種類別分布率</span><span class="sxs-lookup"><span data-stu-id="177d8-149">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage based subscription type</span></span>

- <span data-ttu-id="177d8-150">**Active subscription count by product** (製品別アクティブなサブスクリプション数): 製品をアクティブなサブスクリプション数の順に表示</span><span class="sxs-lookup"><span data-stu-id="177d8-150">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="177d8-151">**Subscriptions over last 12 months** (過去 12 か月間のサブスクリプション): 過去 12 か月間にわたって月単位で集計された新規サブスクリプションとチャーン サブスクリプションの月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-151">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="177d8-152">**Customer subscription details** (顧客のサブスクリプションの詳細): 詳細、サブスクリプション、プランの詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="177d8-152">**Customer subscription details**: Detailed view of the customers, subscriptions and offers</span></span> 


### <a name="license-insights-report"></a><span data-ttu-id="177d8-153">ライセンス インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="177d8-153">License Insights report:</span></span>

- <span data-ttu-id="177d8-154">**Total licenses** (ライセンス合計): すべてのライセンス ベースのサブスクリプションを合わせたライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="177d8-154">**Total licenses**: Total number of licenses aggregated across all license based subscriptions</span></span>

- <span data-ttu-id="177d8-155">**New (last 30 days)** (新規 (過去 30 日)): 過去 30 日以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="177d8-155">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="177d8-156">**Churn (last 30 days)**: (チャーン (過去 30 日)): 過去 30 日以内のライセンス減少数</span><span class="sxs-lookup"><span data-stu-id="177d8-156">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="177d8-157">**New (last 24 hours)** (新規 (過去 24 時間)): 過去 24 時間以内のライセンス増加数</span><span class="sxs-lookup"><span data-stu-id="177d8-157">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="177d8-158">**Licenses over last 90 days** (過去 90 日間のライセンス): 過去 90 日間にわたって月単位で集計されたライセンス増減の月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-158">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="177d8-159">**Active license count by product** (製品別アクティブなライセンス数): 製品をアクティブなライセンス数の順に表示</span><span class="sxs-lookup"><span data-stu-id="177d8-159">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="177d8-160">**Active license count by customer** (顧客別アクティブなライセンス数): 顧客をアクティブなライセンス数の順に表示</span><span class="sxs-lookup"><span data-stu-id="177d8-160">**Active license count by customer**: Customers sorted by sorted by active license count</span></span>

- <span data-ttu-id="177d8-161">**Customer license event details over last 90 days** (過去 90 日間の顧客ライセンス イベントの詳細) : 顧客、サブスクリプション、サブスクリプション イベント (イベント発生日、イベント名、数量、数量の変化など) の詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="177d8-161">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions and subscription events including event date, event name, quantity and change in quantity.</span></span>


### <a name="licenses-usage-report"></a><span data-ttu-id="177d8-162">ライセンス使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="177d8-162">Licenses Usage report:</span></span>

- <span data-ttu-id="177d8-163">**Licenses assigned by product**(製品別割り当て済みライセンス): 販売された製品をライセンス割り当て数の順に表示</span><span class="sxs-lookup"><span data-stu-id="177d8-163">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="177d8-164">**Licenses in use by product**(製品別使用中ライセンス): 販売された製品をライセンス使用数の順に表示</span><span class="sxs-lookup"><span data-stu-id="177d8-164">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="177d8-165">**Customer distribution of licenses assigned** (割り当て済みライセンスの顧客分布): 全顧客を 20% 刻みのライセンス割り当て率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="177d8-165">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="177d8-166">**Customer distribution of licenses in use** (使用中ライセンスの顧客分布): すべての顧客を 20% 刻みの使用中ライセンス率の範囲ごとに分割した分布率</span><span class="sxs-lookup"><span data-stu-id="177d8-166">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="177d8-167">**Licenses assigned by customer** (顧客別割り当て済みライセンス): 販売されたライセンスと割り当てられたライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="177d8-167">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="177d8-168">**Licenses in use by customer** (顧客別使用中ライセンス): 販売されたライセンスと使用中ライセンスを顧客別および製品別に表示した詳細ビュー</span><span class="sxs-lookup"><span data-stu-id="177d8-168">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>


### <a name="azure-insights-report"></a><span data-ttu-id="177d8-169">Azure インサイト レポート:</span><span class="sxs-lookup"><span data-stu-id="177d8-169">Azure Insights report:</span></span>

- <span data-ttu-id="177d8-170">**Usage based customers over last 12 months** (過去 12 か月間の使用量ベースの顧客): 過去 12 か月間にわたって月単位で集計された使用量ベースの新規顧客と使用量ベースのチャーン顧客の月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-170">**Usage based customers over last 12 months**: Month over month trend of new usage based customers and churned usage based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="177d8-171">**Usage based subscriptions over last 12 months** (過去 12 か月間の使用量ベースのサブスクリプション): 過去 12 か月間にわたって月単位で集計された使用量ベースの新規サブスクリプションと使用量ベースのチャーン サブスクリプションの月別推移</span><span class="sxs-lookup"><span data-stu-id="177d8-171">**Usage based subscriptions over last 12 months**: Month over month trend of new usage based subscriptions and churned usage based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="177d8-172">**[Estimated cost of usage by customer over last 60 days]** (過去 60 か日間の顧客別推定使用コスト): 使用量ベースの顧客を過去 60 日間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-172">**Estimated cost of usage by customer over last 60 days**: Usage based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="177d8-173">これにより、収益性の高い使用量ベースの主要顧客が明確になります。</span><span class="sxs-lookup"><span data-stu-id="177d8-173">This will indicate top usage based customers bringing most revenue</span></span>

- <span data-ttu-id="177d8-174">**Estimated cost of usage by category over last 60 days** (過去 60 か日間のカテゴリ別推定使用コスト): 使用量ベースのサブスクリプションの従量制課金カテゴリを、過去 60 日間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-174">**Estimated cost of usage by category over last 60 days**: Meter categories of usage based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="177d8-175">**[Estimated cost of usage by subscription over last 60 days]** (過去 60 か日間のサブスクリプション別推定使用コスト): 使用量ベースのサブスクリプションを過去 60 日間にわたって集計された税抜き推定コスト (単位: ドル) の順に表示したレポート。</span><span class="sxs-lookup"><span data-stu-id="177d8-175">**Estimated cost of usage by subscription over last 60 days**: Usage based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="177d8-176">**Customer estimated usage cost by spending budget** (予算支出別顧客推定使用コスト): 顧客を、現在の使用量予算支出のしきい値 (100%) を超えた部分のパーセント率の順に表示。</span><span class="sxs-lookup"><span data-stu-id="177d8-176">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>


### <a name="azure-resource-usage-report"></a><span data-ttu-id="177d8-177">Azure リソース使用状況レポート:</span><span class="sxs-lookup"><span data-stu-id="177d8-177">Azure Resource Usage report:</span></span>

- <span data-ttu-id="177d8-178">**Usage of Azure resources by day for selected period** (選択した期間の 1 日当たりの Azure リソース使用量): 過去 60 日間のうち選択した期間の使用量ベースのサブスクリプション別および従量制課金リソース別の 1 日当たりの消費単位。</span><span class="sxs-lookup"><span data-stu-id="177d8-178">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="177d8-179">**Estimated usage cost of Azure resources for selected period** (選択した期間の Azure リソース推定使用コスト): 過去 60 日間のうち選択した期間の使用量ベースのサブスクリプション別および従量制課金リソース別の最新の価格カードに基づく推定使用コスト。</span><span class="sxs-lookup"><span data-stu-id="177d8-179">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage based subscription for selected period within the last 60 days.</span></span> 

## <a name="see-also"></a><span data-ttu-id="177d8-180">関連項目</span><span class="sxs-lookup"><span data-stu-id="177d8-180">See also</span></span>

[<span data-ttu-id="177d8-181">Power BI 用パートナー センター分析アプリの概要</span><span class="sxs-lookup"><span data-stu-id="177d8-181">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)


[<span data-ttu-id="177d8-182">Power BI 用パートナー センター分析アプリをインストールしてプレビューする</span><span class="sxs-lookup"><span data-stu-id="177d8-182">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
