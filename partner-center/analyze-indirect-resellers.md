---
title: 間接リセラーのパフォーマンス分析 | パートナー センター
ms.date: 08/02/2019
Description: 間接リセラーのパフォーマンスに関するデータを取得して、成功度とさらに注意が必要な領域を識別します。
author: LauraBrenner
ms.author: labrenne
ms.assetid: 4D7DAD9D-4B69-4741-8E80-44256320982E
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: c46a155b99087f6d6019db4ed81247c269883ae2
ms.sourcegitcommit: c8d42c122f420d4116239530c01ed28cb2ab6b30
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2019
ms.locfileid: "68781990"
---
# <a name="analyze-indirect-resellers-performance"></a><span data-ttu-id="3c1d3-104">間接リセラーのパフォーマンス分析</span><span class="sxs-lookup"><span data-stu-id="3c1d3-104">Analyze indirect resellers performance</span></span> 

<span data-ttu-id="3c1d3-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-105">**Applies to**</span></span>
- <span data-ttu-id="3c1d3-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="3c1d3-106">Partner Center</span></span>

<span data-ttu-id="3c1d3-107">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="3c1d3-107">Data drives business decisions.</span></span> <span data-ttu-id="3c1d3-108">**リセラー分析**のページのメトリックを使用して、パートナーの成功度、間接リセラーの成功度、注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="3c1d3-108">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="3c1d3-109">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3c1d3-109">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="3c1d3-110">間接リセラー分析は、クラウド ソリューション プロバイダー プログラムに参加しているパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="3c1d3-110">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="3c1d3-111">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="3c1d3-111">We are tracking the following metrics:</span></span>

<span data-ttu-id="3c1d3-112">**要約**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-112">**Summary**</span></span>  
 - <span data-ttu-id="3c1d3-113">**合計リセラー数**: サブスクリプションの最終日にアクティブなリセラーの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-113">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="3c1d3-114">**新規リセラー数**: 指定した期間の新規間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-114">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="3c1d3-115">**アクティブなリセラー数**: MPNID に 1 つ以上のサブスクリプションがあり、サブスクリプションの状態がプロビジョニング解除されていない間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-115">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="3c1d3-116">**取引のあるリセラー数**: 指定した期間に販売したサブスクリプションがある間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-116">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="3c1d3-117">**市場別のリセラー数**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-117">**Resellers by market**</span></span>  
 - <span data-ttu-id="3c1d3-118">地域別の合計リセラー数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-118">Total resellers by geographic location</span></span>  

<span data-ttu-id="3c1d3-119">**サブスクリプションの販売数による上位リセラー**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-119">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="3c1d3-120">リセラーのサブスクリプション販売数で並べ替えられたリセラーの一覧</span><span class="sxs-lookup"><span data-stu-id="3c1d3-120">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="3c1d3-121">**サブスクリプション数による上位製品**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-121">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="3c1d3-122">**Dynamics 365**: サブスクリプションの販売数で並べ替えられた Dynamics 365 製品</span><span class="sxs-lookup"><span data-stu-id="3c1d3-122">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="3c1d3-123">**EMS**: エンタープライズ管理サービス サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-123">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="3c1d3-124">**Microsoft 365**: Microsoft 365 サブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-124">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="3c1d3-125">**Office 365**: サブスクリプションの販売数で並べ替えられた Office 365 製品</span><span class="sxs-lookup"><span data-stu-id="3c1d3-125">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="3c1d3-126">**新規サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-126">**New subscriptions**</span></span>  
 - <span data-ttu-id="3c1d3-127">日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-127">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="3c1d3-128">**サブスクリプションのチャーン**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-128">**Subscription churn**</span></span>  
 - <span data-ttu-id="3c1d3-129">**新規サブスクリプション**: 日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-129">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="3c1d3-130">**プロビジョニング解除されたサブスクリプション数**: 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-130">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="3c1d3-131">**新規リセラーの詳細**</span><span class="sxs-lookup"><span data-stu-id="3c1d3-131">**New reseller details**</span></span>  
 - <span data-ttu-id="3c1d3-132">**リセラー名**: 間接リセラーの名前</span><span class="sxs-lookup"><span data-stu-id="3c1d3-132">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="3c1d3-133">**場所**:間接リセラーが営業している市場</span><span class="sxs-lookup"><span data-stu-id="3c1d3-133">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="3c1d3-134">**サブスクリプション**: リセラーが販売したサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-134">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="3c1d3-135">**ライセンス**: すべてのサブスクリプションを合わせてリセラーが販売したライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="3c1d3-135">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
  