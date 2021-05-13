---
title: 教育顧客にオファーを販売する方法
description: 教育顧客を作成し、顧客にオファーを販売する方法についてパートナー センター。 教育顧客の確認状態の確認が含まれます。
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1b1b89841faf77a78c8cc268357daaaf95307223
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855405"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>教育顧客にオファーを販売する方法と、顧客に教育顧客を作成するパートナー センター

**適切なロール**: グローバル管理者|管理エージェント |セールス エージェント

## <a name="create-an-education-customer"></a>教育機関の顧客を作成する

この記事では、 で教育顧客を作成し、パートナー センター製品を販売する方法について説明します。 また、確認の状態を表示し、必要に応じて検証要求を再送信する方法も説明します。 現在、教育オファー **は、** ライセンス ベースのサービス (Microsoft 365 Dynamics、Intune など) でのみ使用できます。他の種類 (ソフトウェア サブスクリプション、永続的ソフトウェア、または Azure 製品) では使用できません。

> [!IMPORTANT]
> Microsoft は、新しく作成された各教育顧客テナントを検証して、教育オファーの資格を確認します。  検証プロセスの遅延を防ぐために、必要な情報を可能な限り正確かつ完全に入力してください。

1. パートナー センターにサインインします。

2. [顧客 **] を** 選択し、[ **顧客の追加] を選択します**。 [特別 **な資格** ] ドロップダウン **から [教育] を選択** します。  必要に応じて、残りのアカウント情報を入力します。  検証プロセスを支援する主なフィールドは次のとおりです。

   - **会社名**: 法人名を入力する - 検証に必須
   - **国/地域と住所の行**: 完全なエンティティのメール アドレスを入力します。確認に必要です
   - **電子メール アドレス**: 検証に必要な、無料または電子メールではなく、エンティティ所有 on.microsoft.com 電子メールを入力します
   - **顧客の連絡先情報**: これらの詳細は、検証プロセスの一部として使用されます
   - **プライマリ ドメイン名**: 顧客のアカウントと電子メール アドレスを作成するために使用されます。  スペースや特殊文字を含めない会社名に似た名前を選択します。  この名前は後で変更することはできません。

3. 操作が完了したら、[ **レビュー**] を選択します。

   :::image type="content" source="images/eduaccountinfo.png" alt-text="教育機関の顧客アカウント":::

4. **レビュー** を確認すると、送信された情報が有効な場合は、 **inreview** の状態が表示されます。 

    :::image type="content" source="images/edu/create-review.png" alt-text="教育機関の顧客アカウントのレビュー"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>教育機関の顧客の検証の状態を確認する

お客様の **アカウント** ページで、 **特別な認定の状態** を参照してください。
状態の例:

- 顧客が検証に合格した場合: 教育

   :::image type="content" source="images/edupassedvetting.png" alt-text="教育機関の検証に成功しました":::

- 顧客が検証に合格しなかった場合: 教育機関ではありません

   :::image type="content" source="images/edu/fail-reason.png" alt-text="教育機関の検証に失敗しました" lightbox="images/edu/fail-reason-expanded.png":::

- 顧客が教育機関の顧客としてタグ付けされていない場合: なし

   :::image type="content" source="images/edu/account-one.png" alt-text="教育機関のお客様にはタグ付けされていません" lightbox="images/edu/account-one-expanded.png":::

- お客様が教育機関としてレビューを行っている場合: レビュー中

    :::image type="content" source="images/edu/in-review.png" alt-text="教育機関のお客様はレビュー中です" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>お客様のアカウント情報を修正し、検証のために再送信する

顧客が初期検証に失敗した場合は、情報を修正して再送信することができます。

### <a name="correct-the-customer-account-information"></a>お客様のアカウント情報を修正する

顧客の情報を更新するには、グローバル管理者特権が必要です。 このデータはパートナーセンターポータルから更新できないため、Office 365 ポータルで情報を更新します。

1. [ **アカウント** ] ページには、顧客の資格が "教育機関ではない" と見なされることを示す情報が表示されます。

2. ブラウザーを更新してページをリセットします。 [ **更新** ] ボタンが表示され、 **特別な** 制限の状態が **[なし**] に設定されます。

3. **[更新]** を選択します。 [ **サービス管理** ] ページで、[ **Office 365**] を選択します。

4. ブラウザーの新しいタブで Office 365 管理センターにリダイレクトされます。 資格情報を使用してサインインするように要求される場合があります。

5. **[設定]** を選択します。

6. 画面の上部にある [ **組織のプロファイル** ] タブを選択し、[ **組織情報**] をクリックします。 これで、顧客の詳細を更新できるようになりました。

7. サイドバーの下部にある [ **変更を保存** ] を選択します。  

### <a name="resubmit-for-verification"></a>確認のために再送信します

1. [パートナーセンター] タブに移動し、[顧客 **アカウント** ] ページに移動します。 ブラウザーを更新し、会社のページが新しい情報に更新されていることを確認します。 [ **更新** ] ボタンを選択して、教育の再検証を要求します。

2. 更新された顧客の詳細が教育機関の資格を受けられる場合は、 **特別な要件** が **教育機関** に更新されていることがわかります。 まだ **教育機関のお客様でない** 場合は、手動による検証についてサポートにお問い合わせください。

## <a name="next-steps"></a>次の手順

- [特別価格の対象となる業界への販売](get-special-pricing-for-offers.md)

- [新しい顧客の追加](add-a-new-customer.md)

- [Minecraft の販売: 教育機関のお客様へのサブスクリプション](minecraft-subscriptions.md)
