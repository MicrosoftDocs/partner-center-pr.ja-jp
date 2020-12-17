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
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="68562-103">顧客の Azure CSP サブスクリプションの管理者特権を復元する</span><span class="sxs-lookup"><span data-stu-id="68562-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="68562-104">**該当するロール**</span><span class="sxs-lookup"><span data-stu-id="68562-104">**Applicable roles**</span></span>

- <span data-ttu-id="68562-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="68562-105">Global admin</span></span>
- <span data-ttu-id="68562-106">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="68562-106">Admin agent</span></span>

<span data-ttu-id="68562-107">CSP パートナーの顧客は、自分の Azure の使用状況とシステムを、自分の代わりに CSP パートナーに管理してもらうことを望む場合がよくあります。</span><span class="sxs-lookup"><span data-stu-id="68562-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="68562-108">これを行うには、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="68562-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="68562-109">一部の特権は、顧客とのリセラーの関係が確立されると付与されます。</span><span class="sxs-lookup"><span data-stu-id="68562-109">Some privileges are granted these when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="68562-110">それ以外は、顧客によってパートナーに付与されます。</span><span class="sxs-lookup"><span data-stu-id="68562-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="68562-111">CSP での Azure に対する管理者特権</span><span class="sxs-lookup"><span data-stu-id="68562-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="68562-112">CSP では Azure に対して 2 つのレベルの管理者特権があります。</span><span class="sxs-lookup"><span data-stu-id="68562-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="68562-113">**テナント レベルの管理者特権** (**委任された管理者特権**) - CSP パートナーは、顧客との CSP リセラーの関係を確立する際に、これらの特権を取得します。</span><span class="sxs-lookup"><span data-stu-id="68562-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="68562-114">これにより、CSP パートナーは顧客のテナントにアクセスできるようになり、ユーザーの追加/管理、パスワードのリセット、ユーザー ライセンスの管理などの管理機能を実行できます。</span><span class="sxs-lookup"><span data-stu-id="68562-114">This gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="68562-115">**サブスクリプション レベルの管理者特権** - CSP パートナーは、顧客のための Azure CSP サブスクリプションを作成する際に、これらの特権を取得します。</span><span class="sxs-lookup"><span data-stu-id="68562-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="68562-116">これらの特権により、CSP パートナーはこれらのサブスクリプションに完全にアクセスできるようになり、Azure リソースのプロビジョニングと管理を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="68562-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="68562-117">CSP パートナーの管理者特権を復元する</span><span class="sxs-lookup"><span data-stu-id="68562-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="68562-118">委任された管理者特権を回復するには、顧客と協力する必要があります。</span><span class="sxs-lookup"><span data-stu-id="68562-118">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="68562-119">パートナー センター ダッシュボードにサインインし、パートナー センター メニューから **[顧客]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="68562-119">Sign in to Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="68562-120">協力する顧客を選択し、 **[リセラーの関係を要求する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="68562-120">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="68562-121">これにより、テナント管理者権限を持つ顧客へのリンクが生成されます。</span><span class="sxs-lookup"><span data-stu-id="68562-121">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="68562-122">そのユーザーはリンクを選択し、リセラーの関係の要求を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="68562-122">That user needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="リセラーの関係":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a><span data-ttu-id="68562-124">Azure CSP サブスクリプションの所有者として管理者エージェント グループを追加する</span><span class="sxs-lookup"><span data-stu-id="68562-124">Adding the admin agents group as an owner for the Azure CSP subscription</span></span>

<span data-ttu-id="68562-125">貴社の顧客は、Azure CSP サブスクリプション、リソース グループ、またはリソースの所有者として、貴社の管理者エージェント グループを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="68562-125">Your customer will need to add your admin agent group as the owner of a Azure CSP subscription, a Resource group or a resource.</span></span> 

1. <span data-ttu-id="68562-126">PowerShell コンソールまたは PowerShell Integrated Scripting Environment (ISE) のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="68562-126">Use either PowerShell Console or PowerShell Integrated Scripting Environment(ISE).</span></span> <span data-ttu-id="68562-127">AzureAD モジュールがインストールされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="68562-127">Ensure that AzureAD modules are installed.</span></span>

2. <span data-ttu-id="68562-128">Azure AD テナントに接続します。</span><span class="sxs-lookup"><span data-stu-id="68562-128">Connect to your Azure AD Tenant.</span></span>

   ```powershell
   Connect-AzureAD
   ```

3. <span data-ttu-id="68562-129">管理者エージェント グループの ObjectId を取得します。</span><span class="sxs-lookup"><span data-stu-id="68562-129">Get ObjectId of the Admin Agents groups.</span></span>

   ```powershell
   Get-AzureADGroup
   ```
   <span data-ttu-id="68562-130">次の手順は、顧客の会社の、Azure CSP サブスクリプションに対する所有者アクセス権を持つユーザーが実行します。</span><span class="sxs-lookup"><span data-stu-id="68562-130">The following steps are performed by the user in your customer's company who has owner access to the Azure CSP subscription.</span></span>

4. <span data-ttu-id="68562-131">Azure CSP サブスクリプションへの所有者アクセス権を持つユーザーは、自分の資格情報を使用して Azure にサインインします。</span><span class="sxs-lookup"><span data-stu-id="68562-131">The user with owner access to the Azure CSP subscription, signs into Azure using her credentials.</span></span>

   ```powershell
   Connect-AzureRmAccount
   ```

5. <span data-ttu-id="68562-132">その後、適切なリソース URI を Scope パラメーターに適用して、貴社の管理者エージェント グループを所有者として CSP Azure サブスクリプション、リソース グループ、またはリソースに追加できます。</span><span class="sxs-lookup"><span data-stu-id="68562-132">She can then add your admin agent group as owner to the CSP Azure subscription, Resource group or Resource by applying a proper Resource Uri in Scope parameter.</span></span> 

    ```powershell
    # Grant owner role at subscription level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"

    # Grant owner role at resource group level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>/resourceGroups/<Resource group name>"

    # Grant owner role at resource level
    New-AzureRmRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "<Resource Uri>"
    ```

## <a name="next-steps"></a><span data-ttu-id="68562-133">次の手順</span><span class="sxs-lookup"><span data-stu-id="68562-133">Next steps</span></span>

[<span data-ttu-id="68562-134">Azure プランのサブスクリプションとリソースを管理する</span><span class="sxs-lookup"><span data-stu-id="68562-134">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
