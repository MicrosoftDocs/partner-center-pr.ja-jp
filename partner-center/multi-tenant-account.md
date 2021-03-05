---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントで複数の Azure AD テナントを追加、統合、または管理する方法と、その方法について説明します。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124807"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>パートナーセンターアカウントで複数のテナントを追加して管理する


**適切なロール**

- グローバル管理者
- アカウント管理者

この記事では、会社の複数の Azure Active Directory (Azure AD) テナントを統合し、パートナーセンターアカウントで追加および管理する方法について説明します。 これには多くの理由があります。 次に例を示します。

- Contoso 社が Fabrikam という別の会社を買収したとします。 2つの会社を別々に残しておく必要があり、新しい従業員がパートナーセンターを使用できるようにする必要があるとします。 この場合は、新しい会社の Azure AD テナントをパートナーのグローバルアカウント (PGA) に関連付けます。 この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。

- 複数のテナント (たとえば、 *contoso.com*、 *contoso.uk*、 *contoso.in*) を使用してビジネスを実行する場合は、マルチテナント機能を使用して同じ PC アカウントでそれらをグループ化できます。

- 合併と買収のガイドラインで両方の企業のテナントを操作する必要がある場合は、 *constoso.com* テナントと *fabrikam.com* テナントの両方を使用します。

- テナントのユーザーは、次のことができる必要があります。
    * トレーニング、デジタルダウンロード、または Microsoft 認定プロフェッショナル (MCP) のアソシエーションのパートナーセンターにアクセスします。
    * Microsoft Partner Network (MPN) 管理者やインセンティブ管理者などのパートナーセンターの役割が割り当てられている。

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Azure AD テナントをアカウントに追加する

1. グローバル管理者として [Microsoft パートナーセンター](https://partner.microsoft.com/dashboard)にサインインします。

1. 右上にある [ **設定**] を選択し、[ **アカウントの設定**] を選択して、[ **テナント**] を選択します。
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Azure AD プロファイル] ウィンドウの [関連付け] ボタンのスクリーンショット。"::: 

1. [ **関連付け**] を選択し、関連付けるテナントを指定します。

1. プロンプトで、関連付けるテナントにグローバル管理者としてサインインし、[ **確認**] を選択します。 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[新しい Azure AD の関連付けの確認] ウィンドウの [確認] ボタンのスクリーンショット。"::: 

   関連付けを確認すると、すべての **設定** メッセージが表示されます。 新しく追加されたテナントを表示するには、[ **テナント管理に戻る**] を選択します。 
 
>[!NOTE]
>既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。


## <a name="remove-a-tenant-from-your-account"></a>アカウントからテナントを削除する
 
1. グローバル管理者として [Microsoft パートナーセンター](https://partner.microsoft.com/dashboard)にサインインします。

1. 右上にある [ **設定** ] アイコンを選択し、[ **アカウントの設定**] を選択します。

1. 左側のウィンドウで、[ **テナント**] を選択します。 [ **Azure AD テナントの管理**] で、[ **パートナー** ] タブを選択します。
 
1. 関連付けを削除するテナントの横にある [ **削除** ] を選択します。

   :::image type="content" source="images/disassociate.png" alt-text="現在のテナントの関連付けとその削除リンクのスクリーンショット。":::

   前のスクリーンショットに示されているように、関連付けられているすべてのテナントに対して [ **削除** ] リンクが有効になっています。ただし、プライマリテナントと、現在サインインしているテナントは除きます。 

   > [!NOTE]   
   > テナントを削除すると、そのテナントのユーザーはパートナーセンターアカウントにアクセスできなくなり、削除がコンピテンシーに影響を与える可能性があります。 

## <a name="next-steps"></a>次の手順

- [ユーザー アカウントの作成](create-user-accounts-and-set-permissions.md)






