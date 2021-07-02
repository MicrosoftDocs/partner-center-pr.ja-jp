---
title: 次の方法でプライベート Azure Marketplaceを作成および管理Azure portal
description: このページでは、プライベート Azure Marketplace (プレビュー) の作成と管理についてAzure portal。 プライベート Azure Marketplace (プレビュー) を使用すると、管理者は、ユーザーが使用できるサードパーティのソリューションを管理できます。
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173688"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="4dcda-104">次の方法でプライベート Azure Marketplaceを作成および管理Azure portal</span><span class="sxs-lookup"><span data-stu-id="4dcda-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="4dcda-105">プライベート Azure Marketplaceを使用すると、ユーザーが使用できるサードパーティのソリューションを管理者が管理できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="4dcda-106">これを行うのは、管理者によって承認され、企業のポリシーに準拠しているオファーのみをユーザーが展開できるようにすることで行います。</span><span class="sxs-lookup"><span data-stu-id="4dcda-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="4dcda-107">Private Azure Marketplaceを使用すると、ユーザーはオンライン ストアで準拠しているオファーを検索して購入およびデプロイできます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="4dcda-108">Marketplace 管理者 (割り当てられたロール) は、無効で空のプライベート ストアから始め、承認されたオファーとプランを追加できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="4dcda-109">この記事では、必要なロールの割り当て、プライベート ストアの作成、アイテムの管理、ユーザー要求の承認、ユーザーに対するプライベート Azure Marketplaceの有効化を行う方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="4dcda-110">プライベート Azure Marketplaceはテナント レベルなので、テナントのすべてのユーザーに同じキュキュされた一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="4dcda-111">すべての Microsoft ソリューション ( [サポートされている Linux ディストリビューション](/azure/virtual-machines/linux/endorsed-distros)を含む) は、Private Azure Marketplace に追加されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-111">All Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="4dcda-112">Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4dcda-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="4dcda-113">テナントグローバル管理者は、プライベート ストアを管理するプライベート 管理者に **Marketplace** Azure Marketplaceロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="4dcda-114">プライベート アカウント管理Azure Marketplace、Marketplace 管理者ロールが割り当てられている IT 管理者だけが使用できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="4dcda-115">[前提条件]</span><span class="sxs-lookup"><span data-stu-id="4dcda-115">Prerequisites</span></span>

<span data-ttu-id="4dcda-116">テナント スコープのユーザーに Marketplace 管理者ロールを割り当てる前に、次の前提条件が必要です。</span><span class="sxs-lookup"><span data-stu-id="4dcda-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="4dcda-117">グローバル管理者ユーザーに **アクセス** できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="4dcda-118">テナントには、少なくとも 1 つのサブスクリプションがあります (任意の種類を指定できます)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="4dcda-119">グローバル管理者ユーザーには、選択したサブスクリプションの **共同** 作成者ロール以上が割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="4dcda-120">アクセス制御 (IAM) を使用して Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4dcda-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="4dcda-121">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4dcda-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

1. <span data-ttu-id="4dcda-122">[すべての **サービス] を選択し\*\*\*\*、[Marketplace] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-122">Select **All services** and then **Marketplace**.</span></span>

1. <span data-ttu-id="4dcda-123">左側 **のメニューから** [プライベート マーケットプレース] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-123">Select **Private Marketplace** from the menu on the left.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Marketplace の左側にプライベート マーケットプレース メニュー オプションが表示されます。":::

1. <span data-ttu-id="4dcda-125">[ **アクセス制御 (IAM)] を選択して** Marketplace 管理者ロールを割り当てる。</span><span class="sxs-lookup"><span data-stu-id="4dcda-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="[I A M アクセス制御] 画面が表示されます。":::

1. <span data-ttu-id="4dcda-127">**[+ 追加]**  >  **[ロール割り当ての追加]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-127">Select **+ Add** > **Add role assignment**.</span></span>

