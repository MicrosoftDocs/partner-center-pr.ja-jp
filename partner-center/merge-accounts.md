---
title: パートナー アカウントを別のパートナー アカウントにマージする
description: パートナーアカウントをパートナーセンターの別のパートナーアカウントにマージする方法について説明します。パートナーセンターで、Microsoft パートナーがアクティブである場合に使用します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276639"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a>パートナー アカウントを別のパートナー アカウントにマージする

**適切なロール**: アカウント管理者

複数の企業がアクティブな Microsoft パートナーであり、パートナーセンターにアカウントを持っている場合、それらのアカウントをマージすることができます。

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a>2つのパートナーがパートナーセンターのアカウントをマージすることを選択した場合の動作

- マージを開始するパートナー組織は、パートナーグローバルアカウント (PGA) になります。

- 招待された組織の PGA が、発信元企業の場所になります。

- マージするアカウントのすべての場所は、PGA の下の場所になります。

- アカウントの合併が完了すると、PGA プロファイル内の場所やユーザーなど、両方のアカウントの詳細が表示されます。 このプロセスを元に戻すことはできません。

- この統合中に、場所のすべての MPN Id が保持されます。

- ユーザーのロールが引き継がれます。 たとえば、特定の場所のインセンティブ管理者であるユーザーは、合併後もそのロールを持ち、合併前に見たインセンティブを確認することができます。

- Azure AD テナントと CSP アカウントはマージされず、影響もありません。

- 両方の会社に関連付けられている公開済みプランと共同販売パイプラインデータは保持されます

### <a name="view-of-merged-accounts"></a>マージされたアカウントの表示

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="アカウントの合併。":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a>パートナーセンターアカウントを別のパートナーセンターアカウントにマージするように招待されている場合の対処方法

アカウントの結合への招待に同意する場合は、次のようにします。MPN ID と場所は、招待されたパートナーアカウントの PGA にマージされます。

- ユーザーは、自分のロールとそのままの状態で、統合されたアカウントに移動します。

- 既存の特典とコンピテンシーは、合併後に更新されるまで、両方の企業において保持されます。 更新時、アカウントは1つの会社として扱われ、標準の更新規則が適用されます。

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a>パートナーがアカウントを結合する場合のプログラムと利点への影響について理解する

- すべての既存のコンピテンシー (Gold/シルバー)、購入 (Microsoft Action Pack など)、および関連する特典は、統合時に保持されます。 両方の企業が同じコンピテンシーを持ち、もう1つはゴールドで、もう1つはゴールドの場合、最高レベルのスキルを持つコンピテンシーが獲得され、パートナーは次の更新まで、そのコンピテンシーに対して1つのシルバー特典とゴールド特典のセットを持ちます。 

- Microsoft Action Pack の最高の記念日は、合併後も保持されます。 たとえば、会社1の記念日が Action Pack 更新の場合は6月2020、会社2の Action Pack 更新の記念日が2020年10月である場合、Microsoft では、マージされた会社の新しい記念日として2020年10月日を使用します。

- アカウントの合併中、次回の更新までは、各アカウントは Action Pack やコンピテンシーの特典を保持します。 更新時には、標準 Action Pack とコンピテンシー更新ルールが適用されます。

- 更新が行われると、コンピテンシーの達成と Action Pack に含まれている特典が、パートナー企業のパートナーグローバルアカウントに実装されます。

  - Microsoft Action Pack: パートナー企業は、パートナーのグローバルアカウントごとに1つの Action Pack を購入できます。

  - コンピテンシー: パートナー企業は、最大の達成度に関連するコア特典の1つのパッケージと、パートナーがパートナーグローバルアカウントごとの資格を持つコンピテンシー固有の特典を受け取ります。

