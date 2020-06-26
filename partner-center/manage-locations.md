---
title: パートナー アカウントで場所を管理する
ms.topic: article
ms.date: 06/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: パートナー センターで、新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプションなどのトランザクションでどのように使用されるかについて説明します。
author: LauraBrenner
ms.author: labrenne
keywords: パートナー アカウント, 場所
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 6cce4b38cb27d8cef88f71ced6fe985631a24914
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909060"
---
# <a name="manage-your-partner-account-locations-in-partner-center-and-add-a-new-location"></a><span data-ttu-id="01449-104">パートナー センターでのパートナー アカウントの場所の管理と新しい場所の追加</span><span class="sxs-lookup"><span data-stu-id="01449-104">Manage your partner account locations in Partner Center and add a new location</span></span>

<span data-ttu-id="01449-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="01449-105">**Appropriate roles**</span></span>
- <span data-ttu-id="01449-106">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="01449-106">Global admin</span></span>
- <span data-ttu-id="01449-107">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="01449-107">User admin</span></span>
- <span data-ttu-id="01449-108">課金管理者</span><span class="sxs-lookup"><span data-stu-id="01449-108">Billing admin</span></span>
- <span data-ttu-id="01449-109">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="01449-109">Admin agent</span></span>
- <span data-ttu-id="01449-110">販売代理店</span><span class="sxs-lookup"><span data-stu-id="01449-110">Sales agent</span></span>

<span data-ttu-id="01449-111">場所 MPN ID では、パートナー企業の特定の場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="01449-111">The location MPN IDs identify each specific location of your company.</span></span> <span data-ttu-id="01449-112">場所 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、新しいサブスクリプションを追加し、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="01449-112">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, to add new subscriptions, and other business transactions.</span></span> <span data-ttu-id="01449-113">会社 MPN ID は、サポート要求などの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="01449-113">The company MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="01449-114">一般的なシナリオを示します。</span><span class="sxs-lookup"><span data-stu-id="01449-114">The following is a typical scenario:</span></span>

<span data-ttu-id="01449-115">パートナー企業は、CSP ビジネスと発行ビジネスを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="01449-115">A partner company can have a CSP business and a publishing business.</span></span> <span data-ttu-id="01449-116">その CSP ビジネスは複数のロケールで行うことができ、発行ビジネスは他のロケールで行うことができます。登録済みの法的ビジネスでは、ユーザーの追加やサポート要求のログ記録など、すべての非トランザクション ビジネスを管理するために 1 つの MPN ID を使用しています。</span><span class="sxs-lookup"><span data-stu-id="01449-116">Their CSP business can be located in several locales and their pub business may be located in other locales.Their registered legal business has one MPN ID used for managing all non-transactional business such as adding users or logging support requests.</span></span>


<span data-ttu-id="01449-117">それぞれの場所には、CSP やインセンティブ プログラムなどのトランザクション ビジネスに使用される MPN ID があります。</span><span class="sxs-lookup"><span data-stu-id="01449-117">Each of their locations has an MPN ID used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="01449-118">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="01449-118">Payouts are tied to specific locations.</span></span>

<span data-ttu-id="01449-119">ユーザーは場所をまたがってロールを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="01449-119">Users may have roles that cross locations.</span></span> <span data-ttu-id="01449-120">たとえば、インセンティブ管理者は、ヨーロッパのすべての場所でそのロールを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="01449-120">For example, the incentives admin could have that role for all locations in Europe.</span></span>

## <a name="to-add-a-location"></a><span data-ttu-id="01449-121">場所を追加するには</span><span class="sxs-lookup"><span data-stu-id="01449-121">To add a location</span></span>

1. <span data-ttu-id="01449-122">**設定アイコン**から **[Partner settings]\(パートナーの設定\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="01449-122">From the **Setting icon**, select the **Partner settings**.</span></span>

2. <span data-ttu-id="01449-123">**[場所]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="01449-123">Select **Locations.**</span></span>

3. <span data-ttu-id="01449-124">**[Add a location]\(場所の追加\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="01449-124">Select **Add a location**.</span></span>  

4. <span data-ttu-id="01449-125">**[Add a location]\(場所の追加\)** ページで、会社に追加する場所の住所の詳細と、その場所の主要な連絡先を挿入します。</span><span class="sxs-lookup"><span data-stu-id="01449-125">In the **Add a location** page, insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="01449-126">パートナー センターで追加した場所は削除できません。</span><span class="sxs-lookup"><span data-stu-id="01449-126">Once a location is added in Partner Center, it cannot be removed.</span></span>

## <a name="change-legal-headquarters-location"></a><span data-ttu-id="01449-127">法的な本社の場所を変更する</span><span class="sxs-lookup"><span data-stu-id="01449-127">Change legal headquarters location</span></span>

1. <span data-ttu-id="01449-128">**[場所]** ページで場所の一覧を確認して、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="01449-128">On the **Locations** page, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="01449-129">ない場合は、追加します。</span><span class="sxs-lookup"><span data-stu-id="01449-129">If it isn't, add it.</span></span>

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="現在のすべての場所の一覧が表示されている、パートナー センターのアカウントの場所ページのスクリーンショット。":::

2. <span data-ttu-id="01449-131">**[パートナー プロファイル]** を選択してから、 **[Update legal business profile] (法的ビジネス プロファイルの更新)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="01449-131">Select **Partner profile** and then select **Update legal business profile**</span></span>

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="パートナー センターのアカウント パートナー プロファイル情報を示すスクリーンショット。[更新] オプションが選択可能になっています。":::

3. <span data-ttu-id="01449-133">地域と法人を選択し、その **[送信]** を実行します。</span><span class="sxs-lookup"><span data-stu-id="01449-133">Select the region and legal entity and **Submit** it.</span></span>

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="パートナーの法的ビジネス プロファイルを更新する画面のスクリーンショット。国または地域と法人を更新するためのドロップダウン リストが表示されています。":::
