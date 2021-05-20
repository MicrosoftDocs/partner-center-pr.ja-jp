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
# <a name="dynamics-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナー センター Insights ダッシュボードから使用できる Dynamics 使用状況レポート

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

Dynamics 使用状況レポートには、顧客に対して販売または管理した Dynamics 365 サブスクリプションの使用状況データが表示されます。 次のセクションは、Dynamics 使用状況レポートから確認できます。

- まとめ
- 地域別の Dynamics の使用
- SKU 別の Dynamics の使用状況
- サブスクリプションのパフォーマンス
- Dynamics の使用状況の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、エグゼクティブ レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客に対して販売または管理した Dynamics の使用状況サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。  

- 使用可能なシート: 選択した期間に販売されたライセンスの総数。

   [マイクロ] グラフには、選択した日付範囲の使用可能なシート数の月の過去 1 か月の傾向が表示されます。

- 割り当てられたシート: 選択した期間に割り当てられたライセンスの総数。

   マイクロ グラフには、選択した日付範囲内の割り当て済みシート数の月別の傾向が表示されます。

- アクティブなシート: 選択した期間に使用されたライセンスの総数。 

   マイクロ グラフには、選択した期間における月間アクティブシートの月次傾向が表示されます。

- アクティブな使用率%: 選択した期間の使用可能な座席数に対する割合で表されたアクティブなシートの合計数。 

   マイクログラフは、選択した期間のアクティブな使用率の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-dynamics-usage-summary.png" alt-text="Dynamics の使用状況の概要":::

## <a name="dynamics-usage-by-geography"></a>Geography による Dynamics の使用状況

**地理的な使用量** は、顧客の国別の座席とアクティブな座席の分布を表します。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内の国を検索して選択できます。 拡大して表示することもできます。

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-dynamics-usage-geography.png" alt-text="Geography による Dynamics の使用状況":::

## <a name="dynamics-usage-by-sku"></a>SKU による Dynamics の使用状況

Dynamics usage by SKU は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-dynamics-usage-sku.png" alt-text="SKU による Dynamics の使用状況":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の月ごとの傾向を示します。 収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードしてすべてのサブスクリプションの詳細を表示できます。

:::image type="content" source="images/pci/pci-dynamics-usage-subscription.png" alt-text="Dynamics サブスクリプションのパフォーマンス":::

## <a name="dynamics-usage-distribution"></a>Dynamics usage 分布

Dynamics usage 分布は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の内訳を示します。

:::image type="content" source="images/pci/pci-dynamics-usage-distribution.png" alt-text="Dynamics の使用状況の分布":::

## <a name="next-steps"></a>次のステップ

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

- このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
