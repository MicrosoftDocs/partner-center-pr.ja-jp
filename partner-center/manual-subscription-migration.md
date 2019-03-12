---
title: Dynamics 365 と顧客エンゲージメント プランを Basic (修飾プラン) から新しいバージョンに移行 |パートナー センター
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales]、[Basic (修飾提供) のサブスクリプションから Customer Engagement プランは更新不要になったことができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 プラン、オファー、新しい Dynamics 365 の Sku を更新します。
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586945"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行

**適用対象**

-  パートナー センター

Dynamics 365 for Sales で効果的な 2019 年 1 月 1日の顧客 (修飾提供) Basic サブスクリプションから Customer Engagement プランですこれらのレガシ プランを更新できなく/。有効期限が切れるときに、既存のサブスクリプションは自動的に更新されません。 サブスクリプションの詳細] ページで、サブスクリプションの状態は、「自動更新 [date]」から「有効期限 [date]」に変更されます。 


お客様の継続性をできるように、以下に、サポートされているオプションに期限切れのサブスクリプションのあるものを移行する必要があります。 お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。

(CREST またはパートナー センター) API を使用する場合、自動と共にサブスクリプションの終了日を評価することによって期限切れのサブスクリプションの更新を見つけることができます = False プロパティ。 対象のサブスクリプションは自動に設定されます更新 = False、2019 年 1 月 1 日を。 お客様は、いつでも新しいプランに移動できます。 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 の提供が中止

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (修飾プラン)
- Dynamics 365 for Faculty 販売の Enterprise Edition CRMOL basic (修飾プラン)
- Dynamics 365 の学生向け販売の Enterprise Edition CRMOL Basic (修飾プラン)
- Dynamics 365 for 販売の Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)
- Dynamics 365 営業の Enterprise Edition 用 CRM Basic (修飾プラン) 用の SA から
- Dynamics 365 営業の Enterprise edition for Faculty CRM Basic (修飾プラン) 用の SA から
- 学生向けの CRM Basic (修飾プラン) 用の SA から売上の Enterprise Edition 用 Dynamics 365
- Dynamics 365 (政府機関向け価格) 販売の Enterprise Edition 用 CRM Basic (修飾プラン) 用の SA から
- Dynamics 365 営業の Enterprise Edition のアドオンの CRM basic (修飾プラン)
- Dynamics 365 営業の Enterprise Edition のアドオンの CRM basic (修飾プラン) for Faculty
- Dynamics 365 営業の Enterprise Edition のアドオンの学生向けの CRM basic (修飾プラン)
- Dynamics 365 営業の Enterprise Edition (政府機関向け価格) のアドオンの CRM basic (修飾プラン)
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン)
- Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン) for Students
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (修飾プラン) for Faculty
- CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition
- Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) CRM の Basic (修飾プラン) 用の SA から
- 学生向けの CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition
- For Faculty CRM Basic (修飾プラン) 用の SA から Dynamics 365 Customer Engagement プラン Enterprise Edition
- Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン CRM basic (修飾プラン)
- Dynamics 365 Customer Engagement プラン Enterprise Edition (政府機関向け価格) アドオン CRM basic (修飾プラン)
- Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン CRM basic (修飾プラン) の学生向け
- Dynamics 365 Customer Engagement プラン Enterprise Edition アドオン for Faculty CRM basic (修飾プラン)



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales]、[プラン (修飾提供) Basic 置換から Customer Engagement の計画

**提供終了になったプラン**   

- CRM Basic または CRMOL (修飾プラン) からの売り上げ高の Dynamics 365
- CRM Basic または CRMOL (修飾プラン) から Dynamics 365 Customer Engagement プラン

**置換オプション**
- Dynamics 365 for Sales Professional (新規)
- Dynamics 365 for Sales Professional (新規)
- Dynamics 365 のカスタマー サービスについて
- Dynamics 365 Customer Engagement プランまたは
- Dynamics 365 のチーム メンバー



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
 

 



