---
title: Qualified Dynamics 365 サブスクリプションの移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 既存のサブスクリプションの有効期限が切れる前に、qualified、basic Dynamics 365 サブスクリプションから新しいサブスクリプションに移行する方法について説明します。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Dynamics 365 プラン、更新プラン、新しい Dynamics 365 Sku
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795990"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行

**適用対象**

-  パートナー センター

**適切なロール**
-   グローバル管理者
-   ユーザー管理者
-   管理エージェント
-   販売代理店

2019年1月1日より、Basic (認定提供) サブスクリプションの Dynamics 365 for Sales/Customer Engagement プランをお持ちのお客様は、これらのレガシプランを更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。 サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。 

顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。 顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。

API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。 該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。 お客様は、いつでも新しいプランに移動できます。 

### <a name="the-dynamics-365-offers-being-retired"></a>Dynamics 365 の提供終了

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (限定プラン)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for 教職員
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (認定オファー) for Students
- Dynamics 365 for Sales Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)
- Dynamics 365 for Sales Enterprise Edition for CRM Basic (限定プラン)
- Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー) for 教職員
- 学生向けの SA からの Dynamics 365 for Sales Enterprise Edition for CRM Basic (認定オファー)
- Dynamics 365 for Sales Enterprise Edition (Government 価格) From CRM Basic (限定プラン)
- CRM Basic 用 Dynamics 365 for Sales Enterprise Edition アドオン (修飾されるプラン)
- CRM Basic (認定オファー) 用の Dynamics 365 for Sales Enterprise Edition アドオン
- CRM Basic (認定オファー) for Students 用 Dynamics 365 for Sales Enterprise Edition アドオン
- CRM Basic 用 Dynamics 365 for Sales Enterprise Edition (Government 価格) アドオン (修飾されるプラン)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (限定プラン)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) CRMOL Basic (限定プラン)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定オファー) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (認定プラン) (教職員向け)
- Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (限定プラン)
- Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition (Government 価格) (SA for CRM Basic) (限定プラン)
- Dynamics 365 Customer Engagement Plan Enterprise Edition for CRM Basic (認定オファー) for Students
- Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition for CRM Basic (認定オファー) for 教職員
- Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (修飾されるプラン)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government 価格) アドオン for CRM Basic (認定プラン)
- CRM Basic (修飾されるオファー) 用の Dynamics 365 カスタマーエンゲージメントプラン Enterprise Edition アドオン
- Dynamics 365 Customer Engagement Plan Enterprise Edition アドオン for CRM Basic (認定オファー) for 教職員



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Basic (認定オファー) 置換プランからの Sales/Customer Engagement プランの Dynamics 365

**提供終了**   

- CRM Basic または CRMOL Basic (修飾プラン) からの Sales の Dynamics 365
- CRM Basic または CRMOL Basic (限定プラン) からの Dynamics 365 カスタマーエンゲージメントプラン

**置換オプション**
- Dynamics 365 for Sales Professional (新規)
- Dynamics 365 for Sales Professional (新規)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement プランまたは
- Dynamics 365 チームメンバー



## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

廃止された Sku から新しいバージョンに顧客を移動するには、次の手順を順番に実行する必要があります。

- 新しいサブスクリプションを購入する
- 現在のユーザー ライセンスをもう一度割り当てる
- 以前のサブスクリプションを取り消す

## <a name="purchase-the-new-plan-for-your-customer"></a>顧客の新しいプランを購入する

1. 左側のナビゲーションから [ **Customers** ] を選択し、新しいサブスクリプションに移動する顧客を選択します。
2. [**サブスクリプションの追加**] を選択します。
3. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。 

これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。 次の手順では、顧客のユーザーにライセンスを再割り当てします。

1. 左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。
2. [**ユーザーとライセンス**] を選択します。
3. ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[**ライセンスの管理**] を選択します。 
4. [**ライセンスの管理**365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。 
5. **[Submit]\(送信\)** をクリックします。 この操作は、新しいライセンスが必要なユーザーごとに行います。 

新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。 

1. 左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。
2. [サブスクリプションの詳細] ページで、古いサブスクリプションを "**中断**" に設定し、[**送信**] を選択します。

古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 お客様には、古いサブスクリプションに対して追加料金は発生しません。
 

 



