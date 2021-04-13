---
title: パートナー テナントに多要素認証 (MFA) を義務付ける
ms.topic: article
ms.date: 10/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー テナントに MFA を義務付けることが顧客リソースへのアクセスのセキュリティ保護にどのように役立つかについて説明します。 サンプル シナリオが含まれています。
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 21e0ebd58835be34f9cc161072ff3690b30abf57
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/31/2021
ms.locfileid: "106086364"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>パートナー テナントに多要素認証 (MFA) を義務付ける

**適切なロール**

- 管理エージェント
- 販売代理店
- ヘルプデスク エージェント
- 課金管理者
- グローバル管理者

この記事では、パートナー センターで多要素認証 (MFA) を義務付けるための詳細な例とガイダンスを示します。 この機能の目的は、パートナーが顧客リソースへのアクセスをセキュリティ保護して資格情報の侵害を防止できるように支援することです。 パートナーは、パートナー テナント内のすべてのユーザー アカウント (ゲスト ユーザーを含む) に対して MFA を強制する必要があります。 ユーザーは次の領域に対して MFA 検証を完了することが義務付けられます。

- [パートナー センター ダッシュボード](#partner-center-dashboard)
- [パートナー センター API](#partner-center-api)
- [パートナー代理管理](#partner-delegated-administration)

高いレベルのセキュリティおよびプライバシーの保護の継続的な実施は最優先事項の1つであり、パートナーが顧客とテナントを保護する上で Microsoft は引き続き支援を提供していきます。 クラウド ソリューション プロバイダー (CSP) プログラムに参加するすべてのパートナー、コントロール パネル ベンダー (CPV)、アドバイザーは、準拠した状態を保つために[パートナーのセキュリティ要件](partner-security-requirements.md)を実装する必要があります。

パートナーが ID の盗難や未承認のアクセスからビジネスや顧客を保護できるようにするため、パートナーのテナントに対して追加のセキュリティ セーフガードがアクティブ化されました。それに伴い、MFA が義務付けられ、検証されるようになりました。 

## <a name="partner-center-dashboard"></a>パートナー センター ダッシュボード

次のようなパートナー センター ダッシュボードの特定のページが MFA で保護されます。

- **[Customers]** タブのすべてのページ。例: 以下の URL でアクセス可能なすべてのページ https://partner.microsoft.com/commerce/*
- **[サポート] > [Customer requests (顧客の要求)]** タブのすべてのページ。例：[請求] ページでアクセスする https://partner.microsoft.com/dashboard/support/csp/customers/*
- [請求] ページ

次の表は、どのユーザーの種類がこれらの MFA で保護されたページへのアクセスを認可されるか (したがって、この機能による影響を受けるか) を示しています。


| MFA 保護対象のページ       | 管理エージェント      |  販売エージェント     |   ヘルプデスク エージェント     | 全体管理者      |  課金管理者     | 
|---    |---    |---    |---    |---    |---    |
| [Customers] タブのすべてのページ      |   x    |    x   |  x     |       |       |
| [サポート] > [Customer requests (顧客の要求)] タブのすべてのページ     | x      |       |    x   |       |       |
| [請求] ページ     |   x    |       |       |    x   |   x    |

これらのページのいずれかにアクセスしようとしたときに MFA 検証をまだ完了していない場合は、それを行うよう要求されます。 パートナー センターのその他のページ ([概要] ページ、[サービスの正常性状態] 確認ページなど) には MFA は不要です。

## <a name="verification-examples"></a>検証の例

パートナー センター ダッシュボードで検証がどのように動作するかについて、次の例を使って説明します。

### <a name="example-1-partner-has-implemented-azure-ad-mfa"></a>例 1:パートナーが Azure AD MFA を実装している

1. Jane は CSP Contoso に勤めています。 Contoso では、Azure Active Directory (Azure AD) MFA を使用して、Contoso のパートナー テナントのすべてのユーザーに対して MFA を実装しています。

2. Jane は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、Jane を Azure AD にリダイレクトして、サインインを求めます。

3. Contoso による既存の Azure AD MFA セットアップのために、Jane は MFA 検証を完了するよう要求されます。 サインインと MFA 検証に成功すると、Jane は、パートナー センター ダッシュボードの概要ページに再びリダイレクトされます。

4. Jane は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 Jane は以前にサインイン中に既に MFA 検証を完了しているため、Jane は MFA 検証を再び実行するよう要求されることなく、MFA で保護されたページにアクセスできます。

### <a name="example-2-partner-has-implemented-third-party-mfa-using-identity-federation"></a>例 2:パートナーは、ID フェデレーションを使用するサードパーティの MFA を実装しています

1. Trent は CSP Wingtip に勤めています。 Wingtip では、ID フェデレーション経由で Azure AD に統合されているサードパーティの MFA を使用して、Wingtip のパートナー テナントのすべてのユーザーに対して MFA を実装しています。

2. Trent は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、Trent を Azure AD にリダイレクトして、サインインを求めます。

3. Wingtip は ID フェデレーションを設定しているため、Azure AD は、サインインと MFA 検証を完了するために Trent をフェデレーション ID プロバイダーにリダイレクトします。 サインインと MFA 検証に成功すると、Trent はまず Azure AD に、次にパートナー センター ダッシュボードの概要ページに再びリダイレクトされます。

4. Trent は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 Trent は以前にサインイン中に既に MFA 検証を完了しているため、Trent は MFA 検証を再び実行するよう要求されることなく、MFA で保護されたページにアクセスできます。

### <a name="example-3-partner-hasnt-implemented-mfa"></a>例 3: パートナーが MFA を実装していない

1. John は CSP Fabrikam に勤めています。 Fabrikam は、Fabrikam パートナー テナントのどのユーザーに対しても MFA を実装していません。

2. John は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは、John を Azure AD にリダイレクトして、サインインを求めます。

3. Fabrikam は MFA を実装していないため、John は MFA 検証を完了するよう要求されません。 サインインに成功すると、John は、パートナー センター ダッシュボードの概要ページに再びリダイレクトされます。

4. John は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 John は MFA 検証を完了していないため、パートナー センターは、MFA 検証を完了するために John を Azure AD にリダイレクトします。 John が MFA 検証の完了を求められるのはこれが初めてであるため、John は [MFA への登録](#mfa-registration-experience)も要求されます。 MFA 登録と MFA 検証に成功すると、John は、MFA で保護されたページにアクセスできるようになります。

5. Fabrikam がユーザーに対する MFA を実装する前のある日、John は新しいブラウザー セッションを開始し、パートナー センター ダッシュボードの (MFA で保護されていない) 概要ページに移動します。 パートナー センターは John を Azure AD にリダイレクトして、MFA プロンプトは表示せず、サインインを求めます。 

6. John は、パートナー センターの MFA で保護されたページのいずれかにアクセスしようとします。 John は MFA 検証を完了していないため、パートナー センターは、MFA 検証を完了するために John を Azure AD にリダイレクトします。 John は MFA 登録を完了しているため、今回は MFA の検証の完了のみが要求されます。

> [!NOTE]
>アクション:会社の管理者には、MFA を実装するための[選択肢が 3 つ](partner-security-requirements.md#implementing-multi-factor-authentication)あります。

## <a name="partner-center-api"></a>パートナー センター API

パートナー センター API では、アプリのみの認証とアプリ + ユーザー認証の両方がサポートされます。 

アプリとユーザー認証が使用される場合は、パートナー センターに MFA 検証が必要です。 具体的には、パートナー アプリケーションがパートナー センターに API 要求を送信しようとする場合、そのアプリケーションは要求の承認ヘッダーにアクセス トークンを含める必要があります。 

> [!NOTE]
>[セキュア アプリケーション モデル フレームワーク](/partner-center/develop/enable-secure-app-model)は、パートナー センター API を呼び出す際に Microsoft Azure MFA アーキテクチャを介して CSP パートナーおよび CPV を認証するためのスケーラブルなフレームワークです。 テナントで MFA を有効にする前に、このフレームワークを実装する必要があります。 

App+User (アプリ + ユーザー) 認証を使用して取得したアクセス トークンを含む API 要求をパートナー センターが受信すると、パートナー センター API が、*認証方法参照 (AMR)* 要求に *MFA* 値が存在することを確認します。 JWT デコーダーを使用すると、アクセス トークンに、予測される認証方法参照 (AMR) 値が含まれているかどうかを検証できます。

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
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
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

アプリのみの認証が使用されている場合、アプリのみの認証をサポートする API は、MFA を必要とせずに継続して機能します。

## <a name="partner-delegated-administration"></a>パートナー代理管理

パートナー アカウント (管理エージェントとヘルプデスク エージェントを含む) は、パートナー代理管理特権を使用して、Microsoft Online Services ポータル、コマンドライン インターフェイス (CLI)、API (アプリ + ユーザー認証を使用) 経由で顧客リソースを管理できます。

### <a name="using-service-portals"></a>サービス ポータルの使用

パートナー代理管理特権 (Admin-On-Behalf-Of) を使用して Microsoft Online Services ポータルにアクセスし、顧客リソースを管理する場合、これらのポータルの多くでは、顧客の Azure AD テナントを認証コンテキストとして設定し、パートナー アカウントをインタラクティブに認証する必要があります。つまり、パートナー アカウントは顧客テナントにサインインする必要があります。

Azure AD でこのような認証要求が受信されると、パートナー アカウントに対し、MFA 検証を完了するよう求められます。 パートナー アカウントがマネージド ID またはフェデレーション ID のどちらであるかに応じて、次の 2 つのユーザー エクスペリエンスが考えられます。

- パートナー アカウントが **マネージド** ID である場合、Azure AD からユーザーに対して直接 MFA 検証を完了するよう求めるプロンプトが表示されます。 パートナー アカウントが以前に Azure AD を使用して MFA に登録していない場合、ユーザーは、まず [MFA 登録を完了する](#mfa-registration-experience)よう求められます。

- パートナー アカウントが **フェデレーション** ID である場合のエクスペリエンスは、パートナー管理者が Azure AD でフェデレーションを構成した方法によって異なります。 Azure AD でフェデレーションを設定するとき、パートナー管理者は、フェデレーション ID プロバイダーで MFA がサポートされるかどうかを Azure AD に示すことができます。 サポートされる場合、MFA 検証を完了するため、Azure AD によってユーザーはフェデレーション ID プロバイダーにリダイレクトされます。 そうでない場合、Azure AD からユーザーに対して直接 MFA 検証を完了するよう求めるプロンプトが表示されます。 パートナー アカウントが以前に Azure AD を使用して MFA に登録していない場合、ユーザーは、まず [MFA 登録を完了する](#mfa-registration-experience)よう求められます。

全体的なエクスペリエンスは、エンド カスタマーのテナントがその管理者に対して MFA を実装しているシナリオと同様です。 たとえば、顧客テナントで [Azure AD のセキュリティの既定値](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)が有効になっているとします。この場合は、管理者権限を持つすべてのアカウント (管理エージェントとヘルプデスク エージェントを含む) が MFA 検証を使用して顧客テナントにサインインするよう要求されます。 テストのために、パートナーは顧客テナントで [Azure AD のセキュリティの既定値](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にしてから、パートナー代理管理特権を使用して顧客テナントにアクセスしてみることができます。

> [!NOTE]
> パートナー代理管理特権を使用して顧客リソースにアクセスするときに、すべての Microsoft Online Service ポータルで、パートナー アカウントが顧客テナントにサインインするよう要求されるわけではありません。 代わりに、パートナー アカウントは、パートナー テナントにサインインするよう要求されるだけです。 1 つの例は Exchange 管理センターです。 いずれは、パートナー代理管理特権を使用するとき、これらのポータルではパートナー アカウントが顧客テナントにサインインするよう要求されると予測しています。

### <a name="using-service-apis"></a>サービス API の使用

一部の Microsoft Online Services API (Azure Resource Manager、Azure AD Graph、Microsoft Graph など) では、パートナーがパートナー代理管理特権を使用してプログラムで顧客リソースを管理することがサポートされています。 これらの API でパートナー代理管理特権を使用するには、パートナー アプリケーションが API 要求の Authorization ヘッダーにアクセス トークンを含める必要があります。ここで、このアクセス トークンは、パートナー ユーザー アカウントに Azure AD に対して、認証コンテキストとして設定された顧客の Azure AD を使用して認証させることによって取得されます。 パートナーのユーザー アカウントが顧客テナントにサインインするには、パートナー アプリケーションが必要です。

Azure AD が認証要求などを受信すると、Azure AD は、パートナー ユーザー アカウントに MFA 検証を完了するよう要求します。 パートナー ユーザー アカウントが以前に MFA に登録していない場合、ユーザー アカウントは、まず MFA 登録を完了するよう要求されます。

パートナー代理管理特権を使用してこれらの API に統合されているすべてのパートナー アプリケーションがこの機能によって影響を受けます。 パートナー アプリケーションが引き続き、中断することなく確実にこれらの API を操作できるようにするには、次のようにします。

- パートナーは、アクセス トークンを取得するために Azure AD に対する非対話型のユーザー認証方法を使用することを避ける必要があります。 [パスワード フロー](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password)などの非対話型のユーザー認証方法を使用している場合、Azure AD は、ユーザーに MFA 検証を完了するよう求めることができなくなります。 代わりに、パートナーは、[OpenID Connect フロー](/azure/active-directory/develop/v1-protocols-openid-connect-code)などの対話型のユーザー認証方法の使用に切り替える必要があります。

- 対話型のユーザー認証方法中に、パートナーは、MFA に対して既に有効になっているパートナー ユーザー アカウントを使用する必要があります。 あるいは、Azure AD からプロンプトが表示されたら、パートナーはサインイン中に MFA 登録と MFA 検証を完了できます。

- これは、エンド カスタマーのテナントがその管理者に対して MFA を実装しているシナリオと同様です。 たとえば、顧客テナントで [Azure AD のセキュリティの既定値](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)が有効になっているとします。この場合は、管理者権限を持つすべてのユーザー アカウント (管理エージェントとヘルプデスク エージェントを含む) が MFA 検証を使用して顧客テナントにサインインするよう要求されます。 テストのために、パートナーは顧客テナントで [Azure AD のセキュリティの既定値](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にしてから、パートナー代理管理特権を使用してプログラムで顧客テナントにアクセスしてみることができます。

### <a name="mfa-registration-experience"></a>MFA 登録エクスペリエンス

MFA 検証中に、パートナー アカウントが以前に MFA に登録していない場合、Azure AD は、まずユーザーに MFA 登録を完了するよう求めます。

:::image type="content" source="images/MfaRegistration1.png" alt-text="MFA 登録手順 1":::

**[次へ]** をクリックすると、ユーザーは、検証方法の一覧から選択することを求められます。

:::image type="content" source="images/MfaRegistration2.png" alt-text="MFA 登録手順 2":::

登録に成功すると、ユーザーは次に、ユーザーが選択した検証方法に基づいて MFA 検証を完了するよう要求されます。
 
## <a name="list-of-common-issues"></a>一般的な問題の一覧

MFA 要件に対する[技術的な例外](#how-to-submit-a-request-for-technical-exception)を申請する前に、その要求が有効かどうかを把握するために、他のパートナーによって報告された一般的な問題の一覧を確認してください。

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>問題 1: パートナーに、パートナー エージェントに対して MFA を実装するためのさらに多くの時間が必要である
あるパートナーが、顧客リソースを管理するためにパートナー代理管理特権を使用した Microsoft Online Services ポータルへのアクセスを必要としているパートナー エージェントに対する MFA の実装をまだ開始していないか、またはその最中です。 このパートナーには、MFA 実装を完了するためのさらに多くの時間が必要です。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 パートナーは、中断を回避するために、ユーザーに対して MFA を実装するための計画を作成する必要があります。

> [!NOTE]
> パートナーがパートナー エージェントに対して MFA を実装していないとしても、顧客テナントへのサインイン中にプロンプトが表示されたときに MFA 登録と MFA 検証を完了できる場合、パートナー エージェントは引き続き、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。 MFA 登録を完了しても、そのユーザーに対して MFA が自動的に有効になるわけではありません。

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>問題 2: パートナーが、代理管理特権を使用していないユーザー アカウントに対して MFA を実装していない
あるパートナーのパートナー テナントに、パートナー代理管理特権を使用して顧客リソースを管理するための Microsoft Online Services ポータルへのアクセスを必要としていない何人かのユーザーが存在します。 このパートナーは、これらのユーザーに対して MFA を実装している最中であり、完了にはさらに時間が必要です。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 これらのユーザー アカウントは、顧客リソース管理にパートナー代理管理特権を使用していないため、顧客テナントへのサインインは要求されません。 これらは、顧客テナントへのサインイン中に MFA 検証が必要な Azure AD によって影響を受けません。

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>問題 3: パートナーがユーザー サービス アカウントに対して MFA を実装していない
あるパートナーのパートナー テナントに、サービス アカウントとしてデバイスに使用されているいくつかのユーザー アカウントが存在します。 これらは、パートナー代理管理特権を使用して顧客リソースを管理するためのパートナー センターや Microsoft Online Services ポータルへのアクセスを必要としていない低特権アカウントです。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。 これらのユーザー アカウントは、顧客リソース管理にパートナー代理管理特権を使用していないため、顧客テナントへのサインインは要求されません。 これらは、顧客テナントへのサインイン中に MFA 検証が必要な Azure AD によって影響を受けません。

##### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>問題 4: パートナーが MS Authenticator アプリを使用して MFA を実装できない
あるパートナーが、従業員の個人用モバイル デバイスの作業領域への持ち込みを許可しない "クリーン デスク" ポリシーを設定しています。 個人用モバイル デバイスへのアクセスがない場合、従業員は、Azure AD セキュリティ既定値でサポートされる唯一の MFA 検証である MS Authenticator アプリをインストールできません。 この問題は、技術的な例外の有効な理由ですか?

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 このパートナーは、従業員がパートナー センターにアクセスするときに引き続き MFA 検証を完了できるように、次の代替手段を検討する必要があります。
- また、パートナーは追加の検証方法を提供できる Azure AD Premium または (Azure AD と互換性のある) サードパーティの MFA ソリューションにサインアップすることもできます。

##### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>問題 5: パートナーが、レガシ認証プロトコルの使用のために MFA を実装できない
あるパートナーの一部のパートナー エージェントが、MFA と互換性のないレガシ認証プロトコルを引き続き使用しています。 たとえば、ユーザーが、レガシ認証プロトコルに基づく Outlook 2010 を引き続き使用しています。 これらのパートナー エージェントに対して MFA を有効にすると、レガシ認証プロトコルの使用が中断されます。

**回答**: いいえ。これは、技術的な例外の有効な理由ではありません。 これらのレガシ認証プロトコルは MFA 検証では保護できず、資格情報の侵害を受ける可能性が非常に高いため、セキュリティへの潜在的な影響を考慮し、パートナーにはその使用を避けることを強くお勧めします。 レガシ認証プロトコルの使用を避けることができない場合、パートナーは、アプリケーション パスワードの使用をサポートする Azure AD Premium へのサインアップを検討する必要があります。 アプリケーション パスワードはシステムで生成されたワンタイム パスワードであり、通常、人間が生成したパスワードより強力です。 アプリケーション パスワードを使用すると、パートナーはレガシ認証プロトコルの場合にのみアプリケーション パスワードにフォールバックしながら、ユーザーに対して MFA を実装できます。

Outlook のレガシ認証のサポートに関する最新の計画については、[基本認証と Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) に関する投稿を参照してください。また、[Exchange チームのブログ](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) をフォローして、今後も最新のニュースを入手してください。 

> [!NOTE]
> パートナーがパートナー エージェントに対して MFA を実装していないとしても、顧客テナントへのサインイン中にプロンプトが表示されたときに MFA 登録と MFA 検証を完了できる場合、パートナー エージェントは引き続き、パートナー代理管理特権を使用して Microsoft Online Services ポータルにアクセスできます。 MFA 登録を完了しても、そのユーザーに対して MFA が自動的に有効になるわけではありません。

##### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>問題 6: パートナーが、Azure AD が認識しないサードパーティの MFA を実装している
あるパートナーが、サードパーティの MFA ソリューションを使用して、ユーザーに対して MFA を実装しました。 ただし、このパートナーは、サードパーティの MFA ソリューションを正しく構成できておらず、ユーザー認証中に MFA 検証が完了したことが Azure AD に伝達されません。 これは、技術的な例外の有効な理由ですか?

**回答**: はい。この問題は、技術的な例外の有効な理由と見なされる可能性があります。 技術的な例外の要求を提出する前に、ユーザー認証中に MFA 検証が完了したことを示すために *authenticationmethodsreferences* 要求 (値は *multipleauthn*) を Azure AD に渡すように MFA ソリューションを構成できないということを、サードパーティの MFA ソリューションのプロバイダーに確認してください。 技術的な例外の要求を提出する際、使用するサードパーティの MFA ソリューションの詳細を提供し、統合の方法 (ID フェデレーション経由、Azure AD カスタム コントロールの使用など) を記載し、サポート ドキュメントとして技術的な例外の要求中に以下の情報を必ず提供してください。

- サードパーティの MFA の構成。

- サードパーティの MFA が有効であるアカウントで実行された[パートナー セキュリティ要件テスト](/powershell/partnercenter/test-partner-security-requirements)の結果。

- 使用中または使用する予定のサードパーティの MFA ソリューションの注文書。

## <a name="how-to-submit-a-request-for-technical-exception"></a>技術的な例外の要求を提出する方法

パートナーは、Microsoft Online Services で技術的な問題が発生しており、実現可能な解決策または回避策が存在しない場合、MFA 検証を抑制するための技術的な例外を申請できます。 これを行う前に、前のセクションで説明した[一般的な問題の一覧](#list-of-common-issues)を確認してください。

技術的な例外の要求を提出するには:

1. グローバル管理者または管理エージェントとしてパートナー センターにサインインします。

2. **[サポート]**  >  **[パートナー サポート リクエスト]** に移動し、 **[新しい要求]** を選択することによって、新しいパートナー サービス要求を作成します。

3. [検索] ボックスで、**MFA - 例外の要求** を検索します。または、[カテゴリ] から **CSP** を選択し、[トピック] から **[アカウント]、[オンボード]、[アクセス]** の順に選択し、サブトピックから **MFA - 例外の要求** を選択し、 **[次のステップ]** を選択します。

4. 技術的な例外のサービス要求を提出するために求められた詳細を提供し、 **[提出]** を選択します。

技術的な例外の要求への応答を Microsoft から提供するまでに最大 3 営業日かかることがあります。

## <a name="next-steps"></a>次のステップ

 - [パートナー セキュリティ要件の状態](partner-security-compliance.md)