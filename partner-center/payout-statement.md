---
title: パートナーセンターのコマーシャル市場向けの支払い明細書
description: 支払明細書と概要、およびコマーシャルマーケットプレースの支払いデータを表示およびエクスポートする方法について説明します。
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/23/2020
ms.openlocfilehash: 34d7d162673992601267db03beaddda1573b73c0
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532057"
---
# <a name="payout-statements"></a>支払い明細

**支払い明細書** には、商用マーケットプレースを通じて販売されたプランからの支払いの概要が示されています。 収益のトランザクション履歴が表示され、次の支払いが推定され、支払いの傾向が表示されます。 トランザクション履歴と支払い明細書をダウンロードすることもできます。 この記事では、支払い明細書にアクセスする方法について説明します。また、パートナーセンターでは、さまざまな支払いページとダウンロードにアクセスできます。

## <a name="roles-and-permissions"></a>ロールとアクセス許可

支払い明細書にアクセスするには、 **アカウント所有者** または **財務共同作成者** ロールが割り当てられている必要があります。

| レポート/ページ | アカウント所有者 | Manager | Developer | 経営担当者 | 財務担当者 | マーケター |
| --- | --- | --- | --- | --- | --- | --- |
| 取得レポート (ほぼリアルタイムのデータを含む) | 表示可能 | 表示可能 | アクセス権なし | アクセス権なし | 表示可能 | アクセス権なし |
| フィードバック レポート/応答 | フィードバックの表示および送信可能 | フィードバックの表示および送信可能 | フィードバックの表示および送信可能 | アクセス権なし | アクセス権なし | フィードバックの表示および送信可能 |
| 正常性レポート (ほぼリアルタイムのデータを含む) | 表示可能 | 表示可能 | 表示可能 | 表示可能 | アクセス権なし | アクセス権なし |
| 利用状況レポート | 表示可能 | 表示可能 | 表示可能 | 表示可能 | アクセス権なし | アクセス権なし |
| 支払い受取口座 | 更新可能 | アクセス権なし | アクセス権なし | アクセス権なし | 更新可能 | アクセス権なし |
| 税プロファイル | 更新可能 | アクセス権なし | アクセス権なし | アクセス権なし | 更新可能 | アクセス権なし |
| 支払いの概要 | 表示可能 | アクセス権なし | アクセス権なし | アクセス権なし | 表示可能 | アクセス権なし |
|

## <a name="access-your-payout-statement"></a>支払い明細書にアクセスする