1. <span data-ttu-id="4dcda-128">[ロール **] で\*\*\*\*、[Marketplace 管理者] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="[ロールの割り当て] メニューが表示されます。":::

1. <span data-ttu-id="4dcda-130">ドロップダウン リストから目的のユーザーを選択し、[完了] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="4dcda-131">PowerShell を使用して Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="4dcda-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="4dcda-132">Marketplace 管理者ロールを割り当てるには、次の PowerShell スクリプトを使用します。次のパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="4dcda-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="4dcda-133">**TenantId:** スコープ内のテナントの ID (Marketplace 管理者ロールはテナント スコープで割り当て可能)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="4dcda-134">**SubscriptionId:** グローバル管理者に共同作成者ロール **以上が割** り当てられているサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="4dcda-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="4dcda-135">**GlobalAdminUsername:** グローバル管理者のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="4dcda-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="4dcda-136">**UsernameToAssignRoleFor:** Marketplace 管理者ロールを割り当てるユーザー名。</span><span class="sxs-lookup"><span data-stu-id="4dcda-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="4dcda-137">テナントに招待されたゲスト ユーザーの場合、自分のアカウントが Marketplace 管理者ロールを割り当て可能になるまで、最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="4dcda-138">詳細については[、「B2B コラボレーション ユーザーのAzure Active Directory」を参照してください](/azure/active-directory/b2b/user-properties)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="4dcda-139">Az.Portal PowerShell モジュールに含まれているコマンドレットの詳細については、「ポータル ダッシュボードコマンドレット」Microsoft Azure PowerShell[を参照してください](/powershell/module/az.portal/)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="4dcda-140">プライベート アカウントを作成Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4dcda-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="4dcda-141">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="4dcda-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="4dcda-142">[すべての **サービス] を選択し\*\*\*\*、[Marketplace] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="メイン ウィンドウAzure portalを表示します。":::

3. <span data-ttu-id="4dcda-144">左側 **のメニューから** [プライベート マーケットプレース] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="4dcda-145">**[はじめに]** を選択してプライベート Azure Marketplace作成します (これを行う必要があるのは 1 回だけです)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="メイン ウィンドウで [はじめに] をAzure portal方法を示します。":::

    <span data-ttu-id="4dcda-147">このテナントAzure Marketplaceプライベート アカウントが既に存在する場合は、既定で **[Marketplace** の管理] が選択されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="4dcda-148">完了すると、空の無効なプライベート アカウントがAzure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空の [プライベート] Azure Marketplace表示します。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="4dcda-150">ギャラリーから項目を追加する</span><span class="sxs-lookup"><span data-stu-id="4dcda-150">Add items from gallery</span></span>

<span data-ttu-id="4dcda-151">項目は、オファーとプランの組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="4dcda-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="4dcda-152">[Marketplace の管理] ページで項目を検索して追加できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4dcda-153">[項目 **の追加] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-153">Select **Add items**.</span></span>

2. <span data-ttu-id="4dcda-154">ギャラリーを **参照するか** 、検索フィールドを使用して目的の項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="ギャラリーを参照する方法、または検索フィールドを使用する方法を示します。":::

3. <span data-ttu-id="4dcda-156">既定では、新しいオファーを追加すると、現在のすべてのプランが承認済みリストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="4dcda-157">選択した項目を追加する前にプランの選択を変更するには、オファーのタイルのドロップダウン メニューを選択し、必要なプランを更新します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer's tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="必要なプランを更新する方法を示します。":::

4. <span data-ttu-id="4dcda-159">選択 **が** 完了したら、左下にある [完了] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="4dcda-160">**Marketplace への項目** の追加は、Microsoft 以外のオファーでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="4dcda-161">Microsoft ソリューション ( [承認された Linux](/azure/virtual-machines/linux/endorsed-distros)ディストリビューションを含む) は、"既定で承認済み" としてタグ付けされ、プライベート マーケットプレースでは管理できません。</span><span class="sxs-lookup"><span data-stu-id="4dcda-161">Microsoft solutions (including [Endorsed Linux Distributions](/azure/virtual-machines/linux/endorsed-distros)) will be tagged as "Approved by default" and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="4dcda-162">項目のプランを編集する</span><span class="sxs-lookup"><span data-stu-id="4dcda-162">Edit item's plans</span></span>

