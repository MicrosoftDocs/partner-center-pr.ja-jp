---
title: サブスクリプションとライセンスの分析 | パートナー センター
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: '[サブスクリプションとライセンス分析] ページのメトリックを使用して、注意が必要な成功と領域を特定する方法について説明します。'
author: LauraBrenner
ms.author: labrenne
ms.assetid: 1922FCE8-3A89-44ED-B4E1-BFCD2326BB06
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 494ef694410f193e3b76e476e5a6571b7ecf27e0
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722373"
---
# <a name="analyze-subscriptions-and-licenses"></a><span data-ttu-id="d26e1-104">サブスクリプションとライセンスの分析</span><span class="sxs-lookup"><span data-stu-id="d26e1-104">Analyze subscriptions and licenses</span></span> 

<span data-ttu-id="d26e1-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="d26e1-105">**Applies to**</span></span>

- <span data-ttu-id="d26e1-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="d26e1-106">Partner Center</span></span>
- <span data-ttu-id="d26e1-107">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="d26e1-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="d26e1-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="d26e1-108">**Appropriate roles**</span></span>

- <span data-ttu-id="d26e1-109">グローバル管理</span><span class="sxs-lookup"><span data-stu-id="d26e1-109">Global admin</span></span>
- <span data-ttu-id="d26e1-110">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="d26e1-110">User management admin</span></span>
- <span data-ttu-id="d26e1-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="d26e1-111">Admin agent</span></span>
- <span data-ttu-id="d26e1-112">販売代理店</span><span class="sxs-lookup"><span data-stu-id="d26e1-112">Sales agent</span></span>

<span data-ttu-id="d26e1-113">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="d26e1-113">Data drives business decisions.</span></span> <span data-ttu-id="d26e1-114">**サブスクリプションとライセンスの分析**ページのメトリックを使用して、パートナーの成功度や注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="d26e1-114">Use the metrics in the **Subscription and license analytics** page to identify your successes and areas that need more attention.</span></span> <span data-ttu-id="d26e1-115">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d26e1-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="d26e1-116">サブスクリプションとライセンスの分析は、クラウド ソリューション プロバイダー プログラムに参加しているパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="d26e1-116">Subscription license analytics is available only for partners in the Cloud Solution Provider program.</span></span>


<span data-ttu-id="d26e1-117">このレポートは、以下の製品に基づいてピボットで表示できます。</span><span class="sxs-lookup"><span data-stu-id="d26e1-117">This report can pivot based on the following products:</span></span>

 - <span data-ttu-id="d26e1-118">**Dynamics 365**: Dynamics 365 のデータ</span><span class="sxs-lookup"><span data-stu-id="d26e1-118">**Dynamics 365**: Dynamics 365 data</span></span>  
 - <span data-ttu-id="d26e1-119">**EMS**: エンタープライズ管理サービスのデータ</span><span class="sxs-lookup"><span data-stu-id="d26e1-119">**EMS**: Enterprise Management Services data</span></span>  
 - <span data-ttu-id="d26e1-120">**Microsoft 365**: Microsoft 365 データ</span><span class="sxs-lookup"><span data-stu-id="d26e1-120">**Microsoft 365**: Microsoft 365 data</span></span>  
 - <span data-ttu-id="d26e1-121">**Office 365**: Office 365 データ</span><span class="sxs-lookup"><span data-stu-id="d26e1-121">**Office 365**: Office 365 data</span></span>  


<span data-ttu-id="d26e1-122">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="d26e1-122">We are tracking the following metrics:</span></span>

<span data-ttu-id="d26e1-123">**要約**</span><span class="sxs-lookup"><span data-stu-id="d26e1-123">**Summary**</span></span>  
 - <span data-ttu-id="d26e1-124">**Subscriptions sold** (サブスクリプションの販売数): 指定した期間に作成されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="d26e1-124">**Subscriptions sold**: Count of subscriptions created for the specified time period</span></span>  
 - <span data-ttu-id="d26e1-125">**Licenses sold** (ライセンスの販売数): 指定した期間に販売されたライセンスの数</span><span class="sxs-lookup"><span data-stu-id="d26e1-125">**Licenses sold**: Count of licenses sold for the specified time period</span></span>   
 - <span data-ttu-id="d26e1-126">**Subscriptions renewing in 30 days** (30 日以内に更新するサブスクリプション): 指定した期間中に状態がアクティブで、**Autorenew** が true であるサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="d26e1-126">**Subscriptions renewing in 30 days**: Count of subscriptions where the status is active for the specified time period and where **Autorenew** is true</span></span>
 - <span data-ttu-id="d26e1-127">**Active subscriptions** (アクティブなサブスクリプション): 状態が **Active** であるサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="d26e1-127">**Active subscriptions**: Subscriptions where the status is **Active**</span></span>  
 - <span data-ttu-id="d26e1-128">**Suspended subscriptions** (中断されたサブスクリプション): 中断されたサブスクリプションの数、日付フィルターなし</span><span class="sxs-lookup"><span data-stu-id="d26e1-128">**Suspended subscriptions**: Count of suspended subscriptions, there is no date filter</span></span>  

