---
title: パートナーセンターの Insights の概要ダッシュボード
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ライセンス、サブスクリプション、および Azure の消費量を使用した販売とデプロイ、顧客の成長、および収益の増加に関するスナップショットをご覧ください。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855201"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>パートナー センターの分析情報で利用できる概要ダッシュボード レポート
 
**適切なロール**: 全体管理者 |管理エージェント |レポートビューアー |エグゼクティブレポートビューアー

Insights の概要ダッシュボードには、顧客、サブスクリプション、Azure 従量課金、ライセンスなど、主要業績評価指標のスナップショットビューが表示されます。 概要レポートでは、次のグラフを視覚化できます。

- まとめ  
- 顧客、サブスクリプション、ライセンスの地理的拡散  
- 顧客成長傾向 
- サブスクリプションの増加傾向 
- Azure で消費された収益成長傾向 
- ライセンスの増加傾向 

## <a name="summary"></a>まとめ

概要には、顧客、Azure で使用された収益 (ACR)、販売されているサブスクリプション、アクティブなサブスクリプション、およびデプロイされたライセンスに関する情報が含まれます。 

:::image type="content" source="images/pci/summary.png" alt-text="ライセンスの概要":::

概要の各セクションの詳細については、「」を参照してください。

### <a name="customers"></a>顧客

[ **顧客** ] 領域には次のものが含まれます。

- さまざまな種類の組織に関連付けられている、少なくとも1つのアクティブなサブスクリプションがあるすべての顧客の現在の数を、すべてのクラウド製品でカウントします。
- 選択した日付範囲内の顧客の増加率。
- マイクログラフは、選択した日付範囲内の顧客数の月単位の傾向を示します。

### <a name="azure-consumed-revenue-acr"></a>Azure で消費された収益 (ACR)

概要の Azure の使用 **収益 (ACR)** 領域には次のものが含まれます。

- 選択した日付範囲について、Azure で消費された合計 (米ドル単位)。
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

このビューは、顧客、サブスクリプション、ライセンスの合計を顧客の国別に地理的に分布したビューです。 さまざまなタブを選択すると、これらの各分析情報がマップに表示されます。 グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ホーム] ボタンを押して、元のビューに戻します。 各タブ (Customers、サブスクリプションなど) をクリックすると、国ごとのメトリックの値と、その国の合計の割合が表示されます。  

:::image type="content" source="images/pci/geosummary.png" alt-text="地理的な概要":::

## <a name="customers-growth-trend"></a>顧客成長傾向

選択した日付範囲の合計顧客数の月ごとの傾向。 X 軸は選択した日付範囲の月を表し、Y 軸はその月の合計顧客数を表します。 

:::image type="content" source="images/pci/customergrowth.png" alt-text="顧客成長傾向":::

## <a name="subscriptions-growth-trend"></a>サブスクリプションの増加傾向

これは、選択した日付範囲に対する顧客サブスクリプションの数の傾向を示します。 X 軸は選択した日付範囲の月を表し、Y 軸は製品のサブスクリプション数を表します。 グラフの上部にあるスライダーをスクロールして、特定の期間にグラフを拡大します。 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="サブスクリプションの増加傾向":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure で消費された収益成長傾向

選択された日付範囲に対して Azure が使用した収益の月単位の傾向 (米ドル)。 X 軸は、選択された日付範囲の月を表し、Y 軸は月の間に、Azure が使用した総収益 (米国ドル) を表します。

> [!NOTE]
> Azure で使用された収益 (ACR) は、Executive レポートビューアーロールが割り当てられているユーザーのみに表示されます。 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure の使用量":::

## <a name="licenses-growth-trend"></a>ライセンスの増加傾向
 
選択した日付範囲内のすべての顧客によって割り当てられたライセンスの傾向。 X 軸は選択した日付範囲の月を表し、Y 軸は選択した製品のライセンス数を表します。 グラフの上部にあるスライダーをスクロールして、グラフを特定の期間にズームします。  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="ライセンス":::

## <a name="next-steps"></a>次の手順

その他のレポートについては [、「パートナー センター Insights 」を参照してください](partner-center-insights.md)。
