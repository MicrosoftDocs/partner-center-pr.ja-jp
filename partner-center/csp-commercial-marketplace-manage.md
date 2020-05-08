---
title: '& プランの marketplace 製品を管理する'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターを使用して、クラウドソリューションプロバイダーが、コマーシャルマーケットプレースから購入したサードパーティの ISV プランを管理する方法について説明します。
author: LauraBrenner
ms.author: labrenne
keywords: サブスクリプション、Marketplace、サードパーティ、ISV、SaaS プラン、クラウドソリューションプロバイダープログラム、プランの管理、サブスクリプションの管理、ライセンスの管理、サブスクリプションの取り消し、座席、自動更新の無効化、間接リセラーの MPN ID
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 53e750c3e661115071c359ce56fbb97a31edeef9
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908100"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>顧客向けの市販の marketplace 製品とプランを管理する

**適用対象**

- パートナー センター
- CSP プログラムのパートナー

**適切なロール**

- グローバル管理者
- 管理エージェント

クラウドソリューションプロバイダー (CSP) プログラムのパートナーは、パートナーセンターポータルを使用して、商用マーケットプレースから、多くの ISV SaaS プランや顧客のサブスクリプションを購入できます。 プランを購入すると、さまざまな方法で管理できるようになります。

## <a name="view-or-edit-a-subscription"></a>サブスクリプションを表示または編集する

サードパーティの ISV 発行元からサブスクリプションを購入した後、次のようにしてレビューまたは編集することができます。

1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [Customers] \ (**顧客**\) を選択します。

2. 適切な顧客を選択し、[**サブスクリプション**] を選択します。 これには、顧客用に購入したライセンスベースのサブスクリプションが一覧表示されます。

3. [**サブスクリプション**] 列で、表示または編集するサブスクリプションを選択します。 これにより、プランを設定またはプロビジョニングするための詳細情報が表示されます。 (プランに関してさらに操作が必要な場合は、[状態] 列に "アクションが必要" という状態が表示されることもあります。 これには、ISV 発行元のサイトへのリンクが付随する場合もあります)。

4. 表示または編集するサブスクリプションを選択すると、[サブスクリプションの詳細] ページでサブスクリプションを編集し、次のような操作を行うことができます。

    - サブスクリプションのニックネームを変更する

    - サブスクリプション内のシート数 (ライセンス) を追加/縮小します。

    - サブスクリプションを取り消す

    - 自動更新をオフにする

    - 間接リセラー MPN ID を追加します (該当する場合)

> [!NOTE]
> サブスクリプションのキャンセルなど、サブスクリプションに対して何らかの変更を行う前に、ISV 発行者によって定義された特定の手順を完了する必要がある場合があります。

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>顧客に代わってライセンスを割り当ててサブスクリプションをアクティブ化する

商用マーケットプレースで独立系ソフトウェアベンダー (ISV) の発行元から提供されているサービスとしてのソフトウェア (SaaS) を購入すると、ISV 発行者は、顧客に代わってライセンスを割り当て、サブスクリプションをアクティブ化するプロセスを管理するのに役立ちます。

発行元は、パーソナライズされたリンクと、特定の購入を識別する認証コードを提供する必要があります。

1. ISV 発行元からのこのパーソナライズされたリンクは、いくつかの方法で見つけることができます。

    - ISV SaaS プランを購入した後に表示される確認ページからリンクを確認できます。

    - 特定の顧客の [サブスクリプション] ページからのリンクが表示されます。 この発行元リンクは、顧客用に購入した ISV プランまたはサブスクリプションに関連付けられている行に表示されます。

    - [パートナーセンター api を使用してリンクを取得](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item)できます。

2. ISV 発行元のサイトまたはシステムにいる場合、発行元は、顧客のセットアッププロセスを完了し、ライセンスをプロビジョニングまたは割り当てるために必要な追加の手順をお知らせします。

3. お客様の代理として働いている CSP プログラムのパートナーとして、次のタスクを実行する責任があります。

    - 必要な情報をパブリッシャーに送信します。

    - 必要な URL を直接顧客に送信する (または、このサブスクリプションの詳細情報をお客様に直接伝える)

4. 発行元に必要な情報を入力すると、パブリッシャーは適切なライセンスを準備して割り当てます。 サブスクリプションの課金は、次のイベントが発生した後に開始されます。

    - ISV 発行者に適切なライセンスが正常に割り当てられました

    - ISV 発行者は、アカウントのセットアップが正常に完了したことを、(別の SaaS フルフィルメント API を使用して) Microsoft に確認しました。

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>ISV 発行元からライセンスベースの SaaS サブスクリプションをキャンセルする

商用マーケットプレース内の ISV 発行元によって提供されるライセンスベースの SaaS 製品にサブスクライブする場合は、指定された取り消し期間内にサブスクリプションを取り消すことができます。 このキャンセル期間は、月単位または年間サブスクリプションがあるかどうかによって変わります。 また、貴社は、サブスクリプションを自動的に更新するかどうかを選択することもできます。

適用されるキャンセル期間、キャンセルする方法、またはサブスクリプションを自動更新する方法の詳細については、以下を参照してください。

- [サブスクリプションを取り消す](create-a-new-subscription.md#cancel-a-subscription)

- [商用 marketplace サブスクリプションの自動更新](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>SaaS サブスクリプションのライセンスを追加または削除する

SaaS 商用 marketplace プランでは、顧客サブスクリプションのユーザーライセンスを追加または削除できます。

1. パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインし、左側のナビゲーションメニューから [Customers] \ (**顧客**\) を選択します。

2. 適切な顧客を選択し、[**サブスクリプション**] を選択します。 これには、顧客用に購入したライセンスベースのサブスクリプションが一覧表示されます。

3. [**サブスクリプション**] 列で、変更するサブスクリプションを選択します。

4. [サブスクリプションの詳細] ページで、[ **Quantity** ] フィールドを見つけます。 ここで、ライセンスの数を増減できます。

5. 数量を変更し、[**送信**] を選択します。

## <a name="manage-subscriptions-using-partner-center-apis"></a>パートナー センター API を使用してサブスクリプションを管理する

また、パートナーセンター Api を使用して、ライフサイクル管理を実行し、サブスクリプションの請求書を管理することもできます。 詳細については、「[商用 marketplace 製品のサブスクリプションを作成する](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)」を参照してください。

## <a name="next-steps"></a>次のステップ

- [商用 marketplace プランの購入](csp-commercial-marketplace-purchase.md)
- [商用マーケットプレースでの課金についての詳細情報](csp-commercial-marketplace-billing.md)