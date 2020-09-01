---
title: パートナー販売 Connect (PSC) からパートナーセンター (PC) に移行するパートナー向けの紹介101
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft の認定パートナーとして、Microsoft との共同販売を行うことができます。 取引を定義する方法、Microsoft に招待して共同作業を行う方法、または送信された取引を表示する方法を説明します。
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 207a6013f11ab795bf46e184a4e98379e3ef3301
ms.sourcegitcommit: 3670c6e7f22e4f56545886052b68b9d5b6b3092c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/01/2020
ms.locfileid: "89281346"
---
# <a name="guide-to-co-selling-in-partner-centerpc-for-partners-migrating-from-partner-sales-connect-psc"></a>Partner sales Connect (PSC) から移行するパートナー向けのパートナーセンター (PC) での共同販売のガイド

**適用対象**

- 紹介
- Microsoft と共同販売する
- PSC ユーザーアカウントのセットアップ
- Partner Sales Connect (PSC) ユーザー 

**適切なロール**

- アカウント管理者
- 紹介管理者
- Partner Sales Connect (PSC) 販売者
- Partner Sales Connect (PSC) 管理者
- Partner Sales Connect (PSC) 取引マネージャー

ご存じのように、会社は2020年12月31日の投稿にアクセスできなくなります。 パートナーセンターで Microsoft の販売元によって送信された取引を作成したり、取引を管理したり、取引を操作したりするために必要なすべてのものを見つけることができます。 ただし、違いはありますが、次のガイダンスを参考にして、パートナーセンターへの移行を円滑に進めることができます。

>[!Important]
> ここでは、移行に関する PSC にバナーが表示されているので、適切な場所にあります。 このガイドは、PSC での取引を管理するソリューション評価 (SA) および OEM IOT パートナーには適用されません。

## <a name="before-you-move-things-you-need-to-know"></a>移動する前に理解しておくべきこと

### <a name="if-you-are-psc-admin"></a>PSC 管理者の場合