<span data-ttu-id="4dcda-163">項目のプランは、[Marketplace の管理] ページで編集できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="4dcda-164">[プラン **] 列** で、その項目のドロップダウン メニューから使用可能なプランを確認します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>

2. <span data-ttu-id="4dcda-165">チェック ボックスをオンまたはオフにして、ユーザーが利用できるプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="必要な項目のチェック ボックスをオンまたはオフにする方法を示します。":::

   > [!NOTE]
   > <span data-ttu-id="4dcda-167">各オファーには、更新を実行するために少なくとも 1 つのプランが選択されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="4dcda-168">オファーに関連するプランを削除するには、オファー全体を削除します (次のセクションを参照)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="4dcda-169">オファーの削除</span><span class="sxs-lookup"><span data-stu-id="4dcda-169">Delete offers</span></span>

<span data-ttu-id="4dcda-170">[Marketplace の管理] ページで、オファー名の横にあるチェック ボックス (上の画面を参照) を選択し、[ 項目の削除] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="4dcda-171">プライベート アカウントを有効または無効Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4dcda-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="4dcda-172">[Marketplace の管理] ページに、プライベート アカウントの現在の状態を示す次のいずれかのバナーがAzure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="[状態を無効にする] バナーを表示します。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="[状態を有効にする] バナーを表示します。":::

<span data-ttu-id="4dcda-175">必要に応じて、プライベート Azure Marketplace有効または無効にできます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="4dcda-176">無効になっている場合は、[プライベート **マーケットプレースを有効にする] を** 選択して有効にします。</span><span class="sxs-lookup"><span data-stu-id="4dcda-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="4dcda-177">有効になっている場合は、 [プライベート マーケット **プレースを無効にする] を選択して** 無効にします。</span><span class="sxs-lookup"><span data-stu-id="4dcda-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="4dcda-178">プライベート Azure Marketplace通知センター</span><span class="sxs-lookup"><span data-stu-id="4dcda-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="4dcda-179">Notification Center は 3 種類の通知で構成され、Marketplace 管理者は通知に基づいてアクションを実行できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="4dcda-180">承認された一覧に含されていない項目に対するユーザーからの承認要求 (以下の「オファーまたはプランの追加要求 [」を参照](#request-to-add-offers-or-plans) )。</span><span class="sxs-lookup"><span data-stu-id="4dcda-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="4dcda-181">承認済みリストに 1 つ以上のプランが既に含むオファーの新しいプラン通知。</span><span class="sxs-lookup"><span data-stu-id="4dcda-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="4dcda-182">承認済みリストに含まれていますが、グローバル リストから削除された項目のプラン通知を削除Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="4dcda-183">通知センターにアクセスするには:</span><span class="sxs-lookup"><span data-stu-id="4dcda-183">To access the notification center:</span></span>

1. <span data-ttu-id="4dcda-184">左側 **のメニュー** から [通知] を選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-184">Select **Notifications** from the left-side menu.</span></span>

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="[通知] メニューが表示されます。":::

1. <span data-ttu-id="4dcda-186">その他のアクションについては、省略記号メニューを選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="[その他のオプション] メニューの結果が表示されます。":::

1. <span data-ttu-id="4dcda-188">プラン要求の場合、[ **要求の** 表示] で承認要求フォームが開き、特定のオファーのすべてのユーザー要求を確認できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="4dcda-189">[承認 **] または [拒否** ] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-189">Select **Approve** or **Reject**.</span></span>

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="承認オプションと拒否オプションを表示します。":::

