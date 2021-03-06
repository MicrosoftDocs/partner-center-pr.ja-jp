---
title: Skype for Business サブスクリプションの移行
description: 有効期限が切れた Skype for Business Online プラン1サブスクリプションを持つ特定の顧客を新しい Office 365 バージョンに移行する方法とタイミングについて説明します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: a8de5b824a24b07607b5365848ec1027ca0d08e8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551539"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Skype for Business Online プラン 1 サブスクリプションの新しい Office 365 バージョンへの移行

**適切なロール**: Sales agent

Skype for Business Online プラン1は、2018年8月1日をもって廃止される予定です。 この日付以降、新たに Skype for Business プラン 1 のサブスクリプションを購入することはできません。既存のサブスクリプションは、有効期限になると自動更新されず、更新のオプションは提供されません。 サブスクリプションの詳細ページでは、Skype for Business Online プラン 1 のサブスクリプションの状態が、"自動更新: [日付]" から "有効期限: [date]" に変更されています。  

お客様への継続的なサービス提供のためには、有効期限が迫っている Skype for Business Online プラン 1 のサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。 顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。 

>[!NOTE]
>Skype for Business Online プラン 1 の商用 SKU と行政機関用 SKUは、どちらも提供終了となります。

API (コマース REST (CREST) またはパートナーセンター) を使用する場合は、サブスクリプションの終了日を自動更新 = False プロパティと共に評価して、期限切れのサブスクリプションを見つけます。 Skype for Business Online プラン 1 のサブスクリプションは、2018 年 9 月 1 日に auto renew = False に設定されます。 お客様は、いつでも新しいプランに移動できます。 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype for Business Online プラン 1 の代替プラン

新しいプランでは、お客様は Office 365 の新機能を活用できます。 料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。 

- オプション1: Office 365 Enterprise F1
- オプション 2: Microsoft 365 Enterprise F1
- オプション 3: その他の Office 365 プラン

|**機能**    |**方法 1**   |**方法 2**   |**オプション3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Skype for Business Online プラン 1 に含まれるすべての機能の利用|はい   |はい   |はい   |
|IM とプレゼンス |はい   |はい   |はい   |
|IP を経由したピアツーピア オーディオとビデオ|はい   |はい   |はい   
|認証ユーザーとして会議に参加| はい   |はい   |はい   |

## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。 パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。 廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。

- 新しいサブスクリプションを購入する
- 現在のユーザー ライセンスをもう一度割り当てる
- 以前のサブスクリプションを取り消す

### <a name="migrate-your-customers-to-new-plans"></a>新しいプランにお客様を移行する

1. 新しいサブスクリプションを購入するには、**パートナー センター メニュー** で **[顧客]** を選び、移行する顧客を選んでから、**[サブスクリプションの追加]** を選択します。

2. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。 

お客様には、古い Skype for Business Online プラン1サブスクリプションと、オプション 1-Office 365 Enterprise F1 などの新しい "ターゲット" サブスクリプションの両方が含まれるようになりました。

3. 顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。 顧客の [ユーザーとライセンス] ページが開きます。

4. ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んで **[ライセンスの管理]** を選びます。

5. **[ライセンスの管理]** ページで、Skype for Business Online プラン 1 のライセンスのチェック ボックスをオフにし、お客様の移行先サブスクリプションの新しいサービス プランを選びます。

6. **[Submit]\(送信\)** をクリックします。 確認ページに新しいライセンスの割り当てが一覧表示されます。 ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。

ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。

7. **パートナー センター** メニューで、**[顧客]** を選択します。 サブスクリプションをキャンセルする顧客を選択します。

8. サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。

9. [送信] を選択し **ます。**

以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 お客様には、以前のサブスクリプションの追加コストは発生しません。

## <a name="next-steps"></a>次の手順

- [アドバイザー: クライアントが Office 365 を試すための試用版への招待を作成して送信する](advisors-create-a-trial-invitation.md)
- [アドバイザー: Office 365 試用版への招待と購入プランを使用して、クライアントベースを構築する](advisors-build-your-business.md)
- [アドバイザー: 購入プランを作成する](advisor-create-a-purchase-offer.md)
