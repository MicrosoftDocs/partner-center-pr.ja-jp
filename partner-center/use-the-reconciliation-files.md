---
title: 調整ファイルを使用する |パートナーセンター
ms.topic: article
ms.date: 11/21/2019
description: 調整ファイルを使用して、パートナーセンターの料金の詳細な行項目ビューを把握します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340220"
---
# <a name="use-your-reconciliation-files"></a>調整ファイルを使用する

適用対象

- Partner Center
- 米国政府機関向け Microsoft Cloud のパートナー センター

パートナーセンターから調整ファイルをダウンロードして、請求サイクルの各料金の詳細な行項目ビューをダウンロードできます。 行項目の詳細には、各顧客のサブスクリプションの料金と詳細なイベント (サブスクリプションへの接続クライアントの追加など) が含まれます。

適切なロール:

- 課金の管理
- 全体管理者

**請求書**を読む方法の詳細については、「請求書の[読み取り](read-your-bill.md)」を参照してください。

## <a name="understand-reconciliation-file-fields"></a>調整ファイルのフィールドについて

- [ライセンスベースの調整ファイルのフィールド](license-based-recon-files.md)
- [使用法に基づく調整ファイルのフィールド](usage-based-recon-files.md)
- [1回限りの定期的な調整ファイルのフィールド](one-time-recurring-recon-files.md)
- [日単位で評価した使用状況の調整ファイルのフィールド](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>調整ファイルの料金の種類について

調整ファイル ( **ChargeType**列) の料金の種類については、「[調整ファイルの料金の種類](recon-file-charge-types.md)」を参照してください。

## <a name="fix-formatting-issues"></a>書式設定の問題の修正

場合によっては、調整ファイルに書式設定の問題が含まれていることがあります。 たとえば、en-us ロケールが使用されていない場合に、この問題が発生する可能性があります。

調整ファイルの書式設定に関する問題を修正するには、次の手順に従います。

1. Microsoft Excel で調整ファイル (.csv 形式) を開きます。
2. ファイルの最初の列を選択します。
3. **テキストを列に変換ウィザード**を開きます。 リボンで、 **[データ]** を選択し、 **[列のテキスト]** を選択します。
4. ウィザードで、[区切られた**ファイルの種類**] を選択します。 次に、 **[次へ]** を選択します。
5. **[区切り記号]** ボックスで、 **[コンマ]** を選択します。 (**タブ**が既に選択されている場合は、このオプションを選択したままにしておくことができます)。次に、 **[次へ]** を選択します。
6. **[列のデータ形式]** フィールドで、 **[Date: MDY]** を選択します。 次に、 **[次へ]** を選択します。
7. **列のデータ形式** フィールドで、すべての金額列 の**テキスト**を選択します。 次に、 **[完了]** を選択します。

## <a name="download-reconciliation-files-programmatically"></a>プログラムによる調整ファイルのダウンロード

調整ファイルは非常に大きくなる可能性があり、ダウンロードが困難な場合があります。 プログラムによって調整ファイルをダウンロードするには、「[請求書の品目を取得](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items)する」を参照してください。

## <a name="map-taxes-or-vat"></a>税または VAT をマップする

税金または付加価値税 (VAT) を請求書にマッピングするには、次のようにします。

- ライセンスベースのファイルから**税**列を合計します。
- 使用状況に基づくファイルから**taxationitem.taxamount**列を合計します。

## <a name="itemize-reconciliation-files-by-partner"></a>パートナー別の調整ファイルの明細

**間接モデル**のパートナーは、これらの追加フィールドをライセンスベースと使用状況に基づく調整ファイルの両方で使用して、リセラーごとにファイルを作成することができます。

| MPN ID | 説明 |
| ------ | ----------- |
| MPN ID | クラウドソリューションプロバイダー (CSP) パートナー (直接または間接) の Microsoft Partner Network (MPN) 識別子。 |
| [再販業者の MPN ID](#reseller-mpn-id) | [サブスクリプションの販売店の MPN 識別子](#reseller-mpn-id)。 このフィールドは、パートナーセンターの特定のサブスクリプションについて一覧表示されているリセラー ID に対応しています。 インダイレクト モデルのパートナーの調整ファイルにのみ表示されます。 |

### <a name="reseller-mpn-id"></a>リセラーの MPN ID

CSP パートナーが顧客にサブスクリプションを直接販売した場合、 **MPN id**と**再販業者の MPN id**の両方として、 **MPN id**が2回表示されます。

CSP パートナーが**MPN id**のない再販業者を持っている場合、この値は代わりにパートナーの**MPN id**に設定されます。

CSP パートナーが**リセラーの MPN ID**を削除した場合、この値は *-1*に設定されます。

**リセラー MPN ID**を表示または更新するには:

1. パートナー センターにサインインします。
2. パートナー センター メニューで、 **[顧客]** を選びます。
3. 一覧から顧客を選びます。
4. カスタマーメニューで、 **[サブスクリプション]** を選択します。
5. 一覧からサブスクリプションを選択します。
6. **[更新]** を選んで、 **[再販業者 (MPN ID)]** を変更します。
