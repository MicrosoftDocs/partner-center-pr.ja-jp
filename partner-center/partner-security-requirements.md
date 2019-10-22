---
title: パートナーのセキュリティ要件 | パートナー センター
ms.topic: article
ms.date: 09/25/2019
description: クラウド ソリューション プロバイダー プログラムに参加するアドバイザーとパートナーのセキュリティ要件について説明します。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.openlocfilehash: ea155cf760850def85146d8c4e7e847fab5d7213
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318487"
---
# <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

**適用対象**

- クラウド ソリューション プロバイダー プログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロール パネル ベンダー
- すべてのアドバイザー

プライバシーの保護とセキュリティの強化は、マイクロソフトの最優先事項の 1 つです。 最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。 だから、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。 パートナーと顧客を保護するために、マイクロソフトは、アドバイザー、コントロール パネル ベンダー、およびクラウド ソリューション プロバイダー プログラムに参加しているパートナーを対象とした一連の必須セキュリティ要件を導入しています。

2019 年 8 月 1 日以降、すべてのパートナーが、パートナー テナントのすべてのユーザー (サービス アカウントを含む) に対して多要素認証を適用する必要があります。

> [!NOTE]
> ソブリン クラウド (21Vianet、米国政府、およびドイツ) を介して取引するすべてのパートナーが直ちに行動し、これらの新しいセキュリティ要件を採用することを強くお勧めします。 ただし、これらのパートナーは、2019 年 8 月 1 日に開始される新しいセキュリティ要件を満たす必要はありません。 マイクロソフトでは、今後、ソブリン クラウドに対するこれらのセキュリティ要件の適用に関して、追加の詳細情報を提供する予定です。

