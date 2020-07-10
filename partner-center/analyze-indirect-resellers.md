---
title: 間接リセラーのパフォーマンス分析
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: 分析を使用して、間接リセラーがどのように実行されているかを確認します。成功と領域の両方で、さらに注意が必要になる場合があります。
author: amitravat
ms.author: amrava
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 33d435b6497f84d87ce866624deb47e2bd6ebc89
ms.sourcegitcommit: cba3c73520b8f72d0ba9ca3725f355cab79342c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/09/2020
ms.locfileid: "86175968"
---
# <a name="use-analytics-to-analyze-performance-of-your-indirect-resellers"></a><span data-ttu-id="24468-104">分析を使用して間接リセラーのパフォーマンスを分析する</span><span class="sxs-lookup"><span data-stu-id="24468-104">Use analytics to analyze performance of your indirect resellers</span></span>

<span data-ttu-id="24468-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="24468-105">**Applies to**</span></span>

- <span data-ttu-id="24468-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="24468-106">Partner Center</span></span>
- <span data-ttu-id="24468-107">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="24468-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="24468-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="24468-108">**Appropriate roles**</span></span>

- <span data-ttu-id="24468-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="24468-109">Global admin</span></span>
- <span data-ttu-id="24468-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="24468-110">User management admin</span></span>
- <span data-ttu-id="24468-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="24468-111">Admin agent</span></span>
- <span data-ttu-id="24468-112">販売代理店</span><span class="sxs-lookup"><span data-stu-id="24468-112">Sales agent</span></span>

<span data-ttu-id="24468-113">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="24468-113">Data drives business decisions.</span></span> <span data-ttu-id="24468-114">**リセラー分析**のページのメトリックを使用して、パートナーの成功度、間接リセラーの成功度、注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="24468-114">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="24468-115">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="24468-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="24468-116">間接リセラー分析は、クラウド ソリューション プロバイダー プログラムに参加しているパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="24468-116">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a><span data-ttu-id="24468-117">表示可能なリセラー分析メトリックの種類</span><span class="sxs-lookup"><span data-stu-id="24468-117">Types of reseller analytics metrics you can view</span></span>

<span data-ttu-id="24468-118">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="24468-118">We are tracking the following metrics:</span></span>

<span data-ttu-id="24468-119">**まとめ**</span><span class="sxs-lookup"><span data-stu-id="24468-119">**Summary**</span></span>  
 - <span data-ttu-id="24468-120">**Total resellers** (リセラーの合計数): サブスクリプションの最終日にアクティブなリセラーの数</span><span class="sxs-lookup"><span data-stu-id="24468-120">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="24468-121">**New resellers** (新規リセラー数): 指定した期間の新規間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="24468-121">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="24468-122">**Active resellers** (アクティブなリセラー数): MPNID に 1 つ以上のサブスクリプションがあり、サブスクリプションの状態がプロビジョニング解除ではない間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="24468-122">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="24468-123">**Transacting resellers** (取引のあるリセラー数): 指定した期間に販売したサブスクリプションがある間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="24468-123">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="24468-124">**市場別のリセラー数**</span><span class="sxs-lookup"><span data-stu-id="24468-124">**Resellers by market**</span></span>  
 - <span data-ttu-id="24468-125">地域別の合計リセラー数</span><span class="sxs-lookup"><span data-stu-id="24468-125">Total resellers by geographic location</span></span>  

<span data-ttu-id="24468-126">**サブスクリプションの販売数による上位リセラー**</span><span class="sxs-lookup"><span data-stu-id="24468-126">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="24468-127">リセラーのサブスクリプション販売数で並べ替えられたリセラーの一覧</span><span class="sxs-lookup"><span data-stu-id="24468-127">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="24468-128">**サブスクリプション数による上位製品**</span><span class="sxs-lookup"><span data-stu-id="24468-128">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="24468-129">**Dynamics 365**: サブスクリプションの販売数で並べ替えられた Dynamics 365 製品</span><span class="sxs-lookup"><span data-stu-id="24468-129">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="24468-130">**EMS**: エンタープライズ管理サービス サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="24468-130">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="24468-131">**Microsoft 365**: Microsoft 365 サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="24468-131">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="24468-132">**Office 365**: サブスクリプションの販売数で並べ替えられた Office 365 製品</span><span class="sxs-lookup"><span data-stu-id="24468-132">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="24468-133">**新しいサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="24468-133">**New subscriptions**</span></span>  
 - <span data-ttu-id="24468-134">日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="24468-134">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="24468-135">**サブスクリプションのチャーン**</span><span class="sxs-lookup"><span data-stu-id="24468-135">**Subscription churn**</span></span>  
 - <span data-ttu-id="24468-136">**New subscriptions** (新規サブスクリプション数): 日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="24468-136">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="24468-137">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="24468-137">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="24468-138">**新規リセラーの詳細**</span><span class="sxs-lookup"><span data-stu-id="24468-138">**New reseller details**</span></span>  
 - <span data-ttu-id="24468-139">**Reseller name** (リセラー名): 間接リセラーの名前</span><span class="sxs-lookup"><span data-stu-id="24468-139">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="24468-140">**Location** (場所): 間接リセラーが営業している市場</span><span class="sxs-lookup"><span data-stu-id="24468-140">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="24468-141">**Subscriptions** (サブスクリプション数): リセラーが販売したサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="24468-141">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="24468-142">**Licenses** (ライセンス数): すべてのサブスクリプションを合わせてリセラーが販売したライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="24468-142">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
## <a name="next-steps"></a><span data-ttu-id="24468-143">次の手順</span><span class="sxs-lookup"><span data-stu-id="24468-143">Next steps</span></span>

- [<span data-ttu-id="24468-144">サブスクリプションとライセンスを分析して、ビジネス上の意思決定を促進する</span><span class="sxs-lookup"><span data-stu-id="24468-144">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)