1. <span data-ttu-id="4dcda-191">ドロップダウン メニューから、承認するプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="4dcda-192">コメントを追加し、 [送信] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="4dcda-193">プライベート Azure Marketplace の参照</span><span class="sxs-lookup"><span data-stu-id="4dcda-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="4dcda-194">[プライベート Azure Marketplace有効にすると、Marketplace 管理者が承認したプランがユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="4dcda-195">緑色の **承認済み通知** は、承認されたパートナー (Microsoft 以外) オファーを示します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="4dcda-196">青色の **承認済み** 通知は、承認された Microsoft オファー (承認された [Linux](/azure/virtual-machines/linux/endorsed-distros)ディストリビューションを含む) を示します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="4dcda-197">ユーザーは、承認されていないオファーと承認されていないオファーをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-197">Users can filter between offers that are and are not approved:</span></span>

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="フィルターオプションを表示します。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="4dcda-199">プライベート サービスで購入またはデプロイAzure Marketplace</span><span class="sxs-lookup"><span data-stu-id="4dcda-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="4dcda-200">製品の詳細ページのエクスペリエンスはグローバル サービスと似ていますがAzure Marketplace、3 つのプライベート Azure Marketplaceシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="4dcda-201">ユーザーが承認されたプランを選択すると、[作成] **ボタンが** 有効になります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="プランを作成できるというオファー バナーが表示されます。":::

- <span data-ttu-id="4dcda-203">製品プランの選択内容が製品の詳細ページに表示されないが、管理者が 1 つ以上のプランを承認した場合は、承認されているプランと [作成] ボタンが有効になっているバナー メモが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="プランを作成し、使用可能なプランを表示できるオファー バナーを表示します。":::

- <span data-ttu-id="4dcda-205">ユーザーが承認されていないプランを選択すると、バナーによってプランが承認されていないと示され、[作成] **ボタンは** 無効になります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="4dcda-206">ユーザーは、承認された一覧にプランを追加する要求を引き続き行います (次のセクションを参照してください)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="4dcda-207">オファーまたはプランの追加を要求する</span><span class="sxs-lookup"><span data-stu-id="4dcda-207">Request to add offers or plans</span></span>

<span data-ttu-id="4dcda-208">プライベート プランで現在承認されていないパブリック オファーまたはプランの追加を要求Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="4dcda-209">バナー **で [要求] を選択** して追加し、 [ **アクセス要求] フォームを開きます**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="[追加する要求] リンクを含むバナーが表示されます。":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="オファーまたはプランのアクセス要求フォームを表示します。":::

1. <span data-ttu-id="4dcda-212">要求に追加するプランを選択します **([** 任意のプラン] は、オファー内のプランに対する優先設定を持たなかったと Marketplace 管理者に指示します)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="4dcda-213">理由を **追加し、[** 要求] **を選択して** 要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-213">Add a **Justification** and select **Request** to submit your request.</span></span>

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="サンプル エントリを含むオファーまたはプランのアクセス要求フォームを表示します。":::

1. <span data-ttu-id="4dcda-215">保留中の要求の兆候が [アクセス要求] フォームに表示され、要求を取り消すオプション **が表示されます**。</span><span class="sxs-lookup"><span data-stu-id="4dcda-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="[取り消し要求] リンクを含む承認済みプランまたは保留中のプランの一覧が表示されます。":::