- すべてのメリットについては、 [Microsoft Partner Network 特典の使用方法](https://aka.ms/partner-benefits-use-guide)に関するガイドを参照してください。 例: アクティブ化された O365 E3 トークンは、アクティブ化してから12か月間機能します。 トークンがテナントのライセンスに対してアクティブ化されると、そのライセンスは別のテナントに移動されない可能性があります。

- 両方の企業の MCP ID の関連付けが保持され、PGA MPN ID に関連付けられます。

- 市場投入と技術的なメリットは、コンピテンシーコア特典として提供されます。 マージ後、銀行と税の情報を確認して正確さを確認することをお勧めします。

- 会社が Azure エキスパート MSP プログラムに含まれている場合、特典は更新されるまで保持されます。

- 会社が高度な特殊化を獲得している場合は、両方のアカウントで保持されます。

- ソフトウェアアシュアランスのバウチャーは、両方のアカウントにわたって保持されます。 

- または PAL の関連付けには影響しません。 関連付けられた収益の投稿は、新しいパートナーグローバルアカウントへのフローを開始します。

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a>パートナーセンターアカウントをパートナーセンターアカウントにマージするように会社を招待する

>[!Note]
>アカウントの合併を実行するには、会社の **アカウント管理者** である必要があります。

1. パートナーセンターのダッシュボードから [ **設定** ] を選択します。 

2. [ **Account merge**] を選択します。

3. 自分と結合するために招待するアカウントの **パートナープロファイル** にある MPN ID を追加します。 パートナーのグローバル MPN ID を使用する必要があります。 Location MPN ID を使用することはできません。

4. [ **マージ**] を選択すると、パートナー企業に招待が送信されます。 要求を受け入れると、パートナーセンター内でアカウントのマージを開始できます。 組織がアカウントのマージ要求を拒否した場合、その要求が拒否された理由を説明することができます。 [ **マージ履歴**] では、すべてのアカウントのマージの一覧を使用できます。
 
### <a name="example-of-two-companies-merging-accounts"></a>アカウントをマージする2つの企業の例

1. Contoso, Ltd. 

    a. [グローバル MPN id 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile)と[MPN id 2222222 の](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)1 つの下位の場所。
  
    b. Azure AD テナント = @contoso.com
 
    c. 2020年10月1日に有効期限が切れる gold コンピテンシー
2. Fabrikam, Inc. は
 
    a.  グローバル MPN ID 3333333 と MPN Id 4444444 と5555555の2つの下位の場所

    b.  Azure AD テナント = @fabrikam.com

    c.  2020年12月1日に有効期限が切れる2つの gold コンピテンシー
3.  Contoso 社が Fabrikam を購入し、 [ここ](https://partner.microsoft.com/dashboard/account/merger) に移動して、merge 要求を開始します。
4.  Fabrikam はパートナーセンターにサインインし、手順 #3 で Contoso が行ったのと同じページに移動して、Contoso の要求を承認します。
5.  Contoso は、同じページでのマージの詳細を確認し、アカウントの合併を続行するための確認を提供します。
6.  合併後、会社のアカウントは次のように表示されます。

    a.  グローバル MPN ID 1111111 と4の下位の location MPN Id (2222222、3333333、4444444、5555555) を持つ Contoso という会社。
    
    b.  @contoso.com @fabrikam.com 同じパートナーセンターアカウントにアクセスできる2つの Azure AD テナント (+) があります。
    
    c.  これには、2020年10月1日に有効期限が切れ、もう1つは2020年12月1日という2つのコンピテンシー特典パッケージがあります。 2020年12月1日に、1つのコンピテンシー特典パッケージとして更新することができます。 これらの機能を更新すると、Contoso は1つの特典パッケージのみを保持できる場合でも、3つのコンピテンシーをすべて保持します。
    
7.  Contoso の管理者は、ユーザーのパートナーセンターの役割を引き続き管理し @contoso.com ます。 Fabrikam の管理者は、ユーザーのパートナーセンターの役割を引き続き管理し @fabrikam.com ます。 Contoso の管理者は、fabrikam のテナントにゲストとして招待されている場合にのみ、Fabrikam のユーザーを管理できます。
8.  Contoso は @fabrikam.com テナントを無視し、 @contoso.com 新しいロールとアクセス許可を持つ Fabrikam の従業員に新しい資格情報を再発行することができます。

## <a name="next-steps"></a>次のステップ

- [ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)

- [パートナー プロファイルの情報を確認する](update-your-partner-profile.md)

- [パートナーが自分で使用するために Azure サブスクリプションを購入できるように Azure パートナー共有サービスを追加する](shared-services.md)
