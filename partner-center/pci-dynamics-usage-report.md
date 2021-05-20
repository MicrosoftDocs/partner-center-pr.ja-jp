---
title: パートナー センターの分析情報の Dynamics 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客に対して販売または管理する Dynamics サブスクリプションの使用状況に関して、何がうまく機能し、どこで改善できるのかを確認します。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 0e2880f8548b220d708c61c08a0ea9fb37700240
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152802"
---
# <a name="dynamics-usage-report-available-from-the-partner-center-insights-dashboard"></a><span data-ttu-id="80c05-103">パートナー センター Insights ダッシュボードから使用できる Dynamics 使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="80c05-103">Dynamics usage report available from the Partner Center Insights dashboard</span></span>

<span data-ttu-id="80c05-104">**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="80c05-104">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="80c05-105">Dynamics 使用状況レポートには、顧客に対して販売または管理した Dynamics 365 サブスクリプションの使用状況データが表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-105">The Dynamics usage report provides usage data for the Dynamics 365 subscriptions that you sold or manage for your customers.</span></span> <span data-ttu-id="80c05-106">次のセクションは、Dynamics 使用状況レポートから確認できます。</span><span class="sxs-lookup"><span data-stu-id="80c05-106">You can view the following sections from the dynamics usage report.</span></span>

- <span data-ttu-id="80c05-107">まとめ</span><span class="sxs-lookup"><span data-stu-id="80c05-107">Summary</span></span>
- <span data-ttu-id="80c05-108">地域別の Dynamics の使用</span><span class="sxs-lookup"><span data-stu-id="80c05-108">Dynamics usage by geography</span></span>
- <span data-ttu-id="80c05-109">SKU 別の Dynamics の使用状況</span><span class="sxs-lookup"><span data-stu-id="80c05-109">Dynamics usage by SKU</span></span>
- <span data-ttu-id="80c05-110">サブスクリプションのパフォーマンス</span><span class="sxs-lookup"><span data-stu-id="80c05-110">Subscriptions performance</span></span>
- <span data-ttu-id="80c05-111">Dynamics の使用状況の分布</span><span class="sxs-lookup"><span data-stu-id="80c05-111">Dynamics usage distribution</span></span>

 > [!NOTE]
 > <span data-ttu-id="80c05-112">このレポートは、Insights ダッシュボードから使用できます。</span><span class="sxs-lookup"><span data-stu-id="80c05-112">This report is available from the Insights dashboard.</span></span> <span data-ttu-id="80c05-113">このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、エグゼクティブ レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="80c05-113">To view this report, you must be assigned a specific role in Partner Center, such as Global Admin, Account Admin, Report Viewer or Executive Report Viewer.</span></span> <span data-ttu-id="80c05-114">詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。</span><span class="sxs-lookup"><span data-stu-id="80c05-114">For more information, see your company's Global Admin. Specific types of data in this report may also be available only to users with Executive Report Viewer privileges.</span></span>

## <a name="summary"></a><span data-ttu-id="80c05-115">まとめ</span><span class="sxs-lookup"><span data-stu-id="80c05-115">Summary</span></span>

<span data-ttu-id="80c05-116">概要セクションには、顧客に対して販売または管理した Dynamics の使用状況サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-116">The summary section presents a snapshot view of the key indicators related to Dynamics usage subscriptions that you sold or manage for your customers.</span></span>  

- <span data-ttu-id="80c05-117">使用可能なシート: 選択した期間に販売されたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="80c05-117">Available seats: Total number of licenses sold during the selected time frame.</span></span>

   <span data-ttu-id="80c05-118">[マイクロ] グラフには、選択した日付範囲の使用可能なシート数の月の過去 1 か月の傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-118">The Micro chart presents a month-over-month trend of available seats count for your selected date range.</span></span>

- <span data-ttu-id="80c05-119">割り当てられたシート: 選択した期間に割り当てられたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="80c05-119">Assigned seats: Total number of licenses assigned during the selected time frame.</span></span>

   <span data-ttu-id="80c05-120">マイクロ グラフには、選択した日付範囲内の割り当て済みシート数の月別の傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-120">The Micro chart presents a month-over-month trend of the assigned seats count during your selected date range.</span></span>

- <span data-ttu-id="80c05-121">アクティブなシート: 選択した期間に使用されたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="80c05-121">Active seats: Total number of licenses that had usage during the selected time frame.</span></span> 

   <span data-ttu-id="80c05-122">マイクロ グラフには、選択した期間における月間アクティブシートの月次傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-122">The Micro chart presents a monthly trend of monthly active seats over the selected time period.</span></span>

- <span data-ttu-id="80c05-123">アクティブな使用率%: 選択した期間の使用可能な座席数に対する割合で表されたアクティブなシートの合計数。</span><span class="sxs-lookup"><span data-stu-id="80c05-123">Active Usage %: Total number of active seats expressed as a percentage of the available seats for the selected time frame.</span></span> 

   <span data-ttu-id="80c05-124">マイクログラフは、選択した期間のアクティブな使用率の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="80c05-124">The Micro chart presents a monthly trend of active usage percentage over the selected time period.</span></span>

