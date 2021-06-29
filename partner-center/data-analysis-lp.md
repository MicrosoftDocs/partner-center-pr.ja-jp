---
title: サブスクリプションの分析情報に分析を使用する
ms.topic: article
ms.date: 11/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: ビジネスと顧客が購入したライセンスを使用する方法をよりよく理解するために、パートナー センター分析を使用する方法について説明します。
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ae31e7d917e96763e107212a78f28bfa10acf2f4
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013320"
---
# <a name="use-analytics-to-learn-more-about-subscription-revenue"></a>分析を使用してサブスクリプションの収益の詳細を確認する

**適切なロール**: グローバル管理者|MPN パートナー管理者

CSP ビジネスを展開する方法の計画には、顧客が Microsoft 製品をどのように使用しているかを把握することが含まれます。 パートナー センターでは、データを収集するためのいくつかのオプションを用意しており、貴社のビジネスと、貴社の顧客が購入したライセンスを使用しているかどうか、またどのように使用しているかについてデータを収集できます。 CSP ダイレクト モデルを使用している場合は、追加のデータを収集するために、Power BI 用パートナー センター分析アプリをインストールして使用する機会があります。

## <a name="access-to-the-subscription-analytics"></a>Subscription Analytics へのアクセス

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。
1. [CSP] メニューの [パートナー センター分析] を **選択** し、[サブスクリプション分析] **を選択します**。

1. 後続の 12 か月の CSP 収益がページの上部に表示されます

:::image type="content" source="images/analytics/subscription1.png" alt-text="[サブスクリプション] 画面。":::

## <a name="trailing-twelve-month-ttm-csp-revenue"></a>末尾Twelve-Month (TTM) CSP 収益

後続の 12 か月の CSP 収益は、パートナー グローバル アカウント レベルクラウド ソリューション プロバイダープログラムの収益の末尾を表します。 データは毎月 8 月に更新され、前月までの 12 か月の収益が表示されます。 たとえば、2020 年 9 月 9 日には、2019 年 9 月から 2020 年 8 月までの固定期間の TTM を確認できます。 ソフトウェア サブスクリプションは除外されます。 TTM Revenue には、請求書が既に支払われた対象の収益だけが反映されます。 

パートナー センターに表示される収益は、12 か月の一定の時間間隔で計算され、より短い期間に変更することはできません。

パートナーの場所アカウント レベルで収益の内訳を表示するには:

- [ダウンロードの詳細] リンクを選択し、すべての場所の TTM 収益を表示する .tsv ファイルをダウンロードします。

>[!NOTE] 
>.tsv ファイル内の MPN ID 全体の個々の TTM 収益数を合計すると、パートナー センター に表示される TTM 収益全体を超える可能性があります。 これは、ダウンロードしたファイルに複数のパートナー属性があるサブスクリプションの収益が 2 倍になる可能性があるためです。

## <a name="subscription-summary"></a>サブスクリプションの概要

画面の下半分には、サブスクリプションの概要が表示されます。 次のフィルターを使用して、必要なサブスクリプションの詳細を確認します。  

1. **期間**: サブスクリプションの概要を表示することを選択できます。 

- 30D – 過去 30 日間
- 3 分 – 過去 3 か月
- 6 分 – 過去 6 か月
- 12 分 – 過去 12 か月

2. **製品の種類**:
 
- Office 365
- Microsoft 365
- Dynamics 365
- EMS

これらのフィルターを適用すると、このレポートの上部にある TTM 収益メトリックに影響はありません。


 
## <a name="next-steps"></a>次のステップ

- [購入したライセンスを顧客がどのように使用しているのか分析する](increasing-adoption-and-satisfaction.md)  
- [顧客のアクティビティ ログの表示](activity-logs.md)
- [Power BI 用パートナー センター分析アプリ](power-bi-app-for-direct-partners.md)






