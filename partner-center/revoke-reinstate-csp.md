---
title: Azure CSP サブスクリプションの管理者特権を復元する | パートナー センター
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: このドキュメントでは、顧客がパートナーの管理者特権を復元する方法について説明します
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 1bcbcf32e3b3f4513ed3e55984b49b090da4a734
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651711"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Azure CSP サブスクリプションの管理者特権を復元する  

**該当するロール**

- 全体管理者
- 管理エージェント

CSP パートナーの顧客は、自分の Azure の使用状況とシステムを、自分の代わりに CSP パートナーに管理してもらうことを望む場合がよくあります。 これを行うには、パートナーに管理者特権が必要です。 一部の特権は、顧客とのリセラーの関係が確立されると付与されます。 それ以外は、顧客によってパートナーに付与されます。

## <a name="admin-privileges-for-azure-in-csp"></a>CSP での Azure に対する管理者特権 

CSP では Azure に対して 2 つのレベルの管理者特権があります。 

**テナント レベルの管理者特権** (**委任された管理者特権**) - CSP パートナーは、顧客との CSP リセラーの関係を確立する際に、これらの特権を取得します。 これにより、CSP パートナーは顧客のテナントにアクセスできるようになり、ユーザーの追加/管理、パスワードのリセット、ユーザー ライセンスの管理などの管理機能を実行できます。 

**サブスクリプション レベルの管理者特権** - CSP パートナーは、顧客のための Azure CSP サブスクリプションを作成する際に、これらの特権を取得します。 これにより、CSP パートナーはこれらのサブスクリプションに完全にアクセスできるようになり、Azure リソースのプロビジョニングと管理を行うことができます。 


## <a name="reinstate-csp-partners-admin-privileges"></a>CSP パートナーの管理者特権を復元する

委任された管理者特権を回復するには、顧客と協力する必要があります。
 
 1. パートナー センター ダッシュボードにサインインし、パートナー センター メニューから **[顧客]** を選択します。

 2. 協力する顧客を選択し、 **[リセラーの関係を要求する]** を選択します。 これにより、テナント管理者権限を持つ顧客へのリンクが生成されます。

 3. そのユーザーはリンクを選択し、リセラーの関係の要求を承認する必要があります。
 
![リセラーの関係](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Azure CSP サブスクリプションの所有者として管理者エージェント グループを追加する

 顧客は、Azure CSP サブスクリプションの所有者として、パートナーの管理者エージェント グループを追加する必要があります。

1. PowerShell コンソールまたは PowerShell Integrated Scripting Environment (ISE) のいずれかを使用します。 AzureRM モジュールと AzureAD モジュールがインストールされていることを確認します。 

2.  Azure AD テナントに接続します。
PowerShell コマンドレット: Connect-AzureAD

3.  管理者エージェント グループの ObjectId を取得します。
PowerShell コマンドレット: Get-AzureADGroup`1nn

![管理者エージェント グループ](images/azure/revoke5.png)

次の手順は、顧客の会社の、Azure CSP サブスクリプションに対する所有者アクセス権を持つユーザーが実行します。

4. Azure CSP サブスクリプションへの所有者アクセス権を持つユーザーは、自分の資格情報を使用して Azure Resource Manager にサインインします。

    PowerShell コマンドレット: Login-AzureRMAccount

5.  その後、パートナーの管理者エージェント グループを、CSP Azure サブスクリプションに所有者として追加できます。

    PowerShell コマンドレット: New-AzureRMRoleAssignment -ObjectId <ステップ 3 で取得したオブジェクト ID> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![管理者エージェント所有者](images/azure/revoke6.png)    

**詳細情報**

[Azure プランのサブスクリプションとリソースを管理する](azure-plan-manage.md)
