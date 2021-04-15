---
title: Azure CSP の管理者特権を復元する
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーが顧客の Azure CSP サブスクリプションを管理できるように、顧客がパートナーの管理者特権を復元する方法について説明します。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315849"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>顧客の Azure CSP サブスクリプションの管理者特権を復元する  

**該当するロール**

- グローバル管理者
- 管理エージェント

CSP パートナーの顧客は、自分の Azure の使用状況とシステムを、自分の代わりに CSP パートナーに管理してもらうことを望む場合がよくあります。 これを行うには、管理者特権が必要です。 一部の特権は、顧客とのリセラーの関係が確立されると付与されます。 それ以外は、顧客によってパートナーに付与されます。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP での Azure に対する管理者特権

CSP では Azure に対して 2 つのレベルの管理者特権があります。

**テナント レベルの管理者特権** (**委任された管理者特権**) - CSP パートナーは、顧客との CSP リセラーの関係を確立する際に、これらの特権を取得します。 委任された管理者特権により、CSP パートナーは顧客のテナントにアクセスできるようになり、ユーザーの追加/管理、パスワードのリセット、ユーザー ライセンスの管理などの管理機能を実行できます。

**サブスクリプション レベルの管理者特権** - CSP パートナーは、顧客のための Azure CSP サブスクリプションを作成する際に、これらの特権を取得します。 これらの特権により、CSP パートナーはこれらのサブスクリプションに完全にアクセスできるようになり、Azure リソースのプロビジョニングと管理を行うことができます。

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP パートナーの管理者特権を復元する

AdminAgents グループのオブジェクト ID を顧客に提供していれば、顧客は CSP ロールの割り当てを再作成できます。 委任された管理者特権を回復するには、顧客と協力する必要があります。

1. パートナー センター ダッシュボードにサインインし、パートナー センター メニューから **[顧客]** を選択します。

2. 協力する顧客を選択し、 **[リセラーの関係を要求する]** を選択します。 これにより、テナント管理者権限を持つ顧客へのリンクが生成されます。

3. その顧客はリンクを選択し、リセラーの関係の要求を承認する必要があります。

   :::image type="content" source="images/azure/revoke4.png" alt-text="リセラー関係の作成の電子メール サンプル":::

4. パートナーは、パートナー テナントに接続して、AdminAgents グループのオブジェクト ID を取得する必要があります。

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. **所有者またはユーザー アクセス管理者** のロールを持ち、サブスクリプション レベルでロールの割り当てを作成する権限を持っている顧客は、次のことを行います。


    1. CSP サブスクリプションが存在するテナントに接続します。
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. サブスクリプションに接続します (ユーザーがテナント内の複数のサブスクリプションに対するロールの割り当て権限を持っている場合にのみ該当)。
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"`


    3. ロールの割り当てを作成します。
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


目的が、サブスクリプション スコープではなく、リソース グループ レベルまたはリソース レベルで所有者ロールの権限を付与することである場合は、次のコマンドを使用できます。


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>次の手順

- [Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)
