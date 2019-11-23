---
title: Invoice files | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Understand the fields in your invoice file for Partner Center billing.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: billing, invoice
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389840"
---
# <a name="invoice-files"></a>Invoice files

You can use the following tables to understand the fields in Partner Center invoice files.

## <a name="invoice-file-fields"></a>Invoice file fields

The following fields appear on your invoice files.

| フィールド | 定義 |
| ----- | ---------- |
| US FEIN | Your Federal Employer Identification Number (FEIN). This is your United States federal tax identifier number. |
| 顧客番号 | お客様の番号。 |
| 請求先 | 請求書の送付先となる住所。 You can change your company name and/or address in your Partner Center billing profile. |
| ライセンスベースの料金 | The flat monthly or annual charges for your purchased usage-based licenses, billed in advance of the service. This number is the sum of all charges in the **Subtotal** column (column **T**) in your license-based reconciliation file. |
| 使用量ベースの料金 | Your Azure usage. This includes new services or applications enabled and used during the billing period. This number is the sum of all charges in the **PretaxCharges** column (column **Z**) in your usage-based reconciliation file. |
| 割引 | The discount that the customer receives from subscription's normal price. This number is shown as a *flat amount*, not as a price per unit or license. |
| クレジット | Credits or adjustments for changes made to subscriptions (for example, seat increases or decreases). |
| Subtotal | 課税前の税抜き料金とクレジットの合計。 |
| Tax | The total tax for your current charges, as totaled in the **Details** section beginning on page 2 of your invoice. This number is the sum of all charges in the **TaxAmount** column (column **AA**) in your usage-based reconciliation file, and the **Tax** column (column **U**) in your license-based reconciliation file. |
| その他のクレジット | 税抜きクレジット。 |
| 当月の請求額合計 | The amount due in your billing currency for the billing period. These charges are due by the payment due date. |
| お支払いについて | Description of how to pay your invoice, based on your region. *Always be sure to include your invoice number when making a payment.* |
| 請求書番号 | 請求書の番号。 |
| 課金期間 | 請求日に至るまでの月単位の期間。 これは、クレジットの調整またはライセンス数の変更のための、使用量ベースのサービスが消費された期間、またはライセンス ベースのサービスが調整された期間です。 |
| 請求書作成日 | The billing date or anniversary date on which your invoice is generated each month. |
| 支払条件 | The payment term. 1 回限りの購入の場合は、常に 60 日間になります。 |
| 支払期日 | The date by which your payment must be received. |
| 顧客 PO | Your purchase number order. |
| カスタマー サービス | The website address where you can access customer service. |
| サービス利用者 | The address where the service is being used. (これは、会社の審査に関連付けられている会社の正式な住所です。) |

## <a name="one-time-charges-fields"></a>One-time charges fields

The following fields only apply to **one-time charges** in Partner Center:

| フィールド | 定義 |
| ----- | ---------- |
| 日付 | 購入日。 |
| 説明 | 製品名。 |
| Quantity | The number of products (such as reservations) purchased. |
| 単価 | Price per product (such as a reservation). |
| 割引 | 適用される割引。 |
| 税抜き額 | 課税前の購入額の小計。 |
| 売上税 | 税額。 |
| Total | Total amount to be paid. |
