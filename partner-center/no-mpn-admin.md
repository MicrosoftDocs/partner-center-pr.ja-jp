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
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277676"
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

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="[管理者] を [Azure portal] で見Azure portal。":::

4. 次のページで推奨されるソリューションを確認したら、[次へ: 詳細] を **選択し、** 必要なフィールドに入力します。
1. サポート リクエストを確認して作成します。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>シナリオ 3: MPN パートナー管理者/アカウント管理者/グローバル管理者が離社し、会社の管理者にアクセスできる他のユーザー Azure AD。 これは、アクセスの完全な損失です。

管理者の [引き継ぎ手順](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) に従って、管理されていないディレクトリを管理者Azure Active Directoryします。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>職場アカウントが会社に既にあるかどうかわからない場合

会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。

1. Azure 管理ポータル [にサインインします](https://ms.portal.azure.com)。
2. 左側 **Azure Active Directory** メニューから [ドメイン名] を選択し、[ ] **を選択します**。
既に職場アカウントがある場合、ドメイン名が表示されます。

>[!Note]
>Microsoft Azure または Office 365 のアクティブなサブスクリプションがある場合は、既に仕事用アカウントを持っているので、サインイン資格情報は、それらのサービスへのアクセスに使用されるサブスクリプションと同じである必要があります。