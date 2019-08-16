---
title: パートナーのセキュリティ要件に関する FAQ |パートナーセンター
ms.topic: article
ms.date: 07/18/2019
description: パートナーのセキュリティ要件についてよく寄せられる質問
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウドソリューションプロバイダー, Cloud Solution Provider プログラム, CSP, コントロールパネルベンダ, CPV, multi-factor authentication, MFA, 安全なアプリケーションモデル, セキュリティで保護されたアプリモデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820590"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>パートナーのセキュリティ要件についてよく寄せられる質問

この記事では、[パートナーのセキュリティ要件](partner-security-requirements.md)に関してよく寄せられる質問をいくつか紹介します。

## <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

### <a name="what-are-the-new-partner-security-requirements"></a>新しいパートナーのセキュリティ要件は何ですか。

パートナーと顧客を保護するために、パートナーは次のアクションをすぐに実行するように要求しています。  

1. **パートナーテナントのすべてのユーザーに対して多要素認証 (MFA) を有効に**します。 パートナーテナントのすべてのユーザーは、Microsoft 商用クラウドサービスにサインインするとき、またはパートナーセンターまたは Api 経由で CSP を使用するときに、多要素認証 (MFA) を使用する必要があります。 ベースライン保護ポリシーを有効にすることで、パートナーテナントのすべてのユーザーに対して MFA を無料で利用できます。

2. **セキュリティで保護されたアプリケーションモデルフレームワークを採用**します。 Azure Resource Manager、Microsoft Graph、パートナーセンター API などの Microsoft API と統合しているすべてのパートナーは、ベースラインポリシーが有効になっている場合、統合の中断を避けるために、セキュリティで保護されたアプリケーションモデルフレームワークを採用する必要があります。 
 
多要素認証 (MFA) を有効にし、セキュリティで保護されたアプリケーションモデルフレームワークを採用することで、インフラストラクチャを保護し、盗難やその他の不正行為インシデントの特定などの潜在的なセキュリティリスクから顧客のデータを保護することができます。  

### <a name="which-partners-need-to-meet-the-requirements"></a>どのパートナーが要件を満たす必要がありますか。

これらの要件は、次のパートナーグループを対象としています。
- クラウドソリューションプロバイダー (CSP) プログラムに参加しているすべてのパートナー組織が、Microsoft の商用クラウドサービスを使用して動作しています
  - 直接請求パートナー
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロールパネルベンダー
- すべての Advisor プログラムパートナー  

ソブリンクラウド (21Vianet、米国政府、ドイツ) を介して活動するすべてのパートナーは、8月1日よりも新しいセキュリティ要件を満たす必要はありません。 ただし、ソブリン cloud を使用しているすべてのパートナーが、これらの新しいセキュリティ要件をすぐに導入することを強くお勧めします。 Microsoft では、将来のソブリンクラウドに対するこれらのセキュリティ要件の適用に関する追加情報を提供します。

### <a name="what-are-the-key-timelines-and-milestones"></a>主要なタイムラインとマイルストーンは何ですか。

これらのセキュリティ要件に関連付けられている用語は、Cloud Solution Provider プログラムガイドにすぐに追加されます。 2019年8月1日より有効になる CSP プログラムへの参加に準拠するには、これらのセキュリティ要件を実装する必要があります。 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>操作を行わないとどうなりますか。

これらのセキュリティプラクティスと義務を遵守していないパートナーは、これらのパートナーのセキュリティ要件が適用された後、クラウドソリューションプロバイダープログラムでは、または代理管理者権限を利用して顧客のテナントを管理することはできません。 ここでは、要件の実施日を設定しています。パートナーには、その日の詳細情報が通知されます。

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>マイクロソフトがこれらの新しい要件を適用する理由
お客様とパートナーのセキュリティとプライバシーは、Microsoft の最優先事項です。 さらに洗練され、セキュリティ攻撃の数が増え続けています。主に id の侵害のインシデントに関連しています。 予防的な制御は、セキュリティ攻撃を阻止するために、全体的な防御戦略で重要な役割を果たすため、パートナーと顧客を保護するために、一連の必須のセキュリティ要件の適用を開始します。

