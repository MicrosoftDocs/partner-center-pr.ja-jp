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
ms.openlocfilehash: cd302a7b4839b98cdd96fda38b381d9282b00620
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112275993"
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
選択した日付範囲内での属性付き ACR US$ の増加率または減少率。 

マイクロ グラフには、選択した期間における ACR US$ の月次傾向が表示されます


> [!NOTE]
 > Azure 使用による収益 (ACR) は、エグゼクティブ レポート ビューアー ロールが割り当てられているユーザーにのみ表示されます。

:::image type="content" source="images/pci/pci-azure-usage-summary-1.png" alt-text="Azure の使用状況の概要。":::

## <a name="azure-usage-by-geography"></a>地域別の Azure の使用状況

[ **地域別の Azure** 使用状況] ビューには、Azure の消費収益 (ACR US$) の地理的分布、または選択した Azure サービス レベル/測定カテゴリの使用量時間が表示されます。 マップ上の明るい色は低い値を表し、濃い色は高い値を表します。 ズームするグリッド内の国を検索して選択できます。 

[ **国/地域の数] テーブル** には、Azure 使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップ上 **の [ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-azure-usage-by-geography-2.png" alt-text="地域別の Azure の使用状況。":::

## <a name="azure-utilization"></a>Azure の使用率

このビューには、選択した Azure サービス レベル/測定カテゴリ別の月別の Azure 消費収益または使用時間の傾向が表示されます。 

棒グラフには、月次収益/使用時間の傾向が表示されます。 線グラフは、選択した Azure サービス レベル/メーター カテゴリの前月と比較した増加傾向を示します。

:::image type="content" source="images/pci/pci-azure-usage-utilization-3.png" alt-text="Azure の使用状況。":::

## <a name="next-steps"></a>次のステップ

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

>[!NOTE] 
> このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
