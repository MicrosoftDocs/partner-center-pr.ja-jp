---
title: One-time and recurring reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand one-time and recurring reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389680"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>One-time and recurring reconciliation files

適用対象:

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

This topic explains how to read one-time and recurring reconciliation files in Partner Center.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Fields in one-time and recurring reconciliation files

| Column | 説明 |
| ------ | ----------- |
| PartnerId | Unique Azure Active Directory (Azure AD) tenant identifier for a specific billing entity, in GUID format. Not required for reconciliation. すべての行で同じです。 |
| Customer Id | Unique Azure AD tenant identifier, in GUID format. Identifies the customer. |
| 顧客名 | Customer's organization name, as reported in Partner Center. |
| CustomerDomainName | Customer's domain name. このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* |
| Customer Country | 顧客の在住国。 |
| 請求書番号 | 指定されたトランザクションが含まれる請求書番号。 |
| MpnId | MPN identifier of the CSP partner. |
| Reseller MpnId | MPN identifier of the reseller of record for the subscription. |
| 注文 ID | Microsoft コマース プラットフォームでの注文に対する一意の識別子。 Not used for reconciliation. |
| 発注日 | 注文が作成された日付。 |
| ProductId | The identifier for the product. |
| SkuId | The identifier for a particular SKU (stock-keeping unit). |
| AvailabilityId | The identifier for a particular SKU's availability. This shows whether the SKU is available for purchase in the given country, currency, industry segment, etc. |
| SKU Name | 特定 SKU のタイトル。 |
| 製品名 | 製品の名前。 |
| PublisherName | The name of the product's publisher.
| PublisherID | Unique identifier for a particular publisher. |
| Subscription Description | サブスクリプションのフレンドリ名。 |
| サブスクリプション ID | Microsoft コマース プラットフォームでのサブスクリプションの一意の識別子。 Not used for reconciliation. *This identifier is not the same as the **Subscription ID** on the partner admin console.* |
| ChargeStartDate | 課金の開始日。 時刻は常に、その日の始まりの時刻 (0:00) になります。 |
| ChargeEndDate | 課金の終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 |
| Term and Billingcycle | The term length and billing cycle for the purchase (for example, *1 Year, Monthly*). |
| 請求の種類 | 課金または調整の種類。 |
| 単価 | The unit price as published in the price list at the time of purchase. *Be sure this matches the information stored in your billing system during reconciliation.* |
| Effective Unit Price | 調整が行われた後の単価。 |
| Quantity | ユニット数。 *Be sure this matches the information stored in your billing system during reconciliation.* |
| Unit type | 購入したユニットの種類。 |
| DiscountDetails | 適用可能なすべての割引の説明。 |
| Sub Total | 合計額 (税抜)。 Checks if your subtotal matches your expected total, in case of a discount. |
| Tax Total | Tax amount charge. Based on your market's tax rules and specific circumstances. |
| Total | 合計額 (税込)。 請求書に課税されるかどうかを確認します。 |
| Currency | 通貨の種類。 各課金エンティティの通貨は 1 つのみです。 Make sure this matches your first invoice and check again after any major billing platform updates. |
| AlternateID | An alternative identifier to an **Order ID**. |
