---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005909"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="7b248-103">MPN アカウントの所在地を管理し、場所を追加 (削除) する</span><span class="sxs-lookup"><span data-stu-id="7b248-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="7b248-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="7b248-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7b248-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="7b248-105">Global admin</span></span>
- <span data-ttu-id="7b248-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="7b248-106">Account admin</span></span>

<span data-ttu-id="7b248-107">所在地 MPN ID では、貴社の特定の各場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="7b248-108">所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="7b248-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="7b248-109">グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="7b248-110">一般的なシナリオを示します。</span><span class="sxs-lookup"><span data-stu-id="7b248-110">The following is a typical scenario:</span></span>

<span data-ttu-id="7b248-111">Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。</span><span class="sxs-lookup"><span data-stu-id="7b248-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="7b248-112">これは、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="7b248-113">Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。</span><span class="sxs-lookup"><span data-stu-id="7b248-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="7b248-114">MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="7b248-115">PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="7b248-116">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="7b248-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="7b248-117">CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。</span><span class="sxs-lookup"><span data-stu-id="7b248-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="7b248-119">CSP ビジネスの新しいアカウントを追加するための前提条件</span><span class="sxs-lookup"><span data-stu-id="7b248-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="7b248-120">新しい CSP ビジネス アカウントを追加するには、まず前提条件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7b248-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="7b248-121">CSP ビジネスを遂行する国に、所在地 MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b248-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="7b248-122">新しい MPN 所在地を作成するには、以下の「MPN 所在地を追加する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b248-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="7b248-123">新しい CSP Indirect Reseller 登録を作成するには、[間接プロバイダーとの連携](indirect-reseller-tasks-in-partner-center.md#get-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b248-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="7b248-124">必ず、**新しい** CSP アカウントの **新しい** 資格情報でサインインするようにしてください。</span><span class="sxs-lookup"><span data-stu-id="7b248-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="7b248-125">既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。</span><span class="sxs-lookup"><span data-stu-id="7b248-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="7b248-126">Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="7b248-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="7b248-127">直接請求パートナーとして登録する場合は、[直接請求パートナーの要件](direct-partner-new-requirements.md)に関する記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="7b248-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="7b248-128">MPN 所在地を表示する</span><span class="sxs-lookup"><span data-stu-id="7b248-128">View your MPN locations</span></span>

1. <span data-ttu-id="7b248-129">MPN アカウントの資格情報を使用して、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7b248-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="7b248-130">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)</span><span class="sxs-lookup"><span data-stu-id="7b248-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="7b248-131">**[設定]** アイコンで、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[Legal]\(法務\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b248-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="7b248-132">**[パートナー]** タブで、PMC から移行した場所の修正を求めるバナー エラー メッセージがないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="7b248-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="7b248-133">存在する場合は、指示に従って、それらの場所を修正します。</span><span class="sxs-lookup"><span data-stu-id="7b248-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="7b248-134">エラー メッセージがない場合は、 **[設定]** で、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[識別子]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b248-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="7b248-135">この CSP アカウントの国と一致する "Location" という種類の MPN ID を見つけ、それを使用して以下の検索を行い、関連付けを完了します。</span><span class="sxs-lookup"><span data-stu-id="7b248-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="7b248-136">使用する CSP アカウントと一致する場所の MPN ID が見つからない場合は、新しい場所を追加して新しい MPN ID を作成できます。</span><span class="sxs-lookup"><span data-stu-id="7b248-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="7b248-137">下の「**MPN 所在地を追加する**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b248-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="7b248-138">MPN 所在地を追加する</span><span class="sxs-lookup"><span data-stu-id="7b248-138">Add an MPN location</span></span>

1. <span data-ttu-id="7b248-139">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="7b248-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7b248-140">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="7b248-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="7b248-141">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b248-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="7b248-142">**設定アイコン** で、 **[Account settings]\(アカウント設定\)** を選択し、 **[組織プロファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b248-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="7b248-143">**[Legal]\(法務\)** 選択し、 **[パートナー]** タブで **[事業所]** を選択してから、 **[Add a location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7b248-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="7b248-144">会社に追加する場所の法人名、住所、連絡先など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="7b248-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="7b248-145">**[Add location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7b248-145">Click **Add location**.</span></span> <span data-ttu-id="7b248-146">これにより、CSP 取引とインセンティブに使用できる新しい場所の新しい MPN ID が作成されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新しい法的ビジネスの追加":::

> [!NOTE]
> <span data-ttu-id="7b248-148">パートナー センターで追加された場所は、削除できません。</span><span class="sxs-lookup"><span data-stu-id="7b248-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="7b248-149">正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="7b248-150">場所を削除する</span><span class="sxs-lookup"><span data-stu-id="7b248-150">Delete a location</span></span>

<span data-ttu-id="7b248-151">アカウントから場所を削除するには、[パートナー サポート](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)に連絡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7b248-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="7b248-152">このアクションによる影響を十分に理解してください。</span><span class="sxs-lookup"><span data-stu-id="7b248-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="7b248-153">削除された場所は取得できなくなり、その特定の MPN ID に関連付けられているものはすべて認識されなくなるか、貴社に対して有効でなくなります。</span><span class="sxs-lookup"><span data-stu-id="7b248-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="7b248-154">パートナー グローバル アカウントの国を変更する</span><span class="sxs-lookup"><span data-stu-id="7b248-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="7b248-155">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="7b248-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="7b248-156">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="7b248-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="7b248-157">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="7b248-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="7b248-158">**[パートナー]** タブの **[事業所]** で場所の一覧を確認し、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="7b248-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="7b248-159">場所を追加するには、 **[Add a location]\(場所の追加\)** をクリックし、ポップアップに、会社に追加する場所の法人名、住所、第一連絡先担当者など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="7b248-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="7b248-160">**[国/地域]** ドロップダウンの横にある **[Change your country]\(国の変更\)** を選択し、手順に従います。</span><span class="sxs-lookup"><span data-stu-id="7b248-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法的ビジネス プロファイル データのポップアップ":::

5. <span data-ttu-id="7b248-162">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7b248-162">Click **Save**.</span></span>

6. <span data-ttu-id="7b248-163">MPN グローバル アカウントの国が、新しい法律上の国に変更されます。</span><span class="sxs-lookup"><span data-stu-id="7b248-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="7b248-164">次のステップ</span><span class="sxs-lookup"><span data-stu-id="7b248-164">Next steps</span></span>

- <span data-ttu-id="7b248-165">[検証プロセス](verification-responses.md)に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="7b248-165">Learn about the [verification process](verification-responses.md).</span></span>
