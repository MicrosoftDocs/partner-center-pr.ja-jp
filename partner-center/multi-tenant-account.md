---
title: パートナーセンターアカウントにテナントを追加する
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーセンターアカウントを使用して複数のテナントを管理する
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846964"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>パートナーセンターアカウントで複数のテナントを追加して管理する

**適用対象**

- パートナー センター

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
1. **設定**アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="テナントの関連付け"::: 

3. [ **別の AD テナントを関連付ける** ] を選択し、関連付けるテナントを指定します。

1. グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="テナントの関連付けの確認"::: 

5. 確認が完了すると、すべての **設定** の通知が表示されます。  [ **テナント管理に戻る** ] を選択すると、新しく追加されたテナントが一覧表示されます。 
 

>[!NOTE]
>既に別のパートナーセンターアカウントに関連付けられている場合、そのテナントをアカウントに関連付けることはできません。

 
## <a name="next-steps"></a>次の手順

- [ユーザーの追加](create-user-accounts-and-set-permissions.md)
