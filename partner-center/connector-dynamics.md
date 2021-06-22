---
title: Dynamics 365 CRM の共同販売パートナー センター
description: Dynamics 365 CRM パートナー センター共同販売コネクタを使用して、顧客の紹介を同期します。 その後、CRM システム内から Microsoft と共同販売できます。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: e656f728789bf5b13dd09732b0b2f5ef30de760a
ms.sourcegitcommit: b7203f1393c3d8f8db4683acdebd09a89e086c3c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2021
ms.locfileid: "112425085"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Dynamics 365 CRM の共同販売コネクタの概要

**適切なロール**: 紹介管理者|CRM のシステム管理者またはシステム カスタマイザー

パートナー センターコネクタを使用すると、販売者は CRM システム内から Microsoft と共同販売できます。 共同販売取引を管理するために、パートナー センタートレーニングする必要は" は "ない"。 共同販売コネクタを使用して、新しい共同販売の紹介を作成して、Microsoft 販売者を引き付け、Microsoft 販売者から紹介を受け取り、紹介を受け入れるか拒否し、取引価値や終了日などの取引データを変更します。 また、これらの共同販売取引に関する Microsoft 販売者から更新プログラムを受け取る場合があります。 すべての紹介作業は、顧客が選択した CRM で管理パートナー センター。

このソリューションは、API のPower Automate基パートナー センターしています。

## <a name="prerequisites"></a>前提条件

ソリューションをインストールする前に、次の前提条件を満たしていることを確認してください。

