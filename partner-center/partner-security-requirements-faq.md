---
title: パートナーのセキュリティ要件の FAQ | パートナー センター
ms.topic: article
ms.date: 09/27/2019
description: パートナーのセキュリティ要件についてよく寄せられる質問
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.openlocfilehash: 43ad23ea7d4b4b39fb2dc6d15095a8416c7360ab
ms.sourcegitcommit: 1fe366f787d97c96510cfd409304e7d48af7c286
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2019
ms.locfileid: "73142031"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>パートナーのセキュリティ要件についてよく寄せられる質問

この記事では、[パートナーのセキュリティ要件](partner-security-requirements.md)に関してよく寄せられる質問をいくつか紹介します。

## <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

### <a name="what-are-the-new-partner-security-requirements"></a>新しいパートナーのセキュリティ要件はどのようなものですか?

パートナーとその顧客を保護するため、パートナーには次のアクションをすぐに実行するようお願いします。  

1. **パートナー テナント内のすべてのユーザーに対して多要素認証 (MFA) を有効にします**。 パートナー テナントのすべてのユーザーは、パートナー センターまたは API を使用して、Microsoft の商用クラウド サービスにサインインするとき、またはCSP で取引を行うときは、多要素認証 (MFA) を使用する必要があります。 ベースライン保護ポリシーを有効にすることで、パートナー テナントのすべてのユーザーは MFA を無料で利用できます。

2. **セキュリティで保護されたアプリケーション モデル フレームワークを採用します**。 Azure Resource Manager、Microsoft Graph、Partner Center API などの Microsoft API と統合しているすべてのパートナーは、ベースライン ポリシーが有効になっているときの統合の中断を避けるため、セキュリティで保護されたアプリケーション モデル フレームワークを採用する必要があります。

多要素認証 (MFA) を有効にし、セキュリティで保護されたアプリケーション モデル フレームワークを採用することにより、インフラストラクチャを保護し、ID 盗難や他の不正行為インシデントなどの潜在的なセキュリティ リスクから顧客のデータを保護することができます。  

### <a name="which-partners-need-to-meet-the-requirements"></a>どのパートナーが要件を満たす必要がありますか?

これらの要件は、次のパートナー グループを対象としています。

- クラウド ソリューション プロバイダー (CSP) プログラムに参加し、Microsoft の商用クラウド サービスを使用して取引を行っている、すべてのパートナー組織
  - 直接請求パートナー
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロール パネル ベンダー
- すべてのアドバイザー プログラム パートナー  

ソブリン クラウド (21Vianet、米国政府、およびドイツ) を使用して取引を行っているすべてのパートナーは、8 月 1 日に発効された新しいセキュリティ要件を満たす必要はありません。 ただし、ソブリン クラウドを使用するすべてのパートナーがこれらの新しいセキュリティ要件を直ちに採用することを強くお勧めします。 マイクロソフトでは、今後、ソブリン クラウドに対するこれらのセキュリティ要件の適用に関して、追加の詳細情報を提供する予定です。

### <a name="what-are-the-key-timelines-and-milestones"></a>重要なタイムラインとマイルストーンは何ですか?

