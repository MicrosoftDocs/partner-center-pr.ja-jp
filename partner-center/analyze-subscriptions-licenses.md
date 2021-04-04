---
title: サブスクリプションとライセンスの分析
description: '[サブスクリプションとライセンス分析] ページのメトリックを使用して、注意が必要な成功と領域を特定する方法について説明します。'
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 03/31/2021
ms.openlocfilehash: 3f84026cc6402bea71837b06a5e330f2c879a06b
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103793"
---
# <a name="analyze-subscriptions-and-licenses-to-help-you-drive-business-decisions-and-new-goals"></a><span data-ttu-id="a247a-103">サブスクリプションとライセンスを分析して、ビジネス上の意思決定や新しい目標を促進</span><span class="sxs-lookup"><span data-stu-id="a247a-103">Analyze subscriptions and licenses to help you drive business decisions and new goals</span></span>

<span data-ttu-id="a247a-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="a247a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a247a-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a247a-105">Global admin</span></span>
- <span data-ttu-id="a247a-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="a247a-106">User management admin</span></span>
- <span data-ttu-id="a247a-107">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="a247a-107">Admin agent</span></span>
- <span data-ttu-id="a247a-108">販売代理店</span><span class="sxs-lookup"><span data-stu-id="a247a-108">Sales agent</span></span>

<span data-ttu-id="a247a-109">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="a247a-109">Data drives business decisions.</span></span> <span data-ttu-id="a247a-110">[ **サブスクリプションとライセンス分析** ] ページのメトリックを使用して、さらに注意が必要な成功と領域を特定します。</span><span class="sxs-lookup"><span data-stu-id="a247a-110">Use the metrics in the **Subscription and license analytics** page to identify your successes and areas that need more attention.</span></span> <span data-ttu-id="a247a-111">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a247a-111">Use this information as you plan new business goals.</span></span>

<span data-ttu-id="a247a-112">**CSP TTM 収益 (米国ドル)**: このメトリックは、この csp アカウントが関連付けられているパートナーの場所アカウントとパートナーのグローバルアカウント (PGA) の末尾の12か月 (ttm) に対して請求される、集計された csp を表します。</span><span class="sxs-lookup"><span data-stu-id="a247a-112">**CSP TTM Revenue (USD)**: This metric represents the aggregated CSP billed revenue (USD) for the trailing twelve months (TTM) for the Partner Location Accounts and Partner Global Account (PGA) this CSP account is associated with.</span></span> <span data-ttu-id="a247a-113">別の PGA がある他の CSP アカウントがある場合は、それぞれにサインインして、対応する集計された TTM 収益を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a247a-113">If you have other CSP accounts with a different PGA, you must sign in into each of them to view the corresponding aggregated TTM revenue.</span></span>  <span data-ttu-id="a247a-114">[Download details] \ (ダウンロードの詳細 \) リンクをクリックすると、MPN ID ごとの TTM 収益 (USD) の内訳が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a247a-114">Click on the download details link to get a breakdown of the TTM revenue (USD) per MPN ID.</span></span>

>[!NOTE]
><span data-ttu-id="a247a-115">商用の現地通貨料金 (レガシコマース FX) は、米ドルの +/-5% 以内に管理されます。</span><span class="sxs-lookup"><span data-stu-id="a247a-115">Local currency prices (Legacy Commerce FX) in Commercial are managed to within +/-5% of US dollars.</span></span> <span data-ttu-id="a247a-116">従来のコマース販売率 (FX) は、最新のコマースエクスペリエンスで Azure によって使用される請求 FX の料金とは異なります。</span><span class="sxs-lookup"><span data-stu-id="a247a-116">The Legacy Commerce exchange rate (FX) is different from billing FX rates used by Azure in the Modern Commerce experience.</span></span> <span data-ttu-id="a247a-117">最新のコマース請求 FX 料金は、Microsoft P&L 料金 (Reuters FX レート from 財務省 feed) に基づいています。</span><span class="sxs-lookup"><span data-stu-id="a247a-117">The Modern Commerce billing FX rates are based on Microsoft P&L rates (Reuters FX rates from Treasury feed).</span></span> <span data-ttu-id="a247a-118">従来のコマース FX 料金は Microsoft 社外秘です。</span><span class="sxs-lookup"><span data-stu-id="a247a-118">Legacy Commerce FX rates are Microsoft confidential.</span></span>


<span data-ttu-id="a247a-119">レポートの残りの部分は、次の製品に基づいてピボットできます。</span><span class="sxs-lookup"><span data-stu-id="a247a-119">The rest of the report can pivot based on the following products:</span></span>

 - <span data-ttu-id="a247a-120">**Dynamics 365**: Dynamics 365 のデータ</span><span class="sxs-lookup"><span data-stu-id="a247a-120">**Dynamics 365**: Dynamics 365 data</span></span>  
 - <span data-ttu-id="a247a-121">**EMS**: エンタープライズ管理サービスのデータ</span><span class="sxs-lookup"><span data-stu-id="a247a-121">**EMS**: Enterprise Management Services data</span></span>  
 - <span data-ttu-id="a247a-122">**Microsoft 365**: Microsoft 365 データ</span><span class="sxs-lookup"><span data-stu-id="a247a-122">**Microsoft 365**: Microsoft 365 data</span></span>  
 - <span data-ttu-id="a247a-123">**Office 365**: Office 365 データ</span><span class="sxs-lookup"><span data-stu-id="a247a-123">**Office 365**: Office 365 data</span></span>  


## <a name="types-of-subscription-and-license-metrics-you-can-view"></a><span data-ttu-id="a247a-124">表示可能なサブスクリプションとライセンスメトリックの種類</span><span class="sxs-lookup"><span data-stu-id="a247a-124">Types of subscription and license metrics you can view</span></span>

