---
title: パートナーのセキュリティ要件 |パートナーセンター
ms.topic: article
ms.date: 07/18/2019
description: Cloud Solution Provider プログラムに参加するアドバイザーとパートナーのセキュリティ要件について説明します。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウドソリューションプロバイダー, Cloud Solution Provider プログラム, CSP, コントロールパネルベンダ, CPV, multi-factor authentication, MFA, 安全なアプリケーションモデル, セキュリティで保護されたアプリモデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: 0ce8a8dd5a58d1647c8d9e53dec0d0bbf7fe6592
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "68313935"
---
# <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

**適用対象**

- クラウドソリューションプロバイダープログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロールパネルベンダー
- すべてのアドバイザー

プライバシー保護とセキュリティの向上は、最優先事項の1つです。 最も防御力の高い防御策であり、最も弱いリンクとしてのみ強力であることがわかっています。 そのため、エコシステムのすべてのユーザーに対して、適切なセキュリティ保護が適用されていることを確認する必要があります。 パートナーと顧客を保護するために、クラウドソリューションプロバイダープログラムに参加している、advisor、コントロールパネルベンダー、およびパートナーに必要な一連の必須セキュリティ要件を導入しています。

2019年8月1日以降、パートナーテナント内のすべてのユーザー (サービスアカウントを含む) に対して multi-factor authentication を強制するために、すべてのパートナーが必要になります。

> [!NOTE]
> ソブリンクラウド (21Vianet、US Government、およびドイツ) を介して行動するすべてのパートナーが、これらの新しいセキュリティ要件をすぐに採用することを強くお勧めします。 ただし、2019年8月1日より有効になる新しいセキュリティ要件を満たすために、これらのパートナーは必要ありません。 Microsoft では、将来のソブリンクラウドに対するこれらのセキュリティ要件の適用に関する追加情報を提供します。

