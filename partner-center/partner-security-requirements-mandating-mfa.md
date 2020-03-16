---
title: パートナー テナントに MFA を義務付ける | パートナー センター
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー テナントに MFA を義務付けることが顧客リソースへのアクセスのセキュリティ保護にどのように役立つかについて説明します。 サンプル シナリオが含まれています。
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウド ソリューションプロバイダー, クラウド ソリューション プロバイダー プログラム, CSP, コントロール パネル ベンダー, CPV, 多要素認証, MFA, 安全なアプリケーション モデル, セキュリティで保護されたアプリ モデル, セキュリティ
ms.localizationpriority: high
ms.openlocfilehash: bf57b489f84540e50e28df5568391818f50c79d4
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340190"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>パートナー テナントに多要素認証 (MFA) を義務付ける

**適用対象**

- クラウド ソリューション プロバイダー プログラムのすべてのパートナー
  - 直接請求
  - 間接プロバイダー
  - 間接リセラー
- すべてのアドバイザー

**該当するユーザー**
-    ゲスト ユーザーを含むすべての有効なユーザー

これらのパートナーは、次の領域に対して MFA 検証を完了するよう要求されます。

- [パートナー センター ダッシュボード](#partner-center-dashboard) (暦年 2020 年第 2 四半期を対象)
- [パートナー センター API](#partner-center-api) (暦年 2020 年第 2 四半期を対象)
- [パートナー代理管理](#partner-delegated-administration) (2019 年 11 月 18 日から)

この機能の目的は、パートナーが顧客リソースへのアクセスをセキュリティ保護して資格情報の侵害を防止できるように支援することです。

## <a name="partner-center-dashboard"></a>パートナー センター ダッシュボード
次のようなパートナー センター ダッシュボードの特定のページが MFA で保護されます。

* **[顧客]** タブのすべてのページ。
* **[サポート] > [Customer requests] (顧客の要求)** タブのすべてのページ。

これらのページのいずれかにアクセスしようとしたときに MFA 検証をまだ完了していない場合は、それを行うよう要求されます。

次のユーザーの種類は、これらの MFA で保護されたページへのアクセスが承認されているため、この機能によって影響を受けます。

* 管理エージェント
* 販売エージェント
* ヘルプデスク エージェント

検証がどのように動作するかを示すために、次の 2 つの例について考えてみます。

**例 1:パートナーが Azure AD MFA を実装している**
1.    Jane は CSP Contoso に勤めています。 Contoso は、Azure AD MFA を使用して Contoso パートナー テナントのすべてのユーザーに対して MFA を実装しました。
2.    Jane は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、サインインのために Jane を Azure AD にリダイレクトします。
3.    Contoso による既存の Azure AD MFA セットアップのために、Jane は MFA 検証を完了するよう要求されます。 サインインと MFA 検証に成功すると、Jane は、パートナー センター ダッシュボードの概要ページに再びリダイレクトされます。
4.    Jane は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 Jane は以前にサインイン中に既に MFA 検証を完了しているため、Jane は MFA 検証を再び実行するよう要求されることなく、MFA で保護されたページにアクセスできます。

**例 2:パートナーが ID フェデレーションを使用してサードパーティの MFA を実装している**
1. Trent は CSP Wingtip に勤めています。 Wingtip は、ID フェデレーション経由で Azure AD に統合されているサードパーティの MFA を使用して Wingtip パートナー テナントのすべてのユーザーに対して MFA を実装しました。
2. Trent は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、サインインのために Trent を Azure AD にリダイレクトします。
3. Wingtip は ID フェデレーションを設定しているため、Azure AD は、サインインと MFA 検証を完了するために Trent をフェデレーション ID プロバイダーにリダイレクトします。 サインインと MFA 検証に成功すると、Trent はまず Azure AD に、次にパートナー センター ダッシュボードの概要ページに再びリダイレクトされます。
4. Trent は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 Trent は以前にサインイン中に既に MFA 検証を完了しているため、Trent は MFA 検証を再び実行するよう要求されることなく、MFA で保護されたページにアクセスできます。

**例 3: パートナーが MFA を実装していない**
1. John は CSP Fabrikam に勤めています。 Fabrikam は、Fabrikam パートナー テナントのどのユーザーに対しても MFA を実装していません。
2. John は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、サインインのために John を Azure AD にリダイレクトします。
3. Fabrikam は MFA を実装していないため、John は MFA 検証を完了するよう要求されません。 サインインに成功すると、John は、パートナー センター ダッシュボードの概要ページに再びリダイレクトされます。
4. John は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 John は MFA 検証を完了していないため、パートナー センターは、MFA 検証を完了するために John を Azure AD にリダイレクトします。 John が MFA 検証を完了するよう要求されるのはこれが初めてであるため、John は、Microsoft Authenticator アプリを使用して MFA に登録することも要求されます。 MFA 登録と MFA 検証に成功すると、John は、MFA で保護されたページにアクセスできるようになります。

## <a name="partner-center-api"></a>パートナー センター API

パートナー センター API では、アプリのみの認証とアプリとユーザー認証の両方がサポートされます。 アプリとユーザー認証が使用される場合は、パートナー センターに MFA 検証が必要です。 具体的には、パートナー アプリケーションがパートナー センターに API 要求を送信しようとする場合、そのアプリケーションは要求の承認ヘッダーにアクセス トークンを含める必要があります。 パートナー センターが、アプリとユーザー認証を使用して取得されたアクセス トークンを含む API 要求を受信すると、パートナー センター API は、*認証方法参照 (AMR)* 要求に *MFA* 値が存在することを確認します。 JWT デコーダーを使用すると、アクセス トークンに、予測される認証方法参照 (AMR) 値が含まれているかどうかを検証できます。

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

この値が存在する場合、パートナー センターは MFA 検証が完了していると判断し、API 要求を処理します。 この値が存在しない場合、パートナー センター API は次の応答で要求を拒否します。

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>パートナー代理管理

### <a name="using-service-portals"></a>サービス ポータルの使用

パートナー アカウント (管理エージェントとヘルプデスク エージェントを含む) は、パートナー代理管理特権を使用して、Microsoft Online Services ポータル、コマンド ライン インターフェイス (CLI)、API (アプリとユーザー認証を使用) 経由で顧客リソースを管理できます。

顧客リソースを管理するためにパートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスした場合、これらのポータルの多くでは、パートナー アカウントは、認証コンテキスとして設定された顧客の Azure Active Directory テナントに対して対話的に認証する必要があります。つまり、パートナー アカウントは顧客テナントにサインインするよう要求されます。

Azure Active Directory は、このような認証要求を受信すると、パートナー アカウントに MFA 検証を完了するよう要求します。 パートナー アカウントがマネージド ID またはフェデレーション ID のどちらであるかに応じて、次の 2 つのユーザー エクスペリエンスが考えられます。

- パートナー アカウントが**マネージド** ID である場合、Azure Active Directory は直接、ユーザーに MFA 検証を完了するよう求めます。 パートナー アカウントが以前に Azure Active Directory を使用して MFA に登録していない場合、ユーザーは、まず [MFA 登録を完了する](#mfa-registration-experience)よう求められます。

- パートナー アカウントが**フェデレーション** ID である場合のエクスペリエンスは、パートナー管理者が Azure Active Directory でフェデレーションを構成した方法によって異なります。 Azure Active Directory でフェデレーションを設定するとき、パートナー管理者は、フェデレーション ID プロバイダーで MFA がサポートされるかどうかを Azure Active Directory に示すことができます。 サポートされる場合、Azure Active Directory は、MFA 検証を完了するためにユーザーをフェデレーション ID プロバイダーにリダイレクトします。 そうでない場合、Azure Active Directory は直接、ユーザーに MFA 検証を完了するよう求めます。 パートナー アカウントが以前に Azure Active Directory を使用して MFA に登録していない場合、ユーザーは、まず [MFA 登録を完了する](#mfa-registration-experience)よう求められます。

全体的なエクスペリエンスは、エンド カスタマーのテナントがその管理者に対して MFA を実装しているシナリオと同様です。 たとえば、顧客テナントで [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)が有効になっているとします。この場合は、管理者権限を持つすべてのアカウント (管理エージェントとヘルプデスク エージェントを含む) が MFA 検証を使用して顧客テナントにサインインするよう要求されます。 テストのために、パートナーは顧客テナントで [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にしてから、パートナー代理管理特権を使用して顧客テナントにアクセスしてみることができます。

> [!NOTE]
> パートナー代理管理特権を使用して顧客リソースにアクセスするときに、すべての Microsoft Online Service ポータルで、パートナー アカウントが顧客テナントにサインインするよう要求されるわけではありません。 代わりに、パートナー アカウントは、パートナー テナントにサインインするよう要求されるだけです。 1 つの例は Exchange 管理センターです。 いずれは、パートナー代理管理特権を使用するとき、これらのポータルではパートナー アカウントが顧客テナントにサインインするよう要求されると予測しています。

### <a name="using-service-apis"></a>サービス API の使用
一部の Microsoft Online Services API (Azure Resource Manager、Azure AD Graph、Microsoft Graph など) では、パートナーがパートナー代理管理特権を使用してプログラムで顧客リソースを管理することがサポートされています。 これらの API でパートナー代理管理特権を利用するには、パートナー アプリケーションが API 要求の承認ヘッダーにアクセス トークンを含める必要があります。ここで、このアクセス トークンは、パートナー ユーザー アカウントに Azure AD に対して、認証コンテキスとして設定された顧客の Azure AD に対して認証させることによって取得されます。 パートナー アプリケーションは、パートナー ユーザー アカウントに顧客テナントにサインインさせるよう要求されます。

Azure AD が認証要求などを受信すると、Azure AD は、パートナー ユーザー アカウントに MFA 検証を完了するよう要求します。 パートナー ユーザー アカウントが以前に MFA に登録していない場合、ユーザー アカウントは、まず MFA 登録を完了するよう要求されます。

パートナー代理管理特権を使用してこれらの API に統合されているすべてのパートナー アプリケーションがこの機能によって影響を受けます。 パートナー アプリケーションが引き続き、中断することなく確実にこれらの API を操作できるようにするには、次のようにします。

- パートナーは、アクセス トークンを取得するために Azure AD に対する非対話型のユーザー認証方法を使用することを避ける必要があります。 [パスワード フロー](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)などの非対話型のユーザー認証方法を使用している場合、Azure AD は、ユーザーに MFA 検証を完了するよう求めることができなくなります。 代わりに、パートナーは、[OpenID Connect フロー](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code)などの対話型のユーザー認証方法の使用に切り替える必要があります。
- 対話型のユーザー認証方法中に、パートナーは、MFA に対して既に有効になっているパートナー ユーザー アカウントを使用する必要があります。 あるいは、Azure AD からプロンプトが表示されたら、パートナーはサインイン中に MFA 登録と MFA 検証を完了できます。
- これは、エンド カスタマーのテナントがその管理者に対して MFA を実装しているシナリオと同様です。 たとえば、顧客テナントで [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)が有効になっているとします。この場合は、管理者権限を持つすべてのユーザー アカウント (管理エージェントとヘルプデスク エージェントを含む) が MFA 検証を使用して顧客テナントにサインインするよう要求されます。 テストのために、パートナーは顧客テナントで [Azure AD のセキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にしてから、パートナー代理管理特権を使用してプログラムで顧客テナントにアクセスしてみることができます。

### <a name="mfa-registration-experience"></a>MFA 登録エクスペリエンス
MFA 検証中に、パートナー アカウントが以前に MFA に登録していない場合、Azure AD は、まずユーザーに MFA 登録を完了するよう求めます。

![MFA 登録手順 1](images/MfaRegistration1.png)

**[次へ]** をクリックすると、ユーザーは、検証方法の一覧 (電話、SMS、Authenticator アプリなど) から選択するよう求められます。

![MFA 登録手順 2](images/MfaRegistration2.png)

登録に成功すると、ユーザーは次に、ユーザーが選択した検証方法に基づいて MFA 検証を完了するよう要求されます。



## <a name="request-for-technical-exception"></a>技術的な例外の要求

パートナーは、Microsoft Online Services で技術的な問題が発生しており、実現可能な解決策または回避策が存在しない場合、MFA 検証を抑制するための技術的な例外を申請できます。 これを行う前に、次のセクションを確認してください。

 - [パートナーによって報告された一般的な問題の一覧](#list-of-common-issues-reported-by-partners)
 - [技術的な例外の要求を提出する方法](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>パートナーによって報告された一般的な問題の一覧
技術的な例外を申請する前に、それが技術的な例外の有効な理由であるかどうかを判断するために、他のパートナーによって報告された一般的な問題の一覧を確認してください。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>問題 1: パートナーに、パートナー エージェントに対して MFA を実装するためのさらに多くの時間が必要である
あるパートナーが、顧客リソースを管理するためにパートナー代理管理特権を使用した Microsoft Online Services ポータルへのアクセスを必要としているパートナー エージェントに対する MFA の実装をまだ開始していないか、またはその最中です。 このパートナーには、MFA 実装を完了するためのさらに多くの時間が必要です。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 パートナーは、中断を回避するために、ユーザーに対して MFA を実装するための計画を作成する必要があります。

> [!NOTE]
> パートナーがパートナー エージェントに対して MFA を実装していないとしても、顧客テナントへのサインイン中にプロンプトが表示されたときに MFA 登録と MFA 検証を完了できる場合、パートナー エージェントは引き続き、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。 MFA 登録を完了しても、そのユーザーに対して MFA が自動的に有効になるわけではありません。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>問題 2: パートナーが、代理管理特権を使用していないユーザー アカウントに対して MFA を実装していない
あるパートナーのパートナー テナントに、パートナー代理管理特権を使用して顧客リソースを管理するための Microsoft Online Services ポータルへのアクセスを必要としていない何人かのユーザーが存在します。 このパートナーは、これらのユーザーに対して MFA を実装している最中であり、完了のためにさらに多くの時間が必要です。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 これらのユーザー アカウントは、顧客リソースを管理するためにパートナー代理管理特権を使用していないため、顧客テナントにサインインするよう要求されません。 これらは、顧客テナントへのサインイン中に MFA 検証が必要な Azure AD によって影響を受けません。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>問題 3: パートナーがユーザー サービス アカウントに対して MFA を実装していない
あるパートナーのパートナー テナントに、サービス アカウントとしてデバイスに使用されているいくつかのユーザー アカウントが存在します。 これらは、パートナー代理管理特権を使用して顧客リソースを管理するためのパートナー センターや Microsoft Online Services ポータルへのアクセスを必要としていない低特権アカウントです。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 これらのユーザー アカウントは、顧客リソースを管理するためにパートナー代理管理特権を使用していないため、顧客テナントにサインインするよう要求されません。 これらは、顧客テナントへのサインイン中に MFA 検証が必要な Azure AD によって影響を受けません。

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>問題 4: パートナーが MS Authenticator アプリを使用して MFA を実装できない
あるパートナーが、従業員の個人用モバイル デバイスの作業領域への持ち込みを許可しない "クリーン デスク" ポリシーを設定しています。 個人用モバイル デバイスへのアクセスがないと、Azure AD ベースライン ポリシーでサポートされている唯一の MFA 検証である MS Authenticator アプリを従業員がインストールできません。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 このパートナーは、従業員がパートナー センターにアクセスするときに引き続き MFA 検証を完了できるように、次の代替手段を検討する必要があります。
- MS Authenticator アプリの他にも、Azure AD ベースライン ポリシーは、サードパーティの互換性のある Authenticator アプリでも使用できます。これは、Microsoft Windows を実行している Windows コンピューターでサポートされている可能性があります。
- パートナーはまた、追加の検証方法を提供できる Azure AD Premium または (Azure AD と互換性のある) サードパーティの MFA ソリューションにサインアップすることもできます。

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>問題 5: パートナーが、レガシ認証プロトコルの使用のために MFA を実装できない
あるパートナーの一部のパートナー エージェントが、MFA と互換性のないレガシ認証プロトコルを引き続き使用しています。 たとえば、ユーザーが、レガシ認証プロトコルに基づく Outlook 2010 を引き続き使用しています。 これらのパートナー エージェントに対して MFA を有効にすると、レガシ認証プロトコルの使用が中断されます。

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 これらのレガシ認証プロトコルは MFA 検証では保護できず、資格情報の侵害を受ける可能性が非常に高いため、セキュリティへの潜在的な影響を考慮し、パートナーにはその使用を避けることを強くお勧めします。 レガシ認証プロトコルの使用を避けることができない場合、パートナーは、アプリケーション パスワードの使用をサポートする Azure AD Premium へのサインアップを検討する必要があります。 アプリケーション パスワードはシステムで生成されたワンタイム パスワードであり、通常、人間が生成したパスワードより強力です。 アプリケーション パスワードを使用すると、パートナーはレガシ認証プロトコルの場合にのみアプリケーション パスワードにフォールバックしながら、ユーザーに対して MFA を実装できます。

> [!NOTE]
> パートナーがパートナー エージェントに対して MFA を実装していないとしても、顧客テナントへのサインイン中にプロンプトが表示されたときに MFA 登録と MFA 検証を完了できる場合、パートナー エージェントは引き続き、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。 MFA 登録を完了しても、そのユーザーに対して MFA が自動的に有効になるわけではありません。

#### <a name="issue-6-partner-is-using-exchange-online-powershell-that-does-not-support-mfa"></a>問題 6: パートナーが、MFA をサポートしていない Exchange Online PowerShell を使用している
あるパートナーが、顧客の代わりに Exchange Online サービスを管理するためにパートナー代理管理特権で Exchange Online PowerShell を使用しています。 Exchange Online PowerShell は MFA をサポートしていません。 このパートナーがユーザーに対して MFA を実装した場合、これらのユーザーは Exchange Online PowerShell にアクセスできなくなります。 この問題は、技術的な例外の有効な理由ですか?

**回答**: はい。この問題は、技術的な例外の有効な理由と見なされる可能性があります。 [パートナー代理管理をサポートする既存の Exchange Online PowerShell モジュール](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)は、パートナー ユーザーに顧客テナントにサインインするよう要求しないため、MFA 検証が必要な Azure AD によって影響を受けません。 ただし、これは MFA と互換性がありません。 Microsoft Exchange Online チームは、パートナー代理管理特権と MFA の両方をサポートする新しい PowerShell モジュールを開発しています。 新しい PowerShell モジュールが使用可能になるまで、パートナーは、既存の PowerShell モジュールを使用する必要があるユーザーに対して MFA を実装できません。 テナントにまたがるサインイン中に MFA 検証が必要な Azure AD のために、これらのユーザーが他の Microsoft Online Services にアクセスしたときに問題が発生する場合、パートナーは MFA 検証を抑制するための技術的な例外を要求できます。

> [!NOTE]
> パートナーが、Exchange Online PowerShell モジュールへのアクセスを必要としているユーザーに対して MFA を実装できないとしても、顧客テナントへのサインイン中にプロンプトが表示されたときに MFA 登録と MFA 検証を完了できる場合、これらのユーザーは引き続き、パートナー代理管理特権を使用して顧客リソースを管理するために Microsoft Online Services にアクセスできます。 MFA 登録を完了しても、そのユーザーに対して MFA が自動的に有効になるわけではないため、Exchange Online PowerShell モジュールへのアクセスには影響を与えません。

#### <a name="issue-7-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>問題 7: パートナーが、Azure AD によって認識されないサードパーティの MFA を実装している
あるパートナーが、サードパーティの MFA ソリューションを使用してユーザーに対して MFA を実装しました。 ただし、このパートナーは、ユーザー認証中に MFA 検証が完了したことを Azure AD に中継するようにサードパーティの MFA ソリューションを正しく構成できません。 これは、技術的な例外の有効な理由ですか?

**回答**: はい。この問題は、技術的な例外の有効な理由と見なされる可能性があります。 技術的な例外の要求を提出する前に、サードパーティの MFA ソリューションのプロバイダーに、ユーザー認証中に MFA 検証が完了したことを示すために *authenticationmethodsreferences* 要求 (値は *multipleauthn*) を Azure AD に渡すように MFA ソリューションを構成できないことを確認してください。 技術的な例外の要求を提出するとき、使用されているサードパーティの MFA ソリューションの詳細を指定し、統合の方法 (ID フェデレーション経由や Azure AD カスタム コントロールの使用など) を示す必要があります。

### <a name="how-to-submit-a-request-for-technical-exception"></a>技術的な例外の要求を提出する方法

技術的な例外の要求を提出するには:

1. グローバル管理者または管理エージェントとしてパートナー センターにログインします。
2. **[サポート]**  >  **[Partner support requests] (パートナー サポート要求)** に移動し、 **[新しい要求]** をクリックすることによって、新しいパートナー サービス要求を作成します。
4. **[MFA and Secure Application Model] (MFA とセキュア アプリケーション モデル)** のトピックで、問題の種類として **[Submit request for technical exception] (技術的な例外の要求を提出する)** を選択します。
6. 技術的な例外のサービス要求を提出するよう要求された詳細を指定し、 **[提出]** をクリックします。

Microsoft では、技術的な例外の要求への応答を提供するまでに最大 3 営業日かかることがあります。
