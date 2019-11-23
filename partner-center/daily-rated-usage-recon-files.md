---
title: Daily-rated usage reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand daily-rated usage reconciliation files in Partner Center.
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
# <a name="daily-rated-usage-reconciliation-files"></a>Daily-rated usage reconciliation files

適用対象:

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

This topic explains how to read daily-rated usage reconciliation files.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Fields in daily-rated usage reconciliation files

| Column | 説明 |
| ------ | ----------- |
| PartnerId | Partner identifier in GUID format. |
| PartnerName | Partner name. |
| CustomerId | Unique Microsoft identifier for the customer in GUID format. |
| CustomerCompanyName | パートナー センターで報告される顧客の組織名。 *This column is very important for reconciling the invoice with your system information.* |
| CustomerDomainName | The customer's domain name. 現在のアクティビティには使用できません。 |
| Customer country | 顧客の在住国。 |
| MPNID | MPN identifier of the CSP partner. |
| Reseller MPNID | MPN identifier of the reseller of record for the subscription. 現在のアクティビティには使用できません。 |
| InvoiceNumber | 指定されたトランザクションが含まれる請求書番号。 現在のアクティビティには使用できません。 |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU. |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 特定 SKU のタイトル。 |
| PublisherName | 発行元の名前。 |
| PublisherID | The identifier of the publisher in GUID format. 現在のアクティビティには使用できません。 |
| Subscription Description | 価格表で定義されている、顧客が購入したサービス プランの名前 (This is an identical field to **OfferName**). |
| サブスクリプション ID | Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | Start date of the billing cycle (except when presenting dates of previously uncharged latent usage data from the previous billing cycle). 時刻は常に、その日の始まりの時刻 (0:00) になります。 |
| ChargeEndDate | End date of billing cycle (except when presenting dates of previously uncharged latent usage data from the previous biling cycle). 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| Usage Date | サービス使用の日付。 |
| Meter Type | メーターの種類。 |
| Meter Category | 使用状況の最上位サービス。 |
| Meter Id | The identifier for the meter being used. |
| Meter Sub-category | The type of Azure service, which can affect the rate. |
| Meter Name | 使用しているメーターの測定単位。 |
| Meter Region | この列は、これが該当し、設定されている場合に、サービスの領域内でのデータ センターの場所を識別します。 |
| Unit | The unit of the resource **Name**. |
| Consumed Quantity | The amount of service consumed (such as *hours* or *GB*) during the reporting period. Includes any unbilled usage from previous reporting periods. |
| Resource Location | >The data center where the meter is running. |
| Consumed Service | 使用した Azure プラットフォーム サービス。 |
| Resource URI | 使用されているリソースの URI。 |
| 請求の種類 | 課金または調整の種類。 現在のアクティビティには使用できません。 |
| 単価 | Price per license, as published in the price list at the time of purchase. Make sure this price matches the information stored in your billing system during reconciliation. |
| Quantity | ライセンス数。 Make sure this price matches the information stored in your billing system during reconciliation. |
| Unit type | メーターが課金するユニットの種類。 現在のアクティビティには使用できません。 |
| Billing pre tax | Total billing amount before taxes. |
| Billing currency | The currency in the customer's geographic region. |
| Pricing pretax total | 税金が追加される前の価格。 |
| Pricing currency | The currency in the price list. |
| Service Info 1 | The number of Service Bus connections that were provisioned and utilized on a given day. |
| Service Info 2 | 省略可能なサービスに固有のメタデータをキャプチャするレガシ フィールド。 |
| Additional Info | 他の列で網羅されていないすべての追加情報。 |
