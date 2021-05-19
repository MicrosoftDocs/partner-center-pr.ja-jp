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
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151204"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>パートナーセンターアカウントで複数のテナントを追加して管理する


**適切なロール**: 全体管理者 |アカウント管理者

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

1. プロンプトで、関連付けるテナントにグローバル管理者としてサインインし、[確認] を **選択します**。 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="[Confirm new Azure AD association]/(新しいグループの関連付けを確認するAzure ADボタンのスクリーンショット。"::: 

   関連付けを確認すると、[すべての設定 **] メッセージ** が表示されます。 新しく追加されたテナントを表示するには、[テナント管理に戻 **る] を選択します**。 
 
>[!NOTE]
>テナントが別のアカウントに既に関連付けられている場合、テナントをアカウントパートナー センターできません。


## <a name="remove-a-tenant-from-your-account"></a>アカウントからテナントを削除する
 
1. グローバル管理者として Microsoft パートナー センター に [サインインします](https://partner.microsoft.com/dashboard)。

1. 右上にある [設定] アイコン **を選択し** 、[アカウント設定] **を選択します**。

1. 左側のウィンドウで、[テナント] **を選択します**。 [ **テナントのAzure AD管理] で**、[パートナー] タブ **を選択** します。
 
1. 関連 **付けを** 削除するテナントの横にある [削除] を選択します。

   :::image type="content" source="images/disassociate.png" alt-text="現在のテナントの関連付けとその [削除] リンクのスクリーンショット。":::

   前のスクリーンショットに示すように、プライマリテナントと現在サインインしているテナントを除き、関連付けられているすべてのテナントに対して [リンクの削除] リンクが有効になっています。 

   > [!NOTE]   
   > テナントを削除すると、そのテナントのユーザーは パートナー センター アカウントにアクセスできなくなったので、その削除はコンピテンシーに影響を与える可能性があります。 

## <a name="next-steps"></a>次の手順

- [ユーザー アカウントの作成](create-user-accounts-and-set-permissions.md)






