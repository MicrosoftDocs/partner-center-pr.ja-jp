---
title: Customer insights の分析を使用する
ms.topic: article
ms.date: 05/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターで analytics を使用して、ビジネスについて理解を深め、顧客が購入したライセンスをどのように使用するかについて説明します。
author: shthota77
ms.author: shthota
keywords: データ, 分析, データ分析, power bi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f69fc08712ca13a9593383c0a629382b0eb3b023
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947598"
---
# <a name="use-analytics-to-learn-more-about-customer-license-use-and-how-you-can-help-meet-their-needs"></a><span data-ttu-id="9c13a-104">分析を使用して、お客様のライセンスの使用に関する詳細と、そのニーズを満たす方法を確認してください</span><span class="sxs-lookup"><span data-stu-id="9c13a-104">Use analytics to learn more about customer license use and how you can help meet their needs</span></span>

<span data-ttu-id="9c13a-105">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="9c13a-105">**Applies to**</span></span>

- <span data-ttu-id="9c13a-106">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="9c13a-106">Partner Center</span></span>
- <span data-ttu-id="9c13a-107">MPN パートナー</span><span class="sxs-lookup"><span data-stu-id="9c13a-107">MPN partners</span></span>
- <span data-ttu-id="9c13a-108">CSP プログラムのパートナー</span><span class="sxs-lookup"><span data-stu-id="9c13a-108">Partners in the CSP program</span></span>

<span data-ttu-id="9c13a-109">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="9c13a-109">**Appropriate role**</span></span>

- <span data-ttu-id="9c13a-110">MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="9c13a-110">MPN Partner admin</span></span>

<span data-ttu-id="9c13a-111">CSP ビジネスを展開する方法の計画には、顧客が Microsoft 製品をどのように使用しているかを把握することが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-111">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="9c13a-112">パートナー センターでは、データを収集するためのいくつかのオプションを用意しており、貴社のビジネスと、貴社の顧客が購入したライセンスを使用しているかどうか、またどのように使用しているかについてデータを収集できます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-112">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="9c13a-113">CSP の直接モデルの場合は、Power BI 用パートナー センター分析アプリをインストールして使用し、追加のデータを収集できます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-113">If you are in the CSP direct model, you have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-user-analytics"></a><span data-ttu-id="9c13a-114">ユーザー分析にアクセスする</span><span class="sxs-lookup"><span data-stu-id="9c13a-114">Access to user analytics</span></span>

<span data-ttu-id="9c13a-115">パートナー センターでは、MPN パートナーの管理者だけがユーザー分析にアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-115">In Partner Center, only the MPN partner admin has access to user analytics.</span></span> <span data-ttu-id="9c13a-116">貴社にこのアクセスを必要とするユーザーがいる場合 (たとえば、請求管理者)、そのユーザーに MPN パートナー管理者ロールを割り当てることによって付与できます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-116">If someone in your company needs this access (for example, a billing admin), you can grant it by assigning that person the MPN Partner Admin role.</span></span>

>[!NOTE] 
><span data-ttu-id="9c13a-117">アクセスの許可は、MPN パートナー管理者が行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c13a-117">To grant access, you must be an MPN partner admin.</span></span>

<span data-ttu-id="9c13a-118">**パートナー センターでユーザー分析へのアクセスを許可する**</span><span class="sxs-lookup"><span data-stu-id="9c13a-118">**Grant access to user analytics in Partner Center**</span></span> 

