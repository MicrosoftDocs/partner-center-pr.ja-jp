---
title: 間接リセラーのパフォーマンス分析 | パートナー センター
ms.date: 07/12/2018
Description: 成功とさらに注意が必要になる領域を識別するために間接リセラーのパフォーマンスに関するデータを取得します。
Author: Xansky
ms.author: mhopkins
ms.assetid: 4D7DAD9D-4B69-4741-8E80-44256320982E
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: c86640d0334063b8daaffd3c447597a57b9662dd
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134902"
---
# <a name="analyze-indirect-resellers-performance"></a><span data-ttu-id="f7b2b-104">間接リセラーのパフォーマンス分析</span><span class="sxs-lookup"><span data-stu-id="f7b2b-104">Analyze indirect resellers performance</span></span> 

<span data-ttu-id="f7b2b-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-105">**Applies to**</span></span>
- <span data-ttu-id="f7b2b-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="f7b2b-106">Partner Center</span></span>

<span data-ttu-id="f7b2b-107">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-107">Data drives business decisions.</span></span> <span data-ttu-id="f7b2b-108">**リセラー分析**のページのメトリックを使用して、パートナーの成功度、間接リセラーの成功度、注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-108">Use the metrics in the **Reseller analytics** page to identify your successes, your indirect resellers' successes, and areas that need more attention.</span></span> <span data-ttu-id="f7b2b-109">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-109">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="f7b2b-110">間接リセラー分析は、クラウド ソリューション プロバイダー プログラムに参加しているパートナーのみが利用できます。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-110">Indirect resellers analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="f7b2b-111">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-111">We are tracking the following metrics:</span></span>

<span data-ttu-id="f7b2b-112">**要約**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-112">**Summary**</span></span>  
 - <span data-ttu-id="f7b2b-113">**再販業者の合計**:サブスクリプションの最終日にアクティブな再販業者の数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-113">**Total resellers**: Count of active resellers on the last day of the subscription</span></span>  
 - <span data-ttu-id="f7b2b-114">**新しいリセラー**:指定した期間内の新しい間接リセラーの数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-114">**New resellers**: Count of new indirect resellers for the specified time period</span></span>  
 - <span data-ttu-id="f7b2b-115">**アクティブな販売店**:サブスクリプションの状態がプロビジョニング解除できませんし、MPNID は 1 つ以上のサブスクリプション間接リセラーの数します。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-115">**Active resellers**: Count of indirect resellers where the MPNID is at least 1 subscription, and where the subscription status is not deprovisioned</span></span>  
 - <span data-ttu-id="f7b2b-116">**再販業者をいっそう**:サブスクリプション間接リセラーの数が、指定された期間で販売されています。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-116">**Transacting resellers**: Count of indirect resellers with a subscription sold in the specified time period</span></span>  

<span data-ttu-id="f7b2b-117">**市場別の販売店**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-117">**Resellers by market**</span></span>  
 - <span data-ttu-id="f7b2b-118">地域別の合計リセラー数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-118">Total resellers by geographic location</span></span>  

<span data-ttu-id="f7b2b-119">**サブスクリプションで最上位の再販業者販売**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-119">**Top resellers by subscriptions sold**</span></span>
 - <span data-ttu-id="f7b2b-120">リセラーのサブスクリプション販売数で並べ替えられたリセラーの一覧</span><span class="sxs-lookup"><span data-stu-id="f7b2b-120">A list of resellers, sorted by the number of subscriptions they've sold</span></span>  

<span data-ttu-id="f7b2b-121">**サブスクリプションの数によって上位製品**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-121">**Top products by subscription count**</span></span>  
 - <span data-ttu-id="f7b2b-122">**Dynamics 365**:Dynamics 365 製品が販売されているサブスクリプションによって並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-122">**Dynamics 365**: Dynamics 365 products sorted by subscriptions sold</span></span>  
 - <span data-ttu-id="f7b2b-123">**EMS**:エンタープライズ管理サービスのサブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-123">**EMS**: Number of Enterprise Management Services subscriptions sold</span></span>  
 - <span data-ttu-id="f7b2b-124">**Microsoft 365**:Microsoft 365 のサブスクリプションの販売数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-124">**Microsoft 365**: Number of Microsoft 365 subscriptions sold</span></span>  
 - <span data-ttu-id="f7b2b-125">**Office 365**:Office 365 製品が販売されているサブスクリプションによって並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="f7b2b-125">**Office 365**: Office 365 products sorted by subscriptions sold</span></span>  

<span data-ttu-id="f7b2b-126">**新しいサブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-126">**New subscriptions**</span></span>  
 - <span data-ttu-id="f7b2b-127">日付ごとの追加された新規サブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-127">The number of new subscriptions added by date</span></span>  

<span data-ttu-id="f7b2b-128">**サブスクリプションの変更頻度**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-128">**Subscription churn**</span></span>  
 - <span data-ttu-id="f7b2b-129">**新しいサブスクリプション**:日付によって追加された新しいサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-129">**New subscriptions**: Count of new subscriptions added by date</span></span>  
 - <span data-ttu-id="f7b2b-130">**サブスクリプションをプロビジョニング解除**:プロビジョニングが解除されたり、日付によって中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-130">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

<span data-ttu-id="f7b2b-131">**新しい販売店の詳細**</span><span class="sxs-lookup"><span data-stu-id="f7b2b-131">**New reseller details**</span></span>  
 - <span data-ttu-id="f7b2b-132">**再販業者名**:間接リセラーの名前</span><span class="sxs-lookup"><span data-stu-id="f7b2b-132">**Reseller name**: Names of indirect resellers</span></span>  
 - <span data-ttu-id="f7b2b-133">**場所**:間接リセラーの動作、市場</span><span class="sxs-lookup"><span data-stu-id="f7b2b-133">**Location**: Markets where the indirect resellers operate</span></span>  
 - <span data-ttu-id="f7b2b-134">**サブスクリプション**:サブスクリプションが、再販業者の販売数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-134">**Subscriptions**: Number of subscriptions the reseller has sold</span></span>  
 - <span data-ttu-id="f7b2b-135">**ライセンス**:すべてのサブスクリプションで、再販業者が販売ライセンスの合計数</span><span class="sxs-lookup"><span data-stu-id="f7b2b-135">**Licenses**: Total number of licenses the reseller has sold across all subscriptions</span></span>  
  
  