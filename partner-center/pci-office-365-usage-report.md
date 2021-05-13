---
title: Partner center insights office 365 使用状況レポート
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: お客様のお客様のために販売または管理する Office 365 サブスクリプションの使用状況について、お客様が何をしているかをご確認ください。
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 685dce8d521bc27b9b91efd5206e9da0d7e45f34
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854605"
---
# <a name="office-365-usage-report-available-from-the-partner-center-insights-dashboard"></a>パートナーセンターの Insights ダッシュボードから使用可能な Office 365 使用状況レポート

**適切なロール**: 全体管理者 |管理エージェント |レポートビューアー |エグゼクティブレポートビューアー

Office 365 使用状況レポートには、顧客が販売または管理している Office 365 サブスクリプションの使用状況データが表示されます。 Office 365 の使用状況レポートでは、次のセクションを表示できます。

- まとめ
- 地理的に別の Office 365 の使用状況
- Office 365 ワークロード別の使用状況
- サブスクリプションのパフォーマンス
- Office 365 の使用量の分布

 > [!NOTE]
 > このレポートは、Insights ダッシュボードから入手できます。 このレポートを表示するには、グローバル管理者、アカウント管理者、レポートビューアー、エグゼクティブレポートビューアーなど、パートナーセンターの特定のロールが割り当てられている必要があります。 詳細については、会社のグローバル管理者に問い合わせてください。このレポートの特定の種類のデータは、役員レポートビューアーの特権を持つユーザーのみが使用できる場合もあります。

## <a name="summary"></a>まとめ

[概要] セクションには、顧客が販売または管理している Office 365 サブスクリプションに関連する主要指標のスナップショットビューが表示されます。  

- 新しいサブスクリプション: 選択した期間に販売または管理されているサブスクリプションの合計数。

   マイクログラフは、選択した日付範囲の新しいサブスクリプション数の月単位の傾向を示します。

- 使用可能なシート数: 選択した期間中に販売されたライセンスの合計数。

   マイクログラフは、選択した日付範囲内のライセンス販売数の月ごとの傾向を示します。

- 月間アクティブユーザー数: 先月、ワークロードを使用したユーザーの数。 

   このマイクログラフは、選択した期間における月間アクティブユーザーの月間傾向を示しています。

:::image type="content" source="images/pci/pci-o365-usage-summary.png" alt-text="Office 365 の使用状況の概要":::

## <a name="office-365-usage-by-geography"></a>地域別の Office 365 の使用状況

**地域別 Office 365** の使用状況は、顧客の国別の月間アクティブ ユーザー (MAU) と有料利用可能ユニット (PAU) の分布を示しています。 MAU は前月に使用されたライセンスの数を指し、PAU は選択した期間に販売または管理された有料シートの数を指します。 マップ上の明るい色は低い値を表し、濃い色は高い値を表します。 グリッドで国を検索して選択できます。 さらに詳しく見る場合は、拡大して表示できます。

[ **国/地域の数] テーブル** には、Azure 使用状況イベントが生成される国/地域の合計が表示されます。

グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップ上 **の [ホーム** ] オプションを選択して、元のビューに戻します。


:::image type="content" source="images/pci/pci-o365-usage-geography.png" alt-text="地域別の Office 365 の使用状況":::

## <a name="office-365-usage-by-workload"></a>ワークロード別の Office 365 の使用状況

ワークロード別の Office 365 の使用状況は、ワークロード別の MAU と PAU の内訳を示しています。

:::image type="content" source="images/pci/pci-o365-usage-workload.png" alt-text="ワークロード別の Office 365 の使用状況":::

## <a name="subscriptions-performance"></a>サブスクリプションのパフォーマンス

サブスクリプションのパフォーマンスは、顧客ごとのワークロード別の MAU と PAU の内訳を示しています。 請求された収益別の上位 100 人の顧客のデータが表に表示され、任意の顧客を検索したり、生データをダウンロードしてすべての顧客の詳細を表示することができます。

:::image type="content" source="images/pci/pci-o365-usage-subscription.png" alt-text="Office 365 サブスクリプションのパフォーマンス":::

## <a name="office-365-usage-distribution"></a>Office 365 の使用状況の分布

Office 365 の使用状況の分布は、SKU 別の PAU とサブスクリプションの内訳を示しています。

:::image type="content" source="images/pci/pci-o365-usage-distribution.png" alt-text="Office 365 の使用状況の分布":::

## <a name="next-steps"></a>次の手順

- 詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。

- このレポートを作成する生データは、Insights ダッシュボードの [レポートのダウンロード] セクションからダウンロードできます。 [詳細情報](pci-download-reports.md) 