> [!NOTE]
> <span data-ttu-id="4dcda-217">送信されると、承認要求フォームが通知センターに送信され[](#private-azure-marketplace-notification-center)、Marketplace 管理者が要求を確認してアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

> [!CAUTION]
> <span data-ttu-id="4dcda-218">プライベート マーケットプレースへの承認は、ソリューションの調達を示すのではありません。</span><span class="sxs-lookup"><span data-stu-id="4dcda-218">Approval into Private Marketplace does not indicate procurement of a solution.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="4dcda-219">よく寄せられる質問 (FAQ)</span><span class="sxs-lookup"><span data-stu-id="4dcda-219">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="4dcda-220">Marketplace のサード パーティ製アプリケーションは、既にアプリを通じてブロックAzure Policy。</span><span class="sxs-lookup"><span data-stu-id="4dcda-220">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="4dcda-221">これはどのように異なりますか?</span><span class="sxs-lookup"><span data-stu-id="4dcda-221">How is this different?</span></span>

<span data-ttu-id="4dcda-222">現在、Marketplace でサードパーティのサービスを制限するには、次の 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-222">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="4dcda-223">EA ポータルまたはポータルを使用Azure portalサード パーティのサービスを無効にするか、"Free SKU または BYOL SKU のみ" に制限します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-223">Through EA portal or the Azure portal, disable third-party services or restrict to "Free or BYOL SKUs only".</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="サービスのサービスを制限する方法をAzure portal。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="E A ポータルでサービスを制限する方法を示します。":::

2. <span data-ttu-id="4dcda-226">特定の VM のみを許可する Azure ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-226">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="4dcda-227">VM にポリシーを適用する方法の詳細については、「Windows VM にポリシーを適用するWindowsを参照[Azure Resource Manager。](/azure/virtual-machines/windows/policy)</span><span class="sxs-lookup"><span data-stu-id="4dcda-227">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="4dcda-228">プライベート Azure Marketplaceを使用すると、特定のオファーとプランを制限および許可する柔軟性が向上します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-228">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="4dcda-229">サード パーティのサービスのデプロイを試みる前でも、マーケットプレース ギャラリーでのデプロイの可用性をエンド ユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-229">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="4dcda-230">サード パーティのサービスのデプロイを許可するには、Azure Marketplace の [オン/有効] に設定EA Portal、Azure portal。</span><span class="sxs-lookup"><span data-stu-id="4dcda-230">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="4dcda-231">プライベート Azure Marketplace仮想マシンに限定されないパートナー ソリューションをキュレーションできます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-231">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="4dcda-232">プライベート Azure Marketplaceプラン レベルでキュレーションできます。また、"現在および将来のプラン" を設定できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-232">Private Azure Marketplace can curate at the plan level and can also set "Current and future plan".</span></span>
- <span data-ttu-id="4dcda-233">プライベート Azure Marketplace、展開できるものとできないものについてエンド ユーザーに事前に通知できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-233">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="4dcda-234">プライベート オファーとプライベート オファーの違いAzure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-234">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="4dcda-235">プライベート **オファーを使用** すると、発行元は、対象となる顧客にのみ表示されるプランを作成できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-235">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="4dcda-236">これにより、ネゴシエートされた価格、プライベートの使用条件、特殊な構成を使用して、カスタマイズされたソリューションを非公開で共有できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-236">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="4dcda-237">詳細については、コマーシャル マーケットプレース [のプライベート オファーに関するページを参照してください](/azure/marketplace/private-offers)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-237">For details, see [Private offers in the commercial marketplace](/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="4dcda-238">**プライベート Azure Marketplace** のAzure portalユーザーが展開できるサードパーティソリューションを管理者が事前に承認できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-238">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="4dcda-239">プライベート サービスを使用Azure Marketplace、ユーザーは、準拠しているオファーを検索、購入、デプロイすることで、Azure Marketplaceの利点を利用できます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-239">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="4dcda-240">プライベート マーケットプレースでサブスクリプションベースのプライベート オファーを管理するには、Marketplace 管理者が特定のサブスクリプションに対して少なくとも "読み取り" ロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-240">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of "read" role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="4dcda-241">プライベート オファーをプライベート オファーに追加Azure Marketplace、[マーケットプレースの管理] タブに表示されない理由は何ですか?</span><span class="sxs-lookup"><span data-stu-id="4dcda-241">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="4dcda-242">サブスクリプションベースのプライベート オファーは、プライベート オファーの設定に一覧表示されているサブスクリプションに対してのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-242">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="4dcda-243">プライベート オファーを表示するには、グローバル サブスクリプション フィルターにすべてのサブスクリプションが表示されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-243">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="プライベート マーケットプレース フィルターを表示します。":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="4dcda-245">Private Azure Marketplace にカスタム イメージを含Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-245">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="4dcda-246">できませんね。</span><span class="sxs-lookup"><span data-stu-id="4dcda-246">No.</span></span> <span data-ttu-id="4dcda-247">プライベート Azure Marketplaceを使用すると、すべての IT 管理者は、グローバル なソリューションからサードパーティのソリューションを管理Azure Marketplace。</span><span class="sxs-lookup"><span data-stu-id="4dcda-247">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="4dcda-248">カスタム イメージはグローバル イメージ上にAzure Marketplace、IT 管理者はカスタム イメージを選択して選択することはできません。</span><span class="sxs-lookup"><span data-stu-id="4dcda-248">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="4dcda-249">カスタム イメージを共有する場合は、 を使用[Shared Image Gallery。](/azure/virtual-machines/shared-image-galleries)</span><span class="sxs-lookup"><span data-stu-id="4dcda-249">If you would like to share custom images, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="4dcda-250">ステップ バイ ステップ ガイド: アプリケーションの作成 (SIG)[](/azure/virtual-machines/shared-images-cli)(CLI、PowerShell) Shared Image Galleryを[作成します](/azure/virtual-machines/shared-images-powershell)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-250">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](/azure/virtual-machines/shared-images-cli), [PowerShell](/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="4dcda-251">SIG 内にイメージ定義を作成します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-251">Create an image definition within a SIG.</span></span> <span data-ttu-id="4dcda-252">お客様は、[OS **状態] フィールドに** [一般化] を選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4dcda-252">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="4dcda-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [、PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition))。</span><span class="sxs-lookup"><span data-stu-id="4dcda-253">([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="4dcda-254">マネージド イメージをアプリケーションに取りShared Image Gallery [(CLI、PowerShell)。](/azure/virtual-machines/image-version-managed-image-powershell)[](/azure/virtual-machines/image-version-managed-image-cli)</span><span class="sxs-lookup"><span data-stu-id="4dcda-254">Bring managed image into the Shared Image Gallery ([CLI](/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="4dcda-255">SIG VM イメージは 1 つのサブスクリプションに存在します。</span><span class="sxs-lookup"><span data-stu-id="4dcda-255">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="4dcda-256">他のサブスクリプションで使用するには、アプリの登録[(CLI、PowerShell](/azure/virtual-machines/linux/share-images-across-tenants)) [を使用します](/azure/virtual-machines/windows/share-images-across-tenants)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-256">To make it available to other subscriptions, use an app registration ([CLI](/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="4dcda-257">発行元が Microsoft **ではないにもかかわらず、** 一部のオファーが既定で承認されるのを確認する理由</span><span class="sxs-lookup"><span data-stu-id="4dcda-257">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="4dcda-258">Microsoft では、Azure で Linux とオープンソースのテクノロジをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="4dcda-258">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="4dcda-259">[Azure では、サポートされている Linux](/azure/virtual-machines/linux/endorsed-distros) ディストリビューションがサポートされ、価格は仮想マシンに統合されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-259">[Endorsed Linux distributions](/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="4dcda-260">Azure Linux エージェントは既に Azure Marketplaceにインストール済みなので、Microsoft オファーと同様に扱います。</span><span class="sxs-lookup"><span data-stu-id="4dcda-260">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="4dcda-261">Microsoft オファーは既定で承認されます。承認された Linux ディストリビューションはプライベート サービスで管理Azure Marketplace既定で承認されます。</span><span class="sxs-lookup"><span data-stu-id="4dcda-261">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="4dcda-262">サポートにお問い合せください</span><span class="sxs-lookup"><span data-stu-id="4dcda-262">Contact support</span></span>

- <span data-ttu-id="4dcda-263">サポートAzure Marketplaceについては [、Microsoft Q&A を参照してください](/answers/products/)。</span><span class="sxs-lookup"><span data-stu-id="4dcda-263">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>