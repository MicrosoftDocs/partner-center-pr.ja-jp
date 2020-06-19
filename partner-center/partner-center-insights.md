---
title: パートナー センター インサイト
description: このパートナーセンターの統合レポートダッシュボードを参照してください。 売上とデプロイ、顧客開発などの Kpi での作業方法をご確認ください。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
keywords: PCI、パフォーマンス、顧客の成功、測定、レポートデータ
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 05/26/2020
ms.openlocfilehash: ecd244507b0a2ec1373bcb7954b4d5eb2d72c819
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991920"
---
# <a name="partner-center-insights---a-dashboard-that-shows-how-a-microsoft-commercial-partner-is-doing"></a><span data-ttu-id="5e0a7-105">パートナーセンターの洞察-Microsoft の商用パートナーがどのように実行しているかを示すダッシュボード</span><span class="sxs-lookup"><span data-stu-id="5e0a7-105">Partner Center Insights - a dashboard that shows how a Microsoft commercial partner is doing</span></span>

<span data-ttu-id="5e0a7-106">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="5e0a7-106">**Appropriate roles**</span></span>
- <span data-ttu-id="5e0a7-107">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="5e0a7-107">Global admin</span></span>
- <span data-ttu-id="5e0a7-108">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="5e0a7-108">Account admin</span></span>
- <span data-ttu-id="5e0a7-109">エグゼクティブ レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="5e0a7-109">Executive report viewer</span></span>
- <span data-ttu-id="5e0a7-110">レポート ビューアー</span><span class="sxs-lookup"><span data-stu-id="5e0a7-110">Report viewer</span></span>

## <a name="introduction"></a><span data-ttu-id="5e0a7-111">はじめに</span><span class="sxs-lookup"><span data-stu-id="5e0a7-111">Introduction</span></span>

<span data-ttu-id="5e0a7-112">Insights は、Microsoft Partner Network (MPN) プログラムに登録されている Microsoft のコマーシャルパートナー向けのパートナーセンターの統合されたレポートダッシュボードです。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-112">Insights is a unified reporting dashboard in Partner Center for Microsoft’s Commercial partners who are enrolled in the Microsoft Partner Network (MPN) program.</span></span> <span data-ttu-id="5e0a7-113">Insights ダッシュボードでは、Office、Azure、Dynamics などのクラウド製品や、CSP や EA などのライセンスモデルにわたる、主要業績評価指標 (KPI) の360度のビューが提供されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-113">The Insights dashboard provides 360-degree view of your key performance indicators (KPI) across Cloud products such as Office, Azure, Dynamics, and licensing models such as CSP and EA.</span></span> <span data-ttu-id="5e0a7-114">組織のデータに基づく意思決定に役立つ、豊富な KPI レポートのセットが公開されています。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-114">It exposes a rich set of KPI reports that can help you make data driven decisions for your organization.</span></span> 

## <a name="role-based-access-control-to-the-insights-dashboard"></a><span data-ttu-id="5e0a7-115">Insights ダッシュボードへのロールベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="5e0a7-115">Role-based access control to the Insights dashboard</span></span>

<span data-ttu-id="5e0a7-116">パートナーセンターには、**レポートビューアー**と**エグゼクティブレポートビューアー**の2つの新しいロールが用意されています。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-116">There are two new roles in Partner Center designed specifically for access to Insights: **Report Viewer** and **Executive Report Viewer**.</span></span> <span data-ttu-id="5e0a7-117">Executive レポートビューアーロールのユーザーは、すべてのレポートデータセットにアクセスできますが、レポートビューアーロールのユーザーは、収益や従業員の個人データなどの機微なデータセットにアクセスすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-117">Users in the Executive Report Viewer role have access to all reporting data sets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span> 

<span data-ttu-id="5e0a7-118">全体管理者またはアカウント管理者は、ユーザーにこれらのロールを割り当てることができ、会社全体または特定の MPN の場所に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-118">The Global admin or the Account admin can assign users these roles and are assigned either for the entire company or for a specific MPN location.</span></span>  

>[!Note] 
><span data-ttu-id="5e0a7-119">2020年1月20日の MPN に管理されていたユーザーは、会社全体のレポートビューアーの役割に自動的に追加されました。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-119">Users who were MPN admins as of Jan 20th, 2020 were automatically added to the company-wide report viewer role.</span></span> <span data-ttu-id="5e0a7-120">これらのユーザーは、グローバル管理者またはアカウント管理者による明示的な操作を必要とせずに、レポートビューアーとしてレポートにアクセスできます。グローバル管理者またはアカウント管理者は、必要に応じてこれらの割り当てを上書きできます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-120">They are able to access the reports as a report viewer without any explicit action required by Global admin or Account admin. The Global admins or account admin can override these assignments if necessary.</span></span> 

