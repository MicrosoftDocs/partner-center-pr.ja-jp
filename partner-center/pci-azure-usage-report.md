---
title: パートナー センター Insights Azure 使用状況レポート
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 何をうまく行い、顧客のために販売または管理する Azure サブスクリプションの使用を改善できる場所を確認します。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0d9224e9d86c540cc463538acc435f682cdc2d58
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146852"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナー センター Insights ダッシュボードから使用できる Azure 使用状況レポート

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

Azure 使用状況レポートには、顧客の Azure サブスクリプションに関連するメトリックが表示されます。 このレポートには、測定カテゴリ別の Azure の消費収益と使用量が含まれます。 次のセクションは、Azure の使用状況レポートから確認できます。

- まとめ
- 地域別の Azure の使用状況
- Azure の使用率

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、エグゼクティブ レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客が販売または管理する Azure サブスクリプションに関連する主要業績評価指標 (KPI) のスナップショット ビューが表示されます。  

- Azure サブスクリプション: お客様が販売または管理している Azure 顧客サブスクリプションの現在の数。
選択した日付範囲内におけるこれらの Azure サブスクリプションの増加率または減少率。

[マイクロ] グラフには、選択した日付範囲の Azure サブスクリプション数の月別の傾向が表示されます。
- アクティブな Azure サブスクリプション: 過去 30 日間にアクティブな使用量を使用していたユーザーが販売または管理した Azure サブスクリプションの現在の数。
選択した日付範囲内でのこれらのサブスクリプションの増加率または減少率。

[マイクロ] グラフには、選択した日付範囲内の Azure のアクティブなサブスクリプション数の月別の傾向が表示されます。

- Azure 使用による収益 (ACR): 選択したAzure 使用による収益に対してユーザーに属性付けされた合計値 (US$) です。
選択した日付範囲内の属性付き ACR US $ の増加率または拒否比率。 

マイクログラフは、選択した期間における ACR US $ の月ごとの傾向を示します。


> [!NOTE]
 > Azure で使用された収益 (ACR) は、Executive レポートビューアーロールが割り当てられているユーザーのみに表示されます。

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Azure の使用状況の概要":::

## <a name="azure-usage-by-geography"></a>地理的に別の Azure の使用状況

[ **Azure usage by geography] ビューで** は、azure 従量課金 (ACR US $) の地理的分布、またはすべての azure サービスレベル/メーターカテゴリの使用時間が表示されます。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内で拡大する国を検索して選択することができます。 

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="地理的に別の Azure の使用状況":::

## <a name="azure-utilization"></a>Azure の使用率

このビューには、選択した Azure サービスレベル/メーターカテゴリごとの月単位の Azure 従量課金または使用時間の傾向が表示されます。 

横棒グラフには、毎月の収益/使用時間の傾向が表示されます。 折れ線グラフでは、選択した Azure サービスレベル/メーターカテゴリの前月と比較した場合の成長傾向が示されます。

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Azure の使用率":::

## <a name="next-steps"></a>次のステップ

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

>[!NOTE] 
> このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