:::image type="content" source="images/pci/pci-dynamics-usage-summary.png" alt-text="Dynamics の使用状況の概要":::

## <a name="dynamics-usage-by-geography"></a><span data-ttu-id="80c05-126">Geography による Dynamics の使用状況</span><span class="sxs-lookup"><span data-stu-id="80c05-126">Dynamics usage by geography</span></span>

<span data-ttu-id="80c05-127">**地理的な使用量** は、顧客の国別の座席とアクティブな座席の分布を表します。</span><span class="sxs-lookup"><span data-stu-id="80c05-127">The **Dynamics usage by geography** depicts the distribution of available seats and active seats by customer country.</span></span> <span data-ttu-id="80c05-128">マップ上の薄い色は下限値を表し、濃い色は高い値を表します。</span><span class="sxs-lookup"><span data-stu-id="80c05-128">Lighter colors on the map represent lower values, while darker colors represent higher values.</span></span> <span data-ttu-id="80c05-129">グリッド内の国を検索して選択できます。</span><span class="sxs-lookup"><span data-stu-id="80c05-129">You can search and select a country in the grid.</span></span> <span data-ttu-id="80c05-130">拡大して表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="80c05-130">You can also zoom in for a closer look.</span></span>

<span data-ttu-id="80c05-131">[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。</span><span class="sxs-lookup"><span data-stu-id="80c05-131">The **Number of countries/region** table presents the total countries/regions where Azure usage events are generated.</span></span>

<span data-ttu-id="80c05-132">グリッドで国を検索して選択すると、マップ内の場所にズームできます。</span><span class="sxs-lookup"><span data-stu-id="80c05-132">You can search and select a country in the grid to zoom to the location in the map.</span></span> <span data-ttu-id="80c05-133">マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。</span><span class="sxs-lookup"><span data-stu-id="80c05-133">Select the **Home** option on the map to revert to the original view.</span></span>

:::image type="content" source="images/pci/pci-dynamics-usage-geography.png" alt-text="Geography による Dynamics の使用状況":::

## <a name="dynamics-usage-by-sku"></a><span data-ttu-id="80c05-135">SKU による Dynamics の使用状況</span><span class="sxs-lookup"><span data-stu-id="80c05-135">Dynamics usage by SKU</span></span>

<span data-ttu-id="80c05-136">Dynamics usage by SKU は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="80c05-136">The Dynamics usage by SKU depicts monthly trend of available seats, active seats, and assigned seats by SKUs.</span></span>

:::image type="content" source="images/pci/pci-dynamics-usage-sku.png" alt-text="SKU による Dynamics の使用状況":::

## <a name="subscriptions-performance"></a><span data-ttu-id="80c05-138">サブスクリプションのパフォーマンス</span><span class="sxs-lookup"><span data-stu-id="80c05-138">Subscriptions performance</span></span>

<span data-ttu-id="80c05-139">サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="80c05-139">The Subscriptions performance depicts the monthly trend of Active Usage per customer subscription.</span></span> <span data-ttu-id="80c05-140">収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードしてすべてのサブスクリプションの詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="80c05-140">Data for the top 100 customers by billed revenue is shown in the table and you can search for any customer or download the raw data to view details for all subscriptions.</span></span>

:::image type="content" source="images/pci/pci-dynamics-usage-subscription.png" alt-text="Dynamics サブスクリプションのパフォーマンス":::

## <a name="dynamics-usage-distribution"></a><span data-ttu-id="80c05-142">Dynamics usage 分布</span><span class="sxs-lookup"><span data-stu-id="80c05-142">Dynamics usage distribution</span></span>

<span data-ttu-id="80c05-143">Dynamics usage 分布は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="80c05-143">The Dynamics usage distribution depicts the breakdown of available seats, active seats, and assigned seats by SKUs.</span></span>

:::image type="content" source="images/pci/pci-dynamics-usage-distribution.png" alt-text="Dynamics の使用状況の分布":::

## <a name="next-steps"></a><span data-ttu-id="80c05-145">次のステップ</span><span class="sxs-lookup"><span data-stu-id="80c05-145">Next steps</span></span>

- <span data-ttu-id="80c05-146">その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。</span><span class="sxs-lookup"><span data-stu-id="80c05-146">For more reports, see [Partner Center Insights](partner-center-insights.md).</span></span>

- <span data-ttu-id="80c05-147">このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="80c05-147">You can download the raw data powering this report from the Download Reports section in the Insights dashboard.</span></span> [<span data-ttu-id="80c05-148">詳細情報</span><span class="sxs-lookup"><span data-stu-id="80c05-148">Learn More</span></span>](pci-download-reports.md) 
