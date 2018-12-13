---
title: Basic (修飾プラン) から新しいバージョンへし、Dynamics 365 Customer Engagement プランの移行 |パートナー センター
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales/Basic (修飾を提供) サブスクリプションから Customer Engagement プランは更新されなくなったことができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968272"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Basic (修飾プラン) から新しいバージョンにし、Dynamics 365 Customer Engagement プランを移行します。

**適用対象**

-  パートナー センター

Dynamics 365 for Sales を 2019 年 1 月 1 日、ユーザーに効果的な Basic (修飾を提供) サブスクリプションから Customer Engagement プランことができますこれらのレガシ プランの更新できなく/。期限が切れたとき、既存のサブスクリプションは自動的に更新されません。 サブスクリプションの詳細ページで、サブスクリプションの状態は、「自動更新 [日付]」から「有効期限 [日付]」に変更されます。 


顧客の継続性を確認するを以下に、サポートされているオプション近づいたサブスクリプションを持つを移行する必要があります。 お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。

API (CREST またはパートナー センター) を使用する場合、自動と共に、サブスクリプションの終了日を評価することによって有効期限が切れるサブスクリプションの更新を検索できます = False プロパティ。 対象のサブスクリプションは自動的に設定されます renew = False 2019 年 1 月 1 日にします。 パートナー様はお客様をいつでも新しいプランに移行することができます。 

### <a name="the-dynamics-365-offers-being-retired"></a>廃止される Dynamics 365 をプランします。

- Dynamics 365 販売 Enterprise Edition CRMOL basic (修飾プラン)
- Dynamics 365 for Faculty 販売 Enterprise エディション CRMOL basic (修飾プラン)
- Dynamics 365 for Students 販売 Enterprise エディション CRMOL basic (修飾プラン)
- Dynamics 365 販売 Enterprise Edition (政府機関向け価格) CRMOL basic (修飾プラン)
- CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション
- 教職員用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション
- 学生用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディション
- CRM Basic (修飾プラン) 用の SA から Dynamics 365 を販売 Enterprise エディションの (政府機関向け価格)
- Dynamics 365 販売 Enterprise エディションのアドオンの CRM basic (修飾プラン)
- Dynamics 365 販売 Enterprise エディションのアドオンの教職員用の CRM basic (修飾プラン)
- Dynamics 365 販売 Enterprise エディションのアドオンの学生用の CRM basic (修飾プラン)
- Dynamics 365 販売 Enterprise Edition (政府機関向け価格) アドオンの CRM basic (修飾プラン)
- Dynamics 365 顧客契約計画 Enterprise Edition CRMOL Basic (修飾プラン)
- Dynamics 365 顧客契約計画 Enterprise Edition (政府機関向け価格) CRMOL Basic (修飾プラン)
- Dynamics 365 顧客エンゲージメント計画 Enterprise Edition CRMOL Basic (修飾プラン) for Students
- Dynamics 365 顧客エンゲージメント計画 Enterprise Edition CRMOL Basic (修飾プラン) for Faculty
- CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション
- Dynamics 365 顧客契約計画 Enterprise エディション (政府機関向け価格) CRM Basic (修飾プラン) 用の SA から
- 学生用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション
- 教職員用の CRM Basic (修飾プラン) 用の SA から Dynamics 365 顧客契約計画 Enterprise エディション
- Dynamics 365 顧客契約計画 Enterprise エディションのアドオン CRM Basic (修飾プラン)
- Dynamics 365 顧客契約計画 Enterprise Edition (政府機関向け価格) のアドオン CRM Basic (修飾プラン)
- Dynamics 365 顧客契約計画 Enterprise エディションのアドオン学生用の CRM Basic (修飾プラン)
- Dynamics 365 顧客契約計画 Enterprise エディションのアドオン教職員用の CRM Basic (修飾プラン)



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/計画 (修飾を提供) Basic 代替から Customer Engagement プラン

**廃止されたプラン**   

- Dynamics 365 for Sales から CRM Basic または CRMOL (修飾プラン)
- CRM Basic または CRMOL (修飾プラン) から Dynamics 365 Customer Engagement プラン

**代替オプション**
- Dynamics 365 の販売 Professional (新機能)
- Dynamics 365 の販売 Professional (新機能)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement プランまたは
- Dynamics 365 チームのメンバー



## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

廃止された Sku から顧客を新しいものを移動するには、この順序で、次の手順が必要です。

- 新しいサブスクリプションを購入する
- 現在のユーザー ライセンスをもう一度割り当てる
- 以前のサブスクリプションを取り消す

## <a name="purchase-the-new-plan-for-your-customer"></a>顧客の新しいプランを購入します。

1. 左側のナビゲーションから**顧客**を選択し、新しいサブスクリプションを移行する顧客を選択します。
2. **[サブスクリプションの追加**を選択します。
3. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。 

顧客以前のサブスクリプションと新しいの 1 つの両方がされます。 次の手順では、顧客のユーザーへのライセンスをもう一度割り当てます。

1. 左側のナビゲーションから**顧客**を選択し、移動する顧客を選択します。
2. **[ユーザーとライセンス]** を選びます。
3. ユーザーにライセンスを再割り当てするには、ユーザーを選択し、**ライセンスの管理**を選択します。 
4. **ライセンスの管理**] ページで、クリア for Sales、Dynamics 365/Basic (修飾提供) から Customer Engagement プランのライセンスのチェック ボックスと、お客様の移行先サブスクリプションの新しいサービス プランを選択します。 
5. **[送信]** を選びます。 これは、新しいライセンスを必要とする各ユーザーの行います。 

新しいサブスクリプションを経由でライセンスを移動した後は、以前のサブスクリプションを取り消すことができます。 

1. 左側のナビゲーションから**顧客**を選択し、移動する顧客を選択します。
2. サブスクリプションの詳細ページでは、以前のサブスクリプションを**中断**に設定し、**送信**を選択します。

以前のサブスクリプションが一時停止できるようになりましたと新しいサブスクリプションがアクティブになっています。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 顧客が以前のサブスクリプションの追加コストが発生しません。
 

 



