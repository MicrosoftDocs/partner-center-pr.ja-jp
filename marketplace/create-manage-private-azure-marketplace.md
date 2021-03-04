---
title: Azure portal でのプライベート Azure Marketplace の作成と管理
description: Azure portal でのプライベート Azure Marketplace (プレビュー) の作成と管理について説明します。 プライベート Azure Marketplace (プレビュー) を使用すると、管理者は、ユーザーが使用できるサードパーティ製のソリューションを管理できます。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756964"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="4c6b4-104">Azure portal でのプライベート Azure Marketplace の作成と管理</span><span class="sxs-lookup"><span data-stu-id="4c6b4-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="4c6b4-105">プライベート Azure Marketplace を使用すると、管理者は、ユーザーが使用できるサードパーティ製のソリューションを管理できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="4c6b4-106">これを行うには、管理者によって承認され、企業のポリシーに準拠しているオファーのみをユーザーが展開できるようにします。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="4c6b4-107">プライベート Azure Marketplace では、ユーザーはオンラインストアで準拠しているプランを検索し、購入してデプロイすることができます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="4c6b4-108">Marketplace 管理者 (割り当てられたロール) として、無効になっている空のプライベートストアから開始します。このストアで、承認されたオファーとプランを追加できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="4c6b4-109">この記事では、必要なロールを割り当てる方法、プライベートストアを作成する方法、項目を管理する方法、ユーザー要求を承認する方法、プライベート Azure Marketplace をユーザーに対して有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="4c6b4-110">プライベート Azure Marketplace はテナントレベルであるため、テナントのすべてのユーザーに同じ curated リストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="4c6b4-111">すべての Microsoft ソリューション (保証された [Linux ディストリビューション](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)を含む) は、プライベート Azure Marketplace に自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="4c6b4-112">Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4c6b4-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="4c6b4-113">テナントのグローバル管理者は、プライベートストアを管理するプライベート Azure Marketplace 管理者に **Marketplace 管理** 者ロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="4c6b4-114">プライベート Azure Marketplace 管理へのアクセスは、Marketplace 管理者ロールが割り当てられている IT 管理者のみが使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4c6b4-115">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c6b4-115">Prerequisites</span></span>

