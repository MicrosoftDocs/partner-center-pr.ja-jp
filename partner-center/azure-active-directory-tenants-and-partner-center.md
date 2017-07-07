---
title: "Azure Active Directory テナントとパートナー センター | パートナー センター"
description: "パートナー センター アカウントを作成するには、Azure Active Directory (Azure AD) テナントが会社に必要です。 Azure AD は、マイクロソフトのクラウド ベース ディレクトリおよび ID 管理サービスです。"
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Azure Active Directory テナントとパートナー センター  

**適用対象**

-  パートナー センター

## <a name="why-you-need-an-azure-ad-tenant"></a>Azure AD テナントが必要な理由

テナント ユーザーが Azure AD (Microsoft アカウント) のユーザー名とパスワードを使ってパートナー センターにサインインできるように、組織の Azure AD テナントを新しいパートナー センター アカウントにリンクする必要があります。

会社に Azure AD テナントが既にある場合は、そのテナントをパートナー センター アカウントにリンクできます。 

>**注**<br> 既存の Azure AD テナントの使用を決める前に、パートナー センターで作業する必要があるテナント内のユーザーの数について考慮してください。 パートナー センターで作業する必要がないユーザーがテナントにいる場合、パートナー センターで作業する必要があるユーザーだけの新しいテナントを作成することを検討してください。

Azure AD テナントが会社にまだない場合は、登録プロセスを通じて無料で作成できます。 **[Azure Active Directory にサインインします]** ページで **[新しいテナントを作成する]** を選択します。 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>Azure AD テナントが会社に既にあるかどうかわからない場合

Azure AD テナントが会社にあるかどうかわからない場合、次の手順に従って確認します。 Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合、既に Azure AD テナントがある点に注意してください。
1.  Azure 管理ポータル (https://ms.portal.azure.com) にサインインする
2.  メニューから Azure Active Directory を選択し、ドメイン名を選択します。
3.  既にテナントがある場合、ドメイン名が表示されます。

### <a name="using-an-existing-tenant"></a>既存のテナントを使う場合

既存の Azure AD テナントを使おうとしてもサインインで問題が発生する場合、状況に最も合うシナリオを次の図から探し、推奨される手順に従います。 

![Azure AD テナントがあるか、もう 1 つ作成する必要がある場合](images/onboardingAADFlow.png)

Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)をご覧ください。

## <a name="about-microsoft-azure"></a>Microsoft Azure について

Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。 企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。 

Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。 オフィス ビルの所有者に対して、企業はテナントです。 

Azure AD テナントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。 

テナントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。 テナントには、グループ、アプリケーション、および会社とそのセキュリティに関連する他の情報も含まれています。 

Azure AD について詳しくは、[Azure Active Directory のドキュメント](https://docs.microsoft.com/ azure/active-directory/)をご覧ください。 