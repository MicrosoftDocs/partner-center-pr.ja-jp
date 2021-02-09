---
title: インセンティブに関する FAQ
ms.topic: how-to
ms.date: 02/05/2021
description: Microsoft インセンティブに関してよく寄せられる質問。 この記事には、ユーザーロール、登録方法、またはエラーメッセージの処理方法に関する質問が含まれています。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 332832b14e3434824aee2b1a6bcf7eb321fb7a60
ms.sourcegitcommit: 2d1f0d7bc897278ef37af6d43c1a088f5ca14807
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/08/2021
ms.locfileid: "99835069"
---
# <a name="frequently-asked-questions-on-incentives"></a>インセンティブに関してよく寄せられる質問

**適切なロール:**

- インセンティブ管理者

- インセンティブ ユーザー

## <a name="do-i-need-to-be-the-global-admin-to-enroll-in-incentives"></a>インセンティブに登録するには、グローバル管理者である必要がありますか。

いいえ。 全体管理者とアカウント管理者は、ユーザーをインセンティブ管理者として割り当てることができます。 インセンティブ管理者は、パートナーセンターを通じて会社のインセンティブプログラムを管理します。 詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

## <a name="what-do-i-need-to-do-if-i-find-my-company-is-already-a-member-of-the-microsoft-partner-network-mpn"></a>会社が既に Microsoft Partner Network (MPN) のメンバーであることが判明した場合は、どうすればよいですか。

MPN に参加しようとすると、会社が既にメンバーである場合、MPN はドメインを認識し、既存のアカウントに関連付けます。 既存のアカウントは、同じ電子メールドメインを使用している会社または関連会社である場合があります。また、同じ Azure アクティビティディレクトリ (Azure AD) を使用して複数のドメインを管理することもできます。

主要な連絡先は、[法的プロファイル] ページで確認できます。 場所が MPNHQ の場所である場合は、インセンティブを管理するために必要なアクセス許可を設定するだけで済みます。 ロールとアクセス許可の詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

MPNHQ の所在地と同じ国にいない場合、このシナリオの詳細については、 [多国籍アカウントの説明](https://support.microsoft.com/help/4515619/special-considerations-for-multi-national-partners-joining-the-microso) を参照してください。

## <a name="what-user-roles-are-available"></a>使用できるユーザーロール

パートナーセンターで会社を登録したユーザーは、既定では主要連絡先とグローバル管理者になります。 管理者は、ポータルでユーザーを招待および管理できます。

インセンティブの主要な役割は、インセンティブ管理者とインセンティブユーザーです。 インセンティブ管理者は、インセンティブプログラムに登録し、パートナーの銀行と税金の詳細を管理できます。 インセンティブユーザーは、ツールでレポートを表示して、支払い額と各支払いの内訳を確認できますが、銀行の詳細を表示または編集することはできません。 どちらのロールも、パートナーグローバルアカウントの下のすべての場所に適用できます。

詳細については、「 [アクセス許可の概要](permissions-overview.md)」を参照してください。

## <a name="how-can-i-find-out-who-has-global-or-account-admin-rights-for-my-company"></a>会社のグローバルまたはアカウントの管理者権限を持つユーザーを見つけるにはどうすればよいですか。

ロールの変更を行ったり、新しいユーザーにロールを割り当てたりできる、グローバル管理者またはアカウント管理者を見つけるには、次のようにします。

1. パートナーセンターの右上にある [アカウント設定] アイコンで、[ **ユーザー管理**] を選択します。
2. **グローバル管理者** または **アカウント管理者** のいずれかでフィルター処理します。
3. また、 **[マイプロファイル**] にアクセスし、[ **役割とアクセス許可** ] を選択して、アクセス許可を昇格させるのに役立つ管理者の一覧を表示することもできます。
 
詳細については、「 [ロールを検索](find-your-role.md)する」を参照してください。  

## <a name="i-cant-access-incentives-using-my-credentials"></a>資格情報を使用してインセンティブにアクセスできません。

インセンティブが表示されない理由として、適切なアクセス許可がないことが考えられます。 この問題を解決するには、次の手順を使用します。

1. Azure AD テナントの資格情報 (自分の職場の資格情報) を使用して、 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインします。 サインインできない場合は、会社のグローバル管理者に問い合わせてください。

2. サインイン時に、 **職場アカウント** または **個人アカウント** から選択するように求められた場合は、[ **職場アカウント**] を選択します。

3. パートナーセンターのメニューで、[ **インセンティブ**] を選択し、[ **概要**] を選択します。 インセンティブ管理者またはインセンティブユーザーのアクセス許可がない場合は、会社のすべてのグローバル管理者とアカウント管理者の連絡先情報が表示されます。 これらの管理者のいずれかに問い合わせて、必要な MPN IDs およびインセンティブプログラムのインセンティブロールを取得してください。

4. 既にインセンティブ管理者ロールを持っている場合は、お客様がアクセスできる MPN IDs およびインセンティブプログラムについて、会社の登録が表示されます。

## <a name="some-enrollments-are-missing-from-the-incentives-overview-page"></a>インセンティブの概要ページに登録されていない登録があります。

ダッシュボードに表示されなくなったインセンティブプログラムを、から、またはに登録したことがある場合は、適切なアクセス権があるかどうかを再確認する必要があります。 インセンティブユーザーまたはインセンティブ管理者ロールを持つユーザーのみがプログラムを表示できます。 「 [ロールを検索する](https://docs.microsoft.com/partner-center/find-your-role)」を参照してください。

ロールまたはアクセス許可を変更する必要がある場合は、会社のグローバルまたはアカウント管理者にお問い合わせください。これらのユーザーについては、「 [グローバル管理者を見つける](https://docs.microsoft.com/partner-center/find-your-role#find-your-global-admin)」を参照してください。

[概要] ページには、Azure AD テナントに関連付けられているパートナーグローバルアカウント (PGA) に関連付けられている登録のみが表示されることに注意してください。 会社に複数の PGA がある場合は、それぞれに異なる資格情報が必要になります。

## <a name="who-should-i-contact-if-i-get-an-error-message-or-need-help-during-the-enrollment-process"></a>エラーメッセージが表示された場合、または登録プロセス中にヘルプが必要な場合は、どのユーザーに問い合わせる必要がありますか。

ダッシュボードの [インセンティブ] セクション内で問題が発生した場合は、オンラインサポートサービスがあります。サポートオプション (? アイコン) を右上にあります。

## <a name="next-steps"></a>次の手順

- [インセンティブの概要](incentives-get-started-intro.md)
