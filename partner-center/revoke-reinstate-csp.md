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
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018189"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="8c0c4-103">顧客の Azure CSP サブスクリプションの管理者特権を復元する</span><span class="sxs-lookup"><span data-stu-id="8c0c4-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="8c0c4-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="8c0c4-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8c0c4-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="8c0c4-105">Global admin</span></span>
- <span data-ttu-id="8c0c4-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="8c0c4-106">Admin agent</span></span>

<span data-ttu-id="8c0c4-107">CSP パートナーの顧客は、自分の Azure の使用状況とシステムを、自分の代わりに CSP パートナーに管理してもらうことを望む場合がよくあります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="8c0c4-108">これを行うには、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="8c0c4-109">一部の特権は、顧客とのリセラーの関係が確立されると付与されます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="8c0c4-110">それ以外は、顧客によってパートナーに付与されます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="8c0c4-111">CSP での Azure に対する管理者特権</span><span class="sxs-lookup"><span data-stu-id="8c0c4-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="8c0c4-112">CSP では Azure に対して 2 つのレベルの管理者特権があります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="8c0c4-113">**テナント レベルの管理者特権** (**委任された管理者特権**) - CSP パートナーは、顧客との CSP リセラーの関係を確立する際に、これらの特権を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="8c0c4-114">委任された管理者特権により、CSP パートナーは顧客のテナントにアクセスできるようになり、ユーザーの追加/管理、パスワードのリセット、ユーザー ライセンスの管理などの管理機能を実行できるようになります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-114">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="8c0c4-115">**サブスクリプション レベルの管理者特権** - CSP パートナーは、顧客のための Azure CSP サブスクリプションを作成する際に、これらの特権を取得します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="8c0c4-116">これらの特権により、CSP パートナーはこれらのサブスクリプションに完全にアクセスできるようになり、Azure リソースのプロビジョニングと管理を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="8c0c4-117">CSP パートナーの管理者特権を復元する</span><span class="sxs-lookup"><span data-stu-id="8c0c4-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="8c0c4-118">AdminAgents グループのオブジェクト ID を顧客に提供していれば、顧客は CSP ロールの割り当てを再作成できます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-118">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="8c0c4-119">委任された管理者特権を回復するには、顧客と協力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="8c0c4-120">パートナー センター ダッシュボードにサインインし、パートナー センター メニューから **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="8c0c4-121">協力する顧客を選択し、 **[リセラーの関係を要求する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="8c0c4-122">この操作により、テナント管理者権限を持つ顧客へのリンクが生成されます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-122">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="8c0c4-123">その顧客はリンクを選択し、リセラーの関係の要求を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="リセラー関係の作成の電子メール サンプル":::

4. <span data-ttu-id="8c0c4-125">パートナーは、パートナー テナントに接続して、AdminAgents グループのオブジェクト ID を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="8c0c4-126">**所有者またはユーザー アクセス管理者** のロールを持ち、サブスクリプション レベルでロールの割り当てを作成する権限を持っている顧客は、次のことを行います。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="8c0c4-127">CSP サブスクリプションが存在するテナントに接続します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="8c0c4-128">サブスクリプションに接続します (ユーザーがテナント内の複数のサブスクリプションに対するロールの割り当て権限を持っている場合にのみ該当)。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="8c0c4-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span><span class="sxs-lookup"><span data-stu-id="8c0c4-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="8c0c4-130">ロールの割り当てを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="8c0c4-131">目的が、サブスクリプション スコープではなく、リソース グループ レベルまたはリソース レベルで所有者ロールの権限を付与することである場合は、次のコマンドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8c0c4-131">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="8c0c4-132">次の手順</span><span class="sxs-lookup"><span data-stu-id="8c0c4-132">Next steps</span></span>

- [<span data-ttu-id="8c0c4-133">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="8c0c4-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
