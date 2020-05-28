---
title: 1回限りの定期的な調整ファイル
ms.topic: article
ms.date: 05/26/2020
description: パートナーセンターの1回限りおよび定期的な調整ファイルの各フィールドまたは列の意味を理解します。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e5fc08500cfe78f8e814ed361062c209b0f76ef
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998418"
---
# <a name="one-time-and-recurring-reconciliation-files-in-partner-center"></a>パートナーセンターでの1回限りの定期的な調整ファイル

**適用対象**

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

**適切なロール**

- グローバル管理者
- ユーザー管理者
- 課金管理者
- 管理エージェント
- 販売代理店

このトピックでは、パートナーセンターで1回限りの定期的な調整ファイルを読み取る方法について説明します。

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>1回限りの定期的な調整ファイルのフィールド

| Column | 説明 |
| ------ | ----------- |
| PartnerId | 特定の請求エンティティの一意の Azure Active Directory (Azure AD) テナント識別子 (GUID 形式)。 調整には必要ありません。 すべての行で同じです。 |
| CustomerId | 一意の Azure AD テナント識別子 (GUID 形式)。 顧客を指定します。 |
| CustomerName | パートナー センターで報告される顧客の組織名。 |
| CustomerDomainName | 顧客のドメイン名。 このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 *このフィールドは、顧客の一意の識別子として使用しないでください。顧客/パートナーは、Office 365 ポータルを使用してバニティまたは既定のドメインを更新できます。* |
| CustomerCountry | 顧客の在住国。 |
| InvoiceNumber | 指定されたトランザクションが含まれている請求書番号。 |
| MpnId | CSP パートナーの MPN 識別子。 |
| OrderId | Microsoft コマース プラットフォームでの注文に対する一意の識別子。 調整には使用されません。 |
| OrderDate | 注文が作成された日付。 |
| ProductId | 製品の識別子。 |
| SkuId | 特定の SKU (在庫保持ユニット) の識別子。 |
| AvailabilityId | 特定の SKU の可用性の識別子。 これは、指定された国、通貨、業界セグメントなどで SKU を購入できるかどうかを示します。 |
| SkuName | 特定 SKU のタイトル。 |
| ProductName | 製品の名前です。 |
| ChargeType | 料金または調整の種類。 |
| UnitPrice | 購入時に価格表に発行された単価。 *これは、調整時に請求システムに格納されている情報と一致していることを確認してください。* |
| Quantity | ユニットの数。 *これは、調整時に請求システムに格納されている情報と一致していることを確認してください。* |
| SubTotal | 合計額 (税抜)。 割引の場合、予想される合計に対して小計が一致するかどうかを確認します。 |
| TaxTotal | 納税額。 市場の税金ルールと特定の状況に基づいています。 |
| 合計 | 合計額 (税込)。 請求書に課税されるかどうかを確認します。 |
| Currency | 通貨の種類。 各請求エンティティの通貨は 1 つのみです。 これが最初の請求書と一致していることを確認し、主要な課金プラットフォームの更新後にもう一度確認してください。 |
| PriceAdjustmentDescription | 適用可能なすべての割引の説明。 |
| 発行元 | 製品の発行元の名前。
| PublisherId | 特定のパブリッシャーの一意識別子。 |
| SubscriptionDescription | サブスクリプションのフレンドリ名。 |
| SubscriptionId | Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。 調整には使用されません。 *この識別子は、パートナー管理コンソールの**サブスクリプション ID**と同じではありません。* |
| ChargeStartDate | 課金の開始日。 この時間は常に、1 日の開始時刻である 0:00 です。 |
| ChargeEndDate | 課金の終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| Termandbilのサイクル | 購入の期間と請求サイクル (たとえば、 *1 年、月単位*)。 |
| EffectiveUnitPrice | 調整が行われた後の単価。 |
| Unittype.pixel 単位 | 購入したユニットの種類。 |
| AlternateId | **注文 ID**の代替識別子。 |
| 各販売数量 | 購入または消費されたユニットの合計を表します。 |
| Ic 周波数 | 品目が月単位または1回限りの請求頻度であるかどうかを示します。 *これは現在、Azure RI でのみサポートされており、サポートされている値は月単位です。1回限りの課金頻度で RI を購入した場合、Recon ファイルのこのフィールドは空白になります。* |
| PricingCurrency | リソースまたはプランの表示価格。 |
| PCToBCExchangeRate | 料金通貨に適用される換算レートが請求通貨に適用されます。 |
| PCToBCExchangeRateDate | 請求通貨の価格の通貨が決定される日付。 |
| MeterDescription | 従量課金品目のメーターの説明。 |
