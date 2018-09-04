---
title: Dynamics AX のサブスクリプションを Dynamics 365 に移行する | パートナー センター
description: Microsoft では、次世代のインテリジェント ビジネス アプリケーションである Dynamics 365 を公開しました。これにより、お客様の組織を成長、進化、および変化させ、顧客のニーズに合わせて、新しいビジネスの機会を捕らえることができます。
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 8a8aaf2591b6a67114da7d2226dde7bf94dd06b0
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876302"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Dynamics AX のサブスクリプションを Dynamics 365 に移行する

**適用対象**

-  パートナー センター

Microsoft では、次世代のインテリジェント ビジネス アプリケーションである Dynamics 365 を公開しました。これにより、お客様の組織を成長、進化、および変化させ、顧客のニーズに合わせて、新しいビジネスの機会を捕らえることができます。 新製品の一部として、マイクロソフトでは、2016 年 11 月 1 日に顧客向けの新しい Microsoft Dynamics サブスクリプション プランを導入しました。このプランは現行のプランと類似していますが、若干の違いがあります。

このドキュメントに示されている手順では、間接プロバイダーが顧客の既存の Microsoft Dynamics AX サブスクリプションと Microsoft Dymanics CRM Online サブスクリプションを Microsoft Dynamics 365 に切り替える方法を説明しています。 この手順は、他の Microsoft 製品を新しいバージョンに更新する場合や、プロバイダーが顧客のサブスクリプションを新しい SKU に移行する必要がある場合にも適用されます。

Microsoft Dynamics CRM Online および AX プランは廃止されます。  2017 年 7 月 1 日以降は、レガシ プランへの更新ができなくなり、既存の E4 サブスクリプションも有効期限満了時に自動更新されません。

CRM Online と AX のサブスクリプションは終了した時点で取り消されます。 お客様への継続的なサービス提供を保証するには、有効期限が迫っているサブスクリプションのお客様を、サポートされている以下の SKU オプションに移行する必要があります。 お客様のサービスが中断することを避けるため、サブスクリプションの年間終了日前に新しいサブスクリプションにお客様を移行することをお勧めします。 

サブスクリプションの詳細ページでは、有効期限の近づいたサブスクリプションに対して、サブスクリプションの状態が "自動更新: [日付]" から "有効期限: [日付]" に変更されています。 

API (CREST またはパートナー センターのいずれか) を使用している場合は、サブスクリプションの終了日と auto renew = False プロパティを評価して、有効期限が迫っているサブスクリプションを検出できます。サブスクリプションは、2017 年 7 月 1 日に ”auto renew=False” に設定されています。 パートナー様は顧客をいつでも新しいプランに移動することができます。 

**Microsoft Dynamics AX ライセンスの変更**

Microsoft Dynamics AX 製品ラインは廃止されました。2016 年 11 月 1 日以降は利用できません。 Dynamics 365 の新しいライセンス オプションについて詳しくは、[ライセンス ガイド](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)をご覧ください。

 ライセンスの関連について詳しくは、次の表をご覧ください。

|**廃止された SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations または Microsoft Dynamics 365 プラン |
|タスク|Microsoft Dynamics 365 for Activity
|タスク/セルフサービス|Microsoft Dynamics 365 for Team Members|
|デバイス|Microsoft Dynamics 365 for Operations デバイス|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Microsoft Dynamics CRM Online ライセンスの変更 

**Microsoft Dynamics CRM Online**

