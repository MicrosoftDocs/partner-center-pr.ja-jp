---
title: Azure portal でのプライベート Azure Marketplace の作成と管理
description: Azure portal でのプライベート Azure Marketplace (プレビュー) の作成と管理について説明します。
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: f62c9aef13b51ba2db42b267d7620f506bbdc1ec
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/21/2020
ms.locfileid: "95006941"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Azure portal でのプライベート Azure Marketplace (プレビュー) の作成と管理

プライベート Azure Marketplace (プレビュー) を使用すると、管理者は、ユーザーが使用できるサードパーティ製のソリューションを管理できます。 これを行うには、承認したオファーと、会社のポリシーに準拠しているオファーのみをデプロイできるようにします。 プライベート Azure Marketplace では、ユーザーはオンラインストアで準拠しているプランを検索し、購入してデプロイすることができます。 

Marketplace 管理者 (割り当てられたロール) として、無効になっている空のプライベートストアから開始します。このストアで、承認されたオファーとプランを追加できます。 この記事では、ユーザーに対してプライベート Azure Marketplace を作成、管理、有効にする方法について説明します。

メモ:

- プライベート Azure Marketplace はテナントレベルであるため、テナントのすべてのユーザーに同じ curated リストが表示されます。
- すべての Microsoft ソリューションは、プライベート Azure Marketplace に自動的に追加されます。

## <a name="assign-the-marketplace-admin-role"></a>Marketplace 管理者ロールを割り当てる

テナントのグローバル管理者は、プライベートストアを管理するプライベート Azure Marketplace 管理者に **Marketplace 管理** 者ロールを割り当てる必要があります。

>[!IMPORTANT]
> プライベート Azure Marketplace 管理へのアクセスは、Marketplace 管理者ロールが割り当てられている IT 管理者のみが使用できます。

### <a name="prerequisites"></a>前提条件

テナントスコープのユーザーに Marketplace 管理者ロールを割り当てる前に、次の前提条件を満たす必要があります。

- **グローバル管理者** ユーザーにアクセスできます。
- テナントには、少なくとも1つのサブスクリプションがあります (任意の種類を指定できます)。
- グローバル管理者のユーザーには、選択したサブスクリプションの **共同作成** 者ロールまたはそれ以降が割り当てられます。
- 全体管理者ユーザーのアクセス権が **[はい]** に設定されています (「 [すべての Azure サブスクリプションと管理グループを管理するためのアクセス権の昇格」を](/azure/role-based-access-control/elevate-access-global-admin)参照してください)。

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>PowerShell を使用して Marketplace 管理者ロールを割り当てる

Marketplace 管理者ロールを割り当てるには、次の PowerShell スクリプトを使用します。次のパラメーターが必要です。

- **TenantId:** スコープ内のテナントの ID (Marketplace 管理者ロールはテナントのスコープで割り当て可能)。
- **SubscriptionId:** 全体管理者に **共同作成者** ロールが割り当てられているサブスクリプション。
- **Globaladminusername:** グローバル管理者のユーザー名。
- **UsernameToAssignRoleFor:** Marketplace 管理者ロールが割り当てられるユーザーの名前。

> [!NOTE]
> テナントに招待されたゲストユーザーについては、Marketplace 管理者ロールを割り当てるためにアカウントが使用できるようになるまで、最大で48時間かかることがあります。 詳細については、「 [AZURE ACTIVE DIRECTORY B2B コラボレーションユーザーのプロパティ](/azure/active-directory/b2b/user-properties)」を参照してください。

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

Az. Portal PowerShell モジュールに含まれるコマンドレットの詳細については、「 [Microsoft Azure PowerShell: ポータルのダッシュボードのコマンドレット](/powershell/module/az.portal/)」を参照してください。

## <a name="create-private-azure-marketplace"></a>プライベート Azure Marketplace を作成する

