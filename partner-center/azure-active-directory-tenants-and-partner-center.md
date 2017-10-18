---
title: "職場アカウントとパートナー センター | パートナー センター"
description: "パートナー センター アカウントを作成するには、お客様の会社の職場アカウントが必要です。"
author: labrenne
robots: 
ms.openlocfilehash: 503d8af5d299a6dd9098fb5f7aafcf998159fb72
ms.sourcegitcommit: f4b2f1a954e865e56e89d3455f48cb6e1f80ea07
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/29/2017
---
# <a name="your-work-account-and-partner-center"></a>職場アカウントとパートナー センター  

**適用対象**

-  パートナー センター

# <a name="why-you-need-a-work-account"></a>職場アカウントが必要な理由

テナント ユーザーが Azure AD (職場アカウント) のユーザー名とパスワードを使ってパートナー センターにサインインできるように、組織の職場アカウントを新しいパートナー センター アカウントにリンクする必要があります。

会社に職場アカウントが既にある場合は、そのアカウントをパートナー センター アカウントにリンクできます。 

**注** 既存の職場アカウントの使用を決める前に、パートナー センターでの作業を必要とするアカウント内のユーザーの数を考慮してください。 パートナー センターで作業する必要がないユーザーがアカウントにいる場合、パートナー センターで作業する必要があるユーザーだけの新しいアカウントを作成することを検討してください。

職場アカウントが会社にまだない場合は、登録プロセスを通じて無料で作成できます。 **[Azure Active Directory にサインインします]** ページで **[新しいテナントを作成する]** を選択します。 新しい Azure Active Directory テナントを作成するときに、新しい職場アカウントを作成します。 Azure Active Directory は、Microsoft のシングル サインオンの ID 管理ソリューションです。

## <a name="not-sure-if-your-company-already-has-an-azure-work-account"></a>Azure 職場アカウントが会社に既にあるかどうかわからない場合

Azure 職場アカウントが会社にあるかどうかわからない場合、次の手順に従って確認します。 Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合、既に Azure 職場アカウントがある点に注意してください。
1.  Azure 管理ポータル (https://ms.portal.azure.com) にサインインする
2.  メニューから Azure Active Directory を選択し、ドメイン名を選択します。
3.  既に職場アカウントがある場合、ドメイン名が表示されます。

## <a name="using-an-existing-work-account"></a>既存の職場アカウントの使用

既存の職場アカウントを使おうとしてもサインインで問題が発生する場合、状況に最も合うシナリオを次の図から探し、推奨される手順に従います。 

![Azure 職場アカウントがあるか、もう 1 つ作成する必要がある場合](images/onboardingAADFlow.png)

Azure AD でドメインを追加する方法について詳しくは、[Azure AD でのドメインの追加または関連付けに関するページ](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)をご覧ください。

# <a name="about-microsoft-azure"></a>Microsoft Azure について

Microsoft Azure は、マイクロソフトが管理するデータセンターのグローバル ネットワークで企業がアプリケーションの構築、展開、管理に使うことができるパブリック クラウド プラットフォームです。 企業は、Azure を使って、物理的なコンピューターではなく仮想的な機能やサービスを提供する仮想 IT インフラストラクチャを構築します。 

Azure サブスクリプションを購入すると、実質的にはセキュリティで保護された専用のペースを Azure パブリック クラウド内に借りることになります。会社の物理的なビジネスを行うためにオフィス ビルのフロアを借りるのと大きな違いはありません。 オフィス ビルの所有者に対して、企業はテナントです。 

Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。 

職場アカウントには、Azure AD ユーザーとユーザーに関する情報 (パスワード、プロフィール データ、アクセス許可など) がホストされます。 職場アカウントには、グループ、アプリケーション、および会社とそのセキュリティに関連する他の情報も含まれています。 
