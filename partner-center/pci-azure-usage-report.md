---
title: パートナーセンターの Insights Azure の使用状況レポート
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様のお客様のために販売または管理している Azure サブスクリプションの使用状況について、お客様がどのように改善できるかをご確認ください。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 72676a714cf944bc9210de8e8f6edfa0d3037da9
ms.sourcegitcommit: 735593129d1a009854a4ed0b03b11035211dbb25
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2020
ms.locfileid: "88239070"
---
# <a name="azure-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナーセンターの Insights ダッシュボードから使用可能な Azure の使用状況レポート

**適切なロール**
- グローバル管理者
- 管理エージェント
- レポート ビューア
- エグゼクティブレポートビューアー

Azure の使用状況レポートには、顧客の Azure サブスクリプションに関連するメトリックが表示されます。 これには、Azure の消費収益とメーターカテゴリごとの使用量が含まれます。 Azure の使用状況レポートでは、次のセクションを確認できます。

- まとめ
- 地理的に別の Azure の使用状況
- Azure の使用率

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、エグゼクティブレポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

**まとめ**

概要セクションには、顧客に対して販売または管理されている Azure サブスクリプションに関連する主要業績評価指標 (Kpi) のスナップショットビューが表示されます。  

- Azure サブスクリプション: 選択した日付範囲における azure サブスクリプションの現在の数の増加または減少率 (%)。

マイクログラフは、選択した日付範囲について、Azure サブスクリプションの数の月ごとの傾向を示します。
- アクティブな Azure サブスクリプション: 過去30日間にアクティブに使用された Azure サブスクリプションの現在の数。
選択した日付範囲内でのこれらのサブスクリプションの増加または拒否の割合。

マイクログラフは、選択した日付範囲における Azure アクティブなサブスクリプション数の月単位の傾向を示します。

- Azure で使用された収益 (ACR): 選択した日付範囲について、Azure で消費された総収益 (US $) の値を示します。
選択した日付範囲内の属性付き ACR US $ の増加率または拒否比率。 

マイクログラフは、選択した期間における ACR US $ の月ごとの傾向を示します。


> [!NOTE]
 > Azure で使用された収益 (ACR) は、Executive レポートビューアーロールが割り当てられているユーザーのみに表示されます。

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Azure の使用状況の概要":::

**地理的に別の Azure の使用状況**

[ **Azure usage by geography] ビューで** は、azure 従量課金 (ACR US $) の地理的分布、またはすべての azure サービスレベル/メーターカテゴリの使用時間が表示されます。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内で拡大する国を検索して選択することができます。 

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="地理的に別の Azure の使用状況":::

**Azure の使用率**

このビューには、選択した Azure サービスレベル/メーターカテゴリごとの月単位の Azure 従量課金または使用時間の傾向が表示されます。 

横棒グラフには、毎月の収益/使用時間の傾向が表示されます。 折れ線グラフでは、選択した Azure サービスレベル/メーターカテゴリの前月と比較した場合の成長傾向が示されます。

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Azure の使用率":::

## <a name="next-steps"></a>次のステップ

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

>[!NOTE] 
> このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
