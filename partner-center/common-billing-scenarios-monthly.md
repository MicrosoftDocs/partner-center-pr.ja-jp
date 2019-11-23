---
title: Common monthly billing scenarios | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common scenarios in Partner Center when you use monthly billing (such as adding new subscriptions, changing license quantity, and suspending subscriptions.)
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, monthly billing, subscriptions, reconciliation file
ms.localizationpriority: medium
ms.openlocfilehash: 95a535ecdd20614e8809d6304609b1a678859efc
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389620"
---
# <a name="monthly-billing-scenarios"></a>Monthly billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable if you use monthly billing in Partner Center.

## <a name="new-monthly-subscription"></a>New monthly subscription

請求日は毎月 15 日です。 1 月 13 日に、4ドル/月のライセンスを 1 つ含む新しいサブスクリプションを購入し、月次請求を選択しました。 1 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2018/2/12    |Cycle fee   |4.00       |1        |4.00 |

2 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/2/13         |2018/3/12    |Cycle fee   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Change license quantity

請求日は毎月 15 日です。 1 月 13 日に、4ドル/月のライセンスを 1 つ含む新しいサブスクリプションを購入し、月次請求を選択しました。 1 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2018/2/12    |Cycle fee   |4.00       |1        |4.00    |

2 月 1 日、ライセンスの数を 1 から 2 に増やします。 2 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 2018/1/13        |2018/2/12    |Cycle Instance Prorate (サイクル インスタンスの日割り料金)   |-4.00       |1        |-4.00   |
|2018/1/13         |2018/1/31    | Cycle Instance Prorate (サイクル インスタンスの日割り料金)   |2.45       |1        |2.45    |
|2018/2/1         |2018/2/12    | Cycle Instance Prorate (サイクル インスタンスの日割り料金)   |1.55       |2        |3.10    |
|2018/2/13         |2018/3/12    | Cycle Instance Prorate (サイクル インスタンスの日割り料金)   |4.00       |2        |8.00    |

月額料金は 4.00 で、サービス期間 2018/1/13 ～ 2018/2/12 には 31 日間あります。 これは、1 日あたりの価格 0.129 (4/31) に相当します。

日割り計算期間 2018/1/13 ～ 2018/1/31 には 19 日間あります。

日割り単価 = 2.451 = 19 x 0.129

日割り計算期間 2018/2/1 ～ 2018/2/12 には 12 日間あります。

日割り単価 = 1.54 = 12 x 0.129

## <a name="suspend-before-30-days"></a>Suspend before 30 days

請求日は毎月 15 日です。 1 月 13 日に、4ドル/月のライセンスを 1 つ含む新しいサブスクリプションを購入し、月次請求を選択しました。 1 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2018/1/13         |2018/2/12    |Cycle fee   |4.00       |1        |4.00    |

2 月 1 日、サブスクリプションを中断します。 2 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/1/13|2018/2/12|Cancel Fee (取り消し料金)|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspend after 30 days

請求日は毎月 15 日です。 1 月 13 日に、4ドル/月のライセンスを 1 つ含む新しいサブスクリプションを購入し、月次請求を選択しました。 1 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/1/13|2018/2/12|サイクル料金|4.00|1|4.00

2 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/2/13|2018/3/12|サイクル料金|4.00|1|4.00

3 月 1 日、サブスクリプションを中断します。 3 月 15 日、ライセンスベースの調整ファイルに次の請求行が追加されます。

|請求開始日 |請求終了日 |請求の種類 |単価 |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2018/3/1|2018/3/12|Cancel Fee (取り消し料金)|-1.72|1|-1.72

月額料金は 4.00 で、サービス期間 2018/2/13 ～ 2018/3/12 には 28 日間あります。 これは、1 日あたりの価格 0.143 (4/28) に相当します。

単価 = サービス期間の日数 x 1 日あたりの価格 x ライセンス数

取り消し期間 2018/3/1 ～ 2018/3/12 には 12 日間あります。

したがって、単価 = -1.716 (12 x 0.143 x (-1)) です。