パートナーのセキュリティ要件に関連する条件は、[クラウド ソリューション プロバイダー プログラム ガイド](https://go.microsoft.com/fwlink/p/?LinkId=617100)に追加されています。 2019 年 8 月 1 日以降、クラウド ソリューション プロバイダー プログラムに参加しているすべてのパートナーが、条件を満たす必要があります。 アドバイザーについても、同じ契約条件が適用されます。

これらの要件が適用されると、必須のセキュリティ要件を実装していないパートナーは、クラウド ソリューション プロバイダー プログラムで取引したり、代理管理者権限を利用して顧客テナントを管理したりできなくなります。 現在、要件の技術的な適用開始日を設定しています。日付と詳細情報については、追ってパートナーに通知します。

## <a name="what-actions-do-i-need-to-take"></a>どのようなアクションが必要ですか。

パートナーには高い特権が付与されている、という点を考えると、すべての単一認証について、MFA チャレンジが各ユーザーに確実に適用されるようにする必要があります。 これは、次のいずれかの方法で実現できます

- Azure AD Premium を実装し、MFA が各ユーザーに確実に適用されるようにする
- [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を実装する
- サードパーティ ソリューションを実装し、MFA が各ユーザーに確実に適用されるようにする

> [!IMPORTANT]
> これらの要件が技術的に適用されると、すべての単一認証に MFA チャレンジが必要になります。 マイクロソフトの商用クラウド サービスにアクセスするときは、MFA を使用した認証を回避する目的で、条件付きアクセスの機能を使用することはできません。

### <a name="considerations"></a>考慮事項

これらの要件はパートナー テナントのすべてのユーザー (サービス アカウントを含む) に適用されるため、円滑なデプロイを実現するために考慮しなければならない点がいくつかあります。 これらの考慮事項には、MFA を実行できない Azure AD の特定、および先進認証に対応していない組織で使用されているアプリケーションとデバイスの特定が含まれます。

操作を実行する前に、次の点について確認することをお勧めします

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>認証時に MFA に対応していないアプリケーションまたはデバイスはありますか。

IMAP、POP3、SMTP などのプロトコルを使用する以前の MFA 認証を適用している場合はブロックされます。これらのプロトコルでは MFA がサポートされていないためです。 この制限に対処するには、[アプリ パスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)と呼ばれる機能を使用します。これにより、アプリケーションまたはデバイスを引き続き認証することができます。 [こちら](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリ パスワード使用時の考慮事項を確認し、お使いの環境でアプリ パスワードを使用できるかどうかを確かめる必要があります。

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>パートナー テナントに関連付けられたライセンスによって提供される Office 365 を使用しているユーザーがいますか。

ソリューションを実装する前に、Microsoft Office のバージョンが、なぜパートナー テナントのユーザーによって使用されているのかを確認することをお勧めします。 アクションを実行する前に、[Office 365 デプロイの多要素認証の計画](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)に関するトピックをご覧ください。 Outlook などのアプリケーションで接続の問題が発生する可能性があります。 MFA を適用する前に、Outlook 2013 SP1 以降が使用され、組織で先進認証が有効になっているかどうかを確認することが重要です。 詳細については、「[Exchange Online で先進認証を有効にする](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)」を参照してください。

Windows が実行され、Microsoft Office 2013 がインストールされているデバイスで先進認証を有効にするには、2 つのレジストリ キーを作成する必要があります。 「[Windows デバイスで Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。

> [!IMPORTANT]
> Azure AD MFA に対してユーザーを有効にした場合、先進認証に対して有効になっていない Office 2013 が実行されているデバイスがあるときは、それらのデバイスでアプリ パスワードを使用する必要があります。 アプリ パスワードと、そのパスワードをいつ/どこで/どのように使用するかの詳細については、[Azure Multi-Factor Authentication でのアプリ パスワード](https://go.microsoft.com/fwlink/p/?LinkId=528178)に関するページをご覧ください。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>作業中にユーザーによるモバイル デバイスの使用を禁止するポリシーがありますか。

実装する MFA ソリューションは、作業中に従業員がモバイル デバイスを使用できないようにする会社のポリシーの影響を受けるため、そのポリシーを特定することが重要です。 [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の実装を通じて提供される MFA ソリューションなど、確認の目的でのみ認証アプリの使用を許可する MFA ソリューションがあります。 モバイル デバイスの使用を禁止するポリシーが組織で採用されている場合は、次のいずれかのオプションを検討する必要があります

- セキュリティで保護されたシステムで実行できる、時間ベースのワンタイム ベース パスワード (TOTP) アプリケーションをデプロイする
- 最適な検証オプションを提供するパートナー テナントのユーザーごとに、MFA を適用するサード パーティのソリューションを実装する
- 影響を受けるユーザーに対して [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) ライセンスを購入する

FIDO セキュリティ キーの使用は、ベースライン保護ポリシーのロード マップに従ってサポートされる予定です。 サポートが追加されると、認証の 2 番目の要素に FIDO セキュリティ キーを利用できるようになります。 それまでは認証アプリの使用に限られます。

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>どの自動化または統合で、認証にユーザー資格情報が使用されていますか。

パートナー ディレクトリの各ユーザー (サービス アカウントを含む) に MFA を適用する必要があるため、認証にユーザー資格情報が使用されているすべての自動化または統合が影響を受けます。 このため、これらの状況で使用されているアカウントを特定することが重要です。 考慮する必要があるアプリケーションまたはサービスの例をいくつか次に示します

- 顧客に代わってリソースをプロビジョニングするときに使用されるコントロール パネル
- 顧客への請求 (CSP プログラムに関連する場合) および顧客サポートに使用される任意のプラットフォームとの統合
- Az、AzureRM、Azure AD、MS Online などのモジュールが利用される PowerShell スクリプト

上記のリストはすべてを網羅しているわけではありません。 そのため、認証にユーザー資格情報が利用されるご自身の環境で、アプリケーションまたはサービスの完全な評価を実行することが重要です。 MFA の要件に対応するには、可能な限り、[セキュリティで保護されたアプリケーション モデル フレームワーク](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)でガイダンスを実装する必要があります。 セキュリティで保護されたアプリケーション モデル フレームワークの実装方法を理解するのに役立つ追加のリソースを次に示します

- [パートナー センターの .NET サンプル](https://github.com/microsoft/partner-center-dotnet-samples): この GitHub リポジトリには、セキュリティで保護されたアプリケーション モデル フレームワークを実装する方法を示す、.NET を使用して開発されたサンプルが含まれています。
- [パートナー センターの Java サンプル](https://github.com/microsoft/partner-center-java-samples): この GitHub リポジトリには、セキュリティで保護されたアプリケーション モデル フレームワークを実装する方法を示す、Java を使用して開発されたサンプルが含まれています。
- [パートナー センターの PowerShell - セキュリティで保護されたアプリケーション モデル](https://docs.microsoft.com/powershell/partnercenter/secure-app-model): この記事では、セキュリティで保護されたアプリケーション モデル フレームワークを、PowerShell を使用して実装する方法を詳しく説明しています。
- [パートナー センター セキュリティ ガイダンス グループコ ミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): 今後のイベントを確認できるオンライン コミュニティです。このコミュニティでは、不明点について質問することもできます。

### <a name="enforcing-mfa-for-all-users"></a>すべてのユーザーに MFA を適用する

このセクションでは、[ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を使用して、パートナー テナントの各ユーザー (サービス アカウントを含む) に MFA を適用する方法について説明します。 Azure AD Premium を使用する場合は、[こちら](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)に記載されている手順に従ってください。

> [!NOTE]
> Azure AD と互換性のあるサードパーティ ソリューションを使用すると、すべてのユーザー (サービス アカウントを含む) に MFA を適用できます。 ソリューションの実装方法の詳細については、ベンダーのドキュメントを参照してください。

ベースライン保護ポリシーは、一般的な数々の攻撃から組織を保護するうえで役立つ定義済みポリシー セットです。 これらの一般的な攻撃には、パスワードのスプレー、リプレイ、フィッシングなどがあります。 ベースライン保護ポリシーは、Azure Active Directory のすべてのエディションで使用できます。 マイクロソフトでは、お客様とパートナーがクラス最高のセキュリティ プラクティスを実装できるように、これらのベースライン保護ポリシーをすべてのユーザーに提供しています。

次の表では、有効にする必要がある 2 つのベースライン保護ポリシーについて説明します。

|**ポリシー**| |
|-----|-----|
|**管理者に MFA を要求する**|"管理者に MFA を要求する" ポリシーを有効にすると、管理者ロールのユーザーが、認証アプリを使用して MFA に登録する必要があります。 MFA の登録が完了したら、管理者はサインインするたびに MFA を実行する必要があります。|
|**エンド ユーザーの保護**|エンド ユーザーの保護は、ディレクトリ内のすべてのユーザーを保護する、リスクベースの MFA ベースライン保護ポリシーです。 このポリシーを有効にすると、すべてのユーザーが認証アプリを使用して MFA に登録する必要があります。 この MFA 登録プロンプトは 14 日間無視できますが、この期間を過ぎると、MFA に登録するまで、そのユーザーのサインインはブロックされます。 MFA に登録されると、ユーザーは危険なサインインの試行中にのみ MFA が求められます。 危害を受けたユーザー アカウントについては、パスワードをリセットし、リスク イベントを無視するまでブロックされます。|

これらのポリシーを有効にすると、各ユーザーが認証アプリを使用して Azure MFA を利用し、追加コストなしで認証を行うことができます。

#### <a name="configure-self-service-password-reset"></a>セルフ サービスのパスワード リセットを構成する

セルフサービスのパスワード リセット (SSPR) は Azure Active Directory の機能で、ユーザーがサポート チームに連絡しなくてもパスワードをリセットできるようにします。 このサービスを使用するには、ユーザーが事前にセルフサービスのパスワード リセットを登録するか、または登録済みである必要があります。 登録時に、ユーザーは、組織が有効にした 1 つ以上の認証方法を選択します。

[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)ベースライン保護ポリシーが有効になっている場合、危害を受けたユーザー アカウントについては、パスワードをリセットし、リスク イベントを無視するまでブロックされます。 このため、全体管理者は各自で次の手順を実行して、自身がロックアウトされないように SSPR に登録することをお勧めします。

1. [SSPR セットアップ ページ](https://aka.ms/ssprsetup)に移動します
2. ユーザー名とパスワードを入力します
3. パスワードをリセットするときのユーザー確認に使用される検証オプションのうち、少なくとも 1 つを構成します。  

アカウントが危害を受けた場合、管理者は、影響を受けたユーザーのアクセスを復元するアクションを実行する必要があります。 ユーザーのブロックを解除するプロセスの詳細については、「[ユーザーのブロックを解除する手順](#recovering-compromised-accounts)」を参照してください。

#### <a name="require-mfa-for-admins"></a>管理者に MFA を要求する

"*管理者に MFA を要求する*" ベースライン ポリシーでは、最も特権の高い Azure Active Directory ロールと見なされる次のディレクトリ ロール に MFAが 必要です。

- 全体管理者
- SharePoint 管理者
- Exchange 管理者
- 条件付きアクセス管理者
- セキュリティ管理者
- ヘルプデスク管理者/パスワード管理者
- 課金管理者
- ユーザー管理者

"管理者に MFA を要求する" ポリシーを有効にするときに、上記の 9 つの管理者ロールは、認証アプリを使用して MFA に登録する必要があります。 MFA の登録が完了したら、管理者はサインインするたびに MFA を実行する必要があります。

ご自身の組織にこれらのアカウントがあり、スクリプトまたはコードで使用されている場合は、それを[マネージド ID](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview) に置き換えることを検討してください。

このポリシーを有効にして管理者を保護するには:

1. 全体管理者、セキュリティ管理者、または条件付きアクセス管理者として **Azure portal** にサインインします。
2. **[Azure Active Directory]**  >  **[条件付きアクセス]** に移動します。
3. ポリシーの一覧で、 **[ベースライン ポリシー: 管理者に MFA を要求する]** を選択します。
4. **[ポリシーを有効にする]** を **[ポリシーをすぐに有効にする]** に設定します。
5. **[保存]** をクリックします。

> [!WARNING]
> このポリシーを有効にする前に、ユーザーが以前の認証プロトコルを使用していないことを確認してください。 このポリシーを実装すると、以前の認証はブロックされます。

> [!IMPORTANT]
> 代理管理者権限を使用して Exchange Online PowerShell に接続する機能に影響する既知の問題があります。 この PowerShell モジュールを使用している場合は、このポリシーを有効にする前に、[Exchange Online PowerShell](#exchange-online-powershell) の既知の問題を参照してください。

#### <a name="end-user-protection"></a>エンド ユーザーの保護

エンド ユーザー保護ベースライン ポリシーでは、ディレクトリ内のすべてのユーザーが保護されます。 このポリシーを有効にすると、すべてのユーザーが 14 日以内に Azure MFA に登録する必要があります。 登録されると、ユーザーは危険なサインインの試行中にのみ MFA が求められます。 危害を受けたユーザー アカウントについては、パスワードをリセットし、リスクを無視するまでブロックされます。

**[ベースラインポリシー: エンド ユーザーの保護]** ポリシーは事前に構成されており、Azure portal で [条件付きアクセス] ブレードに移動すると上部に表示されます。

このポリシーを有効にしてユーザーを保護するには:

1. 全体管理者、セキュリティ管理者、または条件付きアクセス管理者として **Azure portal** にサインインします。
2. **[Azure Active Directory]**  >  **[条件付きアクセス]** に移動します。
3. ポリシーの一覧で、 **[ベースライン ポリシー: エンド ユーザーの保護 (プレビュー)]** を選択します。
4. **[ポリシーを有効にする]** を **[ポリシーをすぐに有効にする]** に設定します。
5. **[保存]** をクリックします。

> [!WARNING]
> このポリシーを有効にする前に、ユーザーが以前の認証プロトコルを使用していないことを確認してください。 このポリシーを実装すると、以前の認証はブロックされます。

> [!IMPORTANT]
> 代理管理者権限を使用して Exchange Online PowerShell に接続する機能に影響する既知の問題があります。 この PowerShell モジュールを使用している場合は、このポリシーを有効にする前に、[Exchange Online PowerShell](#exchange-online-powershell) の既知の問題を参照してください。

## <a name="assessing-your-environment"></a>環境を評価する

現在のパートナー セキュリティ要件の 1 つを通じて、パートナー テナントの各ユーザーに MFA を適用する必要があります。 この要件にはさまざまな方法で対応できるため、追加のアクションが必要かどうかを評価することが困難な場合があります。 MFA でテナントを保護するために追加のアクションが必要かどうかを評価するには、Azure Active Directory 監査ログや [Microsoft セキュア スコア](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score)などのツールを利用します。 マイクロソフトでは、MFA およびセキュリティで保護されたアプリケーション モデルの要件について迅速にコンプライアンス チェックを実行できるように、パートナー センターの操作性に取り組んでいます。

Microsoft セキュア スコアでは、堅牢な視覚化、他の Microsoft 製品との統合、他の企業とのスコアの比較、カテゴリによるフィルター処理などが可能です。 このツールを使用すると、組織内でセキュリティ強化アクションを実行し、スコアの履歴を追跡できます。 また、推奨される改善アクションにサード パーティ ソリューションで対処する場合も、スコアに反映されます。

![Microsoft セキュア スコア](images/security/secure-score.png)

> [!NOTE]
> Microsoft セキュア スコアを上げるアクションが反映されるには、最大 24 時間かかる場合があります。

Microsoft セキュア スコアは、ご自身のセキュリティ体制を数値で表現しているにすぎません。 MFA チャレンジなしで何が、または誰が認証しているかをよく理解するには、Azure Active Directory 監査ログに対してクエリを実行することをお勧めします。 これを行うには、[Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) モジュールと次のスクリプトを使用します。 これにより、MFA チャレンジが行われなかった過去 1 日の間に行われた認証試行の洞察を提供するレポートが生成されます。

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

上記のスクリプトを実行すると、report.csv ファイルで詳細情報を入手できます。 これには、ユーザーの MFA チャレンジが行われなかった過去 1 日の間に行われた認証試行の一覧が含まれます。 各エントリを確認して、それが予期された動作かどうかを判断し、必要に応じて対応します。

![評価レポート](images/security/assessment-report.png)

## <a name="common-issues"></a>一般的な問題

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

ベースライン ポリシーを有効にすると、自動化や統合で次のような例外が発生することがあります

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

この例外が発生する理由は、ユーザー資格情報を使用して認証しているため、MFA が必要になったからです。 この例外に対処するには、認証にアクセス トークンを使用する必要があります。 詳細については、[セキュリティで保護されたアプリケーション モデル ガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。

>[!IMPORTANT]
>最新の API と PowerShell モジュールでは、認証にアクセス トークンを利用できますが、 現時点でこの機能がサポートされていないモジュールもあります。 使用しようとしている API または PowerShell モジュールで、認証にアクセス トークンを使用できるかどうかを確認するためのサポートが必要な場合は、[パートナー センター セキュリティ ガイダンス グループ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) コミュニティでメッセージを投稿してください。

#### <a name="aadsts700082"></a>AADSTS700082

セキュリティで保護されたアプリケーション モデル フレームワークを実装すると、最初の更新トークンを生成してから 90 日後に次の例外が発生する可能性があります

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Azure Active Directory の場合、更新トークンの最長有効期間は 90 日です。 このエラーに対処するには、新しい更新トークンを生成し、安全に保存する必要があります。 更新トークンは、アクセス トークンが Azure Active Directory に要求されるたびに新しいものが返されるため、プログラムによって更新される可能性があることに注意してください。 適切なロジックを実装することで、安全に保存された更新トークンを、期限切れになる前に更新できます。

詳細については、「[Azure Active Directory における構成可能なトークンの有効期間](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。

### <a name="recovering-compromised-accounts"></a>危害を受けたアカウントを回復する

お客様を保護するために、マイクロソフトが提供するリークされた資格情報に関するサービスでは、公開されているユーザー名とパスワードのペアが検出されます。 そのいずれかが、マイクロソフト ユーザーのものと一致する場合、マイクロソフトでは、直ちにそのアカウントを保護します。 資格情報がリークされていると見なされたユーザーは、侵害ありと確認されたうえで、 パスワードがリセットされるまで、サインインがブロックされます。

Azure AD Premium ライセンスを割り当てられたユーザーは、自身のディレクトリでセルフサービスのパスワード リセット (SSPR) が有効になっていれば、その機能を使ってアクセスを復元できます。 Premium ライセンスを持たないユーザーがブロックされた場合、そのユーザーは管理者に連絡して、パスワードのリセットを手動で実行し、フラグ付きユーザー リスク イベントを無視する必要があります。

#### <a name="steps-to-unblock-a-user"></a>ユーザーのブロックを解除する手順

ユーザーのサインイン ログを調べて、ユーザーがポリシーによってブロックされていることを確認します。

1. 管理者が **Azure portal** にサインインし、 **[Azure Active Directory]**  >  **[ユーザー]** に移動したうえで、ユーザーの名前をクリックし、[サインイン] に移動する必要があります。
2. ブロックされたユーザーのパスワードのリセットを開始するには、管理者が **[Azure Active Directory]**  >  **[リスクのフラグ付きユーザー]** に移動する必要があります
3. アカウントがブロックされているユーザーをクリックして、ユーザーの最近のサインイン アクティビティに関する情報を表示します。
4. [パスワードのリセット] をクリックして、一時パスワードを割り当てます。このパスワードは、次のログイン時に変更する必要があります。
5. [すべてのイベントを無視する] をクリックして、ユーザーのリスク スコアをリセットします。

これによりユーザーがサインインし、パスワードをリセットして、アプリケーションにアクセスできるようになります。

## <a name="known-issues"></a>既知の問題

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

MFA が適用されると、パートナーが Exchange Online PowerShell で代理管理者権限を利用して、顧客に対してアクションを実行できなくなります。 この制限事項の詳細については、「[多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)」を参照してください。

この制限を回避するには、新しいアカウントを作成し、そのアカウントでは対話型認証を行わないようにします。 [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) を利用して新しいアカウントを作成し、初期構成を行うことをお勧めします。 次の PowerShell を使用すると、アカウントを作成し、構成することができます

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

次回 PowerShell を使用して Exchange Online に接続するときに、このアカウントを使用すると、期待どおりに動作します。

> [!IMPORTANT]
> MFA が適用されているときに、パートナーが Exchange Online PowerShell で代理管理者権限を利用して、顧客に対してアクションを実行する機能は、今後提供される予定です。 それまでは、この回避策をご利用ください。

## <a name="resources-and-support"></a>リソースとサポート

[パートナー センター セキュリティ ガイダンス グループ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) コミュニティでは、その他のリソースを検索し、技術部門の営業時間を含め、今後のイベントの情報を確認することができます。 要件の詳細については、[よく寄せられる質問](partner-security-requirements-faq.md)のドキュメントを参照してください。
