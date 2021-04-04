---
title: Dynamics 365 Business Edition の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有効期限が切れる前に、限定された Dynamics 365 Business Edition のプランを新しいバージョンに移行する方法について説明します。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132640"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition プランの新しいバージョンへの移行

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 管理エージェント
- 販売代理店

2019年1月1日より、Dynamics 365 Business Edition サブスクリプションをお持ちのお客様は、これらの従来のプランに更新できなくなります。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。 サブスクリプションの詳細ページで、[日付] の [自動更新] の [日付] にサブスクリプションの状態が [有効期限切れ] に変わります。

顧客の継続性を確保するには、有効期限が切れたサブスクリプションを使用して、以下のサポートされているオプションに切り替える必要があります。 顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。

API (CREST またはパートナーセンター) を使用する場合は、サブスクリプションの終了日と自動更新 = False プロパティを評価することで、有効期限が切れたサブスクリプションを見つけることができます。 該当するサブスクリプションは、2019年1月1日に自動更新 = False に設定されます。 お客様は、いつでも新しいプランに移動できます。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 Business Edition が廃止されています

- Dynamics 365 for Finance and Operations (Business Edition)
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central-Dynamics 365 Business Edition の新しいプラン

新しい Dynamics Business Central を利用することで、お客様は財務、営業、サービス、操作を接続して、ビジネスプロセスを効率化し、顧客とのやり取りを改善し、より良い意思決定を行うことができます。 Dynamics 365 Business Central はクラウドベースであり、クラウドソリューションプロバイダー (CSP) プログラムパートナーのみが利用できます。
Dynamics 365 Business Edition のお客様は、2020年6月30日まで、新しい Business Central プランに対する割引された移行料金を受け取ることができます。

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
