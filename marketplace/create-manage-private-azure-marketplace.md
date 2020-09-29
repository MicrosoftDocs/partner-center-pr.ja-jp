---
title: Azure portal でのプライベート Azure Marketplace の作成と管理
description: Azure portal でのプライベート Azure Marketplace (プレビュー) の作成と管理について説明します。
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: c0a395a7c5bfe926cdc56d7386aaaebb0305fb68
ms.sourcegitcommit: d31c06022624ca2d1db12b3c60ef1d0a3861f763
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/19/2020
ms.locfileid: "91429356"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="68342-103">Azure portal でのプライベート Azure Marketplace (プレビュー) の作成と管理</span><span class="sxs-lookup"><span data-stu-id="68342-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="68342-104">プライベート Azure Marketplace (プレビュー) を使用すると、管理者は、ユーザーが使用できるサードパーティ製のソリューションを管理できます。</span><span class="sxs-lookup"><span data-stu-id="68342-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="68342-105">これを行うには、承認したオファーと、会社のポリシーに準拠しているオファーのみをデプロイできるようにします。</span><span class="sxs-lookup"><span data-stu-id="68342-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="68342-106">プライベート Azure Marketplace では、ユーザーはオンラインストアで準拠しているプランを検索し、購入してデプロイすることができます。</span><span class="sxs-lookup"><span data-stu-id="68342-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="68342-107">Marketplace 管理者 (割り当てられたロール) として、無効になっている空のプライベートストアから開始します。このストアで、承認されたオファーとプランを追加できます。</span><span class="sxs-lookup"><span data-stu-id="68342-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="68342-108">この記事では、ユーザーに対してプライベート Azure Marketplace を作成、管理、有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="68342-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="68342-109">メモ:</span><span class="sxs-lookup"><span data-stu-id="68342-109">Notes:</span></span>

- <span data-ttu-id="68342-110">プライベート Azure Marketplace はテナントレベルであるため、テナントのすべてのユーザーに同じ curated リストが表示されます。</span><span class="sxs-lookup"><span data-stu-id="68342-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="68342-111">すべての Microsoft ソリューションは、プライベート Azure Marketplace に自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="68342-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="68342-112">Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="68342-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="68342-113">テナントのグローバル管理者は、プライベートストアを管理するプライベート Azure Marketplace 管理者に **Marketplace 管理** 者ロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="68342-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="68342-114">プライベート Azure Marketplace 管理へのアクセスは、Marketplace 管理者ロールが割り当てられている IT 管理者のみが使用できます。</span><span class="sxs-lookup"><span data-stu-id="68342-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="68342-115">[前提条件]</span><span class="sxs-lookup"><span data-stu-id="68342-115">Prerequisites</span></span>

