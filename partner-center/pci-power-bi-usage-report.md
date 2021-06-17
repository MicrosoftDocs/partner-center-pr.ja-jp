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
ms.openlocfilehash: 36993633ab2e2be0a726c70bf930f842bfaf890f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276299"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a>Power BI Insights ダッシュボードから使用できる使用状況パートナー センターレポート

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

[Power BI使用状況レポートには、顧客に対して販売または管理Power BIサブスクリプションの使用状況データが表示されます。 次のセクションは、使用状況レポートのPower BI表示できます。

- まとめ
- Power BI別の使用状況の確認
- Power BI SKU 別の使用状況
- サブスクリプションのパフォーマンス
- Power BI使用量の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、エグゼクティブ レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客に対して販売または管理した Power BI使用状況サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。 

- 使用可能なシート: 選択した期間に販売されたライセンスの総数。

   [マイクロ] グラフには、選択した日付範囲の使用可能なシート数の月の過去 1 か月の傾向が表示されます。

- 割り当てられたシート: 選択した期間に割り当てられたライセンスの総数。

   マイクロ グラフには、選択した日付範囲内の割り当て済みシート数の月別の傾向が表示されます。

- アクティブなシート: 選択した期間に使用されたライセンスの総数。 

   マイクロ グラフには、選択した期間における月間アクティブシートの月次傾向が表示されます。

- アクティブな使用率 %: 選択した時間枠で使用可能なシートに対する割合で表されるアクティブなシートの総数。 

   マイクロ グラフには、選択した期間におけるアクティブな使用率の月間傾向が表示されます。

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Power BIの概要。":::

## <a name="power-bi-usage-by-geography"></a>Power BI別の使用状況の確認

地域 **Power BI使用状況の一覧は** 、顧客の国別の利用可能なシートとアクティブなシートの分布を示しています。 マップ上の明るい色は低い値を表し、濃い色は高い値を表します。 ズームするグリッド内の国を検索して選択できます。

[ **国/地域の数] テーブル** には、Azure 使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップ上 **の [ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="Power BI別の使用状況。":::

## <a name="power-bi-usage-by-sku"></a>Power BI SKU 別の使用状況

SKU 別Power BIの使用量は、SKU 別の利用可能なシート、アクティブなシート、および割り当てられたシートの月次傾向を示しています。

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="Power BI SKU 別の使用量。":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の毎月の傾向を示しています。 請求収益別の上位 100 人の顧客のデータが表に表示されます。すべての顧客を検索したり、生データをダウンロードしてすべてのサブスクリプションの詳細を表示することができます。

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="Power BIパフォーマンスが向上します。":::

## <a name="power-bi-usage-distribution"></a>Power BI使用量の分布

[Power BIの分布は、使用可能なシート、アクティブなシート、および割り当てられたシートの SKU 別の内訳を示しています。

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BIの分布。":::

## <a name="next-steps"></a>次のステップ

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

- このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
