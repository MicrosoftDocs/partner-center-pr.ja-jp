---
title: ライセンス ベースの調整ファイル
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターでライセンスベースの調整ファイルを読み取る方法について説明します。 この記事では、ライセンスベースの偵察ファイルの各フィールドの意味について説明します。
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4c311de4a504785e15cefc7a93f1ee3da396ea7d
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441287"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>パートナーセンターのライセンスベースの調整ファイルのフィールドについて

**適用対象**

- 米国政府機関向け Microsoft Cloud のパートナー センター

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 課金管理者
- 管理エージェント

顧客の注文に対して変更を調整するには、調整ファイルの **Syndication_Partner_Subscription_Number** と、パートナーセンターの **サブスクリプション ID** を比較します。

## <a name="fields-in-license-based-reconciliation-files"></a>ライセンスベースの調整ファイルのフィールド

| 列 | 説明 | 値の例 |
| ------ | ----------- | ------------ |
| PartnerId | 特定の請求エンティティの GUID 形式の一意識別子。 調整には必要ありません。 すべての行で同じです。 | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | GUID 形式の顧客の一意の Microsoft 識別子。 | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | パートナー センターで報告される顧客の組織名。 *請求書をシステム情報と調整するための非常に重要なフィールドです。* | *Test Customer A* |
| MpnId | CSP パートナーの MPN 識別子。 「 [パートナー別に明細を表示する方法」を](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner)参照してください。 | *4390934* |
| ResellerMpnId | サブスクリプションの販売店の MPN 識別子。  |
| OrderId | Microsoft 請求プラットフォームでの注文の一意識別子。 サポートに連絡するときに、注文を識別するのに役立つ場合があります。 調整には使用されません。 | *566890604832738111* |
| SubscriptionId | Microsoft 請求プラットフォームでのサブスクリプションの一意識別子。 サポートへの連絡時にサブスクリプションを特定すると便利な場合があります。 調整には使用されません。 *この値は、パートナー管理コンソールの **サブスクリプション ID** と同じではありません。代わりに **SyndicationPartnerSubscriptionNumber** を参照してください。* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | サブスクリプションの一意の識別子。 顧客は、同じプランに対して複数のサブスクリプションを持つことができます。 この列は、ファイルの調整分析に重要です。 このフィールドは、パートナー管理コンソールの **サブスクリプション ID** にマップされます。 | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | 一意のプラン識別子。 価格表に定義されている標準プラン識別子。 *この値は、価格表の **オファー ID** と一致しません。代わりに **DurableOfferID** を参照してください。* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferId | 価格表で定義されている一意の永続的なプラン識別子。 *この値は、価格表の **プラン ID** と一致します。* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 価格表で定義されている、顧客が購入したサービス プランの名前。 | *Microsoft Office 365 (プラン E3)* |
| SubscriptionStartDate | サブスクリプションの開始日。 この時間は常に、1 日の開始時刻である 0:00 です。 このフィールドは、注文が送信された日に設定されます。 **Subscriptionenddate** と共に使用して、顧客がまだサブスクリプションの最初の年内にあるかどうか、またはサブスクリプションが次の年に更新されたかどうかを判断します。 | *2/1/2019 0:00* |
| SubscriptionEndDate | サブスクリプションの終了日。 この時間は常に、1 日の開始時刻である 0:00 です。 パートナーの請求日または *更新日から12か月* 後に、*開始日から12か月を加算した日数* 。 更新時に、価格は最新の価格表に更新されます。 自動更新の前に、顧客とのやり取りが必要になる場合があります。 | *2/1/2019 0:00* |
| ChargeStartDate | 課金の開始日。 この時間は常に、1 日の開始時刻である 0:00 です。 顧客がライセンス番号を変更したときの日単位の料金 (*pro 対する比率* の料金) を計算するために使用されます。 | *2/1/2019 0:00* |
| ChargeEndDate | 課金の終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 顧客がライセンス番号を変更したときの日単位の料金 (*pro 対する比率* の料金) を計算するために使用されます。 | *2/28/2019 23:59* |
| ChargeType | 料金または調整 [の種類](recon-file-charge-types.md) 。 | [料金の種類](recon-file-charge-types.md)を参照してください。 |
| UnitPrice | ライセンスあたりの料金。購入時の価格表に記載されています。 これは、調整時に請求システムに格納されている情報と一致していることを確認してください。 | *6.82* |
| Quantity | ライセンス数。 これは、調整時に請求システムに格納されている情報と一致していることを確認してください。 | *2* |
| Amount | 数量に対する合計価格。 金額の計算が顧客に対してこの値を計算する方法と一致するかどうかを確認するために使用されます。 | *13.32* |
| TotalOtherDiscount | これらの料金に適用される割引額。 コンピテンシーまたは地図に含まれる製品ライセンス、またはインセンティブの対象となる新しいサブスクリプションには、このコラムの割引額も含まれます。 | *2.32* |
| 小計 | 合計額 (税抜)。 割引の場合、予想される合計に対して小計が一致するかどうかを確認します。 | *11* |
| 税 | 納税額。 市場の税金ルールと特定の状況に基づいています。 | *0* |
| TotalForCustomer | 合計額 (税込)。 請求書に課税されるかどうかを確認します。 | *11* |
| Currency | 通貨の種類。 各請求エンティティの通貨は 1 つのみです。 最初の請求書と一致するかどうかを確認します。 課金プラットフォームの主要な更新後に、もう一度確認してください。 | *EUR* |
| DomainName | 顧客のドメイン名。 このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 *このフィールドは、顧客の一意の識別子として使用しないでください。顧客/パートナーは、Office 365 ポータルを使用してバニティまたは既定のドメインを更新できます。* | *example.onmicrosoft.com* |
| SubscriptionName | サブスクリプションのニックネーム。 ニックネームが指定されていない場合、パートナーセンターは **Offername** を使用します。 | *プロジェクトをオンラインにする* |
| SubscriptionDescription | 価格表で定義されている、顧客が購入したサービス プランの名前。 (これは **オフ** と同じフィールドです)。 | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
| BillingCycleType | 1回限りの請求頻度。| *毎月* |