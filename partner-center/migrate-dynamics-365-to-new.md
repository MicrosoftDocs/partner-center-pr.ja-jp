---
title: Dynamics 365 Business Edition には新しいバージョンに移行 |パートナー センター
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 Business Edition のサブスクリプションを更新することが不要になったことができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 プラン、オファー、新しい Dynamics 365 の Sku を更新します。
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584625"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition プランの新しいバージョンへの移行 

**適用対象**

- パートナー センター

これらの従来の製品に Dynamics 365 Business Edition のサブスクリプションを持つ有効な 2019 年 1 月 1日顧客を更新できなく有効期限が切れるときに、既存のサブスクリプションは自動的に更新されません。 サブスクリプションの詳細] ページで、サブスクリプションの状態は、「自動更新 [date]」から「有効期限 [date]」に変更されます。

お客様の継続性をできるように、以下に、サポートされているオプションに期限切れのサブスクリプションのあるものを移行する必要があります。 お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。

(CREST またはパートナー センター) API を使用する場合、自動と共にサブスクリプションの終了日を評価することによって期限切れのサブスクリプションの更新を見つけることができます = False プロパティ。 対象のサブスクリプションは自動に設定されます更新 = False、2019 年 1 月 1 日を。 お客様は、いつでも新しいプランに移動できます。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>提供が中止される Dynamics 365 Business Edition

- Dynamics 365 for Finance and Operations、Business edition
- Dynamics 365 Business edition、チーム メンバー

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics ビジネス中部 - Dynamics 365 Business Edition の新しいプラン

新しい Dynamics Business Central で提供では、お客様は、財務、sales、サービス、およびビジネス プロセスの合理化、顧客とのやり取りを改善する操作を接続しより優れた意思決定します。 Dynamics 365 Business Central では、クラウド ベースでクラウド ソリューション プロバイダー (CSP) プログラムのパートナーのみで使用できる説明です。
Dynamics 365 Business Edition のお客様は割引の遷移が新しい Business Central の価格を受信するが、2020 年 6 月 30日まで提供しています。

## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

 提供終了になった Sku から新しいものに顧客を移動すると、この順序で次の手順が必要です。

- 新しいサブスクリプションを購入する
- 現在のユーザー ライセンスをもう一度割り当てる
- 以前のサブスクリプションを取り消す

## <a name="purchase-the-new-plan-for-your-customer"></a>お客様の新しいプランを購入します。

1. 選択**顧客**から、左側のナビゲーションし、新しいサブスクリプションに移動する顧客を選択します。
2. 選択**サブスクリプション追加**します。
3. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。 

古いサブスクリプションと、新しい顧客になりますようになりました。 次の手順では、お客様のユーザーにライセンスを再割り当ています。

1. 選択**顧客**から、左側のナビゲーションと選択し、顧客が移動します。
2. **[ユーザーとライセンス]** を選びます。
3. ユーザーにライセンスを再割り当てするユーザーを選択し、**ライセンスを管理する**します。 
4. **ライセンスを管理する** ページで、Dynamics 365 for Sales の消去/(修飾提供) Basic から Customer Engagement プランのライセンスのチェック ボックスとへの移行は、顧客サブスクリプションの新しいサービス プランを選択します。 
5. **[送信]** を選びます。 これは、新しいライセンスが必要とする各ユーザーの行います。 

経由でライセンスを新しいサブスクリプションに移行した後は、古いサブスクリプションをキャンセルできます。 

1. 選択**顧客**から、左側のナビゲーションと選択し、顧客が移動します。
2. サブスクリプションの詳細 ページで、古いサブスクリプションを設定**Suspended**選択**送信**します。

古いサブスクリプションが中断されていますし、新しいサブスクリプションがアクティブにします。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 お客様には、古いサブスクリプションの追加のコストは生じません。