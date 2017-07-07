---
title: "請求書の記載事項 | パートナー センター"
description: "請求書には、当月のすべての料金 (プログラム、製品、顧客の料金) の要約が記載されます。 請求書は、パートナー センターのダッシュボードで利用できます。"
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 65c3777c0bd35933f2622fc0de105c051001974e
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2017
---
# <a name="read-your-bill"></a>請求書の記載事項

**適用対象**

-  パートナー センター
-  米国政府機関向け Microsoft Cloud のパートナー センター
-  Microsoft Cloud ドイツのパートナー センター

請求書には、当月のすべての料金 (プログラム、製品、顧客の料金) の要約が記載されます。 請求書は、パートナー センターのダッシュボードで利用できます。

料金の項目別明細については、関連する調整ファイルを使用します。 調整ファイルには、顧客への請求書の作成に使用される顧客 ID とサブスクリプション ID が含まれます。 詳しくは、「[調整ファイルの使用](use-the-reconciliation-files.md)」をご覧ください。

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
<td>請求書の送付先となる住所。 この住所を変更するには、パートナー センターのアカウント プロファイルを編集します。</td>
</tr>
<tr class="odd">
<td>当月サービス利用料金</td>
<td>購入した使用量ベースのライセンスに対する定額の月額 (または年額) 料金で、サービスの前に課金されます。 この数値は、ライセンスベースの調整ファイルの &quot;Subtotal&quot; 列 (T 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="even">
<td>利用料金</td>
<td>請求月の間に有効にした、または使用された Azure の利用料金 (新しいサービスやアプリケーションが含まれます)。 この数値は、使用量ベースの調整ファイルの &quot;PretaxCharges&quot; 列 (Z 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="odd">
<td>調整額</td>
<td>サブスクリプションに加えられた変更内容 (シートの増減など) に対するクレジットまたは調整の金額。</td>
</tr>
<tr class="even">
<td>その他の割引</td>
<td>たとえば、サブスクリプションの通常価格に対してお客様が受け取る割引です。 これは単価やライセンスではなく、定額で表示されます。</td>
</tr>
<tr class="odd">
<td>税</td>
<td>請求書の 2 ページ目から始まる明細セクションに示される、現在の合計料金に対する税金の合計。 この数値は、以下の列にあるすべての料金の合計です。
<ul>
<li>使用量ベースの調整ファイルの &quot;TaxAmount&quot; 列 (AA 列)、および</li>
<li>ライセンスベースのファイルの &quot;Tax&quot; 列 (U 列)。</li>
</ul></td>
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
<td>支払期日</td>
<td>この日付までに、お客様からの支払いが受領される必要があります。</td>
</tr>
<tr class="even">
<td>顧客 PO</td>
<td>お客様の注文書番号です。</td>
</tr>
<tr class="odd">
<td>カスタマー サービス</td>
<td>カスタマー サービスにアクセスするための Web サイトのアドレス。</td>
</tr>
<tr class="even">
<td>サービス利用者</td>
<td>サービスが使われる住所。 (これは、会社の審査に関連付けられている会社の正式な住所です。変更することはできません)。</td>
</tr>
</tbody>
</table>

 

 

 



