---
title: パートナーのセキュリティ要件
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 多要素認証 (MFA) を有効にして、セキュア アプリケーション モデル フレームワークを採用するためのパートナーのセキュリティ要件を紹介します。
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087061"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>パートナー センターまたはパートナー センター API を使用するためのパートナーのセキュリティ要件

**適切なロール**

- すべてのパートナー センター ユーザー

この記事では、クラウド ソリューション プロバイダー プログラムに参加しているアドバイザー、コントロール パネル ベンダー、パートナーに必須のセキュリティ要件に加え、認証オプションやその他のセキュリティに関する考慮事項について説明します。 プライバシーの保護とセキュリティは、Microsoft の最優先事項の 1 つです。 最善の防御とは予防することで、私たちの強さが、最も弱いリンクと同程度でしかないことはわかっています。 そのために、エコシステムの全員が行動し、適切なセキュリティ保護を確保する必要があるのです。

## <a name="mandatory-security-requirements"></a>必須のセキュリティ要件

必須のセキュリティ要件を実装していないパートナーは、クラウド ソリューション プロバイダー プログラムで取引したり、代理管理者権限を使用して顧客テナントを管理したりできなくなります。 また、セキュリティ要件を実装していないパートナーは、プログラムへの参加を危険にさらす可能性があります。 パートナーのセキュリティ要件に関連する条件は、Microsoft Partner Agreement に追加されています。 アドバイザーについても、同じ契約条件が適用されます。

パートナーとその顧客を保護するため、パートナーには次のアクションをすぐに実行するようお願いします。  

1. **パートナー テナント内のすべてのユーザー アカウントに対して多要素認証 (MFA) を有効にします**。 パートナー テナント内のすべてのユーザー アカウントに対して MFA を強制する必要があります。 ユーザーは、パートナー センターまたは API を使用して Microsoft の商用クラウド サービスにサインインするとき、またはクラウド ソリューション プロバイダー プログラムで取引を行うときに、多要素認証 (MFA) によるチャレンジを受ける必要があります。

2. **セキュリティで保護されたアプリケーション モデル フレームワークを採用します**。 パートナー センター API と統合しているすべてのパートナーは、すべてのアプリとユーザー認証モデルのアプリケーションに対して[セキュア アプリケーション モデル フレームワーク](/partner-center/develop/enable-secure-app-model)を採用する必要があります。

    > [!IMPORTANT]
    > パートナーには、MFA を強制するときの中断を避ける目的で、Azure Resource Manager や Microsoft Graph などの Microsoft API と統合するために、またはユーザー資格情報を使用する PowerShell などの自動化を利用する際に、セキュア アプリケーション モデルを実装することを強くお勧めします。

これらのセキュリティ要件は、お客様のインフラストラクチャを保護し、ID の盗難やその他の不正行為インシデントなどの潜在的なセキュリティ リスクから顧客のデータを保護するのに役立ちます。  

## <a name="implementing-multi-factor-authentication"></a>多要素認証の実装

パートナー セキュリティ要件に準拠するには、パートナー テナント内の各ユーザー アカウントに MFA を実装して強制する必要があります。 この操作は次のいずれかの方法で行うことができます。

