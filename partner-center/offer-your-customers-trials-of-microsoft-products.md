---
title: Microsoft 製品の試用版を顧客に提供する | パートナー センター
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客は、Microsoft サブスクリプション製品を 30 日間テストすることができます。 他の多くのオンライン サービスと同様、カタログ内の試用版にサインアップします。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384833"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Microsoft 製品の試用版を顧客に提供する

適用対象:

- パートナー センター

新しい Microsoft 製品を顧客に紹介する効果的な方法として、30 日間の無料試用版を提供できます。 他の多くのオンライン サービスと同様、カタログ内の試用版にサインアップします。 すべてのパートナーが参加できます。

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. たとえば、Office 365 Business Premium の無料試用版 を 1 つ、Office 365 E3 の無料試用版を 1 つ取得できます。 However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

無料試用版は、以下の製品について提供が可能です。

- Office 365 Business Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Dynamics 365 Customer Engagement Plan 1
- Dynamics 365 for Financials
- Microsoft 365 Business

最も人気のある包括的なビジネス製品に、無料試用版が提供されています。 今後、他の製品についても、無料試用版プランが追加される可能性があります。

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. パートナー センターの **[Sell]\(販売\)** から **[Catalog]\(カタログ\)** に移動します。 
2. カタログで、 **[請求頻度]** から **[試用版プラン]** をクリックします。 これにより、無料試用版の表示のみが有効になり、他の無料ではないプランは無効になります。 試用版は、カタログの **[試用版]** タブに表示されます。
3. 提供する無料試用版を選択し、 **[送信]** を選択します。 すべての試用版は、30 日間請求がありません。 試用期間中いつでも有料サブスクリプションに切り替えることができます。

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. お客様のサブスクリプション ページに移動し、無料試用版を選びます。
2. **[試用版を有料サブスクリプションに変換]** を選びます。
3. 必要なライセンス数と請求頻度を入力し、 **[適用]** を選びます。
4. 有料サブスクリプションの請求は変換日に開始し、サブスクリプションは変換日から 12 か月後に自動更新されます。 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [試用版サブスクリプションを有料版に変換する](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [試用版の変換プランの一覧を取得する](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. パートナー様は、有効期限日を頻繁に確認し、有料版への切り替えを決める時期が近付いたお客様に対して、適切なフォローアップを行うことをお勧めします。

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>請求

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. 無料試用版が年次請求の有料プランに切り替えられた場合、サブスクリプションの更新日は切り替え日から 12 か月後です。 無料試用版が月次請求の有料プランに切り替えられた場合、サブスクリプションの更新日は切り替え日の次の請求日から 12 か月後です。

### <a name="invoices"></a>請求書

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>インセンティブ

Free trials do not have an impact on incentives.

## <a name="support"></a>サポート

For support on free trials, submit a service request through Partner Center.
