---
title: 一般的な月次請求シナリオ
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 月単位の課金パートナー センター使用する場合の一般的なシナリオには、新しいサブスクリプションの追加、ライセンス数の変更、サブスクリプションの中断が含まれます。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148654"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>新しいサブスクリプション、ライセンス金額の変更、または中断に関する月次課金シナリオのサンプル

**適切なロール**: 管理エージェント |課金管理者|ヘルプデスク エージェント |セールス エージェント

これらの一 [般的な課金シナリオの](common-billing-scenarios.md) 例は、月次課金を使用する場合にパートナー センター。

## <a name="new-monthly-subscription"></a>新しい月次サブスクリプション

請求日は毎月 15 日です。 1 月 13 日に、1 つのライセンスで $4/月の新しいサブスクリプションを購入し、毎月の課金を選択します。 1 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2/12/2018    |Cycle fee   |4.00       |1        |4.00 |

2 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/2/13         |2018/3/12    |Cycle fee   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>ライセンス数の変更

請求日は毎月 15 日です。 1 月 13 日に、1 つのライセンスで $4/月の新しいサブスクリプションを購入し、毎月の課金を選択します。 1 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2/12/2018    |Cycle fee   |4.00       |1        |4.00    |

2 月 1 日には、ライセンス数量を 1 から 2 に増やします。 2 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 2018/1/13        |2/12/2018    |サイクル インスタンスの日割り料金   |-4.00       |1        |-4.00   |
|2018/1/13         |2018/1/31    | サイクル インスタンスの日割り料金   |2.45       |1        |2.45    |
|2018 年 2 月 1 日         |2/12/2018    | サイクル インスタンスの日割り料金   |1.55       |2        |3.10    |
|2018/2/13         |2018/3/12    | サイクル インスタンスの日割り料金   |4.00       |2        |8.00    |

月額料金は 4.00 で、サービス期間 2018/1/13 ～ 2018/2/12 には 31 日間あります。 これは、1 日あたりの価格 0.129 (4/31) に相当します。

日割り計算期間 2018/1/13 ～ 2018/1/31 には 19 日間あります。

日割り単価 = 2.451 = 19 x 0.129

日割り計算期間 2018/2/1 ～ 2018/2/12 には 12 日間あります。

日割り単価 = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>30 日経過前に中断

請求日は毎月 15 日です。 1 月 13 日に、1 つのライセンスで $4/月の新しいサブスクリプションを購入し、毎月の課金を選択します。 1 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2/12/2018    |Cycle fee   |4.00       |1        |4.00    |

2 月 1 日に、サブスクリプションを中断します。 2 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/1/13|2/12/2018|取り消し料金|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>30 日経過後に中断

請求日は毎月 15 日です。 1 月 13 日に、1 つのライセンスで $4/月の新しいサブスクリプションを購入し、毎月の課金を選択します。 1 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/1/13|2/12/2018|サイクル料金|4.00|1|4.00

2 月 15 日のライセンス ベースの調整ファイルには、次の請求行が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/2/13|2018/3/12|サイクル料金|4.00|1|4.00

3月1日にサブスクリプションを中断します。 3月15日のライセンスベースの調整ファイルには、次の請求明細が含まれます。

|請求開始日 |請求終了日 |料金タイプ |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/3/1|2018/3/12|取り消し料金|-1.72|1|-1.72

月額料金は 4.00 で、サービス期間 2018/2/13 ～ 2018/3/12 には 28 日間あります。 これは、1 日あたりの価格 0.143 (4/28) に相当します。

単価 = サービス期間の日数 x 1 日あたりの価格 x ライセンス数

取り消し期間 2018/3/1 ～ 2018/3/12 には 12 日間あります。

したがって、単価 = -1.716 (12 x 0.143 x (-1)) です。

## <a name="next-steps"></a>次のステップ

- [1回限りの課金および選択された定期的な購入の課金シナリオ](common-billing-scenarios-onetime-recurring.md)