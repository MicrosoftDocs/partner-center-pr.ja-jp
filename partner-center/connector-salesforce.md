---
title: Salesforce CRM サービスの共同販売パートナー センター
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Salesforce CRM を使用して、パートナー センターの紹介を同期します。 その後、販売者は CRM システム内から Microsoft と共同販売できます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: fa9b35343e1251cfce5caff107de8dff344f4e68
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148416"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM のための共同販売コネクタ - 概要

**適切なロール**: 紹介管理者|CRM のシステム管理者またはシステム カスタマイザー

パートナー センター共同販売コネクタを使用すると、販売者は CRM システム内から Microsoft と共同販売できます。 共同販売の取引を管理するためにパートナー センタートレーニングする必要は" は"ない"。 共同販売コネクタを使用すると、新しい共同販売の紹介を作成して、Microsoft 販売者を引き付け、Microsoft 販売者から紹介を受け取り、紹介を受け入れる/拒否したり、取引価値や終了日などの取引データを変更することができます。  これらの共同販売取引については、Microsoft 販売者から更新プログラムを受け取る場合があります。 すべての紹介作業は、お客様が選択した CRM 内で作業する際に、お客様が行パートナー センター。 

このソリューションは Microsoft Power Automate Solution に基づいており、パートナー センター API を使用します。

## <a name="before-you-install---pre-requisites"></a>インストールする前に - 前提条件

