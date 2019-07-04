---
title: パートナーのセキュリティ要件 |パートナー センター
ms.topic: article
ms.date: 06/25/2019
description: アドバイザーとクラウド ソリューション プロバイダー プログラムに参加しているパートナーのセキュリティ要件について説明します。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory、クラウド ソリューション プロバイダー、クラウド ソリューション プロバイダー プログラム、CSP、コントロール パネルの仕入先、CPV、多要素認証、MFA、セキュア アプリケーション モデル、セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: 8f513b96619819cd6ba892625e47731170d22130
ms.sourcegitcommit: de88bb4cd994f1a106a5d02242261042958d4300
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2019
ms.locfileid: "67549538"
---
# <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

**適用対象**

- クラウド ソリューション プロバイダー プログラム内のすべてのパートナー
  - 直接の請求書
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロール パネルの仕入先
- すべてのアドバイザー

お客様とパートナーのセキュリティとプライバシーは、Microsoft の最優先事項です。 引き続きを侵害された id に関連する主より高度なセキュリティ攻撃の増加を確認します。 予防的な制御は、セキュリティ攻撃を阻止するために全体的な防御戦略の重要な役割を再生には、まず一連のパートナーや顧客を保護するために必須のセキュリティ要件を適用します。

> [!NOTE]
> ソブリン クラウド (21 vianet、米国政府機関、およびドイツ) を介して処理のすべてのパートナーが機能し、これらの新しいセキュリティ要件をすぐに採用を強くお勧めします。 ただし、これらのパートナーは、2019 年 8 月 1 日に有効な新しいセキュリティ要件を満たすには必要ありません。 Microsoft では、ソブリン クラウドの場合は、これらのセキュリティ要件の強制は、将来に関する詳細を提供します。

## <a name="overview-of-the-requirements"></a>要件の概要

クラウド ソリューション プロバイダー プログラム、コントロール パネルの仕入先、およびアドバイザー パートナーに参加しているすべてのパートナーは、パートナー テナントのサービス アカウントを含む、各ユーザーの Multi-factor Authentication (MFA) を適用する必要があります。 これを行う 2 つの有効化[ベースライン ポリシーを Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)します。 ベースライン ポリシーでは、多くの一般的な攻撃から組織を保護するための定義済みのポリシーのセットです。 これらの一般的な攻撃には、パスワード スプレー、再生、およびフィッシングを含めることができます。 ベースライン ポリシーは、Azure Active Directory のすべてのエディションで使用できます。 Microsoft はこれらの基準の保護ポリシーを使用できるようにさらに、クラス最高のセキュリティ プラクティスを実装するには、お客様やパートナーにすべてのユーザー。

有効にする必要がある 2 つのベースライン ポリシーは、次の表で説明します。

|**ポリシー**| |
|-----|-----|
|**管理者の MFA を要求します。**|管理者ポリシーに対して MFA を要求を有効にするには、Authenticator アプリを使用して、mfa に登録する管理者の役割のユーザーが必要です。 MFA の登録が完了すると、管理者がサインインするたびに MFA を実行する必要があります。|
|**エンドユーザーの保護**|エンドユーザーの保護は、ディレクトリ内のすべてのユーザーを保護するリスクに基づく MFA ベースライン ポリシーです。 このポリシーを有効にするには、Authenticator アプリを使用して、mfa に登録するすべてのユーザーが必要です。 ユーザーは、14 日間、その後 MFA に登録するまでのサインインからブロックされます、MFA 登録プロンプトを無視できます。 MFA に登録されると、リスクの高いサインインの試行中にのみ、ユーザーが MFA を求められます。 侵害されたユーザー アカウントは、自分のパスワードがリセットされ、リスク イベントが消去されたまでブロックされます。|

これらのポリシーを有効にすると、各ユーザーは同じ追加コストなしで Azure MFA を利用することができます。 サード パーティ製ソリューションを使用している場合は、Microsoft の商用クラウド サービスにアクセスするときに、各ユーザーの MFA を適用する必要があります。

