---
title: パートナー センター分析情報 Office 365 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客に対して販売または管理する Office 365 サブスクリプションの使用状況に関して、何がうまく機能し、どこで改善できるのかを確認します。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 43ac7763b32eed5c63fd3766262ad1649ae81e11
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565374"
---
# <a name="office-365-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナー センター Insights ダッシュボードから利用できる Office 365 使用状況レポート

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

Office 365 使用状況レポートには、顧客に対して販売または管理した Office 365 サブスクリプションの使用状況データが表示されます。 Office 365 使用状況レポートから次のセクションを表示できます。

- まとめ
- 地域別の Office 365 の使用状況
- ワークロード別の Office 365 の使用状況
- サブスクリプションのパフォーマンス
- Office 365 の使用状況の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、役員レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客に対して販売または管理した Office 365 サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。  

- 新しいサブスクリプション: 選択した期間に販売または管理されたサブスクリプションの総数。

   [マイクロ] グラフには、選択した日付範囲の [新しいサブスクリプション数] の月別の傾向が表示されます。

- 使用可能なシート: 選択した期間に販売されたライセンスの総数。

   [マイクロ] グラフには、選択した日付範囲内のライセンスの販売数の月別の傾向が表示されます。

- 月間アクティブ ユーザー数: 前月にワークロードを使用したユーザーの数。 

   [マイクロ] グラフには、選択した期間における月間アクティブ ユーザーの月次傾向が表示されます。

:::image type="content" source="images/pci/pci-o365-usage-summary.png" alt-text="Office 365 の使用状況の概要。":::

## <a name="office-365-usage-by-geography"></a>地域別の Office 365 の使用状況

**地域別 Office 365** の使用状況は、顧客の国別の月間アクティブ ユーザー (MAU) と有料利用可能ユニット (PAU) の分布を示しています。 MAU は前月に使用されたライセンスの数を指し、PAU は選択した期間に販売または管理された有料シートの数を指します。 マップ上の明るい色は低い値を表し、濃い色は高い値を表します。 グリッドで国を検索して選択できます。 さらに詳しく見る場合は、拡大して表示できます。

[ **国/地域の数] テーブル** には、Azure 使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップ上 **の [ホーム** ] オプションを選択して、元のビューに戻します。


:::image type="content" source="images/pci/pci-o365-usage-geography.png" alt-text="地域別の Office 365 の使用状況。":::

## <a name="office-365-usage-by-workload"></a>ワークロード別の Office 365 の使用状況

ワークロード別の Office 365 の使用状況は、ワークロード別の MAU と PAU の内訳を示しています。

:::image type="content" source="images/pci/pci-o365-usage-workload.png" alt-text="ワークロード別の Office 365 の使用状況。":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客ごとのワークロード別の MAU と PAU の内訳を示しています。 請求された収益別の上位 100 人の顧客のデータが表に表示され、任意の顧客を検索したり、生データをダウンロードしてすべての顧客の詳細を表示することができます。

:::image type="content" source="images/pci/pci-o365-usage-subscription.png" alt-text="Office 365 サブスクリプションのパフォーマンス。":::

## <a name="office-365-usage-distribution"></a>Office 365 の使用状況の分布

Office 365 の使用状況の分布は、SKU 別の PAU とサブスクリプションの内訳を示しています。

:::image type="content" source="images/pci/pci-o365-usage-distribution.png" alt-text="Office 365 の使用状況の分布。":::

## <a name="next-steps"></a>次の手順

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

- このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