1. <span data-ttu-id="9c13a-119">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="9c13a-119">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="9c13a-120">パートナーセンターメニューの [パートナーセンターの**ユーザー管理**] ページで、[検索] ボックスを使用して、アクセスが必要なユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="9c13a-120">From the Partner Center menu, On the Partner Center **User management** page, use the Search box to find the person who needs access.</span></span>
2.  <span data-ttu-id="9c13a-121">検索結果で、ユーザーの名前を選択して、[**ユーザーの詳細**] ページを開きます。</span><span class="sxs-lookup"><span data-stu-id="9c13a-121">In the search results, select the person's name to open the **User details** page.</span></span>
3.  <span data-ttu-id="9c13a-122">**[Roles and permissions]\(ロールとアクセス許可\)** で **[MPN partner admin]\(MPN パートナー管理者\)** を選択した後、**[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9c13a-122">Under **Roles and permissions**, select **MPN partner admin** and then select **Update**.</span></span>

 
## <a name="access-data-in-partner-center"></a><span data-ttu-id="9c13a-123">パートナー センターでのデータへのアクセス</span><span class="sxs-lookup"><span data-stu-id="9c13a-123">Access data in Partner Center</span></span>

|<span data-ttu-id="9c13a-124">**取得するデータ**</span><span class="sxs-lookup"><span data-stu-id="9c13a-124">**To get data on**</span></span>   |<span data-ttu-id="9c13a-125">**ダウンロードする対象**</span><span class="sxs-lookup"><span data-stu-id="9c13a-125">**Download this**</span></span>   |<span data-ttu-id="9c13a-126">**参照先**</span><span class="sxs-lookup"><span data-stu-id="9c13a-126">**Read this**</span></span>   | <span data-ttu-id="9c13a-127">**適用対象**</span><span class="sxs-lookup"><span data-stu-id="9c13a-127">**Applies to**</span></span>    |
|---------------------|:-----------------------|:---------------|:--------------|
|<span data-ttu-id="9c13a-128">顧客が購入したライセンスの使用状況</span><span class="sxs-lookup"><span data-stu-id="9c13a-128">How your customers are using the licenses they purchased</span></span>   |<span data-ttu-id="9c13a-129">パートナー センターから展開と使用状況データ => 製品分析</span><span class="sxs-lookup"><span data-stu-id="9c13a-129">Deployment and usage data from Partner Center => Product analytics</span></span>   |[<span data-ttu-id="9c13a-130">導入実績と満足度の向上</span><span class="sxs-lookup"><span data-stu-id="9c13a-130">Increase adoption and satisfaction</span></span>](increasing-adoption-and-satisfaction.md)|<span data-ttu-id="9c13a-131">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="9c13a-131">CSP partners</span></span>|
|<span data-ttu-id="9c13a-132">サブスクリプションに関する顧客のアクティビティ</span><span class="sxs-lookup"><span data-stu-id="9c13a-132">Customer activity regarding subscriptions</span></span>   |<span data-ttu-id="9c13a-133">アクティビティ ログ</span><span class="sxs-lookup"><span data-stu-id="9c13a-133">Activity logs</span></span>   |[<span data-ttu-id="9c13a-134">顧客のアクティビティ ログの表示</span><span class="sxs-lookup"><span data-stu-id="9c13a-134">View customer activity logs</span></span>](activity-logs.md)|<span data-ttu-id="9c13a-135">CSP パートナー</span><span class="sxs-lookup"><span data-stu-id="9c13a-135">CSP partners</span></span>   |
|<span data-ttu-id="9c13a-136">顧客数、使用状況、Azure の利用状況などの増加</span><span class="sxs-lookup"><span data-stu-id="9c13a-136">Growth of customer base, usage, Azure consumption and more</span></span>   |<span data-ttu-id="9c13a-137">Power BI 用パートナー センター アプリ</span><span class="sxs-lookup"><span data-stu-id="9c13a-137">Partner Center app for Power BI</span></span>   |[<span data-ttu-id="9c13a-138">Power BI 用パートナー センター分析アプリ (CSP の直接パートナー向け)</span><span class="sxs-lookup"><span data-stu-id="9c13a-138">Partner Center Analytics app for Power BI (direct partners in CSP)</span></span>](power-bi-app-for-direct-partners.md)|<span data-ttu-id="9c13a-139">CSP 直接パートナー</span><span class="sxs-lookup"><span data-stu-id="9c13a-139">CSP direct partners</span></span>|