> [!IMPORTANT]
> パートナー ディレクトリのすべてのユーザーに対して MFA が強制されますので、任意のオートメーションまたはユーザーの資格情報を利用するための統合に影響があります。 この影響に対処するには、オートメーションまたは統合は、Microsoft の商用クラウド サービスに接続する方法を変更する必要があります。 接続しているサービスは、トークン ベースの認証をサポートしているかどうかは、実装することをお勧め、[アプリケーション モデルをセキュリティで保護されたフレームワーク](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)します。

## <a name="what-actions-do-i-need-to-take"></a>実行する必要があるどのようなアクションをでしょうか。 

パートナー テナントのユーザーが保護されていることを確認するには、するには、(サービス アカウントを含む)、各ユーザーに対して MFA を強制する必要があります。 これは有効にすると実現できます、[管理者向けの MFA を要求](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)ベースライン ポリシー。 これらのポリシーを有効にする前がどのようにし、任意のオートメーションまたは統合と、ユーザーに影響する方法を理解しておく必要です。

> [!NOTE]
> [ベースライン ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)超過進化し続けます。 詳細については、ポリシーの進化は、ドキュメントを定期的に確認することをお勧めします。

### <a name="considerations"></a>考慮事項

パートナー ディレクトリのすべてのユーザーに、セキュリティ要件が適用ので、いくつかの考慮事項は、スムーズな展開に必要があります。 これらの考慮事項には、MFA、またアプリケーションや組織で使用される先進認証をサポートしていないクライアントを実行する必要がありますまたはできない Azure Active Directory でユーザーの識別が含まれます。

#### <a name="self-service-password-reset"></a>セルフ サービスのパスワード リセット

セルフ サービス パスワード リセット (SSPR) は、従業員が IT スタッフに連絡することがなく、パスワードをリセットできるようにする Azure Active Directory 機能です。 従業員は、登録する必要があります。 またはセルフ サービス パスワード リセット サービスを使用する前に登録します。 登録時に、従業員は自分の組織で有効になっている 1 つまたは複数の認証方法を選択します。

SSPR は、従業員が迅速にブロックを解除している場所や時間帯に関係なく動作を続行できます。 自体のブロックを解除するユーザーを許可すると、組織は、非生産性時間とパスワードに関連する最も一般的な問題の高いサポート コストを削減できます。

ときに、[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)ベースライン ポリシーが有効になっているまで、パスワードをリセットし、リスク イベントが閉じられているすべてのセキュリティを侵害されたユーザー アカウントはブロックされます。 この点を考えることをお勧めグローバル管理者である、各ユーザーが SSPR に登録するには、次を実行します。

