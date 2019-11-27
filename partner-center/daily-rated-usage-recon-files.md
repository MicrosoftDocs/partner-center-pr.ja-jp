---
title: 毎日評価済みの使用状況の調整ファイル |パートナーセンター
ms.topic: article
ms.date: 11/21/2019
description: パートナーセンターで、毎日評価される使用量調整ファイルについて説明します。
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389700"
---
# <a name="daily-rated-usage-reconciliation-files"></a>毎日評価済みの使用状況調整ファイル

適用対象

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

このトピックでは、毎日評価される使用状況の調整ファイルを読み取る方法について説明します。

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>日単位で評価される使用状況の調整ファイルのフィールド

| [列] | 説明 |
| ------ | ----------- |
| PartnerId | GUID 形式のパートナー識別子。 |
| PartnerName | パートナー名。 |
| CustomerId | GUID 形式の顧客の一意の Microsoft 識別子。 |
| CustomerCompanyName | パートナー センターで報告される顧客の組織名。 *このコラムは、請求書をシステム情報に合わせて調整する場合に非常に重要です。* |
| CustomerDomainName | 顧客のドメイン名。 現在のアクティビティには使用できません。 |
| Customer country | 顧客の在住国。 |
| MPNID | CSP パートナーの MPN 識別子。 |
| Reseller MPNID | サブスクリプションの販売店の MPN 識別子。 現在のアクティビティには使用できません。 |
| InvoiceNumber | 指定されたトランザクションが含まれる請求書番号。 現在のアクティビティには使用できません。 |
| ProductId | 製品の識別子。 |
| SkuId | 特定の SKU の識別子。 |
| AvailabilityId | 特定の SKU の可用性の識別子。 これは、指定された国、通貨、業界セグメントなどで SKU を購入できるかどうかを示します。 |
| SKU Name | 特定 SKU のタイトル。 |
| PublisherName | 発行元の名前。 |
| PublisherID | GUID 形式のパブリッシャーの識別子。 現在のアクティビティには使用できません。 |
| Subscription Description | 価格表で定義されている、顧客が購入したサービス プランの名前。 (これは、 **Offername**と同じフィールドです)。 |
| サブスクリプション ID | Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 調整には使用されません。 *この識別子は、パートナー管理コンソールの**サブスクリプション ID**と同じではありません。* |
| ChargeStartDate | 請求サイクルの開始日 (以前の請求サイクルから以前に使用されていた使用状況データを表示していない日付を表示する場合を除く)。 時刻は常に、その日の始まりの時刻 (0:00) になります。 |
| ChargeEndDate | 請求サイクルの終了日 (以前のサイクルから過去の使用状況データを除外した日付を表示する場合を除く)。 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| Usage Date | サービス使用の日付。 |
| Meter Type | メーターの種類。 |
| Meter Category | 使用状況の最上位サービス。 |
| Meter Id | 使用されているメーターの識別子。 |
| Meter Sub-category | 料金に影響する可能性のある Azure サービスの種類。 |
| Meter Name | 使用しているメーターの測定単位。 |
| Meter Region | この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。 |
| ユニット | リソース**名**の単位です。 |
| Consumed Quantity | レポート期間中に消費されるサービスの量 (*時間*や*GB*など)。 以前のレポート期間の未請求の使用状況が含まれます。 |
| Resource Location | メーターが実行されているデータセンターを > します。 |
| Consumed Service | 使用した Azure プラットフォーム サービス。 |
| Resource URI | 使用されているリソースの URI。 |
| 請求の種類 | 課金または調整の種類。 現在のアクティビティには使用できません。 |
| 単価 | ライセンスあたりの料金。購入時の価格表に記載されています。 この価格が、調整中に請求システムに格納されている情報と一致していることを確認してください。 |
| Quantity | ライセンス数。 この価格が、調整中に請求システムに格納されている情報と一致していることを確認してください。 |
| Unit type | メーターが課金するユニットの種類。 現在のアクティビティには使用できません。 |
| Billing pre tax | 税金までの合計請求額。 |
| Billing currency | 顧客の地域における通貨。 |
| Pricing pretax total | 税金が追加される前の価格。 |
| Pricing currency | 価格表の通貨。 |
| Service Info 1 | 特定の日にプロビジョニングおよび使用された Service Bus 接続の数。 |
| Service Info 2 | 省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。 |
| Additional Info | 他の列で網羅されていないすべての追加情報。 |