<span data-ttu-id="a247a-125">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="a247a-125">We are tracking the following metrics:</span></span>

<span data-ttu-id="a247a-126">**まとめ**</span><span class="sxs-lookup"><span data-stu-id="a247a-126">**Summary**</span></span>  
 - <span data-ttu-id="a247a-127">**Subscriptions sold** (サブスクリプションの販売数): 指定した期間に作成されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="a247a-127">**Subscriptions sold**: Count of subscriptions created for the specified time period</span></span>  
  
 - <span data-ttu-id="a247a-128">**Licenses sold** (ライセンスの販売数): 指定した期間に販売されたライセンスの数</span><span class="sxs-lookup"><span data-stu-id="a247a-128">**Licenses sold**: Count of licenses sold for the specified time period</span></span>  
  
 - <span data-ttu-id="a247a-129">**Subscriptions renewing in 30 days** (30 日以内に更新するサブスクリプション): 指定した期間中に状態がアクティブで、**Autorenew** が true であるサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="a247a-129">**Subscriptions renewing in 30 days**: Count of subscriptions where the status is active for the specified time period and where **Autorenew** is true</span></span>
 
 - <span data-ttu-id="a247a-130">**Active subscriptions** (アクティブなサブスクリプション): 状態が **Active** であるサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="a247a-130">**Active subscriptions**: Subscriptions where the status is **Active**</span></span>  
 
 - <span data-ttu-id="a247a-131">**Suspended subscriptions** (中断されたサブスクリプション): 中断されたサブスクリプションの数、日付フィルターなし</span><span class="sxs-lookup"><span data-stu-id="a247a-131">**Suspended subscriptions**: Count of suspended subscriptions, there is no date filter</span></span>  

<span data-ttu-id="a247a-132">**製品の内訳**</span><span class="sxs-lookup"><span data-stu-id="a247a-132">**Product breakdown**</span></span>
  
 - <span data-ttu-id="a247a-133">**Subscription count** (サブスクリプション数): サブスクリプションの販売数で並べ替えた上位 5 つの製品</span><span class="sxs-lookup"><span data-stu-id="a247a-133">**Subscription count**: Top 5 products sorted by subscriptions sold</span></span>  
 
 - <span data-ttu-id="a247a-134">**License count** (ライセンス数): ライセンスの販売数で並べ替えた上位 5 つの製品</span><span class="sxs-lookup"><span data-stu-id="a247a-134">**License count**: Top 5 products by sorted licenses sold</span></span>

<span data-ttu-id="a247a-135">**サブスクリプションの維持**</span><span class="sxs-lookup"><span data-stu-id="a247a-135">**Subscription Retention**</span></span>

 - <span data-ttu-id="a247a-136">**Renewed subscriptions** (更新されたサブスクリプション): 過去 30 日間に更新されたサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="a247a-136">**Renewed subscriptions**: Subscriptions that renewed in the last 30 days</span></span>  

<span data-ttu-id="a247a-137">**サブスクリプションのチャーン**</span><span class="sxs-lookup"><span data-stu-id="a247a-137">**Subscription churn**</span></span>  
 - <span data-ttu-id="a247a-138">**New subscriptions** (新規サブスクリプション): 期間中の新しいサブスクリプションの数 (試用版プランを除く)</span><span class="sxs-lookup"><span data-stu-id="a247a-138">**New subscriptions**: count of new subscriptions for the time period, excluding trial offers</span></span>  
 
 - <span data-ttu-id="a247a-139">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="a247a-139">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="a247a-140">**中断されたサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="a247a-140">**Suspended subscriptions**</span></span> 
 
 - <span data-ttu-id="a247a-141">状態が **Suspended** (中断) であるすべてのサブスクリプションの一覧 (試用版プランを除く)</span><span class="sxs-lookup"><span data-stu-id="a247a-141">List of all subscriptions with a status of **Suspended**, excluding trial offers</span></span>  
  
<span data-ttu-id="a247a-142">**アクティブなサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="a247a-142">**Active subscriptions**</span></span>

 - <span data-ttu-id="a247a-143">すべてのアクティブなサブスクリプションの一覧</span><span class="sxs-lookup"><span data-stu-id="a247a-143">List of all active subscriptions</span></span>  

<span data-ttu-id="a247a-144">**試用版のサブスクリプションの変換**</span><span class="sxs-lookup"><span data-stu-id="a247a-144">**Trial subscription conversions**</span></span>  

 - <span data-ttu-id="a247a-145">**Trial conversion** (試用版の変換): 指定した期間中に試用版から有料版への変換が行われたすべての **アクティブ** サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="a247a-145">**Trial conversion**: Count of all **Active** subscriptions where trial paid to conversion occurred during the specified time period</span></span>  

<span data-ttu-id="a247a-146">**30 日以内に終了する試用版サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="a247a-146">**Trial subscriptions ending in 30 days**</span></span>  

 - <span data-ttu-id="a247a-147">開始されたが、終了日が 30 日以内であり、有料版の開始日がサブスクリプションに関連付けられていない試用版の一覧</span><span class="sxs-lookup"><span data-stu-id="a247a-147">List of trials that were started, where the end date is within 30 days, and there is no paid start date associated with the subscription</span></span>  



## <a name="next-steps"></a><span data-ttu-id="a247a-148">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a247a-148">Next steps</span></span>

- [<span data-ttu-id="a247a-149">間接リセラーのパフォーマンスを分析する</span><span class="sxs-lookup"><span data-stu-id="a247a-149">Analyze the performance of your indirect resellers</span></span>](analyze-indirect-resellers.md)