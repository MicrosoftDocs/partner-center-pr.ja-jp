---
title: 請求の概要 | パートナー センター
ms.topic: article
ms.date: 11/21/2019
description: Basic billing and invoice information for Partner Center.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: 請求, 支払い,注文,取り消し, 注文管理, 未払い, 詐欺, 不正使用, 税, 税額控除, 調整ファイル, 調整用のファイル
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 10fe47ea038fadf8ca26fe0ab42a0d0d3a9472bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384548"
---
# <a name="billing-overview"></a>請求の概要

適用対象:

- パートナー センター
- Partners in the Cloud Solution Provider (CSP) program

## <a name="find-your-bill"></a>Find your bill

To find your bill:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Billing**.
3. On the **Billing** page, you can download your latest bill or download previous bills in the **Billing history** section.

## <a name="bill-your-customers"></a>Bill your customers

Microsoft has no requirements or conditions about how you handle your own invoicing.

To determine a customer's usage, [see your reconciliation files](#find-your-bill). You can use the customer name and other relevant fields to determine usage.

Next, you can add your own fees and charges for services and products that you provide. Then, you can send a single bill for all charges to your customer.

### <a name="billing-types"></a>Billing types

Billing types in Partner Center include **license-based billing**, **usage-based billing**, and **one-time billign**. For more information, see the full explanation of [billing types in Partner Center](billing-different-types.md).

### <a name="billing-currency"></a>Billing currency

You'll be billed for product(s) in the currency of the country or region in which you're located. You're billed the same regardless of the location of the customer to whom you sold the product(s).

## <a name="invoices"></a>請求書

Your invoice is a summary of all charges for the current billing period. This includes charges across the program, all products, and all customers. For examples of monthly and annual billing scenarios, see [common billing scenarios](common-billing-scenarios.md)

Your invoice is available within two (2) days of your selected billing date in UTC time. たとえば、請求日が 9 月 12 日の場合、請求書生成プロセスは 13 日の午前 0 時 00分 UTC に開始し、14 日の午前 0 時 00分 UTC に完了します。 15 日の午後 11 時 59 分 UTC までに請求書が表示されない場合は、サービス レベル アグリーメントが満たされていないので、サービス要求を提出する必要があります。

Partners in the Cloud Solution Provider (CSP) program who choose to be billed monthly pay Microsoft 60 days in arrears for their customers' subscriptions (both license-based and usage-based).

## <a name="price-lists"></a>Price lists

Price lists are updated monthly. Preview price lists are available one (1) month in advance.

To view price lists:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Sell**, then select **Pricing and offers**.
3. On the **Pricing and offers** page, you can see 6 months of price lists (including the current month) and preview price lists (where applicable).

**License-based** prices are guaranteed for the term of the subscription, usually 12 months from the purchase date. 

**Usage-based prices** can change on a monthly basis.

**Prices for products, services, and software subscriptions** are guaranteed through the subscription duration. However, prices may change when you renew.

You'll see **adjustments** and **credits** in arrears on your next billing invoice after the credit or adjustment is applied.

## <a name="payment-terms"></a>支払条件

支払期間は正味 60 日です。 請求書の期限 (請求日から 60 日) までに支払う必要があります。それを過ぎると、アカウントは延滞になり、CSP での登録に影響する可能性があります。 

支払い期限の過ぎた未払い額を支払うと、中断されているアカウントのすべての機能を復旧できます。

### <a name="taxes-and-vat"></a>Taxes and VAT

