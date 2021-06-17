---
title: パートナー センター Insights の概要ダッシュボード
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ライセンス、サブスクリプション、Azure の消費による売上とデプロイ、顧客の成長、収益の増加に関する方法のスナップショットを参照してください。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aea78f2a9b60f5d8adcc7962d15749479424c9f1
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277489"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>パートナー センターの分析情報で利用できる概要ダッシュボード レポート
 
**適切なロール**: グローバル管理者|管理エージェント |レポート ビューアー |エグゼクティブ レポート ビューアー

[分析情報の概要] ダッシュボードには、顧客、サブスクリプション、Azure 消費収益、ライセンスなどの主要業績評価指標のスナップショット ビューが表示されます。 概要レポートでは、次のグラフを視覚化できます。

- まとめ  
- 顧客、サブスクリプション、ライセンスの地理的分散  
- 顧客の成長傾向 
- サブスクリプションの増加傾向 
- Azure の消費収益増加傾向 
- ライセンスの増加傾向 

## <a name="summary"></a>まとめ

[概要] には、顧客、Azure 使用による収益 (ACR)、販売されたサブスクリプション、アクティブなサブスクリプション、デプロイされたライセンスに関する情報が含まれます。 

:::image type="content" source="images/pci/summary.png" alt-text="概要ライセンス。":::

概要の各セクションの詳細については、以下を参照してください。

### <a name="customers"></a>顧客

[ **顧客] 領域** には次が含まれます。

- 異なる属性の種類とすべてのクラウド製品にわたって、少なくとも 1 つのアクティブなサブスクリプションが会社に関連付けられているすべての顧客の現在の数。
- 選択した日付範囲内の顧客の増加率。
- マイクロ グラフには、選択した日付範囲内の顧客数の月別の傾向が表示されます。

### <a name="azure-consumed-revenue-acr"></a>Azure 使用による収益 (ACR)

[ **概要Azure 使用による収益 (ACR)** 領域には次が含まれます。

- 選択したAzure 使用による収益に対して属性付けされた合計値 (米国ドル)。
- 選択した日付範囲内の属性付き ACR (米国ドル) の増加率または減少率。
- マイクロ グラフには、選択した日付範囲に対する ACR US$ の月次傾向が表示されます 

> [!NOTE]
> Azure 使用による収益 (ACR) データは、エグゼクティブ レポート ビューアー ロールが割り当てられているユーザーが使用できます 
 
### <a name="subscriptions-sold"></a>販売されたサブスクリプション

[ **概要] の [サブスクリプションの** 販売] 領域には、次が含まれます。

- お使いによって販売または管理されているクラウド製品サブスクリプション (アクティブおよび非アクティブ) の現在の総数。  
- 選択した日付範囲内のサブスクリプションの増加率または減少率。
- マイクロ グラフは、選択した日付範囲に対するサブスクリプションの合計の月別の傾向を示します。

### <a name="active-subscriptions"></a>アクティブなサブスクリプション

[ **概要] の [アクティブ** なサブスクリプション] 領域には、次が含まれます。

- 製品テレメトリに基づいて測定されたアクティブな使用状況を持つクラウド製品サブスクリプションの現在の数。 Azure サブスクリプションの場合、すべての試用版サブスクリプションは除外されます。  
- 選択した日付範囲におけるアクティブなサブスクリプションの増加率。
- マイクロ グラフは、選択した日付範囲におけるアクティブなサブスクリプションの月別の傾向を示します。
 
### <a name="licenses-deployed"></a>デプロイされたライセンス

[ **概要] の [デプロイ** されたライセンス] 領域には、次が含まれます。
 
- 選択した期間に顧客サブスクリプションにデプロイされたクラウド製品ライセンスの数。 
- 選択した日付範囲内におけるこれらのライセンスの増加率または減少率。 
- マイクロ グラフには、選択した日付範囲に対するこれらの割り当て済みライセンス数の月別の傾向が表示されます。

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>顧客、サブスクリプション、ライセンスの地理的分散

このビューは、顧客、サブスクリプション、ライセンスの合計を顧客の国別に地理的に分布したビューです。 さまざまなタブを選択して、マップ上にこれらの各分析情報を表示します。 グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ホーム] ボタンを押して、元のビューに戻します。 各タブ (顧客、サブスクリプションなど) をクリックすると、各国のメトリックの値と国の合計の割合が表示されます。  

:::image type="content" source="images/pci/geosummary.png" alt-text="地理的な概要。":::

## <a name="customers-growth-trend"></a>顧客の成長傾向

選択した日付範囲の合計顧客数の月次傾向。 X 軸は、選択した日付範囲の月を表し、Y 軸は、その月の合計顧客数を表します。 

:::image type="content" source="images/pci/customergrowth.png" alt-text="顧客の成長傾向。":::

## <a name="subscriptions-growth-trend"></a>サブスクリプションの増加傾向

これは、選択した日付範囲の顧客サブスクリプション数の傾向を示します。 X 軸は選択した日付範囲の月を表し、Y 軸は選択した製品のサブスクリプション数を表します。 グラフの上部にあるスライダーをスクロールして、グラフを特定の期間にズームします。 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="サブスクリプションの増加傾向。":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure 使用による収益増加傾向

選択した日付範囲に対する Azure 消費収益の月次傾向 (米国ドル)。 X 軸は、選択した日付範囲の月を表し、Y 軸は、その月のユーザーに属性付けされた Azure 消費収益の合計 US$ を表します。

> [!NOTE]
> Azure 使用による収益 (ACR) は、エグゼクティブ レポート ビューアー ロールが割り当てられているユーザーにのみ表示されます。 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure の消費。":::

## <a name="licenses-growth-trend"></a>ライセンスの増加傾向
 
選択した日付範囲内のすべての顧客によって割り当てられたライセンスの傾向。 X 軸は選択した日付範囲の月を表し、Y 軸は選択した製品のライセンス数を表します。 グラフの上部にあるスライダーをスクロールして、グラフを特定の期間にズームします。  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="ライセンス。":::

## <a name="next-steps"></a>次のステップ

その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。
