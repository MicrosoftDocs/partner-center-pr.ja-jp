---
title: Common billing scenarios for one-time and select recurring purchases | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Common billing scenarios in Partner Center for one-time and select recurring purchases (such as purchasing subscriptions, adding more subscriptions, adding and removing seats).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, one-time purchase, recurring purchase, subscriptions, seats
ms.localizationpriority: medium
ms.openlocfilehash: 69a7f1d4ded608942ea8b4bd7bec6054a44d52c7
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389640"
---
# <a name="one-time-and-select-recurring-purchase-billing-scenarios"></a>One-time and select recurring purchase billing scenarios

These example [common billing scenarios](common-billing-scenarios.md) are applicable to [one-time and select recurring charges](one-time-and-recurring-billing.md) in Partner Center.

## <a name="purchase-a-subscription-and-add-a-seat-on-the-same-day"></a>Purchase a subscription and add a seat on the same day

シナリオ 1 では、サブスクリプションを 6 月 11 日に単価 $4 で購入します。 同じ日に、後で、同じサブスクリプションを別の価格で購入します。

調整ファイルには、次のものが含まれます。

- サービス期間 6/10 から 7/9 に対する請求額: $4。
- サービス期間 6/11 から 6/11 に対する日割り換算の再請求額: $-4.00。 これは、お客様が 1 ライセンスを所有していた期間です。 計算は、(月額/サービス期間内の合計日数) x サービス期間内で日割り換算する日数 x ライセンス数 = (4/30) x 30 x 1 = 4.00 となります。
- サービス期間 6/10 ～ 7/9 に対する日割り換算の再請求額: $8.00。 これは、お客様が 2 ライセンスを所有していた期間です。 計算は (4/30) x 30 x 2 = 8.00 となります。

|**購入日**   |**課金開始** |**課金終了**  |**単価**  |**数量**  |**金額** |**請求の種類** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/9         |$4                |1                 |$4            |新規         |
|2019/6/11     | 2019/6/10    |2019/7/9        |$4        |1        | -$4       |addQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/9        |$4        | 2      |$8         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Purchase a subscription and add more subscriptions later

シナリオ 2 では、6 月 11 日にサブスクリプションを単価 $4 で購入し、6 月 12 日に同じ製品の別のサブスクリプションを同じ価格で購入します。

調整ファイルには、次のものが含まれます。

- サービス期間 6/10 から 7/9 に対する請求額: $4。
- サービス期間 6/11 から 6/12 に対する日割り換算の再請求額: $-3.87。 これは、お客様が 1 ライセンスを所有していた期間です。 計算は、(月額/サービス期間内の合計日数) x サービス期間内で日割り換算する日数 x ライセンス数 = (4/30) x 29 x 1 = 3.87 となります。
- サービス期間 6/12 から 7/9 に対する日割り換算の再請求額: $7.74。 これは、お客様が 2 ライセンスを所有していた期間です。 計算は (4/30) x 29 x 2 = 7.74 となります。

|**購入日**   |**課金開始** |**課金終了**  |**単価**  |**数量**  |**金額** |**請求の種類** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11 (1 ライセンスを所有)     |2019/6/10   |2019/7/9         |$4         |1        |$4            |新規         |
|2019/6/12     | 2019/6/10    |2019/7/9        |$4        |1        | -$3.87       |addQuantity           |
|2019/6/12     | 2019/6/10    |2019/7/9        |$4        | 2      |$7.74       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-seat-on-the-same-day"></a>Purchase a subscription and remove a seat on the same day

シナリオ 3 では、6 月 11 日に同じ製品の 2 つのサブスクリプションを単価 $4 で購入します。 同じ日に、後で、シートの 1 つを削除します。  

調整ファイルには、次のものが含まれます。

- サービス期間 6/10 から 7/9 の 2 ライセンスに対する請求額: $8。
- サービス期間 6/11 から 6/11 に対する日割り換算の再請求額: $-8.00。 これは、お客様が 2 ライセンスを所有していた期間です。 計算は、(月額/サービス期間内の合計日数) x サービス期間内で日割り換算する日数 x ライセンス数 = (4/30) x 30 x 2 = 8.00 となります。
- サービス期間 6/11 から 7/9 に対する日割り換算の再請求額: $4.00。 これは、お客様が 1 ライセンスを所有していた期間です。 計算は (4/30) x 30 x 1 = 4.00 となります。

|**購入日**   |**課金開始** |**課金終了**  |**単価**  |**数量**  |**金額** |**請求の種類** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11      |2019/6/10   |2019/7/9         |$4                |2                 |$8            |新規         |
|2019/6/11     | 2019/6/10    |2019/7/9        |$4        |2        | -$8       |removeQuantity           |
|2019/6/11     | 2019/6/10    |2019/7/9        |$4        | 1      |$4         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-seats-later"></a>Purchase a subscription and remove seats later

シナリオ 4 では、6 月 11 日に単価 $4 で 2 つのサブスクリプションを購入し、6 月 12 日に 1 つのシートを削除します。

調整ファイルには、次のものが含まれます。

- サービス期間 6/10 から 7/9 に対する請求額: $8。
- サービス期間 6/11 ～ 6/12 に対する日割り換算の再請求額: $-7.74。 これは、お客様が 2 ライセンスを所有していた期間です。 計算は、(月額/サービス期間内の合計日数) x サービス期間内で日割り換算する日数 x ライセンス数 = (4/30) x 29 x 2 = 7.74 となります。
- サービス期間 6/12 から 7/9 に対する日割り換算の再請求額: $3.87。 これは、お客様が 1 ライセンスを所有していた期間です。 計算は (4/30) x 29 x 1 = 3.87 となります。

|**購入日**   |**課金開始** |**課金終了**  |**単価**  |**数量**  |**金額** |**請求の種類** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|2019/6/11 (2 ライセンスを所有)     |2019/6/10   |2019/7/9         |$4         |2        |$8       |新規       |
|2019/6/12     | 2019/6/10    |2019/7/9        |$4        |2        | -$7.74       |removeQuantity           |
|2019/6/12 (1 ライセンスを所有)    | 2019/6/10    |2019/7/9   |$4    |1      |$3.87    |removeQuantity |
