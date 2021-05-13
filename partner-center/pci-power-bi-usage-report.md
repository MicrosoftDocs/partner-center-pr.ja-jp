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

- アクティブな使用率%: 選択した期間の使用可能な座席数に対する割合で表されたアクティブなシートの合計数。 

   マイクログラフは、選択した期間のアクティブな使用率の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="Power BI 使用状況の概要":::

## <a name="power-bi-usage-by-geography"></a>地理別の使用状況の Power BI

**地理的な Power BI 使用量** は、顧客の国別の使用可能な座席とアクティブな座席の分布を表します。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内で拡大する国を検索して選択できます。

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="地理別の使用状況の Power BI":::

## <a name="power-bi-usage-by-sku"></a>SKU 別の使用状況の Power BI

SKU 別の Power BI 使用量は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="SKU 別の使用状況の Power BI":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の月ごとの傾向を示します。 収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードしてすべてのサブスクリプションの詳細を表示できます。

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="Power BI サブスクリプションのパフォーマンス":::

## <a name="power-bi-usage-distribution"></a>Power BI 使用量の分布

Power BI 使用分布は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の内訳を示します。

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="Power BI 使用量の分布":::

## <a name="next-steps"></a>次の手順

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

- このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
