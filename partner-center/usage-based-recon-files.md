---
title: 使用量ベースの調整ファイル
ms.topic: article
ms.date: 06/08/2020
description: 使用状況ベースの調整ファイルのすべての項目については、パートナー センター。 いくつかの例が含まれています。
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc31915660b6a82954daee5fcc8fb2d5292e725c
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109795008"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>使用状況ベースの調整ファイルとその特定のフィールドをパートナー センター

**適切なロール**: アカウント管理者|課金管理者

顧客の使用量に対して料金を調整するには、調整ファイルの **ResellerID、ResellerName、** および **ResellerBillableAccount** を、パートナー センター の顧客名とサブスクリプション **ID** と比較します。 

## <a name="fields-in-usage-based-reconciliation-files"></a>使用状況ベースの調整ファイルのフィールド

次のフィールドで、どのサービスが使用されるか、およびレートについて説明します。

| 列 | 説明 | サンプル値 |
| ------ | ----------- | ------------ |
| PartnerId | GUID 形式のパートナー識別子。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | パートナー名。 | *Contoso, Ltd.* |
| PartnerBillableAccountId | パートナー アカウント識別子。 | *1010578050* |
| CustomerCompanyName | パートナー センターで報告される顧客の組織名。 *請求書をシステム情報と調整する場合に非常に重要です。* | *顧客をテストする* |
| MpnId | CSP パートナーの MPN 識別子。 | *4390934* |
| ResellerMpnId | サブスクリプションのレコードのリセラーの MPN 識別子。  |
| InvoiceNumber | 指定されたトランザクションが含まれている請求書番号。 | *D020001IVK* |
| ChargeStartDate | (前の請求サイクルからの) 潜在的な未請求の使用状況データの日付を提示するときを除く、請求サイクルの開始日。 この時間は常に、1 日の開始時刻である 0:00 です。 | *2/1/2019 0:00* |
| ChargeEndDate | (前の請求サイクルからの) 潜在的な未請求の使用状況データの日付を提示するときを除く、請求サイクルの終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 | *2/28/2019 23:59* |
| SubscriptionId | Microsoft 請求プラットフォームでのサブスクリプションの一意識別子。 サポートに問い合わせするときに、サブスクリプションを識別するのに役立つ場合があります。 調整には使用されません。 *これは、パートナー管理コンソールの **サブスクリプション ID** と同じではありません。* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | サービス内容のニックネーム。 | *Microsoft Azure* |
| SubscriptionDescription | サービス プランの区分。 | *Microsoft Azure* |
| OrderID | Microsoft 請求プラットフォームでの注文の一意識別子。 サポートへの連絡時にサブスクリプションを特定すると便利な場合があります。 調整には使用されません。 | *566890604832738111* |
| ServiceName | 対象の Azure サービスの名前。 | *仮想マシン* |
| ServiceType | 特定の種類の Azure サービス。 | *Service Bus-個人またはパック*、 *SQL Azure Database – Business Edition または Web Edition* |
| ResourceGuid | すべてのサービス データと価格設定構造の特定の一意識別子。 | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | Azure リソースの名前。 | *データ転送 (GB)*、 *データ転送 (送信) (GB)* |
| リージョン | 使用法が適用される領域。 料金はリージョンによって異なるため、主にデータ転送にレートを割り当てるために使用されます。 | *アジア太平洋*、 *ヨーロッパ*、 *ラテンアメリカ*、 *北米* |
| Sku | オファーの一意の Microsoft 識別子。 | *7UD-00001* |
| DetailLineItemId | 特定の請求期間におけるサービスまたはリソースの異なる料金を指定するための識別子と数量。 Azure の階層化された価格設定では、課金対象ユニットの特定の数量につき1つの料金が発生する可能性があります。その後、その数量を過ぎると別の料金が発生します。 | *1* |
| ConsumedQuantity | レポート期間中に消費されるサービスの量 (時間や GB など)。 前のレポート期間から未請求の使用量も含まれます。 | *11* |
| IncludedQuantity | 単位数はプランの一部として含まれません。 通常、CSP には存在しません。 | *0* |
| OverageQuantity | ユニットは、プランの一部として含まれていません。 これらは、パートナーが支払う必要があります。 **ConsumedQuantity** - **IncludedQuantity** と等しい。 | *11* |
| ListPrice | サブスクリプションの開始日に有効なプラン料金。 | *$0.0808* |
| PretaxCharges | **ListPrist に** **OverageQuantity** を乗算した値に等しくなります。最も近いセントに丸められます。 | *$0.085* |
| TaxAmount | 課金される税額。 市場の税規則と特定の状況に基づく。 | *$0.08* |
| PostTaxTotal | 課税後の合計額 (税が適用される場合)。 | *$0.93* |
| 通貨 | 通貨の種類。 各請求エンティティの通貨は 1 つのみです。 最初の請求書と一致し、その後、主要な課金プラットフォームの更新後に一致する必要があります。 | *EUR* |
| PretaxEffectiveRate | 単位あたりの税込み単価。 **PretaxCharges を** **OverageQuantity** で割った値と等しくなります。最も近いセントに丸められます。 | *$0.08* |
| PostTaxEffectiveRate | 単位あたりの税引き後の単価。 **PostTaxTotal を** **OverageQuantity** で割った値と等しくなります。最も近いセントに丸められます。 または **、PretaxEffectiveRate** に単位金額あたりの税率を加え、最も近いセントに丸めた値に等しくなります。 | *$0.08* |
| ChargeType | 料金 [または調整の](recon-file-charge-types.md) 種類。 | 料金 [の種類に関するページを参照してください](recon-file-charge-types.md)。 |
| CustomerId | 顧客の一意の Microsoft 識別子 (GUID 形式)。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | 顧客のドメイン名。 このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 | *example.onmicrosoft.com* |
| BillingCycleType | 時間の課金頻度。| **毎月**  |
| ユニット | リソース名 の **単位**。 | *GB* または *時間* |
| CustomerBillableAccount | Microsoft 課金プラットフォームでの一意のアカウント識別子。 | *1280018095* |
| UsageDate | サービスのデプロイ日。 | *2/1/2019 0:00* |
| MeteredRegion | リージョン内のデータセンターの場所を示します (この値が適用可能で設定されているサービスの場合)。 | *東アジア*、 *南部東アジア*、 *北ヨーロッパ*、 *西ヨーロッパ*、 *米国中北部*、 *米国中南部* |
| MeteredService | **ServiceName** 列で明確に特定されていない場合に、個々の Azure サービスの使用状況を識別します。 たとえば、データ転送は、 **ServiceName** 列の *Microsoft Azure すべてのサービス* として報告されます。 | *Accesscontrol-namespace*、 *CDN*、 *Compute*、 *Database*、 、 *Storage* |
| MeteredServiceType | Azure サービスの使用状況をさらに明確に示す、 **Meteredservice** フィールドの小見出し。 | *EXTERNAL* |
| Project | サービス インスタンスの顧客定義の名前。 | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | 特定の日にプロビジョニングおよび使用された Azure Service Bus 接続の数。 | *1.000000 接続/30 日* (30 日間に個別にプロビジョニングされた接続がある場合)、 *25 個の接続/30 日が使用されています: 1.000000* (Service Bus 接続の25パックがあり、その日に1を使用した場合) |

## <a name="next-steps"></a>次の手順

- [パートナーセンターのライセンスベースの調整ファイルのフィールドについて](license-based-recon-files.md)