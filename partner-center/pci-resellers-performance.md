---
title: パートナー センター Insights Resellers のパフォーマンス ダッシュボード
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー センター Insights のリセラー パフォーマンス ダッシュボードには、クラウド ソリューション プロバイダー (CSP) 間接プロバイダーのさまざまな間接リセラーのパフォーマンスの概要が表示されます。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 65fddcc47105cf329bb8f5d3e1aa342deee556b4
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565170"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>パートナー センター Insights の Reseller Performance ダッシュボード

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

パートナー センター Insights のリセラー パフォーマンス ダッシュボードには、クラウド ソリューション プロバイダー (CSP) 間接プロバイダーのさまざまな間接リセラーのパフォーマンスの概要が表示されます。 ダッシュボードには、アクティブなリセラー、生成される収益、収益を推進している製品に関するデータが表示されます。 間接プロバイダーは、特定のリセラーを名前で検索し、リセラーのパフォーマンス ダッシュボードでリセラーの詳細を検索できます。

次のセクションは、リセラーのパフォーマンス ダッシュボードから確認できます。

- まとめ
- リセラーの地理的分散
- リセラーの追加/チャーン 
- リセラーの収益傾向 
- 製品別のリセラーのパフォーマンス
- パートナーの場所別のアクティブなリセラー
- 収益地域分布の傾向
- 顧客セグメント別のリセラーのパフォーマンス
- Reseller Microsoft Partner Agreement (MPA) の署名状態

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、役員レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、概要に関連する主要業績評価指標 (KPI) のスナップショット ビュー CSP Indirect Provider。

- アクティブなリセラー: その月に少なくとも 1 つのアクティブなサブスクリプションを持つリセラーの数。

[マイクロ] グラフには、選択した日付範囲内にアクティブだった個別のリセラーの月別の月別の傾向が表示されます。

- 取引リセラー: その月に少なくとも 1 つのサブスクリプションを販売したリセラーの数。 

[マイクロ] グラフには、選択した日付範囲に登録されているリセラーの月別の傾向が表示されます。

- 新しいリセラー: その月に間接プロバイダーとの取引を開始したリセラーの数。 

[マイクロ] グラフには、選択した日付範囲内の新しいリセラーの総数の月累計傾向が表示されます。

- 請求収益 USD: その月のリセラーによって駆動される USD の収益。 

マイクロ グラフは、選択した日付範囲内の月別収益の傾向を示します。

- [Billed revenue by products]/(製品別の請求収益)" セクションでは、請求収益の月の内訳 (USD) が販売された製品別に 1 か月分表示されます。 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="リセラーのパフォーマンスの概要。":::

## <a name="geographical-spread-of-resellers"></a>リセラーの地理的分散

**[地域別のリセラー] ビューでは、リセラーの地理的な分布が提供されます。 このウィジェットを使用すると、パートナーは、リセラー、**新** しいリセラー、および請求収益 **(USD)** の合計をさまざまな地域で分割して表示できます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの **[ホーム** ] オプションを押して、元のビューに戻ります。 マップにマウス ポインターを合わせると、国別 **の請求収益 (USD)** が表示されます。 グリッドの [請求収益 (USD) ] フィールドは並べ替え可能です。

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="地域別のリセラー。":::

## <a name="resellers-addchurns"></a>リセラーの追加/チャーン

このビューでは、新しいリセラー、チャーンドリセラー、および既存のリセラーの数の月 **分割が提供されます**。 

- 新しいリセラー: 選択した日付範囲内に間接プロバイダーに新しく登録されたリセラーの数。
- チャーンリセラー: 当月を除く過去 6 か月間取引を行ってなかったリセラーの数。
- 既存のリセラー: 前月に取引を行ったリセラーの数。

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="リセラーは、チャーンを追加します。":::

## <a name="resellers-revenue-trend"></a>リセラーの収益傾向 

このビューでは、請求収益 (USD) の月次傾向を製品 (Office 365、Dynamics 365、Enterprise Mobility and Security (EMS)、Microsoft Power BI、Azure) で分割します。 全体的なメトリックは、各月のさまざまな製品にわたって集計されます。 パートナーは、名前で特定のリセラーを検索し、その特定のリセラーのデータを検索できます。 グリッドの [請求収益 (USD) ] フィールドは並べ替え可能です。

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="リセラーの収益傾向。":::

## <a name="reseller-performance-by-products"></a>製品別のリセラーのパフォーマンス

このビューでは、月単位で、請求収益、サブスクリプションの数、さまざまな製品別のライセンス数など、主要なメトリックの分割が提供されます。 右側の円グラフは、さまざまな製品によるメトリックの全体的な分割を示しています。そのため、パートナーは、リセラーが販売しているさまざまな製品による分割を簡単に確認できます。

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="製品別のリセラーのパフォーマンス。":::

## <a name="active-resellers-by-partner-locations"></a>パートナーの場所別のアクティブなリセラー

このビューでは、パートナーの地域別にアクティブなリセラーを分割できます。 上位 5 つの地域が凡例に表示され、残りの地域は "その他" に分類されます。

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="パートナーの場所別のアクティブなリセラー。":::

## <a name="revenue-geo-distribution-trend"></a>収益地域分布の傾向

このビューは、上位 5 つの地域で分割された請求収益 (USD) の月の傾向を示します。  残りの収益は "その他" に分類されます。

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="収益地域分布の傾向。":::

## <a name="reseller-performance-by-customer-segment"></a>顧客セグメント別のリセラーのパフォーマンス

このビューを使用すると、パートナーは、収益の毎月の傾向 (USD)、サブスクリプションとライセンスの数を、さまざまな顧客セグメントで分割して把握できます。 上位 5 つの顧客セグメントがグラフに表示され、残りのセグメントは "その他" に分類されます。

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="顧客セグメント別のリセラーのパフォーマンス。":::

## <a name="reseller-mpa-signing-status"></a>リセラー MPA 署名の状態

このビューには、リセラーの MPA 署名状態と、Microsoft Partner Network (MPN) の確認状態、Partner Membership Center (PMC) から パートナー センター への移行状態などの追加のメタデータが表示されます。

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="リセラー MPA 署名状態。":::

## <a name="next-steps"></a>次の手順

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

>[!NOTE] 
> このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
