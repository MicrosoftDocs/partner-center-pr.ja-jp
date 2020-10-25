---
title: インセンティブに関する FAQ
ms.topic: how-to
ms.date: 10/22/2020
description: Microsoft インセンティブに関してよく寄せられる質問。 この記事には、ユーザーロール、登録方法、またはエラーメッセージの処理方法に関する質問が含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 468ad99771aabfd42960e43e0a711e10eddc62f0
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2020
ms.locfileid: "92523597"
---
# <a name="frequently-asked-questions-on-incentives"></a>インセンティブに関してよく寄せられる質問

**適用対象:**

- パートナー センター

**適切なロール:**

- インセンティブ管理者

- インセンティブ ユーザー

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>インセンティブに登録するには、グローバル管理者である必要がありますか。

グローバル管理者である必要はありません。MPN 管理者は、インセンティブ管理者になる必要がある場合に他のユーザーを登録するように招待できます。一方、グローバル管理者は、新しいユーザーアカウントを設定できます。 ツールを使用して会社のインセンティブを管理するには、グローバル管理者である必要はありません。ロールとアクセス許可の詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network"></a>会社が既に Microsoft Partner Network のメンバーであることが判明した場合は、どうすればよいですか。

MPN に参加しようとすると、会社が既にメンバーである場合は、ドメインを認識し、既存のアカウントに関連付けられます。 同じ電子メールドメインを使用している会社または関連会社を指定することも、同じ Azure アクティビティディレクトリ (Azure AD) を使用して複数のドメインを管理することもできます。

プライマリ連絡先は、[パートナープロファイル] ページで確認できます。 場所が MPNHQ の場所である場合は、インセンティブを管理するために必要なアクセス許可を設定するだけで済みます。 ロールとアクセス許可の詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

MPNHQ の所在地と同じ国にいない場合、このシナリオの詳細については、 [多国籍アカウントの説明](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) を参照してください。

## <a name="what-user-roles-are-available"></a>使用できるユーザーロール

既定では、MPN に会社を参加させたユーザーが、主要な連絡先と MPN の管理者になります。 管理者は、ポータルでユーザーを招待および管理できます。 ロールとアクセス許可の詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

インセンティブの主要な役割は、インセンティブ管理者とインセンティブユーザーです。 インセンティブ管理者は、パートナーの銀行の詳細を管理します。 インセンティブユーザーは、ツールでレポートを表示して、支払い額と各支払いの内訳を確認できますが、銀行の詳細を表示または編集することはできません。 インセンティブ管理者とインセンティブユーザーのロールとアクセス許可の詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。 パートナーがインセンティブの登録を招待されるまで、これらのロールは選択できません。 両方のロールは、HQ の下にあるすべての場所に適用できます。

## <a name="how-can-i-find-out-who-has-admin-rights-for-my-company"></a>会社の管理者権限を持つユーザーを見つけるにはどうすればよいですか。

社内のグローバル管理者または MPN アカウント管理者の役割を持つユーザーを確認できます。 詳細については、「 [ロールを検索](/partner-center/find-your-role.md)する」を参照してください。  

## <a name="i-cant-access-incentives-using-my-credentials"></a>資格情報を使用してインセンティブにアクセスできません。

アクセスできない理由としては、パートナーセンターでアクセス許可が適切に設定されていないことが考えられます。 この問題を解決するには、次の手順を使用します。

1. Azure AD テナントの資格情報 (自分の職場の資格情報) を使用して、 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインします。 サインインできない場合は、会社のグローバル管理者に問い合わせてください。

2. サインイン時に、 **職場アカウント** または **個人アカウント**から選択するように求められた場合は、[ **職場アカウント**] を選択します。

3. パートナーセンターのメニューで、[ **インセンティブ**] を選択し、[ **概要**] を選択します。 インセンティブ管理者のアクセス許可を持っていない場合は、会社のすべてのグローバル管理者とアカウント管理者の連絡先情報が表示されます。 これらの管理者のいずれかに問い合わせて、必要な MPN IDs およびインセンティブプログラムのインセンティブロールを取得してください。

4. 既にインセンティブ管理者ロールを持っている場合は、お客様がアクセスできる MPN IDs およびインセンティブプログラムについて、会社の登録が表示されます。
 
## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>インセンティブの概要ページに登録されていない登録があります。

[インセンティブの **概要** ] ページに表示される登録数が予想よりも多い場合は、次の操作を実行できます。

1. [パートナー センターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインします。

2. [ **設定**] で [ [ユーザー管理](https://partner.microsoft.com/pcv/users)] を選択します。

3. 自分の名前を選択すると、アクセス許可が表示されます。 

ロールまたはアクセス許可を変更する必要がある場合は、会社のグローバルまたはアカウント管理者に問い合わせてください。

このページには、Azure AD テナントに関連付けられているパートナーグローバルアカウント (PGA) に関連付けられている登録のみが表示されることに注意してください。 会社に複数の PGA がある場合は、それぞれに異なる資格情報が必要になります。

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>エラーメッセージが表示された場合、または登録プロセス中にヘルプが必要な場合は、どのユーザーに問い合わせる必要がありますか。

ダッシュボードの [インセンティブ] セクション内で問題が発生した場合は、オンラインサポートサービスがあります。サポートオプション (? アイコン) を右上にあります。

## <a name="next-steps"></a>次のステップ

- [インセンティブの概要](incentives-get-started-intro.md)