|**トピック**   |**詳細**   |**リンク**   |
|--------------|--------------------|------|
|Microsoft Partner Network (MPN) ID |有効な MPN ID が必要です。|[パートナー ネットワークに参加する](https://partner.microsoft.com/)|
|共同販売の準備完了|IP/サービス ソリューションは共同販売の準備ができている必要があります。|[Microsoft で販売する](https://partner.microsoft.com/membership/sell-with-microsoft)|
|パートナー センター アカウント|新しいテナントに関連付パートナー センター MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。 コネクタをデプロイする前に、パートナー センターポータルに共同販売の紹介が表示されるのを確認します。|[アカウントの管理](create-user-accounts-and-set-permissions.md)|
|パートナー センターのユーザー ロール|コネクタをインストールして使用する従業員は、紹介管理者である必要があります。|[ユーザー ロールとアクセス許可の割り当て](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|CRM ユーザー ロールは、システム管理者またはシステム カスタマイザーです。|[Dynamics 365 でロールを割り当てる](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate フロー アカウント|テスト、ステージング、および運用用のデータベースを使用して、新しい実稼働環境を作成します。 データベースを含む既存の実稼働環境がある場合は、再利用できます。 コネクタ ソリューションをインストールするユーザーは、この環境にPower Automateライセンスとアクセス権を持っている必要があります。 インストールが失敗した場合は、進行状況を監視し、Power Automate [情報を](https://flow.microsoft.com/) 取得できます。 [ソリューション] **の下の [履歴の** 表示] **を選択します**。|[環境を作成または管理する](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Dynamics 365 パートナー センター参照同期をインストールする (Power Automate ソリューション)

1. [] [Power Automate](https://flow.microsoft.com)に移動し、右上隅 **にある [環境** ] を選択します。 この手順では、使用可能な CRM インスタンスが表示されます。

1. 右上隅のドロップダウン リストから適切な CRM インスタンスを選択します。

1. 左側の **[ソリューション** ] を選択します。

1. 上部の **メニューの [AppSource** を開く] リンクを選択します。

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Open AppSource を示すスクリーンショット。":::

1. ポップアップ画面 **パートナー センター Dynamics 365** の紹介コネクタを検索します。  

1. [今すぐ **取得] ボタンを選択** し、[続行] を **選択します**。

1. CRM (Dynamics 365) 環境を選択してアプリケーションをインストールできるページが表示されます。 使用条件に同意します。

1. 進行状況を監視できます。インストールが失敗した場合は、[ソリューション] の下にある [履歴の表示]を選択Power Automateの詳細を確認 **できます**。

1. インストールが完了したら、[ソリューション] に戻 [りPower Automate](https://flow.microsoft.com) 左側の **[ソリューション]** を選択します。 **パートナー センター Dynamics 365** の紹介の同期がソリューションの一覧で **使用** できます。

1. **[Dynamics 365 パートナー センター参照の同期] を選択します**。 次のPower Automateとエンティティを使用できます。

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="使用可能な CRM を示すスクリーンショット。":::

## <a name="test-before-you-go-live"></a>ライブに進む前にテストする

実稼働環境で Power Automate ソリューションをインストール、構成、カスタマイズする前に、ステージング CRM インスタンスでソリューションをテストしてください。 次のことを行う必要があります。

- ステージング環境POWER AUTOMATE CRM インスタンスに新しいソリューションをインストールします。
- ステージング環境でPower Automateソリューションを構成およびカスタマイズします。
- ステージング CRM インスタンスでソリューションをテストします。
- テストが成功したら、マネージド ソリューションとして実稼働インスタンスにインポートします。

## <a name="configure-the-solution"></a>ソリューションを構成する

1. CRM インスタンスにソリューションをインストールしたら、 に戻[Power Automate。](https://flow.microsoft.com/)

1. 右上隅の **[環境** ] ドロップダウン リストから、新しいソリューションをインストールした CRM インスタンスPower Automateします。

1. 3 つのユーザー アカウントを関連付ける接続を作成する必要があります。

   - パートナー センター管理者の資格情報を持つユーザーを追加する
   - パートナー センターのイベント
   - ソリューション内のPower Automateを含む CRM 管理者

   1. 左側 **の [** 接続] を選択し、一 **覧パートナー センター [** 紹介] ソリューションを選択します。

   1. [接続の作成] を選択 **して接続を作成します**。

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="[接続の作成] を示すスクリーンショット。":::

   1. 右上隅 **のパートナー センターで** 、紹介 (プレビュー) を検索します。

   1. 紹介管理者の資格情報ロールパートナー センターユーザーの接続を作成します。

   1. 次に、紹介管理者パートナー センター資格情報を使用して、パートナー センターユーザーのイベントイベント接続を作成します。

   1. CRM 管理者ユーザーの Common Data Service (現在の環境) の接続を作成します。
     
   1. すべての接続を追加すると、環境に次の接続が表示されます。

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="接続を示すスクリーンショット。":::

## <a name="edit-the-connections"></a>接続を編集する

1. [ソリューション] ページ **に戻り** 、[既定のソリューション] **を選択します**。 [ **すべて] を選択して、接続** 参照 (プレビュー) を **選択します**。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="接続の編集を示すスクリーンショット。":::

1. 省略記号アイコンを選択して、各接続を個別に編集します。 関連する接続を追加します。

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="一覧表示されている接続を示すスクリーンショット。":::

1. [ソリューション] **ページ** に戻り **、Dynamics 365** の [パートナー センター 紹介同期] を選択し、次のシーケンスで各フローの横にある省略記号アイコンを選択してフローを有効にしてください。 フローを有効にしている間に問題が発生した場合は、「カスタマイズ手順」と「トラブルシューティング[手順」](connector-dynamics.md#customize-synchronization-steps)[を参照してください](connectors-troubleshoot.md)。

次の順序でフローを有効にする:

- パートナー センター Webhook 登録 (Insider Preview)
- 共同販売紹介を作成する – Dynamics 365 から パートナー センター (Insider Preview)
- [カスタマイズ]Dynamics 365 フローから詳細を作成または取得する
- パートナー センター Dynamics 365 - Helper (Insider Preview) へのアクセス
- パートナー センター Dynamics 365 (Insider Preview) に対する Microsoft 共同販売紹介の更新プログラム
- パートナー センター Dynamics 365 へのアクセス (Insider Preview)
- Dynamics 365 から パートナー センター (Insider Preview)
- Dynamics 365 Opportunity to パートナー センター (Insider Preview)
- Dynamics 365 Microsoft Solutions to パートナー センター (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook API を使用してリソース変更イベントに登録する

Webhook API パートナー センター使用して、リソース変更イベントに登録できます。 これらの変更イベントは、HTTP 投稿として URL に送信されます。

1. [パートナー センター **Dynamics 365 (Insider Preview) にアクセスする] を選択します**。

1. [編集] **アイコンを** 選択し、 **[HTTP 要求を受信した場合] を選択します**。

1. [コピー] **アイコン** を選択して、指定された HTTP POST URL をコピーします。

   :::image type="content" source="images/webhook-video.gif" alt-text="Webhook を使用してリソースの変更を登録する方法を示すスクリーンショット。":::

1. **[Webhook のパートナー センター (Insider Preview)** フローを選択しPower Automate実行] を **選択します**。

1. 右側のウィンドウで **[フローの実行** ] ウィンドウが開き、[続行] を選択 **します**。

1. 次の詳細を入力します。

   - **Http トリガー エンドポイント**: この URL は、前の手順からコピーされました。
   - **登録するイベント**: 使用可能なすべてのイベント (**紹介** で作成されたイベント、紹介が **更新** されたイベント、 **関連** する紹介で作成された イベント、および関連する紹介が更新された イベント) **を選択します**。
   - **既存のトリガー エンドポイントが存在する場合は上書きしますか?**: はい。 特定の Webhook イベントに登録できる URL は 1 つのみです。

1. [フロー **の実行] を** 選択し、[完了] を **選択します。**

Webhook は、イベントをリッスン、作成、および更新できます。

## <a name="customize-synchronization-steps"></a>同期手順をカスタマイズする

CRM システムは高度にカスタマイズされ、CRM のセットアップPower Automateソリューションをカスタマイズできます。 パートナー センター と CRM システムの間で共同販売の紹介が同期される場合、パートナー センター PC で同期されるフィールドは、カスタム フィールド マッピング ガイド の一覧に [表示されます](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)。

フィールド マッピング ガイドに従い、必要に応じて、[カスタマイズ **] Dynamics 365** フローまたは環境変数から詳細を作成または取得するに関するページで適切な変更を行います。 将来のソリューションのアップグレードに影響を与える可能性Power Automateソリューション内の他のフローは更新しない。

次のカスタマイズを使用できます。

- 営業 **案件** 名にチェック マークを表示する: 既定では、パートナー センター と Dynamics 365 CRM 間の同期が正常に行っていることを示すチェック マークが営業案件名の横に表示されます。 同様に、同期に失敗した場合はクロス マークが表示されます。 営業案件名にチェック マークまたはクロス マークを追加しないようにするには、営業案件名環境変数の [表示] チェック マークの現在の値を [いいえ] に設定します。
- **取引値**: 既定では、CRM の推定値パートナー センターとの間で同期されるトランザクションの **取引** 値。 CRM に、取引価値を同期する別のフィールドがある場合:

  - Dynamics  365 環境変数の Deal 値フィールド名を CRM のフィールド名で更新します。 表示名ではなく、フィールドの名前を指定してください。
  - **[カスタマイズ] Dynamics 365** フローから詳細を作成または取得し、 [CRM での営業案件の作成または更新]に移動し、 [新しい営業案件の作成] と [既存の営業案件の更新] アクションを更新して **、DEALValue** 値を CRM の正しいフィールドに割り当てる方法を更新します。 また、[推定収益] **フィールドから DealValue** の割 **り当てを削除** します。

- **顧客アカウントの国番号**: 新しい紹介を作成するときに、2 文字の国番号 (ISO 3166) を指定する必要があります。 既定では、国コードは CRM のアカウントの address1_country **フィールドと** 同期されます。 国コードを同期する CRM に別のフィールドがある場合:

  - 2 文字のコードを含むアカウントの非lookup 国コード フィールドの場合:
    - Dynamics 365 環境変数の Customer **Account Country Code** フィールド名を CRM のフィールド名で更新します。 表示名ではなく、フィールドの名前を指定してください。
    - **[カスタマイズ] Dynamics 365** フローから詳細を作成または取得し、CRM アクションで顧客アカウントを作成または取得するに移動して、CRM の正しいフィールドに Country 値を割り当てる。 また、[住所 1: **国** /地域] フィールドから Country 値 **の割り当てを削除** します。

  - アカウントの参照ベースの国コード フィールドの場合:
    - アカウントに新しいカスタム フィールドを追加し、ルックアップ ベースのフィールドで選択した値に基づいて、2 文字の国コード (ISO 3166) を自動的に設定します。その逆も同様です。
    - 非lookup 国コード フィールドの前の手順に従って、CRM の新しいカスタム フィールドと、その間で新しいカスタム フィールドを同期パートナー センター。

- **営業** 案件フィールド: 営業案件に入力する必要がある必須フィールドがある場合は、[カスタマイズ **] Dynamics 365** フローから [詳細の作成または取得] を編集し、CRMでの営業案件の作成または更新に関するページに移動し、更新ビジネス要件に基づいて必須フィールドに値を割り当てる新しい営業案件アクションを作成します。
- リード **フィールド:** リードに入力する必要がある必須フィールドがある場合は、[カスタマイズ **] Dynamics 365** フローから [詳細の作成または取得] を編集し、CRM の[リードの作成または更新] に移動して、ビジネス要件に基づいて必須フィールドに値を割り当てる新しいリード アクションの作成に関するページを更新します。
- **顧客** アカウント: 新しい紹介が パートナー センター から CRM に同期されている場合、Power Automate ソリューションは、顧客の会社名と郵便番号を使用して CRM 内の既存のアカウントの検索を試します。 見つからなかった場合は、CRM に新しい顧客アカウントが作成されます。 検索条件と新しいアカウント作成の詳細を更新するには、[カスタマイズ **] Dynamics 365** フローから [作成]または [詳細の取得] を編集し、 [CRM での顧客アカウントの作成または取得] および [顧客アカウントの作成] アクション に移動します **。**

## <a name="update-environment-variable"></a>環境変数を更新する

環境変数の値を更新するには:

1. [ソリューション] ページ **に移動** し、[既定のソリューション] **を選択します**。 [すべて **] を選択** して[環境変数] を **選択します**。

1. 更新する必要がある値の環境変数を選択し、省略記号アイコンを使用して [編集] を選択します。

1. [**新しい値]** オプションを **使用して値** を指定して、現在の値を更新します (既定値は更新されません)。 値は、変数のデータ型と一致する必要があります。 たとえば、 [はい] または [いいえ] のデータ型は、[はい] または [いいえ] の値を受け入れる場合があります。

   :::image type="content" source="images/environment-variables-video.gif" alt-text="環境変数の更新を示すスクリーンショット。":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>エンドツーエンドの双方向共同販売紹介の同期

Power Automate ソリューションをインストール、構成、カスタマイズしたら、Dynamics 365 と パートナー センター の間で共同販売紹介の同期をテストできます。

### <a name="prerequisites"></a>前提条件

パートナー センター と Dynamics 365 CRM 間で紹介を同期するために、Power Automate ソリューションは Microsoft 固有の紹介フィールドを明確にデマーカットします。 この識別により、販売者チームは、共同販売のために Microsoft と共有する紹介を決定できます。

ソリューションのインストールの一環として、一連のカスタム フィールドとオブジェクトが追加されます。 CRM 管理者ユーザーは、営業案件のカスタム フィールドを含む別の CRM セクション **を作成する** 必要があります。

次のカスタム フィールドは CRM セクションの一部である必要があります。

- **[同期] パートナー センター:** 営業案件を他のユーザーと同期パートナー センター。 既定では、このフィールドの値は [いいえ] で、Microsoft と営業案件を共有するには、販売者が明示的に [はい] に設定する必要があります。 CRM から CRM に共有されるパートナー センター、このフィールドの値は [はい] に設定されます。
- **紹介識別子**: 参照の参照の読み取りパートナー センターフィールド。
- **紹介リンク**: ページ内の紹介への読み取りパートナー センター。
- **Microsoft が支援する方法:** 紹介に Microsoft から必要なヘルプ。 共同販売の紹介を作成するには、Microsoft に必要な適切なヘルプを選択します。 顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。 共同販売以外の紹介を作成するには、このフィールドを選択しない必要があります。 共同販売以外の紹介は、ヘルプが必要な適切なオプションを選択することで、いつでも共同販売の紹介に変換できます。
- **Microsoft パートナー センターの参照の可視性**: 参照の表示を選択パートナー センターします。 Microsoft の販売者に表示することで、共同販売以外の紹介が共同販売に変換される可能性があります。 Microsoft のヘルプが必要な場合、紹介は既定で Microsoft 販売者に表示されます。 このフィールドが表示済みとしてマークされた後は、元に戻す必要があります。
- **Microsoft CRM 識別子**: 共同販売の紹介が作成され、Microsoft によって受け入れられると、このフィールドに Microsoft の CRM 識別子が入力されます。
- **製品: 廃止**: このフィールドを使用したり、CRM セクションに追加したりしません。 旧バージョンとの互換性のためにのみ使用できます。 代わりにパートナー センターソリューションを使用してください。
- **監査**: 参照と同期する読み取りパートナー センター証跡。
- **Microsoft パートナー センター ソリューション**: 共同販売対応ソリューションまたは Microsoft ソリューションを機会に関連付けるカスタム オブジェクト。 1 つ以上のソリューションを営業案件に追加または削除できます。 Microsoft と共有する前に、営業案件に少なくとも 1 つの共同販売準備完了または Microsoft ソリューションを追加する必要があります。 このオブジェクトを営業案件に関連付けるには、CRM の **営業案件** フォームを更新します。

  [営業案件] フォームで適切なタブ **を** 選択し、次に示すようにサブグリッドを追加します。

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="営業案件フォームを示すスクリーンショット。":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Microsoft ソリューションを示すスクリーンショット。":::

- Microsoft ソリューションを追加した後は、共同販売の準備完了ソリューションの詳細を事前に設定して、販売者が追加する必要が生じなくすることができます。 新しいソリューションの詳細を追加するには、CRM の Microsoft Solution Detailsオブジェクトに移動し、[レコードの追加] を選択して 1 つのエントリを追加するか **、Excel アップロード** を使用して複数のエントリを追加します。

  :::image type="content" source="images/cosellconnectors/dynamics-solution-1.png" alt-text="新しい Microsoft ソリューションの詳細を示すスクリーンショット。":::

### <a name="scenarios"></a>シナリオ

1. CRM で紹介が作成または更新され、次の方法で同期された場合の紹介パートナー センター。

   1. CRM の営業案件セクションに表示されているユーザーを使用して、Dynamics 365 CRM **環境に** サインインします。

   1. Dynamics 365 **環境パートナー センター** 新しい営業案件を作成するときに、[Microsoft パートナー センター] セクションが表示されます。

      :::image type="content" source="images/cosellconnectors/dynamics-solution-2.png" alt-text="新しい営業案件を示すスクリーンショット。":::

   1. この営業案件を パートナー センターするには、カード ビューで次のフィールドを設定します。

      - **Microsoft が支援する方法:** 共同販売の紹介を作成するには、適切なヘルプ オプションを選択します。

         :::image type="content" source="images/cosellconnectors/dynamics-solution-3.png" alt-text="カード ビューで適切なフィールドを取得する方法を示すスクリーンショット。":::

      - **顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。
      - **[同期と同期パートナー センター:** はい。
      - **Microsoft ソリューション**: Microsoft と紹介を共有するには、有効な共同販売準備完了または Microsoft ソリューションを営業案件に追加します。

        :::image type="content" source="images/cosellconnectors/dynamics-solution-4.png" alt-text="ソリューション ID を示すスクリーンショット。":::

   1. Dynamics 365 で営業案件が作成され、[同期と同期] オプションパートナー センター [は **い** ] に設定された後、10 分待ちます。 次に、自分のアカウントパートナー センターします。 紹介は Dynamics 365 および参照識別子 と **同期されます**。 **紹介リンク** が設定されます。 エラーが発生した場合は、[監査] **フィールド** にエラー情報が入力されます。

      1. 同様に、[ **パートナー センター** と同期する ] オプションが [はい] に設定されている営業案件の場合は、Dynamics 365 CRM で営業案件を更新すると、パートナー センター アカウントで変更が同期されます。

      1. Dynamics 365 では、パートナー センターと正常に同期✔が識別されます。

1. Dynamics 365 環境で参照が作成または更新パートナー センター同期された場合の紹介の同期:

   1. ダッシュボード にサインインパートナー センター [します](https://partner.microsoft.com/dashboard/home)。

   1. 左側 **のメニューから [** 紹介] を選択します。

   1. [新しい取引] オプションを選択して、パートナー センターから新しい **共同販売の紹介を作成** します。

   1. Dynamics 365 CRM 環境にサインインします。

   1. [Open **Opportunities] に移動します**。 このページで作成パートナー センター Dynamics 365 CRM で同期されます。

   1. 同期された紹介を選択すると、カード ビューの詳細が設定されます。

## <a name="next-steps"></a>次の手順

- [見込み客を管理する](manage-leads.md)
- [共同販売の機会を管理する](manage-co-sell-opportunities.md)
- [Microsoft Power Automate プラットフォームの詳細](/power-automate/)
- [パートナー センター Webhook](/partner-center/develop/partner-center-webhooks)
