---
title: 'クイックスタート: PowerShell を使用してプライベート Azure Marketplace を管理する'
description: このクイックスタートでは、Azure PowerShell を使用して、プライベート Azure Marketplace でプランを管理する方法を示します。
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: c5b8b9fcc247818315887109e2163c0722bfbd97
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/02/2020
ms.locfileid: "96536081"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="66f30-103">クイックスタート: PowerShell を使用してプライベート Azure Marketplace を管理する</span><span class="sxs-lookup"><span data-stu-id="66f30-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="66f30-104">この記事では、 [Az. marketplace](/powershell/module/az.marketplace) PowerShell モジュールを使用して、プライベート Azure marketplace でプランを管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="66f30-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="66f30-105">プライベート Azure Marketplace は現在、パブリックプレビュー段階にあります。</span><span class="sxs-lookup"><span data-stu-id="66f30-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="66f30-106">このプレビュー バージョンは、サービス レベル アグリーメントなしに提供されます。</span><span class="sxs-lookup"><span data-stu-id="66f30-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="66f30-107">運用環境のワークロードにはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="66f30-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="66f30-108">一部の機能はサポート対象ではなく、機能が制限されることがあります。</span><span class="sxs-lookup"><span data-stu-id="66f30-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="66f30-109">詳しくは、[Microsoft Azure プレビューの追加使用条件](https://azure.microsoft.com/support/legal/preview-supplemental-terms/)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="66f30-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="66f30-110">必要条件</span><span class="sxs-lookup"><span data-stu-id="66f30-110">Requirements</span></span>

* <span data-ttu-id="66f30-111">Azure サブスクリプションをお持ちでない場合は、開始する前に[無料](https://azure.microsoft.com/free/)アカウントを作成してください。</span><span class="sxs-lookup"><span data-stu-id="66f30-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="66f30-112">Azure PowerShell をローカルで使用する場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="66f30-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="66f30-113">[Az PowerShell モジュールをインストールします](/powershell/azure/install-az-ps)。</span><span class="sxs-lookup"><span data-stu-id="66f30-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="66f30-114">[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用して、Azure アカウントに接続します。</span><span class="sxs-lookup"><span data-stu-id="66f30-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="66f30-115">Azure Cloud Shell を使用する場合は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="66f30-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="66f30-116">詳細については、[Azure Cloud Shell の概要](https://docs.microsoft.com/azure/cloud-shell/overview)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="66f30-116">See [Overview of Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="66f30-117">**Az. Marketplace** PowerShell モジュールはプレビュー段階にありますが、コマンドレットを使用して個別にインストールする必要があり `Install-Module` ます。</span><span class="sxs-lookup"><span data-stu-id="66f30-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="66f30-118">この PowerShell モジュールは、一般提供されると、将来の Az PowerShell モジュール リリースに含まれ、既定で Azure Cloud Shell 内から使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="66f30-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="66f30-119">複数の Azure サブスクリプションをお持ちの場合は、リソースが課金の対象となる適切なサブスクリプションを選択してください。</span><span class="sxs-lookup"><span data-stu-id="66f30-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="66f30-120">[Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを使用して、特定のサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="66f30-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="66f30-121">プライベートストアの一覧表示</span><span class="sxs-lookup"><span data-stu-id="66f30-121">List private stores</span></span>

<span data-ttu-id="66f30-122">プライベートストアの一覧を取得するには、 [AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="66f30-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="66f30-123">次の例では、テナントのスコープの下に作成されたプライベートストアを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="66f30-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="66f30-124">プライベートマーケットプレースにプランを追加する</span><span class="sxs-lookup"><span data-stu-id="66f30-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="66f30-125">プランをプライベートストアに追加するには、 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="66f30-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="66f30-126">次の例では、テナントのスコープの下に作成されたプライベートストアのプライベートマーケットプレースに、指定されたオファーを追加します。</span><span class="sxs-lookup"><span data-stu-id="66f30-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="66f30-127">プライベートストアのプランを取得する</span><span class="sxs-lookup"><span data-stu-id="66f30-127">Get private store offers</span></span>

<span data-ttu-id="66f30-128">1つ以上のプライベートストアプランを取得するには、 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="66f30-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="66f30-129">次の例では、テナントのスコープの下に追加された、指定されたプライベートストアに関連付けられているオファーを取得します。</span><span class="sxs-lookup"><span data-stu-id="66f30-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="66f30-130">プランの削除</span><span class="sxs-lookup"><span data-stu-id="66f30-130">Remove an offer</span></span>

<span data-ttu-id="66f30-131">プライベートストアからプランを削除するには、 [AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="66f30-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="66f30-132">次の例では、テナントのスコープで作成されたプライベートストアからプランを削除します。</span><span class="sxs-lookup"><span data-stu-id="66f30-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="66f30-133">次のステップ</span><span class="sxs-lookup"><span data-stu-id="66f30-133">Next steps</span></span>

<span data-ttu-id="66f30-134">[プライベート Azure Marketplace を作成および管理](create-manage-private-azure-marketplace.md)します。</span><span class="sxs-lookup"><span data-stu-id="66f30-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>
