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
ms.openlocfilehash: 76a589037817707378e39f4301313eee7284422a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565459"
---
# <a name="dynamics-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナー センター Insights ダッシュボードから使用できる Dynamics 使用状況レポート

**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

Dynamics 使用状況レポートには、顧客に対して販売または管理した Microsoft Dynamics 365 サブスクリプションの使用状況データが表示されます。 次のセクションは、Dynamics 使用状況レポートから確認できます。

- まとめ
- 地域別の Dynamics の使用
- SKU 別の Dynamics の使用状況
- サブスクリプションのパフォーマンス
- Dynamics の使用状況の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから使用できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポート ビューアー、役員レポート ビューアーなど、パートナー センター で特定のロールを割り当てる必要があります。 詳細については、会社のグローバル管理者に関するページを参照してください。このレポートの特定の種類のデータは、エグゼクティブ レポート ビューアー特権を持つユーザーだけが使用できる場合もあります。

## <a name="summary"></a>まとめ

概要セクションには、顧客に対して販売または管理した Dynamics の使用状況サブスクリプションに関連する主要なインジケーターのスナップショット ビューが表示されます。  

- 使用可能なシート: 選択した期間に販売されたライセンスの総数。

   [マイクロ] グラフには、選択した日付範囲の使用可能なシート数の月の過去 1 か月の傾向が表示されます。

- 割り当てられたシート: 選択した期間に割り当てられたライセンスの総数。

   マイクロ グラフには、選択した日付範囲内の割り当て済みシート数の月別の傾向が表示されます。

- アクティブなシート: 選択した期間に使用されたライセンスの総数。 

   マイクロ グラフには、選択した期間における月間アクティブシートの月次傾向が表示されます。

- アクティブな使用率 %: 選択した時間枠で使用可能なシートに対する割合で表されるアクティブなシートの総数。 

   マイクロ グラフには、選択した期間におけるアクティブな使用率の月間傾向が表示されます。

:::image type="content" source="images/pci/pci-dynamics-usage-summary.png" alt-text="Dynamics の使用状況の概要。":::

## <a name="dynamics-usage-by-geography"></a>地域別の Dynamics の使用

地域 **別の Dynamics の使用状況は** 、顧客の国別の利用可能なシートとアクティブなシートの分布を示しています。 マップ上の明るい色は低い値を表し、濃い色は高い値を表します。 グリッドで国を検索して選択できます。 さらに詳しく見る場合は、拡大して表示できます。

[ **国/地域の数] テーブル** には、Azure 使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップ上 **の [ホーム** ] オプションを選択して、元のビューに戻します。

:::image type="content" source="images/pci/pci-dynamics-usage-geography.png" alt-text="地域別の Dynamics の使用。":::

## <a name="dynamics-usage-by-sku"></a>SKU 別の Dynamics の使用状況

SKU 別の Dynamics の使用状況は、SKU 別の利用可能なシート、アクティブなシート、および割り当てられたシートの月次傾向を示しています。

:::image type="content" source="images/pci/pci-dynamics-usage-sku.png" alt-text="SKU 別の Dynamics の使用状況。":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客サブスクリプションあたりのアクティブな使用状況の月間傾向を示しています。 請求収益別の上位 100 人の顧客のデータが表に表示されます。すべての顧客を検索したり、生データをダウンロードしてすべてのサブスクリプションの詳細を表示することができます。

:::image type="content" source="images/pci/pci-dynamics-usage-subscription.png" alt-text="Dynamics サブスクリプションのパフォーマンス。":::

## <a name="dynamics-usage-distribution"></a>Dynamics の使用状況の分布

Dynamics の使用状況の分布は、SKU 別の利用可能なシート、アクティブなシート、および割り当てられたシートの内訳を示しています。

:::image type="content" source="images/pci/pci-dynamics-usage-distribution.png" alt-text="Dynamics の使用状況の分布。":::

## <a name="next-steps"></a>次の手順

- その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。

- このレポートを利用する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
