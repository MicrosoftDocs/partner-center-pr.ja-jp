---
title: 間接リセラーのパフォーマンス分析
description: 分析を使用して、間接リセラーがどのように実行されているかを確認します。成功と領域の両方で、さらに注意が必要になる場合があります。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh
ms.author: shganesh
ms.topic: article
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/13/2020
ms.openlocfilehash: b7158f0ba52cece8b143cbaf592f3b0c4667fe27
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474055"
---
# <a name="use-analytics-to-analyze-the-performance-of-your-indirect-resellers"></a><span data-ttu-id="afd20-103">分析を使用して間接リセラーのパフォーマンスを分析する</span><span class="sxs-lookup"><span data-stu-id="afd20-103">Use analytics to analyze the performance of your indirect resellers</span></span>

<span data-ttu-id="afd20-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="afd20-104">**Appropriate roles**</span></span>

- <span data-ttu-id="afd20-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="afd20-105">Global admin</span></span>
- <span data-ttu-id="afd20-106">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="afd20-106">User management admin</span></span>


<span data-ttu-id="afd20-107">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="afd20-107">Data drives business decisions.</span></span> <span data-ttu-id="afd20-108">**リセラー分析** のページのメトリックを使用して、パートナーの成功度、間接リセラーの成功度、注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="afd20-108">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="afd20-109">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="afd20-109">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="afd20-110">間接リセラー分析は、クラウドソリューションプロバイダープログラムの間接プロバイダーに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="afd20-110">Indirect reseller analytics is available only for Indirect providers in the Cloud Solution Provider program.</span></span>

## <a name="types-of-reseller-analytics-metrics-you-can-view"></a><span data-ttu-id="afd20-111">表示可能なリセラー分析メトリックの種類</span><span class="sxs-lookup"><span data-stu-id="afd20-111">Types of reseller analytics metrics you can view</span></span>

<span data-ttu-id="afd20-112">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="afd20-112">We are tracking the following metrics:</span></span>

<span data-ttu-id="afd20-113">**まとめ**</span><span class="sxs-lookup"><span data-stu-id="afd20-113">**Summary**</span></span>  
 - <span data-ttu-id="afd20-114">**Total resellers** (リセラーの合計数): サブスクリプションの最終日にアクティブなリセラーの数</span><span class="sxs-lookup"><span data-stu-id="afd20-114">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="afd20-115">**New resellers** (新規リセラー数): 指定した期間の新規間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="afd20-115">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="afd20-116">**Active resellers** (アクティブなリセラー数): MPNID に 1 つ以上のサブスクリプションがあり、サブスクリプションの状態がプロビジョニング解除ではない間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="afd20-116">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="afd20-117">**Transacting resellers** (取引のあるリセラー数): 指定した期間に販売したサブスクリプションがある間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="afd20-117">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="afd20-118">**市場別のリセラー数**</span><span class="sxs-lookup"><span data-stu-id="afd20-118">**Resellers by market**</span></span>  
 - <span data-ttu-id="afd20-119">地域別の合計リセラー数</span><span class="sxs-lookup"><span data-stu-id="afd20-119">Total resellers by geographic location</span></span>  

<span data-ttu-id="afd20-120">**サブスクリプションの販売数による上位リセラー**</span><span class="sxs-lookup"><span data-stu-id="afd20-120">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="afd20-121">リセラーのサブスクリプション販売数で並べ替えられたリセラーの一覧</span><span class="sxs-lookup"><span data-stu-id="afd20-121">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="afd20-122">**サブスクリプション数による上位製品**</span><span class="sxs-lookup"><span data-stu-id="afd20-122">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="afd20-123">**Dynamics 365**: サブスクリプションの販売数で並べ替えられた Dynamics 365 製品</span><span class="sxs-lookup"><span data-stu-id="afd20-123">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="afd20-124">**EMS**: エンタープライズ管理サービス サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="afd20-124">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="afd20-125">**Microsoft 365**: Microsoft 365 サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="afd20-125">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="afd20-126">**Office 365**: サブスクリプションの販売数で並べ替えられた Office 365 製品</span><span class="sxs-lookup"><span data-stu-id="afd20-126">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="afd20-127">**新しいサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="afd20-127">**New subscriptions**</span></span>  
 - <span data-ttu-id="afd20-128">日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="afd20-128">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="afd20-129">**サブスクリプションのチャーン**</span><span class="sxs-lookup"><span data-stu-id="afd20-129">**Subscription churn**</span></span>  
 - <span data-ttu-id="afd20-130">**New subscriptions** (新規サブスクリプション数): 日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="afd20-130">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="afd20-131">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="afd20-131">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="afd20-132">**新規リセラーの詳細**</span><span class="sxs-lookup"><span data-stu-id="afd20-132">**New reseller details**</span></span>  
 - <span data-ttu-id="afd20-133">**Reseller name** (リセラー名): 間接リセラーの名前</span><span class="sxs-lookup"><span data-stu-id="afd20-133">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="afd20-134">**Location** (場所): 間接リセラーが営業している市場</span><span class="sxs-lookup"><span data-stu-id="afd20-134">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="afd20-135">**Subscriptions** (サブスクリプション数): リセラーが販売したサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="afd20-135">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="afd20-136">**Licenses** (ライセンス数): すべてのサブスクリプションを合わせてリセラーが販売したライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="afd20-136">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  

<span data-ttu-id="afd20-137">**MPA の署名された状態**</span><span class="sxs-lookup"><span data-stu-id="afd20-137">**MPA signed status**</span></span>

<span data-ttu-id="afd20-138">このセクションでは、CSP 間接リセラーの MPA の署名された状態について説明します。</span><span class="sxs-lookup"><span data-stu-id="afd20-138">This section provides the status of MPA signed status of the CSP Indirect Resellers.</span></span>

 - <span data-ttu-id="afd20-139">**再販業者名**: CSP 間接リセラーの名前</span><span class="sxs-lookup"><span data-stu-id="afd20-139">**Reseller name**: Name of the CSP indirect reseller</span></span>
 - <span data-ttu-id="afd20-140">**MPN id**: 間接リセラーの MPN id</span><span class="sxs-lookup"><span data-stu-id="afd20-140">**MPN ID**: MPN ID of the indirect reseller</span></span>
 - <span data-ttu-id="afd20-141">**リージョン**: 間接リセラーが運用するリージョン</span><span class="sxs-lookup"><span data-stu-id="afd20-141">**Region**: Region where the indirect reseller operates</span></span>
 - <span data-ttu-id="afd20-142">**MPN 審査 status**: 間接リセラーの審査の状態</span><span class="sxs-lookup"><span data-stu-id="afd20-142">**MPN vetting status**: Vetting status of the indirect reseller</span></span>
 - <span data-ttu-id="afd20-143">**Mpa の署名済みステータス**: 間接リセラーの mpa 署名状態</span><span class="sxs-lookup"><span data-stu-id="afd20-143">**MPA signed status**: MPA signing status for the indirect reseller</span></span>

<span data-ttu-id="afd20-144">グラフのダウンロードアイコンをクリックして、追加のディメンションを含む MPA 署名済み状態データをダウンロードします</span><span class="sxs-lookup"><span data-stu-id="afd20-144">Click on the download icon in the chart to download MPA signed status data with additional dimensions</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="afd20-145">次のステップ</span><span class="sxs-lookup"><span data-stu-id="afd20-145">Next steps</span></span>

- [<span data-ttu-id="afd20-146">サブスクリプションとライセンスを分析して、ビジネス上の意思決定を促進する</span><span class="sxs-lookup"><span data-stu-id="afd20-146">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)