---
title: パートナーのセキュリティ要件の FAQ | パートナー センター
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーのセキュリティ要件についてよく寄せられる質問
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.openlocfilehash: 72ad7bab25c295fa039e7b29f9d4369c0434814c
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "80529777"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>パートナーのセキュリティ要件についてよく寄せられる質問

**該当するユーザー**

- ゲスト ユーザーを含むすべての有効なユーザー

この記事では、[パートナーのセキュリティ要件](partner-security-requirements.md)に関してよく寄せられる質問をいくつか紹介します。

## <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

### <a name="what-are-the-partner-security-requirements-and-why-should-partners-implement"></a>パートナーのセキュリティ要件とは? パートナーが実装すべき理由とは?

高いレベルのセキュリティおよびプライバシーの保護の継続的な実施は最優先事項の1つであり、パートナーが顧客とテナントを保護する上で Microsoft は引き続き支援を提供していきます。 主に ID 侵害インシデントに関連する、ますます高度になったセキュリティ攻撃の数が増え続けています。 セキュリティ攻撃を阻止する全体的な防御戦略において、予防策は重要な役割を果たすため、 [必須のセキュリティ要件](partner-security-requirements.md) を 2019 年に導入しています。 クラウド ソリューション プロバイダー (CSP) プログラムに参加するすべてのパートナー、コントロール パネル ベンダー (CPV)、およびアドバイザーは、準拠を維持するための要件を実装する必要があります。

### <a name="what-are-the-key-timelines-and-milestones"></a>重要なタイムラインとマイルストーンは何ですか?

これらのセキュリティ要件に関連する条件は、2019 年の Microsoft Partner Agreement に記載されています。 CSP プログラムへの参加に継続して準拠するには、これらのセキュリティ要件をできるだけ早く実装する必要があります。

### <a name="what-will-happen-if-i-dont-implement-these-partner-security-requirements"></a>これらのパートナー セキュリティ要件を実装しないとどうなりますか?

Microsoft Partner Agreement では、パートナーは、ユーザー アカウントに多要素認証を適用し、Partner Center API とのインタラクションのためのセキュア アプリケーション モデルを採用することが要求されています。 

これらのセキュリティ プラクティスを順守していないパートナーは、CSP プログラムでの取引や、委任管理権限を利用した顧客テナントの管理ができなくなる可能性があります。

### <a name="does-this-apply-to-all-geographies"></a>これはすべての地域に適用されますか?

はい、これはすべての地域に適用されます。 ソブリン クラウド (21Vianet、米国政府、およびドイツ) を介して取引するすべてのパートナーが直ちに行動し、これらの新しいセキュリティ要件を採用することを強くお勧めします。 ただし、これらのパートナーは、8 月 1 日から有効となる新しいセキュリティ要件を満たす必要はありません。 マイクロソフトでは、今後、ソブリン クラウドに対するこれらのセキュリティ要件の適用に関して、追加の詳細情報を提供する予定です。

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>アカウントを除外することはできますか?

いいえ。いかなるユーザー アカウントも、MFA 適用要件から除外することはできません。 パートナーは高度な特権を持っているため、Microsoft Partner Agreement では、パートナー テナントの各ユーザー アカウントに対して多要素認証を適用することが要求されています。

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>パートナーのセキュリティ要件を満たしているかどうかを知るにはどうすればよいですか?

以下の手順を完了する必要があります

