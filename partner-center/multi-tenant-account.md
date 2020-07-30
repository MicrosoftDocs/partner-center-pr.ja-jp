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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389517"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>パートナーセンターアカウントで複数のテナントを追加して管理する

**適用対象**

- パートナー センター

**適切なロール**

- グローバル管理者

パートナーセンターアカウントで複数の Azure AD テナントを管理する必要がある理由は多数あります。 たとえば、会社で別の会社を購入し、新しい会社の従業員がパートナーセンターを使用できるようにしたいとします。 ただし、2つの企業を別々に保つ必要があります。 この場合は、新しい会社の Azure AD テナントとパートナーのグローバルアカウント (PNG) を関連付けます。 この関連付けにより、両方の企業のユーザーがパートナーセンターで作業できるようになります。

## <a name="add-another-azure-ad-tenant-to-your-account"></a>アカウントに別の Azure AD テナントを追加する

1. 全体管理者として、パートナーセンターの[ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。
1. **設定**アイコンで、[**アカウントの設定**] を選択し、[**テナント**] を選択します。
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="テナントの関連付け"::: 

3. [**別の AD テナントを関連付ける**] を選択し、関連付けるテナントを指定します。

1. グローバル管理者として、関連付けるテナントにサインインし、関連付けを確認します。 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="テナントの関連付けの確認"::: 

5. 確認が完了すると、すべての**設定**の通知が表示されます。  [**テナント管理に戻る**] を選択すると、新しく追加されたテナントが一覧表示されます。
 
## <a name="next-steps"></a>次のステップ

- [ユーザーの追加](create-user-accounts-and-set-permissions.md)
