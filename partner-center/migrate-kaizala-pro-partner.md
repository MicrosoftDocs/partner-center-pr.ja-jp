---
title: Kaizala Pro サブスクリプションを Microsoft 365 に移行する
description: Kaizala Pro サブスクリプションを Microsoft 365 または Office 365 バージョンに移行する方法について説明します。 お客様の移行の詳細については、この記事をご覧ください。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172406"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Kaizala Pro スタンドアロンサブスクリプションを Microsoft 365 または Office 365 バージョンに移行する

**適切なロール**

- 販売代理店

2020年7月1日より、Microsoft は Kaizala Pro スタンドアロンサービスの売上を終了します。 お客様は、この日より後に新しい Kaizala Pro サブスクリプションを購入することはできなくなります。また、既存の Kaizala Pro サブスクリプションは、有効期限が切れると自動的に更新されません。

お客様の継続性を確保するには、Kaizala Pro スタンドアロンサブスクリプションが期限切れになっているお客様を、サポートされている SKU オプション (下記参照) に移行する必要があります。 顧客のサービスの停止を防ぐために、サブスクリプションの年間終了日前に新しいサブスクリプションに顧客を移動することをお勧めします。

API (CREST またはパートナーセンター) を使用する場合、[自動更新] プロパティを false に設定して、サブスクリプションの終了日を評価することで、期限切れのサブスクリプションを検出できます `auto renew = False` 。

E4 サブスクリプションは `auto renew=False` 、2020年7月1日に設定されます。 お客様は、いつでも新しいプランに移動できます。

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro スタンドアロン置換プラン

新しいプランでは、お客様は Microsoft 365 の新しい機能を利用できます。 料金の詳細は、パートナー センターの料金表またはプランのマトリックスに記載されています。

- 次を含む [**ビジネス向け Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2):  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**最前線の Microsoft 365**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)(次を含む):
   - Microsoft 365 F3 (旧称 Microsoft 365 F1) と Office 365 F3
    
- 以下を含む、 [**Enterprise の Microsoft 365**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans): 
   - Office 365 E1
   - Microsoft 365 E3 および Office 365 E3
   - Microsoft 365 E5 および Office 365 E5

- 以下を含む [**教育の Microsoft 365**](https://www.microsoft.com/education/buy-license/microsoft365): 
    - Microsoft 365 A1 と Office 365 A1
    - Microsoft 365 A3 と Office 365 A3
    - Microsoft 365 A5 と Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する

マイクロソフトは、絶えず新しい製品やサービスをパートナーに提供しています。 パートナーはこれに対応して、お客様を新しいサービスにアップグレードするか、お客様のサブスクリプションを廃止予定の SKU から移行する必要があります。 廃止された SKU から新しい SKU にお客様を移行するには、次の手順を実行します。

A. 新しいサブスクリプションを購入する

B. 現在のユーザー ライセンスをもう一度割り当てる

C. 以前のサブスクリプションを取り消す


## <a name="migrate-your-customers-to-new-plans"></a>新しいプランにお客様を移行する

### <a name="a-purchase-the-new-subscription"></a>A. 新しいサブスクリプションを購入する

1. 新しいサブスクリプションを購入するには、 **パートナーセンター** メニューから [ **顧客**] を選択し、移動する顧客を選択して、[ **サブスクリプションの追加**] を選択します。

2. 購入するサブスクリプション (この場合は、上記のいずれかのオプション) をカタログから選び、ライセンス数を入力して、**[送信]** を選びます。

お客様は、以前のサブスクリプションと新しいサブスクリプション (オプション 1-Office 365 Enterprise F1 など) の両方を使用できるようになります。

### <a name="b-reassign-current-user-licenses"></a>B. 現在のユーザー ライセンスをもう一度割り当てる

1. 顧客のユーザーのライセンスをもう一度割り当てるには、**パートナー センター** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。 顧客の [ユーザーとライセンス] ページが開きます。

2. ユーザーライセンスを再割り当てするには、再割り当てするユーザーを選択し、[ **ライセンスの管理**] を選択します。

3. [ **ライセンスの管理** ] ページで、[Kaizala Pro スタンドアロンライセンス] チェックボックスをオフにし、顧客の移動先のサブスクリプションの新しいサービスプランを選択します。

4.  **[Submit]\(送信\)** をクリックします。 確認ページに新しいライセンスの割り当てが一覧表示されます。 ライセンスの割り当てが必要な他のユーザーにも同じプロセスを続行します。

### <a name="c-cancel-old-subscription"></a>C. 以前のサブスクリプションを取り消す

ユーザー ライセンスを新しいサービスに移行した後は、顧客レベルで廃止されたサブスクリプションを安全に取り消すことができます。

1.  **パートナー センター** メニューで、**[顧客]** を選択します。 サブスクリプションをキャンセルする顧客を選択します。

2.  サブスクリプションの詳細ページで、サブスクリプションを **[中断]** に設定します。

3.  **[Submit]\(送信\)** をクリックします。

以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 お客様には、以前のサブスクリプションの追加コストは発生しません。
