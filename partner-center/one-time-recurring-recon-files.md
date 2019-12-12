---
title: 1回限りの定期的な調整ファイル |パートナーセンター
ms.topic: article
ms.date: 11/21/2019
description: パートナーセンターでの1回限りの定期的な調整ファイルについて説明します。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004901"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>1回限りの定期的な調整ファイル

**適用対象**

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

**適切なロール**
-   グローバル管理
-   ユーザー管理者
-   課金の管理
-   管理エージェント
-   販売代理店

このトピックでは、パートナーセンターで1回限りの定期的な調整ファイルを読み取る方法について説明します。

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>1回限りの定期的な調整ファイルのフィールド

| Column | 説明 |
| ------ | ----------- |
| PartnerId | 特定の請求エンティティの一意の Azure Active Directory (Azure AD) テナント識別子 (GUID 形式)。 調整には必要ありません。 すべての行で同じです。 |
| Customer Id | 一意の Azure AD テナント識別子 (GUID 形式)。 顧客を指定します。 |
| 顧客名 | パートナー センターで報告される顧客の組織名。 |
| CustomerDomainName | 顧客のドメイン名。 このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 *このフィールドは、顧客の一意の識別子として使用しないでください。顧客/パートナーは、Office 365 ポータルを使用してバニティまたは既定のドメインを更新できます。* |
| Customer Country | 顧客の在住国。 |
| 請求書番号 | 指定されたトランザクションが含まれる請求書番号。 |
| MpnId | CSP パートナーの MPN 識別子。 |
| Reseller MpnId | サブスクリプションの販売店の MPN 識別子。 |
| 注文 ID | Microsoft コマース プラットフォームでの注文に対する一意の識別子。 調整には使用されません。 |
| 発注日 | 注文が作成された日付。 |
| ProductId | 製品の識別子。 |
| SkuId | 特定の SKU (在庫保持ユニット) の識別子。 |
| AvailabilityId | 特定の SKU の可用性の識別子。 これは、指定された国、通貨、業界セグメントなどで SKU を購入できるかどうかを示します。 |
| SKU Name | 特定 SKU のタイトル。 |
| 製品名 | 製品の名前。 |
| PublisherName | 製品の発行元の名前。
| PublisherID | 特定のパブリッシャーの一意識別子。 |
| Subscription Description | サブスクリプションのフレンドリ名。 |
| サブスクリプション ID | Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。 調整には使用されません。 *この識別子は、パートナー管理コンソールの**サブスクリプション ID**と同じではありません。* |
| ChargeStartDate | 課金の開始日。 時刻は常に、その日の始まりの時刻 (0:00) になります。 |
| ChargeEndDate | 課金の終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| Term and Billingcycle | 購入の期間と請求サイクル (たとえば、 *1 年、月単位*)。 |
| 請求の種類 | 課金または調整の種類。 |
| 単価 | 購入時に価格表に発行された単価。 *これは、調整時に請求システムに格納されている情報と一致していることを確認してください。* |
| Effective Unit Price | 調整が行われた後の単価。 |
| Quantity | ユニット数。 *これは、調整時に請求システムに格納されている情報と一致していることを確認してください。* |
| Unit type | 購入したユニットの種類。 |
| DiscountDetails | 適用可能なすべての割引の説明。 |
| Sub Total | 合計額 (税抜)。 割引の場合、予想される合計に対して小計が一致するかどうかを確認します。 |
| Tax Total | 納税額。 市場の税金ルールと特定の状況に基づいています。 |
| Total | 合計額 (税込)。 請求書に課税されるかどうかを確認します。 |
| Currency | 通貨の種類。 各課金エンティティの通貨は 1 つのみです。 これが最初の請求書と一致していることを確認し、主要な課金プラットフォームの更新後にもう一度確認してください。 |
| AlternateID | **注文 ID**の代替識別子。 |
