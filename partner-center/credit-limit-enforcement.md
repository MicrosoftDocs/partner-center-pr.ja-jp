---
title: 与信限度額の適用
ms.topic: how-to
ms.date: 05/11/2021
description: クレジット制限と計算方法について学習します。 FAQ が含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cf0d3c38b301c363a4a990db5258cf2a3f30d487
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/12/2021
ms.locfileid: "109819210"
---
# <a name="credit-limit-enforcement-cle"></a>与信限度額の適用 (CLE)

**適切なロール**

- 課金管理者

## <a name="your-credit-limit-and-how-it-works"></a>クレジットの制限と動作

クレジット制限は、パートナーがパートナーとして購入できる最大金額 (米国ドル単位) です。この上限は、パートナー センター。 クレジットの上限を超えると、十分な支払いが行われたまで、新しい購入を行う必要があります。 既存のサブスクリプションは中断されずに続行されます。

クレジット制限は、Azure プラン、Azure 予約、ソフトウェア、Marketplace、Azure 145 P、Office、Dynamics 製品のオファーに適用されます。 クレジット制限は、更新や継続的な消費には適用されません。

オンボード期間中は、テナント レベルでクレジット制限が割り当てされます。 お客様の予測収益、購入力、支払い履歴に基付けています。 次に、次の数式を使用して、使用可能な残高を計算します。

**[与信限度額 – (受信購入 + 未払い請求書 + 未請求料金 – 過払い) ]**

## <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="is-my-credit-limit-set-at-the-tenant-or-global-level"></a>クレジット制限はテナントレベルまたはグローバル レベルで設定されていますか?

テナント レベル。 たとえば、米国、カナダ、日本から運用するとします。 カナダのテナントがクレジット制限に達した場合、そのテナントは、テナントで購入を試みるときに通知を受け取パートナー センター。 その他のテナントは影響を受け "ない"。 

### <a name="if-i-exceed-my-credit-limit-can-i-continue-servicing-existing-customers-and-subscriptions-with-full-access"></a>クレジット制限を超えた場合、フル アクセスで既存の顧客とサブスクリプションにサービスを提供し続けできますか?

はい。 顧客の既存のサブスクリプションは中断することなく継続されます。 ただし、顧客の新しいサブスクリプションを購入することはできません。

### <a name="does-cle-apply-to-both-direct-bill-partners-and-indirect-providers"></a>CLE は直接請求パートナーと間接プロバイダーの両方に適用されますか?

はい。両方に適用されます。

### <a name="after-i-submit-my-payment-to-reinstate-my-account-when-can-i-purchase-more-subscriptions"></a>アカウントを再開するために支払いを送信した後、サブスクリプションを追加購入できる期間 

Microsoft がクレジット チェック プロセスを続行するためにすべての要件を受け取ったと仮定すると、支払いから 24 時間以内に購入を再開できます。

### <a name="how-can-i-check-my-credit-limit"></a>クレジット制限を確認する方法

クレジット制限 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) を確認し、最近の購入に関する情報を取得する場合は、 にお問い合わせください。

### <a name="do-invoices-that-are-in-dispute-count-against-the-credit-limit"></a>クレームに含む請求書は、与信限度額に対してカウントされますか?

はい。 ただし、 で Microsoft に問い合 [ucmwrcsp@microsoft.com](mailto:ucmwrcsp@microsoft.com) わせ、問題を解決することができます。

### <a name="how-soon-will-i-hear-back-if-i-write-to-ucmwrcspmicrosoftcom"></a>に書き込んだ場合、どのくらいの時間が来ますか ucmwrcsp@microsoft.com ?

応答は 24 時間以内に行う必要があります。 

### <a name="what-criteria-does-microsoft-use-for-setting-a-partners-credit-limit"></a>Microsoft はパートナーのクレジット制限を設定するためにどのような基準を使用しますか?

予測収益、購入率、支払い履歴に基づいて、クレジット制限が決定されます。

### <a name="is-the-credit-limit-currently-enforced-on-the-new-commerce-experience"></a>現在、新しいコマース エクスペリエンスに対してクレジット制限が適用されていますか?

はい。 クレジット制限は、すべての CSP プログラムと製品に適用され、パートナー センター。

### <a name="who-will-receive-the-notification-when-my-organization-is-nearing-its-credit-limit"></a>組織が与信限度額に近付いたときに通知を受け取るのは誰ですか?

組織の財務アカウントの支払い担当者が通知を受け取る必要があります。

## <a name="next-steps"></a>次の手順

[課金の基本](./billing-basics.md)