<span data-ttu-id="68342-116">テナントスコープのユーザーに Marketplace 管理者ロールを割り当てる前に、次の前提条件を満たす必要があります。</span><span class="sxs-lookup"><span data-stu-id="68342-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="68342-117">**グローバル管理者**ユーザーにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="68342-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="68342-118">テナントには、少なくとも1つのサブスクリプションがあります (任意の種類を指定できます)。</span><span class="sxs-lookup"><span data-stu-id="68342-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="68342-119">グローバル管理者のユーザーには、手順 2. で選択したサブスクリプションの **共同作成** 者ロールが割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="68342-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="68342-120">全体管理者ユーザーのアクセスが **[はい]** に設定されています (「 [昇格-アクセス-グローバル-管理者](/azure/role-based-access-control/elevate-access-global-admin)」を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="68342-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="68342-121">PowerShell を使用して Marketplace 管理者ロールを割り当てる</span><span class="sxs-lookup"><span data-stu-id="68342-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="68342-122">Marketplace 管理者ロールを割り当てるには、次の PowerShell スクリプトを使用します。次のパラメーターが必要です。</span><span class="sxs-lookup"><span data-stu-id="68342-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="68342-123">**TenantId:** スコープ内のテナントの ID (Marketplace 管理者ロールはテナントのスコープで割り当て可能)。</span><span class="sxs-lookup"><span data-stu-id="68342-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="68342-124">**SubscriptionId:** 全体管理者に **共同作成者** ロールが割り当てられているサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="68342-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="68342-125">**Globaladminusername:** グローバル管理者のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="68342-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="68342-126">**UsernameToAssignRoleFor:** Marketplace 管理者ロールが割り当てられるユーザーの名前。</span><span class="sxs-lookup"><span data-stu-id="68342-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="68342-127">テナントに招待されたゲストユーザーについては、Marketplace 管理者ロールを割り当てるためにアカウントが使用できるようになるまで、最大で48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="68342-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="68342-128">詳細については、「 [AZURE ACTIVE DIRECTORY B2B コラボレーションユーザーのプロパティ](/azure/active-directory/b2b/user-properties)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68342-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."

$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

<span data-ttu-id="68342-129">Az. Portal PowerShell モジュールに含まれるコマンドレットの詳細については、「 [Microsoft Azure PowerShell: ポータルのダッシュボードのコマンドレット](/powershell/module/az.portal/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68342-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="68342-130">プライベート Azure Marketplace を作成する</span><span class="sxs-lookup"><span data-stu-id="68342-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="68342-131">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="68342-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="68342-132">[ **すべてのサービス** ]、[ **Marketplace**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="メインウィンドウ Azure portal ます。":::

3. <span data-ttu-id="68342-134">左側のオプションから [ **プライベートマーケットプレース** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="メインウィンドウ Azure portal ます。":::

4. <span data-ttu-id="68342-136">[ **はじめ** に] を選択してプライベート Azure Marketplace を作成します (これを行う必要があるのは1回だけです)。</span><span class="sxs-lookup"><span data-stu-id="68342-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="メインウィンドウ Azure portal ます。":::

    <span data-ttu-id="68342-138">このテナントに対してプライベート Azure Marketplace が既に存在する場合は、[ **Marketplace の管理** ] が既定で選択されます。</span><span class="sxs-lookup"><span data-stu-id="68342-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="68342-139">完了すると、プライベート Azure Marketplace が空で無効になります。</span><span class="sxs-lookup"><span data-stu-id="68342-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="メインウィンドウ Azure portal ます。":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="68342-141">ギャラリーからの項目の追加</span><span class="sxs-lookup"><span data-stu-id="68342-141">Add items from gallery</span></span>

<span data-ttu-id="68342-142">項目は、オファーとプランの組み合わせです。</span><span class="sxs-lookup"><span data-stu-id="68342-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="68342-143">[Marketplace の管理] ページで項目を検索して追加することができます。</span><span class="sxs-lookup"><span data-stu-id="68342-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="68342-144">[ **項目の追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-144">Select **Add items**.</span></span>

2. <span data-ttu-id="68342-145">**ギャラリー**を参照するか、検索フィールドを使用して目的の項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="68342-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="メインウィンドウ Azure portal ます。":::

3. <span data-ttu-id="68342-147">既定では、新しいオファーを追加すると、現在のすべてのプランが許可リストに追加されます。</span><span class="sxs-lookup"><span data-stu-id="68342-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="68342-148">選択した項目を追加する前に、プランの選択を変更するには、プランのタイルのドロップダウンメニューを選択し、必要なプランを更新します。</span><span class="sxs-lookup"><span data-stu-id="68342-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="メインウィンドウ Azure portal ます。":::

4. <span data-ttu-id="68342-150">選択を行った後、左下にある [ **完了** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="68342-151">Marketplace への**項目の追加**は、Microsoft 以外のプランでのみ利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="68342-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="68342-152">Microsoft プランは、既定で許可されています。</span><span class="sxs-lookup"><span data-stu-id="68342-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="68342-153">項目計画の編集</span><span class="sxs-lookup"><span data-stu-id="68342-153">Edit item plans</span></span>

<span data-ttu-id="68342-154">項目のプランは、[Marketplace の管理] ページで編集できます。</span><span class="sxs-lookup"><span data-stu-id="68342-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="68342-155">[ **プラン** ] 列で、そのアイテムのドロップダウンメニューから使用可能なプランを確認します。</span><span class="sxs-lookup"><span data-stu-id="68342-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="68342-156">チェックボックスをオンまたはオフにして、ユーザーが使用できるようにするプランを選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="メインウィンドウ Azure portal ます。":::

> [!NOTE]
> <span data-ttu-id="68342-158">各プランでは、更新を実行するために少なくとも1つのプランが選択されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="68342-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="68342-159">オファーに関連するすべてのプランを削除するには、プラン全体を削除します (次のセクションを参照)。</span><span class="sxs-lookup"><span data-stu-id="68342-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="68342-160">オファーの削除</span><span class="sxs-lookup"><span data-stu-id="68342-160">Delete offers</span></span>

<span data-ttu-id="68342-161">[Marketplace の管理] ページで、プラン名 (上の画面を参照) の横にあるチェックボックスをオンにし、[ **アイテムの削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="68342-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="68342-162">プライベート Azure Marketplace を有効/無効にする</span><span class="sxs-lookup"><span data-stu-id="68342-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="68342-163">[Marketplace の管理] ページに、次のいずれかのバナーが表示されます。これは、プライベート Azure Marketplace の現在の状態を示しています。</span><span class="sxs-lookup"><span data-stu-id="68342-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="メインウィンドウ Azure portal ます。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="メインウィンドウ Azure portal ます。":::

<span data-ttu-id="68342-166">プライベート Azure Marketplace は、必要に応じて有効または無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="68342-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="68342-167">無効になっている場合は、[ **プライベートマーケットプレースを有効** にする] をオンにします。</span><span class="sxs-lookup"><span data-stu-id="68342-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="68342-168">有効にする場合は、[ **プライベートマーケットプレースを無効** にする] をオンにします。</span><span class="sxs-lookup"><span data-stu-id="68342-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="68342-169">プライベート Azure Marketplace を参照しています</span><span class="sxs-lookup"><span data-stu-id="68342-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="68342-170">プライベート Azure Marketplace が有効になっている場合は、Marketplace 管理者が許可したプランがユーザーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="68342-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="68342-171">緑色の **許可** された通知は、許可されているパートナー (Microsoft 以外の) プランを示します。</span><span class="sxs-lookup"><span data-stu-id="68342-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="68342-172">青の **許可** された通知は、許可されている Microsoft プランを示します。</span><span class="sxs-lookup"><span data-stu-id="68342-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="68342-173">ユーザーは、許可されていないプランと許可されていないプランをフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="68342-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="メインウィンドウ Azure portal ます。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="68342-175">プライベート Azure Marketplace での購入またはデプロイ</span><span class="sxs-lookup"><span data-stu-id="68342-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="68342-176">製品の詳細ページのエクスペリエンスは、パブリック Azure Marketplace に似ていますが、Azure Marketplace 固有の3つのシナリオがあります。</span><span class="sxs-lookup"><span data-stu-id="68342-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="68342-177">ユーザーが許可されたプランを選択すると、[ **作成** ] ボタンが有効になります。</span><span class="sxs-lookup"><span data-stu-id="68342-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="メインウィンドウ Azure portal ます。":::

- <span data-ttu-id="68342-179">ユーザーが許可されていないプランを選択すると、そのプランは許可されておらず、[ **作成** ] ボタンが無効になっていることを示すバナーが示されます。</span><span class="sxs-lookup"><span data-stu-id="68342-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="メインウィンドウ Azure portal ます。":::

- <span data-ttu-id="68342-181">製品計画の選択が [製品の詳細] ページに表示されないが、管理者が1つ以上のプランを承認した場合、次のようなプランが許可され、[ **作成** ] ボタンが有効になります。</span><span class="sxs-lookup"><span data-stu-id="68342-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="メインウィンドウ Azure portal ます。":::

## <a name="contact-support"></a><span data-ttu-id="68342-183">サポートにお問い合せください</span><span class="sxs-lookup"><span data-stu-id="68342-183">Contact support</span></span>

<span data-ttu-id="68342-184">Azure Marketplace のサポートについては、 [Microsoft Q&A](/answers/products/)にアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="68342-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