- [Azure Active Directory (Azure AD) のセキュリティの既定値群](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)を実装する。 詳細については、[次のセクション](#security-defaults)をご覧ください。

- 各ユーザー アカウントについて Azure Active Directory Premium を購入する。 詳しくは、「[Azure AD Multi-Factor Authentication のデプロイを計画する](/azure/active-directory/authentication/howto-mfa-getstarted)」をご覧ください。

- サード パーティのソリューションを使用してパートナー テナント内の各ユーザー アカウントに対して MFA を強制する。 ソリューションが期待されるソリューションを確実に提供できるようにするには、[セキュリティ要件がどのように適用されるか](#how-the-requirements-are-enforced)に関するセクションを参照してください。

> [!NOTE]
> ソブリン クラウド (米国政府およびドイツ) の場合、多要素認証は契約上必須ではありませんが、これらのセキュリティ要件を採用することを強くお勧めします。

### <a name="security-defaults"></a>セキュリティの既定値

MFA 要件を実装するためにパートナーが選択可能なオプションの 1 つは、Azure AD でセキュリティの既定値群を有効にすることです。 セキュリティの既定値群では、基本レベルのセキュリティが追加料金なしで提供されます。 セキュリティの既定値群を有効にする前に、Azure AD で組織の MFA を有効にする方法と、以下の重要な考慮事項を確認してください。

- 既にベースライン ポリシーを採用しているパートナーは、セキュリティの既定に移行するための措置を講じる必要があります。

- セキュリティの既定値は、プレビュー版のベースライン ポリシーに置き換わって一般提供されます。 セキュリティの既定値を有効にしたパートナーは、ベースライン ポリシーを有効にすることはできなくなります。

- セキュリティの既定値を使用すると、すべてのポリシーが一度に有効になります。

- [条件付きアクセス](/azure/active-directory/conditional-access/concept-conditional-access-policy-common)を使用しているパートナーの場合、[セキュリティの既定値は使用できません](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults)。

- 現時点では、レガシ認証はブロックされません。 ただし、セキュリティ侵害を受けた ID に関連するほとんどのイベントは、レガシ認証を使用したサインインの試行が原因であるため、パートナーにはこれらの古いプロトコルの利用を停止することをお勧めします。

- Azure AD Connect の同期アカウントは、セキュリティの既定値から除外されます。

詳細については、「[組織での Azure AD Multi-Factor Authentication の概要](/azure/active-directory/authentication/concept-mfa-get-started)」および「[セキュリティの既定値群とは](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)」をご覧ください。

> [!NOTE]
> Azure AD のセキュリティの既定値は、簡略化されたベースライン保護ポリシーの発展です。 ベースライン保護ポリシーを既に有効にしている場合は、[セキュリティの既定値群](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)を有効にすることを強くお勧めします。

## <a name="implementation-considerations"></a>実装時の注意事項

これらの要件はパートナー テナント内のすべてのユーザー アカウントに適用されるため、円滑なデプロイを実現するにはいくつかの点を考慮する必要があります。 たとえば、Azure AD 内で MFA を実行できないユーザー アカウントを特定したり、組織内で先進認証に対応していないアプリケーションとデバイスを特定したりします。

アクションを実行する前に、以下の検証を行うことをお勧めします。 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>先進認証の使用をサポートしていないアプリケーションまたはデバイスはありますか。

IMAP、POP3、SMTP、その他のプロトコルでは MFA がサポートされていないため、MFA 認証を強制すると、これらを使用するレガシ認証がブロックされます。 この制限に対処するために、[アプリ パスワード](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords)機能を使用すれば、アプリケーションまたはデバイスを引き続き認証することができます。 [アプリ パスワード使用時の考慮事項](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords)を確認し、お使いの環境でそれを使用できるかどうかを確かめる必要があります。

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>パートナー テナントに関連付けられたライセンスを持つ Office 365 ユーザーがいますか。

ソリューションを実装する前に、パートナー テナントの Microsoft Office ユーザーがどのバージョンを使用しているか確認することをお勧めします。 Outlook などのアプリケーションで接続の問題が発生する可能性があります。 MFA を適用する前に、Outlook 2013 SP1 以降が使用されており、組織で先進認証が有効になっていることを確認することが重要です。 詳細については、[Exchange Online での先進認証の有効化](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online)に関するページをご覧ください。 

Windows が実行され、Microsoft Office 2013 がインストールされているデバイスで先進認証を有効にするには、2 つのレジストリ キーを作成する必要があります。 「[Windows デバイスで Office 2013 の先進認証を有効にする](/office365/admin/security-and-compliance/enable-modern-authentication)」を参照してください。

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>作業中にユーザーによるモバイル デバイスの使用を禁止するポリシーがありますか。

実装する MFA ソリューションは、作業中に従業員がモバイル デバイスを使用できないようにする会社のポリシーの影響を受けるため、そのポリシーを特定することが重要です。 [Azure AD のセキュリティの既定値](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)の実装を通じて提供されるソリューションなど、確認の目的でのみ認証アプリの使用を許可するソリューションがあります。 モバイル デバイスの使用を禁止するポリシーが組織で採用されている場合は、次のいずれかのオプションを検討してください。

- セキュリティで保護されたシステムで実行できる、時間ベースのワンタイム ベース パスワード (TOTP) アプリケーションをデプロイする。

- パートナー テナントの各ユーザー アカウントに MFA を強制するサード パーティのソリューションを実装し、最適な検証オプションを提供する。

- 影響を受けるユーザーに対して [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) ライセンスを購入する。

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>どの自動化または統合で、認証にユーザー資格情報が使用されていますか。

MFA の強制は、サービス アカウントを含め、パートナー ディレクトリ内の各ユーザーに及ぶため、認証にユーザー資格情報が使用されているすべての自動化または統合が影響を受けます。 このため、これらの状況でどのアカウントが使用されているかを特定することが重要です。 検討すべきアプリケーションやサービスの例についての次の一覧を確認してください。

- 顧客に代わってリソースをプロビジョニングするときに使用されるコントロール パネル

- 顧客への請求 (CSP プログラムに関連する場合) および顧客サポートに使用される任意のプラットフォームとの統合

- Az、AzureRM、Azure AD、MS Online、その他のモジュールが使用される PowerShell スクリプト

上記のリストはすべてを網羅しているわけではありません。 そのため、認証にユーザー資格情報が使用されるご自身の環境で、アプリケーションまたはサービスの完全な評価を実行することが重要です。 MFA の要件に対応するには、可能な限り、[セキュリティで保護されたアプリケーション モデル フレームワーク](/partner-center/develop/enable-secure-app-model)でガイダンスを実装する必要があります。

## <a name="accessing-your-environment"></a>環境を評価する

MFA のチャレンジを受けないで何が、または誰が認証を行っているかを詳しく理解するには、サインイン アクティビティを確認することをお勧めします。 Azure Active Directory Premium では、サインイン レポートを使用できます。 この件に関する詳細は、「[Azure Active Directory ポータルのサインイン アクティビティ レポート](/azure/active-directory/reports-monitoring/concept-sign-ins)」をご覧ください。 Azure Active Directory Premium がない場合、または PowerShell を使用してこのサインイン アクティビティを実現する方法を探している場合は、[パートナー センターの PowerShell](https://www.powershellgallery.com/packages/PartnerCenter/) モジュールから [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) コマンドレットを使用する必要があります。

## <a name="how-the-requirements-are-enforced"></a>要件はどのように適用されるか

パートナーのセキュリティ要件は、Azure AD により (その後、パートナー センターにより) MFA クレームがあるかどうかが確認され、MFA 検証が実行済みであることが特定されることで、強制されます。 2019 年 11 月 18 日以降、パートナーのテナントに対する追加のセキュリティ セーフガード (以前の "技術的適用") がアクティブ化されています。

このアクティブ化に伴い、パートナー テナントのユーザーは、代理管理者 (AOBO) 操作を実行するとき、パートナー センター ポータルにアクセスするとき、またはパートナー センター API を呼び出すときに、MFA 検証を完了するように要求されます。 詳細については、「[パートナー テナントに多要素認証 (MFA) を義務付ける](partner-security-requirements-mandating-mfa.md)」をご覧ください。 

要件を満たしていないパートナーは、ビジネスの中断を回避するため、できるだけ早くこれらの手段を実装する必要があります。 Azure Active Directory Multi-Factor Authentication または Azure AD のセキュリティの既定値群を使用している場合は、追加のアクションを実行する必要はありません。

サード パーティの MFA ソリューションを使用している場合は、MFA クレームが発行されない可能性があります。 このクレームがないと、Azure AD は、認証要求が MFA によってチャレンジされたかどうかを判断できません。 想定されている要求がソリューションで発行されていることを検証する方法の詳細については、「[パートナーのセキュリティ要件のテスト](/powershell/partnercenter/test-partner-security-requirements)」を参照してください。 

> [!IMPORTANT]
> 想定されている要求がサードパーティ ソリューションによって発行されない場合は、ソリューションを開発したベンダーと協力して、どのようなアクションを実行する必要があるかを判断する必要があります。

## <a name="resources-and-samples"></a>リソースとサンプル

サポートやサンプル コードについては、次のリソースを参照してください。

- [パートナー センター セキュリティ ガイダンス グループ コミュニティ](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance):パートナー センター セキュリティ ガイダンス グループ コミュニティは、今後のイベントを確認でき、不明点について質問することもできるオンライン コミュニティです。
- [パートナー センターの .NET のサンプル](https://github.com/microsoft/partner-center-dotnet-samples):この GitHub リポジトリには、セキュア アプリケーション モデル フレームワークを実装する方法を示す、.NET を使用して開発されたサンプルが含まれています。
- [パートナー センターの Java のサンプル](https://github.com/microsoft/partner-center-java-samples):この GitHub リポジトリには、セキュア アプリケーション モデル フレームワークを実装する方法を示す、Java を使用して開発されたサンプルが含まれています。
- [Partner Center PowerShell - 多要素認証](/powershell/partnercenter/multi-factor-auth):この多要素認証に関する記事では、セキュア アプリケーション モデル フレームワークを、PowerShell を使用して実装する方法を詳しく説明しています。

## <a name="next-steps"></a>次のステップ

- [パートナー テナントに多要素認証 (MFA) を義務付ける](partner-security-requirements-mandating-mfa.md)