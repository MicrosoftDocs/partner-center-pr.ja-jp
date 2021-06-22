---
title: 調整ファイルを使用する
ms.topic: article
ms.date: 03/26/2021
description: パートナーセンターでの調整ファイルと、特定の請求サイクルにおける料金の詳細な行項目ビューを解釈する方法について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431571"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>パートナーセンターの調整ファイルの品目を読み取る方法について説明します。

**適切なロール**: Billing admin |全体管理者

パートナーセンターから調整ファイルをダウンロードして、請求サイクルの各料金の詳細な行項目ビューをダウンロードできます。 行項目の詳細には、各顧客のサブスクリプションの料金と詳細なイベント (サブスクリプションへのライセンスの長期追加など) が含まれます。

**請求書** を読む方法の詳細については、「請求書の [読み取り](read-your-bill.md)」を参照してください。

## <a name="understand-reconciliation-file-fields"></a>調整ファイルのフィールドについて

- [ライセンス ベースの調整ファイルのフィールド](license-based-recon-files.md)
- [使用量ベースの調整ファイルのフィールド](usage-based-recon-files.md)
- [毎日評価される使用状況調整ファイルのフィールド](daily-rated-usage-recon-files.md)
- [1回限りの購入 CSP 調整ファイルのフィールド](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>調整ファイルの料金の種類について

調整ファイル ( **ChargeType** 列) の料金の種類については、「 [調整ファイルの料金の種類](recon-file-charge-types.md)」を参照してください。

## <a name="fix-formatting-issues"></a>書式設定の問題の修正

場合によっては、調整ファイルに書式設定の問題が含まれていることがあります。 たとえば、en-us ロケールが使用されていない場合に、この問題が発生する可能性があります。

調整ファイルの書式設定に関する問題を修正するには、次の手順に従います。

1. Microsoft Excel で調整ファイル (.csv 形式) を開きます。
2. ファイルの最初の列を選択します。
3. **テキストを列に変換ウィザード** を開きます。 リボンで、[ **データ**] を選択し、[ **列のテキスト**] を選択します。
4. ウィザードで、[区切られた **ファイルの種類**] を選択します。 次に、 **[次へ]** を選択します。
5. [ **区切り記号** ] ボックスで、[ **コンマ**] を選択します。 ( **タブ** が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、[ **次へ**] を選択します。
6. [ **列のデータ形式** ] フィールドで、[ **Date: MDY**] を選択します。 次に、 **[次へ]** を選択します。
7. [ **列のデータ形式** ] フィールドで、[すべての金額列] の **テキスト** を選択します。 次に、 **[Finish]\(完了\)** を選択します。

## <a name="download-reconciliation-files-programmatically"></a>プログラムによる調整ファイルのダウンロード

調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。 プログラムによって調整ファイルをダウンロードするには、「 [請求書の品目を取得](/partner-center/develop/get-invoiceline-items)する」を参照してください。

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>ファイルが Excel の行の制限を超えている場合

調整ファイルをダウンロードできても Microsoft Excel で開くことができない場合は、Excel で許可されているよりも多くの行がファイルに含まれていることを意味します。 この問題が発生した場合は、次のいずれかの手順を使用してファイルを開くことができます。

### <a name="open-a-recon-file-in-power-bi"></a>Power BI で偵察ファイルを開きます。

1. 通常どおりに調整ファイルをダウンロードします。
2. Microsoft Power BI のインスタンスをダウンロードし、インストールして開きます。
3. Power BI **ホーム** ] タブで、[ **データの取得**] を選択します。
4. **共通データソース** の一覧で、[ **Text/CSV**] を選択します。
5. メッセージが表示されたら、偵察ファイルを開きます。

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Excel ピボットテーブルで偵察ファイルを開く

1. 通常どおりに調整ファイルをダウンロードします。
2. Microsoft Excel で新しいファイルを開きます。
3. [ **データ** ] タブで [ **データの取得**] を選択し、[ **ファイルから**] を選択して、[ **Text/CSV**] を選択します。
4. メッセージが表示されたら、偵察ファイルを開きます。 データが表示されます。
5. [ **読み込み** ] ドロップダウンメニューで [ **読み込み先**] を選択し、[ **OK]** を選択します。
6. [ **データのインポート** ] ダイアログボックスで、[ **PivotTable レポート** ] を選択してファイルを開きます。

## <a name="negative-amount-displayed"></a>負の値が表示されます

調整ファイルに負の値が表示される場合があります。 おそらく、これは次のいずれかが原因で起こります。

- 最近取り消したか、ライセンス数を減らしました
- サービスライセンス契約 (SLA) または Azure の使用量のクレジットを受け取りました

このトランザクションの詳細情報を取得するには、調整ファイルでその料金の種類の属性を確認します。

## <a name="map-taxes-or-vat"></a>税または VAT をマップする

税金または付加価値税 (VAT) を請求書にマッピングするには、次のようにします。

- ライセンスベースのファイルから **税** 列を合計します。
- 使用状況に基づくファイルから **taxationitem.taxamount** 列を合計します。

## <a name="itemize-reconciliation-files-by-partner"></a>パートナー別の調整ファイルの明細

**間接モデル** のパートナーは、これらの追加フィールドをライセンスベースと使用状況に基づく調整ファイルの両方で使用して、リセラーごとにファイルを作成することができます。

| MPN ID | 説明 |
| ------ | ----------- |
| MPN ID | クラウドソリューションプロバイダー (CSP) パートナー (直接または間接) の Microsoft Partner Network (MPN) 識別子。 |
| [リセラーの MPN ID](#reseller-mpn-id) | [サブスクリプションの販売店の MPN 識別子](#reseller-mpn-id)。 このフィールドは、パートナーセンターの特定のサブスクリプションについて一覧表示されているリセラー ID に対応しています。 インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。 |

### <a name="reseller-mpn-id"></a>リセラーの MPN ID

CSP パートナーが顧客にサブスクリプションを直接販売した場合、 **MPN id** と **再販業者の MPN id** の両方として、 **MPN id** が2回表示されます。

CSP パートナーが **MPN id** のない再販業者を持っている場合、この値は代わりにパートナーの **MPN id** に設定されます。

CSP パートナーが **リセラーの MPN ID** を削除した場合、この値は *-1* に設定されます。

**リセラー MPN ID** を表示または更新するには:

1. パートナー センターにサインインします。
2. パートナー センター メニューで、**[顧客]** を選びます。
3. 一覧から顧客を選択します。
4. カスタマーメニューで、[ **サブスクリプション**] を選択します。
5. 一覧からサブスクリプションを選択します。
6. **[更新]** を選んで、**[再販業者 (MPN ID)]** を変更します。

## <a name="next-steps"></a>次の手順

- [請求書 & 偵察ファイルを読み取る方法](read-your-bill.md) 