---
title: パートナーセンターの Insights Enterprise Mobility + Security 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様のために販売または管理している Enterprise Mobility + Security サブスクリプションの使用状況について、お客様がどのように改善できるかをご確認ください。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 48577571e77bd0181b78e01558a07edd1a3b925d
ms.sourcegitcommit: ce1331c0e600e2f73b85a90ac159a9026ab6a691
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "98146708"
---
# <a name="enterprise-mobility--security-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナーセンターの Insights ダッシュボードから使用可能な Enterprise Mobility + Security 使用状況レポート

**適切なロール**
- グローバル管理者
- 管理エージェント
- レポート ビューア
- エグゼクティブレポートビューアー

Enterprise Mobility + Security 使用状況レポートには、顧客が販売または管理している Enterprise Mobility + Security サブスクリプションの使用状況データが表示されます。 Enterprise Mobility + Security の使用状況レポートでは、次のセクションを表示できます。

- まとめ
- 地理別の使用状況の Enterprise Mobility + Security
- SKU 別の使用状況の Enterprise Mobility + Security
- サブスクリプションのパフォーマンス
- Enterprise Mobility + Security 使用量の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、役員レポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客が販売または管理している Enterprise Mobility + Security 使用状況サブスクリプションに関連する主要指標のスナップショットビューが表示されます。 

- 新しいサブスクリプション: 選択した期間に販売または管理されているサブスクリプションの合計数。

   マイクログラフは、選択した日付範囲の新しいサブスクリプションの月単位の傾向を示します。

- 使用可能なシート数: 選択した期間中に販売されたライセンスの合計数。

   マイクログラフは、選択した日付範囲内の使用可能な座席数の月単位の傾向を示します。

- 月ごとのアクティブな使用状況: 先月の期間に使用されたライセンスの数。

   マイクログラフは、選択した期間にわたって使用されたライセンスの月ごとの傾向を示します。

:::image type="content" source="images/pci/pci-ems-usage-summary.png" alt-text="EMS 使用状況の概要":::

## <a name="enterprise-mobility--security-usage-by-geography"></a>地理別の使用状況の Enterprise Mobility + Security

**地理的な Enterprise Mobility + Security 使用量** は、顧客の国ごとの月間アクティブユーザー数 (mau) と有料使用可能ユニット (pau) の分布を表します。 MAU は、前月に使用されたライセンスの数を示し、PAU は選択した期間に販売または管理されている有料の座席の数を示します。 マップ上の薄い色は下限値を表し、濃い色は高い値を表します。 グリッド内の国を検索して選択できます。 拡大して表示することもできます。

[ **国/地域の数** ] テーブルには、Azure の使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ **ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-ems-usage-geography.png" alt-text="地理的による EMS の使用状況":::

## <a name="enterprise-mobility--security-usage-by-sku"></a>SKU 別の使用状況の Enterprise Mobility + Security

SKU 別の Enterprise Mobility + Security 使用量は、MAU と PAU by Sku の月ごとの内訳を示しています。

:::image type="content" source="images/pci/pci-ems-usage-sku.png" alt-text="SKU による EMS の使用状況":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、ユーザーのサブスクリプションごとに MAU と PAU の Sku 別に分類されています。 収益を請求して上位100の顧客のデータがテーブルに表示されます。顧客を検索するか、生データをダウンロードして、すべての顧客の詳細を表示できます。

:::image type="content" source="images/pci/pci-ems-usage-subscription.png" alt-text="EMS サブスクリプションのパフォーマンス":::

## <a name="enterprise-mobility--security-usage-distribution"></a>Enterprise Mobility + Security 使用量の分布

Enterprise Mobility + Security 使用分布は、Sku 別の PAU とサブスクリプションの内訳を示します。

:::image type="content" source="images/pci/pci-ems-usage-distribution.png" alt-text="EMS 使用率の分布":::

## <a name="next-steps"></a>次のステップ

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

- このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
