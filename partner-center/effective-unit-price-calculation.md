---
title: 有効な単価計算
ms.topic: how-to
ms.date: 04/02/2021
description: 有効な単価とその計算方法について説明します。 この記事には、サンプル計算も含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172219"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Azure プランの使用の有効な単価計算

**適切なロール**

- 課金管理者

## <a name="the-effective-unit-price"></a>有効な単価

有効な単価は、(リソースレベルではなく) メーターレベルで計算され、メーターの使用状況に応じて毎日調整されます。

次の3つの要素を使用して、有効な単価を計算します。

- 使用量 (請求サイクル全体で毎日監視されます)
- メーターの課金対象コスト
- 階層化 (該当する場合)

請求サイクル全体にわたって使用量を毎日監視するため、有効な単価が変動します。 特定の請求サイクルの最終的な価格は、使用量の計算を停止し、請求期間を終了した後に利用可能になります。 ほとんどの変更は、4番目または5番目の小数点以下に表示されます。

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>メーターが階層化された価格を使用するかどうかを確認する

メーターが階層化された価格を使用しているかどうかわからない場合は、以下の手順を使用して確認してください。 

1. [パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。
2. [ **販売**] を選択し、[ **価格とオファー**] を選択して、[ **Azure プランの価格**] を選択します。
3. ID でメーターを見つけ、価格データをダウンロードします。 

## <a name="sample-calculation"></a>サンプル計算

次の表は、オープン期間中の有効な単価を計算する方法の例を示しています。

この表では、次の値が適用されます。 

- **UP** = リソースの単価/時間 = 0.868

- **Bcu** = 測定用の課金対象の消費単位

- **BC** = メーターの課金対象コスト = BCU * アップ * 0.85。 これは、15% の PEC 割引の調整を反映しています。 次に、関数の下限を使用して、最小金額を請求するために、小数点の後の2桁に値を制限します。 

- **有効な単価** = bcu/BC

>[!NOTE]

>注: この例のメーターには、価格またはその他の割引のレベルはありません。割引率とその他の調整における有効な単価の係数です。


| Date | BCU (課金対象の使用量単位) | BC (請求可能なコスト) | 有効な単価 |
| ------ | ----------- | ----------- | ----------- |  
| 3-8 月 | 29 | 21.39 | 0.737586206896552 |
| 10 ~ 8 月 | 210.950039 | 155.63 | 0.737757626107858 |
| 25 ~ 8 月 | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>次のステップ

- [請求と税金](billing.md)
