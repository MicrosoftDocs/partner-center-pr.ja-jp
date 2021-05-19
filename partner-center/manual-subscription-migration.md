---
title: Qualified Dynamics 365 サブスクリプションの移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 既存のサブスクリプションの有効期限が切れる前に、qualified、basic Dynamics 365 サブスクリプションから新しいサブスクリプションに移行する方法について説明します。
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151646"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Dynamics 365 および Customer Engagement プランの Basic (対象プラン) から新しいバージョンへの移行

**適切なロール**: 全体管理者 |ユーザー管理の管理者 |管理エージェント |営業担当者

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
- CRM Basic の Dynamics 365 for Sales Enterprise Edition Add-On (修飾プラン)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (資格のあるオファー) for Faculty
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (修飾オファー) for Students
- Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (限定オファー)
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (限定オファー)
- Dynamics 365 Customer Engagement プラン Enterprise Edition (Government 価格) CRMOL Basic (限定オファー)
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (限定オファー) for Students
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRMOL Basic (資格のあるオファー) for Faculty
- Dynamics 365 Customer Engagement プラン Enterprise Edition SA for CRM Basic (限定オファー) から
- Dynamics 365 Customer Engagement プラン Enterprise Edition (Government 価格) FROM SA for CRM Basic (限定オファー)
- Dynamics 365 Customer Engagement プラン Enterprise Edition SA for CRM Basic (資格のあるオファー) から受講者向けプラン
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRM Basic (資格のあるオファー) for Faculty の SA から
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (限定オファー)
- Dynamics 365 Customer Engagement プラン Enterprise Edition CRM Basic (限定オファー) Add-On (Government 価格) プラン
- Dynamics 365 Customer Engagement プラン Enterprise Edition Add-On CRM Basic (適格オファー) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (資格のあるオファー) for Faculty



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/ Customer Engagement Plan from Basic (修飾オファー) 交換プラン

**廃止されたオファー**   

- Dynamics 365 for Sales from CRM Basic または CRMOL Basic (限定オファー)
- CRM Basic または CRMOL Basic (限定オファー) の Dynamics 365 Customer Engagement プラン

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
2. [ **サブスクリプションの追加**] を選択します。
3. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。 

これで、お客様は古いサブスクリプションと新しいサブスクリプションの両方を使用できるようになります。 次の手順では、顧客のユーザーにライセンスを再割り当てします。

1. 左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。
2. [ **ユーザーとライセンス**] を選択します。
3. ライセンスをユーザーに再割り当てするには、ユーザーを選択し、[ **ライセンスの管理**] を選択します。 
4. [ **ライセンスの管理** 365] ページで、[Basic (限定されたプラン) のライセンス] チェックボックスをオンにして、顧客が移動しているサブスクリプションの新しいサービスプランを選択します。 
5. **[Submit]\(送信\)** をクリックします。 この操作は、新しいライセンスが必要なユーザーごとに行います。 

新しいサブスクリプションにライセンスを移行したら、古いサブスクリプションを取り消すことができます。 

1. 左側のナビゲーションから [ **Customers** ] を選択し、移動する顧客を選択します。
2. [サブスクリプションの詳細] ページで、古いサブスクリプションを " **中断** " に設定し、[ **送信**] を選択します。

古いサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 お客様には、古いサブスクリプションに対して追加料金は発生しません。
 

 



