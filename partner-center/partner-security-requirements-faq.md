---
title: パートナーのセキュリティ要件に関する FAQ |パートナーセンター
ms.topic: article
ms.date: 07/18/2019
description: パートナーのセキュリティ要件についてよく寄せられる質問
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, クラウドソリューションプロバイダー, Cloud Solution Provider プログラム, CSP, コントロールパネルベンダ, CPV, multi-factor authentication, MFA, 安全なアプリケーションモデル, セキュリティで保護されたアプリモデル, セキュリティ
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315551"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>パートナーのセキュリティ要件についてよく寄せられる質問

この記事では、[パートナーのセキュリティ要件](partner-security-requirements.md)に関してよく寄せられる質問をいくつか紹介します。 よく寄せられる質問の一覧については、[こちら](http://assetsprod.microsoft.com/security-requirements-faq.pdf)を参照してください。

## <a name="conditional-access"></a>条件付きアクセス

### <a name="can-conditional-access-be-used"></a>条件付きアクセスを使用できますか?

はい。条件付きアクセスを使用して、パートナーテナントの各ユーザー (サービスアカウントを含む) に MFA を適用できます。 ただし、パートナーになるという高度な特権がある場合は、各ユーザーが単一の認証ごとに MFA チャレンジを使用できるようにする必要があります。 これは、MFA の要件を回避する条件付きアクセスの機能を利用できないことを意味します。

## <a name="multi-factor-authentication"></a>多要素認証

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

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>ベースライン保護ポリシーの実装により、どのような検証オプションが提供されますか。 

ベースライン保護ポリシーの実装によって利用可能な MFA のバージョンに関して、使用可能な認証オプションは authenticator アプリだけです。 通話とテキストメッセージメッセージの使用は、安全性が低いと見なされます。 そのため、これらのオプションは、このバージョンの MFA では使用できません。

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件の影響を受けますか。

いいえ。 Azure AD Connect によって使用されるサービスアカウントは、パートナーのセキュリティ要件による影響を受けません。 MFA を適用した結果として Azure AD Connect の問題が発生した場合は、Microsoft サポートに問い合わせてテクニカルサポートを依頼してください。
