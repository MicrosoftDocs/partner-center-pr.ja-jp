---
title: 請求書を読み取る | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 請求書は、当月のすべての (プログラム、製品、顧客全体の) 料金の概要です。 これは、パートナー センターで利用できます。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: サブスクリプションの請求, 請求, パートナー センターでの請求, パートナー センターの請求, 請求書の記載事項, 請求書, パートナー センターの請求書, CSP 請求書, 請求書の場所
ms.localizationpriority: medium
ms.openlocfilehash: 8505e0cc42bd294f6c6645ed02c1c5529cffff54
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795695"
---
# <a name="read-your-bill"></a>請求書の記載事項

**適用対象**

-  パートナー センター
-  米国政府機関向け Microsoft Cloud のパートナー センター
-  Microsoft Cloud ドイツのパートナー センター

請求書の**パートナー センター**メニューに移動します選び、**請求**に請求の履歴と傾向、請求書と調整ファイルの場合は、前回のお支払いへのリンクを参照してください。

クラウド ソリューション プロバイダー プログラムに参加中で月次請求を選択した場合は、顧客 (ライセンスベースおよび使用量ベース) のサブスクリプション料金を 60 日以内に Microsoft にお支払いください。

> [!NOTE]  
> 請求書は、当月のすべての料金 (プログラム、製品、顧客の料金) の要約が記載されたものであり、指定の請求日から 4 日以内に表示可能になります。

ライセンス ベース (Office365) と (Azure) 料金の使用量ベースの 1 つの請求書と 1 回限り (Azure reserved VM instances の) 別の請求書を受け取ったら料金。

料金の項目別明細については、関連する調整ファイルを使用します。 調整ファイルには、顧客への請求書の作成に使用される顧客 ID とサブスクリプション ID が含まれます。 詳しくは、「[調整ファイルの使用方法](use-the-reconciliation-files.md)」をご覧ください。

## <a name="invoice-file-definitions"></a>請求書ファイルの定義


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>フィールド</strong></td>
<td><strong>説明</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>連邦税の ID 番号。</td>
</tr>
<tr class="odd">
<td>顧客番号</td>
<td>お客様の番号。</td>
</tr>
<tr class="even">
<td>請求先</td>
<td>請求書の送付先となる住所。 この住所を変更するには、[アカウント設定] > [パートナー課金プロファイル] に移動します。 </td>
</tr>
<tr class="odd">
<td>ライセンス ベースの課金</td>
<td>購入した使用量ベースのライセンスに対する定額の月額 (または年額) 料金で、サービスの前に課金されます。 この数値は、ライセンスベースの調整ファイルの &quot;Subtotal&quot; 列 (T 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="even">
<td>使用量ベースの課金</td>
<td>請求月の間に有効にした、または使用された Azure の利用料金 (新しいサービスやアプリケーションが含まれます)。 この数値は、使用量ベースの調整ファイルの &quot;PretaxCharges&quot; 列 (Z 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="odd">
<td>割引</td>
<td>たとえば、サブスクリプションの通常価格に対してお客様が受け取る割引です。 これは単価やライセンスではなく、定額で表示されます。</td>
</tr>
<tr class="odd">
<td>クレジット</td>
<td>サブスクリプションに加えられた変更内容 (シートの増減など) に対するクレジットまたは調整の金額。</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>税金と税金排他的料金とクレジット前に、の合計です。</td>
</tr>
<td>税金</td>
<td>請求書の 2 ページ目から始まる明細セクションに示される、現在の合計料金に対する税金の合計。 この数値は、以下の列にあるすべての料金の合計です。
<ul>
<li>使用量ベースの調整ファイルの &quot;TaxAmount&quot; 列 (AA 列)、および</li>
<li>ライセンス ベースのファイルの &quot;Tax&quot; 列 (U 列)。</li>
</ul></td>
</tr>
<tr class="odd">
<td>その他のクレジット</td>
<td>税排他的クレジット。</td>
</tr>
<tr class="even">
<td>当月の請求額合計</td>
<td>支払い期限ごとの、請求期間の請求通貨での支払い額。</td>
</tr>
<tr class="odd">
<td>お支払いについて</td>
<td>地域に基づく、請求書の支払い方法の説明です。 支払いを行うときには、常に請求書番号を含めます。</td>
</tr>
<tr class="even">
<td>請求書番号</td>
<td>請求書の番号。</td>
</tr>
<tr class="odd">
<td>課金期間</td>
<td>CSP パートナー様は、月 1 回または年 1 回請求されます。</td>
</tr>
<tr class="even">
<td>請求書作成日</td>
<td>請求書を受け取る日付。</td>
</tr>
<tr class="odd">
<td>支払条件</td>
<td>1 回限りの購入の場合は、常に 60 日間になります。</td>
</tr>
<tr class="even">
<td>支払期日</td>
<td>この日付までに、お客様からの支払いが受領される必要があります。</td>
</tr>
<tr class="odd">
<td>顧客 PO</td>
<td>お客様の注文書番号です。</td>
</tr>
<tr class="even">
<td>カスタマー サービス</td>
<td>カスタマー サービスにアクセスするための Web サイトのアドレス。</td>
</tr>
<tr class="odd">
<td>サービス利用者</td>
<td>サービスが使われる住所。 (これは、会社の審査に関連付けられている会社の正式な住所です。変更することはできません。)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>1 回限りの料金の項目一覧

|**フィールド** |**説明**|
|:----------------|:-----------------------------|
|日付 |購入日。 |
|説明 |製品名。 |
|数量 |購入した製品 (予約など) の数。 |
|単価 |製品 (予約など) ごとの価格。 |
|割引 |適用される割引。 |
|税抜き額 |課税前の購入額の小計。 |
|売上税 |税額。 |
|合計 |お支払いの合計額。 |
 



