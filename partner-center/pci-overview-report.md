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
ms.openlocfilehash: cca136670fa2891eea32e4561b97692ca98a77a9
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565408"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>パートナー センターの分析情報で利用できる概要ダッシュボード レポート
 
**適切なロール**: 全体管理者 |管理エージェント |レポートビューアー |エグゼクティブレポートビューアー

Insights の概要ダッシュボードには、顧客、サブスクリプション、Azure 従量課金、ライセンスなど、主要業績評価指標 (Kpi) のスナップショットビューが表示されます。 概要レポートでは、次のグラフを視覚化できます。

- まとめ  
- 顧客、サブスクリプション、ライセンスの地理的拡散  
- 顧客成長傾向 
- サブスクリプションの増加傾向 
- Azure で消費された収益成長傾向 
- ライセンスの増加傾向 

## <a name="summary"></a>まとめ

概要には、顧客、Azure で使用された収益 (ACR)、販売されているサブスクリプション、アクティブなサブスクリプション、およびデプロイされたライセンスに関する情報が含まれます。 

:::image type="content" source="images/pci/summary.png" alt-text="ライセンスの概要。":::

概要の各セクションの詳細については、「」を参照してください。

### <a name="customers"></a>顧客

[ **顧客** ] 領域には次のものが含まれます。

- さまざまな種類の組織に関連付けられている、少なくとも1つのアクティブなサブスクリプションがあるすべての顧客の現在の数を、すべてのクラウド製品でカウントします。
- 選択した日付範囲内の顧客の増加率。
- マイクログラフは、選択した日付範囲内の顧客数の月単位の傾向を示します。

### <a name="azure-consumed-revenue-acr"></a>Azure で消費された収益 (ACR)

概要の Azure の使用 **収益 (ACR)** 領域には次のものが含まれます。

- 選択した日付範囲について、ユーザーに対して指定された ACR の合計 (米ドル単位)。
- 選択した日付範囲内の属性 ACR (米ドル単位) での拡張または拒否の割合。
- マイクログラフでは、選択した日付範囲について、米国ドルの ACR の月ごとの傾向が示されます。 

> [!NOTE]
> ACR データは、Executive レポートビューアーロールが割り当てられているユーザーが使用できます。
 
### <a name="subscriptions-sold"></a>販売済みサブスクリプション

概要で販売されている **サブスクリプション** の領域は次のとおりです。

- お持ちのクラウド製品サブスクリプション (アクティブおよび非アクティブ) の現在の合計数。  
- 選択した日付範囲内のサブスクリプションでの増加または拒否の割合。
- マイクログラフは、選択した日付範囲に対するサブスクリプションの合計の月単位の傾向を示します。

### <a name="active-subscriptions"></a>アクティブなサブスクリプション

概要の [ **アクティブなサブスクリプション** ] 領域には次のものが含まれます。

- 製品テレメトリに基づいてアクティブな使用状況を測定した、クラウド製品サブスクリプションの現在の数。 これにより、すべての試用版 Azure サブスクリプションが除外します。  
- 選択した日付範囲に対するアクティブなサブスクリプションの増加率。
- マイクログラフは、選択した日付範囲に対するアクティブなサブスクリプションの月単位の傾向を示します。
 
### <a name="licenses-deployed"></a>展開されたライセンス

概要の [ **展開済みライセンス** ] 領域には次のものが含まれます。
 
- 選択した期間にわたって顧客のサブスクリプションにデプロイされているすべてのクラウド製品ライセンスの数。 
- 選択した日付範囲内でのこれらのライセンスの増加または拒否の割合。 
- マイクログラフは、選択した日付範囲に割り当てられたこれらのライセンス数の月単位の傾向を示します。

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>顧客、サブスクリプション、ライセンスの地理的拡散

このビューは、顧客、サブスクリプション、およびライセンスの合計を顧客の国別に地理的に分散したものです。 さまざまなタブを選択すると、これらの各分析情報がマップに表示されます。 グリッドで国を検索して選択すると、マップ内の場所にズームできます。 マップの [ホーム] ボタンを押して、元のビューに戻します。 各タブ (Customers、サブスクリプションなど) をクリックすると、国ごとのメトリックの値と、その国の合計の割合が表示されます。  

:::image type="content" source="images/pci/geosummary.png" alt-text="地理的な概要。":::

## <a name="customers-growth-trend"></a>顧客成長傾向

選択した日付範囲の合計顧客数の月ごとの傾向。 X 軸は選択した日付範囲の月を表し、Y 軸はその月の合計顧客数を表します。 

:::image type="content" source="images/pci/customergrowth.png" alt-text="顧客の成長傾向。":::

## <a name="subscriptions-growth-trend"></a>サブスクリプションの増加傾向

これは、選択した日付範囲に対する顧客サブスクリプションの数の傾向を示します。 X 軸は選択した日付範囲の月を表し、Y 軸は製品のサブスクリプション数を表します。 グラフの上部にあるスライダーをスクロールして、特定の期間にグラフを拡大します。 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="サブスクリプションの増加傾向。":::

## <a name="azure-consumed-revenue-growth-trend"></a>Azure で消費された収益成長傾向

Azure の月単位の傾向は、選択した日付範囲に対して、米国ドルの収益を消費しました。 X 軸は、選択された日付範囲の月を表し、Y 軸は月中にユーザーに対して使用された Azure の総収益 (米ドル) を表します。

> [!NOTE]
> ACR は、Executive レポートビューアーロールが割り当てられているユーザーにのみ表示されます。 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Azure の使用量。":::

## <a name="licenses-growth-trend"></a>ライセンスの増加傾向
 
選択した日付範囲内のすべての顧客によって割り当てられたライセンスの傾向。 X 軸は選択した日付範囲の月を表し、Y 軸は選択した製品のライセンス数を表します。 グラフの上部にあるスライダーをスクロールして、特定の期間にグラフを拡大します。  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="ライン.":::

## <a name="next-steps"></a>次の手順

詳細なレポートについては、「 [Partner Center Insights](partner-center-insights.md)」を参照してください。
