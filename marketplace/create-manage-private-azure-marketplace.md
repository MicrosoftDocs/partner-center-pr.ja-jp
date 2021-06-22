---
title: 次の方法でプライベート Azure Marketplaceを作成および管理Azure portal
description: このページでは、プライベート Azure Marketplace (プレビュー) の作成と管理についてAzure portal。 プライベート Azure Marketplace (プレビュー) を使用すると、管理者は、ユーザーが使用できるサードパーティのソリューションを管理できます。
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 9da9eb4944508e815d1664fb44b13bce52f37150
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431665"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>次の方法でプライベート Azure Marketplaceを作成および管理Azure portal

プライベート Azure Marketplaceを使用すると、ユーザーが使用できるサードパーティのソリューションを管理者が管理できます。 これを行うのは、管理者によって承認され、企業のポリシーに準拠しているオファーのみをユーザーが展開できるようにすることで行います。 Private Azure Marketplaceを使用すると、ユーザーはオンライン ストアで準拠しているオファーを検索して購入およびデプロイできます。

Marketplace 管理者 (割り当てられたロール) は、無効で空のプライベート ストアから始め、承認されたオファーとプランを追加できます。 この記事では、必要なロールの割り当て、プライベート ストアの作成、アイテムの管理、ユーザー要求の承認、ユーザーに対するプライベート Azure Marketplaceの有効化を行う方法について説明します。

> [!NOTE]
> - プライベート Azure Marketplaceはテナント レベルなので、テナントのすべてのユーザーに同じキュキュされた一覧が表示されます。
> - すべての Microsoft ソリューション ( [サポートされている Linux ディストリビューション](/azure/virtual-machines/linux/endorsed-distros)を含む) は、Private Azure Marketplace に追加されます。

## <a name="assign-the-marketplace-admin-role"></a>Marketplace 管理者ロールを割り当てる

テナントグローバル管理者は、プライベート ストアを管理するプライベート 管理者に **Marketplace** Azure Marketplaceロールを割り当てる必要があります。

>[!IMPORTANT]
> プライベート アカウント管理Azure Marketplace、Marketplace 管理者ロールが割り当てられている IT 管理者だけが使用できます。

### <a name="prerequisites"></a>前提条件

テナント スコープのユーザーに Marketplace 管理者ロールを割り当てる前に、次の前提条件が必要です。

- グローバル管理者ユーザーに **アクセス** できます。
- テナントには、少なくとも 1 つのサブスクリプションがあります (任意の種類を指定できます)。
- グローバル管理者ユーザーには、選択したサブスクリプションの **共同** 作成者ロール以上が割り当てられます。

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>アクセス制御 (IAM) を使用して Marketplace 管理者ロールを割り当てる