<span data-ttu-id="d26e1-129">**製品の内訳**</span><span class="sxs-lookup"><span data-stu-id="d26e1-129">**Product breakdown**</span></span>  
 - <span data-ttu-id="d26e1-130">**Subscription count** (サブスクリプション数): サブスクリプションの販売数で並べ替えた上位 5 つの製品</span><span class="sxs-lookup"><span data-stu-id="d26e1-130">**Subscription count**: Top 5 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="d26e1-131">**License count** (ライセンス数): ライセンスの販売数で並べ替えた上位 5 つの製品</span><span class="sxs-lookup"><span data-stu-id="d26e1-131">**License count**: Top 5 products by sorted licenses sold</span></span>

<span data-ttu-id="d26e1-132">**サブスクリプションの維持**</span><span class="sxs-lookup"><span data-stu-id="d26e1-132">**Subscription Retention**</span></span>
 - <span data-ttu-id="d26e1-133">**Renewed subscriptions** (更新されたサブスクリプション): 過去 30 日間に更新されたサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="d26e1-133">**Renewed subscriptions**: Subscriptions that renewed in the last 30 days</span></span>  

<span data-ttu-id="d26e1-134">**サブスクリプションのチャーン**</span><span class="sxs-lookup"><span data-stu-id="d26e1-134">**Subscription churn**</span></span>  
 - <span data-ttu-id="d26e1-135">**New subscriptions** (新規サブスクリプション): 期間中の新しいサブスクリプションの数 (試用版プランを除く)</span><span class="sxs-lookup"><span data-stu-id="d26e1-135">**New subscriptions**: count of new subscriptions for the time period, excluding trial offers</span></span>  
 - <span data-ttu-id="d26e1-136">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="d26e1-136">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="d26e1-137">**中断されたサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="d26e1-137">**Suspended subscriptions**</span></span>  
 - <span data-ttu-id="d26e1-138">状態が **Suspended** (中断) であるすべてのサブスクリプションの一覧 (試用版プランを除く)</span><span class="sxs-lookup"><span data-stu-id="d26e1-138">List of all subscriptions with a status of **Suspended**, excluding trial offers</span></span>  
  
<span data-ttu-id="d26e1-139">**アクティブなサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="d26e1-139">**Active subscriptions**</span></span>
 - <span data-ttu-id="d26e1-140">すべてのアクティブなサブスクリプションの一覧</span><span class="sxs-lookup"><span data-stu-id="d26e1-140">List of all active subscriptions</span></span>  

<span data-ttu-id="d26e1-141">**試用版のサブスクリプションの変換**</span><span class="sxs-lookup"><span data-stu-id="d26e1-141">**Trial subscription conversions**</span></span>  
 - <span data-ttu-id="d26e1-142">**Trial conversion** (試用版の変換): 指定した期間中に試用版から有料版への変換が行われたすべての**アクティブ** サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="d26e1-142">**Trial conversion**: Count of all **Active** subscriptions where trial paid to conversion occurred during the specified time period</span></span>  

<span data-ttu-id="d26e1-143">**30 日以内に終了する試用版サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="d26e1-143">**Trial subscriptions ending in 30 days**</span></span>  
 - <span data-ttu-id="d26e1-144">開始されたが、終了日が 30 日以内であり、有料版の開始日がサブスクリプションに関連付けられていない試用版の一覧</span><span class="sxs-lookup"><span data-stu-id="d26e1-144">List of trials that were started, where the end date is within 30 days, and there is no paid start date associated with the subscription</span></span>  

  