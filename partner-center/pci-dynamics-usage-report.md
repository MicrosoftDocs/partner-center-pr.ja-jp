---
title: パートナーセンターインサイト dynamics 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様にとって、お客様のために販売または管理している Dynamics サブスクリプションの使用に関して、何をしているかをご確認ください。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: d8755cadf7b572972c5abe1483ff6f0be98a1eb8
ms.sourcegitcommit: ce1331c0e600e2f73b85a90ac159a9026ab6a691
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "98146692"
---
# <a name="dynamics-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナーセンターの Insights ダッシュボードから使用可能な Dynamics usage レポート

**適切なロール**
- グローバル管理者
- 管理エージェント
- レポート ビューア
- エグゼクティブレポートビューアー

Dynamics usage レポートには、顧客が販売または管理している Dynamics 365 サブスクリプションの使用状況データが表示されます。 Dynamics の使用状況レポートでは、次のセクションを表示できます。

- まとめ
- Geography による Dynamics の使用状況
- SKU による Dynamics の使用状況
- サブスクリプションのパフォーマンス
- Dynamics usage 分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、役員レポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

## <a name="summary"></a>まとめ

[概要] セクションには、顧客向けに販売または管理している Dynamics usage サブスクリプションに関連する主要なインジケーターのスナップショットビューが表示されます。  

- 使用可能なシート数: 選択した期間中に販売されたライセンスの合計数。

   マイクログラフは、選択した日付範囲について、使用可能な座席数の月ごとの傾向を示します。

- 割り当てられた座席数: 選択した期間に割り当てられたライセンスの合計数。

   マイクログラフは、選択した日付範囲内で、割り当てられた座席数の月ごとの傾向を示します。

- アクティブなシート数: 選択した期間中に使用されたライセンスの合計数。 

   このマイクログラフは、選択した期間の月間アクティブなシート数の月ごとの傾向を示しています。

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

:::image type="content" source="images/pci/pci-dynamics-usage-distribution.png" alt-text="Dynamics usage 分布":::

## <a name="next-steps"></a>次のステップ

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

- このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