You are taxed based on your details (not your customers' details) because the billing relationship is between Microsoft and you. You can submit your tax identifier during the account setup process or through a support request later. 料金は次の課金サイクルに反映されます。

For **withholding and sales tax exemption**, you must submit tax documentation through a support request. 料金と適切な返金は次の課金サイクルに反映されます。

For **value-added tax (VAT) exemption**, you must submit your VAT ID (validated by Microsoft) through a service request. 料金と適切な返金は次の課金サイクルに反映されます。

さらに詳しい税金の詳細については、地域の税務署または税務アドバイザーにお問い合わせください。

### <a name="annual-billing-rules"></a>Annual billing rules

サブスクリプションは毎年自動更新されます。

請求は、年間サブスクリプションごとに 12 回の月払いまたは 1 回の年払いになります。

以前の課金期間の終了時のライセンス数に基づいて、ライセンス ベースのサービスの次の課金期間について前払いで課金されます。

ライセンス数の変更 (ライセンスの日数に基づく日割り計算) で、後で課金/クレジットが行われます。 Pro-rata calculation uses the following formula:

`[ROUND((ROUND(Unit Price * Quantity / Number of days in pro-rated Month, 2) * Number of pro-rated days) / Quantity, 2) * Quantity]`

Payments are billed for licenses sold, not licenses provisioned.

### <a name="change-billing-frequency"></a>Change billing frequency

To change the billing frequency of an online service for a customer:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. In the left-hand menu, choose **Customers**.
3. Select the customer whose subscription billing frequency you want to change.
4. On the customer's **Subscriptions** page, select the subscription that you want to change.
5. On the **Details** page, under **Billing frequency**, select **Monthly** or **Annual**. 請求頻度の変更に関する重要な情報と、変更されるサブスクリプションの一覧を含む、確認ページが表示されます。
6. Choose **OK** to make the change (or **Cancel** to undo it).

### <a name="adjustmentscreditscancellations"></a>調整/クレジット/取り消し

ライセンスベースのサービスの取り消しに対して、早期終了手数料は課金されません。

Cancellation credits for licensed-based services are pro-rated for unused days for mid-cycle cancellations (as well as license decreases according to the formula above).

### <a name="billing-rules"></a>課金の規則

サブスクリプションは新しい従量制サービスの料金で、毎月自動的に更新されます。 毎月、前月の使用量に対して請求されます。

従量制サービスの料金は、請求サイクル内で変更される場合があります。

#### <a name="price-changes"></a>Price changes

For **price increases**, 30 days' notice is provided.

**Price decreases** are reflected on the day of change.

**Existing subscriptions** use the rate in effect at the beginning of the bill cycle.

**New subscriptions**, when created within the same billing cycle, use the rate in effect on the date you create them. 

### <a name="adjustmentscreditscancellations"></a>調整/クレジット/取り消し

支払いの調整は、次の月次請求書に表示されます。

使用量ベースのサービスの取り消しに対して、早期終了手数料は課金されません。 

SLA のクレジットを含むあらゆる種類のクレジットが、次の月次請求書に表示されます。

>[!IMPORTANT]
>通貨が異なる場所の顧客用に Azure Reservations およびソフトウェア サブスクリプションを購入する場合、既定の請求通貨はパートナーではなく顧客の場所がベースになります。 顧客が複数の場所に存在する場合は、顧客への請求が必要な各通貨について、個別の請求書と調整ファイルが届き、適切な通貨で顧客に請求できます。

## <a name="manage-one-time-billing"></a>Manage one-time billing

### <a name="billing-status-invoices-and-reconciliation-files"></a>Billing status, invoices and reconciliation files

To view your current billing status, invoices, and reconciliation files:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. On the left-hand menu, choose **Billing**, then select **One time**.
3. On the billing status page, select an invoice or reconciliation file to view more detailed information.

### <a name="customer-order-history"></a>Customer order history

To view a customer's order history:

1. [Sign in to the Partner Center dashboard](https://partner.microsoft.com/dashboard/home).
2. On the left-hand menu, choose **Customers**.
3. On the **Customers** page, find the customer whose order history you want to view. Select the down arrow to expand the customer's record.
4. Choose **View orders** to display the customer's order history.

### <a name="credit-notes"></a>Credit notes

You might need to request a credit or rebill for the following reasons:

- You need to make address or purchase order corrections.
- A tax refund was applied after the invoice was generated. You can request a credit or rebill to get the tax refund pulled back into the original invoice. The same is also true for refunds. You can request a credit or rebill of the original invoice, then pull in a refund.

If you request a credit or rebill, we'll give you a **credit note** to cancel the original invoice.
