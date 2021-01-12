---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントで複数の Azure AD テナントを追加、統合、または管理する方法について説明します。 いくつかの理由についても説明します。
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105556"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>パートナーセンターアカウントで複数のテナントを追加して管理する


**適切なロール**

- グローバル管理者

この機能を使用すると、自社の複数のテナントを管理し、パートナー センター アカウントに統合できます。 パートナーセンターアカウントで複数の Azure AD テナントを管理する必要がある理由は多数あります。 次に例を示します。

- 会社は別の会社を購入して、新しい会社の従業員がパートナーセンターを使用できるようにすることができます。 ただし、2つの企業を別々に保つ必要があります。 この場合は、新しい会社の Azure AD テナントとパートナーのグローバルアカウント (PGA) を関連付けます。 この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。

- 複数のテナントを使用してビジネスを実行する場合 (例: contoso.com、contoso.uk、contoso.in)、マルチテナントを使用して同じ PC アカウントで関連付けることができます。

- 合併と買収には複数のテナントを使用する必要があります (Contoso が Fabrikam を買収する場合は、Constoso.com と Fabrikam.com の両方のテナントを使用できるようにする必要があります)。

- いずれかのテナントのユーザーは、次の操作を実行できる必要があります。
    1.  トレーニング、デジタルダウンロード、MCP アソシエーションのためのパートナーセンターへのアクセス
    2.  MPN Admin、インセンティブ管理者などのパートナーセンターの役割を割り当てられます。


## <a name="add-another-azure-ad-tenant-to-your-account"></a>アカウントに別の Azure AD テナントを追加する

1. 全体管理者として、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。
1. **設定** アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="テナントの関連付け"::: 

3. [ **別の AD テナントを関連付ける** ] を選択し、関連付けるテナントを指定します。

1. グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="テナントの関連付けの確認"::: 

5. 確認が完了すると、すべての **設定** の通知が表示されます。  [ **テナント管理に戻る** ] を選択すると、新しく追加されたテナントが一覧表示されます。 
 

>[!NOTE]
>既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。


## <a name="remove-a-tenant-from-your-account"></a>アカウントからテナントを削除する
 
1. 全体管理者として、パートナーセンターの [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

1. **設定** アイコンで、[**アカウントの設定**-> テナント] を選択し、[**パートナー** ] タブをクリックします。
 
3. 関連付けを解除するテナントの [ **削除** ] をクリックします。

4. 関連付け a テナントは、そのテナントのユーザーがパートナーセンターアカウントにアクセスできなくなることを意味します。これは、コンピテンシーに影響を与える可能性があります。 

[ **削除** ] ボタンは、現在サインインしているプライマリテナントとテナントを除く、関連付けられているすべてのテナントに対して有効になっています。

:::image type="content" source="images/disassociate.png" alt-text="[削除] ボタンがあるテナント":::
 

## <a name="next-steps"></a>次のステップ

- [ユーザーの追加](create-user-accounts-and-set-permissions.md)






