---
title: サブスクリプションの分析情報を使用する
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターで analytics を使用して、ビジネスについて理解を深め、顧客が購入したライセンスをどのように使用するかについて説明します。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1693545449abf33bc7a4f5216b7d6ef0d5713829
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276860"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a><span data-ttu-id="44dd3-103">分析を使用してサブスクリプション収益の詳細を確認する</span><span class="sxs-lookup"><span data-stu-id="44dd3-103">Use analytics to learn more about subscription revenue</span></span>

<span data-ttu-id="44dd3-104">**適切なロール**: 全体管理者 |MPN パートナー管理者</span><span class="sxs-lookup"><span data-stu-id="44dd3-104">**Appropriate roles**: Global admin | MPN partner admin</span></span>

<span data-ttu-id="44dd3-105">CSP ビジネスを展開する方法の計画には、顧客が Microsoft 製品をどのように使用しているかを把握することが含まれます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-105">Planning ways to develop your CSP business includes understanding how your customers use their Microsoft products.</span></span> <span data-ttu-id="44dd3-106">パートナー センターでは、データを収集するためのいくつかのオプションを用意しており、貴社のビジネスと、貴社の顧客が購入したライセンスを使用しているかどうか、またどのように使用しているかについてデータを収集できます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-106">You have several options for gathering data in Partner Center, and you can gather data on both your business and on if and how your customers are using the licenses they've purchased.</span></span> <span data-ttu-id="44dd3-107">CSP direct モデルを使用している場合は、Power BI 用のパートナーセンター分析アプリをインストールして使用し、追加のデータを収集することもできます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-107">If you are in the CSP direct model, you also have the opportunity to install and use the Partner Center Analytics app for Power BI to gather additional data.</span></span>

## <a name="access-to-the-subscription-analytics"></a><span data-ttu-id="44dd3-108">サブスクリプション分析へのアクセス</span><span class="sxs-lookup"><span data-stu-id="44dd3-108">Access to the Subscription Analytics</span></span>