## <a name="reports-available"></a><span data-ttu-id="5e0a7-121">使用可能なレポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-121">Reports available</span></span>

<span data-ttu-id="5e0a7-122">次のレポートは、Insights ダッシュボードの一部として利用できます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-122">The following reports are available as part of the Insights dashboard.</span></span>

<span data-ttu-id="5e0a7-123">**概要**: 概要レポートには、顧客数、アクティブなサブスクリプション数、Azure 従量課金、アクティブなライセンスなど、関心のあるさまざまな kpi のスナップショットビューが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-123">**Overview**: The Overview report presents a snapshot view of various KPIs of interest to you such as Customer count, Active Subscriptions count, Azure Consumption Revenue, Active licenses etc.</span></span>

<span data-ttu-id="5e0a7-124">**顧客**: 顧客レポートには、顧客の取得データ、アクティブな顧客など、顧客に関する分析が示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-124">**Customer**: The Customer report presents analytics around your customers such as Customer acquisition data, Active customers, etc.</span></span>

<span data-ttu-id="5e0a7-125">**製品-サブスクリプション**: サブスクリプションレポートには、クラウドサブスクリプション (O365、Azure、Dynamics など) の取得と使用状況の分析が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-125">**Product - Subscriptions**: The Subscriptions report presents acquisition and usage analytics for your Cloud subscriptions (such as O365, Azure, Dynamics etc.)</span></span>

<span data-ttu-id="5e0a7-126">**製品ライセンス**: ライセンスダッシュボードには、O365、Dynamics、Power BI などのライセンスベースのクラウド製品のライセンス分析が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-126">**Product- Licenses**: The Licenses dashboard presents license analytics for license-based Cloud products such as O365, Dynamics, Power BI etc.</span></span>

<span data-ttu-id="5e0a7-127">**製品-azure の使用状況**: Azure の使用状況レポートには、顧客の azure サブスクリプションに関連するメトリックが表示されます。これには、Azure の使用量の売上やメーターカテゴリ別の使用量が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-127">**Product - Azure usage**: The Azure Usage report presents metrics related to your customers’ Azure subscriptions including Azure consumption revenue and usage by meter categories.</span></span>

<span data-ttu-id="5e0a7-128">**コンピテンシー**: コンピテンシーレポートには、アクティブ、修飾、およびリスクのあるコンピテンシーのメトリックが表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-128">**Competencies**: The Competencies report presents metrics on your Active, Qualified, and At-risk competencies.</span></span>

<span data-ttu-id="5e0a7-129">**特典**: 特典レポートには、獲得したパートナー特典と使用したパートナー特典の分析が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-129">**Benefits**: The Benefits report presents analytics on partner benefits you have earned vs consumed.</span></span>

## <a name="navigating-the-insights-reports"></a><span data-ttu-id="5e0a7-130">Insights レポート内の移動</span><span class="sxs-lookup"><span data-stu-id="5e0a7-130">Navigating the Insights reports</span></span>

<span data-ttu-id="5e0a7-131">**日付範囲フィルター**: 各ページの右上隅にある日付範囲の選択を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-131">**Date range filters**: You can find a date range selection at the top-right corner of each page.</span></span> <span data-ttu-id="5e0a7-132">[概要] ページのグラフの出力をカスタマイズするには、過去3、6、または12か月に基づいて日付範囲を選択するか、カスタムの日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-132">The output of the overview page graphs can be customized by selecting a date range based on the past 3, 6, or 12 months, or by selecting a custom date range.</span></span> <span data-ttu-id="5e0a7-133">既定の日付範囲の選択は12か月です。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-133">The default date range selection is 12 months.</span></span> 

:::image type="content" source="images/pci/intro1.png" alt-text="概要マップ":::

<span data-ttu-id="5e0a7-135">**フィードバックボタン**: すべてのインサイトレポートの各グラフ/コントロールには、レポート機能に関するインスタンスフィードバックを提供するためのフィードバックボタンが組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-135">**Feedback button**: Each chart/control in all the Insights reports is incorporated with a feedback button to let you provide instance feedback on a report feature.</span></span> 

 
<span data-ttu-id="5e0a7-136">**ページレベルフィルター**: 概要、利点、コンピテンシーレポートを除き、すべての分析情報レポートでページレベルのフィルターを適用できます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-136">**Page level filters**: Except for the Overview, Benefits, and Competencies reports, all Insights reports enable you to apply page level filters.</span></span> 

- <span data-ttu-id="5e0a7-137">選択したフィルターは、[概要] セクションを含む、ページ上のすべてのグラフとメトリックに適用されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-137">The filters selected will be applicable for all charts and metrics on a page, including the summary section.</span></span> <span data-ttu-id="5e0a7-138">フィルター項目は、そのフィルター条件内にデータがある場合に使用できます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-138">A filter item will be available if you have any data within that filter criteria.</span></span> 

