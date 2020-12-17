---
title: Azure CSP の管理者特権を復元する
ms.topic: how-to
ms.date: 07/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーが顧客の Azure CSP サブスクリプションを管理できるように、顧客がパートナーの管理者特権を復元する方法について説明します。
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 13fdeb01ecd73dc1a63d174a4ad5cb8e1bdc813a
ms.sourcegitcommit: 455894365fa488368f7572ac72312e84a267ef5e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/10/2020
ms.locfileid: "97011504"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>顧客の Azure CSP サブスクリプションの管理者特権を復元する  

**該当するロール**

- グローバル管理者
- 管理エージェント

CSP パートナーの顧客は、自分の Azure の使用状況とシステムを、自分の代わりに CSP パートナーに管理してもらうことを望む場合がよくあります。 これを行うには、管理者特権が必要です。 一部の特権は、顧客とのリセラーの関係が確立されると付与されます。 それ以外は、顧客によってパートナーに付与されます。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP での Azure に対する管理者特権

CSP では Azure に対して 2 つのレベルの管理者特権があります。

**テナント レベルの管理者特権** (**委任された管理者特権**) - CSP パートナーは、顧客との CSP リセラーの関係を確立する際に、これらの特権を取得します。 これにより、CSP パートナーは顧客のテナントにアクセスできるようになり、ユーザーの追加/管理、パスワードのリセット、ユーザー ライセンスの管理などの管理機能を実行できます。

**サブスクリプション レベルの管理者特権** - CSP パートナーは、顧客のための Azure CSP サブスクリプションを作成する際に、これらの特権を取得します。 これらの特権により、CSP パートナーはこれらのサブスクリプションに完全にアクセスできるようになり、Azure リソースのプロビジョニングと管理を行うことができます。

## <a name="reinstate-csp-partners-admin-privileges"></a>CSP パートナーの管理者特権を復元する

委任された管理者特権を回復するには、顧客と協力する必要があります。

1. パートナー センター ダッシュボードにサインインし、パートナー センター メニューから **[顧客]** を選択します。

2. 協力する顧客を選択し、 **[リセラーの関係を要求する]** を選択します。 これにより、テナント管理者権限を持つ顧客へのリンクが生成されます。

3. そのユーザーはリンクを選択し、リセラーの関係の要求を承認する必要があります。

   :::image type="content" source="images/azure/revoke4.png" alt-text="リセラーの関係":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Azure CSP サブスクリプションの所有者として管理者エージェント グループを追加する

貴社の顧客は、Azure CSP サブスクリプション、リソース グループ、またはリソースの所有者として、貴社の管理者エージェント グループを追加する必要があります。 

1. PowerShell コンソールまたは PowerShell Integrated Scripting Environment (ISE) のいずれかを使用します。 AzureAD モジュールがインストールされていることを確認します。

2. Azure AD テナントに接続します。

   ```powershell
   Connect-AzureAD
   ```

3. 管理者エージェント グループの ObjectId を取得します。

   ```powershell
   Get-AzureADGroup
   ```
   次の手順は、顧客の会社の、Azure CSP サブスクリプションに対する所有者アクセス権を持つユーザーが実行します。

4. Azure CSP サブスクリプションへの所有者アクセス権を持つユーザーは、自分の資格情報を使用して Azure にサインインします。

   ```powershell
   Connect-AzureRmAccount
   ```

5. その後、適切なリソース URI を Scope パラメーターに適用して、貴社の管理者エージェント グループを所有者として CSP Azure サブスクリプション、リソース グループ、またはリソースに追加できます。 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a>次の手順

[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)
