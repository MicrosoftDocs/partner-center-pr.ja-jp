---
title: Salesforce CRM パートナーセンターの共同販売コネクタ
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターの紹介を Salesforce CRM と同期します。 販売元は、CRM システム内から Microsoft と共同で販売することができます。
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: 726e9071347e1590885b4bf82676f7767311f945
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173680"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Salesforce CRM のための共同販売コネクタ - 概要

**適切なロール**: 紹介 admin |CRM のシステム管理者またはシステムカスタマイザー

パートナーセンターの共同販売コネクタを使用すると、販売元は CRM システム内から Microsoft と共同で販売することができます。 パートナーセンターを使用して共同販売取引を管理するためのトレーニングを行う必要はありません。 共同販売コネクタを使用して、Microsoft の販売者に連絡したり、Microsoft 販売者からの推薦を受け取ったり、紹介を受け入れたり拒否したりすることができます。また、商談の価値や決算日などの商談データを変更することもできます。  また、これらの共同販売取引に関するマイクロソフト販売者からの更新を受け取ることもできます。 パートナーセンターではなく、選択した CRM 内での作業中に、すべての紹介作業を行うことができます。

このソリューションは、Microsoft Power Automate ソリューションに基づいており、パートナーセンター api を使用します。

## <a name="before-you-install---pre-requisites"></a>をインストールする前に-前提条件

