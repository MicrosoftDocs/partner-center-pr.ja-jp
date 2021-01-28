---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925052"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="fcbe8-103">MPN アカウントの所在地を管理し、新しい場所を追加する</span><span class="sxs-lookup"><span data-stu-id="fcbe8-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="fcbe8-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="fcbe8-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fcbe8-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="fcbe8-105">Global admin</span></span>
- <span data-ttu-id="fcbe8-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="fcbe8-106">Account admin</span></span>

<span data-ttu-id="fcbe8-107">所在地 MPN ID では、貴社の特定の各場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="fcbe8-108">所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="fcbe8-109">グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="fcbe8-110">一般的なシナリオを示します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-110">The following is a typical scenario:</span></span>

<span data-ttu-id="fcbe8-111">Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="fcbe8-112">これは、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="fcbe8-113">Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="fcbe8-114">MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="fcbe8-115">PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="fcbe8-116">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="fcbe8-117">CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="fcbe8-119">CSP ビジネスの新しいアカウントを追加するための前提条件</span><span class="sxs-lookup"><span data-stu-id="fcbe8-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="fcbe8-120">新しい CSP ビジネス アカウントを追加するには、まず前提条件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="fcbe8-121">CSP ビジネスを遂行する国に、所在地 MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="fcbe8-122">新しい MPN 所在地を作成するには、以下の「MPN 所在地を追加する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="fcbe8-123">新しい CSP Indirect Reseller 登録を作成するには、[間接プロバイダーとの連携](indirect-reseller-tasks-in-partner-center.md#get-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="fcbe8-124">必ず、**新しい** CSP アカウントの **新しい** 資格情報でサインインするようにしてください。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="fcbe8-125">既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="fcbe8-126">Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="fcbe8-127">MPN 所在地を追加する</span><span class="sxs-lookup"><span data-stu-id="fcbe8-127">Add an MPN location</span></span>

1. <span data-ttu-id="fcbe8-128">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="fcbe8-128">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fcbe8-129">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-129">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fcbe8-130">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-130">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="fcbe8-131">**設定アイコン** で、 **[Account settings]\(アカウント設定\)** を選択し、 **[組織プロファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-131">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="fcbe8-132">**[Legal]\(法務\)** 選択し、 **[パートナー]** タブで **[事業所]** を選択してから、 **[Add a location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-132">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="fcbe8-133">会社に追加する場所の法人名、住所、連絡先など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-133">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="fcbe8-134">**[Add location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-134">Click **Add location**.</span></span> <span data-ttu-id="fcbe8-135">これにより、CSP 取引とインセンティブに使用できる新しい場所の新しい MPN ID が作成されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-135">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新しい法的ビジネスの追加":::

> [!NOTE]
> <span data-ttu-id="fcbe8-137">パートナー センターで追加した場所は削除できません。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-137">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="fcbe8-138">正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-138">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="fcbe8-139">パートナー グローバル アカウントの国を変更する</span><span class="sxs-lookup"><span data-stu-id="fcbe8-139">Change country of Partner global account</span></span> 

1. <span data-ttu-id="fcbe8-140">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="fcbe8-140">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="fcbe8-141">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-141">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="fcbe8-142">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-142">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="fcbe8-143">**[パートナー]** タブの **[事業所]** で場所の一覧を確認し、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-143">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="fcbe8-144">場所を追加するには、 **[Add a location]\(場所の追加\)** をクリックし、ポップアップに、会社に追加する場所の法人名、住所、第一連絡先担当者など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-144">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="fcbe8-145">**[国/地域]** ドロップダウンの横にある **[Change your country]\(国の変更\)** を選択し、手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-145">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法的ビジネス プロファイル データのポップアップ":::

5. <span data-ttu-id="fcbe8-147">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-147">Click **Save**.</span></span>

6. <span data-ttu-id="fcbe8-148">MPN グローバル アカウントの国が、新しい法律上の国に変更されます。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-148">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="fcbe8-149">次のステップ</span><span class="sxs-lookup"><span data-stu-id="fcbe8-149">Next steps</span></span>

- <span data-ttu-id="fcbe8-150">[検証プロセス](verification-responses.md)に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="fcbe8-150">Learn about the [verification process](verification-responses.md).</span></span>