|**トピック**   |**詳細**   |**リンク**   |
|--------------|--------------------|------|
|Microsoft Partner Network ID |有効な MPN ID が必要です|[MPN に参加する方法](https://partner.microsoft.com/)|
|共同販売の準備完了|IP/サービス ソリューションは共同販売の準備ができている必要があります。|[Microsoft で販売する](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|パートナー センター アカウント|共同販売ソリューションに関連付パートナー センター MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。 コネクタをデプロイする前に、ポータルで共同販売パートナー センター確認してください。|[アカウントの管理](create-user-accounts-and-set-permissions.md)|
|パートナー センターのユーザー ロール|コネクタをインストールして使用する従業員は、紹介管理者である必要があります|[ユーザー ロールとアクセス許可の割り当て](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。|[Salesforce CRM でロールを割り当てる](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|パワー自動化フローアカウント|CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。 そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft カスタムフィールド用の Salesforce パッケージのインストール 

パートナーセンターと Salesforce CRM 間で紹介を同期するために、Power solution の自動化ソリューションでは、Microsoft 固有の紹介フィールドを明確に識別する必要があります。 このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。

1. Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。 
[参照](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. 次の手順に従って **営業案件チーム** をアクティブ化します。 
    - セットアップで、[ **クイック検索** ] ボックスを使用して営業案件チームの設定を検索します。
    - 必要に応じて設定を定義します。
[参照](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. Salesforce で、 [パッケージインストーラー](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)を使用してカスタムフィールドおよびオブジェクトをインストールします。 これを使用して、任意の会社にパッケージをインストールします。

>[!NOTE]
>サンドボックスにをインストールする場合は、URL の最初の部分をに置き換える必要があります。 http://test.salesforce.com

4. Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。 追加したら、 **レンチ** アイコンを選択し、プロパティを更新します。

## <a name="best-practice-test-before-you-go-live"></a>ベストプラクティス: 運用前にテストする

運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。

- ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。

- ソリューションのコピーを作成し、構成を実行しPower Automate環境でフローのカスタマイズを実行します。

- ステージング/CRM インスタンスでソリューションをテストします。

- 成功した場合は、マネージド ソリューションとして実稼働インスタンスにインポートします。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM パートナー センター参照同期をインストールする

1. [環境] [Power Automate](https://flow.microsoft.com) に移動し、右上隅 **にある** [環境] を選択します。 これにより、使用可能な CRM インスタンスが表示されます。

2. 右上隅のドロップダウンから適切な CRM インスタンスを選択します。

3. 左側の **ナビゲーション バー** で [ソリューション] を選択します。

4. 上部の **メニューの [AppSource** を開く] リンクを選択します。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. ポップアップ画面 **パートナー センターで Salesforce** の紹介コネクタを検索します。  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. [今すぐ **取得] ボタンを選択** し、[ 続行] **を選択します**。

7. これにより、Salesforce CRM 環境を選択してアプリケーションをインストールできるページが開きます。  使用条件に同意します。

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="利用可能な CRM":::

8. その後、[ソリューションの管理 **] ページに移動** します。  ページの下部パートナー センター矢印ボタンを使用して、[紹介] に移動します。 **[紹介]** ソリューションの横に、スケジュールパートナー センターインストールが表示されます。 インストールには 10 から 15 分かかります。

9. インストールが完了したら、[ソリューション] に戻り [Power Automate](https://flow.microsoft.com) 左側のナビゲーション領域から [ **ソリューション** ] を選択します。 **Salesforce のパートナーセンターの紹介同期** は、[ソリューション] の一覧で確認できます。

10. **Salesforce のパートナーセンター紹介同期** を選択します。 次の電源の自動化フローとエンティティを利用できます。

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Salesforce フロー":::



## <a name="configure-the-solution"></a>ソリューションを構成する

1. CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。

2. 右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。
3. 次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。
    - 参照管理者の資格情報を持つパートナーセンターのユーザー
    - パートナー センターのイベント
    - Power を使用した CRM 管理ソリューションのフローが自動化されます。
4. 左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。

5. [ **接続の作成**] をクリックして接続を作成します。

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="接続を作成する":::

- 右上隅の検索バーで、パートナーセンターの参照 (プレビュー) を検索します。

- 参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。

-  次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。

- CRM 管理者ユーザーの Salesforce の接続を作成します。

-  すべての接続を追加すると、環境内に次の接続が表示されます。

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="接続を監視する":::

### <a name="edit-the-connections"></a>接続を編集する

1. [ソリューション] ページに戻り、[ **既定のソリューション**] を選択します。  [**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="コネクタの編集を開始します":::

2. 3つのドットアイコンを選択して、各接続を個別に編集します。 関連する接続を追加します。

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="コネクタの編集":::

3. 次の順序でフローを有効にします。

- パートナーセンターの Webhook の登録 (Insider Preview)
- パートナーセンターへの共同販売参照の作成-Salesforce (Insider Preview)
- パートナーセンター: Microsoft 共同での Salesforce の参照の更新 (Insider Preview)
- パートナーセンターから Salesforce へ (Insider Preview)
- Salesforce からパートナーセンターへ (Insider Preview)
- パートナーセンターへの Salesforce の営業案件 (Insider Preview)
- パートナーセンターへの Salesforce Microsoft ソリューション (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api を使用してリソース変更イベントに登録する

パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。 これらの変更イベントは、HTTP 投稿として url に送信されます。

1. Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。

2. 参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. これらの更新を行うと、次のように表示されます。

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 変更内容を保存し、[ **有効にする**] を選択します。

   パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。

5. [Salesforce **CRM パートナー センター (Insider Preview) にアクセスする] を選択します**。

6. [編集] **アイコンを** 選択し **、[HTTP 要求を受信した場合] を選択します**。

7. [コピー] **アイコン** を選択して、指定された HTTP POST URL をコピーします。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL のコピー":::

8. 次に、"パートナー センター Webhook 登録 (Insider Preview)" フローを選択しPower Automateを選択 **します**。

9. 右側のウィンドウで [フローの実行] ウィンドウが開き、[続行] を選択 **します**。

10. 次の詳細を入力します。

    1. **Http トリガー エンドポイント**: 前の手順からコピーした URL

    2. **登録するイベント**: "紹介作成" と "紹介更新"

    3. **存在する場合は既存のトリガー エンドポイントを上書** きする: はい (既存のエンドポイントが上書きされます)。

11. [実行 **] を選択** し、[完了] **を選択します。**

Webhook は、イベントの作成と更新をリッスンできます。

## <a name="customize-synchronization-steps"></a>同期手順をカスタマイズする

パートナー センター と CRM システムの間で共同販売の紹介が同期される場合、パートナー センター PC で同期されるフィールドがここに一覧表示されます。

多くの場合、CRM システムは高度にカスタマイズされています。 データ フローをカスタマイズPower Automateできます。 フィールド マッピング ガイドに従い、必要に応じて、データ フローの手順で適切な変更Power Automateします。  Microsoft パートナー センターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。

各フローの複数のステップPower Automateニーズに基づいてカスタマイズできます。 使用可能なカスタマイズの例を次に示します。

1. CRM 参照同期を使用して、パートナー センターイベントのフィールドをカスタマイズするには:

   1. [Salesforce CRM パートナー センター (Insider Preview) にアクセスする] を選択します。

   2. [ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。

   3. 選択 **(スコープ) 潜在顧客または営業案件を同期** します。

2. 作成イベントの CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[**] の順に選択します。 [ **はい] の場合** はサブステップを選択し、 **CRM で [新しい営業案件の作成**] を展開します。 このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。

   1. 更新イベントの CRM フィールドマッピングをカスタマイズするには、[(スコープ) 潜在顧客または営業案件を同期する] ステップを選択します。

   2. **営業案件の更新である場合は、** を選択します。 [ **はい] の場合** はサブステップを選択し、 **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合は**[] を展開します。  

   3. **既存の営業案件を更新** する場合は、[**はい]** を選択します。

3. 更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。

   1. [ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。

   2. [ **(スコープ)] を選択して、営業案件を同期** します。

   3. 更新イベントの CRM フィールドマッピング (フィールドマッピングガイドに基づく) をカスタマイズする場合は、 **パートナーセンターと CRM の潜在顧客オブジェクトが異なるかどうか** を選択してから、を選択します。

   4. [ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。

   このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。

4. Create events の CRM to PC 参照同期のフィールドをカスタマイズするには

   1. [ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。

   2. **参照の同期を選択 (スコープ) します。**

   3. [イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。

このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>エンドツーエンドの双方向の共同販売紹介の同期

Power Automate ソリューションをインストール、構成、カスタマイズしたら、Salesforce CRM と パートナー センター の間で共同販売紹介の同期をテストできます。

### <a name="pre-requisites"></a>前提条件

パートナー センター と Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで Microsoft 固有の紹介フィールドを明確に定義する必要があります。 この識別により、販売者チームは、共同販売のために Microsoft と共有する紹介を決定できます。

カスタム フィールドのセットは、Salesforce CRM ソリューション営業案件パートナー センターの参照同期の一部として **使用** できます。 CRM 管理者ユーザーは、営業案件のカスタム フィールドを含む別の CRM セクション **を作成する** 必要があります。

次のカスタム フィールドは CRM セクションの一部である必要があります。

- **[同期パートナー センター:** 営業案件を Microsoft パートナー センター と同期するかどうか

- **紹介識別子**: Microsoft の参照用の読み取りパートナー センターフィールド

- **紹介リンク**: Microsoft パートナー センター の紹介への読み取り専用パートナー センター

- **Microsoft がどのように役立つのか**: 紹介に必要な Microsoft からのヘルプ

- **製品**: この営業案件に関連付けられている製品の一覧

- **監査**: 参照と同期する読み取り専用パートナー センター証跡

### <a name="scenarios"></a>シナリオ：

1. CRM で紹介が作成または更新され、次の方法で同期された場合の紹介パートナー センター。

   1. CRM の [営業案件] セクションに表示されているユーザーを使用して、Salesforce CRM **環境に** サインインします。

   2. Salesforce CRM 環境で "新しい営業案件" を作成するときに、次のセクションが存在する必要があります

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Salesforce 環境":::

   3. この機会を Microsoft パートナー センター と同期するには、カード ビューで次のフィールドを設定してください。

       - "Sync with パートナー センター": はい
       - 「Microsoft がどのように役立つか」: 次のオプションから選択してください。
       - 製品: 製品のソリューション Id

   4. [営業案件  **とパートナーセンターの同期** ] オプションを **[はい]** に設定したら、10分待ってから、パートナーセンターアカウントにサインインします。 参照は、Salesforce CRM と同期されます。

   5. [パートナーセンターとの同期] オプションが [はい] に設定されている場合、Salesforce CRM で営業案件を更新すると、変更がパートナーセンターアカウントと同期されます。

   6. パートナーセンターで正常に同期された営業案件は、Salesforce CRM の✔アイコンで識別されます。

2. Microsoft パートナーセンターで参照が作成または更新され、Salesforce CRM 環境で同期される場合の紹介の同期:

    1. パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。

    2. 左側のメニューから [ **紹介** ] を選択します。

    3. [新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。

    4. Salesforce CRM 環境にサインインします。

    5. **[Open opportunity**] に移動します。 Microsoft パートナーセンターで作成された紹介が、Salesforce CRM で同期されるようになりました。

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Salesforce の営業案件画面":::

    6. 同期された参照を選択すると、カードビューの詳細が設定されます。

## <a name="next-steps"></a>次のステップ

- [見込み客を管理する](manage-leads.md)

- [共同販売の機会を管理する](manage-co-sell-opportunities.md)

- [パートナー センター Webhook](/partner-center/develop/partner-center-webhooks)