- <span data-ttu-id="5e0a7-139">各フィルター一覧の既定の選択は**all**です。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-139">Default selection of each filter list is **all**.</span></span> <span data-ttu-id="5e0a7-140">たとえば、製品フィルターで特定の製品を選択していない場合、既定の選択は [すべての製品] になります。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-140">For example, if you have not selected a specific product in products filter, default selection will be all products.</span></span>

- <span data-ttu-id="5e0a7-141">選択したフィルターは、ページの上部に表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-141">Filters selected will be displayed at the top of the page.</span></span> 

:::image type="content" source="images/pci/filters.png" alt-text="仕分け":::

### <a name="filters-definitions"></a><span data-ttu-id="5e0a7-143">フィルターの定義:</span><span class="sxs-lookup"><span data-stu-id="5e0a7-143">Filters definitions:</span></span>

- <span data-ttu-id="5e0a7-144">Products: 組織で販売または管理されているすべての Microsoft Cloud 製品 (O365、Azure、D365、EMS、PowerBI など) の一覧。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-144">Products: List of all Microsoft Cloud products sold/managed by your organization, for example,  O365, Azure, D365, EMS, PowerBI etc.</span></span>
- <span data-ttu-id="5e0a7-145">顧客市場: 顧客の国の一覧</span><span class="sxs-lookup"><span data-stu-id="5e0a7-145">Customer markets: List of customer countries</span></span>
- <span data-ttu-id="5e0a7-146">Partner 帰属: 顧客サブスクリプションとの関連付けの種類。たとえば、デジタルパートナーのレコード (購入者または)、委任された管理者特権 (DAP)、パートナー管理リンク (PAL) などがあります。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-146">Partner attributions: Your association type with your customers subscriptions, for example,  Digital partner of record (DPOR), Delegated admin privilege (DAP), Partner Admin link (PAL) etc.</span></span> 
- <span data-ttu-id="5e0a7-147">パートナーの場所: 組織のすべての MPN の場所の一覧。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-147">Partner locations: List of all your organization’s MPN locations.</span></span>
- <span data-ttu-id="5e0a7-148">販売チャネル: 製品とサービスの購入/プロビジョニングを行うすべての販売チャネル/価格。 CSP、EA、CSP 間接、直接、アドバイザー、オープン、その他</span><span class="sxs-lookup"><span data-stu-id="5e0a7-148">Sales channels: All sales channel/pricing through which you are purchasing/provisioning products and services namely CSP, EA, CSP indirect, Direct, Advisor, Open, others</span></span>
- <span data-ttu-id="5e0a7-149">顧客セグメント: パートナーの顧客ベース全体にわたる顧客セグメントの一覧。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-149">Customer segments: List of customer segments across the partners customer base.</span></span>

## <a name="read-about-each-of-the-dashboards-and-reports"></a><span data-ttu-id="5e0a7-150">各ダッシュボードとレポートについて確認します。</span><span class="sxs-lookup"><span data-stu-id="5e0a7-150">Read about each of the dashboards and reports:</span></span>

- [<span data-ttu-id="5e0a7-151">パートナーセンターの洞察-概要ダッシュボード</span><span class="sxs-lookup"><span data-stu-id="5e0a7-151">Partner Center Insights - Overview dashboard</span></span>](pci-overview-report.md)

- [<span data-ttu-id="5e0a7-152">パートナー センター インサイト - 顧客ダッシュボード</span><span class="sxs-lookup"><span data-stu-id="5e0a7-152">Partner Center Insights - Customer dashboard</span></span>](pci-customer-report.md)

- [<span data-ttu-id="5e0a7-153">パートナーセンターの洞察-サブスクリプションレポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-153">Partner Center Insights - Subscriptions report</span></span>](pci-product-subscriptions-report.md)

- [<span data-ttu-id="5e0a7-154">パートナーセンターの洞察-ライセンスレポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-154">Partner Center Insights - Licenses report</span></span>](pci-product-licenses-report.md)

- [<span data-ttu-id="5e0a7-155">パートナーセンターの洞察-Azure の使用状況レポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-155">Partner Center Insights - Azure usage report</span></span>](pci-azure-usage-report.md)

- [<span data-ttu-id="5e0a7-156">パートナー センター インサイト - コンピテンシー レポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-156">Partner Center Insights - Competencies report</span></span>](pci-competencies-report.md)

- [<span data-ttu-id="5e0a7-157">パートナー センター インサイト -特典レポート</span><span class="sxs-lookup"><span data-stu-id="5e0a7-157">Partner Center Insights - Benefits report</span></span>](pci-benefits-report.md)