|**トピック**|**詳細**|**リンク**|
|--------------|--------------------|------|
|Microsoft Partner Network ID |有効な MPN ID が必要です|[MPN](https://partner.microsoft.com/)に参加するには|
|共同販売の準備完了|お客様の IP/サービスソリューションは、共同販売の準備ができている必要があります。|[Microsoft との販売](https://partner.microsoft.com/membership/sell-with-microsoft)|
|パートナー センター アカウント|パートナーセンターのテナントに関連付けられている MPN ID は、共同販売ソリューションに関連付けられている MPN ID と同じである必要があります。 コネクタをデプロイする前に、パートナーセンターポータルで共同販売の紹介を確認できることを確認します。|[アカウントの管理](create-user-accounts-and-set-permissions.md)|
|パートナー センターのユーザー ロール|コネクタをインストールして使用する従業員は、参照管理者である必要があります|[ユーザー ロールとアクセス許可の割り当て](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|CRM ユーザーロールは、システム管理者またはシステムカスタマイザーです。|[Salesforce CRM でロールを割り当てる](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Flow アカウントの Power Automate|テスト、ステージング、および運用のためのデータベースを使用して、新しい運用環境を作成します。 データベースを含む既存の運用環境がある場合は、再利用できます。 コネクタソリューションをインストールするユーザーには、Power Automate ライセンスとこの環境へのアクセス権が必要です。 インストールが失敗した場合は、進行状況を監視し、 [Power Automate](https://flow.microsoft.com/)の詳細情報を取得できます。 [**ソリューション**] の [**履歴の表示**] を選択します。|[環境の作成または管理](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Microsoft カスタムフィールド用の Salesforce パッケージのインストール

パートナーセンターと Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで、Microsoft 固有の紹介フィールドを明確に識別する必要があります。 このような境界は、パートナーの販売者チームが、共同販売のために Microsoft と共有する参照を決定する機能を提供します。

1. Salesforce で、 **メモ** をアクティブ化し、営業案件の関連リストに追加します。 [参照](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. 次の手順に従って **営業案件チーム** をアクティブ化します。
    - セットアップで、[**クイック検索**] ボックスを使用して営業案件チームの設定を検索します。
    - 必要に応じて設定を定義します。 [参照](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. Salesforce で、 [パッケージインストーラー](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV)を使用してカスタムフィールドおよびオブジェクトをインストールします。 このインストーラーを使用して、任意の会社にパッケージをインストールします。

    >[!NOTE]
    >をサンドボックスにインストールする場合は、URL の最初の部分をに置き換える必要があり `http://test.salesforce.com` ます。

1. Salesforce で、 **営業案件** 関連の一覧に Microsoft ソリューションを追加します。 追加したら、 **レンチ** アイコンを選択し、プロパティを更新します。

## <a name="best-practice-test-before-you-go-live"></a>ベストプラクティス: 運用前にテストする

運用環境で Power Automate ソリューションをインストール、構成、およびカスタマイズする前に、必ずステージング CRM インスタンスでソリューションをテストしてください。

- Microsoft Power Automate ソリューションをステージング環境/CRM インスタンスにインストールします。

- ソリューションのコピーを作成し、構成を実行して、ステージング環境でフローのカスタマイズを Power Automate します。

- ステージング/CRM インスタンスでソリューションをテストします。

- 成功した場合は、運用インスタンスにマネージドソリューションとしてインポートします。

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Salesforce CRM のパートナーセンターの紹介同期をインストールする

1. [Power Automate](https://flow.microsoft.com)にアクセスし、右上隅にある [**環境**] を選択します。 これにより、使用可能な CRM インスタンスが表示されます。

1. 右上隅にあるドロップダウンリストから適切な CRM インスタンスを選択します。

1. 左側のナビゲーションバーで [ **ソリューション** ] を選択します。

1. 上部のメニューの [ **AppSource を開く** ] リンクを選択します。

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="AppSource を開きます。":::

1. ポップアップ画面で、 **Salesforce のパートナーセンターの紹介コネクタ** を検索します。  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="今すぐ入手できるスクリーンショットです。":::

1. [ **今すぐ入手** する] ボタンを選択し、[ **続行**] を選択します。

1. 次のページで、アプリケーションをインストールする Salesforce CRM 環境を選択します。 使用条件に同意します。

1. その後、[ **ソリューションの管理** ] ページに移動します。  ページの下部にある矢印ボタンを使用して、[パートナーセンターの紹介] に移動します。 [パートナーセンターの紹介] ソリューションの横に、[**インストールのスケジュール**] が表示されます。 インストールには10-15 分かかります。

1. インストールが完了したら、[ [Power Automate](https://flow.microsoft.com)に戻り、[左側のナビゲーション領域] から [**ソリューション**] を選択します。 [ソリューション] の一覧で、 **Salesforce のパートナーセンターの紹介同期** が使用できるようになりました。

1. **Salesforce のパートナーセンター紹介同期** を選択します。 次の Power Automate フローとエンティティを使用できます。

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Salesforce フロー。":::

## <a name="configure-the-solution"></a>ソリューションを構成する

1. CRM インスタンスにソリューションをインストールしたら、[ [Power Automate](https://flow.microsoft.com/)に戻ります。

1. 右上隅にある [**環境**] ドロップダウンで、Power Automate ソリューションをインストールした CRM インスタンスを選択します。

1. 次の3つのユーザーアカウントを関連付ける接続を作成する必要があります。

   - 参照管理者の資格情報を持つパートナーセンターのユーザー
   - パートナー センターのイベント
   - ソリューション内の Power Automate フローを持つ CRM 管理者

   1. 左側のナビゲーションバーから [ **接続** ] を選択し、一覧から [ **パートナーセンターの紹介** ] ソリューションを選択します。

   1. 接続を作成するに **は、[接続の作成**] を選択します。

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="接続の作成を示すスクリーンショット。":::

   1. 右上隅の検索バーで、 **パートナーセンターの参照 (プレビュー)** を検索します。

   1. 参照管理者の資格情報ロールを使用して、パートナーセンターユーザーの接続を作成します。

   1. 次に、パートナーセンターのユーザーに、参照管理者の資格情報を使用してパートナーセンターのイベント接続を作成します。

   1. CRM 管理者ユーザーの Salesforce の接続を作成します。
  
   1. CRM 管理者ユーザーの Microsoft Dataverse 接続を作成します。

   1. すべての接続を追加すると、環境内に次の接続が表示されます。

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="接続を監視する方法を示すスクリーンショット。":::

### <a name="edit-the-connections"></a>接続を編集する

1. [ **ソリューション** ] ページに戻り、[ **既定のソリューション**] を選択します。 [**すべて**] をクリックして、[**接続の参照 (プレビュー)** ] を選択します。

   :::image type="content" source="images/connection-reference-video.gif" alt-text="接続の編集を示すスクリーンショット。":::

1. 省略記号アイコンを選択して、各接続を個別に編集します。 関連する接続を追加します。

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="atht のスクリーンショットは、コネクタを編集する方法を示しています。":::

1. 次の順序でフローを有効にする:
   - パートナー センター Webhook 登録 (Insider Preview)
   - [カスタマイズ]Salesforce から詳細を作成または取得する
   - 共同販売サービスをReferral-Salesforceするパートナー センター (Insider Preview)
   - パートナー センターに Microsoft 共同販売紹介の更新プログラムを追加する (Insider Preview)  
   - パートナー センター Salesforce へのアクセス (Insider Preview)
   - Salesforce から パートナー センター (Insider Preview)
   - Salesforce Opportunity to パートナー センター (Insider Preview)
   - Salesforce Microsoft Solutions to パートナー センター (Insider Preview)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Webhook API を使用してリソース変更イベントに登録する

Webhook API パートナー センター使用して、リソース変更イベントに登録できます。 これらの変更イベントは、HTTP 投稿として URL に送信されます。

1. [Salesforce **CRM パートナー センター (Insider Preview) にアクセスする] を選択します**。

1. [編集] **アイコンを選択し** 、 **[HTTP 要求を受信した場合] を選択します**。

1. [コピー] **アイコンを** 選択して、指定された **HTTP POST URL をコピーします**。

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="URL をコピーする方法を示すスクリーンショット。":::

1. **[Webhook のパートナー センター (Insider Preview)** フローを選択しPower Automate実行] を **選択します**。

1. 右側のウィンドウで **[フローの実行** ] ウィンドウが開き、[続行] を選択 **します**。

1. 次の詳細を入力します。

   - **Http トリガー エンドポイント**: この URL は、前の手順からコピーされました。
   - **登録するイベント**: 使用可能なすべてのイベント (**紹介** で作成されたイベント、紹介が **更新** されたイベント、 **関連** する紹介で作成された イベント、および関連する紹介が更新された イベント) **を選択します**。
   - **既存のトリガー エンドポイントが存在する場合は上書きしますか?**: はい。 特定の Webhook イベントに登録できる URL は 1 つのみです。

1. [フロー **の実行] を** 選択し、[完了] を **選択します**。

Webhook は、イベントをリッスン、作成、および更新できます。

## <a name="customize-synchronization-steps"></a>同期手順をカスタマイズする

CRM システムは高度にカスタマイズされ、CRM のセットアップにPower Automateソリューションをカスタマイズできます。 パートナー センター と CRM システムの間で共同販売の紹介が同期される場合、パートナー センター PC で同期されるフィールドは、カスタム フィールド マッピング ガイド の一覧に [表示されます](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S)。

フィールド マッピング ガイドに従い、必要に応じて、[カスタマイズ **] Salesforce** または環境変数から詳細を作成または取得するに関するページで適切な変更を行います。 将来のソリューションのアップグレードに影響を与える可能性Power Automateソリューション内の他のフローは更新しない。

次のカスタマイズを使用できます。

- **営業案件名に** チェック マークを表示する: 既定では、営業案件名の横にチェック マークが表示され、パートナー センター と Salesforce CRM の間の同期が正常に行っていることを示します。 同様に、同期に失敗した場合はクロス マークが表示されます。 営業案件名にチェック マークまたはクロス マークを追加しないようにするには、営業案件名環境変数の [表示] チェック マークの現在の値を [いいえ] に設定します。

- **ステージ名**:

  - **アクティブなステージ** 名: Salesforce の営業案件の営業パイプラインのステージです。  アクティブなステージを表し、アクティブなステージで受け入れ可能な状態の紹介とパートナー センター。 これは、オンホールド ステージの後の販売パイプラインの次のステージになります。 営業案件の販売ステージを保留ステージからアクティブステージに移動すると、パートナー センター での紹介が受け入れされ、変更の同期が開始されます。

  - **保留ステージ名**: Salesforce の営業案件の営業パイプライン内のステージの名前。 これは、保留ステージを表します。 まだ受け入れされていない Microsoft から共有される新しい共同販売紹介は、Salesforce のこのステージに設定されます。 保留ステージ中に営業案件に加えた変更は、その営業案件とパートナー センター。 この保留ステージから営業案件の販売ステージを移動すると、営業案件のパートナー センター受け入れ、変更の同期が開始されます。

- **顧客アカウントの国番号**: 新しい紹介を作成するときに、2 文字の国番号 (ISO 3166) を指定する必要があります。 既定では、国コードは Salesforce のアカウントの **BillingCountry** フィールドと同期されます。 同期する国コードの Salesforce に別のフィールドがある場合:

  - 2 文字のコードを含むアカウントの非lookup 国コード フィールドの場合:

    - Salesforce 環境変数 **の Customer Account Country Code** フィールド名を CRM のフィールド名で更新します。 表示名ではなく、フィールドの名前を指定してください。

    - [**カスタマイズ] Salesforce** の [作成] または [詳細の取得] を編集し、[CRMアクションで顧客アカウントを作成または取得する] に移動して **、CRM** の正しいフィールドに Country 値を割り当てる。 また、BillingCountry **から Country** 値の割 **り当てを削除します**。

  - アカウントの参照ベースの国コード フィールドの場合:

    - アカウントに新しいカスタム フィールドを追加し、ルックアップ ベースのフィールドで選択した値に基づいて、2 文字の国コード (ISO 3166) を自動的に設定します。その逆も同様です。

    - 非lookup 国コード フィールドの前の手順に従って、CRM の新しいカスタム フィールドと、その間で新しいカスタム フィールドを同期パートナー センター。

- **取引値**: 既定では、CRM の Amount パートナー センターとの間で同期されるトランザクションの **取引** 値。 CRM に、取引値を同期する別のフィールドがある場合:

  - Salesforce 環境変数 **の Deal 値** フィールド名を CRM のフィールド名で更新します。 表示名ではなく、フィールドの名前を指定してください。

  - **[カスタマイズ] Salesforce** から詳細を作成または取得し、[CRM での営業案件の作成または更新] に移動し、[新しい営業案件の作成] と [既存の営業案件の更新] アクションの両方を更新して、Salesforce の正しいフィールドに **DealValue** を割り当てる。

- **取引値の通貨コード**: Salesforce の取引価値通貨コード フィールドの名前。 このフィールド API 名は、Microsoft パートナー センター で紹介を作成または更新するときに、営業案件の取引価値の通貨コードを取得するために使用されます。 取引値の通貨コード フィールドが既定のフィールド **CurrencyIsoCode** と異なる場合は、この環境変数の現在の値を更新します。

  - Salesforce 環境変数 **の Deal 値の通貨** フィールド名を CRM のフィールド名で更新します。 表示名ではなく、フィールドの名前を指定してください。

  - **[カスタマイズ] Salesforce** から詳細を作成または取得し、[CRM での営業案件の作成または更新] に移動し、[新しい営業案件の作成] と [既存の営業案件の更新] アクションの両方を更新して、Salesforce の正しいフィールドに **DealValueCurrency** を割り当てる。

- **[共同販売の** 機会の同期] : **[は** い] に設定すると、共同販売とパイプライン共有の営業案件だけが、パートナー センター Salesforce に同期されます。 [いいえ] **に設定** すると、リード、共同販売、パイプライン共有の機会が、パートナー センター Salesforce に同期されます。 この変数は、Salesforce から パートナー センター に同期される機会には影響を与パートナー センター。

## <a name="update-environment-variable"></a>環境変数を更新する

環境変数の値を更新するには:

1. [ソリューション] ページ **に移動** し、[既定のソリューション] **を選択します**。 [すべて **] を選択** して[環境変数] を **選択します**。

1. 更新する必要がある値の環境変数を選択し、省略記号アイコンを使用して [編集] を選択します。

1. [**新しい値]** オプションを **使用して値** を指定して、現在の値を更新します (既定値は更新されません)。 値は、変数のデータ型と一致する必要があります。 たとえば、 [はい] または [いいえ] のデータ型は、[はい] または [いいえ] の値を受け入れる場合があります。

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="環境変数の更新を示すスクリーンショット。":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>エンドツーエンドの双方向の共同販売紹介の同期

Power Automate ソリューションをインストール、構成、カスタマイズしたら、Salesforce CRM と パートナー センター の間で共同販売紹介の同期をテストできます。

### <a name="pre-requisites"></a>前提条件

パートナー センター と Salesforce CRM 間で紹介を同期するには、Power Automate ソリューションで Microsoft 固有の紹介フィールドを明確に定義する必要があります。 この識別により、販売者チームは、共同販売のために Microsoft と共有する紹介を決定できます。

カスタム フィールドのセットは、Salesforce CRM ソリューション営業案件パートナー センターの参照同期の一部として **使用** できます。 CRM 管理者ユーザーは、営業案件のカスタム フィールドを含む別の CRM セクション **を作成する** 必要があります。

次のカスタム フィールドは CRM セクションの一部である必要があります。

- **[同期] パートナー センター:** 営業案件を他のユーザーと同期パートナー センター。 既定では、このフィールドの値は [いいえ] で、Microsoft と営業案件を共有するには、販売者が明示的に [はい] に設定する必要があります。 CRM から CRM に共有されるパートナー センター、このフィールドの値は [はい] に設定されます。

- **紹介識別子**: Microsoft の参照用の読み取りパートナー センターフィールド。

- **紹介リンク**: Microsoft サービスの紹介への読み取りパートナー センター。

- **Microsoft がどのように役立つのか**: 紹介に必要な Microsoft からのヘルプ。 共同販売の紹介を作成するには、Microsoft に必要な適切なヘルプを選択します。 顧客の連絡先は、共同販売の紹介を作成する機会に関連付けられている必要があります。 共同販売以外の紹介を作成するには、このフィールドを選択しない必要があります。 共同販売以外の紹介は、ヘルプが必要な適切なオプションを選択することで、いつでも共同販売の紹介に変換できます。

- **Microsoft パートナー センターの参照の可視性**: 参照の表示を選択パートナー センターします。 Microsoft の販売者に表示することで、共同販売以外の紹介が共同販売に変換される可能性があります。 Microsoft のヘルプが必要な場合、紹介は既定で Microsoft 販売者に表示されます。 このフィールドが表示済みとしてマークされた後は、元に戻す必要があります。

- **Microsoft CRM識別子**: 共同販売の紹介が作成され、Microsoft によって受け入れられると、このフィールドに Microsoft の CRM 識別子が入力されます。

- **Microsoft パートナー センター ソリューション**: 共同販売対応ソリューションまたは Microsoft ソリューションを機会に関連付けるカスタム オブジェクト。 1 つ以上のソリューションを営業案件に追加または削除できます。 Microsoft と共有する前に、営業案件に少なくとも 1 つの共同販売準備完了または Microsoft ソリューションを追加する必要があります。 このオブジェクトを営業案件に関連付けるには、CRM の **営業案件** フォームを更新します。

- **監査**: 参照と同期する読み取り専用パートナー センター証跡

### <a name="scenarios"></a>シナリオ

1. CRM で紹介が作成または更新され、次の方法で同期された場合の紹介パートナー センター。

   1. CRM の [営業案件] セクションに表示されているユーザーを使用して、Salesforce CRM **環境に** サインインします。

   1. Salesforce CRM 環境で新しい営業案件 **を作成パートナー センター、** セクション [Microsoft **パートナー センター]** が存在する必要があります。

   1. Salesforce CRM の [パートナー センター] アイコンを使用して、✔に同期された案件が特定されます。
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Salesforce 環境のスクリーンショット。":::

   1. この機会を Microsoft パートナー センター と同期するには、カード ビューで次のフィールドを設定してください。

      - **Microsoft が支援する方法:** 共同販売の紹介を作成するには、適切なヘルプ オプションを選択します。

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="カード ビューで適切なフィールドを取得する方法を示すスクリーンショット。":::

      - **[同期と同期パートナー センター:** はい
      - **顧客の連絡先**: 共同販売の紹介を作成するには、営業案件に顧客の連絡先を追加します。
      - **Microsoft ソリューション**: Microsoft と紹介を共有するには、有効な共同販売準備完了または Microsoft ソリューションを営業案件に追加します。

   1. [Sync with パートナー センター] オプションを [はい]**に設定した後**、10 分間待ち、自分のアカウントパートナー センターします。 紹介は Salesforce CRM と同期され、紹介リンクが設定されます。 エラーが発生した場合は、[監査] フィールドにエラー情報が入力されます。

   1. 同様に、[**パートナー センター と** 同期する ] オプションが [はい] に設定されている場合は、Salesforce CRM で営業案件を更新すると、変更は パートナー センター アカウントと同期されます。

2. Microsoft パートナー センターで紹介が作成または更新され、Salesforce CRM 環境で同期された場合の紹介の同期:

    1. ダッシュボード にサインインパートナー センター [します](https://partner.microsoft.com/dashboard/home)。

    1. 左側 **のメニューから** [紹介] を選択します。

    1. [新しい取引] オプションをクリックパートナー センター新しい共同販売紹介を作成します。

    1. Salesforce CRM 環境にサインインします。

    1. [Open **Opportunities] に移動します**。 Microsoft パートナー センターで作成された紹介は、Salesforce CRM で同期されます。

    1. 同期された紹介を選択すると、カード ビューの詳細が設定されます。

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Salesforce 営業案件ページのスクリーンショット。":::

>[!NOTE]
>**デプロイに関するヘルプが必要ですか?**
>共同販売紹介コネクタのデプロイに関するサポートについては、パートナー テクニカル コンサルタントに問い合わせてください。 実装を成功に向け、デプロイのサポートとベスト プラクティスを提供できます。
>
>詳細については、「技術プリ [セールスおよびデプロイ サービス要求を送信する方法」を参照してください。](technical-benefits.md)

## <a name="next-steps"></a>次のステップ

- [見込み客を管理する](manage-leads.md)

- [共同販売の機会を管理する](manage-co-sell-opportunities.md)

- [パートナー センター Webhook](/partner-center/develop/partner-center-webhooks)