<span data-ttu-id="4c6b4-116">テナントのスコープでユーザーに Marketplace 管理者ロールを割り当てるには、次の前提条件が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="4c6b4-117">**グローバル管理者** ユーザーにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="4c6b4-118">テナントには、少なくとも1つのサブスクリプションがあります (任意の種類を指定できます)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="4c6b4-119">グローバル管理者のユーザーには、選択したサブスクリプションの **共同作成** 者ロールまたはそれ以降が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="4c6b4-120">アクセス制御 (IAM) を使用して Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4c6b4-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="4c6b4-121">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="4c6b4-122">[ **すべてのサービス** ]、[ **Marketplace**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="4c6b4-123">左側のメニューから [ **プライベートマーケットプレース** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="4c6b4-124">[![Marketplace の左側に [プライベートマーケットプレース] メニューオプションが表示されます。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="4c6b4-125">Marketplace 管理者ロールを割り当てるには、[ **アクセス制御 (IAM)** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="I A M アクセス制御画面を表示します。":::

1. <span data-ttu-id="4c6b4-127">**[+ 追加]**  >  **[ロール割り当ての追加]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="4c6b4-128">[ **ロール**] で、[ **Marketplace 管理**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="ロールの割り当てメニューを表示します。":::

1. <span data-ttu-id="4c6b4-130">ドロップダウンリストから目的のユーザーを選択し、[ **完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="4c6b4-131">PowerShell を使用して Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4c6b4-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="4c6b4-132">Marketplace 管理者ロールを割り当てるには、次の PowerShell スクリプトを使用します。次のパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="4c6b4-133">**TenantId:** スコープ内のテナントの ID (Marketplace 管理者ロールはテナントのスコープで割り当て可能)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="4c6b4-134">**SubscriptionId:** 全体管理者に **共同作成者** ロールが割り当てられているサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="4c6b4-135">**Globaladminusername:** グローバル管理者のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="4c6b4-136">**UsernameToAssignRoleFor:** Marketplace 管理者ロールが割り当てられるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="4c6b4-137">テナントに招待されたゲストユーザーについては、Marketplace 管理者ロールを割り当てるためにアカウントが使用できるようになるまで、最大で48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="4c6b4-138">詳細については、「 [AZURE ACTIVE DIRECTORY B2B コラボレーションユーザーのプロパティ](/azure/active-directory/b2b/user-properties)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

<span data-ttu-id="4c6b4-139">Az. Portal PowerShell モジュールに含まれるコマンドレットの詳細については、「 [Microsoft Azure PowerShell: ポータルのダッシュボードのコマンドレット](/powershell/module/az.portal/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="4c6b4-140">プライベート Azure Marketplace を作成する</span><span class="sxs-lookup"><span data-stu-id="4c6b4-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="4c6b4-141">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="4c6b4-142">[ **すべてのサービス** ]、[ **Marketplace**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure portal のメインウィンドウを表示します。":::

3. <span data-ttu-id="4c6b4-144">左側のメニューから [ **プライベートマーケットプレース** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="4c6b4-145">[ **はじめ** に] を選択してプライベート Azure Marketplace を作成します (これを行う必要があるのは1回だけです)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="[Azure portal の開始] メインウィンドウを選択する方法について説明します。":::

    <span data-ttu-id="4c6b4-147">このテナントに対してプライベート Azure Marketplace が既に存在する場合は、[ **Marketplace の管理** ] が既定で選択されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="4c6b4-148">完了すると、プライベート Azure Marketplace が空で無効になります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空のプライベート Azure Marketplace の画面を表示します。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="4c6b4-150">ギャラリーからの項目の追加</span><span class="sxs-lookup"><span data-stu-id="4c6b4-150">Add items from gallery</span></span>

<span data-ttu-id="4c6b4-151">項目は、オファーとプランの組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="4c6b4-152">[Marketplace の管理] ページで項目を検索し、追加することができます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4c6b4-153">[ **項目の追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-153">Select **Add items**.</span></span>

2. <span data-ttu-id="4c6b4-154">**ギャラリー** を参照するか、検索フィールドを使用して目的の項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="4c6b4-155">[![ギャラリーを参照する方法、または検索フィールドを使用する方法を示します。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="4c6b4-156">既定では、新しいオファーを追加すると、現在のすべてのプランが承認済みリストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="4c6b4-157">選択した項目を追加する前に、プランの選択を変更するには、プランのタイルのドロップダウンメニューを選択し、必要なプランを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="必要なプランを更新する方法について説明します。":::

4. <span data-ttu-id="4c6b4-159">選択を行った後、左下にある [ **完了** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="4c6b4-160">Marketplace への **項目の追加** は、Microsoft 以外のプランでのみ利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="4c6b4-161">Microsoft のソリューション (動作保証済みの [Linux ディストリビューション](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)を含む) は、"既定で承認済み" としてタグ付けされ、プライベートマーケットプレースで管理することはできません。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="4c6b4-162">項目の計画の編集</span><span class="sxs-lookup"><span data-stu-id="4c6b4-162">Edit item's plans</span></span>

<span data-ttu-id="4c6b4-163">[Marketplace の管理] ページで、項目の計画を編集できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4c6b4-164">[ **プラン** ] 列で、そのアイテムのドロップダウンメニューから使用可能なプランを確認します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="4c6b4-165">チェックボックスをオンまたはオフにして、ユーザーが使用できるようにするプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="必須項目のチェックボックスをオンまたはオフにする方法について説明します。":::

> [!NOTE]
> <span data-ttu-id="4c6b4-167">各プランでは、更新を実行するために少なくとも1つのプランが選択されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="4c6b4-168">オファーに関連するすべてのプランを削除するには、プラン全体を削除します (次のセクションを参照)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="4c6b4-169">オファーの削除</span><span class="sxs-lookup"><span data-stu-id="4c6b4-169">Delete offers</span></span>

<span data-ttu-id="4c6b4-170">[Marketplace の管理] ページで、プラン名 (上の画面を参照) の横にあるチェックボックスをオンにし、[ **アイテムの削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="4c6b4-171">プライベート Azure Marketplace を有効/無効にする</span><span class="sxs-lookup"><span data-stu-id="4c6b4-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="4c6b4-172">[Marketplace の管理] ページに、次のいずれかのバナーが表示されます。これは、プライベート Azure Marketplace の現在の状態を示しています。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="&quot;状態の無効化&quot; バナーを表示します。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="[状態の有効化] バナーを表示します。":::

<span data-ttu-id="4c6b4-175">プライベート Azure Marketplace は、必要に応じて有効または無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="4c6b4-176">無効になっている場合は、[ **プライベートマーケットプレースを有効** にする] をオンにします。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="4c6b4-177">有効にする場合は、[ **プライベートマーケットプレースを無効** にする] をオンにします。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="4c6b4-178">プライベート Azure Marketplace 通知センター</span><span class="sxs-lookup"><span data-stu-id="4c6b4-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="4c6b4-179">通知センターは、次の3種類の通知で構成されており、Marketplace 管理者は通知に基づいてアクションを実行できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="4c6b4-180">承認済みリストに含まれていない項目に対するユーザーからの承認要求 (「 [プランまたはプランの追加要求](#request-to-add-offers-or-plans) 」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="4c6b4-181">承認済みリストに1つ以上のプランが既に含まれているオファーの新しいプラン通知。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="4c6b4-182">承認済みリストに含まれているがグローバル Azure Marketplace から削除された項目のプラン通知を削除しました。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="4c6b4-183">通知センターにアクセスするには:</span><span class="sxs-lookup"><span data-stu-id="4c6b4-183">To access the notification center:</span></span>

1. <span data-ttu-id="4c6b4-184">左側のメニューから [ **通知** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="4c6b4-185">[![[通知] メニューを表示します。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="4c6b4-186">その他のアクションについては、省略記号メニューを選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="[その他のオプション] メニューの結果を表示します。":::

1. <span data-ttu-id="4c6b4-188">プラン要求の場合、[ **要求の表示** ] では、特定のオファーに対するすべてのユーザー要求を確認できる承認要求フォームが開きます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="4c6b4-189">[ **承認** ] または [ **拒否**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="4c6b4-190">[![承認オプションと拒否オプションを表示します。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="4c6b4-191">ドロップダウンメニューから、承認する計画を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="4c6b4-192">コメントを追加し、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="4c6b4-193">プライベート Azure Marketplace を参照しています</span><span class="sxs-lookup"><span data-stu-id="4c6b4-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="4c6b4-194">プライベート Azure Marketplace が有効になっている場合は、Marketplace 管理者が承認したプランがユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="4c6b4-195">緑色の **承認済み** の通知は、承認されているパートナー (Microsoft 以外の) オファーを示します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="4c6b4-196">**承認された青の** 通知は、承認済みの Microsoft プラン (保証された [Linux ディストリビューション](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)を含む) を示します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="4c6b4-197">ユーザーは、承認されていないオファーと承認されていないプランをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="4c6b4-198">[![フィルターオプションを示します。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="4c6b4-199">プライベート Azure Marketplace での購入またはデプロイ</span><span class="sxs-lookup"><span data-stu-id="4c6b4-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="4c6b4-200">製品の詳細ページのエクスペリエンスは、グローバルな Azure Marketplace に似ていますが、Azure Marketplace 固有の3つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="4c6b4-201">ユーザーが承認済みのプランを選択すると、[ **作成** ] ボタンが有効になります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="4c6b4-202">[![プランを作成できることを示すオファーバナーを表示します。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="4c6b4-203">製品計画の選択が [製品の詳細] ページに表示されず、管理者が1つまたは複数のプランを承認した場合は、承認されているプランと [ **作成** ] ボタンが有効になっているバナーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="4c6b4-204">[![プランを作成し、使用可能なプランを表示できることを示すオファーバナーを表示します。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="4c6b4-205">ユーザーが承認されていないプランを選択すると、バナーはプランを未承認としてメモし、[ **作成** ] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="4c6b4-206">ユーザーは、承認されたリストにプランを追加するように要求できます (次のセクションを参照)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="4c6b4-207">オファーまたはプランの追加要求</span><span class="sxs-lookup"><span data-stu-id="4c6b4-207">Request to add offers or plans</span></span>

<span data-ttu-id="4c6b4-208">プライベート Azure Marketplace で現在承認されていないパブリックプランまたはプランを追加するように要求できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="4c6b4-209">バナーに **追加する要求** を選択して、 **アクセス要求フォーム** を開きます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="4c6b4-210">[![[追加の要求] リンクを含むバナーを表示します。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="4c6b4-211">[![オファーまたはプランのアクセス要求フォームを表示します。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="4c6b4-212">要求に追加するプランを選択します (**プラン** によっては、プランのプランを設定していないことが Marketplace 管理者に通知されます)。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="4c6b4-213">**理由** を追加し、要求を送信するための **要求** を選択します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="4c6b4-214">[![サンプルエントリを持つオファーまたはプランのアクセス要求フォームを表示します。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="4c6b4-215">要求を **取り消す** オプションを使用して、保留中の要求を示す通知がアクセス要求フォームに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="4c6b4-216">[![撤回要求リンクを含む承認済みまたは保留中のプランの一覧を表示します。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="4c6b4-217">送信されると、Marketplace 管理者が要求をレビューしてアクションを実行するために、承認要求フォームが [通知センター](#private-azure-marketplace-notification-center) に送信されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="4c6b4-218">よく寄せられる質問 (FAQ)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="4c6b4-219">Azure Policy を通じて、Marketplace のサードパーティ製アプリケーションを既にブロックしています。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="4c6b4-220">これはどのような違いがあるのでしょうか。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-220">How is this different?</span></span>

<span data-ttu-id="4c6b4-221">現在、Marketplace でサードパーティのサービスを制限する方法は2つあります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="4c6b4-222">EA ポータルまたは Azure portal を通じて、サードパーティのサービスを無効にするか、"Free または BYOL Sku のみ" に制限します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure portal でサービスを制限する方法について説明します。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="電子メールポータルでサービスを制限する方法について説明します。":::

2. <span data-ttu-id="4c6b4-225">特定の Vm のみを許可する Azure ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="4c6b4-226">Windows Vm にポリシーを適用する方法の詳細については、「Azure Resource Manager を使用して [Windows vm にポリシーを適用](https://docs.microsoft.com/azure/virtual-machines/windows/policy)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="4c6b4-227">プライベート Azure Marketplace を使用すると、特定のオファーとプランをより柔軟に制限し、許可することができます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="4c6b4-228">エンドユーザーがサードパーティのサービスをデプロイする前であっても、marketplace ギャラリーにデプロイできるかどうかをエンドユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="4c6b4-229">サードパーティのサービスのデプロイを許可するには、EA ポータルと Azure portal で Azure Marketplace をオン/有効に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="4c6b4-230">プライベート Azure Marketplace では、仮想マシンに限定されないパートナーソリューションを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="4c6b4-231">プライベート Azure Marketplace はプランレベルで調整でき、"現在および将来の計画" を設定することもできます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="4c6b4-232">プライベート Azure Marketplace では、エンドユーザーに対して、展開可能なものと配置できないものを事前に通知できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="4c6b4-233">プライベートプランとプライベート Azure Marketplace の違いは何ですか?</span><span class="sxs-lookup"><span data-stu-id="4c6b4-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="4c6b4-234">**プライベートオファー** を使用すると、発行元は、対象ユーザーにのみ表示されるプランを作成できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="4c6b4-235">これにより、カスタマイズされたソリューションを、ネゴシエートされた価格、プライベートの使用条件、および特殊な構成でプライベートに共有できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="4c6b4-236">詳細については、「 [商業市場におけるプライベートプラン](https://docs.microsoft.com/azure/marketplace/private-offers)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="4c6b4-237">Azure portal の **プライベート Azure Marketplace** を使用すると、管理者は、ユーザーが展開できるサードパーティ製ソリューションを事前に承認できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="4c6b4-238">プライベート Azure Marketplace を使用すると、ユーザーは準拠しているプランを検索、購入、デプロイすることで、Azure Marketplace のメリットを享受できます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="4c6b4-239">プライベートマーケットプレースでサブスクリプションベースのプライベートプランを管理するには、Marketplace 管理者が特定のサブスクリプションに対して最低でも "読み取り" ロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="4c6b4-240">プライベートな Azure Marketplace にプライベートプランを追加しましたが、[Marketplace の管理] タブに表示されないのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="4c6b4-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="4c6b4-241">サブスクリプションベースのプライベートプランは、一覧表示されたサブスクリプションのプライベートプランの設定でのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="4c6b4-242">プライベートプランを表示するには、グローバルサブスクリプションフィルターにすべてのサブスクリプションが表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="4c6b4-243">[![プライベートマーケットプレースフィルターを表示します。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="4c6b4-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="4c6b4-244">カスタムイメージをプライベート Azure Marketplace に含めることはできますか?</span><span class="sxs-lookup"><span data-stu-id="4c6b4-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="4c6b4-245">いいえ。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-245">No.</span></span> <span data-ttu-id="4c6b4-246">プライベート Azure Marketplace を使用すると、すべての IT 管理者は、グローバルな Azure Marketplace からサードパーティ製のソリューションを管理および制御することができます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="4c6b4-247">カスタムイメージはグローバル Azure Marketplace にはないため、IT 管理者はカスタムイメージを選択して選択することはできません。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="4c6b4-248">カスタムイメージを共有する場合は、 [共有イメージギャラリー](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries)を使用します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="4c6b4-249">ステップバイステップガイド: 共有イメージギャラリー (SIG) を作成する ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell))。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="4c6b4-250">SIG 内にイメージ定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="4c6b4-251">お客様は、[OS 状態] フィールドで [ **一般化** ] を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="4c6b4-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition))。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="4c6b4-253">管理対象イメージを共有イメージギャラリー ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)) に取り込みます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="4c6b4-254">SIG VM イメージは1つのサブスクリプションに存在します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="4c6b4-255">他のサブスクリプションで使用できるようにするには、アプリの登録 ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)) を使用します。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="4c6b4-256">発行元が Microsoft ではないにもかかわらず、一部のプランが **既定で承認** されるのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="4c6b4-257">Microsoft は、Azure での Linux およびオープンソーステクノロジをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="4c6b4-258">Azure では、保証された[Linux ディストリビューション](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)がサポートされており、仮想マシンにも価格が統合されています。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="4c6b4-259">Azure Linux エージェントは Azure Marketplace に既にプレインストールされているため、Microsoft のプランと同じように扱われます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="4c6b4-260">Microsoft のプランは既定で承認されるため、保証された Linux ディストリビューションは、プライベート Azure Marketplace では管理できず、既定で承認されます。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="4c6b4-261">サポートにお問い合せください</span><span class="sxs-lookup"><span data-stu-id="4c6b4-261">Contact support</span></span>

- <span data-ttu-id="4c6b4-262">Azure Marketplace のサポートについては、 [Microsoft Q&A](/answers/products/)にアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="4c6b4-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