1. 参照、 [SSPR のセットアップ ページ](https://aka.ms/ssprsetup)
2. ユーザー名とパスワードを入力します。
3. 少なくとも 1 つのパスワードのリセット時にあるかを確認するために使用する検証のオプションを構成します。  

アカウントが侵害されたときに、管理者は、影響を受けるユーザーのアクセスを復元するアクションを実行する必要があります。 参照してください、[ユーザーのブロック解除する手順](#recovering-compromised-accounts)詳細については、ユーザーのブロックを解除するプロセス。

#### <a name="legacy-protocols"></a>従来のプロトコル

レガシ認証プロトコル (IMAP、SMTP、POP3 など) は、認証要求を行うメール クライアントによって使用されます。 これらのプロトコルは、MFA をサポートしていません。 悪意のあるユーザーが MFA をバイパスしようとする従来のプロトコルに対する攻撃を実行するアカウントのセキュリティ侵害のほとんどが原因です。 パートナー ディレクトリのアカウントにログインするときに MFA が必要な悪意のあるユーザーが MFA をバイパスすることがないことを確認、これらのセキュリティ要件が従来のプロトコルからのすべての認証要求がブロックされます。

### <a name="enabling-the-baseline-policies"></a>ベースライン ポリシーを有効にします。

参照してください、[パートナーのセキュリティ要件のチュートリアルを実装する](tutorials/partner-security-requirements.yml)基準ポリシーの実装についてのガイド付きエクスペリエンス。  

#### <a name="require-mfa-for-admins"></a>管理者の MFA を要求します。

*管理者の MFA を要求*ベースライン ポリシーでは、最も特権の Azure Active Directory ロールと見なされる、次のディレクトリ ロールの MFA が必要です。

- 全体管理者
- SharePoint 管理者
- Exchange 管理者
- 条件付きアクセス管理者
- セキュリティ管理者
- ヘルプデスク管理者/パスワード管理者
- 課金管理者
- ユーザー管理者

管理者ポリシーに対して MFA を要求を有効にすると、上記の 9 つの管理者ロールは、Authenticator アプリを使用して、mfa に登録する必要があります。 MFA の登録が完了すると、管理者がサインインするたびに MFA を実行する必要があります。

お客様の組織は、これらのアカウントをスクリプトまたはコードで使用されているがある場合、は、それらを置き換えることを検討してください [の id を管理](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)します。

このポリシーを有効にして、管理者を保護する.

1. サインイン、 **Azure portal** グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者として。
2. 参照する**Azure Active Directory** > **条件付きアクセス**します。
3. ポリシーの一覧で選択**ベースライン ポリシー。管理者の MFA を要求する**します。
4. 設定**ポリシーを有効にする**に**ポリシーを使用して、すぐに**します。
5. クリックして **保存**します。

    ![管理者の MFA を要求します。](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> このポリシーを有効にする前に、ユーザーがレガシ認証プロトコルを使用していないことを確認します。 記事をご覧ください[方法。Azure Active Directory と条件付きアクセスをブロック レガシ認証](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)詳細についてはします。

> [!IMPORTANT]
> 委任された管理者特権を使用して Exchange Online の PowerShell に接続する機能に影響を与える既知の問題があります。 参照してください、 [Exchange Online PowerShell](#exchange-online-powershell)既知の問題の場合は、このポリシーを有効にする前にこの PowerShell モジュールを使用します。

#### <a name="end-user-protection"></a>エンドユーザーの保護

エンドユーザーの保護のベースライン ポリシーは、ディレクトリ内のすべてのユーザーを保護します。 このポリシーを有効にするには、すべてのユーザーに 14 日以内に Azure MFA の登録が必要です。 登録されると、リスクの高いサインインの試行中にのみ、ユーザーが MFA を求められます。 パスワードのリセットし、ジョンソンをリスクになるまで、侵害されたユーザー アカウントはブロックされます。

ポリシー**ベースライン ポリシー。エンド ユーザー保護**事前構成されていて、Azure portal で条件付きアクセス ブレードに移動するとき、上部に表示されます。

このポリシーを有効にして、ユーザーを保護する.

1. サインイン、 **Azure portal** グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者として。
2. 参照する**Azure Active Directory** > **条件付きアクセス**します。
3. ポリシーの一覧で選択**ベースライン ポリシー。エンド ユーザー protection (プレビュー)** します。
4. 設定**ポリシーを有効にする**に**ポリシーを使用して、すぐに**します。
5. クリックして **保存**します。

    ![エンドユーザーの保護](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> このポリシーを有効にする前に、ユーザーがレガシ認証プロトコルを使用していないことを確認します。 記事をご覧ください[方法。Azure Active Directory と条件付きアクセスをブロック レガシ認証](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use)詳細についてはします。

> [!IMPORTANT]
> 委任された管理者特権を使用して Exchange Online の PowerShell に接続する機能に影響を与える既知の問題があります。 参照してください、 [Exchange Online PowerShell](#exchange-online-powershell)既知の問題の場合は、このポリシーを有効にする前にこの PowerShell モジュールを使用します。

## <a name="common-issues"></a>一般的な問題

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

ベースライン ポリシーを有効にした後のオートメーションまたは統合が、次のような例外を発生していることを見つける可能性があります。

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

この例外の原因は、ユーザーの資格情報を使用して認証することと、MFA が必要です。 この例外に対処するためには、認証アクセス トークンを利用する必要があります。 参照してください、[アプリケーション モデルをセキュリティで保護されたガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)詳細についてはします。

>[!IMPORTANT]
>ほとんどの最新の Api と PowerShell モジュールは、認証アクセス トークンを使用することをサポートします。 ただしがいくつかありますが、現在この機能をサポートしません。 見ればを活用しようとしている API または PowerShell モジュールの場合は、認証アクセス トークンの使用をサポートを必要がある場合にメッセージを投稿し、[パートナー センターのセキュリティ ガイダンス グループ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)コミュニティ。

#### <a name="aadsts700082"></a>AADSTS700082

最初の更新トークンを生成した後 90 日間、次の例外を受け取るは可能性があるアプリケーション モデルをセキュリティで保護されたフレームワークを実装します。

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

に関しては、Azure Active Directory の更新の最長有効期間トークンは 90 日です。 このエラーに対処するためには、生成し、新しい更新トークンを安全に保存する必要があります。 Azure Active Directory にアクセス トークンの要求ごとに新しい更新トークンが返されるために、更新トークンをプログラムで更新することができますに注意してください。 有効期限が切れる前にセキュアに保管された更新トークンを更新する適切なロジックを実装することができます。

参照してください[Azure Active Directory で構成可能なトークンの有効期間](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)詳細についてはします。

### <a name="recovering-compromised-accounts"></a>侵害されたアカウントを回復します。

お客様を保護するため、Microsoft の漏洩した資格情報サービスが公開されているユーザー名とパスワードの組み合わせを検索します。 ユーザーのいずれかに一致する場合は、すぐにそのアカウントをセキュリティで保護を支援します。 漏洩した資格情報を持つものとして識別されるユーザーが侵害を確認します。 これらのユーザーは自分のパスワードがリセットされるまでのサインインからブロックされます。

自分のディレクトリで、機能が有効になっている場合、Azure AD Premium ライセンスが割り当てられているユーザーはセルフ サービス パスワード リセット (SSPR) 経由のアクセスを復元できます。 Premium ライセンスがなくてもユーザーがブロックされているは、手動によるパスワードのリセットを実行し、フラグが設定されたユーザーのリスク イベントを無視する管理者に連絡する必要があります。

#### <a name="steps-to-unblock-a-user"></a>ユーザーのブロック解除する手順

ユーザーがユーザーのサインイン ログを調べることで、ポリシーによってブロックされていることを確認します。

1. 管理者にサインインする必要があります、 **Azure portal**に移動します**Azure Active Directory** > **ユーザー** > ユーザーの名前をクリックし、移動しますサインインします。
2. 管理者をブロックされたユーザーにパスワードのリセットを開始するに移動する必要があります**Azure Active Directory** > **リスクのフラグ付きユーザー**
3. ユーザーの最近使用したサインイン アクティビティに関する情報を表示するアカウントがブロックされているユーザーをクリックします。
4. 次回ログイン時に変更する必要があります一時的なパスワードを割り当てるには、[パスワードのリセット] をクリックします。
5. ユーザーのリスク スコアをリセットするすべてのイベントを無視する をクリックします。

、には、ユーザーはサインインできるようになりました、自分のパスワードをリセットし、アプリケーションにアクセスします。

## <a name="known-issues"></a>既知の問題

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA が有効にすると、パートナーは顧客に対してアクションを実行する Exchange Online PowerShell を使用した、委任された管理者特権を利用できません。 参照してください[多要素認証を使用して Exchange Online PowerShell への接続](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)この制限に関する詳細についてはします。

## <a name="resources-and-support"></a>リソースとサポート

を通じて、[パートナー センターのセキュリティ ガイダンス グループ コミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)その他のリソースを見つけ、技術的な office 時間などの今後のイベントについて説明しますができます。 参照してください、[よく寄せられる質問](http://assetsprod.microsoft.com/security-requirements-faq.pdf)要件の詳細については、ドキュメント。

### <a name="developers"></a>開発者

- [セキュリティで保護されたアプリケーション モデルを有効にします。](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [パートナー センターの .NET のサンプル](https://github.com/microsoft/partner-center-dotnet-samples)
- [パートナー センターの Java サンプル](https://github.com/microsoft/partner-center-java-samples)
- [セキュリティで保護されたアプリケーション モデルを実装するパートナー センターの PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
