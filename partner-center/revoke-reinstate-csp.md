---
title: Azure CSP の管理者特権を復元する
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナーが顧客の Azure CSP サブスクリプションを管理できるように、顧客がパートナーの管理者特権を復元する方法について説明します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6ffc6f4203d43a756dc3a0bf1de65eeda3d41d
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909100"
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

顧客は、Azure CSP サブスクリプションの所有者として、パートナーの管理者エージェント グループを追加する必要があります。

1. PowerShell コンソールまたは PowerShell Integrated Scripting Environment (ISE) のいずれかを使用します。 AzureRM モジュールと AzureAD モジュールがインストールされていることを確認します。

2. Azure AD テナントに接続します。

   ```powershell
   Connect-AzureAD
   ```

3. 管理者エージェント グループの ObjectId を取得します。

   ```powershell
   Get-AzureADGroup
   ```

   :::image type="content" source="images/azure/revoke5.png" alt-text="管理者エージェント グループ":::

   次の手順は、顧客の会社の、Azure CSP サブスクリプションに対する所有者アクセス権を持つユーザーが実行します。

4. Azure CSP サブスクリプションへの所有者アクセス権を持つユーザーは、自分の資格情報を使用して Azure Resource Manager にサインインします。

   ```powershell
   Login-AzureRMAccount
   ```

5. その後、パートナーの管理者エージェント グループを、CSP Azure サブスクリプションに所有者として追加できます。

    ```powershell
    New-AzureRMRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

   :::image type="content" source="images/azure/revoke6.png" alt-text="管理者エージェント所有者":::

## <a name="next-steps"></a>次の手順

[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)
