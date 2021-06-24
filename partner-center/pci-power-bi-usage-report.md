---
title: パートナーセンターの insights Power BI 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様のために販売または管理している Power BI サブスクリプションの使用状況について、お客様がどのように改善できるかをご確認ください。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 75aa86ebc768b9d6d252a29eb84aef97ab99ab0c
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565340"
---
# <a name="power-bi-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナーセンターの Insights ダッシュボードから使用可能な Power BI 使用状況レポート

**適切なロール**: 全体管理者 |管理エージェント |レポートビューアー |エグゼクティブレポートビューアー

Power BI 使用状況レポートには、顧客が販売または管理している Microsoft Power BI サブスクリプションの使用状況データが表示されます。 Power BI の使用状況レポートでは、次のセクションを表示できます。

- まとめ
- 地理別の使用状況の Power BI
- SKU 別の使用状況の Power BI
- サブスクリプションのパフォーマンス
- Power BI 使用量の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、エグゼクティブレポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客が販売または管理している Power BI 使用状況サブスクリプションに関連する主要指標のスナップショットビューが表示されます。 

- 使用可能なシート数: 選択した期間中に販売されたライセンスの合計数。

   マイクログラフは、選択した日付範囲について、使用可能な座席数の月ごとの傾向を示します。

- 割り当てられた座席数: 選択した期間に割り当てられたライセンスの合計数。

   マイクログラフは、選択した日付範囲内で、割り当てられた座席数の月ごとの傾向を示します。

- アクティブなシート数: 選択した期間中に使用されたライセンスの合計数。 

   このマイクログラフは、選択した期間の月間アクティブなシート数の月ごとの傾向を示しています。

- アクティブな使用率%: 選択した期間の使用可能な座席数に対する割合で表されたアクティブなシートの合計数。 

   マイクログラフは、選択した期間のアクティブな使用率の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-pbi-usage-summary.png" alt-text="使用状況の概要を Power BI します。":::

## <a name="power-bi-usage-by-geography"></a>地理別の使用状況の Power BI

**地理的な Power BI 使用量** は、顧客の国別の使用可能な座席とアクティブな座席の分布を表します。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内で拡大する国を検索して選択できます。

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-pbi-usage-geography.png" alt-text="地理によって使用 Power BI ます。":::

## <a name="power-bi-usage-by-sku"></a>SKU 別の使用状況の Power BI

SKU 別の Power BI 使用量は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-pbi-usage-sku.png" alt-text="SKU 別の使用状況を Power BI します。":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客サブスクリプションごとのアクティブな使用状況の月ごとの傾向を示します。 収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードしてすべてのサブスクリプションの詳細を表示できます。

:::image type="content" source="images/pci/pci-pbi-usage-subscription.png" alt-text="サブスクリプションのパフォーマンスを Power BI します。":::

## <a name="power-bi-usage-distribution"></a>Power BI 使用量の分布

Power BI 使用分布は、使用可能な座席、アクティブなシート数、および Sku 別に割り当てられた座席の内訳を示します。

:::image type="content" source="images/pci/pci-pbi-usage-distribution.png" alt-text="使用量の分布を Power BI します。":::

## <a name="next-steps"></a>次の手順

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

- このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
