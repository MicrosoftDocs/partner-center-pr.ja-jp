---
title: パートナーのセキュリティ要件 | パートナー センター
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーにとって必須となった、多要素認証 (MFA) の有効化と、セキュリティで保護されたアプリケーション モデル フレームワークの採用に関する概要。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.openlocfilehash: b0fe328008ae56272ddd8e22722071e5858881c8
ms.sourcegitcommit: 5379fbbe7fab1a26314c42bca40674c7f2faa432
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/27/2020
ms.locfileid: "77672802"
---
# <a name="partner-security-requirements"></a>パートナーのセキュリティ要件

**適用対象**

- クラウド ソリューション プロバイダー プログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのコントロール パネル ベンダー
- すべてのアドバイザー

**該当するユーザー**
-   ゲスト ユーザーを含むすべての有効なユーザー

プライバシーの保護とセキュリティの強化は、マイクロソフトの最優先事項の 1 つです。 最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。 そのために、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。 パートナーと顧客を保護するために、マイクロソフトは、アドバイザー、コントロール パネル ベンダー、およびクラウド ソリューション プロバイダー プログラムに参加しているパートナーを対象とした一連の必須セキュリティ要件を導入しています。

## <a name="overview"></a>概要

パートナーは、パートナー テナントのすべてのユーザー アカウントに対して多要素認証を適用する必要があります。 パートナーのセキュリティ要件に関連する条件は、Microsoft Partner Agreement に追加されています。 アドバイザーについても、同じ契約条件が適用されます。

これらの要件が適用されると、必須のセキュリティ要件を実装していないパートナーは、クラウド ソリューション プロバイダー プログラムで取引したり、代理管理者権限を利用して顧客テナントを管理したりできなくなります。 また、セキュリティ要件を実装していないパートナーは、プログラムへの参加を危険にさらす可能性があります。  

パートナーとその顧客を保護するため、パートナーには次のアクションをすぐに実行するようお願いします。  

1. **パートナー テナント内のすべてのユーザー アカウントに対して多要素認証 (MFA) を有効にします**。 パートナー テナントのすべてのユーザー アカウントは、パートナー センターまたは API を使用して、Microsoft の商用クラウド サービスにサインインするとき、またはクラウド ソリューション プロバイダーで取引を行うときに、多要素認証 (MFA) によるチャレンジを受ける必要があります。 

2. **セキュリティで保護されたアプリケーション モデル フレームワークを採用します**。 セキュリティで保護されたアプリケーション モデル フレームワークを採用します。 Partner Center API と統合しているすべてのパートナーは、すべてのアプリとユーザー認証モデルのアプリケーションに対し、セキュリティで保護されたアプリケーション モデル フレームワークを採用する必要があります。

    > [!IMPORTANT]
    > パートナーには、MFA を適用するときの中断を避けるために、Azure Resource Manager や Microsoft Graph などの Microsoft API との統合、またはユーザー資格情報を使用する PowerShell などの自動化の利用に対し、セキュリティで保護されたアプリケーション モデルを実装することを強くお勧めします。

多要素認証 (MFA) を有効にし、セキュリティで保護されたアプリケーション モデル フレームワークを採用することにより、インフラストラクチャを保護し、ID 盗難や他の不正行為インシデントなどの潜在的なセキュリティ リスクから顧客のデータを保護することができます。  

## <a name="actions-that-you-need-to-take"></a>実行する必要のあるアクション

パートナー セキュリティ要件に準拠するには、パートナー テナント内の各ユーザー アカウントに多要素認証を適用する必要があります。 これは、次のいずれかの方法で実現できます。

- [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)を実装する。

- 各ユーザー アカウントについて Azure Active Directory Premium を購入する。 詳しくは、「[クラウドベースの Azure Multi-Factor Authentication のデプロイの計画](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted)」を参照してください。

