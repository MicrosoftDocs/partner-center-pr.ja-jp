---
title: 職場アカウントとパートナー センター | パートナー センター
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー センター アカウントの作成に職場アカウントが必要な理由と、既に職場アカウントを持っているかどうかを確認します。
author: LauraBrenner
ms.author: labrenne
Keywords: 職場アカウント, 電子メール, テナント, Azure テナント, アカウントの作成, ドメイン名
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: c8b731eeed6590e040eda18cb0e7093b389447b4
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253317"
---
# <a name="your-company-work-account-and-partner-center"></a>会社の職場アカウントとパートナー センター  

**適用対象**

-  パートナー センター

## <a name="why-you-need-a-work-account"></a>職場アカウントが必要な理由

アカウント ユーザーが職場アカウントのユーザー名とパスワードを使ってパートナー センターにサインインできるように、会社の職場アカウントを新しいパートナー センター アカウントにリンクする必要があります。

## <a name="the-work-account-email-address"></a>職場アカウントのメール アドレス

職場アカウントまたは勤務先メールは、会社によって指定されたメール アドレスです。 通常、職場アカウントのメールの形式は you@yourcompany.com です。 Hotmail、Gmail などの個人のメール アドレスは勤務先メールではなく、パートナー センター アカウントには使用できません。 

有効な勤務先メール アドレスが複数ある場合は、地域部門ではなく本社に関連付けられているメール アドレスを使用します。たとえば、contoso.uk アドレスではなく contoso.com メールを使用します。

> [!NOTE]  
>  既存の職場アカウントの使用を決める前に、パートナー センターでの作業を必要とするアカウント内のユーザーの数を考慮してください。 パートナー センターで作業する必要がないユーザーがアカウントにいる場合、パートナー センターで作業する必要があるユーザー用にのみ、新しいアカウントを作成することを検討してください。


## <a name="not-sure-if-your-company-already-has-a-work-account"></a>職場アカウントが会社に既にあるかどうかわからない場合

会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。 Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合は、既に職場アカウントが用意されています。

1.  Azure 管理ポータル (https://ms.portal.azure.com ) にサインインします。
2.  メニューから Azure Active Directory を選択し、ドメイン名を選択します。
3.  既に職場アカウントがある場合、ドメイン名が表示されます。

会社に職場アカウントがまだない場合は、登録プロセスを通じて無料で作成できます。

次の図は、いくつかの一般的なシナリオの手順を示しています。

- 職場アカウントがあるかどうかを確認する 
- 職場アカウントにサインインする方法を確認する 
- 新しい職場アカウントを作成する必要があるかどうかを判断する


![職場アカウントがあるか、作成する必要があるかのチェック](images/onboardingAADFlow.png)

Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)をご覧ください。

## <a name="about-microsoft-azure"></a>Microsoft Azure について

Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。 企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。 

Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のスペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。 オフィス ビルの所有者に対して、企業はテナントです。 

Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。 

職場アカウントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。 職場アカウントには、グループ、アプリケーション、および会社とそのセキュリティに関連する他の情報も含まれています。 
