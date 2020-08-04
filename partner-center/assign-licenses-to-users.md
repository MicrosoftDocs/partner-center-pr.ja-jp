---
title: 顧客アカウントのユーザーを管理する
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 顧客のユーザーアカウントを作成する方法、ユーザーライセンスを追加または削除する方法、ユーザーパスワードをリセットする方法、ユーザーアカウントを削除する方法、または復元する方法について説明します。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527678"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a>パートナーセンターでの顧客アカウントのユーザー管理タスク

**適用対象**

- パートナー センター

**適切なロール**

- グローバル管理者
- ユーザー管理の管理者
- 管理エージェント
- 販売代理店
- ヘルプデスク エージェント

顧客のアカウントで新しいユーザーを作成および削除することができます。 また、削除後30日以内に削除した1つ以上のユーザーアカウントを復元することもできます。 ユーザーの以前のサブスクリプションの割り当ても (以前の割り当てが利用可能な場合は) 復元されます。

顧客の新しいサブスクリプションを購入する場合、顧客は、アカウントを必要とするすべてのユーザー、ユーザーのアクセス許可、および各ユーザーが必要とするサービスの一覧を提供する必要があります。  

一度に[複数のユーザーにサブスクリプションを割り当てる](bulk-license-provisioning-for-multiple-users.md)ことができます。これには、[Excel 互換の .csv スプレッドシート ファイル](adding-multiple-users-to-a-customer-account.md) を使って、名前をインポートします。

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>顧客のユーザー アカウントを作成する

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

2. パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。

3. 顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。

4. 追加するユーザーごとに、**[サブスクリプションの追加]** を選び、アクセス許可やライセンスなどの情報を入力します。 変更内容を**保存**します。

5. 必ずユーザー名と一時パスワードを記録してユーザーに送信してください。

6. 複数のユーザーを 1 人ずつ追加する場合は、**[別のユーザーの追加]** を使います。

7. 一度に複数のユーザーを追加することもできます。これには、[Excel 互換の .csv スプレッドシート ファイルをインポート](adding-multiple-users-to-a-customer-account.md)します。 すべてのユーザーの設定が完了するまで待ち、その後で、確認画面からユーザー名とパスワードを電子メールで送信したり印刷したりすることができます。

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>顧客のユーザー ライセンスを追加または削除する

次の手順は、Microsoft 製品のユーザーライセンスを追加または削除する場合に適用されます。 商用マーケットプレースでライセンスベースの SaaS サブスクリプションのユーザーライセンスを追加または削除するには、「 [saas サブスクリプションのライセンスを追加または削除](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)する」を参照してください。

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

2. パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。

3. 顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。

4. 一覧から 1 人以上のユーザーを選びます。 たとえば、顧客が新しいライセンスを購入したばかりで、まだライセンスを持っていないユーザーにライセンスを割り当てる場合、**[Filter users by...]** (ユーザーのフィルター条件) オプションを使って適切なグループを見つけます。

5. **[ライセンスの管理]** を選びます。 変更を加えてから、**[保存]** を選びます。

> [!NOTE]
> [Azure Marketplace 製品](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)の場合、ライセンスの割り当てとライセンス認証は、製品を発行した独立系ソフトウェアベンダー (ISV) によって管理されます。

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>顧客のユーザー パスワードをリセットする

1. パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard)にサインインします。

2. パートナー センター メニューから **[顧客]** を選択し、一覧から顧客を選びます。

3.  顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。 一覧からユーザーを選択します。

4.  画面の下部で **[パスワードのリセット]** を選びます。 

5.  新しい一時的なパスワードをユーザーに送信します。

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>顧客のユーザー アカウントを削除する

1.  **パートナー センター** メニューで、**[顧客]** を選択します。 一覧から顧客を選択します。

2.  顧客メニューで、**[Users and Licenses]\(ユーザーとライセンス\)** を選択します。 一覧からユーザーを選択します。

3.  画面の下部にある **[ユーザー アカウントの削除]** を選択します。

このアカウントを復元する必要が生じた場合、顧客の **[ユーザーとライセンス]** の一覧の **[削除されたアカウント]** タブで見つけることができます。 削除したユーザーを復元できるのは、削除から 30 日以内です。

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>削除されたユーザー アカウントを復元する

1.  **パートナー センター** メニューの **[顧客]** を選択し、一覧から顧客を選びます。

2.  [**ユーザーとライセンス**] を選択します。

3.  **[削除したユーザー ( 人)]** タブを選びます。復元できる削除済みユーザーが存在する場合は、**(1)** 以上の数値が表示されます。

4.  削除されたユーザーのチェック ボックスを 1 つ以上を選択し、**[復元]** を選びます。

    選択したすべてのユーザー アカウントが、**[ユーザーとライセンス]** ページに再び表示されます。

## <a name="related-topics"></a>関連トピック


[複数のユーザーへのライセンスの割り当てまたは取り消し](bulk-license-provisioning-for-multiple-users.md)

[顧客のアカウントに複数のユーザーを作成する](adding-multiple-users-to-a-customer-account.md)