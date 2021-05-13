---
title: パートナー センターの分析情報Power BI使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客に対して販売または管理するサブスクリプションの使用状況に関して、Power BIを改善できる場所を確認します。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 9626ceda405b54ea2043814fef3d7f5c81bc35af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854589"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a><span data-ttu-id="361d5-103">Power BI Insights ダッシュボードから使用できる使用状況パートナー センターレポート</span><span class="sxs-lookup"><span data-stu-id="361d5-103">Power BI usage report available from the Partner Center Insights dashboard</span></span>

<span data-ttu-id="361d5-104">**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="361d5-104">**Appropriate roles**: Global admin | Admin agent | Report viewer | Executive report viewer</span></span>

<span data-ttu-id="361d5-105">[Power BI使用状況レポートには、顧客に対して販売または管理Power BIサブスクリプションの使用状況データが表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-105">The Power BI usage report provides usage data for the Power BI subscriptions that you sold or manage for your customers.</span></span> <span data-ttu-id="361d5-106">次のセクションは、使用状況レポートのPower BI表示できます。</span><span class="sxs-lookup"><span data-stu-id="361d5-106">You can view the following sections from the Power BI usage report.</span></span>

- <span data-ttu-id="361d5-107">まとめ</span><span class="sxs-lookup"><span data-stu-id="361d5-107">Summary</span></span>
- <span data-ttu-id="361d5-108">Power BI別の使用状況の確認</span><span class="sxs-lookup"><span data-stu-id="361d5-108">Power BI usage by geography</span></span>
- <span data-ttu-id="361d5-109">Power BI SKU 別の使用状況</span><span class="sxs-lookup"><span data-stu-id="361d5-109">Power BI usage by SKU</span></span>
- <span data-ttu-id="361d5-110">サブスクリプションのパフォーマンス</span><span class="sxs-lookup"><span data-stu-id="361d5-110">Subscriptions performance</span></span>
- <span data-ttu-id="361d5-111">Power BI使用量の分布</span><span class="sxs-lookup"><span data-stu-id="361d5-111">Power BI usage distribution</span></span>

 > [!NOTE]
 > <span data-ttu-id="361d5-112">このレポートは、Insights ダッシュボードから使用できます。</span><span class="sxs-lookup"><span data-stu-id="361d5-112">This report is available from the Insights dashboard.</span></span> <span data-ttu-id="361d5-113">このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、エグゼクティブ レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="361d5-113">To view this report, you must be assigned a specific role in Partner Center, such as Global Admin, Account Admin, Report Viewer or Executive Report Viewer.</span></span> <span data-ttu-id="361d5-114">詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。</span><span class="sxs-lookup"><span data-stu-id="361d5-114">For more information, see your company's Global Admin. Specific types of data in this report may also be available only to users with Executive Report Viewer privileges.</span></span>

## <a name="summary"></a><span data-ttu-id="361d5-115">まとめ</span><span class="sxs-lookup"><span data-stu-id="361d5-115">Summary</span></span>

<span data-ttu-id="361d5-116">概要セクションには、顧客に対して販売または管理した Power BI使用状況サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-116">The summary section presents a snapshot view of the key indicators related to Power BI usage subscriptions that you sold or manage for your customers.</span></span> 

- <span data-ttu-id="361d5-117">使用可能なシート: 選択した期間に販売されたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="361d5-117">Available seats: Total number of licenses sold during the selected time frame.</span></span>

   <span data-ttu-id="361d5-118">[マイクロ] グラフには、選択した日付範囲の使用可能なシート数の月の過去 1 か月の傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-118">The Micro chart presents a month-over-month trend of available seats count for your selected date range.</span></span>

- <span data-ttu-id="361d5-119">割り当てられたシート: 選択した期間に割り当てられたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="361d5-119">Assigned seats: Total number of licenses assigned during the selected time frame.</span></span>

   <span data-ttu-id="361d5-120">マイクロ グラフには、選択した日付範囲内の割り当て済みシート数の月別の傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-120">The Micro chart presents a month-over-month trend of the assigned seats count during your selected date range.</span></span>

- <span data-ttu-id="361d5-121">アクティブなシート: 選択した期間に使用されたライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="361d5-121">Active seats: Total number of licenses that had usage during the selected time frame.</span></span> 

   <span data-ttu-id="361d5-122">マイクロ グラフには、選択した期間における月間アクティブシートの月次傾向が表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-122">The Micro chart presents a monthly trend of monthly active seats over the selected time period.</span></span>

- <span data-ttu-id="361d5-123">アクティブな使用率%: 選択した期間の使用可能な座席数に対する割合で表されたアクティブなシートの合計数。</span><span class="sxs-lookup"><span data-stu-id="361d5-123">Active Usage %: Total number of active seats expressed as a percentage of the available seats for the selected time frame.</span></span> 

   <span data-ttu-id="361d5-124">マイクログラフは、選択した期間のアクティブな使用率の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="361d5-124">The Micro chart presents a monthly trend of active usage percentage over the selected time period.</span></span>

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Power BI 使用状況の概要":::

## <a name="power-bi-usage-by-geography"></a><span data-ttu-id="361d5-126">地理別の使用状況の Power BI</span><span class="sxs-lookup"><span data-stu-id="361d5-126">Power BI usage by geography</span></span>

<span data-ttu-id="361d5-127">**地理的な Power BI 使用量** は、顧客の国別の使用可能な座席とアクティブな座席の分布を表します。</span><span class="sxs-lookup"><span data-stu-id="361d5-127">The **Power BI usage by geography** depicts the distribution of available seats and active seats by customer country.</span></span> <span data-ttu-id="361d5-128">マップ上の薄い色は下限値を表し、濃い色は高い値を表します。</span><span class="sxs-lookup"><span data-stu-id="361d5-128">Lighter colors on the map represent lower values, while darker colors represent higher values.</span></span> <span data-ttu-id="361d5-129">グリッド内で拡大する国を検索して選択できます。</span><span class="sxs-lookup"><span data-stu-id="361d5-129">You can search and select a country in the grid to zoom to.</span></span>

<span data-ttu-id="361d5-130">[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。</span><span class="sxs-lookup"><span data-stu-id="361d5-130">The **Number of countries/region** table presents the total countries/regions where Azure usage events are generated.</span></span>

<span data-ttu-id="361d5-131">グリッドで国を検索して選択すると、マップ内の場所にズームできます。</span><span class="sxs-lookup"><span data-stu-id="361d5-131">You can search and select a country in the grid to zoom to the location in the map.</span></span> <span data-ttu-id="361d5-132">マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。</span><span class="sxs-lookup"><span data-stu-id="361d5-132">Select the **Home** option on the map to revert to the original view.</span></span>

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="地理別の使用状況の Power BI":::

## <a name="power-bi-usage-by-sku"></a><span data-ttu-id="361d5-134">SKU 別の使用状況の Power BI</span><span class="sxs-lookup"><span data-stu-id="361d5-134">Power BI usage by SKU</span></span>

<span data-ttu-id="361d5-135">SKU 別の Power BI 使用量は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="361d5-135">The Power BI usage by SKU depicts monthly trend of available seats, active seats, and assigned seats by SKUs.</span></span>

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="SKU 別の使用状況の Power BI":::

## <a name="subscriptions-performance"></a><span data-ttu-id="361d5-137">サブスクリプションのパフォーマンス</span><span class="sxs-lookup"><span data-stu-id="361d5-137">Subscriptions performance</span></span>

<span data-ttu-id="361d5-138">サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の月ごとの傾向を示します。</span><span class="sxs-lookup"><span data-stu-id="361d5-138">The Subscriptions performance depicts monthly trend of active usage per customer subscription.</span></span> <span data-ttu-id="361d5-139">収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードしてすべてのサブスクリプションの詳細を表示できます。</span><span class="sxs-lookup"><span data-stu-id="361d5-139">Data for the top 100 customers by billed revenue is shown in the table and you can search for any customer or download the raw data to view details for all subscriptions.</span></span>

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="Power BI サブスクリプションのパフォーマンス":::

## <a name="power-bi-usage-distribution"></a><span data-ttu-id="361d5-141">Power BI 使用量の分布</span><span class="sxs-lookup"><span data-stu-id="361d5-141">Power BI usage distribution</span></span>

<span data-ttu-id="361d5-142">Power BI 使用分布は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の内訳を示します。</span><span class="sxs-lookup"><span data-stu-id="361d5-142">The Power BI usage distribution depicts the breakdown of available seats, active seats, and assigned seats by SKUs.</span></span>

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BI 使用量の分布":::

## <a name="next-steps"></a><span data-ttu-id="361d5-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="361d5-144">Next steps</span></span>

- <span data-ttu-id="361d5-145">その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。</span><span class="sxs-lookup"><span data-stu-id="361d5-145">For more reports, see [Partner Center Insights](partner-center-insights.md).</span></span>

- <span data-ttu-id="361d5-146">このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="361d5-146">You can download the raw data powering this report from the Download Reports section in the Insights dashboard.</span></span> [<span data-ttu-id="361d5-147">詳細情報</span><span class="sxs-lookup"><span data-stu-id="361d5-147">Learn More</span></span>](pci-download-reports.md) 