- [パートナーセンター](https://partner.microsoft.com/)にログインするには、職場の電子メールが必要です。
- パートナーセンターの [アカウント管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant)に問い合わせて、アカウントを設定します。
- このドキュメントを読んで、パートナーセンターで共同販売する方法を説明します。
- すべての PSC ユーザー (管理者、取引先担当者、および販売者ロール) にパートナーセンターのユーザーアカウントを設定し、 [参照管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) ロールを割り当てます。

### <a name="if-you-are-psc-deal-manager-or-seller"></a>PSC 取引マネージャーまたは販売者の場合

- [パートナーセンター](https://partner.microsoft.com/)にログインするには、職場の電子メールが必要です。
- PSC で仕事用ではないアカウントを使用している場合や、勤務先の電子メールがパートナー組織とは異なる会社の場合は、PSC 管理者に連絡してアカウントをセットアップしてください。
- PSC へのログインに使用するアカウントに関係なく、パートナーセンターアカウントのセットアップが完了している場合は、PSC 管理者に確認してください。
- パートナーセンターと [紹介] セクションにアクセスできるかどうかを確認します。
- このドキュメントを参照して、パートナーセンターでのワークフローと変更について理解してください。

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>PSC の管理者として、次の手順を実行します。

[参照] タブが表示されない場合は、次のようになります。

- 会社の [アカウント管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) は、[紹介] タブへのアクセスを許可できます。アカウント管理者を見つけるには、パートナーセンターの右上にある歯車アイコンから [パートナー設定] にアクセスします。 左側のナビゲーションバーの2番目のレベルで [ユーザー管理] ページを選択します。 ページの右上にある [すべてのユーザー] を表示するドロップダウンをクリックし、"Account Admins" に変更します。 このページには、すべてのアカウント管理者が、それぞれの電子メール Id と共に表示されます。 これらのユーザーに連絡して、職場アカウントの "参照管理者" アクセスを取得してください。

>[!Important]
> 役割が PSC のユーザーのみを管理している場合は、パートナーセンターで [アカウント管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) ロールを取得できます。 ロールに共同販売機会の管理も含まれている場合は、 [参照管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) ロールを取得する必要があります。 また、psc 管理者が1つの変更管理者を指名して、すべての PSC 管理者が PC のアカウント管理者を個別に管理するのではなく、パートナーセンターアカウント管理者と協力します。

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="[パートナーの設定] ユーザー管理ページにアカウント管理者が表示されているイメージ。":::

- 左側のナビゲーションウィンドウの [紹介] タブに移動し、ページにアクセスできるかどうかを確認します。

>[!Note]
> 参照ページにアクセスするために資格情報を更新するには、パートナーセンターからログアウトしてから再度ログインする必要がある場合があります。

パートナーセンターでアカウントを設定した後、

- 次の手順として、PSC で "取引マネージャー" または "販売者" というロールを持つすべてのユーザーを招待します。
- 参照へのアクセスを支援した [アカウント管理](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) 者は、すべてのユーザーを招待できます。
- ユーザーを招待するときに、アカウント管理者に [参照管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) ロールを割り当てるように依頼します。
- 一部の PSC ユーザーは、パートナーセンターで使用しているものとは異なるドメインのアカウントを使用している可能性があります。 このようなユーザーは、Azure AD テナントに関連付けられている職場アカウントを使用して、パートナーセンターにサインインする必要があります。 [グローバル管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles)はこれを支援できます。 全体管理者を見つけるには、パートナーセンターの右上にある歯車アイコンから [パートナー設定] にアクセスします。 左側のナビゲーションバーの2番目のレベルの [ユーザー管理] ページをクリックします。 ページの右上にある "すべてのユーザー" と表示されているドロップダウンをクリックし、[全体管理者] に変更します。
- 全体管理者は、Azure AD テナントに新しいユーザーアカウントを作成するか、他のドメインアカウントユーザーにゲストユーザーのアクセス権を割り当てることができます。
- すべての PSC 取引マネージャーとユーザーに対してアカウントを設定したら、パートナーセンターにサインインし、左側のナビゲーションで [参照] タブに移動して、[参照] ページが表示されることを確認します。

企業が PDM を所有している場合-パートナーセンターアカウントがセットアップされていて、ユーザーが移動し、ロールとアクセス許可を持っている場合は、パートナーセンターに共同販売活動を移動できます。 移行が完了するまで待機するのではなく、スイッチを作成するように PDM に通知します。これにより、すべての新しい取引がパートナーセンターに送られます。
>[!Note]
>このスイッチを作成すると、PSC の既存のアクティブな取引だけを操作できます。 新しい取引を作成したり、PSC で Microsoft の販売元から取引を受けたりすることはできません。

会社が PDM を持っていない場合は、すべてのユーザーアカウントがすべてのユーザーによって設定および検証されていることを確認してください。 パートナーセンターで共同販売を開始できるという正確な日付について、PSC の電子メールとバナーで通知されます。 PSC では、既存のアクティブな取引を引き続き管理する必要があることに注意してください。

>[!Important]
>アクティブな取引は PC に移行されません。 2020年12月31日まで、取引を終了して登録することができます。

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>PSC 管理者、PSC 取引マネージャー、および PSC 販売者向けの次のステップ

パートナーセンターで共同販売を行う方法について説明します。
これは重要な手順であり、パートナーセンターでの共同販売の準備に役立ちます。 1日から効率的に共同販売できるように、パートナーセンターのワークフローと変更について理解します。 まず、このドキュメントを完全に読んでください。 [共同販売エクスペリエンスギャラリー](https://aka.ms/cosellexperience)でも、適切なリソースのセットを利用できます。

## <a name="major-differences-between-psc-and-pc-workflows"></a>PSC と PC のワークフローの大きな違い

|**シナリオ**|**Partner Sales Connect**|**パートナー センター**|
|-----|:-----|:-----|
|ユーザー ロール|PSC には、管理者、取引マネージャー、および販売者ロールがあります。|PC には、すべての取引に対して読み取りと書き込みの両方の権限を付与する [参照管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) ロールがあります。|
|共同販売に関してマイクロソフトに招待する|Microsoft 販売者によって開始されたパートナーによる明示的な ask はありません。|パートナーは、Microsoft の販売者向けヘルプが必要な場合は、 [明示的な要求](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) を行う必要があります。 Microsoft 販売者には、要求を拒否するオプションがあります。|
|Expiry|案件の有効期限という概念はありません。|パートナーがパートナーに受け入れられない場合、パートナーの受信取引は14日後に期限切れになります。 これは、Microsoft 販売者が14日以内に有効期限切れになった場合に、パートナーの送信取引と同じです。|
|Microsoft 販売者の詳細|取引が作成されるとすぐに表示されます。|Microsoft 販売者の詳細情報は、販売者がパートナーからの共同販売の招待を明示的に受け入れる場合にのみ、パートナーと共有されます。|
|[プライベートパイプライン](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities)|使用できません。|パートナーは、Microsoft の販売者に可視性を提供することなく、パイプラインを共有できます。|
|ソリューション|1つの価格表のみに属するソリューションは、取引に追加できます。|パートナーは、次のリストに属する [ソリューション](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) を追加できます。 a) Microsoft ファーストパーティカタログ (PSC のトランザクション取引取引と同様) のソリューション b) ソリューションと c) 他のサードパーティパートナーからのソリューションの共同販売 (PSC の ISV 取引ロールと同様)。|
|取引の割り当て|割り当てられた販売者だけが、取引を表示し、行動を取ることができます。|チームメンバーを追加して、取引先を指定することができます。このような場合、他の参照管理者がそれらの取引を表示または操作できなくなることはありません。|
|お客様の組織|自由形式のテキスト入力。|少数の文字を入力するだけで、 [D&B データベース](https://www.dnb.com/)に対して[顧客組織](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)を検索できます。 有効な名前と住所は、選択した内容に基づいて自動的に設定されます。|
|お客様の連絡先|必須ではありません。|プライベートパイプラインの共有には必須ではありません。 Microsoft 販売者が共同販売要求への参加を招待された場合に必要です。|
|パブリック API|使用できません。|パートナーセンターの紹介をプログラムで管理する[パブリック API](https://docs.microsoft.com/partner/develop/referrals) 。|

## <a name="psc-and-partner-center-field-mapping"></a>PSC とパートナーセンターのフィールドマッピング

このセクションは、PSC とパートナーセンター間の属性の正確なマッピングを理解するのに役立ちます。 PSC の各画面は、「パートナーセンターの共同販売機会」セクションで関連するビューと比較されます。 

>[!Note]
>PSC のスクリーンショットの黄色いバブルに記載されている番号に従って、パートナーセンターで同等の属性を見つけます。 赤色のバブルは、取引先センターでそのファイリングを利用できないことを示しています。

**パートナーセンターにおける PSC のホームページと共同販売機会の既定のビュー**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="パートナーの Sales Connect のホームページとパートナーセンターの共同販売機会の既定のビューとの間のフィールドマッピングを示す画像。":::

**PSC グリッドビューとパートナーセンター取引ビュー**

- PSC のようなリストビューはパートナーセンターにはありません。  すべての取引は、顧客情報と取引の種類を使用して、received または created の最新の日付に基づいて一覧表示されます。 既定では、ビューの最初の処理が選択されています。 PSC テーブル形式で表示される値の大部分は、PC の詳細ビューで利用できます。
- 取引の役割は、PC では必須のフィールドではありません。 どのワークフローにも表示されず、キャプチャされることもありません。 これは、取引先に追加されたソリューションに基づいて、Microsoft 販売者側で自動的に派生します。
- 最後に変更された日付は、PC の [紹介の詳細] ページには表示されません。 パートナーは、並べ替え機能を使用して、最終更新日に基づいて取引を並べ替えることができます。

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Partner Sales Connect (PSC) グリッドビューとパートナーセンター取引ビューの間のフィールドマッピングを示す画像。":::

**PSC とパートナーセンターの案件の詳細ビュー**

- パートナーは、パートナー取引詳細ビュー (6) の [編集] ボタンをクリックして、取引を編集できます。 [編集] ボタンをクリックすると、すべてのフィールドが編集可能になります。このオプションを選択すると、処理に対して行われた編集を保存または取り消すことができます。
- パートナーセンターで取引を終了するオプションはありません。
- 顧客の結果はパートナーセンターでは利用できません。 顧客とのやり取りに関連するすべての詳細情報は、「PC」の「メモ」セクションで更新できます。
- 推定ソリューションの終了日は、パートナーセンターの OEM IOT 取引でのみ利用できます。 その他の種類の取引では表示されません。
- PC では、ライセンスプログラムは必要ありません。 これは、取引で選択されたソリューションに基づいて自動的に推論されます。

>[!Note]
>"勝ち" または "lost" とマークされている案件は、その投稿を編集することはできません。 これらのターミナル状態のいずれかに取引を移動するときは注意が必要です。

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Partner Sales Connect (PSC) 取引詳細ビューとパートナーセンターの取引詳細ビューの間のフィールドマッピングを示す画像。":::

**PSC の [製品の追加] ビューとパートナーセンターの [ソリューションの追加] ビュー**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Partner Sales Connect (PSC) の [製品の追加] ビューと、パートナーセンターの [ソリューションの追加] ビューの間のフィールドマッピングを示す画像。":::

**PSC およびパートナーセンターでのユーザー管理**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="アカウント設定ビューの Partner Sales Connect (PSC) ユーザー管理ホームとパートナーセンターのユーザー管理の間のフィールドマッピングを示す画像。":::

**PSC およびパートナーセンターでのユーザーロールの割り当て**

- PSC 管理者の同等の役割は、パートナーセンターのアカウント管理者ロールです。
- パートナーセンターには、参照管理者ロールである共同販売取引管理のロールが1つだけあります。

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Partner Sales Connect (PSC) ロールの割り当てビューとパートナーセンターロールの割り当てビューの間のフィールドマッピングを示す画像。":::

**PSC およびパートナーセンターでの通知**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Partner Sales Connect (PSC) 通知とパートナーセンターの通知ビュー間のマッピングを示す画像。":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>PSC からパートナーセンターへの移行-よく寄せられる質問

**四半期.パートナーセンターにアクセスできない場合はどうすればよいですか?**

[アクセスなし] ページに表示されている管理者に連絡して、ロールを割り当てることができます。 [紹介] セクションの [読み取りと書き込み] アクセス許可には "[参照管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals)" ロールが必要です。 ビジネスプロファイルのみを管理している場合は、パートナーセンターの "ビジネスプロファイル管理者" ロールが必要になります。

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="パートナーセンターにアクセスなしのエクスペリエンスを示すイメージ。":::

**Q2.パートナーセンターの [紹介] セクションへのアクセス権を付与できるユーザー**

[アカウント管理者](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant)は、[紹介] タブへのアクセスを許可できます。アカウント管理者を見つけるには、パートナーセンターの右上にある歯車アイコンから [パートナー設定] にアクセスします。 左側のナビゲーションバーの2番目のレベルの [ユーザー管理] ページをクリックします。 ページの右上にある [すべてのユーザー] を表示するドロップダウンをクリックし、"Account Admins" に変更します。 このページには、すべてのアカウント管理者が、それぞれの電子メール Id と共に表示されます。 これらのユーザーに連絡して、職場アカウントの "参照管理者" アクセスを取得してください。

**Q3.アカウントでは、[+ 新しい商談] ボタンがグレーで表示されます。取引の作成を開始するにはどうすればよいですか?**

これは、パートナーセンターで使用している MPN 組織に関連付けられている共同販売準備済みソリューションがない場合にのみ発生します。 お客様のソリューションの MPN ID を取得するには、PDM に連絡するか、「PSC の移行後に新しい商談ボタンがグレーで表示される」という問題に言及するサポートチケットを作成してください。

**終わり.PSC などの組織の特定の担当者に取引を割り当てることはできますか。**

チームメンバーを特定の取引に割り当てることができます。 他の参照管理者がこれらの取引を表示または操作することをブロックすることはありません。 

**Q5.自分に割り当てられているすべての取引のビューはありますか。**

[お気に入り] 機能を使用できます。これは [ユーザーレベル] タブです。自分に割り当てられているすべての取引をお気に入りとしてマークして、取引にすばやくアクセスできるようにすることができます。

**Q6.取引の読み取り専用ビューはありますか。**

いいえ。参照セクションには、取引の読み取り専用ビューはありません。 すべての紹介管理者は、すべての取引に対する完全な読み取りと書き込みアクセス権を持ちます。

**Q7.商談を獲得後に登録するにはどうすればよいですか。**

取引が以下の条件を満たしている場合は、 [登録](https://docs.microsoft.com/partner-center/register-deals)を開始するポップアップが表示されます。

- 取引に関連するインセンティブ対象ソリューションがあります。
- Microsoft 販売者は、商談に参加するよう招待されています。または、お客様に招待します。
- Microsoft カードがパートナーセンターで受け入れられるか、または獲得された状態になっています。

**Q8.[取引登録] セクションで [+ 新しい取引登録] ボタンをクリックすると、エラーメッセージが表示されます。取引を登録するにはどうすればよいですか。**

"+ 新しい商談登録" は、パートナーセンターで対応する共同販売機会を登録しないように、ISV connect プログラムに登録されているパートナーによってのみ使用されます。 共同販売の機会に取引を登録する場合、取引が受注としてマークされているときにポップアップが表示され、それが取引登録の条件を満たしている場合は、ポップアップが表示されます。

**Q9.顧客組織を必須として追加していますか?**

はい。パートナーセンターでは、 [顧客組織](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) を追加することが必須です。 最初に、顧客の所在地を検索します。 使用している詳細情報に基づいています。具体的には、正確な建物名を含めたり、市区町村の詳細を指定したりすることができます。 組織の検索では、入力した名前と一致するすべての法的エンティティがフェッチされるため、アドレスの詳細を入力する必要はありません。 すべての詳細は、選択した組織に基づいて自動的に入力されます。

**Q10.カスタマー連絡先の詳細は必須ですか?**

作成する [取引の種類](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities) によって異なります。 パイプラインを共有するだけで、Microsoft 営業組織の支援を必要としない場合は、顧客の連絡先の詳細を指定しないことを選択できます。 Microsoft 販売者が積極的に支援を求めている場合は、お客様の連絡先の詳細を入力する必要があります。 パートナーセンターで共同販売要求を作成する前に、お客様から明示的な同意を得る必要があります。

**Q11.商談に追加できるソリューションの数を教えてください。**

(PSC の ' 製品 ' に似た) 最大50のソリューションを商談に追加することができます。 PSC とは異なり、お客様独自の共同販売対象ソリューションのソリューション、Microsoft ファーストパーティの Sku、およびその他のサードパーティの共同販売対象ソリューションを組み合わせることができます。 パートナーセンターで選択または使用できる取引の役割はありません。 Microsoft の Sku では、必要に応じて、追加された各 SKU の数量と価格を追加することができます。

**Q12.商談を作成した後に Microsoft 販売者の詳細情報を確認するには、どうすればよいでしょうか。**

Microsoft の販売元は、Microsoft 側で関連する販売者ペルソナとの取引を作成する際に、正確なヘルプ要件を満たすことによってのみ割り当てられます。 Microsoft の販売者は、割り当て後でも、共同販売の招待を受け入れるか拒否するかを選択できます。 共同販売の招待が販売者に受け入れられた場合にのみ、Microsoft 販売者の連絡先の詳細情報で取引が更新されます。 Microsoft の取引先に対する SLA は、14日間です。 これは、パートナーが有効期限切れの状態になる前に、取引に対して行動する必要がある SLA と同じです。

**Q13.営業案件 ID はどこで確認できますか。**

PSC の営業案件 ID は、PC の取引 ID と同じです。 商談を開くと、取引名の横に取引 ID が表示されます。

**Q14.PDM から PC にアクセスするにはどうすればよいですか。**

PSC とは異なり、パートナーセンターには、直接 PDMs からアクセスすることはできません。 この機能を有効にするには、次のような複数のオプションがあります。

- OCP Insights-PDMs がそれらに関連する & の進行状況を表示するだけの場合は、OCP Insights ポータルを使用して組織のビューを取得できます。 これは内部ツールであり、PDMs とユーザーのみが使用できます。 OCP insights は、会社のユーザーには使用できないことに注意してください。
- パートナーセンターのゲストユーザー-PDM @microsoft.com アカウントをパートナーセンターのゲストユーザーとして追加し、それらに参照管理者ロールを割り当てて、参照を表示して操作できるようにすることができます。
- テナントに [新しいユーザー](https://docs.microsoft.com/partner-center/create-user-accounts-and-set-permissions#add-a-new-user) を作成する-独自のテナントに新しいユーザーを作成し、それらの詳細を PDM と共有して、アカウント内の他の参照ユーザーと同様の参照を表示して操作できるようにすることができます。

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>パートナーセンターでの取引の作成と管理に役立つリソース

共同販売に関するヘルプトピックをまだお読みになっていない場合は、次のリソースを参照して、パートナーセンターで取引を管理してください。

|**目的**   |**参照先**   |
|-----------------------|:-----------------------|
|[共同販売機会] ページのタブとナビゲーションについて|[共同販売セクションの移動](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#navigating-the-co-sell-section)|
|D&B 一覧からの顧客組織の選択 |[顧客を選択する](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)|
|[案件の詳細] セクションのフィールドの変更|[案件の詳細](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#deal-details)|
|会社の従業員を取引チームに追加する|[従業員を追加する](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-your-employees)|
|共同販売取引への対応|[共同販売取引を管理する](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#responding-to-a-co-sell-opportunity)
|パートナーセンターで受注した取引を登録する |[新しい取引の登録](https://docs.microsoft.com/partner-center/register-deals)
|紹介の洞察を取得し、参照の実行状況を確認する |[紹介の分析情報](https://docs.microsoft.com/partner-center/referral-insights)
|ビジネスプロファイルの作成と管理|[ビジネス プロファイルの管理](https://docs.microsoft.com/partner-center/create-a-marketing-profile)
|ビジネスプロファイルの潜在顧客を管理する |[見込み客を管理する](https://docs.microsoft.com/partner-center/manage-leads)|

## <a name="additional-resources"></a>その他のリソース

- Partner Sales パートナーセンター[ブックに接続](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx)して、パートナーの販売プロセスとロールを、パートナーセンターとパートナーの sales Connect を介して新しい販売プロセスに合わせます。
- [パートナーセンターの共同販売の操作ガイド](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -パートナーセンターを介して、潜在顧客の管理や共同販売の機会の管理、および取引の登録を行うために、運用モデルを識別するためのガイダンスです。
- [紹介管理デッキ](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -パートナーセンターを使用してリードと共同販売の機会を管理するための、視覚化されたステップバイステップの手順です。
- [商用マーケットプレースでの発行と管理](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) -視覚化されたステップバイステップの手順で、パートナーセンターを通じてプランを作成、管理、発行します。