- サードパーティ ソリューションを使用して、パートナー テナント内の各ユーザー アカウントに対して多要素認証を適用する。 ソリューションにより予期される情報が確実に提供される方法の詳細については、は、[セキュリティ要件がどのように適用されるか](#how-the-requirements-will-be-enforced)に関するセクションを参照してください。

> [!NOTE]
> ソブリン クラウド (21Vianet、米国政府、ドイツ) では多要素認証は契約上は必須ではありませんが、これらのセキュリティ要件を採用することを強くお勧めします。

## <a name="security-defaults"></a>セキュリティの既定値

セキュリティの既定値ポリシーは、パートナーが、ビジネス ニーズに応じてセキュリティ要件に MFA を実装するために選択することができる[オプション](#actions-that-you-need-to-take)の 1 つです。 基本レベルのセキュリティが追加料金なしで有効になります。 セキュリティの既定値を有効にする前に、Azure AD で組織の MFA を有効にする方法と、以下のキーに関する考慮事項を確認してください。

- ベースライン ポリシーは、今後 2 か月維持された後、2020 年 2 月末に非推奨になります。

- 既にベースライン ポリシーを採用しているパートナーは、セキュリティの既定に移行するための措置を講じる必要があります。

- セキュリティの既定値は、プレビュー版のベースライン ポリシーに置き換わって一般提供されます。 セキュリティの既定値を有効にしたパートナーは、ベースライン ポリシーを有効にすることはできなくなります。

- セキュリティの既定値を使用すると、すべてのポリシーが一度に有効になります。 

- [条件付きアクセス](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-policy-common)を使用しているパートナーの場合、[セキュリティの既定値は使用できません](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)。

- 現時点では、パートナーに対してレガシ認証のブロックは強制されません。 ただし、侵害された ID に関連するほとんどのイベントは、従来の認証を使用したサインインの試行が原因であるため、パートナーにはこれらの古いプロトコルの利用を停止することをお勧めします。

- Azure AD Connect の同期アカウントは、セキュリティの既定値から除外されます。

- 詳細については、「[組織に対して Multi-Factor Authentication を有効にする](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-get-started)」および[Azure Active Directory のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)に関する記事をご覧ください。

> [!NOTE]
> Azure AD のセキュリティの既定値は、簡略化されたベースライン保護ポリシーの発展です。 ベースライン保護ポリシーを既に有効にしている場合は、セキュリティの既定値を有効にすることを強くお勧めします。

ベースライン ポリシーからセキュリティの既定値への移行については、「[セキュリティ既定値とは](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)」をご覧ください。

### <a name="consideration"></a>考慮事項

これらの要件は、パートナー テナントのすべてのユーザー アカウントに適用されるため、パートナーは、多要素認証を実行できない Azure Active Directory 内のユーザー アカウントの識別や、組織で使用されているアプリケーションとデバイスのうち先進認証をサポートしていないものなど、円滑な展開を行うためにいくつかのことを考慮する必要があります。

アクションを実行する前に、次の点について確認することをお勧めします 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>先進認証の使用をサポートしていないアプリケーションまたはデバイスはありますか。

IMAP、POP3、SMTP などのプロトコルを使用する以前の多要素認証を適用している場合はブロックされます。これらのプロトコルでは多要素認証がサポートされていないためです。 この制限に対処するには、[アプリ パスワード](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)と呼ばれる機能を使用します。これにより、アプリケーションまたはデバイスを引き続き認証することができます。 [こちら](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)に記載されているアプリ パスワード使用時の考慮事項を確認し、お使いの環境でアプリ パスワードを使用できるかどうかを確かめる必要があります。

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>パートナー テナントに関連付けられたライセンスによって提供される Office 365 を使用しているユーザーがいますか。

ソリューションを実装する前に、パートナー テナントのユーザーによって使用されている Microsoft Office のバージョンを確認することをお勧めします。 アクションを実行する前に、[Office 365 デプロイの多要素認証の計画](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa)に関するトピックをご覧ください。 Outlook などのアプリケーションで接続の問題が発生する可能性があります。 多要素認証を適用する前に、Outlook 2013 SP1 以降が使用され、組織で先進認証が有効になっていることを確認することが重要です。 詳細については、「[Exchange Online で先進認証を有効にする](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)」を参照してください。

Windows が実行され、Microsoft Office 2013 がインストールされているデバイスで先進認証を有効にするには、2 つのレジストリ キーを作成する必要があります。 「[Windows デバイスで Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>作業中にユーザーによるモバイル デバイスの使用を禁止するポリシーがありますか。

実装する多要素認証ソリューションは、作業中に従業員がモバイル デバイスを使用できないようにする会社のポリシーの影響を受けるため、そのポリシーを特定することが重要です。 [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)の実装を通じて提供されるソリューションなど、確認の目的でのみ認証アプリの使用を許可するソリューションがあります。 モバイル デバイスの使用を禁止するポリシーが組織で採用されている場合は、次のいずれかのオプションを検討する必要があります

- セキュリティで保護されたシステムで実行できる、時間ベースのワンタイム ベース パスワード (TOTP) アプリケーションをデプロイする

- 最適な検証オプションを提供するパートナー テナントの各ユーザー アカウントに対して、多要素認証を適用するサードパーティのソリューションを実装する

- 影響を受けるユーザーに対して [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) ライセンスを購入する

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>どの自動化または統合で、認証にユーザー資格情報が使用されていますか。

パートナー ディレクトリの各ユーザー (サービス アカウントを含む) に MFA を適用する必要があるため、認証にユーザー資格情報が使用されているすべての自動化または統合が影響を受けます。 このため、これらの状況で使用されているアカウントを特定することが重要です。 考慮する必要があるアプリケーションまたはサービスの例をいくつか次に示します

- 顧客に代わってリソースをプロビジョニングするときに使用されるコントロール パネル 

- 顧客への請求 (CSP プログラムに関連する場合) および顧客サポートに使用される任意のプラットフォームとの統合

- Az、AzureRM、Azure AD、MS Online などのモジュールが利用される PowerShell スクリプト

上記のリストはすべてを網羅しているわけではありません。 そのため、認証にユーザー資格情報が利用されるご自身の環境で、アプリケーションまたはサービスの完全な評価を実行することが重要です。 多要素認証の要件に対応するには、可能な限り、[セキュリティで保護されたアプリケーション モデル フレームワーク](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)でガイダンスを実装する必要があります。

## <a name="accessing-your-environment"></a>環境を評価する

多要素認証のチャレンジを受けないで何が、または誰が認証を行っているかを詳しく理解するには、サインイン アクティビティを確認することをお勧めします。 Azure Active Directory Premium では、サインイン レポートを利用できます。 詳細については、「[Azure Active Directory ポータルのサインイン アクティビティ レポート](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)」をご覧ください。 Azure Active Directory Premium がない場合、または PowerShell を使用してこれを取得する方法を探している場合は、[パートナー センターの PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) モジュールから、[Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) コマンドレットを利用する必要があります。

## <a name="how-the-requirements-will-be-enforced"></a>要件はどのように適用されるか

パートナーのセキュリティ要件は、Azure Active Directory により (その後、パートナー センターにより) MFA 要求があるかどうかが確認され、多要素認証の検証が実行済みであることが特定されることで、適用されます。 2019 年 11 月 18 日以降、パートナーのテナントに対する追加のセキュリティ保護 (以前の "技術的適用") がアクティブ化されます。 

アクティブ化されると、パートナー テナントのユーザーは、代理管理者 (AOBO) 操作を実行するときに、多要素認証 (MFA) の検証を完了するように要求されます。 今後も引き続き追加のシナリオとユーザー ロールに対するセキュリティ保護の範囲の拡張が行われ、パートナーには事前に通知を提供します。 詳細については、頻繁に更新されるこのドキュメントを参照してください。 要件を満たしていないパートナーは、ビジネスの中断を回避するため、できるだけ早くこれらの手段を実装する必要があります。 

Azure Multi-Factor Authentication または Azure AD のセキュリティの既定値を使用している場合は、追加のアクションを実行する必要はありません。

サードパーティの多要素認証ソリューションを使用する場合、MFA 要求が発行されない可能性があります。 この要求がないと、Azure Active Directory は、認証要求が多要素認証によってチャレンジされたかどうかを判断できません。 想定されている要求がソリューションで発行されていることを検証する方法の詳細については、「[パートナーのセキュリティ要件のテスト](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements)」を参照してください。 

> [!IMPORTANT]
> 想定されている要求がサードパーティ ソリューションによって発行されない場合は、ソリューションを開発したベンダーと協力して、どのようなアクションを実行する必要があるかを判断する必要があります。

## <a name="resources-and-support"></a>リソースとサポート

サポートとサンプル コードに関するリソースは、次のとおりです。

- [パートナー センター セキュリティ ガイダンス グループコ ミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): 今後のイベントを確認できるオンライン コミュニティです。このコミュニティでは、不明点について質問することもできます。
- [パートナー センターの .NET サンプル](https://github.com/microsoft/partner-center-dotnet-samples): この GitHub リポジトリには、セキュリティで保護されたアプリケーション モデル フレームワークを実装する方法を示す、.NET を使用して開発されたサンプルが含まれています。
- [パートナー センターの Java サンプル](https://github.com/microsoft/partner-center-java-samples): この GitHub リポジトリには、セキュリティで保護されたアプリケーション モデル フレームワークを実装する方法を示す、Java を使用して開発されたサンプルが含まれています。
- [パートナー センターの PowerShell - 多要素認証](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth) - この記事では、セキュリティで保護されたアプリケーション モデル フレームワークを、PowerShell を使用して実装する方法を詳しく説明しています。