これらのセキュリティ要件に関連する条項は、[クラウド ソリューション プロバイダー プログラムのプログラム ガイド](https://go.microsoft.com/fwlink/p/?LinkId=617100)にすぐに追加されます。 2019 年 8 月 1 日より有効になる CSP プログラムへの参加に準拠するには、これらのセキュリティ要件を実装する必要があります。

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>アクションを実行しないとどうなりますか?

これらのパートナー セキュリティ要件が適用されると、これらのセキュリティに関するプラクティスと義務に従わないパートナーは、クラウド ソリューション プロバイダー プログラムで取引したり、代理管理者権限を利用して顧客テナントを管理したりできなくなります。 現在、要件の適用開始日を設定しており、日付と詳細情報については、追ってパートナーに通知します。

### <a name="what-will-happen-if-i-dont-implement-mfa-as-per-this-new-security-requirement-by-august-1-2019"></a>2019 年 8 月 1 日までにこの新しいセキュリティ要件に従って MFA を実装していない場合はどうなりますか?

2019 年 8 月 1 日以降、[クラウド ソリューション プロバイダー プログラムのプログラム ガイド](https://go.microsoft.com/fwlink/p/?LinkId=617100)におけるこれらのセキュリティ要件に関連する条項が、有効になりました。 CSP プログラムに参加しているすべてのパートナーは、条項に準って要件を満たし、ビジネスを保護する必要があります。 これらのセキュリティ プラクティスを順守していないパートナーは、近い将来、パートナー セキュリティ要件に対する技術的適用が開始された後、CSP プログラムで取引を行ったり、委任管理者権限を利用して顧客のテナントを管理したりできなくなる可能性があります。 実施日の設定を行っており、間もなくパートナーにその日付が通知されます。

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>Microsoft がこれらの新しい要件を適用するのはなぜですか?

お客様とパートナーのセキュリティとプライバシーは、Microsoft の最優先事項です。 主に ID 侵害インシデントに関連する、ますます高度になったセキュリティ攻撃の数が増え続けています。 予防的な制御は、セキュリティ攻撃を阻止するための全体的な防御戦略において重要な役割を果たすので、パートナーとその顧客を保護するために、一連の必須のセキュリティ要件の適用を開始します。

### <a name="does-this-apply-to-all-geographies"></a>これはすべての地域に適用されますか?

はい、これはすべての地域に適用されます。 ソブリン クラウド (21Vianet、米国政府、およびドイツ) を介して取引するすべてのパートナーが直ちに行動し、これらの新しいセキュリティ要件を採用することを強くお勧めします。 ただし、これらのパートナーは、8 月 1 日に開始される新しいセキュリティ要件を満たす必要はありません。 マイクロソフトでは、今後、ソブリン クラウドに対するこれらのセキュリティ要件の適用に関して、追加の詳細情報を提供する予定です。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>アカウントを除外することはできますか?

いいえ。いかなるアカウントも、MFA 適用要件から除外することはできません。 パートナーは高度な特権を持っているため、[クラウド ソリューション プロバイダー プログラムのプログラム ガイド](https://go.microsoft.com/fwlink/p/?LinkId=617100)では、パートナー テナントの各アカウントに対して MFA を適用することが要求されています。

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>パートナーのセキュリティ要件を満たしているかどうかを知るにはどうすればよいですか?

以下の手順を完了する必要があります

- 「[パートナーのセキュリティ要件](https://docs.microsoft.com/partner-center/partner-security-requirements)」で示されているすべての要件を満たす必要があります
- パートナー テナント内のすべてのユーザー アカウントに多要素認証を適用する必要があります。

アクションを実行できる主要な領域を確認できるよう、パートナー センターから利用できる[セキュリティ要件状態](https://partner.microsoft.com/pcv/security/compliance)レポートが提供されています。

状態レポートの詳細については、「[パートナー セキュリティ要件の状態](https://docs.microsoft.com/partner-center/partner-security-compliance)」を参照してください。

## <a name="required-actions"></a>必要なアクション

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>要件を満たすために行う必要がある重要なアクションは何ですか?

CSP プログラムのすべてのパートナー (直接請求、間接プロバイダー、間接リセラー)、アドバイザー、およびコントロール パネル ベンダーは、要件を満たしている必要があります。

1. **すべてのユーザーに MFA を適用する**

    CSP プログラムのパートナー、アドバイザー、およびコントロール パネル ベンダーはすべて、パートナー テナント内のすべてのユーザーに対して MFA を適用する必要があります。 これを実現するには、[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)、[エンド ユーザー保護ベースライン](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)、および将来のすべてのベースライン ポリシーを有効にします。 ベースライン ポリシーによって提供される機能は、パートナーと顧客が絶え間なく変化するセキュリティの脅威から保護されるように発展し続けます。 そのため、[ベースライン ポリシーのドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を確認してよく理解することが重要です。

    - 「[ベースライン ポリシー: 管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)」で、"管理者に MFA を要求する" ベースライン ポリシーを有効にする方法の詳細を参照してください。
    - 「[ベースライン ポリシー: エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)」で、"エンド ユーザーの保護" ベースライン ポリシーを有効にする方法の詳細を参照してください。
    - [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の概念を理解してください。

    その他の考慮事項:

    - まだ行っていない場合は、間接プロバイダーは間接リセラーと協力して、パートナー センターにオンボードし、リセラーに要件を満たすよう奨励する必要があります。
    - Azure MFA は、[Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)を使用する唯一の認証方法によるベースライン ポリシーを通じて、パートナー テナントのすべてのユーザーが無料で利用できるようになっています。
    - 電話やテキスト メッセージなどの他の方法が必要な場合は、[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) SKU により、追加の検証方法を利用できます。
    - パートナーは、Microsoft の商用クラウド サービスにアクセスするときに、個々のアカウント単位でサードパーティの MFA ソリューションを利用することもできます。

2. **セキュリティで保護されたアプリケーション モデル フレームワークを採用する**

    何らかの API (Azure Resource Manager、Microsoft Graph、Partner Center API など) を使用してカスタム統合を開発したすべてのパートナー、または PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーション モデル フレームワークを採用する](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)を導入して、Microsoft クラウド サービスと統合する必要があります。 これを行わないと、MFA の展開によって中断が発生する可能性があります。 次のリソースでは、モデルの導入方法に関する概要とガイダンスが提供されています。

    - [セキュリティで保護されたアプリケーション モデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [パートナー センター: セキュリティで保護されたアプリケーション モデルのガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための .NET サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための Java サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [パートナー センターの認証に関するドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [パートナー センターの PowerShell Multi-Factor Authentication (MFA) に関するドキュメント](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    コントロール パネルを使用している場合は、セキュリティで保護されたアプリケーション モデル フレームワークの導入について、ベンダーと相談する必要があります。

    コントロール パネル ベンダーは、コントロール パネル ベンダーとしてパートナー センターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始する必要があります。 「[パートナー センター: セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。 コントロール パネル ベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

## <a name="multi-factor-authentication"></a>多要素認証

### <a name="what-is-multi-factor-authentication-mfa"></a>Multi-Factor Authentication (MFA) とは何ですか?

MFA は、ユーザーが複数の必要なセキュリティと検証の手順によって認証されるセキュリティ メカニズムです。 それは、次の認証方法のうち 2 つ以上を必須にすることで機能します。

- ユーザーが知っている情報 (一般にパスワード)
- ユーザーの所持品 (複製が困難な、携帯電話などの信頼されているデバイス)
- ユーザー自身の特性 (生体認証)

### <a name="what-are-baseline-protection-policies"></a>ベースライン保護ポリシーとは何ですか?

[Microsoft ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (現在はプレビュー) は、一般的な数々の攻撃から組織を保護するうえで役立つ定義済みポリシー セットです。 これらの一般的な攻撃には、パスワードのスプレー、リプレイ、フィッシングなどがあります。 ベースライン ポリシーは、Azure Active Directory のすべてのエディションで使用できます。 ID ベースの攻撃がここ数年にわたって増加しているため、Microsoft はこれらのベースライン保護ポリシーをすべてのユーザーが利用できるようにしています。 これらのポリシーの目的は、すべての組織において追加コストなしでベースライン レベルのセキュリティを有効にできるようにすることです。

> [!NOTE]
> Microsoft のベースライン ポリシーと関連する機能は、絶え間なく変化するセキュリティの脅威からパートナーと顧客をより適切に保護するために、進化し続けています。 ベースライン ポリシーでは、名前付けと分類に関するいくつかの変更が間もなく行われる可能性があります。 ベースライン ポリシーのページに直接アクセスし、最新の情報を確認することを強くお勧めします。

### <a name="what-baseline-policies-must-i-enable"></a>有効にする必要があるベースライン ポリシーは何ですか?

現在のベースライン保護ポリシーを使用して、パートナー テナントの各アカウントに MFA を提供する予定の場合は、[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)および[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン ポリシーを有効にする必要があります。 これらのベースライン保護ポリシーでは、モバイル デバイス経由で Microsoft Authenticator アプリを使用しているパートナーについてのみ、パートナー テナントの各ユーザーに対する MFA の要件が無料で満たされます。

[管理者に MFA を要求するベースライン ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)はパートナー ディレクトリ内の管理ユーザーに対して利用され、[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)ベースライン ポリシーはパートナー テナント内の管理者以外のユーザーを保護するために利用されます。 これらのポリシーを有効にすると、ユーザーは MFA に登録する必要があります。 ユーザーは、正常に登録した後、ポリシーの条件に基づいてサインインを試行するときに MFA を要求されます。 ベースライン ポリシーによって提供される機能は、パートナーと顧客が絶え間なく変化するセキュリティの脅威から保護されるように発展し続けます。 そのため、[ベースライン ポリシーのドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)を確認してよく理解することが重要です。

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>管理者に MFA を要求するポリシーを有効にするにはどうすればよいですか?

管理者に MFA を要求するベースライン ポリシーは、Azure 管理ポータルを使用して有効にできます。 「[ベースライン ポリシー: 管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)」で、このベースライン ポリシーを有効にする方法の詳細を参照してください。

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>エンド ユーザーの保護ポリシーを有効にするにはどうすればよいですか?

エンド ユーザーの保護ベースライン ポリシーは、Azure 管理ポータルを使用して有効にできます。 「[ベースライン ポリシー: エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)」で、このベースライン ポリシーを有効にする方法の詳細を参照してください。

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>ベースライン ポリシーは自動的に有効になりますか?

いいえ。これらのポリシーを有効にするには、グローバル管理者、セキュリティ管理者、または条件付きアクセス管理者の役割のメンバーであるユーザーが、ポリシーをすぐに使用するように構成する必要があります。

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA を有効にするとどのようなコストがかかりますか?

MFA は、[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)および[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシーにより、無料で提供されます。 このバージョンの MFA で利用できる検証オプションは、[Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)だけです。 電話呼び出しまたは SMS メッセージが必要な場合は、[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) ライセンスを購入する必要があります。 または、サードパーティのソリューションを利用して、パートナー テナントの各ユーザーに MFA を提供することもできます。この場合、MFA ソリューションが適用されていること、および準拠していることは、パートナーが確認する責任があります。

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>既に MFA ソリューションがある場合、どのようなアクションを実行する必要がありますか?

これらのセキュリティ要件では、パートナー テナントのユーザーは、Microsoft の商用クラウド サービスにアクセスするときに、MFA を使用して認証を行う必要があります。 サードパーティのソリューションを使用して、これらの要件を満たすことができます。 Microsoft では、Azure Active Directory との互換性に関する検証テストを、独立系 ID プロバイダーに提供しなくなりました。 お使いの製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

> [!IMPORTANT]
> サードパーティのソリューションを使用している場合は、そのソリューションで MFA 値を含む認証方法参照 (AMR) 要求が発行されていることを確認することが重要です。 想定されている要求がサードパーティのソリューションで発行されていることを検証する方法の詳細については、「[パートナーのセキュリティ要件のテスト](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)」を参照してください。

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>MFA の認証を行うためにどのような検証方法を使用できますか?

MFA は、[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)および[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシーにより、無料で提供されます。 このバージョンの MFA で利用できる検証オプションは、[Microsoft Authenticator アプリ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview)だけです。 電話呼び出しまたは SMS メッセージが必要な場合は、[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) ライセンスを購入する必要があります。 または、サードパーティのソリューションを利用して、パートナー テナントの各ユーザーに MFA を提供することもできます。この場合、MFA ソリューションが適用されていること、および準拠していることは、パートナーが確認する責任があります。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>複数のパートナー テナントを使用して取引を行っています。 これらすべてに MFA を実装する必要がありますか?

はい。CSP プログラムまたは Advisor プログラムに関連付けられている Azure Active Directory テナントごとに、MFA を適用する必要があります。 Azure Active Directory Premium ライセンスの購入を計画している場合は、各 Azure Active Directory テナントのユーザーに対してライセンスを購入する必要があります。

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>パートナー テナントの各ユーザーに MFA を適用する必要がありますか?*

[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)および[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン保護ポリシーでは、パートナー テナントの各ユーザーに対して MFA が強適用されます。 これらのポリシーを利用して MFA を提供し、[Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) アプリケーションを使用している場合は、追加のライセンスを購入する必要はありません。 それ以外の場合は、パートナー テナントの各ユーザーに MFA を提供するための適切なソリューションを購入する必要があります。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft との直接請求パートナーです。 何をする必要がありますか?

直接請求のクラウド ソリューション プロバイダー パートナーは、パートナー テナント内の各ユーザーに対して MFA を適用する必要があります。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>間接リセラーであり、ディストリビューターを通してだけ取引を行っています。 それでもこれを行う必要がありますか?

すべての間接リセラーは、パートナー テナントの各ユーザーに対して MFA を適用する必要があります。 これは、間接リセラーが実行する必要のあるアクションです。

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Partner Center API を使用していません。 それでも MFA を実装する必要がありますか?

はい。このセキュリティ要件は、パートナー管理者ユーザーと、パートナー テナント内のエンド ユーザーを含む、すべてのユーザーを対象としたものです。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Azure Active Directory と互換性のある MFA ソリューションは、どのサードパーティ ベンダーから提供されていますか?

[Gartner](https://www.gartner.com/en/webinars/3881781) など、MFA ソリューションに関するオンラインの独立したレビューが多数あります。 MFA のベンダーとソリューションをレビューする場合、パートナーは、選択したソリューションが Azure Active Directory と互換性があることを確認する必要があります。

Microsoft では、Azure Active Directory との互換性に関する検証テストを、独立系 ID プロバイダーに提供しなくなりました。 お使いの製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

詳しくは、「[Azure AD のフェデレーション互換性リスト](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)」をご覧ください。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>統合サンドボックスで MFA をテストするにはどうすればよいですか?

[管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)および[エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)のベースライン ポリシーを、統合サンドボックス テナントに対して有効にする必要があります。 このポリシーにより、テナントの各ユーザーは、MFA を使用して認証を行う必要があります。

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>MFA を有効にすると、顧客のテナントと対話する方法に影響がありますか?

いいえ。 これらのセキュリティ要件を実現しても、顧客の管理方法には影響しません。 委任された管理操作を実行する機能は損なわれません。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>パートナーの顧客は、パートナーのセキュリティ要件の対象になりますか?

いいえ。顧客の Azure AD テナント内の各ユーザーに対して、MFA を適用する必要はありません。 ただし、各顧客と協力して、顧客のユーザーの保護に最適な方法を決定することをお勧めします。

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>アプリ パスワードをベースライン保護ポリシーで使用できますか?

はい。[アプリ パスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)を使用できます。 [こちら](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリ パスワード使用時の考慮事項を確認し、ニーズにそれらが対応しているかどうかを確かめる必要があります。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>この要件からユーザーを除外することはできますか?

いいえ。サービス アカウントを含む、パートナー テナントの各ユーザーは、MFA を使用して認証を行う必要があります。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>パートナー セキュリティ要件は統合サンドボックスに適用されますか?

はい。パートナー セキュリティ要件は統合サンドボックスに適用されます。 これは、統合サンドボックス テナント内のユーザーに適切な MFA ソリューションを実装する必要があることを意味します。 ベースライン保護ポリシーを実装して MFA を提供することをお勧めします。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>緊急アクセス (非常事態用) アカウントを構成するにはどうすればよいですか?

Azure AD テナントから誤ってロックアウトされるのを防ぐために、1 つまたは 2 つの緊急アクセス アカウントを作成するのがベスト プラクティスと考えられます。 パートナー セキュリティ要件に関しては、各ユーザーが MFA を使用して認証を行う必要があります。 したがって、これは緊急アクセス アカウントの定義を変更する必要があることを意味します。 MFA にサードパーティ ソリューションを利用しているアカウントでもかまいません。

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>ゲスト ユーザーは、パートナー セキュリティ要件によってどのような影響を受けますか?

ゲスト ユーザーは、パートナー テナント内のリソースにアクセスするときに、MFA を使用して認証を行う必要があります。 ゲスト ユーザーが自分のテナントのリソースにアクセスするときは、パートナー セキュリティ要件の影響を受けません。

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>サードパーティのソリューションを使用している場合、Active Directory フェデレーション サービス (ADFS) は必要ですか?

いいえ、サードパーティのソリューションを使用している場合は、Active Directory フェデレーション サービス (ADFS) を使用する必要はありません。 ソリューションのベンダーと協力して、ソリューションの要件を決定することをお勧めします。

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>ベースライン保護ポリシーを有効にする必要はありますか?

いいえ。ベースライン保護ポリシーを有効にする必要はありません。 唯一の要件は、パートナー テナント内の各ユーザー (サービス アカウントを含む) に MFA を適用することです。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA の要件を満たすために条件付きアクセスを使用できますか?

はい、条件付きアクセスを使用して、パートナー テナント内の各ユーザー (サービス アカウントを含む) に MFA を適用できます。 ただし、パートナーには高い特権が付与されている、という点を考えると、すべての単一認証について、MFA チャレンジが各ユーザーに確実に適用されるようにする必要があります。 これは、MFA の要件を回避する条件付きアクセスの機能は利用できないことを意味します。

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>ベースライン保護ポリシーの実装では、どのような検証オプションが提供されますか?

ベースライン保護ポリシーの実装によって利用可能な MFA のバージョンに関して、使用可能な検証オプションは Authenticator アプリだけです。 電話呼び出しとテキスト メッセージの使用は、安全性が低いものと見なされます。 そのため、これらのオプションは、このバージョンの MFA では使用できません。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect によって使用されるサービス アカウントは、パートナー セキュリティ要件の影響を受けますか?

いいえ、Azure AD Connect によって使用されるサービス アカウントは、パートナー セキュリティ要件の影響を受けません。 MFA を適用した結果として Azure AD Connect で問題が発生する場合は、Microsoft サポートに連絡してテクニカル サポートを依頼してください。

## <a name="secure-application-model"></a>セキュリティで保護されたアプリケーション モデル

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>要件を満たすには、誰がセキュリティで保護されたアプリケーションモデルを採用する必要がありますか?

Microsoft では、多要素認証を利用するクラウド ソリューション プロバイダー (CSP) パートナーおよびコントロール パネル ベンダー (CPV) を認証するために、セキュリティで保護されたスケーラブルなフレームワークを導入しています。 詳細については、[セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。 何らかの API (Azure Resource Manager、Microsoft Graph、Partner Center API など) を使用してカスタム統合を開発したすべてのパートナー、または PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーション モデル フレームワークを採用する](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)を導入して、Microsoft クラウド サービスと統合する必要があります。

### <a name="what-is-the-secure-application-model"></a>セキュリティで保護されたアプリケーション モデルとは何ですか?

Microsoft では、多要素認証を利用するクラウド ソリューション プロバイダー (CSP) パートナーおよびコントロール パネル ベンダー (CPV) を認証するために、セキュリティで保護されたスケーラブルなフレームワークを導入しています。 詳細については、[セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)を参照してください。  

### <a name="how-do-i-implement-the-secure-application-model"></a>セキュリティで保護されたアプリケーション モデルを実装するにはどうすればよいですか?

何らかの API (Azure Resource Manager、Microsoft Graph、Partner Center API など) を使用してカスタム統合を開発したすべてのパートナー、または PowerShell などのツールを使用してカスタム自動化を実装したすべてのパートナーは、[セキュリティで保護されたアプリケーション モデル フレームワークを採用する](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)を導入して、Microsoft クラウド サービスと統合する必要があります。 これを行わないと、MFA の展開によって中断が発生する可能性があります。 次のリソースでは、モデルの導入方法に関する概要とガイダンスが提供されています。

- [セキュリティで保護されたアプリケーション モデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [パートナー センター: セキュリティで保護されたアプリケーション モデルのガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための .NET サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための Java サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [パートナー センターの認証に関するドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [パートナー センターの PowerShell Multi-Factor Authentication (MFA) に関するドキュメント](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

コントロール パネルを使用している場合は、セキュリティで保護されたアプリケーション モデル フレームワークの導入について、ベンダーと相談する必要があります。

コントロール パネル ベンダーは、コントロール パネル ベンダーとしてパートナー センターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始する必要があります。 「[パートナー センター: セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。 コントロール パネル ベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

### <a name="who-is-a-control-panel-vendor-cpv"></a>コントロール パネル ベンダー (CPV) とは何ですか?

コントロール パネル ベンダーとは、Partner Center API と統合するために CSP パートナーによって使用されるアプリを開発する独立系ソフトウェア ベンダーです。 コントロール パネル ベンダーは、パートナー センター ダッシュボードまたは API に直接アクセスできる CSP パートナーではありません。 詳しくは、「[パートナー センター: セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>セキュリティで保護されたアプリケーション モデルは、Partner Center API/SDK に対してのみ実装する必要がありますか?

*管理者に MFA を要求する*と*エンド ユーザーの保護*のベースライン ポリシーを両方とも有効にすると、各ユーザーは多要素認証を使用して認証を行うことが必要になります。 つまり、非対話形式で実行され、認証にユーザー資格情報を使用することが意図されている、各 API、CLI、および PowerShell モジュール (Azure、Azure AD、MS Online、Partner Center など) に対して、セキュリティで保護されたアプリケーション モデルを実装する必要があります。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell などの自動化ツールを使用しています。 セキュリティで保護されたアプリケーション モデルを実装するにはどうすればよいですか?

自動化が、非対話形式で実行され、認証にユーザー資格情報を使用するためである場合は、セキュリティで保護されたアプリケーション モデルを実装する必要があります。 このフレームワークを実装する方法については、[Partner Center PowerShell のセキュリティで保護されたアプリケーション モデル](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5)に関する記事をご覧ください。  すべての自動化ツールでアクセス トークンを使用して認証を行う機能が提供されているわけではないことに注意してください。 どのような変更が必要であるかを理解するために支援が必要な場合は、[パートナー センター セキュリティ ガイダンス](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) グループにメッセージを投稿してください。

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>同意プロセスを実行するとき、アプリケーション管理者はどのようなユーザー資格情報を提供する必要がありますか?

最小限の特権のアクセス許可が割り当てられているサービス アカウントを使用することをお勧めします。 Partner Center API の場合、販売代理店ロールまたは管理エージェント ロールが割り当てられているアカウントを使用する必要があることを意味します。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>同意プロセスを実行するとき、アプリケーション管理者がグローバル管理者のユーザー資格情報を提供してはならないのはなぜですか?

最小限の特権の ID を使用してリスクを軽減するのがベスト プラクティスです。 グローバル管理者特権を持つアカウントを使用することは、必要なものより多くのアクセス許可を提供するため、推奨されません

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>私は CSP パートナーです。 コントロール パネル ベンダー (CPV) がソリューションの実装作業を行っているかどうかを確認するには、どうすればよいですか?

コントロール パネル ベンダー (CPV) ソリューションを使用してクラウド ソリューション プロバイダー (CSP) プログラムで取引を行っているパートナーは、自分で CPV に問い合わせる必要があります。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>私は CPV です。 登録するにはどうすればよいですか?

コントロール パネル ベンダー (CPV) として登録するには、[こちら](https://docs.microsoft.com/partner-center/enroll-as-cpv)のガイドラインに従ってください。

登録リンクを受け取るには、CPV は [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) に連絡し、CPV とビジネス上の関係がある、または CPV のビジネスを理解している、Microsoft 従業員スポンサーを指定する必要があります。 たとえば、パートナー開発マネージャー (PDM) などです。

パートナー センターに登録して、アプリケーションを登録すると、Partner Center API にアクセスできるようになります。 新しく CPV になった場合は、パートナー センターの通知を通じてサンドボックスの情報を受け取ります。 Microsoft CPV として登録を完了し、CPV 契約に同意すると、次のことができるようになります。

1. マルチテナント アプリケーションを管理する (Azure portal へのアプリケーションの追加、パートナー センターでのアプリケーションの登録と登録解除)。 注:CPV は、Partner Center API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。 Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。
2. CPV プロファイルを表示および管理する。
3. CPV 機能にアクセスする必要があるユーザーを表示および管理する。 CPV が持つことのできる唯一のロールは、グローバル管理者です。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Partner Center SDK を使用しています。 SDK ではセキュリティで保護されたアプリケーション モデルが自動的に使用されますか?

いいえ。[セキュリティで保護されたアプリケーションモデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)に記載されているガイドラインに従う必要があります。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>MFA が有効になっていないアカウントを使用して、セキュリティで保護されたアプリケーション モデルに対して更新トークンを生成できますか?

はい。MFA が適用されていないアカウントを使用して、更新トークンを生成できます。 ただし、MFA が有効になっていないアカウントを使用して生成されたトークンでは、MFA の要件によりリソースにアクセスできないため、これは行わないでください。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA が有効になっている場合、アプリケーションでアクセス トークンを取得するにはどうすればよいですか?

[セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)で提供されている、新しいセキュリティ要件に準拠しながらそれを行う方法の詳細に従う必要があります。 .NET のサンプル コードは[こちら](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)に、Java のサンプル コードは[こちら](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)にあります。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV は、CPV テナントまたは CSP パートナーのテナントのどちらに Azure AD アプリケーションを作成しますか?

CPV は、CPV として登録に関連付けられているテナントに Azure Active Directory アプリケーションを作成する必要があります。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>アプリのみの認証を使用している CSP です。 何か変更する必要がありますか?

ユーザーの資格情報はアクセス トークンの要求に使用されないため、アプリのみの認証は影響を受けません。 ユーザーの資格情報が共有されている場合は、コントロール パネル ベンダー (CPV) は[セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)を採用し、所有している既存のパートナー資格情報を消去する必要があります。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV は、アプリのみの認証スタイルを利用してアクセス トークンを取得できますか?

いいえ。コントロール パネル ベンダー パートナーは、パートナーの代わりに、アプリのみの認証スタイルを利用してアクセス トークンを要求することはできません。 アプリとユーザー認証のスタイルが利用される、セキュリティで保護されたアプリケーション モデルを実装する必要があります。

## <a name="enforcement"></a>強制

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>サードパーティの MFA ソリューションを使用していますが、ブロックされます。どうすればよいですか?

リソースにアクセスするアカウントで多要素認証が要求されていることを検証するために、[認証方法参照](https://tools.ietf.org/html/rfc8176)要求を調べて、MFA が含まれているかどうかが確認されます。 一部のサードパーティ ソリューションでは、この要求が発行されないか、MFA 値が含まれていません。 要求が存在しない場合、または MFA 値が表示されない場合は、認証対象のアカウントで多要素認証が要求されたかどうかを判断する方法がありません。 サードパーティのソリューションのベンダーと協力して、ソリューションで認証方法参照要求を発行するために実行する必要があるアクションを決定する必要があります。

想定されている要求がサードパーティのソリューションで発行されているかどうか不明な場合は、「[パートナーのセキュリティ要件のテスト](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0)」を参照してください。

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>AOBO を使用した顧客のサポートが MFA によってブロックされます。どうすればよいですか?

パートナーのセキュリティ要件の技術的適用では、認証対象のアカウントで多要素認証が求められたかどうかが確認されます。 求められていない場合、ログイン ページにリダイレクトされ、再度認証するように求められます。 ドメインがフェデレーションされていない場合は、正常に認証された後、多要素認証を設定するように求められます。 それが完了すると、AOBO を使用して顧客を管理できるようになります。 ドメインがフェデレーションされている場合は、アカウントに対して多要素認証が求められることを確認する必要があります。

## <a name="key-resources"></a>重要なリソース

### <a name="how-to-get-started"></a>開始する方法

- [パートナーのセキュリティ要件: ステップバイステップ ガイド](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 質問とフィードバックは、この[パートナー センター セキュリティ ガイダンス グループ](https://aka.ms/MPCSecurityGuidance)にお送りください。
- 今後予定されているパートナーの業務時間とウェビナーに参加してください。 [詳細なスケジュールとリソースをこちら](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)で確認してください。

### <a name="resources-for-enabling-mfa"></a>MFA の有効化に関するリソース

- [ベースライン保護ポリシー](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)の概念を理解してください。
- 「[ベースライン ポリシー: 管理者に MFA を要求する](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)」で、"管理者に MFA を要求する" ベースライン ポリシーを有効にする方法の詳細を参照してください。
- 「[ベースライン ポリシー: エンド ユーザーの保護](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)」で、"エンド ユーザーの保護" ベースライン ポリシーを有効にする方法の詳細を参照してください。

### <a name="resources-for-adopting-secure-application-model"></a>セキュリティで保護されたアプリケーション モデルの採用に関するリソース

- [セキュリティで保護されたアプリケーション モデルの概要](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [パートナー センター: セキュリティで保護されたアプリケーション モデルのガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための .NET サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [CSP プログラムでのパートナー: セキュリティで保護されたアプリケーション モデルを有効にするための Java サンプル コード](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [パートナー センターの認証に関するドキュメント](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [パートナー センターの PowerShell Multi-Factor Authentication (MFA) に関するドキュメント](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>サポート

### <a name="where-can-i-get-support"></a>サポートの入手場所

セキュリティ要件を満たすためのサポート リソースについては、Advanced Support for Partners (ASfP) をお持ちの場合は、サービス アカウント マネージャーに問い合わせてください。Premier Support for Partners (PSfP) 契約をお持ちの場合は、サービス アカウント マネージャーとテクニカル アカウント マネージャーに問い合わせてください。

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>ベースライン ポリシーの有効化に関するヘルプを得るにはどうすればよいですか?

- パートナーは、MPN 特典の相談時間を利用して、セキュリティ要件の実装方法に関するより詳細なガイダンスを得ることができます。
- Azure Active Directory の技術製品サポート オプションを、MPN 特典で利用できます。 アクティブな ASfP または PSfP 契約にアクセスできるパートナーは、関連付けられているアカウント マネージャー (SAM/TAM) と協力して、利用可能なオプションを最大限に理解することができます。
- パートナー センターでのベースライン ポリシーの実装のサポートには、[パートナー センターのサービス要求](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp)によってアクセスできます。 トピックとして、 *[MFA & Secure Application Model]\(MFA & セキュリティで保護されたアプリケーション モデル\)* を選択します。

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>セキュリティで保護されたアプリケーション モデル フレームワークを導入するのに役立つ技術情報とサポートを利用するにはどうすればよいですか?

Azure Active Directory の技術製品サポート オプションを、MPN 特典で利用できます。 アクティブな ASfP または PSfP サブスクリプションにアクセスできるパートナーは、関連付けられているアカウント マネージャー (SAM/TAM) と協力して、使用可能なオプションを最大限に理解することができます。

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>パートナー センターへのアクセスが失われた場合、サポートに問い合わせるにはどうすればよいですか?

「[マイクロソフト パートナー サポート](https://partner.microsoft.com/support)」にアクセスし、 **[すべてのサポート オプションを表示する]** を選択します。 マイクロソフト パートナー サポートに連絡するために使用できるオプションが表示されます。 これには、サポートに電話するための電話番号と、サポートとチャットするためのオプションが含まれます。 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>一般的な技術的問題に関する詳細情報はどこで入手できますか?

一般的な技術的問題に関する情報については、[こちら](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)を参照してください。
