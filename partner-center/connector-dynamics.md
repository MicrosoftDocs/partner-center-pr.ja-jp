---
title: Dynamics 365 CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Dynamics 365 CRM の共同販売コネクタと同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 18a54bf777cb987e8f486f85afcf277e04c1055c
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556363"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Dynamics 365 CRM の共同販売コネクタ–概要

### <a name="appropriate-roles"></a>適切なロール

- 紹介管理者
- CRM のシステム管理者またはシステムカスタマイザー

パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。 パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。 共同販売コネクタを使用して、Microsoft 販売者に連絡するための新しい共同販売参照を作成したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したり、商談の価値や終了日などの取引データを変更したりします。 また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。 パートナーセンターではなく、選択した CRM 内ですべての紹介作業を行うことができます。 

このソリューションは、Microsoft のパワー自動化ソリューションに基づいており、パートナーセンター Api を使用しています。

## <a name="before-you-install---pre-requisites"></a>をインストールする前に-前提条件

|**トピック**   |**詳細**   |**リンク**   |
|--------------|--------------------|------|
|Microsoft Partner Network ID |有効な MPN ID が必要です|[MPN](https://partner.microsoft.com/)に参加するには|
|共同販売の準備完了|お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。|[Microsoft との販売](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|パートナー センター アカウント|パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。 コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。|[アカウントの管理](create-user-accounts-and-set-permissions.md)|
|パートナー センターのユーザー ロール|コネクタをインストールして使用する従業員は、参照管理者である必要があります|[ユーザー ロールとアクセス許可の割り当て](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。|[Dynamics 365 でロールを割り当てる](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|パワー自動化フローアカウント|CRM システム管理者またはシステムカスタマイザー用のアクティブな [電源自動化](https://flow.microsoft.com) アカウント。 そのユーザーは、インストールの前に少なくとも1回、 [電源の自動](https://flow.microsoft.com) 登録を行う必要があります。|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 のパートナーセンターの紹介同期をインストールする (電源自動化ソリューション)

1. [ [パワー自動化](https://flow.microsoft.com) ] にアクセスし、右上隅にある [ **環境** ] を選択します。 この手順では、使用可能な CRM インスタンスを表示します。

2. 右上隅にあるドロップダウンから適切な CRM インスタンスを選択します。

3. 左側のナビゲーションバーで [ **ソリューション** ] を選択します。

4. 上部のメニューの [ **AppSource を開く** ] リンクをクリックします。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="AppSource を開く":::

5. ポップアップ画面で、 **Dynamics365 のパートナーセンターの紹介コネクタ** を検索します。  

6. [ **今すぐ入手** する] ボタンをクリックし、[ **続行**] をクリックします。

7. これにより、CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが開きます。  使用条件に同意します。

8. その後、[ **ソリューションの管理** ] ページに移動します。  ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。 [パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。 インストールには10-15 分かかります。 

9. インストールが完了したら、[Power の [自動化](https://flow.microsoft.com) ] に戻り、左側のナビゲーション領域から [ **ソリューション** ] を選択します。 **Dynamics 365 のパートナーセンターの紹介同期** は、[ソリューション] の一覧で確認できます。

10. **Dynamics 365 のパートナーセンターの紹介同期** を選択します。 次の電源の自動化フローとエンティティを利用できます。

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRMS":::

## <a name="best-practice-test-before-you-go-live"></a>ベストプラクティス: 運用前にテストする

運用環境でパワー自動化ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。

- ステージング環境/CRM インスタンスに Microsoft Power 自動ソリューションをインストールします。
- ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを自動化します。
- ステージング/CRM インスタンスでソリューションをテストします。 
- 成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。 

## <a name="configure-the-solution"></a>ソリューションの構成

1. CRM インスタンスにソリューションをインストールしたら、[ [Power の自動化](https://flow.microsoft.com/)] に戻ります。


2. 右上隅にある [ **環境** ] ドロップダウンで、パワー自動化ソリューションをインストールした CRM インスタンスを選択します。

3. 次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。

   - 参照管理者の資格情報を持つパートナーセンターのユーザー

   - パートナー センターのイベント

   - Power を使用した CRM 管理ソリューションのフローが自動化されます。

      1. 左側のナビゲーションバーから [ **接続** ] を選択し、一覧から "パートナーセンターの紹介" ソリューションを選択します。

      2. [ **接続の作成**] をクリックして接続を作成します。

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="接続を作成する":::

      3. 右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。

      4. 参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。

      5. 次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。

      6. CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。
       
     
      7. すべての接続を追加すると、環境内に次の接続が表示されます。

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="接続":::
   
## <a name="edit-the-connections"></a>接続を編集する

1. [ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。 [**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="接続する":::

2. 3つのドットアイコンを選択して、各接続を1つずつ編集します。 関連する接続を追加します。

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="一覧表示された接続"::: 

3.  次の順序でフローを有効にします。
- パートナーセンターの Webhook の登録 (Insider Preview)
- パートナーセンターへの共同販売紹介– Dynamics 365 の作成 (Insider Preview)
- パートナーセンターの Microsoft 共同販売参照の更新 Dynamics 365 (Insider Preview)
- パートナーセンターから Dynamics 365 へ (Insider Preview)
- Dynamics 365 からパートナーセンターへ (Insider Preview)
- Dynamics 365 営業案件パートナーセンター (Insider Preview)
- Dynamics 365 Microsoft ソリューション (パートナーセンター) (Insider Preview)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook Api を使用してリソース変更イベントに登録する

パートナーセンターの Webhook Api を使用すると、リソース変更イベントに登録できます。 これらの変更イベントは、HTTP 投稿として url に送信されます。

1. Url を登録するには、 **パートナーセンターの Webhook 登録 (Insider Preview)** パワー自動化フローを選択します。

2. 参照管理者の資格情報を持つパートナーセンターのユーザー (a.) に接続を追加します。パートナーセンターのイベントは、下に強調表示されています。

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="トリガー":::

3. これらの更新を行うと、次のように表示されます。

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhook":::

4. 変更内容を保存し、[ **有効にする**] を選択します。

   パートナーセンターの webhook でイベントの変更をリッスンできるようにするには、次の手順を実行します。

5. [ **パートナーセンター] を Dynamics 365 (Insider Preview) に** 選択します。

6. [ **編集** ] アイコンを選択し、[ **HTTP 要求の受信時**] を選択します。

7. **コピー** アイコンを選択して、指定された HTTP POST URL をコピーします。

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="URL のコピー":::

8. 次に、"パートナーセンターの Webhook の登録 (Insider Preview)" パワー自動化フローを選択し、[ **実行**] を選択します。

9. 右側のウィンドウで [実行フロー] ウィンドウが開いていることを確認し、[ **続行**] をクリックします。

10. 次の詳細を入力します。

    1. **Http トリガーエンドポイント**: 前の手順からコピーされた URL

    2. **登録するイベント**: "紹介-作成" と "参照-更新"

    3. **既存のトリガーエンドポイントがある場合は上書き** します (存在する場合は既存のエンドポイントを上書きします)。

11. [ **実行** ] を選択し、[完了] を選択し **ます。**

Webhook は、イベントの作成と更新をリッスンできるようになりました。

## <a name="customize-synchronization-steps"></a>同期手順のカスタマイズ

パートナーセンターと CRM システムの間で共同販売参照が同期されると、パートナーセンター PC で同期されるフィールドがここに表示されます。

多くの場合、CRM システムは高度にカスタマイズされています。 パワー自動化フローをカスタマイズできます。 フィールドマッピングガイドに従って、必要に応じて、パワー自動化フローの手順に適切な変更を加えます。  Microsoft パートナーセンターから CRM へのマッピングが提供されますが、CRM 環境に基づいて、フィールドをさらにカスタマイズすることもできます。

各パワー自動化フローの複数の手順は、ニーズに応じてカスタマイズできます。 使用可能なカスタマイズの例を次に示します。

1. パートナーセンターで作成または更新イベントのフィールドを CRM の参照同期にカスタマイズするには、次のようにします。 

    a. [パートナーセンター] を選択して Dynamics 365 (Insider Preview) またはパートナーセンターから Salesforce へ (Insider Preview) を選択します。

    b. [ **編集** ] を選択して、パワー自動化フローを編集またはカスタマイズします。

    c. 選択 **(スコープ) 潜在顧客または営業案件を同期** します。

2. イベントの作成用に (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズするには、[ **新しい共有の営業案件]、[] の順** に選択します。 [サブステップ **if]** を選択し、 **CRM で [新しい営業案件の作成**] を展開します。 このセクションでマッピングを編集するには、[フィールドマッピングガイド] を使用します。

    d. 更新イベントの CRM フィールドマッピングをカスタマイズする (フィールドマップガイドに基づく) 場合は、"(スコープ) 潜在顧客または営業案件の同期" ステップをクリックします。

    e. **営業案件の更新である場合は、** を選択します。 [サブステップ **if yes]** を選択し、次に **パートナーセンターと CRM の営業案件オブジェクト間の差異がある場合** は、を展開します。  

    f. **既存の営業案件を更新** する場合は、[**はい]** を選択します。

3. 更新イベントの CRM から PC への参照同期のフィールドをカスタマイズするには、次のようにします。

    a. [ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。

    b. [ **(スコープ)] を選択して、営業案件を同期** します。

    c. 更新イベントの CRM フィールドマッピングをカスタマイズするに **は、パートナーセンターと crm の潜在顧客オブジェクトが異なるかどうか** を選択してから、を選択します。 

    d. [ **はい] の場合** はサブステップを選択し、[ **営業案件データを使用して紹介を更新する**] ステップを展開します。

   このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。

4. Create events の CRM to PC 参照同期のフィールドをカスタマイズするには

   a. [ **編集**  ] を選択して、パワー自動化フローを編集またはカスタマイズします。

   b. **参照の同期を選択 (スコープ) します。**

   c. [イベントの作成] で (フィールドマッピングガイドに基づいて) CRM フィールドマッピングをカスタマイズする場合は、[ **Microsoft の紹介を作成する**] を選択します。

   このセクションのマッピングは、フィールドマッピングガイドに基づいて編集できます。

2つの環境変数が作成されます。

- チェックマーク: パートナーセンターと Dynamics 365 CRM の間で双方向に同期される営業案件以外にチェックマークアイコンが必要かどうかを示します。

- 共同販売機会の同期のみ: 共同販売機会のみを同期するかどうかを指定します。

環境変数の既定値の編集を選択できます。

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="既定値のエディットボックス":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>エンドツーエンドの双方向の共同販売参照の同期

パワー自動化ソリューションをインストールし、構成し、カスタマイズしたら、Dynamics 365 とパートナーセンター間の共同販売参照の同期をテストできます。

### <a name="pre-requisites"></a>前提条件

パートナーセンターと Dynamics 365 CRM 間で紹介を同期するために、Power 区分ソリューションでは、Microsoft 固有の紹介フィールドが明確に示されます。 この id により、販売者チームは、共同販売のために Microsoft と共有する参照を決定することができます。

一連のカスタムフィールドは、 **営業案件** エンティティの一部として使用できます。 CRM 管理者ユーザーは、 **営業案件** のカスタムフィールドを使用して、別の crm セクションを作成する必要があります。

次のカスタムフィールドは、CRM セクションの一部にする必要があります。

- **パートナーセンターとの同期**: 営業案件を Microsoft パートナーセンターと同期するかどうか

- **参照識別子**: Microsoft パートナーセンターの紹介の読み取り専用識別子フィールド

- **紹介リンク**: Microsoft パートナーセンターでの紹介への読み取り専用リンク

- Microsoft の **ヘルプ** を参照してください。

- **製品**: この営業案件に関連付けられている製品の一覧

- **監査**: パートナーセンターの紹介と同期するための読み取り専用の監査証跡

Dynamics 365 CRM の営業案件フォームを更新して、Products フィールドを含めるようにします。

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="営業案件フォーム":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>モデル

1. CRM で参照が作成または更新され、パートナーセンターで同期される場合の参照の同期:

   1. CRM の **営業案件** セクションで可視性を持つユーザーを使用して、DYNAMICS 365 CRM 環境にサインインします。

   2. Dynamics 365 環境で "新しい営業案件" を作成するときに、次のセクションが存在することを確認します。

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Dynamics 365 の Microsoft パートナーセンター情報を示すサンプルの営業案件セクション。":::

   3. この機会を Microsoft パートナーセンターと同期するには、カードビューで次のフィールドを設定していることを確認します。

      - **パートナーセンターとの同期**: はい

      - **Microsoft のヘルプを使用する方法**: 次から選択してください。

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Dynamics 365 のサンプルの営業案件セクションでは、microsoft パートナーセンターのヘルプオプションが表示されます。":::

      - **製品**: 製品のソリューション id

   4. 営業案件が Dynamics 365 で作成され、[ **パートナーセンターとの同期** ] オプションが **[はい]** に設定されたら、10分待ってから、パートナーセンターアカウントにサインインします。 参照は Dynamics 365 と同期されます。

   5. 同様に、[パートナーセンターとの同期] オプションを [はい] に設定した場合は、Dynamics 365 CRM の営業案件を更新すると、パートナーセンターアカウントで変更が同期されます。

   6. パートナーセンターで正常に同期された営業案件は、Dynamics 365 の✔アイコンで識別されます。

2. Microsoft パートナーセンターで参照が作成または更新され、Dynamics 365 環境で同期される場合の参照同期:

   1. パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。

   2. 左側のメニューから [ **紹介** ] を選択します。

   3. [新しい取引] オプションをクリックして、パートナーセンターから新しい共同販売紹介を作成します。

   4. Dynamics 365 CRM 環境にサインインします。

   5. **[Open opportunity**] に移動します。 Microsoft パートナーセンターで作成された紹介が Dynamics 365 CRM で同期されるようになりました。

   6. 同期された参照を選択すると、カードビューの詳細が設定されます。

## <a name="next-steps"></a>次の手順

- [見込み客を管理する](manage-leads.md)

- [共同販売の機会を管理する](manage-co-sell-opportunities.md)

- [Microsoft Power の自動化プラットフォームの詳細](/power-automate/)

- [パートナー センター Webhook](/partner-center/develop/partner-center-webhooks)