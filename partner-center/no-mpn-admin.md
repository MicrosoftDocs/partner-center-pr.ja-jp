---
title: MPN プログラムの唯一の管理者が離社した場合は、どうしますか?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 新しい MPN 管理者を見つけるか、会社のグローバル管理者から支援を受けるために行う方法について学習します。また、グローバル管理者に新しいアカウントをパートナー センターする方法も確認してください。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5efd157078acd72ca47418aaa9559a678fc5b129
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151170"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN プログラムの唯一の管理者が離社した場合は、どうしますか?

**適切な** ロール: MPN パートナー管理者|アカウント管理者|グローバル管理者

次の記事では、MPN 管理者が離社した場合の対応方法に関する 3 つの一般的なシナリオについて説明します。

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>シナリオ 1: MPN パートナー管理者/アカウント管理者が会社を離しましたが、アカウントにグローバル管理者がまだ存在する

この場合、会社の別のユーザーに MPN パートナー管理者のロールを割り当てることができます。特定の MPN パートナー管理者/アカウント管理者ロールのロールを割り当てるには:

1. 自分の仕事用パートナー センターアカウント (例: ) を使用して、自分のアカウントにサインインします tom@contoso.com 。
1. [グローバル **管理者] の [** ユーザー管理] ページ フィルターから、会社のグローバル管理者を確認します。 
1. グローバル管理者の 1 人に問い合わせ、必要な MPN 固有のロールの割り当てをお願いします。 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>シナリオ 2: MPN パートナー管理者/アカウント管理者が離社し、アカウントにグローバル管理者がいない 

[ユーザー管理]ページに移動してグローバル管理者をフィルター処理したが、MPN 固有のロールを取得するのに役立つグローバル管理者が会社にいない場合は、次の手順に従います。

1. [] [portal.azure.com](https://ms.portal.azure.com/)に移動し、自分の仕事用アカウント (例: ) でサインインします tom@contoso.com 。 
1. 左側の **メニュー ナビゲーション バーの [** ヘルプとサポート] オプションを選択します。
1. 次のページで、ドロップダウン メニューで [新しい **Support requestと技術的** な問題の種類] を選択し、追加の詳細を挿入し、[次へ: ソリューション] を **クリックします。**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure portal で管理者を見つける":::

4. 次のページで推奨されるソリューションを確認したら、[次へ: 詳細] を **選択し、** 必要なフィールドに入力します。
1. サポート リクエストを確認して作成します。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>シナリオ 3: MPN Partner admin/Account admin/Global admin が会社を退職し、会社の Azure AD にアクセスできる他のユーザーがいない。 これにより、完全なアクセスが失われます。

[管理者の引き継ぎ](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover)手順に従って、管理されていないディレクトリを Azure Active Directory 管理者として引き継ぎます。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>職場アカウントが会社に既にあるかどうかわからない場合

会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。

1. [Azure 管理ポータル](https://ms.portal.azure.com)にサインインします。
2. 左側のメニューから [ **Azure Active Directory** ] を選択し、[ **ドメイン名**] を選択します。
既に職場アカウントがある場合、ドメイン名が表示されます。

>[!Note]
>Microsoft Azure または Office 365 へのアクティブなサブスクリプションがある場合は、既に職場アカウントを持っていて、サインイン資格情報がこれらのサービスへのアクセスに使用したものと同じである必要があります。