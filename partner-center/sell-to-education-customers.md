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
ms.openlocfilehash: 9d0cff4883e084ccc0acb37d8c3119d91e3f5530
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276452"
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

3. 完了したら、 [確認] を **選択します**。

   :::image type="content" source="images/eduaccountinfo.png" alt-text="教育顧客アカウント。":::

4. [確認] **を確認** すると、送信された情報が有効な場合は **InReview** 状態が表示されます。 

    :::image type="content" source="images/edu/create-review.png" alt-text="レビュー中の教育顧客アカウント。"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>教育顧客の検証状態を確認する

顧客の [アカウント] ページ **で、特別** な資格認定の **状態に関するページを参照してください**。
状態の例:

- 顧客が検証に合格した場合: 教育

   :::image type="content" source="images/edupassedvetting.png" alt-text="教育の検証が成功しました。":::

- 顧客が検証に合格しなかった場合: 教育顧客ではない

   :::image type="content" source="images/edu/fail-reason.png" alt-text="教育の検証に失敗しました。" lightbox="images/edu/fail-reason-expanded.png":::

- 顧客が教育顧客としてタグ付けされていない場合: なし

   :::image type="content" source="images/edu/account-one.png" alt-text="教育の顧客は、そのようなタグ付けされません。" lightbox="images/edu/account-one-expanded.png":::

- 顧客が教育顧客としてレビュー中の場合: レビュー中

    :::image type="content" source="images/edu/in-review.png" alt-text="教育のお客様がレビュー中です。" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>顧客アカウント情報を修正し、確認のために再送信する

顧客が最初の検証に失敗した場合は、情報を修正して再送信できます。

### <a name="correct-the-customer-account-information"></a>お客様のアカウント情報を修正する

顧客の情報を更新するには、グローバル管理者特権が必要です。 Office 365 ポータルで情報を更新します。このデータは、ポータルから更新パートナー センターです。

1. [ **アカウント]** ページに、顧客の資格が "教育顧客ではありません" と見なされるという情報が表示されます。

2. ブラウザーを更新してページをリセットします。 [更新] ボタン **が表示** され、 **特殊な修飾の状態が** [なし] に **設定されます**。

3. **[Update]\(更新\)** を選択します。 [サービス管理 **] ページで****、[Office 365] を選択します**。

4. ブラウザーの新しいタブで Office 365 管理センターにリダイレクトされます。 資格情報を使用してサインインを要求される場合があります。

5. **[設定]** を選択します。

6. 画面の **上部にある [** 組織プロファイル] タブを選択し、[組織情報] **を選択します**。 これで、顧客の詳細を更新できます。

7. サイドバーの **下部にある [** 変更の保存] を選択します。  

### <a name="resubmit-for-verification"></a>確認のために再送信する

1. [アカウント] タブパートナー センター顧客アカウント ページに **移動** します。 ブラウザーを更新し、[会社] ページが新しい情報に更新されたと確認します。 [更新 **] ボタン** を選択して、教育の再検証を要求します。

2. 更新された顧客の詳細が教育オファーの対象である場合は、Education に更新された特別な資格が **表示されます**。 引き続き **[Not an Education Customer]/(教育顧客ではない)が表示される場合は**、手動検証のためにサポートにお問い合わせください。

## <a name="next-steps"></a>次のステップ

- [特別価格の対象となる業界への販売](get-special-pricing-for-offers.md)

- [新しい顧客の追加](add-a-new-customer.md)

- [教育Minecraft: Education Editionサブスクリプションを販売する](minecraft-subscriptions.md)
