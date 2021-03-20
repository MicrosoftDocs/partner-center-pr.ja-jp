---
title: CSP の1回限りの購入のファイルフィールド
ms.topic: conceptual
ms.date: 01/29/2021
description: サンプル値を含む、パートナーセンターの CSP の1回限りの購入調整ファイルに関するすべての項目について説明します。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 74974c68c607ddcee4aff6abd53284a60653fb0b
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712258"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>CSP による1回限りの購入調整ファイルフィールド

## <a name="using-the-recon-file"></a>偵察ファイルの使用
次の表は、CSP の1回限りの購入について、調整ファイル内のフィールドの説明とサンプル値を示しています。

調整ファイルの詳細については、「 [調整ファイルの使用](use-the-reconciliation-files.md)」を参照してください。

| 列 | 説明 | 値の例 |
| ------ | ----------- | ------------ |
| PartnerId | 特定の請求エンティティの GUID 形式の一意識別子。 調整には必要ありません。 すべての行で同じです。 | *0e195b374574-45742-0e539b9684 c0* |
| CustomerId | GUID 形式の顧客の一意の Microsoft 識別子。 | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | パートナー センターで報告される顧客の組織名。 この列は、請求書をシステム情報に合わせて調整するために重要です。 | *Johnny モダン Cust DE2* |
| CustomerDomainName | 顧客のドメイン名。 | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | 顧客が配置されている国。 お客様の地域の [国の](./regional-authorization-overview.md) 完全な一覧をご覧ください。  | *DE* |
| InvoiceNumber | 調整ファイルに関連付けられている請求書番号。  | *G002297372* |
| MpnId | CSP パートナーの MPN 識別子。 詳細については、「 [パートナー別に明細を表示する方法](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)」を参照してください。 | *6034453* |
| ResellerMpnId | サブスクリプションの販売店の MPN 識別子。 | *6048879* |
| OrderId | Microsoft 請求プラットフォームでの注文の一意識別子。 サポートに連絡するときに、注文を識別するのに役立つ場合があります。 調整には使用されません。 | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | 注文が配置された日付。 | *10/3/2020* |
| ProductId | 製品の一意の識別子。 | *DZH318Z0BNZ5* |
| SkuId | SKU の一意識別子。 | *006G* |
| AvailabilityId | 可用性の一意識別子。 | *DZH318Z08B80* |
| SkuName | SKU の名前。 | *テーブル-LRS* |
| ProductName | 製品名。 | *テーブル* |
| ChargeType | 料金または調整 [の種類](./recon-file-charge-types.md) 。 | *[新規作成]* |
| UnitPrice | ライセンスあたりの料金。購入時の価格表に記載されています。 これは、調整時に請求システムに格納されている情報と一致していることを確認してください。 | *0.045* |
| Quantity | ライセンスの数。 これは、調整時に請求システムに格納されている情報と一致していることを確認してください。 | *1* |
| 小計 | 合計額 (税抜)。 小計は、課金対象の数量と有効な単価を乗算した値と同じである必要があります。 | *0* |
| TaxTotal | 納税額。 市場の税金ルールと特定の状況に基づいています。 | *0* |
| 合計 | 合計金額は、小計に税額を加えた値になります。 | *0* |
| Currency | 請求書は顧客の通貨のコンテキストで生成されます。 したあって、請求対象の通貨が異なる顧客と取引を行うパートナーの場合、顧客の通貨の種類ごとに請求書を受け取ることになります。  | *EUR* |
| PriceAdjustmentDescription | 単価の調整の理由。 これらは主な理由ですが、有効な単価の決定に限定されるわけではありません。 | *["15.0% のパートナー獲得クレジット (サービスの管理対象)"]* |
| 発行元 | 製品の発行元。  | *Microsoft* |
| PublisherId | パートナーセンターが発行元を識別するために使用する一意の識別子。 | *NA* |
| SubscriptionDescription | 価格表で定義されている、顧客が購入したサービス プランの名前。 この列は、OfferName と同じフィールドです。 | *Azure プラン* |
| SubscriptionId | Microsoft 請求プラットフォームでのサブスクリプションの一意識別子。 調整には使用されません。 この識別子は、パートナー管理コンソールのサブスクリプション ID と同じではないことに注意してください。 | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | パートナーセンターがサブスクリプション料金に対して料金を請求する日付。 サブスクリプションに年間請求期間と月単位の課金プランが購入されている場合は、最初の調整ファイルで、サブスクリプションが購入された日になります。 次の調整ファイルから、30日後にインクリメントされます。 | *9/1/2020* |
| ChargeEndDate | サブスクリプションの請求サイクルに対する請求の終了日。 サブスクリプションに年間請求期間と月単位の課金プランが購入されている場合、最初の調整ファイルでは、サブスクリプションが購入されてから30日後になります。 次の調整ファイルから、30日後にインクリメントされます。 | *2020 年 9 月 30 日* |
| Termandbilのサイクル | 購入時にサブスクリプションを継続するための期間コミットメント。 | *格納されたデータ (GB/月)* |
| EffectiveUnitPrice | 請求サイクルのコストを計算するための日割り単価。 割引、請求日の調整、およびその他の要因によって、有効な単価が決まります。 詳細については、「 [有効な単価の計算](./effective-unit-price-calculation.md)」を参照してください。  | *0.03825* |
| Unittype.pixel 単位 | メーターが課金される単位の種類。 | *1 GB/月* |
| AlternateId | 参照される注文品目の代替 ID。 | *6dc5c039750a* |
| 各販売数量 | 請求される合計数量。  | *0.005001* |
| Ic 周波数 | 購入時に選択された課金プラン。 | *NA*  |
| PricingCurrency | 価格表の通貨。 | *USD* |
| PCToBCExchangeRate | 料金通貨に適用される換算レート。 | *0.846202666* |
| PCToBCExchangeRateDate | 請求通貨の価格の通貨が決定される日付。 | *2020 年 9 月 30 日* |
| MeterDescription | メーターの説明。  | *テーブル-LRS 格納データ (GB/月)* |
| ReservationOrderId | 予約注文 Id。 | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | クレジットの説明。 | *Azure の消費クレジット* |

>[!NOTE]
>Azure の使用量は、一度だけ購入したファイルで調整できます。 これを行うには、毎日評価される使用法偵察 file にアクセスし、SubscriptionID を検索します。 これにより、Azure プラン ID に関連付けられているすべてのコストが表示されます。 Azure SubscriptionID は EntitlementID として表示されます。

## <a name="next-steps"></a>次のステップ

- [請求と税金](billing.md)
