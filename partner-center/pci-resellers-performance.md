---
title: Partner Center Insights リセラーのパフォーマンスダッシュボード
ms.topic: article
ms.date: 09/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Partner Center Insights の再販業者パフォーマンスダッシュボードには、CSP 間接プロバイダーのさまざまな間接リセラーのパフォーマンスの概要が示されています。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 94cf24309486628d92878e0d8d5038b45c7b85df
ms.sourcegitcommit: eef446698ed4e21afee7fe091fe9c2664767755c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/01/2020
ms.locfileid: "89280547"
---
# <a name="reseller-performance-dashboard-in-partner-center-insights"></a>パートナーセンターインサイトの再販業者パフォーマンスダッシュボード

**適切なロール**

- グローバル管理者
- 管理エージェント
- レポート ビューア
- エグゼクティブレポートビューアー

Partner Center Insights の再販業者パフォーマンスダッシュボードには、CSP 間接プロバイダーのさまざまな間接リセラーのパフォーマンスの概要が示されています。 ダッシュボードには、アクティブなリセラーのデータ、生成された収益の量、収益を促進している製品が表示されます。 間接プロバイダーは、リセラーのパフォーマンスダッシュボードで、特定の再販業者を名前で検索し、リセラーの詳細を参照することができます。

次のセクションは、販売店のパフォーマンスダッシュボードで確認できます。

- まとめ
- リセラーの地理的拡散
- 再販業者の追加/除外 
- 再販業者の収益傾向 
- 製品別の再販業者のパフォーマンス
- パートナーの場所別のアクティブなリセラー
- 収益の geo 分布の傾向
- カスタマーセグメント別の再販業者のパフォーマンス
- 再販業者の MPA 署名の状態

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、役員レポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

## <a name="summary"></a>まとめ

[概要] セクションには、CSP 間接プロバイダーに関連する主要業績評価指標 (Kpi) のスナップショットビューが表示されます。

- アクティブな再販業者: その月にアクティブなサブスクリプションを1つ以上持つ再販業者の数。

マイクログラフは、選択した日付範囲内にアクティブになっている個別の再販業者の月単位の傾向を示します。

- 再販業者: その月に少なくとも1つのサブスクリプションを販売した再販業者の数。 

マイクログラフは、選択した日付範囲に登録されている再販業者の月ごとの傾向を示します。

- 新しい再販業者: その月に間接プロバイダーとのやり取りを開始した再販業者の数。 

マイクログラフは、選択した日付範囲内の新しい再販業者の合計数の月単位の傾向を示します。

- 米ドルの請求額 (米国ドル): その月の再販業者による米ドルの収益。 

このマイクログラフは、選択した日付範囲内での収益の月単位の傾向を示しています。

- [製品ごとの売上の請求] セクションでは、請求された収益の月単位の内訳を USD で、販売済みの製品別に分割します。 

:::image type="content" source="images/pci/pci-res-perf-summary-1.png" alt-text="再販業者のパフォーマンスの概要":::

## <a name="geographical-spread-of-resellers"></a>リセラーの地理的拡散

* * [地理的に別の再販業者] ビューでは、再販業者の地理的分布が提供されます。 このウィジェットを使用すると、パートナーは、さまざまな地域別に分割された **再販業者**、 **新しい再販業者**、および **請求額 (米国ドル)** を表示できます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションをクリックすると、元のビューに戻ります。 マップにマウスポインターを移動すると、国別に請求された **収益 (USD)** が表示されます。 グリッドで [課金収益 (USD)] フィールドは並べ替え可能です。

:::image type="content" source="images/pci/pci-res-perf-resel-by-geo-1.png" alt-text="地域別の再販業者 ":::

## <a name="resellers-addchurns"></a>再販業者の追加/除外

このビューは、 **新しい再販業者**、 **頻繁リセラー**、および **既存の再販業者**の数を月単位で分割したものです。 

- 新しい再販業者: 選択した日付範囲内に間接プロバイダーに新しく登録された再販業者の数。
- 頻繁リセラー: 過去6か月間のトランザクションがない再販業者の数 (当月を除く)。
- 既存の再販業者: 過去1か月間に働いていた再販業者の数。

:::image type="content" source="images/pci/pci-res-perf-resel-add-churn-1.png" alt-text="再販業者の追加/除外":::

## <a name="resellers-revenue-trend"></a>再販業者の収益傾向 

このビューには、請求された収益 (USD) の製品ごとの月ごとの傾向が、O365、D365、EMS、Power BI および Azure で示されます。 全体のメトリックは、毎月、さまざまな製品にわたって集計されます。 パートナーは、特定の再販業者を名前で検索し、その特定の再販業者のデータを検索できます。 グリッドで [課金収益 (USD)] フィールドは並べ替え可能です。

:::image type="content" source="images/pci/pci-res-perf-resel-rev-trend-1.png" alt-text="再販業者の収益傾向":::

## <a name="reseller-performance-by-products"></a>製品別の再販業者のパフォーマンス

このビューには、請求された収益、サブスクリプションの数、さまざまな製品によるライセンスの数など、月単位の主要なメトリックが分割されています。 右側にある円グラフは、さまざまな製品によってそのメトリックが分割されていることを示しています。そのため、パートナーは販売しているさまざまな製品によって分割されたものを簡単に一目で見ていきます。

:::image type="content" source="images/pci/pci-res-perf-resel-perf-product-1.png" alt-text="製品別の再販業者のパフォーマンス":::

## <a name="active-resellers-by-partner-locations"></a>パートナーの場所別のアクティブなリセラー

このビューでは、パートナー地域別にアクティブなリセラーが分割されます。 上位5つの地域が凡例に表示され、残りは "その他" と分類されます。

:::image type="content" source="images/pci/pci-res-perf-part-loc-1.png" alt-text="パートナーの場所別のアクティブなリセラー":::

## <a name="revenue-geo-distribution-trend"></a>収益の geo 分布の傾向

このビューは、上位5つの地域によって請求された売上 (USD) の月単位の傾向を示します。  収益の残りの部分は、"その他" として分類されます。

:::image type="content" source="images/pci/pci-res-perf-rev-geo-trend-1.png" alt-text="収益の geo 分布の傾向":::

## <a name="reseller-performance-by-customer-segment"></a>カスタマーセグメント別の再販業者のパフォーマンス

このビューを使用すると、パートナーは、毎月の収益を計算し、サブスクリプションとライセンスの数をさまざまな顧客セグメント別に分割することができます。 上位5つの顧客セグメントがグラフに表示され、残りは "その他" として分類されます。

:::image type="content" source="images/pci/pci-res-perf-resel-cust-seg-1.png" alt-text="カスタマーセグメント別の再販業者のパフォーマンス":::

## <a name="reseller-mpa-signing-status"></a>再販業者の MPA 署名の状態

このビューでは、再販業者の MPA 署名の状態が、MPN 審査 status、PMC to PC Migration status などの追加のメタデータと共に提供されます。

:::image type="content" source="images/pci/pci-res-perf-mpa-stat-1.png" alt-text="再販業者の MPA 署名の状態":::

## <a name="next-steps"></a>次のステップ

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

>[!NOTE] 
> このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
