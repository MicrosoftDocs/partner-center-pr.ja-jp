---
title: デジタル署名機能
ms.topic: how-to
ms.date: 07/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: インドのパートナーセンターパートナーがデジタル署名された請求書を表示し、パートナーセンターで作成された注文の請求書のデジタルコピーを受信する方法について説明します。
author: keramp
ms.author: keramp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b0d8a560c048f1a1dbb783560cf419145754a6fe
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284300"
---
# <a name="view-digitally-signed-invoices"></a>デジタル署名された請求書の表示

**適用対象**

- インドのパートナーセンター

**適切なロール**

- アカウント管理者
- 課金エージェント
- 販売代理店

インドのパートナーは、Microsoft がデジタル署名した請求書を持っていることがわかりました。 署名を表示するには、Adobe Acrobat Reader ドキュメントクラウド (DC) を使用する必要があります。

## <a name="how-to-view-and-insure-a-valid-digital-signature"></a>有効なデジタル署名を表示して保証する方法


1. パートナーセンターで注文を作成した場合は、電子メールで請求書のデジタルコピーを受け取ることになります。 Adobe Acrobat Reader DC 内から開く請求書を選択します。


2. 請求書の上部には、署名されていて、 **すべての署名が有効** であることが必要です。
 
 :::image type="content" source="images/digitalsig/digital1.png" alt-text="有効な署名通知バナー付きのサンプル請求書。緑色のチェックマークと語句、署名済み、すべての署名が有効です。":::

3. 署名を選択します。 有効性を示す証明書が表示されます。

:::image type="content" source="images/digitalsig/digital2.png" alt-text="[承認された署名者] フィールドと [署名検証の状態] ダイアログボックスの [詳細]、[署名のプロパティ] オプション、[キャンセル] オプションを使用した署名付き請求書。"::: 

4. 署名の **プロパティ** を選択すると、署名の有効性に関する詳細が表示されます。

:::image type="content" source="images/digitalsig/digital4.png" alt-text="署名プロパティの詳細ビューには、だれが、ドキュメントが署名された日時、検証プロセス、署名者の証明書に関する情報が表示されます。"::: 

4. また、証明書のパスが正しいことと、証明書が信頼されていることを確認することもできます。

 :::image type="content" source="images/digitalsig/digital3.png" alt-text="[証明書ビューアー] ダイアログボックスには、証明書とその発行チェーン全体に関する詳細情報を含むタブがいくつか表示されます。":::

### <a name="additional-information-on-invoices-and-digital-signatures"></a>請求書とデジタル署名に関する追加情報

パートナーセンターで注文を作成したユーザーにデジタルコピーが送信されます。 2020年7月17日より前に発行された請求書に対して、デジタル署名付きの請求書を取得することはできません。 また、手動で署名した請求書は使用できません。

## <a name="next-steps"></a>次のステップ

- [一般的な課金シナリオ](common-billing-scenarios.md)