- [パートナーのセキュリティ要件](https://docs.microsoft.com/partner-center/partner-security-requirements)に概説されているすべての要件を満たす必要があります
- パートナー テナント内のすべてのユーザー アカウントに多要素認証を適用する必要があります。

アクションを実行できる主要な領域を確認できるよう、パートナー センターから利用できる[セキュリティ要件状態](https://partner.microsoft.com/pcv/security/compliance)レポートが提供されています。

状態レポートの詳細については、「[パートナー セキュリティ要件の状態](https://docs.microsoft.com/partner-center/partner-security-compliance)」を参照してください。

## <a name="required-actions"></a>必要なアクション

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>要件を満たすために行う必要がある重要なアクションは何ですか?

CSP プログラムのすべてのパートナー (直接請求、間接プロバイダー、間接リセラー)、アドバイザー、およびコントロール パネル ベンダーは、要件を満たす必要があります。

1. **すべてのユーザーに MFA を適用する**

    CSP プログラムのパートナー、アドバイザー、およびコントロール パネル ベンダーはすべて、パートナー テナント内のすべてのユーザーに対して MFA を適用する必要があります。

    その他の考慮事項:

    - まだ行っていない場合は、間接プロバイダーは間接リセラーと協力して、パートナー センターにオンボードし、リセラーに要件を満たすよう奨励する必要があります。
    - Azure AD のセキュリティの規定値により、Azure MFA はパートナー テナントのすべてのユーザーが無料で利用できます。時間ベースのワンタイム パスワード (TOTP) をサポートする認証アプリケーションの検証方法のみが提供されます。
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

    セキュア アプリケーション モデル フレームワークの導入についてコントロール パネルを使用する場合は、ベンダーにお問い合わせください。

    コントロール パネル ベンダーは、コントロール パネル ベンダーとしてパートナー センターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始する必要があります。 「[パートナー センター: セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。 コントロール パネル ベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

## <a name="multi-factor-authentication"></a>多要素認証

### <a name="what-is-multi-factor-authentication-mfa"></a>Multi-Factor Authentication (MFA) とは何ですか?

MFA は、ユーザーが複数の必要なセキュリティと検証の手順によって認証されるセキュリティ メカニズムです。 それは、次の認証方法のうち 2 つ以上を必須にすることで機能します。

- ユーザーが知っている情報 (一般にパスワード)
- ユーザーの所持品 (複製が困難な、携帯電話などの信頼されているデバイス)
- ユーザー個人を特定するもの (生体認証)

### <a name="what-is-the-cost-of-enabling-mfa"></a>MFA を有効にするとどのようなコストがかかりますか?

Microsoft では、Azure AD のセキュリティの既定値を実装することによって、MFA が無料で提供されています。 このバージョンの MFA で利用できる検証オプションは、認証アプリケーションだけです。 電話呼び出しまたは SMS メッセージが必要な場合は、[Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) ライセンスを購入する必要があります。 または、サードパーティのソリューションを利用して、パートナー テナントの各ユーザーに MFA を提供することもできます。この場合、パートナーは、MFA ソリューションが適用され、準拠していることを確認する責任があります。

### <a name="what-actions-do-i-need-to-take-if-i-already-have-an-mfa-solution"></a>既に MFA ソリューションを導入している場合、どのようなアクションをとる必要がありますか?

これらのセキュリティ要件では、パートナー テナントのユーザーは、Microsoft の商用クラウド サービスにアクセスするときに、MFA を使用して認証を行う必要があります。 サードパーティのソリューションを使用して、これらの要件を満たすことができます。 Microsoft では、Azure Active Directory との互換性に関する検証テストを、独立系 ID プロバイダーに提供しなくなりました。 使用する製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

> [!IMPORTANT]
> サードパーティのソリューションを使用している場合は、そのソリューションが MFA 値を含む認証方法参照 (AMR) 要求を発行していることを確認することが重要です。 想定される要求がサードパーティのソリューションで発行されていることを検証する方法の詳細については、「[パートナーのセキュリティ要件のテスト](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)」を参照してください。

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>複数のパートナー テナントを使用して取引を行っています。 これらすべてに MFA を実装する必要がありますか?

はい。CSP プログラムまたは アドバイザー プログラムに関連付けられている Azure Active Directory テナントごとに、MFA を適用する必要があります。 Azure Active Directory Premium ライセンスを購入する場合は、Azure Active Directory テナントの各ユーザーに対してライセンスを購入する必要があります。

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>パートナー テナントの各ユーザー アカウントに MFA を適用する必要がありますか?

はい、各ユーザーに MFA を適用する必要があります。 ただし、Azure AD のセキュリティの既定値を使用している場合は、この機能によりすべてのユーザーアカウントに MFA が適用されるため、追加の作業は必要ありません。 セキュリティの既定値を有効にすることは、ユーザー アカウントが MFA に準拠し、MFA の適用による影響を受けないための、無料の簡単な方法です。

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Microsoft との直接請求パートナーです。 何をする必要がありますか?

直接請求のクラウド ソリューション プロバイダー パートナーは、パートナー テナント内の各ユーザーに対して MFA を適用する必要があります。

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>間接リセラーであり、ディストリビューターを通してだけ取引を行っています。 それでもこれを行う必要がありますか?

すべての間接リセラーは、パートナー テナントの各ユーザーに対して MFA を適用する必要があります。 これは、間接リセラーが実行する必要のあるアクションです。

### <a name="i-dont-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>Partner Center API は使用していません。 それでも MFA を実装する必要がありますか?

はい。このセキュリティ要件は、パートナー管理者ユーザーと、パートナー テナント内のエンド ユーザーを含め、すべてのユーザーを対象としています。

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>Azure Active Directory と互換性のある MFA ソリューションは、どのサードパーティ ベンダーから提供されていますか?

MFA のベンダーとソリューションをレビューする場合、パートナーは、選択したソリューションが Azure Active Directory と互換性があることを確認する必要があります。

Microsoft では、Azure Active Directory との互換性に関する検証テストを、独立系 ID プロバイダーに提供しなくなりました。 使用する製品の相互運用性をテストする場合は、次の[ガイドライン](https://www.microsoft.com/download/details.aspx?id=56843)を参照してください。

詳しくは、「[Azure AD のフェデレーション互換性リスト](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility)」を参照してください。

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>統合サンドボックスで MFA をテストするにはどうすればよいですか?

Azure AD のセキュリティの既定値機能を有効にする必要があります。または、フェデレーションを利用するサードパーティのソリューションを利用することもできます。

### <a name="will-enabling-mfa-affect-how-i-interact-with-my-customers-tenant"></a>MFA を有効にすると、顧客のテナントとのインタラクション方法に影響がありますか?

いいえ。 これらのセキュリティ要件を実現しても、顧客の管理方法には影響しません。 委任された管理操作を実行する機能は損なわれません。

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>パートナーの顧客は、パートナーのセキュリティ要件の対象になりますか?

いいえ。顧客の Azure AD テナント内の各ユーザーに対して、MFA を適用する必要はありません。 ただし、各顧客と協力して、顧客のユーザーの保護に最適な方法を決定することをお勧めします。

### <a name="can-any-user-be-excluded-from-this-requirement"></a>この要件からユーザーを除外することはできますか?

いいえ。サービス アカウントを含む、パートナー テナントの各ユーザーは、MFA を使用して認証を行う必要があります。

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>パートナー セキュリティ要件は統合サンドボックスに適用されますか?

はい。パートナー セキュリティ要件は統合サンドボックスに適用されます。 つまり、統合サンドボックス テナント内のユーザーに適切な MFA ソリューションを実装する必要があります。 Azure AD のセキュリティの既定値を実装して MFA を提供することをお勧めします。

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>緊急アクセス (非常事態用) アカウントを構成するにはどうすればよいですか?

Azure AD テナントから誤ってロックアウトされることを防ぐために、1 つまたは 2 つの緊急アクセス アカウントを作成することがベスト プラクティスとして推奨されます。 パートナー セキュリティ要件に関しては、各ユーザーが MFA を使用して認証を行う必要があります。 つまり、緊急アクセス アカウントの定義を変更する必要があります。 MFA にサードパーティ ソリューションを利用しているアカウントでもかまいません。

### <a name="is-active-directory-federation-service-adfs-required-if-i-am-using-a-third-party-solution"></a>サードパーティのソリューションを使用している場合、Active Directory フェデレーション サービス (ADFS) は必要ですか?

いいえ。サードパーティのソリューションを使用している場合は、Active Directory フェデレーション サービス (ADFS) を使用する必要はありません。 ソリューションのベンダーと協力して、ソリューションの要件を決定することをお勧めします。

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>Azure AD のセキュリティの既定値を有効にすることは必須ですか?

いいえ、Azure AD のセキュリティの既定値を有効にすることは必須ではありません。

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>MFA の要件を満たすために条件付きアクセスを使用できますか?

はい、条件付きアクセスを使用して、パートナー テナント内の各ユーザー (サービス アカウントを含む) に MFA を適用できます。 ただし、パートナーには高い特権が付与されている、という点を考えると、すべての単一認証について、MFA チャレンジが各ユーザーに確実に適用されるようにする必要があります。 つまり、MFA の要件を回避する条件付きアクセスの機能は利用できません。

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

コントロール パネルを使用している場合は、セキュア アプリケーション モデル フレームワークの導入について、ベンダーと相談する必要があります。

コントロール パネル ベンダーは、コントロール パネル ベンダーとしてパートナー センターに[オンボード](https://docs.microsoft.com/partner-center/enroll-as-cpv)し、すぐにこの要件の実装を開始する必要があります。 「[パートナー センター: セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。 コントロール パネル ベンダーは、資格情報ではなく CSP パートナーの同意を受け入れて管理し、既存のすべての CSP パートナーの資格情報を消去する必要があります。

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>セキュリティで保護されたアプリケーション モデルは、Partner Center API/SDK に対してのみ実装する必要がありますか?

すべてのユーザー アカウントに対して多要素認証を適用すると、非対話形式での実行を目的とした自動化または統合が影響を受けます。 パートナーのセキュリティ要件では、パートナーは Partner Center API に対してセキュリティで保護されたアプリケーション モデルを有効にする必要がありますが、それを利用して自動化と統合で認証の 2 番目の要素の必要性に対処することができます。 アクセス対象のリソースでは、アクセス トークン ベースの認証がサポートされている必要があることに注意してください。

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>PowerShell などの自動化ツールを使用しています。 セキュリティで保護されたアプリケーション モデルを実装するにはどうすればよいですか?

自動化が、非対話形式で実行され、認証にユーザー資格情報を使用するためである場合は、セキュア アプリケーション モデルを実装する必要があります。 このフレームワークを実装する方法については、[Partner Center PowerShell のセキュリティで保護されたアプリケーション モデル](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5)に関する記事をご覧ください。  すべての自動化ツールでアクセス トークンを使用して認証を行う機能が提供されているわけではないことに注意してください。 どのような変更が必要であるかを理解する上で支援が必要な場合は、[パートナー センター セキュリティ ガイダンス](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) グループにメッセージを投稿してください。 

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>同意プロセスを実行するとき、アプリケーション管理者はどのようなユーザー資格情報を提供する必要がありますか?

最小限の特権のアクセス許可が割り当てられているサービス アカウントを使用することをお勧めします。 Partner Center API に関しては、販売エージェント ロールまたは管理エージェント ロールが割り当てられているアカウントを使用する必要があります。

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>同意プロセスを実行するとき、アプリケーション管理者がグローバル管理者のユーザー資格情報を提供してはならないのはなぜですか?

最小限の特権の ID を使用してリスクを軽減することがベスト プラクティスとして推奨されます。 グローバル管理者特権を持つアカウントを使用することは、必要以上のアクセス権限が付与されることになるため、推奨されません。

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>私は CSP パートナーです。 コントロール パネル ベンダー (CPV) がソリューションの実装作業を行っているかどうかを確認するには、どうすればよいですか?

コントロール パネル ベンダー (CPV) ソリューションを使用してクラウド ソリューション プロバイダー (CSP) プログラムで取引を行っているパートナーは、自分で CPV に問い合わせる必要があります。

### <a name="who-is-a-control-panel-vendor-cpv"></a>コントロール パネル ベンダー (CPV) とは何ですか?

コントロール パネル ベンダーとは、Partner Center API と統合するために CSP パートナーによって使用されるアプリを開発する独立系ソフトウェア ベンダーです。 コントロール パネル ベンダーは、パートナー センター ダッシュボードまたは API に直接アクセスすることができる CSP パートナーではありません。 詳しくは、「[パートナー センター: セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)」を参照してください。

### <a name="i-am-a-cpv-how-do-i-enroll"></a>私は CPV です。 登録するにはどうすればよいですか?

コントロール パネル ベンダー (CPV) として登録するには、[こちら](https://docs.microsoft.com/partner-center/enroll-as-cpv)のガイドラインに従ってください。

登録リンクを受け取るには、CPV は [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) に連絡し、CPV とビジネス上の関係がある、または CPV のビジネスを理解している、Microsoft の従業員スポンサーを指定する必要があります。 たとえば、パートナー開発マネージャー (PDM) などです。

パートナー センターに登録して、使用するアプリケーションを登録すると、Partner Center API にアクセスできるようになります。 初めて CPV になった場合は、パートナー センターの通知を通じてサンドボックスの情報を受け取ります。 Microsoft CPV として登録を完了し、CPV 契約に同意すると、次のことができるようになります。

1. マルチテナント アプリケーションを管理する (Azure portal へのアプリケーションの追加、パートナー センターでのアプリケーションの登録と登録解除)。 注: CPV は、Partner Center API の承認を取得するには、パートナー センターでアプリケーションを登録する必要があります。 Azure portal にアプリケーションを追加するだけでは、CPV アプリケーションはパートナー センター API に対して承認されません。
2. CPV プロファイルを表示および管理する。
3. CPV 機能にアクセスする必要があるユーザーを表示および管理する。 CPV に許される唯一のロールは、グローバル管理者です。

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Partner Center SDK を使用しています。 SDK ではセキュリティで保護されたアプリケーション モデルが自動的に使用されますか?

いいえ。[セキュア アプリケーションモデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)に記載されているガイドラインに従う必要があります。

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-dont-have-mfa-enabled"></a>MFA が有効でないアカウントを使用して、セキュア アプリケーション モデルの更新トークンを生成できますか?

はい。MFA が適用されていないアカウントを使用して、更新トークンを生成できます。 ただし、MFA が有効になっていないアカウントを使用して生成されたトークンでは、MFA の要件によりリソースにアクセスできないため、これは行わないでください。

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>MFA が有効になっている場合、アプリケーションでアクセス トークンを取得するにはどうすればよいですか?

[セキュリティで保護されたアプリケーション モデル ガイド](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)で提供されている、新しいセキュリティ要件に準拠しながらそれを行う方法の詳細に従う必要があります。 .NET のサンプル コードは[こちら](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)に、Java のサンプル コードは[こちら](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)にあります。

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>CPV は、CPV テナントまたは CSP パートナーのテナントのどちらに Azure AD アプリケーションを作成しますか?

CPV は、CPV として登録に関連付けられているテナントに Azure Active Directory アプリケーションを作成する必要があります。

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>アプリのみの認証を使用している CSP です。 何か変更する必要がありますか?

ユーザーの資格情報はアクセス トークンの要求に使用されないため、アプリのみの認証については影響を受けません。 ユーザーの資格情報が共有されている場合は、コントロール パネル ベンダー (CPV) は[セキュリティで保護されたアプリケーション モデル フレームワーク](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)を採用し、所有している既存のパートナー資格情報を消去する必要があります。

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>CPV は、アプリのみの認証スタイルを利用してアクセス トークンを取得できますか?

いいえ。コントロール パネル ベンダー パートナーは、パートナーの代わりに、アプリのみの認証スタイルを利用してアクセス トークンを要求することはできません。 アプリとユーザー認証のスタイルが利用される、セキュリティで保護されたアプリケーション モデルを実装する必要があります。

## <a name="technical-enforcement"></a>技術的な実施

### <a name="what-is-the-activation-of-security-safeguards"></a>セキュリティセーフガードのアクティブ化とは?

クラウド ソリューション プロバイダー (CSP) プログラムに参加するすべてのパートナー、コントロール パネル ベンダー (CPV)、アドバイザーは、準拠を維持し、パートナーのセキュリティ要件を実装する必要があります。

Microsoft では、追加の保護を提供するために、多要素認証 (MFA) の検証を義務づけて不正アクセスを防止し、パートナーがテナントと顧客を保護する上で役立つセキュリティ保護機能のアクティブ化を開始しています。  

すべてのパートナーテナントに対するパートナーの代理管理 (AOBO) 機能のアクティブ化は既に完了しています。 パートナーおよび顧客の保護をさらに支援するために、2020年の第2四半期より、パートナー センターのトランザクションのアクティブ化を開始し、パートナーのビジネスおよび顧客を個人情報盗難関連のインシデントから保護する上でのサポートを提供します。

詳細については、[パートナー テナントに多要素認証 (MFA) を義務付ける](partner-security-requirements-mandating-mfa.md) ページを参照してください。

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>サードパーティの MFA ソリューションを使用していますが、ブロックされます。どうすればよいですか?

リソースにアクセスするアカウントで多要素認証が要求されていることを検証するには、[認証方法参照](https://tools.ietf.org/html/rfc8176)要求を調べて、MFA が一覧に含まれているかどうかを確認します。 サードパーティ ソリューションによっては、この要求が発行されないか、MFA 値が含まれていない場合があります。 要求が存在しない場合、または MFA 値が表示されない場合は、認証対象のアカウントで多要素認証が要求されたかどうかを判断する方法がありません。 サードパーティのソリューションのベンダーと協力して、ソリューションで認証方法参照要求を発行するために実行する必要があるアクションを決定する必要があります。

想定されている要求がサードパーティのソリューションで発行されているかどうか不明な場合は、「[パートナーのセキュリティ要件のテスト](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0)」を参照してください。

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>AOBO を使用した顧客のサポートが MFA によってブロックされます。どうすればよいですか?

パートナーのセキュリティ要件の技術的適用では、認証対象のアカウントで多要素認証が求められたかどうかが確認されます。 要求されなかった場合、ログイン ページにリダイレクトされ、再度認証するように求められます。 エクスペリエンスとガイダンスの詳細については、「[パートナー テナントに多要素認証 (MFA) を義務付ける](partner-security-requirements-mandating-mfa.md#partner-delegated-administration)」のドキュメントを確認してください。 ドメインがフェデレーションされていない場合は、認証が完了した後、多要素認証を設定するように要求されます。 設定が完了すると、AOBO を使用して顧客を管理できるようになります。 ドメインがフェデレーションされている場合は、アカウントに対して多要素認証が求められることを確認する必要があります。

## <a name="security-defaults-transition"></a>セキュリティの既定値の移行

### <a name="how-can-i-transition-from-baseline-policies-to-security-defaults-or-other-mfa-solutions"></a>ベースライン ポリシーからセキュリティの規定値またはその他の MFA ソリューションに移行するにはどうすればよいですか?

Azure Active Directory (Azure AD) [「ベースライン」ポリシーは削除され、パートナーとその顧客のためのより包括的な保護ポリシーである「セキュリティの既定値」](https://docs.microsoft.com/azure/active-directory/fundamentals/whats-new#replacement-of-baseline-policies-with-security-defaults)に置き換えられます。 [セキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) を使用すると、組織を個人情報盗難関連のセキュリティ攻撃から保護する上で役立ちます。

ベースライン ポリシーからセキュリティの既定値のポリシー、または[その他の MFA 実装オプション](partner-security-requirements.md#actions-that-you-need-to-take)に移行していない場合は、ベースラインポリシーの提供終了にり、多要素認証 (MFA) の実装は削除されます。 MFA で保護された操作を実行するパートナー テナントのユーザーは、MFA の検証を完了するように要求されます。 詳細なガイダンスについては、[ここ](partner-security-requirements-mandating-mfa.md)を参照してください。
準拠を維持し、中断を最小限に抑えるには、以下のいずれかの操作を実行します。

- セキュリティの既定値への移行
    - セキュリティの既定ポリシーは、パートナーが MFA を実装する上で選択可能なオプションの1つです。 基本レベルのセキュリティが追加料金なしで有効になります。
    - Azure AD を使用して組織で MFA を有効にする方法と、[セキュリティの規定値に関する重要な考慮事項](partner-security-requirements.md#security-defaults)を確認してください。
    - ビジネス ニーズを満たす場合は、セキュリティの既定ポリシーを有効にします。
- 条件付きアクセスへの移行
    - セキュリティの既定ポリシーでビジネス ニーズに対応できない場合は、条件付きアクセスを有効にします。 詳細については、Azure AD の条件付きアクセスに関するドキュメントを参照してください。

## <a name="key-resources"></a>重要なリソース

### <a name="how-to-get-started"></a>開始する方法

- [パートナーのセキュリティ要件: ステップバイステップ ガイド](https://docs.microsoft.com/partner-center/partner-security-requirements)。
- 質問とフィードバックは、この[パートナー センター セキュリティ ガイダンス グループ](https://aka.ms/MPCSecurityGuidance)にお送りください。
- 今後予定されているパートナーの業務時間とウェビナーに参加してください。 [スケジュールとリソースの詳細](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)については、こちらで確認してください。

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

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>セキュリティで保護されたアプリケーション モデル フレームワークを導入するのに役立つ技術情報とサポートを利用するにはどうすればよいですか?

Azure Active Directory の技術製品サポート オプションを、MPN 特典で利用できます。 アクティブな ASfP または PSfP サブスクリプションにアクセスできるパートナーは、関連付けられているアカウント マネージャー (SAM/TAM) と協力して、使用可能なオプションを最大限に理解することができます。

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>パートナー センターへのアクセスが失われた場合、サポートに問い合わせるにはどうすればよいですか?

「[マイクロソフト パートナー サポート](https://partner.microsoft.com/support)」にアクセスし、 **[すべてのサポート オプションを表示する]** を選択します。 マイクロソフト パートナー サポートに連絡するために使用できるオプションが表示されます。 これには、サポートに電話するための電話番号と、サポートとチャットするためのオプションが含まれます。 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>一般的な技術的問題に関する詳細情報はどこで入手できますか?

一般的な技術的問題に関する情報については、[こちら](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues)を参照してください。
