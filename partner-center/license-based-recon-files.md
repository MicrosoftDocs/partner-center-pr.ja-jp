---
title: License-based reconciliation files | Partner Center
ms.topic: article
ms.date: 11/21/2019
description: Understand license-based reconciliation files in Partner Center.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 617b49556851a4d9999e6294d61d79c4fe1befa1
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389820"
---
# <a name="license-based-reconciliation-files"></a>ライセンス ベースの調整ファイル

適用対象:

- パートナー センター
- 米国政府機関向け Microsoft Cloud のパートナー センター

To reconcile your changes against a customer's orders, compare the **Syndication_Partner_Subscription_Number** from the reconciliation file against the **Subscription ID** from Partner Center.

## <a name="fields-in-license-based-reconciliation-files"></a>Fields in license-based reconciliation files

| Column | 説明 | サンプル値 |
| ------ | ----------- | ------------ |
| PartnerId | Unique identifier in GUID format for a specific billing entity. Not required for reconciliation. すべての行で同じです。 | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerID | Unique Microsoft identifier for the customer in GUID format. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Microsoft 課金プラットフォームでの注文の一意の識別子。 May be useful to identify the order when contacting support. Not used for reconciliation. | *566890604832738111* |
| SubscriptionID | Microsoft 課金プラットフォームでのサブスクリプションの一意の識別子。 May be useful to identify the subscription when contacting support. Not used for reconciliation. *This value is not the same as the **Subscription ID** on the Partner Admin Console. Please see **SyndicationPartnerSubscriptionNumber** instead.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | サブスクリプションの一意の識別子。 A customer can have multiple subscriptions for the same plan. This column is important for reconciliation file analysis. This field maps to the **Subscription ID** in the Partner Admin Console. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferID | Unique offer identifier. Standard offer identifier, as defined in the price list. *This value does not match **Offer ID** from the price list. See **DurableOfferID** instead.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Unique durable offer identifier, as defined in the price list. *This value matches the **Offer ID** from the price list.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | 価格表で定義されている、顧客が購入したサービス プランの名前 | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | The subscription start date. 時刻は常に、その日の始まりの時刻 (0:00) になります。 This field is set to the day after the order was submitted. Used in conjunction with the **SubscriptionEndDate** to determine: if the customer is still within the first year of the subscription, or if the subscription has been renewed for the following year. | *2/1/2019 0:00* |
| SubscriptionEndDate | The subscription end date. 時刻は常に、その日の始まりの時刻 (0:00) になります。 Either *12 months plus **x** days after the start date* to align with the partner's billing date or *12 months from the renewal date*. 更新時に、価格は最新の価格表に更新されます。 自動更新の前に、顧客とのやり取りが必要になる場合があります。 | *2/1/2019 0:00* |
| ChargeStartDate | 課金の開始日。 時刻は常に、その日の始まりの時刻 (0:00) になります。 Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/1/2019 0:00* |
| ChargeEndDate | 課金の終了日。 時刻は常に、その日の終わりの時刻 (23:59) になります。 Used to calculate daily charges (*pro rata* charges) when a customer changes seat numbers. | *2/28/2019 23:59* |
| ChargeType | The [type of charge](recon-file-charge-types.md) or adjustment. | See [charge types](recon-file-charge-types.md). |
| UnitPrice | シート単価 (購入時に価格表に公開されていた価格)。 Be sure this matches the information stored in your billing system during reconciliation. | *6.82* |
| Quantity | シート数。 Be sure this matches the information stored in your billing system during reconciliation. | *2* |
| Amount | 数量に対する合計価格。 Used to check if the amount calculation matches how you calculate this value for your customers. | *13.32* |
| TotalOtherDiscount | これらの料金に適用される割引額。 Product licenses included with a competency or MAPS, or new subscriptions eligible for an incentive, will also contain a discount amount in this column. | *2.32* |
| Subtotal | 合計額 (税抜)。 Checks if your subtotal matches your expected total, in case of a discount. | *11* |
| Tax | Tax amount charge. Based on your market's tax rules and specific circumstances. | *0* |
| TotalForCustomer | 合計額 (税込)。 請求書に課税されるかどうかを確認します。 | *11* |
| Currency | 通貨の種類。 各課金エンティティの通貨は 1 つのみです。 Check if it matches your first invoice. Check again after any major billing platform updates. | *EUR* |
| CustomerName | Customer's organization name, as reported in Partner Center. *Very important field for reconciling the invoice with your system information.* | *Test Customer A* |
| MPNID | MPN identifier of the CSP partner. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | MPN identifier of the reseller of record for the subscription. See [how to itemize by partner](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Customer's domain name. このフィールドは、2 回目の請求サイクルまで空白になる可能性があります。 *Don't use this field as a unique identifier for the customer. The customer/partner can update the vanity or default domain through the  Office 365 portal.* | *example.onmicrosoft.com* |
| SubscriptionName | サブスクリプションのニックネーム。 If no nickname is specified, Partner Center uses the **OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | 価格表で定義されている、顧客が購入したサービス プランの名前 (This is an identical field to **OfferName**.) | *PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT* |
