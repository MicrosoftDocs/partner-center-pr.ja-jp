---
title: Azure Marketplace でのプライベートプラン
description: Azure Marketplace でのプライベートプランについて説明します。
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 72e886a7cfad067b40674f30a9a21810d832994a
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412660"
---
# <a name="private-offers-in-azure-marketplace"></a><span data-ttu-id="49dcd-103">Azure Marketplace でのプライベートプラン</span><span class="sxs-lookup"><span data-stu-id="49dcd-103">Private offers in Azure Marketplace</span></span>

<span data-ttu-id="49dcd-104">プライベートプランは、パブリッシャーが特定の顧客にカスタムプランを提供する方法です。</span><span class="sxs-lookup"><span data-stu-id="49dcd-104">Private offers are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="49dcd-105">このオプションは現在、Azure portal の Azure Marketplace エクスペリエンスでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="49dcd-105">This option is currently supported only in the Azure Marketplace experience in the Azure portal.</span></span> <span data-ttu-id="49dcd-106">プライベートプランは、Azure portal から購入して直接インストールできる有料プランでのみ利用できます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-106">Private offers are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="49dcd-107">発行元は、ポータルからインストールできるかどうかに関係なく、コンサルティングサービス、アクション呼び出しとしての **連絡** を持つサービス、または無料サービスに対してプライベートプランを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="49dcd-107">Publisher cannot create private offers for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-offers-in-the-azure-portal"></a><span data-ttu-id="49dcd-108">Azure portal でのプライベートプランの検索</span><span class="sxs-lookup"><span data-stu-id="49dcd-108">Find private offers in the Azure portal</span></span>

<span data-ttu-id="49dcd-109">パートナーは、プライベートオファーを発行するときに、Azure portal の **Marketplace** セクションの対象ユーザーのみに表示されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-109">When a partner publishes a private offer, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="49dcd-110">これらのユーザーは、オファーの種類に応じて、サブスクリプション ID またはテナント ID によって定義されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-110">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="49dcd-111">プライベートプランの資格がある場合、ポータルでそれらを検索する方法は2つあります。</span><span class="sxs-lookup"><span data-stu-id="49dcd-111">If you are eligible for  private offers, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="49dcd-112">現在、プライベートプランは、Azure portal で検索またはフィルターできません (カテゴリ別)。</span><span class="sxs-lookup"><span data-stu-id="49dcd-112">Private offers are currently not searchable or filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="49dcd-113">Azure portal で、[ **+ リソースの作成** ] を選択するか、[marketplace] を検索して **marketplace** のページにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="49dcd-113">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="49dcd-114">プライベートプランの資格をお持ちの場合は、ページの上部に **プライベートプランの利用可能なバナーが** 表示されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-114">If you are eligible for private offers, you will see the **You have private offers available** banner on the top of the page.</span></span> <span data-ttu-id="49dcd-115">[プライベート **プランの表示** ] を選択して、プライベートプランページにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="49dcd-115">Select **View private offers** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="使用可能なプライベートプランがあるときに表示されるバナー。":::

<span data-ttu-id="49dcd-117">または、[プライベートプラン] バナーが表示されている場合は、製品ギャラリーページの下部までスクロールしても、プライベートプランのサブセットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-117">Alternately, if you see the private offers banner, you can also scroll to the bottom of the product gallery page and you will see a subset of your private offers.</span></span> <span data-ttu-id="49dcd-118">リンクを選択すると、プライベートプランページにアクセスするための **詳細が表示** されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-118">Select the link to **See More** to go to your private offers page.</span></span>

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="画面の下部にプライベートプランが表示され、[詳細を表示] リンクが表示されます。":::

## <a name="review-private-plans"></a><span data-ttu-id="49dcd-120">プライベートプランの確認</span><span class="sxs-lookup"><span data-stu-id="49dcd-120">Review private plans</span></span>

<span data-ttu-id="49dcd-121">プライベートプランは、実際にはオファー内のプライベートプランです。</span><span class="sxs-lookup"><span data-stu-id="49dcd-121">A private offer is actually a private plan within an offer.</span></span> <span data-ttu-id="49dcd-122">各プランには、パブリックとプライベートの両方の複数のプランを含めることができますが、プライベートプランはパブリックプランとは別のリストに記載されています。</span><span class="sxs-lookup"><span data-stu-id="49dcd-122">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="49dcd-123">使用可能なプライベートプランは、特徴的な **プライベート** バッジでマークされた [**プラン**] タブで確認できます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-123">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="プライベートとマークされたプランのページ。":::

<span data-ttu-id="49dcd-125">複数のサブスクリプションがある場合は、すべてのサブスクリプションで利用可能なすべてのプライベートプランが表示されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-125">If you have more than one subscription, you will see all private offers available for all your subscriptions.</span></span> <span data-ttu-id="49dcd-126">[ **作成**] を選択すると、リソースの作成ページにルーティングされ、リソースの構成が開始されます。</span><span class="sxs-lookup"><span data-stu-id="49dcd-126">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="49dcd-127">[ **作成** ] を選択し、複数のサブスクリプションを持っていても、それらのすべてがプライベートプランに追加されていない場合は、既定のサブスクリプションがこのプライベートプランの対象となるサブスクリプションではない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="49dcd-127">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private offer.</span></span> <span data-ttu-id="49dcd-128">この場合は、適切なサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="49dcd-128">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="使用可能なプライベートプランが他にもあることを示すリンクが表示されます。":::

## <a name="next-steps"></a><span data-ttu-id="49dcd-130">次の手順</span><span class="sxs-lookup"><span data-stu-id="49dcd-130">Next steps</span></span>

- [<span data-ttu-id="49dcd-131">Azure Marketplace とは何ですか?</span><span class="sxs-lookup"><span data-stu-id="49dcd-131">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
