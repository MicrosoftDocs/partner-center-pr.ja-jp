---
title: サブスクリプションの分析情報を使用する
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターで analytics を使用して、ビジネスについて理解を深め、顧客が購入したライセンスをどのように使用するかについて説明します。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 19e7cf9442660a24d36b5f7c20fab156fdc0d59a
ms.sourcegitcommit: bfc9e6f6476766cf10ba714f03ca2e96560003b1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/14/2020
ms.locfileid: "94626074"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>分析を使用してサブスクリプション収益の詳細を確認する

**適切なロール**

- グローバル管理者
- MPN パートナー管理者

CSP ビジネスを展開する方法の計画には、顧客が Microsoft 製品をどのように使用しているかを把握することが含まれます。 パートナー センターでは、データを収集するためのいくつかのオプションを用意しており、貴社のビジネスと、貴社の顧客が購入したライセンスを使用しているかどうか、またどのように使用しているかについてデータを収集できます。 CSP direct モデルを使用している場合は、Power BI 用のパートナーセンター分析アプリをインストールして使用し、追加のデータを収集することもできます。

## <a name="access-to-the-subscription-analytics"></a>サブスクリプション分析へのアクセス

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。
1. [パートナーセンター] メニューの [CSP] で、[ **分析** ] を選択し、[ **サブスクリプション分析** ] を選択します。

1. 最後の12か月の CSP 収益がページの上部に表示されます

:::image type="content" source="images/analytics/subscription1.png" alt-text="サブスクリプション画面":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>末尾の Twelve-Month (TTM) CSP 収益

12か月の末尾の CSP 収益は、パートナーのグローバルアカウントレベルで、最後のクラウドソリューションプロバイダープログラムの収益を USD 単位で表します。 データは毎月8日に更新され、前月までの12か月の売上が表示されます。 たとえば、2020年9月9日には、2019年9月から8月 8 2020 日までの間、TTM を確認することができます。

パートナーセンターに表示される収益は、固定された12か月の期間に対して計算され、より短い時間枠に変更することはできません。

取引先のアカウントレベルで収益の内訳を確認するには、次のようにします。

- [ダウンロードの詳細] リンクを選択して、すべての場所で TTM の売上を表示する tsv ファイルをダウンロードします。

>[!NOTE] 
>Tsv ファイルの MPN Id 全体にわたる個々の TTM 収益数を合計した値が、パートナーセンターに表示される TTM 全体の売上を超えているように見える場合があります。 これは、ダウンロードされたファイルに複数の partner 帰属があるサブスクリプションに対して、収益が二重にカウントされる可能性があるためです。

## <a name="subscription-summary"></a>サブスクリプションの概要

画面の下半分には、サブスクリプションの概要が表示されます。 次のフィルターを使用して、必要なサブスクリプションの詳細を表示します。  

1. **期間** : サブスクリプションの概要を表示することを選択できます。 

- 30D –過去30日間
- 3M –過去3か月間
- 6分–過去6か月
- 12M –過去12か月間

2. **製品の種類** :
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

これらのフィルターを適用しても、このレポートの最上部にある TTM 収益メトリックには影響しません。


 
## <a name="next-steps"></a>次のステップ

- [購入したライセンスを顧客がどのように使用しているかを分析する](increasing-adoption-and-satisfaction.md)  
- [顧客のアクティビティ ログの表示](activity-logs.md)
- [Power BI 用パートナー センター分析アプリ](power-bi-app-for-direct-partners.md)






