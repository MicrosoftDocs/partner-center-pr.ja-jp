---
title: Azure の使用状況を分析してビジネスの成長に役立てます
ms.date: 05/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: パートナーセンターを使用して、顧客の Azure サブスクリプションの使用状況に関するデータを取得する方法について説明します。
author: amrava
ms.author: amrava
ms.topic: article
keywords: ビジネス データ
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e545f8d49f6b852c050e84f2123cbf08d2b6757d
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947357"
---
# <a name="get-data-about-how-well-your-customers-and-azure-subscriptions-are-doing"></a><span data-ttu-id="e8568-104">顧客と Azure サブスクリプションのパフォーマンスに関するデータを取得する</span><span class="sxs-lookup"><span data-stu-id="e8568-104">Get data about how well your customers and Azure subscriptions are doing</span></span>

<span data-ttu-id="e8568-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="e8568-105">**Applies to**</span></span>

- <span data-ttu-id="e8568-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="e8568-106">Partner Center</span></span>
- <span data-ttu-id="e8568-107">クラウド ソリューション プロバイダー プログラム パートナー</span><span class="sxs-lookup"><span data-stu-id="e8568-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="e8568-108">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="e8568-108">**Appropriate roles**</span></span>

- <span data-ttu-id="e8568-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="e8568-109">Global admin</span></span>
- <span data-ttu-id="e8568-110">ユーザー管理の管理者</span><span class="sxs-lookup"><span data-stu-id="e8568-110">User management admin</span></span>
- <span data-ttu-id="e8568-111">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="e8568-111">Admin agent</span></span>
- <span data-ttu-id="e8568-112">販売代理店</span><span class="sxs-lookup"><span data-stu-id="e8568-112">Sales agent</span></span>

<span data-ttu-id="e8568-113">データはビジネス上の意思決定を促進します。</span><span class="sxs-lookup"><span data-stu-id="e8568-113">Data drives business decisions.</span></span> <span data-ttu-id="e8568-114">**Azure 利用状況**のページのメトリックを使用して、パートナーの成功度や注意が必要な分野を把握します。</span><span class="sxs-lookup"><span data-stu-id="e8568-114">Use the metrics in the **Azure usage** page to identify your successes and areas that need more attention.</span></span> <span data-ttu-id="e8568-115">新しいビジネス目標を計画するときに、この情報を使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8568-115">Use this information as you plan new business goals.</span></span>

> [!NOTE]
> <span data-ttu-id="e8568-116">Azure usage analytics は、Cloud Solution Provider プログラムのパートナーに対してのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8568-116">Azure usage analytics is available only for partners in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="e8568-117">次のメトリックを追跡しています。</span><span class="sxs-lookup"><span data-stu-id="e8568-117">We are tracking the following metrics:</span></span>

## <a name="summary"></a><span data-ttu-id="e8568-118">まとめ</span><span class="sxs-lookup"><span data-stu-id="e8568-118">Summary</span></span>

- <span data-ttu-id="e8568-119">**Total Azure subscriptions sold** (Azure サブスクリプションの合計販売数): 指定した期間に販売されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="e8568-119">**Total Azure subscriptions sold**: Number of subscriptions sold in the specified time period</span></span>  
- <span data-ttu-id="e8568-120">**Customers with usage** (利用状況のある顧客数): 指定した期間に Azure の利用状況がある顧客の数</span><span class="sxs-lookup"><span data-stu-id="e8568-120">**Customers with usage**: Number of customers with Azure usage in the specified time period</span></span>  
- <span data-ttu-id="e8568-121">**Customers with usage** (利用状況のない顧客数): 指定した期間に Azure の利用状況がない顧客の数</span><span class="sxs-lookup"><span data-stu-id="e8568-121">**Customers without usage**: Number of customers without Azure usage in the specified time period</span></span>  

## <a name="top-5-customers-in-category"></a><span data-ttu-id="e8568-122">カテゴリ内の上位 5 件の顧客</span><span class="sxs-lookup"><span data-stu-id="e8568-122">Top 5 customers in category</span></span>

- <span data-ttu-id="e8568-123">指定したカテゴリの上位 5 件の顧客</span><span class="sxs-lookup"><span data-stu-id="e8568-123">The top 5 customers for the specified category</span></span>  

## <a name="azure-subscriptions-at-risk"></a><span data-ttu-id="e8568-124">リスクがある Azure サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e8568-124">Azure subscriptions at risk</span></span>

<span data-ttu-id="e8568-125">このセクションでは、Azure サブスクリプションに対する予測変更のリスクを示します。</span><span class="sxs-lookup"><span data-stu-id="e8568-125">This section indicates the predicted churn risk to Azure subscriptions.</span></span> <span data-ttu-id="e8568-126">この情報は、パートナーが顧客とやり取りし、チャーンを最小化するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8568-126">This information can be used by partners to engage with customers and minimize churn</span></span>

## <a name="subscriptions-without-usage"></a><span data-ttu-id="e8568-127">利用状況のないサブスクリプション</span><span class="sxs-lookup"><span data-stu-id="e8568-127">Subscriptions without usage</span></span>

- <span data-ttu-id="e8568-128">指定した期間内に Azure を使用せずに特定のサブスクリプションの一覧を表示する</span><span class="sxs-lookup"><span data-stu-id="e8568-128">List of specific subscriptions without Azure usage in the specified time period</span></span>  

## <a name="azure-subscription-churn"></a><span data-ttu-id="e8568-129">Azure サブスクリプションのチャーン</span><span class="sxs-lookup"><span data-stu-id="e8568-129">Azure subscription churn</span></span>

- <span data-ttu-id="e8568-130">**Active subscriptions** (アクティブなサブスクリプション数): 日付ごとのアクティブなサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="e8568-130">**Active subscriptions**: Count of active subscriptions by date</span></span>  
- <span data-ttu-id="e8568-131">**Deprovisioned subscriptions** (プロビジョニング解除されたサブスクリプション数): 日付ごとのプロビジョニング解除または中断されたサブスクリプションの数</span><span class="sxs-lookup"><span data-stu-id="e8568-131">**Deprovisioned subscriptions**: Count of subscriptions deprovisioned or suspended by date</span></span>  

## <a name="customer-count"></a><span data-ttu-id="e8568-132">顧客数</span><span class="sxs-lookup"><span data-stu-id="e8568-132">Customer count</span></span>

- <span data-ttu-id="e8568-133">指定した期間中に獲得した新規顧客数</span><span class="sxs-lookup"><span data-stu-id="e8568-133">New customers acquired during the specified time period</span></span>  

## <a name="azure-subscription-retention"></a><span data-ttu-id="e8568-134">Azure サブスクリプションの維持</span><span class="sxs-lookup"><span data-stu-id="e8568-134">Azure subscription retention</span></span>

- <span data-ttu-id="e8568-135">更新されたサブスクリプションの数。</span><span class="sxs-lookup"><span data-stu-id="e8568-135">The number of subscriptions that were renewed.</span></span>
