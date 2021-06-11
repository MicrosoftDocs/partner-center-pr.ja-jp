---
title: プライベート プラン (Microsoft AppSource
description: プライベート プランを Microsoft AppSource (Azure Marketplace) で設定します。
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008552"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="1cbcd-103">プライベート プラン (Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="1cbcd-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="1cbcd-104">プライベート プランは、発行元が特定の顧客にカスタム プランを提供する方法です。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="1cbcd-105">このオプションは、次のMicrosoft AppSource。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="1cbcd-106">プライベート プランは、AppSource でサービスとしてのソフトウェア (SaaS) オファーに対して販売できます。このプランは、今すぐ使用する行動を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="1cbcd-107">ISV にプライベート プランを求める</span><span class="sxs-lookup"><span data-stu-id="1cbcd-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="1cbcd-108">AppSource でプライベート プランを利用するには、ISV に直接問い合わせ、カスタム価格と技術仕様をネゴシエートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="1cbcd-109">プライベート プランの条項に同意すると、ISV によって自動的にプランが作成され、組織のテナント ID に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="1cbcd-110">テナント ID の検索</span><span class="sxs-lookup"><span data-stu-id="1cbcd-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="1cbcd-111">AppSource の右上隅にあるアカウント プロファイル アイコンを選択し、[テナントの表示] **を選択します**。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="1cbcd-112">テナント ID をコピーし、ISV に指定します。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="テナント ID を検索する方法を示します。":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="1cbcd-114">AppSource でプライベート プランを検索する</span><span class="sxs-lookup"><span data-stu-id="1cbcd-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="1cbcd-115">ISV が新しいプライベート プランを発行してから AppSource に表示するには、最大で 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="1cbcd-116">テナント ID に関連付けられているプライベート プランを見つけるには、AppSource の右上にある [プライベート プラン] **(ロック** アイコン) を選択します。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="上部のツール バーにロック アイコン (ロックロック) が表示されます。":::

<span data-ttu-id="1cbcd-118">サインインしていない場合は、メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="1cbcd-119">その後、[プランと価格] タブで、テナント ID に関連付 **けられているプライベート プランを購入** できます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="[プランと価格] タブにプライベート オファーが表示されます。":::

<span data-ttu-id="1cbcd-121">テナントでプライベート プランを使用できない場合は、プライベート プランやオファーを持たなかったというメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="1cbcd-122">プライベート プランを購入する</span><span class="sxs-lookup"><span data-stu-id="1cbcd-122">Purchase a private plan</span></span>

<span data-ttu-id="1cbcd-123">ISV には、オファー内に 1 つ以上のプライベート プランを含めできます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="1cbcd-124">各オファーはパブリックプランとプライベート プランの両方を持つ場合がありますが、プライベート プランは、ページの右上にあるプライベート オファー アイコン (ロック) からアクセスされる個別のオファー登録情報ページの下に表示されます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="1cbcd-125">[プランと価格] タブに、使用可能 **なプライベート プランが表示** されます。プライベート プランには、独特の青いバッジが付きます。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="プライベート オファーの横に青いプライベート オファー バッジが表示されます。":::

<span data-ttu-id="1cbcd-127">選択したプランを購入するには、[今すぐ取得] **を選択** し、提供されている手順に従います。</span><span class="sxs-lookup"><span data-stu-id="1cbcd-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1cbcd-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="1cbcd-128">Next steps</span></span>

- [<span data-ttu-id="1cbcd-129">Microsoft AppSource とは</span><span class="sxs-lookup"><span data-stu-id="1cbcd-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
