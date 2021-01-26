---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773428"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="ea410-103">MPN アカウントの所在地を管理し、新しい場所を追加する</span><span class="sxs-lookup"><span data-stu-id="ea410-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="ea410-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="ea410-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ea410-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="ea410-105">Global admin</span></span>
- <span data-ttu-id="ea410-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="ea410-106">Account admin</span></span>

<span data-ttu-id="ea410-107">所在地 MPN ID では、貴社の特定の各場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="ea410-108">所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="ea410-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="ea410-109">グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="ea410-110">一般的なシナリオを示します。</span><span class="sxs-lookup"><span data-stu-id="ea410-110">The following is a typical scenario:</span></span>

<span data-ttu-id="ea410-111">Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。</span><span class="sxs-lookup"><span data-stu-id="ea410-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="ea410-112">これは、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="ea410-113">Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。</span><span class="sxs-lookup"><span data-stu-id="ea410-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="ea410-114">MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="ea410-115">PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="ea410-116">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="ea410-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="ea410-117">CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。</span><span class="sxs-lookup"><span data-stu-id="ea410-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="ea410-119">CSP ビジネスの新しいアカウントの場所を追加するための前提条件</span><span class="sxs-lookup"><span data-stu-id="ea410-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="ea410-120">新しい CSP 事業拠点を追加するには、いくつかの前提条件があります。</span><span class="sxs-lookup"><span data-stu-id="ea410-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="ea410-121">ビジネスを遂行する国に、所在地 MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea410-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="ea410-122">CSP にまだ登録されていない[ビジネス リージョン](regional-authorization-overview.md)には、新しい Azure AD テナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="ea410-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="ea410-123">CSP に登録するときに、これを作成してください。</span><span class="sxs-lookup"><span data-stu-id="ea410-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="ea410-124">新しい AAD テナントを使用して、リージョンの CSP プログラムに登録します。</span><span class="sxs-lookup"><span data-stu-id="ea410-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="ea410-125">法的企業名、住所、主要連絡先の詳細など、会社の法的な詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ea410-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="ea410-126">このアカウントは検証されるため、必ず有効な情報を追加してください。</span><span class="sxs-lookup"><span data-stu-id="ea410-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="ea410-127">必ず、**新しい** Azure AD テナントの **新しい** 資格情報でサインインするようにしてください。</span><span class="sxs-lookup"><span data-stu-id="ea410-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="ea410-128">既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。</span><span class="sxs-lookup"><span data-stu-id="ea410-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="ea410-129">Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="ea410-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="ea410-130">MPN 所在地を追加する</span><span class="sxs-lookup"><span data-stu-id="ea410-130">Add an MPN location</span></span>

1. <span data-ttu-id="ea410-131">パートナー センターで MPN アカウントを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="ea410-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="ea410-132">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="ea410-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="ea410-133">**設定アイコン** から **[組織の設定]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ea410-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="ea410-134">**[Legal]\(法務\)** を選択し、 **[場所]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ea410-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="ea410-135">**[Add a location]\(場所の追加\)** を選択し、会社に追加する場所の住所の詳細と、その場所の主要な連絡先を挿入します。</span><span class="sxs-lookup"><span data-stu-id="ea410-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="ea410-136">パートナー センターで追加した場所は削除できません。</span><span class="sxs-lookup"><span data-stu-id="ea410-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="ea410-137">正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="ea410-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="ea410-138">グローバル パートナー アカウントの場所を変更する</span><span class="sxs-lookup"><span data-stu-id="ea410-138">Change Global partner account location</span></span>

1. <span data-ttu-id="ea410-139">**[[Business locations]\(事業所\)](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** で場所の一覧を確認して、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ea410-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="ea410-140">ない場合は、追加します。</span><span class="sxs-lookup"><span data-stu-id="ea410-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="現在のすべての場所の一覧が表示されている、パートナー センターのアカウントの場所ページのスクリーンショット。":::

2. <span data-ttu-id="ea410-142">**[Legal]\(法務\)** を選択してから、 **[Update legal business profile]\(法的ビジネス プロファイルの更新\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ea410-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="ea410-143">地域と法人を選択し、その **[送信]** を実行します。</span><span class="sxs-lookup"><span data-stu-id="ea410-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="ea410-144">次のステップ</span><span class="sxs-lookup"><span data-stu-id="ea410-144">Next steps</span></span>

- <span data-ttu-id="ea410-145">[検証プロセス](verification-responses.md)に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="ea410-145">Learn about the [verification process](verification-responses.md).</span></span>
