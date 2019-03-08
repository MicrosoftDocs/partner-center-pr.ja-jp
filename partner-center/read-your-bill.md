---
title: 請求書の記載事項 | パートナー センター
ms.topic: article
ms.date: 10/29/2018
description: 請求書は、当月のすべての (プログラム、製品、顧客全体の) 料金の概要です。 パートナー センターで使用可能なです。
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: サブスクリプションの請求, 請求, パートナー センターでの請求, パートナー センターの請求, 請求書の記載事項, 請求書, パートナー センターの請求書, CSP 請求書, 請求書の場所
ms.localizationpriority: medium
ms.openlocfilehash: aec344eb7e4ed6e0a4d5e7e506c9bcf195654293
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584545"
---
# <a name="read-your-bill"></a>請求書の記載事項

**適用対象**

-  パートナー センター
-  米国政府機関向け Microsoft Cloud のパートナー センター


請求書を参照してください、**パートナー センター**メニューから選択し、**課金**最新支払い、請求書と調整ファイルへのリンクを請求履歴と傾向を表示します。

クラウド ソリューション プロバイダー プログラムに参加中で月次請求を選択した場合は、顧客 (ライセンスベースおよび使用量ベース) のサブスクリプション料金を 60 日以内に Microsoft にお支払いください。

> [!NOTE]  
> 請求書は--プログラム、製品、および顧客--間での現在の請求期間のすべての料金の概要を示しますされは UTC 時刻で、選択した請求日の 2 つ (2) 日以内に使用できます。 たとえば、年 9 月 12日請求日がある場合、請求書の生成処理が、13 の 12時 00分 AM UTC から開始され、14th の 12時 00分 AM UTC で完了します。 15 日に 11時 59分 PM UTC で請求書が表示されない場合は、サービス レベル契約からし、サービス要求を提出する必要があります。 

ライセンス ベース (Office 365) と使用量ベース (Azure) の料金については 1 つの請求書を受け取り、1 回限り (Azure Reserved VM Instances) の料金については別の請求書を受け取ります。

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
<td>請求書の送付先となる住所。 会社名またはアドレスを変更するには、請求プロファイル、パートナー センターを編集します。 </td>
</tr>
<tr class="odd">
<td>ライセンスベースの料金</td>
<td>購入した使用量ベースのライセンスに対する定額の月額 (または年額) 料金で、サービスの前に課金されます。 この数値は、ライセンスベースの調整ファイルの &quot;Subtotal&quot; 列 (T 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="even">
<td>使用量ベースの料金</td>
<td>請求月の間に有効にした、または使用された Azure の利用料金 (新しいサービスやアプリケーションが含まれます)。 この数値は、使用量ベースの調整ファイルの &quot;PretaxCharges&quot; 列 (Z 列) にあるすべての料金の合計です。</td>
</tr>
<tr class="odd">
<td>割引</td>
<td>たとえば、サブスクリプションの通常価格に対してお客様が受け取る割引です。 これは単価やライセンスではなく、定額で表示されます。</td>
</tr>
<tr class="odd">
<td>クレジット</td>
<td>サブスクリプションに対して行われた変更のクレジットまたは調整 (例: シートの増減)。</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>課税前の税抜き料金とクレジットの合計。</td>
</tr>
<td>Tax</td>
<td>請求書の 2 ページ目で始まる明細セクションの、現在の合計料金に対する税金の合計。 この数値は、以下の列にあるすべての料金の合計です。
<ul>
<li>使用量ベースの調整ファイルの &quot;TaxAmount&quot; 列 (AA 列)、および</li>
<li>ライセンスベースのファイルの &quot;Tax&quot; 列 (U 列)。</li>
</ul></td>
</tr>
<tr class="odd">
<td>その他のクレジット</td>
<td>税抜きクレジット。</td>
</tr>
<tr class="even">
<td>当月の請求額合計</td>
<td>支払い期限ごとの、請求期間の請求通貨での支払い額。</td>
</tr>
<tr class="odd">
<td>支払い方法</td>
<td>地域に基づく、請求書の支払い方法の説明です。 支払いを行うときには、常に請求書番号を含めます。</td>
</tr>
<tr class="even">
<td>請求書番号</td>
<td>請求書の番号。</td>
</tr>
<tr class="odd">
<td>課金期間</td>
<td>請求日に至るまで月単位の期間。 これは、期間を使用量ベースのサービスを使用し、ライセンス ベースのサービスがのライセンス数の変更やクレジット調整調整されています。</td>
</tr>
<tr class="even">
<td>請求書作成日</td>
<td>請求日または契約応当日の請求書が生成される 1 か月あたり、します。</td>
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
<td>サービスが使われる住所。 (これは、会社の審査に関連付けられている有効な会社のアドレスです)。</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>1 回限りの料金の項目一覧

|**フィールド** |**定義**|
|:----------------|:-----------------------------|
|日付 |購入日。 |
|説明 |製品名。 |
|数量 |購入した製品 (予約など) の数。 |
|単価 |製品 (予約など) ごとの価格。 |
|割引 |適用される割引。 |
|税抜き額 |課税前の購入額の小計。 |
|売上税 |税額。 |
|Total |お支払いの合計額。 |
 