[パートナーセンター](https://partner.microsoft.com/dashboard/home)にサインインし、画面の右上隅にある [支払い] アイコンを選択して、次のさまざまな概要にアクセスします。

- 取引履歴
- 支払い
- データのエクスポート

:::image type="content" source="images/payouts/payout-overview.png" alt-text="パートナーセンターポータルの右上隅にある [支払い] アイコンについて説明します。":::

また、 [パートナーの支払い API](https://apidocs.microsoft.com/services/partnerpayouts) を使用して、支払いトランザクションと支払いデータを直接接続して取得することもできます。


## <a name="transaction-history"></a>取引履歴

[ **トランザクションの履歴** ] ページには、収益の概要、次回の支払いの推定、過去36か月間の収益と支払いの傾向が表示されます。 このセクションからトランザクションの詳細をダウンロードすることもできます。

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="トランザクションの概要。":::

- **今年に送信さ** れた収益-過去1か月間に支払われた収益の合計と収益の内訳。
- **推定支払月** –今後の月に予想される収益の合計。
- **収益と支払いの傾向** –過去36か月間の毎月の収益と支払い額。
- **ダウンロード** –トランザクションの詳細を .csv または .tsv 形式でダウンロードします。

ページの右上隅にある [日付範囲] 選択を使用して、過去3、6、12、または36か月を表示するページの出力をフィルター処理します。 または、36か月までのカスタムの日付範囲を選択します。 既定の日付範囲は12か月です。

:::image type="content" source="images/payouts/search-filter.png" alt-text="ページの右上にある検索フィルター。":::

### <a name="transaction-history-summary"></a>トランザクション履歴の概要

この例では、製品の販売日、状態、および支払い月の推定期間を含む、前払いの詳細が表示されます。

:::image type="content" source="images/payouts/transaction-history.png" alt-text="トランザクションの履歴。":::

- [ **獲得日** ] –購入日。
- [獲得の **種類** ] –販売、リベート、共同操作などの商品の種類。
- **合計金額** –純消費量。 商用マーケットプレースでは、これは、が standard marketplace の料金を差し引くことを意味します。
- **Status** –には次の3つのオプションがあります。
    - **今後** の利益は、保留中の冷却期間です。
    - [ **処理済み** ] –次の支払いのために収益が準備されます。
    - **送信** –収益が支払われています。
- **推定支払い月** -収益が見込まれる月。

トランザクションが支払いの適格性を満たすと、トランザクションが表示されます。 売上が不足している、または予期しない利益が生じる理由を理解するには、「 [商用 marketplace 支払いに関する一般的な質問](payout-faq.md#why-are-my-earnings-missing)」を参照してください。

### <a name="transaction-history-download"></a>取引履歴のダウンロード

詳細を表示するには、ページの上部にある [ **ダウンロード** ] を選択します。 次の表では、レポートの各列について説明します。

| 列名 | 説明 | インセンティブプログラム/マーケットプレースの適用性 |
| --- | --- | --- |
| agreementEndDate | 契約終了日 | インセンティブ - 一部のプログラムのみ |
| agreementNumber | 契約番号 | インセンティブ - 一部のプログラムのみ |
| agreementStartDate | 契約開始日 | インセンティブ - 一部のプログラムのみ |
| calculationDate | 収益がシステムで計算された日付 | All |
| claimId | 要求の一意の識別子 | インセンティブ - 一部のプログラムのみ |
| customerCountry | 顧客の国/地域 | marketplaces |
| 顧客の電子メール |  |  |
| customerName | 常に空白になります | インセンティブプログラムのみ (例外: OEM) とマーケットプレイス |
| 顧客 Tenantid |  |  |
| distributorId | ディストリビューター識別子 | インセンティブ - 一部のプログラムのみ |
| distributorName | ディストリビューター名 | インセンティブ - 一部のプログラムのみ |
| earningAmount | 元の取引通貨での収益金額 | All |
| earningAmountInLastPaymentCurrency | 前回の支払い通貨での収益金額 (前の支払いが行われていない場合、フィールドは空になります) |  |
| earningAmountUSD | 米国ドルでの収益金額 | All |
| earningDate | 収益の日付 | All |
| earningExchangeRate | 対応する米国ドル金額を示すために使用される為替レート | All |
| earningId | 各収益の一意識別子 | All |
| earningRate | 収益を生成するためにトランザクション量に適用されたインセンティブ率 | All |
| earningType | 料金、リベート、共同、販売などであるかどうかを示します | All |
| exchangeRateDate | earningAmountUSD の計算に使用される為替レートの日付 | All |
| externalReferenceId | プログラムの一意識別子 | 直接支払いプログラム (インセンティブとマーケットプレイス) |
| externalReferenceIdLabel | 一意識別子のラベル | 直接支払いプログラム (インセンティブとマーケットプレイス) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | 請求書番号 (enterprise のみに適用) | インセンティブとマーケットプレイス-一部のプログラムのみ |
| lastPaymentCurrency | 前回の支払い通貨 (前の支払いが行われていない場合、フィールドは空になります) |  |
| lever | 収益のビジネス ルールを示します | All |
| LicensingProgramName | ライセンス プログラムの名前 |  |
| LineItemId | 顧客の請求書の個別行 |  |
| localProviderSeller | レコードのローカル プロバイダー/販売者 |  |
| 成熟度月 | 見積支払い月 | すべて |
| OrderId | 顧客の請求書に関連しています  | marketplaces |
| parentProductId | 一意の親製品識別子。 取引の親製品がない場合は、親製品 ID = 製品 ID です。 | marketplaces |
| parentProductName | 親製品の名前。 取引の親製品がない場合は、親製品名 = 製品名です。 | marketplaces |
| participantId | プログラムによるパートナー収益のプライマリ ID | All |
| participantIdType | マーケットプレースの場合は、インセンティブプログラムと販売者のためのほとんどのプログラム ID | All |
| participantName | 収益パートナーの名前 | All |
| partnerCountryCode | 収益パートナーの場所/国/地域 | All |
| partNumber | 常に空白になります | いくつかのインセンティブプログラムとマーケットプレース |
| paymentId | 支払いの一意識別子。 通常、この番号は銀行取引明細書に表示されます | SAP の支払いのみ |
| paymentStatus | 支払いの状態 | All |
| paymentStatusDescription | 支払い状態のわかりやすい説明 | All |
| productId | 一意の製品識別子 | marketplaces |
| productName | 取引にリンクされている製品名 | すべて |
| productType | 製品の種類 (アプリ、アドオン、ゲームなど) | marketplaces |
| Program Code | プログラム名と共にマップする文字列 |  |
| programName | インセンティブ/ストア プログラム名 | All |
| purchaseOrderCoverageEndDate | 常に空白になります | インセンティブ プログラム - CRI |
| purchaseOrderCoverageStartDate | 常に空白になります | インセンティブ プログラム - CRI |
| purchaseOrderType | 常に空白になります | インセンティブ プログラム - CRI |
| purchaseTypeCode | 常に空白になります | インセンティブ プログラム - CRI |
| 数量 | プログラムによって異なります。 取引プログラムの課金数量を示します | All |
| 理由コード |  |  |
| resellerCountry |  |  |
| resellerId | リセラー識別子 | インセンティブ - 一部のプログラムのみ |
| resellerName | リセラー名 |  |
| SkuId | 発行中に定義される SKU ID。 1 つのプランに多数の SKU を関連付けることは可能ですが、1 つの SKU に関連付けることのできるプランは 1 つのみです。 インセンティブ - 一部のプログラムのみ |  |
| storeFee | ストアでアプリまたはアドオンを入手できるようにするための料金として、Microsoft によって保持される金額 | marketplaces |
| subscriptionEndDate | サブスクリプションの終了日 | インセンティブ - 一部のプログラムのみ |
| subscriptionId | 顧客に関連付けられたサブスクリプション識別子 | インセンティブ - 一部のプログラムのみ |
| subscriptionStartDate | サブスクリプションの開始日 | インセンティブ - 一部のプログラムのみ |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | 税の送金を担当する当事者 (消費税、使用税、または VAT/GST 税)。 | marketplaces |
| taxRemitted | 送金された税金額 (消費税、使用税、または VAT/GST 税) | marketplaces |
| taxState | 顧客の都道府県 |  |
| taxZipCode | 顧客の郵便番号 |  |
| tpan | サードパーティの広告ネットワークを示します | マーケットプレース広告のみ |
| transactionAmount | 生成された収益に基づく元の取引通貨の取引金額 | All |
| transactionAmountUSD | 米国ドルでの取引金額 | All |
| transactionCountryCode | 取引が発生した国および地域番号 |  |
| transactionCurrency | 元の顧客取引が発生した通貨 (これは、パートナー拠点の通貨ではありません) | All |
| transactionDate | 取引の日付。 多数の取引が 1 つの収益に寄与するプログラムに便利です | All |
| transactionExchangeRate | 対応する取引の米国ドルでの金額を示すために使用された為替レートの日付 | All |
| transactionId | 取引の一意識別子 | All |
| transactionPaymentMethod | 取引に使用される顧客の支払い方法 (カード、携帯電話会社の請求、または PayPal など) | marketplaces |
| transactionType | 取引の種類 (購入、返金、取消、配賦など) | marketplaces |
| ワークロード | ワークロード | インセンティブ - 一部のプログラムのみ |
|

## <a name="payments"></a>支払い

**支払い** ページには、Microsoft によって獲得された資金の詳細が表示されます。 また、どれだけの支払いが行われるかも示します。

>[!Note]
> 支払いの対象となるには、収益が $50 の[支払いしきい値](payment-thresholds-methods-timeframes.md)に達している必要があります。 詳細については、「 [Microsoft Publisher Agreement](https://go.microsoft.com/fwlink/?LinkID=699560)」を参照してください。

:::image type="content" source="images/payouts/payments-overview.png" alt-text="支払いの概要画面。":::

- **今年度の合計支払額** –すべてのプログラムについて、この年の合計を米国ドルで合計した金額。
- **次の推定支払い** : 米国ドルで、次に支払われる1回の支払い (他のものがある場合でも)。
- [ **最終支払い** ] –最新の支払いの金額 (米ドル単位)、プログラム名、およびプログラム。
- [ **支払い元** ]-過去12か月間の支払い額 (米ドル単位)、プログラムあたり。

### <a name="payments-list"></a>支払い一覧

**支払いテーブルの一覧** には、支払い済みおよび保留中の支払いが表示されます。 サービス料金の税情報を PDF 形式でダウンロードし、特定の支払いの詳細を表示できます。

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="トランザクション履歴のエクスポート":::

- **有料** –すべての支払いが正常に送信されました。 ドロップダウンメニューで年を選択して、その年にリリースされた支払にフィルターを適用します。
- **保留中** –今後の支払い。
- **サービス料金税 (PDF 形式)** : サービス料金税の対象となる支払いに使用できます。 サービス料金の税は、 **その他の税金** で示されています。
- **View** –支払いに含まれる収益の一覧を使用して、トランザクション履歴にリダイレクトします。

売上が不足している、または予期しない利益が生じる理由を理解するには、「 [商用 marketplace 支払いに関する一般的な質問](payout-faq.md#why-are-my-earnings-missing)」を参照してください。

### <a name="payment-status"></a>支払いの状態

次の表では、さまざまな収益状態について説明します。

| 収益の状態 | 理由 | パートナーによる操作の必要性 |
| --- | --- | --- |
| 未処理 | 収益は支払いの対象となります。 インセンティブプログラムの番組ガイドで定義されているように、冷却期間中はこの状態のままになります。 | いいえ |
| 予定 | 支払いが処理される前に、保留中の内部レビューが生成されました。 | いいえ |
| 保留中の税金請求書 | 税金請求書が不完全または無効です。 | 支払いを受けるには、税金請求書を更新する必要があります |
| 審査中に拒否 | 確認中に支払いが拒否されました。 | 詳細については、Microsoft サポートにお問い合わせください |
| 失敗 | Microsoft システムエラーが発生したため、支払いに失敗しました。 | 詳細については、Microsoft サポートにお問い合わせください |
| 進行中 | 支払いが進行中です。 | いいえ |
| 誤った支払い | 支払い recouping が進行中です。 | いいえ |
| 送信済み | 支払いが銀行に送信されました。 | いいえ |
| 再処理中 | Microsoft システムエラーが発生したため、支払いを再処理しています。 | いいえ |
| Reversed | お支払いは銀行によって取り消され、次回の支払いサイクルで再度送信されます。 | いいえ |
| 税金請求書の拒否 | 税金請求書が審査中に拒否されました。 すべての保留中の支払いは、税金請求書の審査が完了するまで保留されます。 | 詳細については、Microsoft サポートにお問い合わせください |
| 税金請求書の審査中 | 税金請求書を審査中です。 税金請求書が承認されると、支払いが行われます。 | いいえ |
| 拒否 | お支払いは銀行によって拒否されました。 | 詳細については、銀行にお問い合わせください。 |
|

### <a name="payments-download"></a>支払いのダウンロード

支払いの詳細を表示するには、ページの上部にある [ **ダウンロード** ] を選択します。 次の表では、レポートの各列について説明します。

| 列名 | 説明 |
| --- | --- |
| participantID | プログラムによるパートナー収益のプライマリ ID |
| participantIDType | 一般に、ストアプログラムのインセンティブプログラムと販売者 ID のプログラム ID |
| participantName | 収益パートナーの名前 |
| programName | インセンティブ/店舗プログラム名 |
| earned | 該当するプログラム/participantID の収益額 (支払先通貨単位) |
| earnedUSD | プログラム/participant ID の収益額 (米国ドル単位) |
| withheldTax | プログラム/participantID の源泉徴収税額 (支払先通貨単位) |
| salesTax | Program/participantID の [従量課金通貨] の売上税の合計金額 (インセンティブプログラムにのみ適用可能) |
| serviceFeeTax | プログラム/participantID の serviceFeeTax の合計金額 (支払先通貨単位) (ストア プログラムと Azure Marketplace にのみ適用) |
| totalPayment | 源泉徴収を除き、消費税 (該当する場合) を含めたプログラム/participantID の合計支払い額 (現地通貨単位) |
| currencyCode | 支払先通貨コード |
| paymentMethod | パートナーへの支払いに使用する方法 (銀行の電子送金、クレジット メモなど) |
| paymentID | 支払いの一意識別子。 この番号は通常、銀行取引明細書に表示されます (SAP の支払いにのみに適用)。 |
| paymentStatus | 支払いの状態 |
| paymentStatusDescription | 支払い状態のわかりやすい説明 |
| paymentDate | Microsoft から支払いが送信された日付 |
|

## <a name="export-data"></a>データのエクスポート

[ **データのエクスポート** ] ページは、それ自体では更新されません。 最新のデータを表示するために、ページを手動で更新しなければならない場合があります。 3つのタブから選択して、 **トランザクション履歴** 、 **支払い** 、 **トランザクションの概要** 、または過去の **ステートメント** のいずれかをエクスポートします。

フィルターを使用すると、 **データが使用できない** というエラーが発生する可能性があります。 これは、既定の期間を3か月で選択したままにしてから、その期間外の前払いの支払い ID を選択した場合に発生する可能性があります。 この問題が発生した場合は、期間を拡大して、もう一度やり直してください。

支払いの輸出例を次に示します。

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="支払いレポートをエクスポートします。":::

### <a name="historical-statements"></a>履歴明細書

また、[ **データのエクスポート** ] 概要では、履歴ステートメントにアクセスすることもできます。

> [!NOTE]
> 履歴ステートメントはスナップショットであり、更新されません。 必要に応じて、 [サポート](https://partner.microsoft.com/support/v2/?stage=1) に連絡し、最新のデータを要求してください。

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="履歴ステートメントをエクスポートします。":::

- 2019年7月1日より前のトランザクション履歴は個別に処理され、後の履歴レポートとは異なるフィールドを使用します。
- 従来のトランザクション履歴には、"予約済み" という名前の列があります。これは、最新の履歴の "収益" 列に対応しています。ただし、状態が "支払い送信済み" に等しいすべての利益が除外される点が異なります。
- 3M、6M、または 12M などのフィルターは、履歴明細書セクションには適用されません。

### <a name="historical-statement-downloads"></a>ステートメントのダウンロード履歴

次の表では、履歴ステートメントの各列について説明します。

| フィールド名 | 説明 |
| --- | --- |
| Revenue Source (収益源) | 取引の発生場所 (Microsoft Store、Windows Phone Store、Windows Store 8、または広告など) に基づく収益のソース |
| 注文 ID | 一意の注文識別子。 この ID を使用すると、購入取引を、それぞれの非購入取引 (返金や配賦など) と共に識別できます。 両方で同じ注文 ID が使用されます。 また、1回の購入に複数の支払い方法が使用されている分割料金がある場合は、注文トランザクションをリンクすることができます。 |
| Transaction ID | 一意の取引識別子。 |
| Transaction Date Time (取引日時) | 取引が発生した日時 (UTC)。 |
| Parent Product ID (親製品 ID) | 一意の親製品識別子。 取引の親製品がない場合は、親製品 ID = 製品 ID です。 |
| Product ID | 一意の製品識別子。 |
| Parent Product Name (親製品名) | 親製品の名前。 取引の親製品がない場合は、親製品名 = 製品名です。 |
| 製品名 | 製品の名前 |
| Product Type (製品の種類) | 製品の種類 (アプリ、アドオン、ゲームなど) |
| Quantity | 収益源がビジネス向け Microsoft Store の場合、[Quantity]\(数量\) は、購入ライセンス数を表します。 その他のすべての収益源については、数量は常に 1 になります。 2 つの異なる支払い方法が使用されたために 1 つの取引が 2 つの品目に分割されている場合でも、各品目には数量 1 が表示されます。 |
| トランザクションの種類 | 取引の種類 (購入、返金、取消、配賦など) |
| Payment Method (支払方法) | 取引に使用される顧客の支払い方法 (カード、携帯電話会社の請求、または PayPal など) |
| Country / Region (国/地域) | 取引が発生した国/地域 |
| Local Provider / Seller (ローカル プロバイダー/販売者) | レコードのローカル プロバイダー/販売者 |
| Transaction Currency (取引通貨) | 取引の通貨 |
| Transaction Amount (取引額) | 取引の金額 |
| 送金された税額 | 送金された税金額 (消費税、使用税、または VAT/GST 税) |
| Net Receipts (純収益) | 送金された税金を引いた取引額 |
| ストア料金 | ストアでアプリまたはアドオンを利用できるようにするための料金として、Microsoft によって保持される純収益の割合 (パーセンテージ)。 |
| App Proceeds (アプリの収益) | 純収益からストア料金を引いたもの |
| Taxes Withheld (源泉徴収税) | 源泉所得税額 ( **Reserved (予約)** CSV ファイルには含まれません) |
| 支払い | アプリの収益から、該当するすべての源泉所得税を引いたもの (金額は取引通貨で表示)。 **Reserved (予約)** CSV ファイルには含まれません。 |
| FX Rate (FX レート) | 取引通貨を支払い通貨に変換するために使用される外国為替レート |
| Payment Currency (支払い通貨) | 支払いを行う通貨 |
| Converted Payment (換算された支払い額) | FX レートを使用して支払い通貨に換算された支払い額 |
| Tax Remit Model (税金の送金モデル) | 税の送金を担当する当事者 (消費税、使用税、または VAT/GST 税)。 |
| Eligibility Date Time (適格日時) | 取引の収益が支払い適格になる日時 (UTC)。 支払いが作成されるときに、支払いの作成日より前の適格日時を含む取引収益が含まれます ( **Reserved (予約)** CSV ファイルにのみ含まれます)。 |
| Charges | [Transaction Amount]\(取引額\) 列で集計されているすべての料金詳細の明細が表示されます (含まれる対象は Azure Marketplace のみになります。 **Reserved (予約)** CSV ファイルには含まれません)。 |
|||

## <a name="next-steps"></a>次の手順

- [パートナー支払い API](https://apidocs.microsoft.com/services/partnerpayouts)
- [支払いポリシーの詳細](payout-policy-details.md)
- 課金サポートについては、コマーシャル マーケットプレースの[発行元のサポート](https://partner.microsoft.com/support/v2/?stage=1)にお問い合わせください。