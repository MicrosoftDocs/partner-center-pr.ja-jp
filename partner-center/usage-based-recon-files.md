---
title: 使用法に基づく調整ファイル |パートナーセンター
ms.topic: article
ms.date: 01/08/2020
description: 使用状況に基づく調整ファイルのすべての項目について、例を挙げて説明します。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d0b50240ec62f10a202c3ad0de3d6425aec878ef
ms.sourcegitcommit: fe1f2730a14ec394caccdbb59b00ef5908acaa29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/09/2020
ms.locfileid: "75757225"
---
# <a name="usage-based-file-fields"></a>使用量ベースのファイルのフィールド

適用先:

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

顧客の使用量に対して料金を調整するには、 **ResellerID**、 **ResellerName**、および**ResellerBillableAccount**を調整ファイルから、パートナーセンターの**顧客名**と**サブスクリプション ID**に比較します。

## <a name="fields-in-usage-based-reconciliation-files"></a>使用法に基づく調整ファイルのフィールド

次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。

| Column | 説明 | サンプル値 |
| ------ | ----------- | ------------ |
| PartnerId | GUID 形式のパートナー識別子。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | パートナー名。 | *Contoso, Ltd.* |
| Partnerの Lableaccountid | パートナーアカウント識別子。 | *1010578050* |
| CustomerCompanyName | パートナー センターで報告される顧客の組織名。 *請求書をシステム情報と調整するために非常に重要です。* | *テスト顧客* |
| MpnId | CSP パートナーの MPN 識別子。 | *4390934* |
| ResellerMpnId | サブスクリプションの販売店の MPN 識別子。 現在のアクティビティには使用できません。 |
| InvoiceNumber | 指定されたトランザクションが含まれる請求書番号。 | *D020001IVK* |
| ChargeStartDate | (前の請求サイクルからの) 潜在的な未請求の使用状況データの日付を提示するときを除く、請求サイクルの開始日。 時刻は常に、その日の始まりの時刻 (0:00) になります。 | *2/1/2019 0:00* |
| ChargeEndDate | (前の請求サイクルからの) 潜在的な未請求の使用状況データの日付を提示するときを除く、請求サイクルの終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 | *2/28/2019 23:59* |
| SubscriptionId | Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 サポートへの連絡時にサブスクリプションを特定すると便利な場合があります。 調整には使用されません。 *これは、パートナー管理コンソールの**サブスクリプション ID**と同じではありません。* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | サービス内容のニックネーム。 | *Microsoft Azure* |
| SubscriptionDescription | サービス プランの区分。 | *Microsoft Azure* |
| OrderID | Microsoft 課金プラットフォームでの注文の一意の識別子。 サポートへの連絡時にサブスクリプションを特定すると便利な場合があります。 調整には使用されません。 | *566890604832738111* |
| ServiceName | 対象の Azure サービスの名前。 | *仮想マシン* |
| ServiceType | 特定の種類の Azure サービス。 | *Service Bus-個人またはパック*、 *SQL Azure Database – Business Edition または Web Edition* |
| ResourceGuid | すべてのサービス データおよび価格設定構造の特定の一意の識別子。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure リソースの名前。 | *データ転送 (GB)* 、*データ転送 (送信) (GB)* |
| Region | 使用法が適用される領域。 料金はリージョンによって異なるため、主にデータ転送にレートを割り当てるために使用されます。 | *アジア太平洋*、*ヨーロッパ*、*ラテンアメリカ*、*北米* |
| SKU | オファーの一意の Microsoft 識別子。 | *7UD-00001* |
| DetailLineItemId | 特定の請求期間におけるサービスまたはリソースの異なる料金を指定するための識別子と数量。 Azure の階層化された価格設定では、課金対象ユニットの特定の数量につき1つの料金が発生する可能性があります。その後、その数量を過ぎると別の料金が発生します。 | *1* |
| ConsumedQuantity | レポート期間中に消費されるサービスの量 (時間や GB など)。 前のレポート期間から課金していない使用も含まれます。 | *11* |
| IncludedQuantity | 単位数はプランの一部として含まれます。 通常、CSP には存在しません。 | *0* |
| OverageQuantity | ユニットは、プランの一部として含まれていません。 これらは、パートナーが支払う必要があります。 **ConsumedQuantity** - **IncludedQuantity**と等しい。 | *11* |
| ListPrice | サブスクリプションの開始日に有効なプラン料金。 | *$0.0808* |
| PretaxCharges | が最も近い**値に丸め**られた、**リスト**に等しい。 | *$0.085* |
| TaxAmount | 料金が請求されます。 市場の税金ルールと特定の状況に基づいています。 | *$0.08* |
| PostTaxTotal | 税が適用されるときの税引き後の合計額。 | *$0.93* |
| 通貨 | 通貨の種類。 各課金エンティティの通貨は 1 つのみです。 最初の請求書と一致していることを確認し、その後、主要な課金プラットフォームを更新します。 | *EUR* |
| PretaxEffectiveRate | 単位あたりの税込み価格。 これは、最も近い**値に丸め**られた、**オーバー**・・・・・・・・・・・・・・・・・・・・・・・・の | *$0.08* |
| PostTaxEffectiveRate | 単位あたりの税引き後の価格。 **PostTaxTotal**は、最も近い値に丸められ、**オーバーオーバー**で除算されます。 または、1ユニットあたりの amoun の税率と、最も近い**値に丸め**られたユニットあたりの税率です。 | *$0.08* |
| ChargeType | 料金または調整[の種類](recon-file-charge-types.md)。 | [料金の種類](recon-file-charge-types.md)を参照してください。 |
| CustomerId | 顧客の一意の Microsoft 識別子 (GUID 形式)。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | 顧客のドメイン名。 このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 | *example.onmicrosoft.com* |
| BillingCycleType | 時間の請求頻度。| **毎月**  |
| Unit | リソース**名**の単位です。 | *GB*または*時間* |
| CustomerBillableAccount | Microsoft billing platform の一意のアカウント識別子。 | *1280018095* |
| UsageDate | サービスの展開の日付。 | *2/1/2019 0:00* |
| MeteredRegion | リージョン内のデータセンターの場所を示します (この値が適用可能で設定されているサービスの場合)。 | *東アジア*、*南部東アジア*、*北ヨーロッパ*、*西ヨーロッパ*、*米国中北部*、*米国中南部* |
| MeteredService | **ServiceName**列で明確に特定されていない場合に、個々の Azure サービスの使用状況を識別します。 たとえば、データ転送は、 **ServiceName**列の*Microsoft Azure すべてのサービス*として報告されます。 | *Accesscontrol-namespace*、 *CDN*、 *Compute*、 *Database*、、 *Storage* |
| MeteredServiceType | Azure サービスの使用状況をさらに明確に示す、 **Meteredservice**フィールドの小見出し。 | *EXTERNAL* |
| プロジェクト | サービス インスタンスの顧客定義の名前。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | 特定の日にプロビジョニングおよび使用された Azure Service Bus 接続の数。 | *1.000000 接続/30 日*(30 日間に個別にプロビジョニングされた接続がある場合)、 *25 個の接続/30 日が使用されています: 1.000000* (Service Bus 接続の25パックがあり、その日に1を使用した場合) |