パートナーのセキュリティ要件に関連付けられている用語は、 [Cloud Solution Provider プログラムガイド](https://go.microsoft.com/fwlink/p/?LinkId=617100)に追加されました。 2019年8月1日以降、クラウドソリューションプロバイダープログラムに参加しているすべてのパートナーは、条件に準拠している必要があります。 アドバイザーに関連するので、同じ契約要件が適用されます。

必須のセキュリティ要件を実装していないパートナーは、これらの要件が適用されると、クラウドソリューションプロバイダープログラムでは、または代理管理者権限を利用して顧客のテナントを管理することはできません。 マイクロソフトは、要件の技術的な実施日を確立する過程で、詳細情報を使用してパートナーに通知します。

## <a name="what-actions-do-i-need-to-take"></a>どのようなアクションを実行する必要がありますか。

パートナーになるという高い特権を持つ性質を持つことから、各ユーザーが1つの認証に対して MFA チャレンジを行うようにする必要があります。 これは、次のいずれかの方法で実現できます。

- Azure AD Premium を実装し、各ユーザーに MFA が適用されるようにする
- [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の実装
- サードパーティのソリューションを実装し、各ユーザーに対して MFA が適用されるようにする

> [!IMPORTANT]
> これらの要件を厳密に適用するには、単一の認証ごとに MFA チャレンジが必要です。 Microsoft の商用クラウドサービスにアクセスするときに、MFA を使用した認証を避けるために、条件付きアクセスの機能を使用することはできません。

### <a name="considerations"></a>考慮事項

これらの要件は、サービスアカウントを含むすべてのユーザーにパートナーテナントで適用されるため、円滑なデプロイを実現するために必要な考慮事項がいくつかあります。 これらの考慮事項には、MFA を実行できない Azure AD のユーザーと、先進認証をサポートしていない組織で使用されるアプリケーションやデバイスを識別することが含まれます。

操作を実行する前に、次のことを確認することをお勧めします。

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>認証時に MFA の使用をサポートしていないアプリケーションまたはデバイスはありますか。

MFA レガシ認証を適用した場合、IMAP、POP3、SMTP などのプロトコルが使用されます。これらのプロトコルでは MFA がサポートされていないためです。 この制限に対処するために、[アプリパスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)と呼ばれる機能を使用して、アプリケーションまたはデバイスが引き続き認証されるようにすることができます。 [ここ](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリパスワードを使用する場合の考慮事項を確認して、環境で使用できるかどうかを判断する必要があります。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>作業中にユーザーが自分のモバイルデバイスを使用できないようにするポリシーがありますか。

企業のポリシーを特定して、従業員がモバイルデバイスを使用できないようにすることが重要です。これは、実装する MFA ソリューションに影響を与えるためです。 構成[基準ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の実装によって提供されるものなど、MFA ソリューションがあります。このソリューションでは、認証に認証アプリを使用することのみが許可されます。 組織がモバイルデバイスの使用を妨げるポリシーを持っている場合は、影響を受けているユーザーの[Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/)を購入するか、または適切な検証を提供するサードパーティ製ソリューションを実装する必要があります。オプション.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>認証にユーザー資格情報を活用するのはどのような自動化または統合ですか。

要件は、サービスアカウントを含め、各ユーザーに対して MFA を強制することであるため、パートナーディレクトリでは、認証にユーザー資格情報を活用する自動化または統合が影響を受けます。 そのため、このような状況で使用されているアカウントを特定することが重要です。 考慮する必要があるアプリケーションまたはサービスの例を次に示します。

- 顧客に代わってリソースをプロビジョニングするために使用されるコントロールパネル
- (CSP プログラムに関連する) 請求に使用される任意のプラットフォームとの統合と顧客のサポート
- Az、AzureRM、Azure AD、MS Online などのモジュールを使用する PowerShell スクリプト

上記の一覧は包括的なものではありません。 そのため、認証にユーザー資格情報を活用している環境で、アプリケーションまたはサービスの完全な評価を実行することが重要です。 MFA の要件に対応するには、可能な限り、セキュリティで[保護されたアプリケーションモデルフレームワーク](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)にガイダンスを実装する必要があります。 ここでは、セキュリティで保護されたアプリケーションモデルフレームワークを実装する方法を理解するのに役立つその他のリソースについて説明します。

- [パートナーセンターの .Net サンプル](https://github.com/microsoft/partner-center-dotnet-samples)-この GitHub リポジトリには、セキュリティで保護されたアプリケーションモデルフレームワークを実装する方法を示す .net を使用して開発されたサンプルが含まれています。
- [パートナーセンターの Java サンプル](https://github.com/microsoft/partner-center-java-samples)-この GitHub リポジトリには、セキュリティで保護されたアプリケーションモデルフレームワークを実装する方法を示す java を使用して開発されたサンプルが含まれています。
- [パートナーセンターの powershell-セキュリティで保護されたアプリケーションモデル](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)-powershell を使用してセキュリティで保護されたアプリケーションモデルフレームワークを実装する方法の詳細については、こちらの記事をご覧ください。
- [パートナーセンターのセキュリティガイダンスグループコミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)-これはオンラインコミュニティであり、今後のイベントについて学習したり、お客様に質問がある場合に質問したりすることができます。

### <a name="enforcing-mfa-for-all-users"></a>すべてのユーザーに MFA を適用する

このセクションでは、[ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を使用して、パートナーテナントの各ユーザー (サービスアカウントを含む) に MFA を適用する方法について説明します。 Azure AD Premium の使用を計画している場合は、[こちら](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)に記載されている手順に従ってください。

> [!NOTE]
> Azure AD と互換性のあるサードパーティのソリューションを使用すると、サービスアカウントを含むすべてのユーザーに MFA を適用できます。 ソリューションの実装方法の詳細については、ベンダーのドキュメントを参照してください。

ベースライン保護ポリシーは、多くの一般的な攻撃から組織を保護するのに役立つ一連の定義済みポリシーです。 これらの一般的な攻撃には、パスワードのスプレー、リプレイ、フィッシングなどがあります。 ベースライン保護ポリシーは、Azure Active Directory のすべてのエディションで使用できます。 Microsoft は、お客様とパートナーが最高クラスのセキュリティプラクティスを実装できるようにするために、これらのベースライン保護ポリシーをすべてのユーザーに提供しています。

次の表では、有効にする必要がある2つのベースライン保護ポリシーについて説明します。

|**ポリシー**| |
|-----|-----|
|**管理者に MFA を要求する**|[管理者に MFA を要求する] ポリシーを有効にすると、認証アプリを使用して、管理者ロールのユーザーが MFA に登録する必要があります。 MFA の登録が完了したら、管理者はサインインするたびに MFA を実行する必要があります。|
|**エンドユーザーによる保護**|エンドユーザー保護は、ディレクトリ内のすべてのユーザーを保護する、リスクベースの MFA ベースライン保護ポリシーです。 このポリシーを有効にすると、すべてのユーザーが Authenticator アプリを使用して MFA に登録する必要があります。 ユーザーは、MFA 登録のプロンプトを14日間無視できます。その後、mfa に登録されるまで、サインインがブロックされます。 MFA に登録されると、ユーザーは、危険なサインインの試行中にのみ MFA の入力を求められます。 危害を受けたユーザーアカウントは、パスワードがリセットされ、リスクイベントが破棄されるまでブロックされます。|

これらのポリシーを有効にすると、各ユーザーは、追加コストなしで認証を行うために Authenticator アプリを使用して Azure MFA を利用できるようになります。

#### <a name="configure-self-service-password-reset"></a>セルフサービスによるパスワードのリセットの構成

セルフサービスによるパスワードのリセット (SSPR) は、ユーザーがサポートチームに連絡しなくてもパスワードをリセットできるようにする Azure Active Directory の機能です。 ユーザーは、サービスを使用する前に、セルフサービスのパスワードリセットの登録または登録を行う必要があります。 登録中に、ユーザーは組織で有効になっている認証方法を1つまたは複数選択します。

[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)ベースライン保護ポリシーが有効になっている場合、侵害されたユーザーアカウントは、パスワードがリセットされ、リスクイベントが破棄されるまでブロックされます。 このことを考慮すると、グローバル管理者である各ユーザーは、次の手順を実行して SSPR に登録し、ロックアウトされないようにすることをお勧めします。

1. [SSPR セットアップページ](https://aka.ms/ssprsetup)に移動します。
2. ユーザー名とパスワードを入力してください
3. パスワードをリセットするユーザーを確認するために使用される検証オプションのうち、少なくとも1つを構成します。  

アカウントが侵害された場合、管理者は影響を受けたユーザーのアクセスを復元するアクションを実行する必要があります。 ユーザーのブロックを解除するプロセスの詳細については、[ユーザーのブロックを解除する手順](#recovering-compromised-accounts)を参照してください。

#### <a name="require-mfa-for-admins"></a>管理者に MFA を要求する

管理ベースラインポリシー*に mfa を要求*するには、次のディレクトリロールに対して mfa が必要です。これは、最も特権の高い Azure Active Directory ロールであると考えられます。

- 全体管理者
- SharePoint 管理者
- Exchange 管理者
- 条件付きアクセス管理者
- セキュリティ管理者
- ヘルプデスク管理者/パスワード管理者
- 課金管理者
- ユーザー管理者

[管理者に MFA を要求する] ポリシーを有効にすると、認証アプリを使用して MFA に登録するために上記の9つの管理者ロールが必要になります。 MFA の登録が完了したら、管理者は、サインインするたびに MFA を実行する必要があります。

組織でこれらのアカウントをスクリプトまたはコードで使用している場合は、それらを [マネージド id](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)に置き換えることを検討してください。

このポリシーを有効にし、管理者を保護するには:

1. グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者として **Azure portal** にサインインします。
2. **条件付きアクセス** **Azure Active Directory** > を参照します。
3. ポリシーの一覧で、[基準**ポリシー] を選択します。管理者**に MFA を要求します。
4. ポリシーを**直ちに使用**する**ようにポリシー**を設定します。
5. [ **保存**] をクリックします。

> [!WARNING]
> このポリシーを有効にする前に、ユーザーが従来の認証プロトコルを使用していないことを確認してください。 このポリシーの実装により、レガシ認証はブロックされます。

> [!IMPORTANT]
> 既知の問題があります。これは、委任された管理者特権を使用して Exchange Online PowerShell に接続する機能に影響します。 この PowerShell モジュールを使用する場合は、このポリシーを有効にする前に、 [Exchange Online PowerShell](#exchange-online-powershell)の既知の問題を参照してください。

#### <a name="end-user-protection"></a>エンドユーザーによる保護

エンドユーザー保護基準ポリシーは、ディレクトリ内のすべてのユーザーを保護します。 このポリシーを有効にすると、すべてのユーザーが Azure MFA に14日以内に登録する必要があります。 登録が完了すると、ユーザーは、危険なサインインの試行中にのみ MFA の入力を求められます。 危害を受けたユーザーアカウントは、パスワードのリセットとリスクの無視までブロックされます。

ポリシー **ベースラインポリシー:エンドユーザーに**よる保護は事前に構成されており、Azure portal の [条件付きアクセス] ブレードに移動すると上部に表示されます。

このポリシーを有効にし、ユーザーを保護するには:

1. グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者として **Azure portal** にサインインします。
2. **条件付きアクセス** **Azure Active Directory** > を参照します。
3. ポリシーの一覧で、[基準**ポリシー] を選択します。エンドユーザー保護 (プレビュー)** 。
4. ポリシーを**直ちに使用**する**ようにポリシー**を設定します。
5. [ **保存**] をクリックします。

> [!WARNING]
> このポリシーを有効にする前に、ユーザーが従来の認証プロトコルを使用していないことを確認してください。 このポリシーの実装により、レガシ認証はブロックされます。

> [!IMPORTANT]
> 既知の問題があります。これは、委任された管理者特権を使用して Exchange Online PowerShell に接続する機能に影響します。 この PowerShell モジュールを使用する場合は、このポリシーを有効にする前に、 [Exchange Online PowerShell](#exchange-online-powershell)の既知の問題を参照してください。

## <a name="common-issues"></a>一般的な問題

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

ベースラインポリシーを有効にすると、次のような自動化や統合によって例外が発生する可能性があります。

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

この例外の理由は、ユーザーの資格情報を使用して認証しているため、MFA が必要になるためです。 この例外に対処するには、認証にアクセストークンを使用する必要があります。 詳細については、「[セキュリティで保護されたアプリケーションモデル」ガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。

>[!IMPORTANT]
>最新の Api と PowerShell モジュールでは、認証にアクセストークンを利用する機能がサポートされています。 ただし、この機能は現在サポートされていません。 使用しようとしている API または PowerShell モジュールが認証にアクセストークンをサポートしているかどうかを判断するのに役立つ場合は、[パートナーセンターのセキュリティガイダンスグループ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)コミュニティにメッセージを投稿してください。

#### <a name="aadsts700082"></a>AADSTS700082

セキュリティで保護されたアプリケーションモデルフレームワークを実装した後、最初の更新トークンを生成してから90日後に、次の例外が発生する可能性があります。

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory に関しては、更新トークンの最長有効期間は90日です。 このエラーに対処するには、新しい更新トークンを生成し、安全に保存する必要があります。 注更新トークンをプログラムで更新することもできます。これは、アクセストークンの Azure Active Directory 要求があるたびに新しい更新トークンが返されるためです。 有効期限が切れる前に、安全に格納されている更新トークンを更新するための適切なロジックを実装できます。

詳細については、「 [Azure Active Directory で構成可能なトークンの有効期間](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。

### <a name="recovering-compromised-accounts"></a>侵害されたアカウントの回復

お客様を保護するために、マイクロソフトが提供する資格情報サービスは、一般公開されているユーザー名とパスワードの組み合わせを検出します。 これらのユーザーがいずれかのユーザーと一致した場合は、すぐにそのアカウントをセキュリティで保護することができます。 漏洩した資格情報があると識別されたユーザーは、侵害されたことを確認します。 これらのユーザーは、パスワードがリセットされるまで、サインインがブロックされます。

Azure AD Premium ライセンスを割り当てられたユーザーは、その機能がディレクトリで有効になっている場合、セルフサービスによるパスワードのリセット (SSPR) を使用してアクセスを復元できます。 Premium ライセンスがブロックされていないユーザーは、管理者に連絡してパスワードのリセットを手動で実行し、フラグが設定されたユーザーリスクイベントを破棄する必要があります。

#### <a name="steps-to-unblock-a-user"></a>ユーザーのブロックを解除する手順

ユーザーのサインインログを調べて、ポリシーによってユーザーがブロックされていることを確認します。

1. 管理者は、 **Azure portal**にサインインし、 **Azure Active Directory** > **ユーザー**に移動 > ユーザーの名前をクリックしてサインインに移動する必要があります。
2. ブロックされたユーザーに対してパスワードのリセットを開始するには、管理者が**リスクのフラグ**が設定された**Azure Active Directory** > ユーザーに移動する必要があります
3. ユーザーの最近のサインインアクティビティに関する情報を表示するには、アカウントがブロックされているユーザーをクリックします。
4. [パスワードのリセット] をクリックして、次のログイン時に変更する必要がある一時パスワードを割り当てます。
5. [すべてのイベントを無視する] をクリックして、ユーザーのリスクスコアをリセットします。

ユーザーはサインインしてパスワードをリセットし、アプリケーションにアクセスできるようになりました。

## <a name="known-issues"></a>既知の問題

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA が有効になっている場合、パートナーは、Exchange Online PowerShell で委任された管理者特権を利用して、顧客に対してアクションを実行することはできません。 この制限事項の詳細については[、「multi-factor authentication を使用した Exchange Online PowerShell への接続](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)」を参照してください。

## <a name="resources-and-support"></a>リソースとサポート

[パートナーセンターのセキュリティガイダンスグループコミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)では、その他のリソースを検索し、技術部の営業時間などの今後のイベントについて学習することができます。 要件の詳細については、[よく寄せられる質問](http://assetsprod.microsoft.com/security-requirements-faq.pdf)のドキュメントを参照してください。
