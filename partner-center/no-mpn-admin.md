---
title: MPN プログラムの唯一の管理者が退職した場合の対処方法
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 新しい MPN 管理者を見つける方法、または会社のグローバル管理者から支援を受ける方法について説明します。また、新しいパートナーセンターのグローバル管理者を追加する方法についても説明します。
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 03cd603cf65b1e999cf95fd10d76e6ccc6c403e8
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999336"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>MPN プログラムの唯一の管理者が退職した場合の対処方法

**適用対象**

- パートナー センター

次の記事では、MPN 管理者が退職した場合の対処方法に関する3つの一般的なシナリオについて説明します。

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>シナリオ 1: MPN Partner Admin/Account Admin が会社を退職したが、まだグローバル管理者がアカウントに存在する

この場合、会社の別のユーザーに MPN Partner admin の役割を割り当てることができます。特定の MPN Partner admin/Account Admin ロールのロールを割り当てるには、次のようにします。

1. 職場アカウントを使用してパートナーセンターアカウントにサインインします (例: tom@contoso.com )。
1. グローバル管理者の [ **ユーザー管理** ] ページフィルターを使用して、会社のグローバル管理者を確認します。 
1. グローバル管理者のいずれかに問い合わせて、必要な MPN 固有のロールを割り当てるように依頼してください。 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>シナリオ 2: MPN Partner Admin/Account Admin が退職し、アカウントにグローバル管理者が存在しない 

[ **ユーザー管理** ] ページにアクセスしてグローバル管理者をフィルター処理しても、MPN 固有のロールを取得するのに役立つグローバル管理者が会社にないことがわかった場合は、次の手順を実行します。

1. [Portal.azure.com](https://ms.portal.azure.com/)にアクセスし、職場のアカウント (など) でサインイン tom@contoso.com します。 
1. 左側のメニューのナビゲーションバーで [ **ヘルプとサポート** ] オプションを選択します。
1. 次のページで、ドロップダウンメニューの [ **新しい Support request** と **技術面の問題** の種類] を選択し、追加の詳細を挿入して、[次へ] をクリックします。 **ソリューション。**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Azure portal で管理者を見つける":::

4. 次のページで推奨されているソリューションを確認したら、[ **次へ: 詳細** ] を選択し、必要なフィールドを入力します。
1. サポートリクエストを確認して作成します。


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>シナリオ 3: MPN Partner admin/Account admin/Global admin が会社を退職し、会社の Azure AD にアクセスできる他のユーザーがいない。 これにより、完全なアクセスが失われます。

[管理者の引き継ぎ](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover)手順に従って、管理されていないディレクトリを Azure Active Directory 管理者として引き継ぎます。

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>職場アカウントが会社に既にあるかどうかわからない場合

会社に職場アカウントがあるかどうかわからない場合は、次の手順に従って確認します。

1. [Azure 管理ポータル](https://ms.portal.azure.com)にサインインします。
2. 左側のメニューから [ **Azure Active Directory** ] を選択し、[ **ドメイン名**] を選択します。
既に職場アカウントがある場合、ドメイン名が表示されます。

>[!Note]
>Microsoft Azure または Office 365 へのアクティブなサブスクリプションがある場合は、既に職場アカウントを持っていて、サインイン資格情報がこれらのサービスへのアクセスに使用したものと同じである必要があります。