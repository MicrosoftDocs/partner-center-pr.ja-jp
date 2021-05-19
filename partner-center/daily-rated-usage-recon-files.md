---
title: 日次評価の使用状況調整ファイル
ms.topic: article
ms.date: 06/12/2020
description: 毎日評価された使用状況調整ファイルを読み取る方法については、パートナー センター。 recon ファイル内の特定のフィールドの説明が含まれます。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147277"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>毎日評価された使用状況調整ファイルを読み取る方法については、パートナー センター

**適用対象**: パートナー センター |パートナー センターのMicrosoft Cloud for US Government

**適切なロール**: 管理エージェント |課金管理者|Sales Agent |ヘルプデスク エージェント

この記事では、日次評価の使用状況調整ファイルを読み取る方法について説明します。

>[!NOTE]
>日次で評価される使用量は、通常、24 時間で表示され、パートナー センター API 経由でアクセスされます。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>日次評価の使用状況調整ファイルのフィールド

| 列 | 説明 |
| ------ | ----------- |
| PartnerId | GUID 形式のパートナー識別子。 |
| PartnerName | パートナー名。 |
| CustomerId | GUID 形式の顧客の一意の Microsoft 識別子。 |
| CustomerName | パートナー センターで報告される顧客の組織名。 *この列は、請求書とシステム情報を調整する場合に重要です。* |
| CustomerDomainName | 顧客のドメイン名。 |
| CustomerCountry | 顧客の在住国。 |
| MpnId | CSP パートナーの MPN 識別子。 |
| Tier2MpnId | サブスクリプションのレコードのリセラーの MPN 識別子。 |
| InvoiceNumber | 指定されたトランザクションが含まれている請求書番号。 |
| ProductId | 製品の識別子。 |
| SkuId | 特定の SKU の識別子。 |
| AvailabilityId | 特定の SKU の可用性の識別子。 この列には、SKU が特定の国、通貨、業界セグメントなどで購入できるかどうかが表示されます。 |
| SkuName | 特定 SKU のタイトル。 |
| ProductName | 製品の名前です。 |
| 発行元 | 発行元の名前。 |
| PublisherId | GUID 形式のパブリッシャーの識別子。 |
| SubscriptionDescription | 価格表で定義されている、顧客が購入したサービス プランの名前。 (この列には、 **Offername** と同じフィールドがあります)。 |
| SubscriptionId | Microsoft 請求プラットフォームでのサブスクリプションの一意識別子。 調整には使用されません。 *この識別子は、パートナー管理コンソールの **サブスクリプション ID** と同じではありません。* |
| ChargeStartDate | 請求サイクルの開始日 (以前の請求サイクルから以前に使用されていた使用状況データを表示していない日付を表示する場合を除く)。 この時間は常に、1 日の開始時刻である 0:00 です。 |
| ChargeEndDate | 請求サイクルの終了日 (以前の請求サイクルから過去に発生した使用状況データを表示する場合を除く)。 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| UsageDate | サービス使用の日付。 |
| MeterType | メーターの種類。 |
| MeterCategory | 使用状況の最上位レベルのサービス。 |
| MeterId | 使用されているメーターの識別子。 |
| MeterSubCategory | 料金に影響する可能性のある Azure サービスの種類。 |
| MeterName | 使用しているメーターの測定単位。 |
| MeterRegion | この列は、MeterRegion が適用可能で設定されているサービスのリージョン内のデータセンターの場所を示します。 |
| ユニット | リソース **名** の単位です。 |
| ResourceLocation | メーターが実行されているデータセンター。 |
| ConsumedService | 使用した Azure プラットフォーム サービス。 |
| ResourceGroup | Azure ソリューションの関連リソースを保持するコンテナーを表します。 |
| ResourceURI | 使用されているリソースの URI。 |
| ChargeType | 料金または調整の種類。  |
| UnitPrice | ライセンスあたりの料金。購入時の価格表に記載されています。 この価格が、調整中に請求システムに格納されている情報と一致していることを確認してください。 |
| Quantity | ライセンス数。 この価格が、調整中に請求システムに格納されている情報と一致していることを確認してください。 |
| Unittype.pixel 単位 | メーターが課金するユニットの種類。  |
| すべての Lingpretaxtotal | 税金までの合計請求額。<br/> _**すべての Lingpretaxtotal** = FLOOR (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ])、2)_ |
| BillingCurrency | 顧客の地域における通貨。 |
| PricingPreTaxTotal | 税金が追加される前の価格。 |
| PricingCurrency | 価格表の通貨。 |
| ServiceInfo1 | 特定の日にプロビジョニングおよび使用された Service Bus 接続の数。 |
| ServiceInfo2 | 省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。 |
| タグ | ユーザーによって設定された Azure リソースの論理編成を表します。 |
| AdditionalInfo | 他の列で説明されていない任意の追加情報。 |
| EffectiveUnitPrice | 割引、獲得したクレジットなど、ユニットごとに課金される実際の値。 |
| PCToBCExchangeRate | 料金通貨に適用される換算レートが請求通貨に適用されます。 |
| PCToBCExchangeRateDate | 請求通貨の価格の通貨が決定される日付。 |
| EntitlementId | Azure サブスクリプション ID を表します。 |
| EntitlementDescription | Azure サブスクリプション ID の名前を表します。 |
| PartnerEarnedCreditPercentage | 品目の PartnerEarnedCredit を表示します。 獲得クレジットは、0または15% になります |
| CreditPercentage | Azure の消費クレジットが表示されます。 獲得クレジットは、0または100% のいずれかになります。 |
| CreditType | クレジットの種類。 たとえば **、Azure クレジットの適用などです。** |
>[!NOTE]
>日次で評価される使用量は、通常、24 時間かかりますが、パートナー センター API 経由でアクセスされます。