1. [Azure portal](https://portal.azure.com/) にサインインします。
1. [すべての **サービス] を選択し****、[Marketplace] を選択します**。
1. 左側 **のメニューから** [プライベート マーケットプレース] を選択します。

    [![Marketplace の左側にプライベート マーケットプレース メニュー オプションが表示されます。](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. [ **アクセス制御 (IAM)] を選択して** Marketplace 管理者ロールを割り当てる。

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="[I A M アクセス制御] 画面が表示されます。":::

1. **[+ 追加]**  >  **[ロール割り当ての追加]** の順に選択します。
1. [ロール **] で****、[Marketplace 管理者] を選択します**。

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="[ロールの割り当て] メニューが表示されます。":::

1. ドロップダウン リストから目的のユーザーを選択し、[完了] を **選択します**。

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>PowerShell を使用して Marketplace 管理者ロールを割り当てる

Marketplace 管理者ロールを割り当てるには、次の PowerShell スクリプトを使用します。次のパラメーターが必要です。

- **TenantId:** スコープ内のテナントの ID (Marketplace 管理者ロールはテナント スコープで割り当て可能)。
- **SubscriptionId:** グローバル管理者に共同作成者ロール **以上が割** り当てられているサブスクリプション。
- **GlobalAdminUsername:** グローバル管理者のユーザー名。
- **UsernameToAssignRoleFor:** Marketplace 管理者ロールを割り当てるユーザー名。

> [!NOTE]
> テナントに招待されたゲスト ユーザーの場合、自分のアカウントが Marketplace 管理者ロールを割り当て可能になるまで、最大 48 時間かかる場合があります。 詳細については [、「B2B コラボレーション ユーザーのAzure Active Directory」を参照してください](/azure/active-directory/b2b/user-properties)。

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

Az.Portal PowerShell モジュールに含まれているコマンドレットの詳細については、「ポータル ダッシュボードコマンドレット」Microsoft Azure PowerShell [を参照してください](/powershell/module/az.portal/)。

## <a name="create-private-azure-marketplace"></a>プライベート アカウントを作成Azure Marketplace

1. [Azure portal](https://portal.azure.com/) にサインインします。
2. [すべての **サービス] を選択し****、[Marketplace] を選択します**。

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="メイン ウィンドウAzure portalを表示します。":::

3. 左側 **のメニューから** [プライベート マーケットプレース] を選択します。

4. **[開始する]** を選択してプライベート Azure Marketplace作成します (これを行う必要があるのは 1 回だけです)。

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="メイン ウィンドウで [開始する] をAzure portal方法を示します。":::

    このテナントAzure Marketplaceプライベート アカウントが既に存在する場合は、既定で **[Marketplace** の管理] が選択されます。

5. 完了すると、空の無効なプライベート アカウントがAzure Marketplace。

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="空の [プライベート] Azure Marketplace表示します。":::

## <a name="add-items-from-gallery"></a>ギャラリーから項目を追加する

項目は、オファーとプランの組み合わせです。 [Marketplace の管理] ページで項目を検索して追加できます。

1. [項目 **の追加] を選択します**。

2. ギャラリーを **参照するか** 、検索フィールドを使用して目的の項目を検索します。

    [![ギャラリーを参照する方法、または検索フィールドを使用する方法を示します。](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. 既定では、新しいオファーを追加すると、現在のすべてのプランが承認済みリストに追加されます。 選択した項目を追加する前にプランの選択を変更するには、オファーのタイルのドロップダウン メニューを選択し、必要なプランを更新します。

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="必要なプランを更新する方法を示します。":::

4. 選択 **が** 完了したら、左下にある [完了] を選択します。

>[!Note]
> **Marketplace への項目** の追加は、Microsoft 以外のオファーでのみ使用できます。 Microsoft ソリューション ( [承認された Linux](/azure/virtual-machines/linux/endorsed-distros)ディストリビューションを含む) は、"既定で承認済み" としてタグ付けされ、プライベート マーケットプレースでは管理できません。

## <a name="edit-items-plans"></a>項目のプランを編集する

項目のプランは、[Marketplace の管理] ページで編集できます。

1. [プラン **] 列** で、その項目のドロップダウン メニューから使用可能なプランを確認します。
2. チェック ボックスをオンまたはオフにして、ユーザーが利用できるプランを選択します。

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="必要な項目のチェック ボックスをオンまたはオフにする方法を示します。":::

> [!NOTE]
> 各オファーには、更新を実行するために少なくとも 1 つのプランが選択されている必要があります。 オファーに関連するプランを削除するには、オファー全体を削除します (次のセクションを参照)。

## <a name="delete-offers"></a>オファーの削除

[Marketplace の管理] ページで、オファー名の横にあるチェック ボックス (上の画面を参照) を選択し、[ 項目の削除] **を選択します**。

## <a name="enabledisable-private-azure-marketplace"></a>プライベート アカウントを有効または無効Azure Marketplace

[Marketplace の管理] ページに、プライベート アカウントの現在の状態を示す次のいずれかのバナーがAzure Marketplace。

:::image type="content" source="media/private-azure/state-disable.png" alt-text="[状態を無効にする] バナーを表示します。":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="[状態を有効にする] バナーを表示します。":::

必要に応じて、プライベート Azure Marketplace有効または無効にできます。

- 無効になっている場合は、[プライベート **マーケットプレースを有効にする] を** 選択して有効にします。
- 有効になっている場合は、 [プライベート マーケット **プレースを無効にする] を選択して** 無効にします。

## <a name="private-azure-marketplace-notification-center"></a>プライベート Azure Marketplace通知センター

Notification Center は 3 種類の通知で構成され、Marketplace 管理者は通知に基づいてアクションを実行できます。

- 承認された一覧に含されていない項目に対するユーザーからの承認要求 (以下の「オファーまたはプランの追加要求 [」を参照](#request-to-add-offers-or-plans) )。
- 承認済みリストに 1 つ以上のプランが既に含むオファーの新しいプラン通知。
- 承認済みリストに含まれていますが、グローバル リストから削除された項目のプラン通知を削除Azure Marketplace。

通知センターにアクセスするには:

1. 左側 **のメニュー** から [通知] を選択します。

    [![[通知] メニューが表示されます。](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. その他のアクションについては、省略記号メニューを選択します。

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="[その他のオプション] メニューの結果が表示されます。":::

1. プラン要求の場合、[ **要求の** 表示] で承認要求フォームが開き、特定のオファーのすべてのユーザー要求を確認できます。
1. [承認 **] または [拒否** ] **を選択します**。

    [![承認オプションと拒否オプションを表示します。](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. ドロップダウン メニューから、承認するプランを選択します。
1. コメントを追加し、 [送信] を **選択します**。

## <a name="browsing-private-azure-marketplace"></a>プライベート Azure Marketplace の参照

[プライベート Azure Marketplace有効にすると、Marketplace 管理者が承認したプランがユーザーに表示されます。

- 緑色の **承認済み通知** は、承認されたパートナー (Microsoft 以外) オファーを示します。
- 青色の **承認済み** 通知は、承認された Microsoft オファー (承認された [Linux](/azure/virtual-machines/linux/endorsed-distros)ディストリビューションを含む) を示します。

ユーザーは、承認されていないオファーと承認されていないオファーをフィルター処理できます。

[![フィルターオプションを表示します。](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>プライベート サービスで購入またはデプロイAzure Marketplace

製品の詳細ページのエクスペリエンスはグローバル サービスと似ていますがAzure Marketplace、3 つのプライベート Azure Marketplaceシナリオがあります。

- ユーザーが承認済みのプランを選択すると、[ **作成** ] ボタンが有効になります。

    [![プランを作成できることを示すオファーバナーを表示します。](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- 製品計画の選択が [製品の詳細] ページに表示されず、管理者が1つまたは複数のプランを承認した場合は、承認されているプランと [ **作成** ] ボタンが有効になっているバナーが表示されます。

    [![プランを作成し、使用可能なプランを表示できることを示すオファーバナーを表示します。](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- ユーザーが承認されていないプランを選択すると、バナーはプランを未承認としてメモし、[ **作成** ] ボタンは無効になります。 ユーザーは、承認されたリストにプランを追加するように要求できます (次のセクションを参照)。

## <a name="request-to-add-offers-or-plans"></a>オファーまたはプランの追加要求

プライベート Azure Marketplace で現在承認されていないパブリックプランまたはプランを追加するように要求できます。

1. バナーに **追加する要求** を選択して、 **アクセス要求フォーム** を開きます。

    [![[追加の要求] リンクを含むバナーを表示します。](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![オファーまたはプランのアクセス要求フォームを表示します。](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. 要求に追加するプランを選択します (**プラン** によっては、プランのプランを設定していないことが Marketplace 管理者に通知されます)。

1. **理由** を追加し、要求を送信するための **要求** を選択します。
  
    [![サンプルエントリを持つオファーまたはプランのアクセス要求フォームを表示します。](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. 要求を **取り消す** オプションを使用して、保留中の要求を示す通知がアクセス要求フォームに表示されます。

    [![撤回要求リンクを含む承認済みまたは保留中のプランの一覧を表示します。](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> 送信されると、Marketplace 管理者が要求をレビューしてアクションを実行するために、承認要求フォームが [通知センター](#private-azure-marketplace-notification-center) に送信されます。

> [!CAUTION]
> プライベートマーケットプレースへの承認は、ソリューションの調達を示すものではありません。

## <a name="frequently-asked-questions-faqs"></a>よく寄せられる質問 (FAQ)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Azure Policy を通じて、Marketplace のサードパーティ製アプリケーションを既にブロックしています。 これはどのような違いがあるのでしょうか。

現在、Marketplace でサードパーティのサービスを制限する方法は2つあります。

1. EA ポータルまたは Azure portal を通じて、サードパーティのサービスを無効にするか、"Free または BYOL Sku のみ" に制限します。

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Azure portal でサービスを制限する方法について説明します。":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="電子メールポータルでサービスを制限する方法について説明します。":::

2. 特定の Vm のみを許可する Azure ポリシーを作成します。 Windows Vm にポリシーを適用する方法の詳細については、「Azure Resource Manager を使用して [Windows vm にポリシーを適用](/azure/virtual-machines/windows/policy)する」を参照してください。

プライベート Azure Marketplace を使用すると、特定のオファーとプランをより柔軟に制限し、許可することができます。 エンドユーザーがサードパーティのサービスをデプロイする前であっても、marketplace ギャラリーにデプロイできるかどうかをエンドユーザーに通知します。 サードパーティのサービスのデプロイを許可するには、EA ポータルと Azure portal で Azure Marketplace をオン/有効に設定します。

- プライベート Azure Marketplace では、仮想マシンに限定されないパートナーソリューションを使用できます。
- プライベート Azure Marketplace はプランレベルで調整でき、"現在および将来の計画" を設定することもできます。
- プライベート Azure Marketplace では、エンドユーザーに対して、展開可能なものと配置できないものを事前に通知できます。

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>プライベートプランとプライベート Azure Marketplace の違いは何ですか?

**プライベートオファー** を使用すると、発行元は、対象ユーザーにのみ表示されるプランを作成できます。 これにより、カスタマイズされたソリューションを、ネゴシエートされた価格、プライベートの使用条件、および特殊な構成でプライベートに共有できます。 詳細については、「 [商業市場におけるプライベートプラン](/azure/marketplace/private-offers)」を参照してください。

Azure portal の **プライベート Azure Marketplace** を使用すると、管理者は、ユーザーが展開できるサードパーティ製ソリューションを事前に承認できます。 プライベート Azure Marketplace を使用すると、ユーザーは準拠しているプランを検索、購入、デプロイすることで、Azure Marketplace のメリットを享受できます。 プライベートマーケットプレースでサブスクリプションベースのプライベートプランを管理するには、Marketplace 管理者が特定のサブスクリプションに対して最低でも "読み取り" ロールを持っている必要があります。

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>プライベートな Azure Marketplace にプライベートプランを追加しましたが、[Marketplace の管理] タブに表示されないのはなぜですか?

サブスクリプションベースのプライベートプランは、一覧表示されたサブスクリプションのプライベートプランの設定でのみ表示されます。 プライベートプランを表示するには、グローバルサブスクリプションフィルターにすべてのサブスクリプションが表示されていることを確認します。

[![プライベートマーケットプレースフィルターを表示します。](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>カスタムイメージをプライベート Azure Marketplace に含めることはできますか?

いいえ。 プライベート Azure Marketplace を使用すると、すべての IT 管理者は、グローバルな Azure Marketplace からサードパーティ製のソリューションを管理および制御することができます。 カスタムイメージはグローバル Azure Marketplace にはないため、IT 管理者はカスタムイメージを選択して選択することはできません。 カスタムイメージを共有する場合は、 [共有イメージギャラリー](/azure/virtual-machines/shared-image-galleries)を使用します。

1. ステップバイステップガイド: 共有イメージギャラリー (SIG) を作成する ([CLI](/azure/virtual-machines/shared-images-cli)、 [PowerShell](/azure/virtual-machines/shared-images-powershell))。
2. SIG 内にイメージ定義を作成します。 お客様は、[OS 状態] フィールドで [ **一般化** ] を選択する必要があります。 ([CLI](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition)、 [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition))。
3. 管理対象イメージを共有イメージギャラリー ([CLI](/azure/virtual-machines/image-version-managed-image-cli)、 [PowerShell](/azure/virtual-machines/image-version-managed-image-powershell)) に取り込みます。
4. SIG VM イメージは1つのサブスクリプションに存在します。 他のサブスクリプションで使用できるようにするには、アプリの登録 ([CLI](/azure/virtual-machines/linux/share-images-across-tenants)、 [PowerShell](/azure/virtual-machines/windows/share-images-across-tenants)) を使用します。

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>発行元が Microsoft ではないにもかかわらず、一部のプランが **既定で承認** されるのはなぜですか。

Microsoft は、Azure での Linux およびオープンソーステクノロジをサポートしています。 Azure では、保証された[Linux ディストリビューション](/azure/virtual-machines/linux/endorsed-distros)がサポートされており、仮想マシンにも価格が統合されています。 Azure Linux エージェントは Azure Marketplace に既にプレインストールされているため、Microsoft のプランと同じように扱われます。 Microsoft のプランは既定で承認されるため、保証された Linux ディストリビューションは、プライベート Azure Marketplace では管理できず、既定で承認されます。

## <a name="contact-support"></a>サポートにお問い合せください

- Azure Marketplace のサポートについては、 [Microsoft Q&A](/answers/products/)にアクセスしてください。