1. [Azure portal](https://portal.azure.com/) にサインインします。
2. [ **すべてのサービス** ]、[ **Marketplace**] の順に選択します。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="メインウィンドウ Azure portal ます。":::

3. 左側のオプションから [ **プライベートマーケットプレース** ] を選択します。

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Azure portal メインウィンドウで [プライベートマーケットプレース] を選択します。":::

4. [ **はじめ** に] を選択してプライベート Azure Marketplace を作成します (これを行う必要があるのは1回だけです)。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Azure portal のメインウィンドウで [開始] を選択します。":::

    このテナントに対してプライベート Azure Marketplace が既に存在する場合は、[ **Marketplace の管理** ] が既定で選択されます。

5. 完了すると、プライベート Azure Marketplace が空で無効になります。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空のプライベート Azure Marketplace 画面。":::

## <a name="add-items-from-gallery"></a>ギャラリーからの項目の追加

項目は、オファーとプランの組み合わせです。 [Marketplace の管理] ページで項目を検索して追加することができます。

1. [ **項目の追加**] を選択します。

2. **ギャラリー** を参照するか、検索フィールドを使用して目的の項目を検索します。

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="ギャラリーを参照するか、検索フィールドを使用します。":::

3. 既定では、新しいオファーを追加すると、現在のすべてのプランが許可リストに追加されます。 選択した項目を追加する前に、プランの選択を変更するには、プランのタイルのドロップダウンメニューを選択し、必要なプランを更新します。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="必要なプランを更新します。":::

4. 選択を行った後、左下にある [ **完了** ] を選択します。

>[!Note]
> Marketplace への **項目の追加** は、Microsoft 以外のプランでのみ利用可能になります。 Microsoft プランは、既定で許可されています。

## <a name="edit-item-plans"></a>項目計画の編集

項目のプランは、[Marketplace の管理] ページで編集できます。

1. [ **プラン** ] 列で、そのアイテムのドロップダウンメニューから使用可能なプランを確認します。
2. チェックボックスをオンまたはオフにして、ユーザーが使用できるようにするプランを選択します。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="必須項目のチェックボックスをオンまたはオフにします。":::

> [!NOTE]
> 各プランでは、更新を実行するために少なくとも1つのプランが選択されている必要があります。 オファーに関連するすべてのプランを削除するには、プラン全体を削除します (次のセクションを参照)。

## <a name="delete-offers"></a>オファーの削除

[Marketplace の管理] ページで、プラン名 (上の画面を参照) の横にあるチェックボックスをオンにし、[ **アイテムの削除**] を選択します。

## <a name="enabledisable-private-azure-marketplace"></a>プライベート Azure Marketplace を有効/無効にする

[Marketplace の管理] ページに、次のいずれかのバナーが表示されます。これは、プライベート Azure Marketplace の現在の状態を示しています。

:::image type="content" source="media/private-azure/state-disable.png" alt-text="状態バナーを無効にする":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="状態バナーを有効にする":::

プライベート Azure Marketplace は、必要に応じて有効または無効にすることができます。

1. 無効になっている場合は、[ **プライベートマーケットプレースを有効** にする] をオンにします。
2. 有効にする場合は、[ **プライベートマーケットプレースを無効** にする] をオンにします。

## <a name="browsing-private-azure-marketplace"></a>プライベート Azure Marketplace を参照しています

プライベート Azure Marketplace が有効になっている場合は、Marketplace 管理者が許可したプランがユーザーに表示されます。

- 緑色の **許可** された通知は、許可されているパートナー (Microsoft 以外の) プランを示します。
- 青の **許可** された通知は、許可されている Microsoft プランを示します。

ユーザーは、許可されていないプランと許可されていないプランをフィルター処理できます。

:::image type="content" source="media/private-azure/filter-option.png" alt-text="フィルターオプション。":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>プライベート Azure Marketplace での購入またはデプロイ

製品の詳細ページのエクスペリエンスは、パブリック Azure Marketplace に似ていますが、Azure Marketplace 固有の3つのシナリオがあります。

- ユーザーが許可されたプランを選択すると、[ **作成** ] ボタンが有効になります。

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="プランを作成できることを示すバナーを提供します。":::

- ユーザーが許可されていないプランを選択すると、そのプランは許可されておらず、[ **作成** ] ボタンが無効になっていることを示すバナーが示されます。

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="プランを作成できないことを示すバナーを提供します。":::

- 製品計画の選択が [製品の詳細] ページに表示されないが、管理者が1つ以上のプランを承認した場合、次のようなプランが許可され、[ **作成** ] ボタンが有効になります。

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="プランを作成し、使用可能なプランを表示できることを示すバナーを提供します。":::

## <a name="contact-support"></a>サポートにお問い合せください

Azure Marketplace のサポートについては、 [Microsoft Q&A](/answers/products/)にアクセスしてください。 
