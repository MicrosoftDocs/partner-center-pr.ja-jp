---
title: パートナーテナントに MFA を義務付ける |パートナーセンター
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーテナントの MFA を義務付けることで、顧客リソースへのアクセスをセキュリティで保護する方法について説明します。 サンプルシナリオが含まれます。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: f0beb695bee9a67f79373ea903158de3fbb66851
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943105"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>パートナーのテナントに Multi-factor Authentication (MFA) を義務付ける

**適用対象**

- クラウド ソリューション プロバイダー プログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのアドバイザー

これらのパートナーは、次の領域の MFA 検証を完了する必要があります。

- [パートナーセンターダッシュボード](#partner-center-dashboard)(H1 CY2020 を対象とする)
- [パートナーセンター API](#partner-center-api) (ターゲット H1 CY2020)
- [パートナー代理管理](#partner-delegated-administration)(2019 年11月18日以降)

この機能の目的は、パートナーが資格情報の侵害から顧客リソースへのアクセスをセキュリティで保護できるようにすることです。

## <a name="partner-center-dashboard"></a>パートナーセンターのダッシュボード
パートナーセンターダッシュボードの特定のページは、次のような MFA で保護されます。

* **[Customers]** タブのすべてのページ。
* **[サポート > 顧客要求]** タブのすべてのページ。

これらのページのいずれかにアクセスしようとしたときに、以前に MFA の検証を完了していない場合は、これを行う必要があります。

次のユーザーの種類は、これらの MFA で保護されたページにアクセスする権限を持っているため、この機能の影響を受けます。次に例を示します。

* 管理エージェント
* 販売担当者
* ヘルプデスクエージェント

このしくみを説明するために、次の2つの例を考えてみます。

**例 1: パートナーが MFA Azure AD 実装している**
1.  加藤さんは、CSP Contoso に勤務しています。 Contoso は Azure AD MFA を使用して Contoso partner テナントのすべてのユーザーに MFA を実装しています。
2.  自分のワークステーションから、加藤さんは新しいブラウザーセッションを開始し、パートナーセンターのダッシュボードの [概要] ページに移動します (これは MFA で保護されていません)。 パートナーセンターは Jane を Azure AD サインインにリダイレクトします。
3.  Contoso によって Azure AD MFA が既に設定されているため、MFA の検証を完了するには Jane が必要です。 サインインと MFA の検証に成功すると、Jane がパートナーセンターのダッシュボードの [概要] ページにリダイレクトされます。
4.  加藤さんは、パートナーセンターで MFA で保護されたページのいずれかにアクセスしようとします。 前にサインインしたときに、加藤さんは既に MFA の検証を完了しているため、加藤さんは mfa で保護されたページにアクセスできます。 MFA の検証を再度行う必要はありません。

**例 2: パートナーが id フェデレーションを使用してサードパーティの MFA を実装している**
1. Trent は CSP Wingtip で動作します。 Wingtip は、id フェデレーションを介して Azure AD と統合されたサードパーティの MFA を使用して、Wingtip partner テナントのすべてのユーザーに MFA を実装しました。
2. このワークステーションから、Trent は新しいブラウザーセッションを開始し、パートナーセンターのダッシュボードの [概要] ページに移動します (これは MFA で保護されていません)。 パートナーセンターは、Justin を Azure AD にリダイレクトしてサインインします。
3. Wingtip が id フェデレーションを設定しているため、Azure AD は Trent をフェデレーション id プロバイダーにリダイレクトして、サインインと MFA の検証を完了します。 サインインと MFA の検証に成功すると、Trent が Azure AD にリダイレクトされ、パートナーセンターのダッシュボードの概要ページにリダイレクトされます。
4. Justin は、パートナーセンターで MFA で保護されたページのいずれかにアクセスしようとします。 以前のサインインでは、Trent は既に MFA の検証を完了しているため、Trent は mfa の検証を再度実行する必要なく、MFA で保護されたページにアクセスできます。

**例 3: パートナーが MFA を実装していない**
1. John は CSP Fabrikam に勤務しています。 Fabrikam は、Fabrikam パートナーのテナント下にあるすべてのユーザーに対して MFA を実装していません。
2. 彼のワークステーションから、John は新しいブラウザーセッションを開始し、パートナーセンターのダッシュボードの [概要] ページに移動します (これは MFA で保護されていません)。 パートナーセンターは John を Azure AD サインインにリダイレクトします。
3. Fabrikam は MFA を実装していないため、MFA の検証を完了するために John は必要ありません。 サインインに成功すると、John はパートナーセンターのダッシュボードの概要ページにリダイレクトされます。
4. John は、パートナーセンターで MFA で保護されたページのいずれかにアクセスしようとします。 John は MFA の検証を完了していないため、パートナーセンターは John を Azure AD にリダイレクトして、MFA の検証を完了します。 これは、初めて MFA を完了する必要があるため、John は Microsoft Authenticator アプリを使用して MFA に登録するように要求されます。 MFA の登録と MFA の検証が成功すると、John は MFA で保護されたページにアクセスできるようになります。

## <a name="partner-center-api"></a>パートナーセンター API

パートナーセンター API は、アプリのみの認証と、アプリとユーザーの認証の両方をサポートしています。 アプリ + ユーザー認証を使用する場合、パートナーセンターは MFA の検証を必要とします。 具体的には、パートナーアプリケーションがパートナーセンターに API 要求を送信する場合、要求の Authorization ヘッダーにアクセストークンを含める必要があります。 パートナーセンターが、App + User 認証を使用して取得されたアクセストークンを使用して API 要求を受信すると、パートナーセンター API は*認証方法参照 (AMR)* 要求に*MFA*値が存在するかどうかを確認します。 JWT デコーダーを使用して、アクセストークンに予期される認証方法参照 (AMR) 値が含まれているかどうかを検証できます。

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

この値が存在する場合、パートナーセンターは MFA の検証が完了したことを確認し、API 要求を処理します。 この値が存在しない場合、パートナーセンター API は次の応答で要求を拒否します。

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>パートナー代理管理

### <a name="using-service-portals"></a>サービスポータルの使用

管理エージェントやヘルプデスクエージェントなどのパートナーアカウントは、パートナーが委任した管理者特権を使用して、Microsoft Online Services ポータル、コマンドラインインターフェイス (CLI)、Api (アプリ + ユーザー認証を使用) を介して顧客リソースを管理できます。

パートナーの委任された管理者特権を使用して顧客のリソースを管理している Microsoft Online Services ポータルにアクセスする場合、これらのポータルの多くでは、パートナーアカウントが対話形式で認証される必要があります。顧客 Azure Active Directory テナントはに設定されます。認証コンテキスト-顧客テナントにサインインするには、パートナーアカウントが必要です。

Azure Active Directory がこのような認証要求を受信すると、MFA の検証を完了するためにパートナーアカウントが必要になります。 パートナーアカウントが管理対象 id であるか、フェデレーション id であるかに応じて、2つのユーザーエクスペリエンスが考えられます。

- パートナーアカウントが**管理対象**id である場合、Azure Active Directory は、ユーザーに対して MFA の検証を完了するように求めるメッセージを表示します。 パートナーアカウントが Azure Active Directory 前に MFA に登録されていない場合、ユーザーは最初に[mfa 登録を完了](#mfa-registration-experience)するように求められます。

- パートナーアカウントが**フェデレーション**id の場合、このエクスペリエンスは、パートナー管理者が Azure Active Directory でフェデレーションを構成した方法によって異なります。 Azure Active Directory でフェデレーションを設定する場合、パートナー管理者は、フェデレーション id プロバイダーが MFA をサポートしているかどうかを Azure Active Directory ことを示すことができます。 その場合、Azure Active Directory は、ユーザーをフェデレーション id プロバイダーにリダイレクトして、MFA の検証を完了します。 それ以外の場合、Azure Active Directory は、ユーザーに MFA の検証を完了するように求めるメッセージを表示します。 パートナーアカウントが Azure Active Directory 前に MFA に登録されていない場合、ユーザーは最初に[mfa 登録を完了](#mfa-registration-experience)するように求められます。

全体的なエクスペリエンスは、エンドカスタマーテナントが管理者に対して MFA を実装しているシナリオと非常によく似ています。 たとえば、顧客テナントは、管理者エージェントやヘルプデスクエージェントなどの MFA 検証を使用して顧客テナントにサインインするために管理者権限を持つすべてのアカウントを必要とする、管理者[向けの Azure AD 基準ポリシー-mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)を有効にしました。 テストの目的で、パートナーは顧客テナントで[管理者ポリシーの MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)を有効にし、パートナーの代理管理特権を使用して顧客のテナントにアクセスすることができます。

> [!NOTE]
> パートナーが代理管理者権限を使用して顧客のリソースにアクセスする場合、すべての Microsoft Online Service ポータルで顧客テナントへのサインインにパートナーアカウントが必要であるとは限りません。 代わりに、パートナーのテナントにサインインするために必要なのはパートナーアカウントだけです。 例として、Exchange 管理センターがあります。 時間の経過と共に、パートナーの代理管理者特権を使用する場合、これらのポータルでは、顧客テナントへのサインインにパートナーアカウントが必要であると想定しています。

### <a name="using-service-apis"></a>サービス Api の使用
一部の Microsoft Online Services Api (Azure Resource Manager、Azure AD Graph、Microsoft Graph など) は、パートナー代理の管理者特権を使用して顧客のリソースをプログラムで管理するパートナーをサポートしています。 これらの Api を使用してパートナーの委任された管理者特権を活用するには、パートナーアプリケーションで API 要求の Authorization ヘッダーにアクセストークンを含める必要があります。この場合、アクセストークンは、Azure AD で認証するパートナーユーザーアカウントを持つことによって取得されます。顧客 Azure AD 認証コンテキストとして設定されます。 パートナーアプリケーションでは、パートナーのユーザーアカウントを顧客テナントにサインインさせる必要があります。

認証要求などの Azure AD 受信する場合、Azure AD は、パートナーユーザーアカウントに MFA の検証を完了させる必要があります。 パートナーユーザーアカウントが以前に MFA に登録されていない場合、ユーザーアカウントはまず MFA 登録を完了するように求められます。

パートナーが代理管理者権限を使用してこれらの Api と統合されているすべてのパートナーアプリケーションは、この機能の影響を受けます。 パートナーアプリケーションが中断せずにこれらの Api を引き続き使用できるようにするには、次の手順を実行します。

- パートナーは、アクセストークンを取得するために、Azure AD で非対話型のユーザー認証方法を使用しないようにする必要があります。 [パスワードフロー](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)など、非対話型のユーザー認証方法を使用する場合、Azure AD は、ユーザーに MFA の検証を完了するように要求することはできません。 パートナーは、代わりに[OpenID connect flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code)などの対話型ユーザー認証方法を使用するように切り替える必要があります。
- 対話ユーザーの認証方法では、パートナーは既に MFA に対して有効になっているパートナーユーザーアカウントを使用する必要があります。 また、Azure AD によってメッセージが表示された場合、パートナーはサインイン時に MFA の登録と MFA の検証を完了できます。
- これは、エンドカスタマーテナントが管理者に対して MFA を実装しているシナリオとよく似ています。 たとえば、顧客テナントは、管理者エージェントやヘルプデスクエージェントなどの MFA 検証を使用して顧客テナントにサインインするために管理者権限を持つすべてのユーザーアカウントを必要とする、管理者[向けの Azure AD 基準ポリシー-mfa](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)を有効にしました。 テストの目的で、パートナーは顧客テナントの[管理者ポリシーに対して MFA](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators)を有効にし、パートナーの代理管理特権を使用して顧客のテナントにプログラムでアクセスすることができます。

### <a name="mfa-registration-experience"></a>MFA の登録エクスペリエンス
MFA の検証中に、パートナーアカウントが MFA に登録されていない場合は、まず、ユーザーに MFA の登録を完了するように求めるメッセージが表示さ Azure AD ます。

![MFA 登録手順1](images/MfaRegistration1.png)

**[次へ]** をクリックすると、ユーザーは確認方法の一覧 (電話、SMS、認証アプリなど) を選択するように求められます。

![MFA 登録手順2](images/MfaRegistration2.png)

正常に登録されると、ユーザーが選択した認証に基づいて MFA の検証を完了するように求められます。



## <a name="request-for-technical-exception"></a>技術的な例外の要求

パートナーは、Microsoft Online Services の技術的な問題が発生していて、解決策や回避策がない場合に、MFA の検証を抑制するために技術的な例外を適用できます。 この作業を行う前に、次のセクションを確認してください。

 - [パートナーによって報告される一般的な問題の一覧](#list-of-common-issues-reported-by-partners)
 - [技術的な例外の要求を送信する方法](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>パートナーによって報告される一般的な問題の一覧
技術的な例外を適用する前に、他のパートナーによって報告された一般的な問題の一覧を確認して、それらが技術的な例外の有効な理由であるかどうかを把握してください。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>問題 1: パートナーエージェントに対して MFA を実装するには、より多くの時間が必要です。
パートナーがお客様のリソースを管理するためにパートナーの代理管理特権を使用して Microsoft Online Services ポータルへのアクセスを必要とするパートナーエージェントに対して、パートナーが開始していないか、まだ MFA を実装しています。 パートナーは、MFA の実装を完了するためにより多くの時間を必要とします。 これは、技術的な例外の有効な理由ですか。

**回答**: いいえ。 パートナーは、中断を回避するために、ユーザーのために MFA を実装する必要があります。

> [!NOTE]
> パートナーがパートナーエージェント用に MFA を実装していない場合でも、パートナーエージェントは、MFA の登録と MFA の検証を完了できる限り、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。カスタマーテナントへのサインイン時にメッセージが表示されます。 MFA の登録を完了しても、ユーザーが MFA に対して自動的に有効になることはありません。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>問題 2: パートナーが、委任された管理者特権を使用していないユーザーアカウントに MFA を実装していない
パートナーはパートナーのテナントに、パートナーの代理管理特権を使用して顧客のリソースを管理するために Microsoft Online Services ポータルへのアクセスを必要としないユーザーがいます。 パートナーは、これらのユーザーに対して MFA を実装するプロセスであり、完了するまでにより多くの時間が必要になります。 これは、技術的な例外の有効な理由ですか。

**回答**: いいえ。 これらのユーザーアカウントは、顧客のリソースを管理するためにパートナーの委任された管理特権を使用しないため、顧客のテナントにサインインする必要はありません。 顧客テナントへのサインイン時に MFA の検証を必要とする Azure AD の影響を受けません。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>問題 3: パートナーがユーザーサービスアカウント用に MFA を実装していない
パートナーのパートナーテナントには、サービスアカウントとしてデバイスで使用されているいくつかのユーザーアカウントがあります。 これらは一般に低特権のアカウントであり、パートナーの代理管理権限を使用して顧客のリソースを管理するために、パートナーセンターや Microsoft Online Services ポータルにアクセスする必要はありません。 これは、技術的な例外の有効な理由ですか。

**回答**: いいえ。 これらのユーザーアカウントは、顧客のリソースを管理するためにパートナーの委任された管理特権を使用しないため、顧客のテナントにサインインする必要はありません。 顧客テナントへのサインイン時に MFA の検証を必要とする Azure AD の影響を受けません。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>問題 4: パートナーが MS Authenticator アプリを使用して MFA を実装できない
パートナーには "クリーンデスク" ポリシーがあり、従業員が自分の個人のモバイルデバイスを作業領域に持ち込むことは許可されていません。 個人のモバイルデバイスにアクセスできない場合、従業員は MS Authenticator アプリをインストールできません。これは、Azure AD 基準ポリシーでサポートされている唯一の MFA 検証です。 これは、技術的な例外の有効な理由ですか。

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 パートナーは、パートナーセンターにアクセスするときに、従業員が引き続き MFA 検証を完了できるように、次の代替手段を検討する必要があります。
- MS Authenticator アプリ以外の Azure AD ベースラインポリシーは、サードパーティの互換性のある Authenticator アプリでも使用できます。これは、Microsoft Windows を実行している Windows コンピューターでサポートされている可能性があります。
- また、パートナーは Azure AD Premium またはサードパーティの MFA ソリューション (Azure AD と互換性がある) にサインアップすることもできます。これにより、追加の検証方法を提供できます。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>問題 5: レガシ認証プロトコルが使用されているため、パートナーは MFA を実装できません
パートナーには、まだ MFA と互換性のない従来の認証プロトコルを使用しているパートナーエージェントがあります。 たとえば、ユーザーが従来の認証プロトコルに基づく Outlook 2010 を引き続き使用しているとします。 これらのパートナーエージェントの MFA を有効にすると、従来の認証プロトコルの使用が中断されます。

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 パートナーは、セキュリティに影響する可能性があるため、レガシ認証プロトコルを使用しないようにすることを強くお勧めします。これは、これらのプロトコルを MFA 検証で保護することができず、資格情報の侵害の影響を受けやすいためです。 レガシ認証プロトコルを使用しない場合、パートナーは、アプリケーションパスワードの使用をサポートする Azure AD Premium にサインアップすることを検討する必要があります。 アプリケーションパスワードは、システムによって生成される1回限りのパスワードであり、通常は人間が生成したパスワードよりも強力です。 アプリケーションパスワードを使用すると、パートナーはユーザーのために MFA を実装でき、レガシ認証プロトコルのアプリケーションパスワードにフォールバックすることができます。

> [!NOTE]
> パートナーがパートナーエージェント用に MFA を実装していない場合でも、パートナーエージェントは、MFA の登録と MFA の検証を完了できる限り、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。カスタマーテナントへのサインイン時にメッセージが表示されます。 MFA の登録を完了しても、ユーザーが MFA に対して自動的に有効になることはありません。

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>問題 6: パートナーが MFA をサポートしていない Exchange Online PowerShell を使用している
パートナーは、Exchange Online PowerShell とパートナー代理管理特権を使用して、顧客に代わって Exchange Online サービスを管理しています。 Exchange Online PowerShell では、MFA はサポートされていません。 パートナーがユーザーの MFA を実装している場合、これらのユーザーは Exchange Online PowerShell にアクセスできなくなります。 これは、技術的な例外の有効な理由ですか。

**回答**: はい。これは、技術的な例外の有効な理由として考慮される可能性があります。 パートナーの[代理管理をサポートする既存の Exchange Online PowerShell モジュール](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)では、パートナーユーザーがカスタマーテナントにサインインする必要がないため、MFA の検証を必要とする Azure AD の影響を受けません。 ただし、MFA との互換性はありません。 Microsoft Exchange Online チームは、パートナーの代理管理特権と MFA の両方をサポートする新しい PowerShell モジュールを開発しています。 新しい PowerShell モジュールが利用可能になるまで、パートナーは、既存の PowerShell モジュールを使用する必要があるユーザーの MFA を実装することはできません。 テナント間のサインイン時に MFA の検証を必要とする Azure AD により、これらのユーザーが他の Microsoft Online Services にアクセスできない場合、パートナーは、MFA の検証を抑制するための技術的な例外を要求できます。

> [!NOTE]
> パートナーは、Exchange Online PowerShell モジュールへのアクセスを必要とするユーザーに対して MFA を実装することはできませんが、これらのユーザーは、提供されたパートナー代理管理特権を使用して、Microsoft Online Services にアクセスして顧客リソースを管理できます。カスタマーテナントへのサインイン時に要求されたときに、MFA の登録と MFA の検証を完了できます。 MFA の登録を完了しても、ユーザーが MFA に対して自動的に有効になることはありません。そのため、Exchange Online PowerShell モジュールへのアクセスには影響しません。

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>問題 7: パートナーがサードパーティの MFA を実装しています。これは、によって認識されません Azure AD
パートナーは、サードパーティの MFA ソリューションを使用してユーザーの MFA を実装しています。 ただし、パートナーは、ユーザー認証中に MFA 検証が完了した Azure AD に、サードパーティの MFA ソリューションを適切に構成できません。 これは、技術的な例外の有効な理由ですか。

**回答**: はい。これは、技術的な例外の有効な理由として考慮される可能性があります。 技術的な例外の要求を送信する前に、サードパーティの MFA ソリューションプロバイダーに確認してください。これは、ユーザー認証時に MFA の検証が完了したことを示すために、 *authenticationmultipleauthn references*要求 (値の) Azure AD をフローするように構成できないことを示しています。 技術的な例外の要求を送信しているときに、使用されているサードパーティの MFA ソリューションの詳細を指定し、統合の方法を示します (例: id フェデレーションまたは Azure AD カスタムコントロールの使用)。

### <a name="how-to-submit-a-request-for-technical-exception"></a>技術的な例外の要求を送信する方法

技術的な例外の要求を送信するには、次のようにします。

1. グローバル管理者または管理エージェントとしてパートナーセンターにログインします。
2. [**サポート** > **パートナーサポート要求**] に移動し、 **[新しい要求]** をクリックして、新しいパートナーサービス要求を作成します。
4. **MFA とセキュリティで保護されたアプリケーションモデル**のトピックの選択するで、問題の種類として**技術的な例外の要求を送信**します。
6. テクニカル例外のサービス要求を送信するために要求された詳細を指定し、 **[送信]** をクリックします。

Microsoft は、技術的な例外の要求に対する応答を提供するまでに、最大3営業日かかることがあります。