### <a name="does-this-apply-to-all-geographies"></a>これはすべての地域に適用されますか。

はい、すべての地域に適用されます。 ソブリンクラウド (21Vianet、US Government、およびドイツ) を介して行動するすべてのパートナーが、これらの新しいセキュリティ要件をすぐに採用することを強くお勧めします。 ただし、このようなパートナーは、8月1日よりも新しいセキュリティ要件を満たす必要はありません。 Microsoft では、将来のソブリンクラウドに対するこれらのセキュリティ要件の適用に関する追加情報を提供します。

## <a name="required-actions"></a>必要な操作

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>要件を満たすために行う必要がある重要な操作は何ですか。  
CSP プログラム (直接請求書、間接プロバイダー、間接リセラー)、アドバイザー、およびコントロールパネルベンダーのすべてのパートナーが要件を満たしている必要があります。

1. **すべてのユーザーに MFA を適用する**

    CSP プログラム、アドバイザー、およびコントロールパネルベンダーのすべてのパートナーは、パートナーテナント内のすべてのユーザーに対して MFA を強制する必要があります。 これを実現するには、[[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)]、[[エンドユーザー保護ベースライン](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)]、およびそれ以降の基準ポリシーを有効にします。 ベースラインポリシーによって提供される機能は、パートナーと顧客が絶え間なく変化するセキュリティの脅威から保護されるように発展し続けます。 そのため、詳細については、[ベースラインポリシーのドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を確認することが重要です。

    - ベース[ラインポリシーを参照してください:管理者基準ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)に mfa を要求する方法の詳細については、管理者に mfa を要求します。
    - ベース[ラインポリシーを参照してください:エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースラインポリシーを有効にする方法の詳細については、「エンドユーザーによる保護」を確認してください。
    - [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の概念を理解します。

    その他の考慮事項:

    - 間接プロバイダーは間接リセラーと協力して、パートナーセンターにオンボードしていない場合はパートナーセンターにオンボードする必要があります。また、リセラーが要件を満たしていることを推奨します。
    - Azure MFA は、 [Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)を使用する唯一の認証方法を使用して、パートナーテナントのすべてのユーザーに対して、ベースラインポリシーを通じて無料で利用できるようになっています。
    - SMS や電子メールなどの他の方法が必要な場合は、 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) sku を通じて追加の検証方法を利用できます。
    - パートナーは、Microsoft の商用クラウドサービスにアクセスするときに、各ユーザーに対してサードパーティの MFA ソリューションを利用することもできます。

2. **セキュリティで保護されたアプリケーションモデルフレームワークを採用する**

    任意の Api (Azure Resource Manager、Microsoft Graph、パートナーセンター API など) を使用してカスタム統合を開発したパートナーや、PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーションモデルを採用する必要があります。](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft クラウドサービスと統合するためのフレームワーク。 この操作を行わないと、MFA の展開によって中断が発生する可能性があります。 次のリソースでは、モデルの導入方法に関する概要とガイダンスを提供しています。

    - [セキュリティで保護されたアプリケーションモデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [パートナーセンター:セキュリティで保護されたアプリケーションモデルのガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP プログラムのパートナー: セキュリティで保護されたアプリケーションモデルを有効にするための .NET サンプルコード](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [CSP プログラムのパートナー:セキュリティで保護されたアプリケーションモデルを有効にするための Java サンプルコード](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [パートナーセンターの認証ドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [パートナーセンターの PowerShell Multi-factor Authentication (MFA) ドキュメント](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    コントロールパネルを使用している場合は、セキュリティで保護されたアプリケーションモデルフレームワークの導入についてベンダーに相談する必要があります。

    コントロールパネルベンダは、コントロールパネルベンダーとしてパートナーセンターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始するために必要です。 [パートナーセンターを参照してください。セキュリティで保護さ](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)れたアプリケーションモデルフレームワーク。 コントロールパネルのベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

## <a name="multi-factor-authentication"></a>多要素認証

### <a name="what-is-mfa"></a>MFA とは

Multi-factor Authentication (MFA) は、複数の必要なセキュリティと検証の手順によって個人を認証するセキュリティメカニズムです。 これは、次の認証方法の2つ以上を要求することによって機能します。

- ユーザーが知っている情報 (一般にパスワード)
- ユーザーの所持品 (複製が困難な、携帯電話などの信頼されているデバイス)
- ユーザー自身の特性 (生体認証)

### <a name="what-are-baseline-protection-policies"></a>ベースライン保護ポリシーとは 

[Microsoft ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)(現在プレビュー) は、多くの一般的な攻撃から組織を保護するために定義された一連のポリシーです。 これらの一般的な攻撃には、パスワードのスプレー、リプレイ、フィッシングなどがあります。 ベースラインポリシーは、Azure Active Directory のすべてのエディションで使用できます。 Microsoft は、これらのベースライン保護ポリシーをすべてのユーザーが利用できるようにしています。これは、id ベースの攻撃が過去数年間にわたって増加しているためです。 これらのポリシーの目的は、すべての組織で追加コストなしでセキュリティのベースラインレベルを有効にすることです。

> [!NOTE]
> Microsoft のベースラインポリシーと関連する機能は、絶え間なく変化するセキュリティの脅威からパートナーと顧客をより適切に保護するために進化し続けています。 基準ポリシーでは、名前付けと分類の変更が間もなく発生する場合があります。 最新の情報を確認するには、ベースラインポリシーのページに直接アクセスすることを強くお勧めします。

### <a name="what-baseline-policies-must-i-enable"></a>有効にする必要がある基準ポリシーを教えてください。

現在のベースライン保護ポリシーを使用して、パートナーテナントの各ユーザーに MFA を提供する予定の場合は、[[管理者](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースラインポリシーに mfa を要求する] を有効にする必要があります。 これらのベースライン保護ポリシーは、モバイルデバイス経由で Microsoft Authenticator アプリを使用しているパートナーに対してのみ、パートナーテナントの各ユーザーに対する MFA の要件を満たします。

管理[者ベースラインポリシーの [MFA が必要](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)] は、パートナーディレクトリの管理ユーザーに利用されます。[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)基準ポリシーは、パートナーテナントの管理者以外のユーザーを保護するために利用されます。 これらのポリシーを有効にすると、ユーザーは MFA に登録する必要があります。 ユーザーが正常に登録されると、ポリシーの条件に基づいてサインインを試行したときに MFA が要求されます。 ベースラインポリシーによって提供される機能は、パートナーと顧客が絶え間なく変化するセキュリティの脅威から保護されるように発展し続けます。 そのため、詳細については、[ベースラインポリシーのドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を確認することが重要です。

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>[管理者に MFA を要求する] ポリシーを有効に操作方法ますか? 

Microsoft Azure 管理ポータルを使用して、管理者ベースラインポリシーの MFA が必要です。 ベース[ラインポリシーを参照してください:この基準ポリシーを](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)有効にする方法の詳細については、管理者に MFA が必要です。

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>エンドユーザー保護ポリシー操作方法有効にしますか?

エンドユーザー保護のベースラインポリシーは、Microsoft Azure 管理ポータルから有効にすることができます。 ベース[ラインポリシーを参照してください:この基準ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)を有効にする方法の詳細については、「エンドユーザーによる保護」を確認してください。

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>ベースラインポリシーは自動的に有効になりますか。 

いいえ。これらのポリシーを有効にするには、グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者の役割のメンバーであるユーザーがポリシーを直ちに使用するように構成する必要があります。

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA を有効にするにはどのようなコストがかかりますか。

Microsoft では、管理者と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシー[に mfa を要求](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)することによって、mfa を無料で提供しています。 このバージョンの MFA で利用できる検証オプションは、 [Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)だけです。 通話または SMS メッセージが必要な場合は、 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)ライセンスを購入する必要があります。 または、サードパーティのソリューションを利用して、パートナーテナントの各ユーザーに MFA を提供することもできます。この場合は、MFA ソリューションが強制的に適用され、準拠していることを確認する必要があります。

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>既に MFA ソリューションがある場合、どのようなアクションを実行する必要がありますか。

これらのセキュリティ要件を通じて、パートナーテナントのユーザーは、Microsoft の商用クラウドサービスにアクセスするときに MFA を使用して認証する必要があります。 サードパーティのソリューションを使用して、これらの要件を満たすことができます。 Microsoft では、Azure Active Directory との互換性のために、独立した id プロバイダーに検証テストを提供しなくなりました。 製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>MFA を認証するためにどのような検証方法を使用できますか。

Microsoft では、管理者と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシー[に mfa を要求](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)することによって、mfa を無料で提供しています。 このバージョンの MFA で利用できる検証オプションは、 [Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)だけです。 通話または SMS メッセージが必要な場合は、 [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium)ライセンスを購入する必要があります。 または、サードパーティのソリューションを利用して、パートナーテナントの各ユーザーに MFA を提供することもできます。この場合は、MFA ソリューションが強制的に適用され、準拠していることを確認する必要があります。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>複数のパートナーテナントを使用して、 これらすべてに MFA を実装する必要はありますか。

はい。 CSP プログラムまたは Advisor プログラムに関連付けられている Azure Active Directory テナントごとに MFA を適用する必要があります。 Azure Active Directory Premium ライセンスの購入を計画している場合は、各 Azure Active Directory テナントのユーザーに対してライセンスを購入する必要があります。

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>パートナーテナントの各ユーザーが MFA を適用する必要がありますか。 

[[管理者](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシーに mfa が必要] は、パートナーテナントの各ユーザーに対して mfa を強制します。 これらのポリシーを利用して MFA を提供し、 [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)アプリケーションを使用している場合は、追加のライセンスを購入する必要はありません。 それ以外の場合は、パートナーテナントの各ユーザーに MFA を提供するための適切なソリューションを購入する必要があります。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft との直接請求パートナーです。 何を行う必要がありますか。

ダイレクト請求のクラウドソリューションプロバイダーパートナーは、パートナーテナント内のユーザーごとに MFA を適用する必要があります。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>私は間接リセラーであり、ディストリビューターだけを transact としています。 この操作を行う必要はありますか。

パートナーテナントの各ユーザーに対して MFA を強制するには、すべての間接リセラーが必要です。 これは、間接リセラーが実行する必要のあるアクションです。

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>パートナーセンター API を使用していません。 MFA を実装する必要はありますか。

はい。このセキュリティ要件は、パートナーテナントのパートナー管理者ユーザーとエンドユーザーを含むすべてのユーザーを対象としています。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Azure Active Directory と互換性のある MFA ソリューションを提供するサードパーティベンダーはどれですか。

[Gartner](https://www.gartner.com/en/webinars/3881781)社など、オンラインでの MFA ソリューションの多くの独立したレビューがあります。 MFA のベンダーとソリューションを確認する場合、パートナーは、選択したソリューションが Azure Active Directory と互換性があることを確認する必要があります。

Microsoft では、Azure Active Directory との互換性のために、独立した id プロバイダーに検証テストを提供しなくなりました。 製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

詳細については、「 [Azure AD のフェデレーション互換性リスト](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)」を参照してください。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>統合サンドボックスで MFA をテストするにはどうすればよいですか。

統合サンドボックステナントでは、[[管理者](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)と[エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースラインポリシーに MFA が必要] が有効になっている必要があります。 このポリシーでは、テナントの各ユーザーが MFA を使用して認証する必要があります。

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>MFA によって顧客のテナントと対話する方法を有効にしますか。 

No. これらのセキュリティ要件の履行は、顧客の管理方法には影響しません。 委任された管理操作を実行する機能は中断されません。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>お客様はパートナーのセキュリティ要件の対象ですか?

いいえ。お客様の Azure AD テナントの各ユーザーに対して MFA を強制する必要はありません。 ただし、各顧客を操作して、ユーザーの保護に最適な方法を決定することをお勧めします。

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>アプリパスワードは、ベースライン保護ポリシーと共に使用できますか。

はい。[アプリパスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)を使用できます。 [ここ](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリパスワードを使用する際の考慮事項を確認し、ニーズに応じてサポートされているかどうかを判断する必要があります。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>どのユーザーでもこの要件を除外することはできますか。 

いいえ。パートナーテナントの各ユーザー (サービスアカウントを含む) は、MFA を使用した認証を要求されます。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>パートナーのセキュリティ要件は統合サンドボックスに適用されますか。

はい、パートナーのセキュリティ要件は統合サンドボックスに適用されます。 これは、統合サンドボックステナントのユーザーに適切な MFA ソリューションを実装する必要があることを意味します。 MFA を提供するには、ベースライン保護ポリシーを実装することをお勧めします。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>緊急アクセス (休憩) アカウントを構成操作方法には

Azure AD テナントから誤ってロックアウトされるのを防ぐために、1つまたは2つの緊急アクセスアカウントを作成することをお勧めします。 パートナーのセキュリティ要件に関しては、各ユーザーが MFA を使用して認証する必要があります。 したがって、これは緊急アクセスアカウントの定義を変更する必要があることを意味します。 MFA のためのサードパーティソリューションを利用しているアカウントを使用することもできます。

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>ゲストユーザーは、パートナーのセキュリティ要件によってどのような影響を受けますか。

パートナーテナント内のリソースにアクセスするときは、ゲストユーザーが MFA を使用して認証する必要があります。 パートナーのセキュリティ要件は、ゲストユーザーが独自のテナントのリソースにアクセスすることには影響しません。

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>サードパーティのソリューションを使用している場合は Active Directory フェデレーションサービス (ADFS) が必要ですか? 

いいえ、サードパーティのソリューションを使用している場合は、Active Directory フェデレーションサービス (ADFS) を用意する必要はありません。 ソリューションのベンダーと協力して、ソリューションの要件を決定することをお勧めします。

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>ベースライン保護ポリシーを有効にする必要がありますか。

いいえ。ベースライン保護ポリシーを有効にする必要はありません。 唯一の要件は、パートナーテナント内のユーザー (サービスアカウントを含む) ごとに MFA を適用することです。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA の要件を満たすために条件付きアクセスを使用できますか。

はい。条件付きアクセスを使用して、パートナーテナントの各ユーザー (サービスアカウントを含む) に MFA を適用できます。 ただし、パートナーになるという高度な特権がある場合は、各ユーザーが単一の認証ごとに MFA チャレンジを使用できるようにする必要があります。 これは、MFA の要件を回避する条件付きアクセスの機能を利用できないことを意味します。

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>ベースライン保護ポリシーの実装により、どのような検証オプションが提供されますか。 

ベースライン保護ポリシーの実装によって利用可能な MFA のバージョンに関して、使用可能な認証オプションは authenticator アプリだけです。 通話とテキストメッセージメッセージの使用は、安全性が低いと見なされます。 そのため、これらのオプションは、このバージョンの MFA では使用できません。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件の影響を受けますか。

いいえ。 Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件による影響を受けません。 MFA を適用した結果として Azure AD Connect の問題が発生した場合は、Microsoft サポートに問い合わせてテクニカルサポートを依頼してください。

## <a name="secure-application-model"></a>セキュリティで保護されたアプリケーションモデル

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>要件を満たすために、セキュリティで保護されたアプリケーションモデルを採用する必要がありますか。

Microsoft では、クラウドソリューションプロバイダー (CSP) パートナーおよび Multi-factor Authentication を活用するコントロールパネルベンダー (CPV) を認証するための、セキュリティで保護されたスケーラブルなフレームワークを導入しています。 詳細については、「[セキュリティで保護されたアプリケーションモデル」ガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。 任意の Api (Azure Resource Manager、Microsoft Graph、パートナーセンター API など) を使用してカスタム統合を開発したパートナーや、PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーションモデルを採用する必要があります。](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft クラウドサービスと統合するためのフレームワーク。

### <a name="what-is-the-secure-application-model"></a>セキュリティで保護されたアプリケーションモデルとは

Microsoft では、クラウドソリューションプロバイダー (CSP) パートナーおよび Multi-factor Authentication を活用するコントロールパネルベンダー (CPV) を認証するための、セキュリティで保護されたスケーラブルなフレームワークを導入しています。 詳細については、「[セキュリティで保護されたアプリケーションモデル」ガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。  

### <a name="how-do-i-implement-the-secure-application-model"></a>セキュリティで保護されたアプリケーションモデルを実装操作方法には

任意の Api (Azure Resource Manager、Microsoft Graph、パートナーセンター API など) を使用してカスタム統合を開発したパートナーや、PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーションモデルを採用する必要があります。](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)Microsoft クラウドサービスと統合するためのフレームワーク。 この操作を行わないと、MFA の展開によって中断が発生する可能性があります。 次のリソースでは、モデルの導入方法に関する概要とガイダンスを提供しています。

- [セキュリティで保護されたアプリケーションモデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [パートナーセンター:セキュリティで保護されたアプリケーションモデルのガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP プログラムのパートナー: セキュリティで保護されたアプリケーションモデルを有効にするための .NET サンプルコード](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP プログラムのパートナー:セキュリティで保護されたアプリケーションモデルを有効にするための Java サンプルコード](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [パートナーセンターの認証ドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [パートナーセンターの PowerShell Multi-factor Authentication (MFA) ドキュメント](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

コントロールパネルを使用している場合は、セキュリティで保護されたアプリケーションモデルフレームワークの導入についてベンダーに相談する必要があります。

コントロールパネルベンダは、コントロールパネルベンダーとしてパートナーセンターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始するために必要です。 [パートナーセンターを参照してください。セキュリティで保護さ](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)れたアプリケーションモデルフレームワーク。 コントロールパネルのベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

### <a name="who-is-a-control-panel-vendor-cpv"></a>誰がコントロールパネルベンダー (CPV) であるか。 
コントロールパネルのベンダは、CSP パートナーがパートナーセンター Api と統合するために使用するアプリを開発する独立系ソフトウェアベンダーです。 コントロールパネルのベンダは、パートナーセンターのダッシュボードまたは Api に直接アクセスできる CSP パートナーではありません。 詳細な説明は、 [パートナーセンター内で利用できます。セキュリティで保護さ](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)れたアプリケーションモデルガイド。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>セキュリティで保護されたアプリケーションモデルは、パートナーセンターの API/SDK に対してのみ実装する必要がありますか。 

[*管理者に MFA を要求*する] と [*エンドユーザー保護*のベースラインポリシー] の両方を有効にすると、各ユーザーは multi-factor Authentication を使用して認証する必要があります。 つまり、非対話形式で実行するための API、CLI、および PowerShell モジュール (Azure、Azure AD、MS Online、パートナーセンターなど) に対して、セキュリティで保護されたアプリケーションモデルを実装する必要があります。これは、認証にユーザーの資格情報を使用することを意図しています。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell などの自動化ツールを使用しています。 セキュリティで保護されたアプリケーションモデルを実装操作方法には  

オートメーションが非対話形式で実行され、認証にユーザー資格情報を使用することを想定している場合は、セキュリティで保護されたアプリケーションモデルを実装する必要があります。 「[セキュリティで保護されたアプリケーションモデル」をご覧ください。](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5)このフレームワークを実装する方法については、パートナーセンターの PowerShell に関するガイダンスをご覧ください。  ただし、すべてのオートメーションツールがアクセストークンを使用して認証する機能を提供するわけではありません。 どのような変更が必要であるかを理解するために支援が必要な場合は、[パートナーセンターのセキュリティガイダンス](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)グループにメッセージを投稿してください。

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>同意プロセスを実行するときにアプリケーション管理者が提供する必要があるユーザー資格情報 

最小限の特権のアクセス許可が割り当てられているサービスアカウントを使用することをお勧めします。 パートナーセンター API に関しては、営業担当者ロールまたは管理エージェントロールが割り当てられているアカウントを使用する必要があります。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>同意プロセスを実行するときに、アプリケーション管理者がグローバル管理者のユーザー資格情報を提供しないのはなぜですか。

最小限の特権を使用して、リスクを軽減することをお勧めします。 グローバル管理者特権を持つアカウントを使用することは推奨されません。これは、必要な権限よりも多くのアクセス許可を提供するためです。

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>私は CSP パートナーです。 コントロールパネルベンダ (CPV) がソリューションの実装に従事しているかどうかを操作方法確認してください。 

Control Panel ベンダ (CPV) ソリューションを使用してクラウドソリューションプロバイダー (CSP) プログラムを提供するパートナーには、お客様の CPV を参照する必要があります。 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>私は CPV です。 登録操作方法ますか? 

コントロールパネルベンダ (CPV) として登録するには、[こちら](https://docs.microsoft.com/partner-center/enroll-as-cpv)のガイドラインに従ってください。

登録リンクを受け取るには、cpvs が、cpvs とのビジネス関係を持つか、またはビジネスを認識している Microsoft 従業員スポンサーに連絡[CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com)して提供する必要があります。 たとえば、パートナー開発マネージャー (PDM) などです。

パートナーセンターに登録してアプリケーションを登録すると、パートナーセンターの Api にアクセスできるようになります。 新しい CPV の場合は、パートナーセンターの通知を通じてサンドボックスの情報を受け取ります。 Microsoft CPV として登録を完了し、CPV 契約に同意すると、次のことができます。

1. マルチテナントアプリケーションを管理します (アプリケーションを Azure portal に追加し、パートナーセンターでアプリケーションを登録または登録解除します)。 注:CPVs は、パートナーセンターの Api に対して承認を受けるには、パートナーセンターにアプリケーションを登録する必要があります。 Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。
2. CPV プロファイルを表示して管理します。
3. CPV 機能にアクセスする必要があるユーザーを表示および管理する。 CPV が持つことができる唯一のロールはグローバル管理者です。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>パートナーセンター SDK を使用しています。 SDK は自動的にセキュリティで保護されたアプリケーションモデルを採用しますか。 

いいえ。[セキュリティで保護](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)されたアプリケーションモデルのガイドに記載されているガイドラインに従う必要があります。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>MFA が有効になっていないアカウントを使用して、セキュリティで保護されたアプリケーションモデルの更新トークンを生成できますか。

はい。更新トークンは、MFA が適用されていないアカウントを使用して生成できます。 ただし、mfa が有効になっていないアカウントを使用して生成されたトークンは、MFA の要件により、リソースにアクセスできないため、この操作は行わないでください。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA を有効にした場合、アプリケーションがアクセストークンを取得する方法

新しいセキュリティ要件に準拠しながら、その方法の詳細については、「[セキュリティで保護されたアプリケーションモデル」ガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)に従う必要があります。 [ここ](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)では .NET サンプルコード、[ここ](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)では Java サンプルコードを紹介します。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV として、CPV テナントまたは CSP パートナーのテナントに Azure AD アプリケーションを作成しますか。

CPV では、その登録に関連付けられているテナントの Azure Active Directory アプリケーションを CPV として作成する必要があります。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>私はアプリのみの認証を使用している CSP です。 変更を加える必要がありますか。

ユーザーの資格情報がアクセストークンを要求するために使用されていないため、アプリのみの認証は影響を受けません。 ユーザーの資格情報が共有されている場合、コントロールパネルのベンダー (CPVs) は、[セキュリティで保護されたアプリケーションモデルフレームワーク](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)を採用し、所有している既存のパートナー資格情報を消去する必要があります。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV では、アプリのみの認証スタイルを利用してアクセストークンを取得できますか。

いいえ。コントロールパネルのベンダーパートナーは、パートナーの代わりにアクセストークンを要求するために、アプリのみの認証スタイルを利用することはできません。 アプリとユーザーの認証スタイルを利用する、セキュリティで保護されたアプリケーションモデルを実装する必要があります。

## <a name="key-resources"></a>主要リソース

### <a name="how-to-get-started"></a>開始する方法

- [パートナーのセキュリティ要件: ステップバイステップガイド](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- この[パートナーセンターセキュリティガイダンスグループ](https://aka.ms/MPCSecurityGuidance)に質問とフィードバックをお送りください。
- 今後のパートナーオフィスの営業時間とウェビナーにご参加ください。 [詳細なスケジュールとリソースをこちらで](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)確認してください。

### <a name="resources-for-enabling-mfa"></a>MFA を有効にするためのリソース

- [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の概念を理解します。
- ベース[ラインポリシーを参照してください:管理者基準ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)に mfa を要求する方法の詳細については、管理者に mfa を要求します。
- ベース[ラインポリシーを参照してください:エンドユーザー保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースラインポリシーを有効にする方法の詳細については、「エンドユーザーによる保護」を確認してください。

### <a name="resources-for-adopting-secure-application-model"></a>セキュリティで保護されたアプリケーションモデルを採用するためのリソース

- [セキュリティで保護されたアプリケーションモデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [パートナーセンター:セキュリティで保護されたアプリケーションモデルのガイド](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP プログラムのパートナー: セキュリティで保護されたアプリケーションモデルを有効にするための .NET サンプルコード](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [CSP プログラムのパートナー:セキュリティで保護されたアプリケーションモデルを有効にするための Java サンプルコード](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [パートナーセンターの認証ドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [パートナーセンターの PowerShell Multi-factor Authentication (MFA) ドキュメント](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>サポート

### <a name="where-can-i-ask-get-support"></a>サポートを受けるにはどうすればよいですか。

さらに、セキュリティ要件を満たすためのリソースの利用をサポートするために、パートナー (ASfP) の高度なサポートがある場合は、サービスアカウントマネージャーに問い合わせてください。パートナーアグリーメント (PSfP) の Premier サポートについては、サービスアカウントマネージャーとテクニカルアカウントマネージャーにお問い合わせください。

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>基準ポリシーの有効化に関するヘルプを表示するにはどうすればよいですか。

- パートナーは、MPN 特典からの勧告時間を利用して、セキュリティ要件の実装方法に関するより詳細なガイダンスを得ることができます。
- Azure Active Directory の技術製品サポートオプションについては、MPN 特典を参照してください。 アクティブな ASfP または PSfP 契約へのアクセス権を持つパートナーは、関連付けられているアカウントマネージャー (SAM/TAM) と連携して、使用可能なオプションを最大限に理解することができます。
- パートナーセンターでのベースラインポリシーの実装のサポートは、[パートナーセンターのサービス要求](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)によってアクセスできます。 トピックとして  *MFA & セキュリティで保護されたアプリケーションモデル* を選択します。

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>セキュリティで保護されたアプリケーションモデルフレームワークを採用するために技術情報を取得操作方法には 

Azure Active Directory の技術製品サポートオプションについては、MPN 特典を参照してください。 アクティブな ASfP または PSfP サブスクリプションへのアクセス権を持つパートナーは、関連付けられているアカウントマネージャー (SAM/TAM) と連携して、使用可能なオプションを最大限に理解することができます。

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>技術的な一般的な問題に関する詳細情報はどこで入手できますか。 

技術的な一般的な問題に関する情報については、[こちら](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)を参照してください。