1. <span data-ttu-id="44dd3-109">パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="44dd3-109">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>
1. <span data-ttu-id="44dd3-110">[パートナーセンター] メニューの [CSP] で、[ **分析**] を選択し、[ **サブスクリプション分析**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="44dd3-110">From CSP in the Partner Center menu, select **Analyze**, and then select **Subscription analytics**.</span></span>

1. <span data-ttu-id="44dd3-111">最後の12か月の CSP 収益がページの上部に表示されます</span><span class="sxs-lookup"><span data-stu-id="44dd3-111">The trailing twelve-month CSP revenue will be displayed at the top of the page</span></span>

:::image type="content" source="images/analytics/subscription1.png" alt-text="サブスクリプション画面。":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a><span data-ttu-id="44dd3-113">末尾の Twelve-Month (TTM) CSP 収益</span><span class="sxs-lookup"><span data-stu-id="44dd3-113">Trailing Twelve-Month (TTM) CSP Revenue</span></span>

<span data-ttu-id="44dd3-114">12か月の末尾の CSP 収益は、パートナーのグローバルアカウントレベルで、最後のクラウドソリューションプロバイダープログラムの収益を USD 単位で表します。</span><span class="sxs-lookup"><span data-stu-id="44dd3-114">Trailing 12-month CSP revenue represents the trailing Cloud Solution Provider program revenue in USD at a Partner Global Account level.</span></span> <span data-ttu-id="44dd3-115">データは毎月8月に更新され、前月までの12か月の売上が表示されます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-115">The data is refreshed on the eighth of every month, to display the trailing twelve-month revenue until the prior month.</span></span> <span data-ttu-id="44dd3-116">たとえば、2020年9月9日より、2019年9月から 8 2020 月8日までの間、TTM を確認できます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-116">For example, on 9 September 2020, you should be able to see the TTM for the fixed period of September 2019 to August 2020.</span></span>

<span data-ttu-id="44dd3-117">パートナーセンターに表示される収益は、12か月の固定期間に対して計算され、より短い期間に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="44dd3-117">The revenue displayed on Partner Center is calculated for a fixed time interval of 12 months, and cannot be modified to a shorter time frame.</span></span>

<span data-ttu-id="44dd3-118">取引先のアカウントレベルで収益の内訳を確認するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="44dd3-118">To see a breakdown of the revenue at your Partner Location Account level:</span></span>

- <span data-ttu-id="44dd3-119">[ダウンロードの詳細] リンクを選択して、すべての場所で TTM の売上を表示する tsv ファイルをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="44dd3-119">Select the ‘Download Details’ link and download a .tsv file that displays the TTM revenue across all your locations.</span></span>

>[!NOTE] 
><span data-ttu-id="44dd3-120">Tsv ファイルの MPN Id 全体にわたる個々の TTM 収益数を合計した値が、パートナーセンターに表示される TTM 全体の売上を超えているように見える場合があります。</span><span class="sxs-lookup"><span data-stu-id="44dd3-120">Summing up the individual TTM Revenue numbers across MPN IDs in the .tsv file may appear to be greater than the overall TTM revenue you see displayed on Partner Center.</span></span> <span data-ttu-id="44dd3-121">これは、ダウンロードされたファイルに複数の partner 帰属があるサブスクリプションに対して、収益が二重にカウントされる可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="44dd3-121">This is because the revenue may be double counted for subscriptions with multiple partner attributions in the downloaded file.</span></span>

## <a name="subscription-summary"></a><span data-ttu-id="44dd3-122">サブスクリプションの概要</span><span class="sxs-lookup"><span data-stu-id="44dd3-122">Subscription Summary</span></span>

<span data-ttu-id="44dd3-123">画面の下半分には、サブスクリプションの概要が表示されます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-123">The lower half of the screen displays a summary of the subscriptions.</span></span> <span data-ttu-id="44dd3-124">次のフィルターを使用して、必要なサブスクリプションの詳細を表示します。</span><span class="sxs-lookup"><span data-stu-id="44dd3-124">Use the following filters to see the necessary subscription details:</span></span>  

1. <span data-ttu-id="44dd3-125">**期間**: サブスクリプションの概要を表示することを選択できます。</span><span class="sxs-lookup"><span data-stu-id="44dd3-125">**Duration**: You may opt to see the subscription summary for</span></span> 

- <span data-ttu-id="44dd3-126">30D –過去30日間</span><span class="sxs-lookup"><span data-stu-id="44dd3-126">30D – Last 30 days</span></span>
- <span data-ttu-id="44dd3-127">3M –過去3か月間</span><span class="sxs-lookup"><span data-stu-id="44dd3-127">3M – Last 3 months</span></span>
- <span data-ttu-id="44dd3-128">6分–過去6か月</span><span class="sxs-lookup"><span data-stu-id="44dd3-128">6M – Last 6 months</span></span>
- <span data-ttu-id="44dd3-129">12M –過去12か月間</span><span class="sxs-lookup"><span data-stu-id="44dd3-129">12M – Last 12 months</span></span>

2. <span data-ttu-id="44dd3-130">**製品の種類**:</span><span class="sxs-lookup"><span data-stu-id="44dd3-130">**Product Type**:</span></span>
 
- <span data-ttu-id="44dd3-131">Office 365</span><span class="sxs-lookup"><span data-stu-id="44dd3-131">Office 365</span></span>
- <span data-ttu-id="44dd3-132">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="44dd3-132">Microsoft 365</span></span>
- <span data-ttu-id="44dd3-133">Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="44dd3-133">Dynamics 365</span></span>
- <span data-ttu-id="44dd3-134">EMS</span><span class="sxs-lookup"><span data-stu-id="44dd3-134">EMS</span></span>

<span data-ttu-id="44dd3-135">これらのフィルターを適用しても、このレポートの最上部にある TTM 収益メトリックには影響しません。</span><span class="sxs-lookup"><span data-stu-id="44dd3-135">Applying these filters will not impact the TTM revenue metric at the top of this report.</span></span>


 
## <a name="next-steps"></a><span data-ttu-id="44dd3-136">次のステップ</span><span class="sxs-lookup"><span data-stu-id="44dd3-136">Next steps</span></span>

- [<span data-ttu-id="44dd3-137">購入したライセンスを顧客がどのように使用しているかを分析する</span><span class="sxs-lookup"><span data-stu-id="44dd3-137">Analyze how your customers are using the licenses they purchased</span></span>](increasing-adoption-and-satisfaction.md)  
- [<span data-ttu-id="44dd3-138">顧客のアクティビティ ログの表示</span><span class="sxs-lookup"><span data-stu-id="44dd3-138">View customer activity logs</span></span>](activity-logs.md)
- [<span data-ttu-id="44dd3-139">Power BI 用パートナー センター分析アプリ</span><span class="sxs-lookup"><span data-stu-id="44dd3-139">Partner Center Analytics app for Power BI</span></span>](power-bi-app-for-direct-partners.md)






