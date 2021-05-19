---
title: Dynamics 365 Business Edition の移行
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 有効期限が切れる前に、資格のある Dynamics 365 Business Edition オファーを新しいバージョンに移行する方法について学習します。
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151527"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Dynamics 365 Business Edition プランの新しいバージョンへの移行

**適切なロール**: グローバル管理者|ユーザー管理管理者|管理エージェント |セールス エージェント

2019 年 1 月 1 日より、Dynamics 365 Business Edition サブスクリプションをお持ちのお客様は、これらのレガシ オファーに更新できなくなりました。既存のサブスクリプションは、有効期限が切れると自動的に更新されません。 サブスクリプションの詳細ページで、サブスクリプションの状態が "[日付] の自動更新" から "[日付] に有効期限が切れる" に変わります。

顧客の継続性を確保するには、サブスクリプションの有効期限が切れているユーザーを、以下に示すサポートされているオプションに移行する必要があります。 顧客のサービス停止を回避するために、サブスクリプションの年間終了日より前に顧客を新しいサブスクリプションに移行することをお勧めします。

API (THE または パートナー センター) を使用する場合は、サブスクリプションの終了日を自動更新 = False プロパティと共に評価することで、期限切れのサブスクリプションを見つける可能性があります。 問題のサブスクリプションは、2019 年 1 月 1 日に auto renew=False に設定されます。 お客様は、いつでも新しいプランに移動できます。 

## <a name="the-dynamics-365-business-editions-being-retired"></a>廃止される Dynamics 365 Business Edition

- Dynamics 365 for Finance and Operations (Business Edition)
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central - Dynamics 365 Business Edition の新しいオファー

新しい Dynamics Business Central オファーを使用すると、顧客は財務、販売、サービス、運用を接続して、ビジネス プロセスを効率化し、顧客とのやり取りを改善し、より良い意思決定を行えます。 Dynamics 365 Business Central はクラウドベースであり、クラウド ソリューション プロバイダー (CSP) プログラム パートナーのみを通じて利用できます。
Dynamics 365 Business Edition のお客様は、2020 年 6 月 30 日まで、新しい Business Central オファーの割引切り替え価格を受け取る資格があります。

## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

 廃止された SKU から新しい SKU に顧客を移行するには、この順序で次の手順が必要です。

- 新しいサブスクリプションを購入する
- 現在のユーザー ライセンスをもう一度割り当てる
- 以前のサブスクリプションを取り消す

## <a name="purchase-the-new-plan-for-your-customer"></a>顧客の新しいプランを購入する

1. 左側 **のナビゲーション** から [顧客] を選択し、新しいサブスクリプションに移動する顧客を選択します。
2. [サブスクリプション **の追加] を選択します**。
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
