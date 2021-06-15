---
title: CSP 1 回購入の調整ファイル フィールド
ms.topic: conceptual
ms.date: 01/29/2021
description: サンプル値を含む、CSP の 1 回購入調整ファイルのすべての項目についてパートナー センターについて説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 3264c793dfb2e8592cd059cd84d5bb08769abbcf
ms.sourcegitcommit: c8d1bcf54cdcdc3f827f9210c8abddab02a686fe
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2021
ms.locfileid: "112073800"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP の 1 回購入調整ファイルのフィールド

**適切なロール**: アカウント管理者|課金エージェント

## <a name="using-the-recon-file"></a>recon ファイルの使用
次の表は、CSP 1 回購入の調整ファイル内のフィールドの説明とサンプル値を示しています。

調整ファイルの詳細については、「調整ファイルを使用 [する」を参照してください](use-the-reconciliation-files.md)。

| 列 | 説明 | 値の例 |
| ------ | ----------- | ------------ |
| PartnerId | 特定の課金エンティティの GUID 形式の一意識別子。 調整には必要ありません。 すべての行で同じです。 | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | GUID 形式の顧客の一意の Microsoft 識別子。 | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | パートナー センターで報告される顧客の組織名。 この列は、請求書とシステム情報を調整する場合に重要です。 | *Johnny Modern Cust DE2* |
| CustomerDomainName | 顧客のドメイン名。 | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 顧客が位置する国。 リージョンの国 [の完全な一覧](./regional-authorization-overview.md) を参照してください。  | *DE* |
| InvoiceNumber | 調整ファイルに関連付けられている請求書番号。  | *G002297372* |
| MpnId | CSP パートナーの MPN 識別子。 詳細については、パートナー 別に [項目化する方法に関するページを参照してください](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)。 | *6034453* |
| ResellerMpnId | サブスクリプションのレコードのリセラーの MPN 識別子。 | *6048879* |
| OrderId | Microsoft 請求プラットフォームでの注文の一意識別子。 サポートに問い合わせの際に注文を識別するのに役立つ場合があります。 調整には使用されません。 | *0ET2qaZvJGfF9wgSKnKnKnR5JLmhp10lOc1* |
| OrderDate | 注文が行された日付 (UTC)。 | *10/3/2020* |
| ProductId | 製品の一意識別子。 | *DZH318Z0BNZ5* |
| SkuId | SKU の一意識別子。 | *006G* |
| AvailabilityId | 可用性の一意識別子。 | *DZH318Z08B80* |
| SkuName | SKU 名。 | *テーブル - LRS* |
| ProductName | 製品名。 | *テーブル* |
| ChargeType | 料金 [または調整の](./recon-file-charge-types.md) 種類。 | *[新規作成]* |
| UnitPrice | 購入時に価格表に公開されているライセンスあたりの価格。 これは、調整中に課金システムに格納されている情報と一致します。 | *0.045* |
| Quantity | ライセンスの数。 これは、調整中に課金システムに格納されている情報と一致します。 | *1* |
| 小計 | 合計額 (税抜)。 小計は、請求可能数量に有効な単価を乗算した値と等しい必要があります。 | *0* |
| TaxTotal | 税額の料金。 市場の税規則と特定の状況に基づく。 | *0* |
| 合計 | 合計金額は、小計に税額を加えた金額と等しくなります。 | *0* |
| Currency | 請求書は、顧客の通貨のコンテキストで生成されます。 したあって、請求対象の通貨が異なる顧客と取引を行うパートナーの場合、顧客の通貨の種類ごとに請求書を受け取ることになります。  | *ユーロ* |
| PriceAdjustmentDescription | 単価の調整の理由。 これらは主な理由ですが、有効な単価の決定に限定されるのではありません。 | *["15.0% Partner earned credit for services managed"]* |
| 発行元 | 製品の発行元。  | *Microsoft* |
| PublisherId | パブリッシャーを識別するためにパートナー センターする一意識別子。 | *Na* |
| SubscriptionDescription | 価格表で定義されている、顧客が購入したサービス プランの名前。 この列は OfferName と同じフィールドです。 | *Azure プラン* |
| SubscriptionId | Microsoft 請求プラットフォームでのサブスクリプションの一意識別子。 調整には使用されません。 この識別子は、パートナー管理コンソールのサブスクリプション ID と同じではありません。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | サブスクリプションの請求期間が開始される日付。 | *9/1/2020* |
| ChargeEndDate | サブスクリプションの請求期間が終了する日付。 | *2020 年 9 月 30 日* |
| TermAndBillingCycle | 購入時にサブスクリプションを継続する期間コミットメント。 | *格納されるデータ (GB/月)* |
| EffectiveUnitPrice | 請求サイクルのコストを計算する日単位価格。 割引、請求日の調整、その他の要因によって、有効な単価が決されます。 詳細については、「有効な単価の [計算」を参照してください](./effective-unit-price-calculation.md)。  | *0.03825* |
| UnitType | メーターが課金される単位の種類。 | *1 GB/月* |
| AlternateId | 参照先の注文品目の代替 ID。 | *6dc5c039750a* |
| BillableQuantity | 請求される合計数量。  | *0.005001* |
| BillingFrequency | 購入時に選択された課金プラン。 | *Na*  |
| PricingCurrency | 価格表の通貨。 | *USD* |
| PCToBCExchangeRate | 請求通貨に対して価格通貨に適用される為替レート。 | *0.846202666* |
| PCToBCExchangeRateDate | 請求通貨に対する価格通貨が決定される日付。 | *2020 年 9 月 30 日* |
| MeterDescription | 測定の説明。  | *テーブル - 格納される LRS データ (GB/月)* |
| ReservationOrderId | 予約注文 ID。 | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | クレジットの説明。 | *Azure Consumption Credit* |
| SubscriptionStartDate | サブスクリプションが購入された日付。 | *5/1/2021* |
| SubscriptionEndDate | サブスクリプションの有効期限が切れる日付。 | *4/30/2022* |
| ReferenceID | アップグレード中に発生するトランザクションへのリンケージ。 | *025d68a6-1bd6-42ab-9636-15e8d776a30e* |
| ProductQualifiers | アドオンまたは試用版の購入を知る識別子。 | *["アドオン"]* |
| PromotionID | 昇格の情報をフェッチするために使用する識別子。 | *78bcf906-b945-4210-8818-cfb93caf12a1* |

>[!NOTE]
>Azure の消費量は、1 回の購入調整ファイルで調整できます。 これを行うには、毎日評価された使用状況の調整ファイルに移動し、SubscriptionID を検索します。 これにより、Azure プラン ID に関連付けられているすべてのコストが表示されます。 Azure SubscriptionID は EntitlementID として表示されます。
>

## <a name="how-to-connect-the-base-subscription-with-the-upgraded-subscription"></a>基本サブスクリプションをアップグレードされたサブスクリプションに接続する方法

基本製品のサブスクリプション ID を使用して、対応する参照 ID を検索し、それらを使用して関連付けられているすべてのトランザクションをフェッチする必要があります。 サブスクリプション ID と参照 ID を組み合わせると、1 つのイベントで発生したすべてのアップグレードを接続できます。

## <a name="next-steps"></a>次のステップ

- [請求と税金](billing.md)