現在の Microsoft Dynamics CRM Online プランは廃止されました。2016 年 11 月 1 日以降は利用できません。 Microsoft Dynamics 365 の新しいライセンス オプションについて詳しくは、[ライセンス ガイド](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf)をご覧ください。 新しいライセンス オプションについて詳しくは、[CRM Online のお客様向けの重要なお知らせ](https://go.microsoft.com/fwlink/?linkid=831667)をご覧ください。

ライセンスの関連について詳しくは、次の表をご覧ください。

|**廃止された SKU**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Dynamics 365 Enterprise Customer Engagement プラン |
|Professional|Dynamics 365 Enterprise Customer Engagement プラン、Dynamics 365 for Sales、Dynamics 365 for Customer Service|
|Basic|Dynamics 365 for Team Members、Dynamics 365 for Sales、Dynamics 365 for Customer Service、Dynamics 365 Enterprise Customer Engagement プラン|
|Essential|Dynamics 365 for Team Members|
|フィールド サービスアドオン|Dynamics 365 Enterprise Customer Engagement プランまたは Dynamics 365 for Field Service|
|プロジェクト サービス オートメーション アドオン|Dynamics 365 Customer Engagement プランまたは Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>顧客を新しい製品プランに移行する


Microsoft では、新しい製品やサービスをリセラーとプロバイダー向けに継続的に提供します。 このような場合、リセラーは、顧客を新しいサービスにアップグレードしたり、顧客のサブスクリプションを最終的には廃止される SKU から移行する必要があります。 以前の SKU から新しい SKU に顧客を移行するには、次の手順に従う必要があります。

-   [新しいサブスクリプションを購入する](#manual-subscription-migration-purchasenewsubsc)。
-   [現在のユーザー ライセンスをもう一度割り当てる](#manual-subscription-migration-reassignlicenses)。
-   [以前のサブスクリプションを取り消す](#manual-subscription-migration-cancelsubscriptions)。

次の手順では、Microsoft Dynamics AX または CRM Online から Dynamics 365 に顧客を移行します。

この例では、リセラーは、Dynamics AX Enterprise の既存のサブスクリプションを持つユーザーを Dynamics 365 for Operations に移行する必要があります。 まず、Dynamics 365 for Operations を購入します。  CRM Online を使っている顧客を Microsoft Dynamics 365 へ移行する場合は、次の手順を繰り返します。

<a href="" id="purchasenewsubsc"></a>

**新しいサブスクリプションを購入する**

1.  **[ダッシュボード]** メニューで **[顧客]** を選び、移行する顧客を選んでから **[サブスクリプションの追加]** を選びます。
2.  カタログから購入するサブスクリプション (この場合は、"業務向け Dynamics 365、Enterprise エディション") を選び、ライセンスの数を入力して、**[送信]** を選びます。

    この時点では、顧客は以前のサブスクリプションと新しいサブスクリプションの両方を保持することになります。この例では、以前の "Dynamics AX エンタープライズ" と、新しい "対象の" サブスクリプションである "業務向け Dynamics 365、Enterprise エディション" です。

<a href="" id="reassignlicenses"></a>次の手順では、既存のすべてのユーザー ライセンスを新しいサブスクリプションにもう一度割り当てます。

**ユーザー ライセンスをもう一度割り当てる**

1.  **[ダッシュボード]** メニューで **[顧客]** を選び、移行する顧客を選んでから **[ユーザーとライセンス]** を選びます。 顧客の [ユーザーとライセンス] ページが開きます。
2.  ユーザー ライセンスをもう一度割り当てるには、割り当てるユーザーを選んでから **[ライセンスの管理]** を選びます。
3.  **[ライセンスの管理]** ページで、**[Dynamics AX エンタープライズ]** ライセンスのチェック ボックスをオフにして、**[業務向け Dynamics 365]** ライセンスを選びます。
4.  **[送信]** を選びます。 確認ページに新しいライセンスの割り当てが一覧表示されます。
5.  ライセンスをもう一度割り当てる必要がある他の顧客ユーザーについて、同じ手順を繰り返します。

<a href="" id="cancelsubscriptions"></a>ユーザー ライセンスを新しいサービスに移行すると、メニューの最上位にある [顧客] から以前のサブスクリプションを安全に取り消すことができます。

**以前のサブスクリプションを取り消す**

1.  **[ダッシュボード]** メニューで **[顧客]** を選び、移行する顧客を選んでから、取り消すサブスクリプションを選びます。
2.  サブスクリプションの詳細ページで、サブスクリプションの **[状態]** を **[中断]** に設定します。
3.  **[送信]** を選びます。

以前のサブスクリプションが中断され、新しいサブスクリプションがアクティブになります。 中断されたサブスクリプションは、120 日後に自動的にプロビジョニングが解除されます。 顧客に対しては、以前のサブスクリプションの追加コストは発生しません。

## <a name="additional-considerations"></a>その他の考慮事項


さらにサブスクリプションをプロビジョニングするために、顧客をオープン チャネルからクラウド サービス プログラムに移行する場合は、それらの既存のサブスクリプションも移行する必要があります。

-   顧客がオープン チャネルを通じて以前のサブスクリプションを受け取る場合、新しい SKU での CSP への移行は簡単です。
-   ユーザーがまだ顧客として確立されていない場合は、それらのユーザーを招待することができます。 詳しくは、「[Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx)」(顧客との関係を要求する) ヘルプ トピックをご覧ください。

顧客がお客様を間接プロバイダーとして承認すると、プロビジョニングの手順は上記の手順とほとんど同じになります。新しいサブスクリプションを購入して、ユーザー ライセンスを割り当てます。 以前のサブスクリプションの取り消しだけが、異なる手順となります。 新しいプロバイダーは、他のチャネルを通じて取得されたサブスクリプションの中断や取り消しを行うことができません。 顧客が他の販売ルート (オープン チャネルなど) で以前にサブスクリプションを取得している場合、顧客自身がその販売ルートを通じてサブスクリプションを取り消す必要があります。

 

 



