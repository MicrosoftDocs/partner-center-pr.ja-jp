---
title: パートナー アカウントで場所を管理する
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 新しい場所を追加する方法や、所在地 MPN ID がインセンティブ プログラム、CSP ビジネス、サブスクリプション、その他のトランザクションでどのように使用されるかについて説明します。
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 13d6e7dc4722227035be2b24df48427f2008bb14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151782"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="969dc-103">MPN アカウントの所在地を管理し、場所を追加 (削除) する</span><span class="sxs-lookup"><span data-stu-id="969dc-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="969dc-104">**対象のロール**: グローバル管理者 | アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="969dc-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="969dc-105">所在地 MPN ID では、貴社の特定の各場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-105">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="969dc-106">所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="969dc-106">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="969dc-107">グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-107">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="969dc-108">以下は、一般的なシナリオです。</span><span class="sxs-lookup"><span data-stu-id="969dc-108">The following scenario is typical:</span></span>

<span data-ttu-id="969dc-109">Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。</span><span class="sxs-lookup"><span data-stu-id="969dc-109">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="969dc-110">PGA は、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-110">The PGA is their registered legal business, and its global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="969dc-111">Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。</span><span class="sxs-lookup"><span data-stu-id="969dc-111">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="969dc-112">MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-112">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="969dc-113">PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-113">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="969dc-114">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="969dc-114">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="969dc-115">CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。</span><span class="sxs-lookup"><span data-stu-id="969dc-115">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="969dc-117">CSP ビジネスの新しいアカウントを追加するための前提条件</span><span class="sxs-lookup"><span data-stu-id="969dc-117">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="969dc-118">新しい CSP ビジネス アカウントを追加するには、まず前提条件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-118">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="969dc-119">CSP ビジネスを遂行する国に、所在地 MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="969dc-119">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="969dc-120">新しい MPN 所在地を作成するには、以下の「MPN 所在地を追加する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="969dc-120">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="969dc-121">新しい CSP Indirect Reseller 登録を作成するには、[間接プロバイダーとの連携](indirect-reseller-tasks-in-partner-center.md#get-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="969dc-121">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="969dc-122">必ず、**新しい** CSP アカウントの **新しい** 資格情報でサインインするようにしてください。</span><span class="sxs-lookup"><span data-stu-id="969dc-122">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="969dc-123">既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。</span><span class="sxs-lookup"><span data-stu-id="969dc-123">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="969dc-124">Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="969dc-124">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="969dc-125">直接請求パートナーとして登録する場合は、[直接請求パートナーの要件](direct-partner-new-requirements.md)に関する記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="969dc-125">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="969dc-126">MPN 所在地の確認と更新</span><span class="sxs-lookup"><span data-stu-id="969dc-126">View and update your MPN locations</span></span>

1. <span data-ttu-id="969dc-127">MPN アカウントの資格情報を使用して、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="969dc-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="969dc-128">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)</span><span class="sxs-lookup"><span data-stu-id="969dc-128">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="969dc-129">**[設定]** アイコンで、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[Legal]\(法務\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-129">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="969dc-130">**[パートナー]** タブで、PMC から移行した場所の修正を求めるバナー エラー メッセージがないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-130">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="969dc-131">場所が PMC で正しく設定されておらず、まだ PC に移行されていない場合は、それらの場所を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="969dc-131">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="場所を更新する方法を示すスクリーンショット。":::
 
4.  <span data-ttu-id="969dc-133">**[Review PMC locations]\(PMC の場所の確認\)** 画面で、 **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-133">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="969dc-134">次のフィールドを更新します。</span><span class="sxs-lookup"><span data-stu-id="969dc-134">Update the following fields:</span></span>

- <span data-ttu-id="969dc-135">**名前フィールド**: 会社の所在地の名前が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-135">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="969dc-136">重複するエラーが表示された場合は、たとえば Contoso から Contoso, Inc. に変更してみてください。</span><span class="sxs-lookup"><span data-stu-id="969dc-136">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="969dc-137">**法人フィールド**: 場所が関連付けられている法人を選択していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-137">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="969dc-138">**住所行 1 および 2 フィールド**: 住所が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-138">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="969dc-139">**市区町村/都道府県フィールド**: 市区町村と都道府県の組み合わせが正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-139">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="969dc-140">市区町村/都道府県を選択するためのドロップダウン メニューが適用される国と、フィールドを手動で挿入する必要がある国があります。</span><span class="sxs-lookup"><span data-stu-id="969dc-140">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="969dc-141">**郵便番号フィールド**: 郵便番号フィールドが、示されている国、地域、都市、または住所と一致していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-141">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="969dc-142">**第一連絡先担当者情報フィールド**: 姓と名フィールドが入力されていること、および指定された電子メール アドレスが個人のものではなく、職場のものであることを確認します (@outlook.com、@live.com など)。</span><span class="sxs-lookup"><span data-stu-id="969dc-142">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="969dc-143">**電話番号フィールド**: 電話番号に特殊文字、スペース、または国番号が含まれていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-143">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="969dc-144">電話番号フィールドに入力した値には、常に最大 10 文字が含まれます。</span><span class="sxs-lookup"><span data-stu-id="969dc-144">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="969dc-145">エラー メッセージがない場合は、 **[設定]** で、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[識別子]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-145">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="969dc-146">この CSP アカウントの国と一致する "Location (場所)" という種類の MPN ID を見つけ、それを使用して関連付けを完了します。</span><span class="sxs-lookup"><span data-stu-id="969dc-146">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="969dc-147">使用する CSP アカウントと一致する場所の MPN ID が見つからない場合は、新しい場所を追加して新しい MPN ID を作成できます。</span><span class="sxs-lookup"><span data-stu-id="969dc-147">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="969dc-148">下の「**MPN 所在地を追加する**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="969dc-148">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="969dc-149">MPN 所在地を追加する</span><span class="sxs-lookup"><span data-stu-id="969dc-149">Add an MPN location</span></span>

1. <span data-ttu-id="969dc-150">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="969dc-150">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="969dc-151">(MPN の資格情報は、CSP の資格情報と異なる場合があります)。MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="969dc-151">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="969dc-152">**設定アイコン** で、 **[Account settings]\(アカウント設定\)** を選択し、 **[組織プロファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-152">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="969dc-153">**[Legal]\(法務\)** を選択し、 **[パートナー]** タブで **[事業所]** を選択してから、 **[Add a location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="969dc-153">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and select **Add a location.**</span></span>

3. <span data-ttu-id="969dc-154">会社に追加する場所の法人名、住所、連絡先など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="969dc-154">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="969dc-155">**[場所の追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-155">Select **Add location**.</span></span> <span data-ttu-id="969dc-156">これにより、CSP 取引とインセンティブに使用できる新しい場所の新しい MPN ID が作成されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-156">This will create a new MPN ID for the new location that you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新しい法的ビジネスの追加":::

> [!NOTE]
> <span data-ttu-id="969dc-158">パートナー センターで追加された場所は、削除できません。</span><span class="sxs-lookup"><span data-stu-id="969dc-158">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="969dc-159">正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-159">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="969dc-160">登録番号 ID の追加</span><span class="sxs-lookup"><span data-stu-id="969dc-160">Add the registration number ID</span></span>

<span data-ttu-id="969dc-161">間接プロバイダー、直接請求パートナー、または間接リセラーであり、次の国で新規または既存の顧客とビジネスを行う場合は、ビジネス用の登録 ID 番号を準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="969dc-161">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="969dc-162">ビジネスを行っている国が下に記載されていない場合、登録 ID はオプションです。</span><span class="sxs-lookup"><span data-stu-id="969dc-162">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="969dc-163">アルメニア</span><span class="sxs-lookup"><span data-stu-id="969dc-163">Armenia</span></span> 
- <span data-ttu-id="969dc-164">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="969dc-164">Azerbaijan</span></span> 
- <span data-ttu-id="969dc-165">ベラルーシ</span><span class="sxs-lookup"><span data-stu-id="969dc-165">Belarus</span></span> 
- <span data-ttu-id="969dc-166">ブラジル</span><span class="sxs-lookup"><span data-stu-id="969dc-166">Brazil</span></span> 
- <span data-ttu-id="969dc-167">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="969dc-167">Hungary</span></span> 
- <span data-ttu-id="969dc-168">インド</span><span class="sxs-lookup"><span data-stu-id="969dc-168">India</span></span> 
- <span data-ttu-id="969dc-169">イラク</span><span class="sxs-lookup"><span data-stu-id="969dc-169">Iraq</span></span> 
- <span data-ttu-id="969dc-170">カザフスタン</span><span class="sxs-lookup"><span data-stu-id="969dc-170">Kazakhstan</span></span> 
- <span data-ttu-id="969dc-171">キルギスタン</span><span class="sxs-lookup"><span data-stu-id="969dc-171">Kyrgyzstan</span></span> 
- <span data-ttu-id="969dc-172">モルドバ</span><span class="sxs-lookup"><span data-stu-id="969dc-172">Moldova</span></span> 
- <span data-ttu-id="969dc-173">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="969dc-173">Myanmar</span></span> 
- <span data-ttu-id="969dc-174">ポーランド</span><span class="sxs-lookup"><span data-stu-id="969dc-174">Poland</span></span> 
- <span data-ttu-id="969dc-175">ロシア</span><span class="sxs-lookup"><span data-stu-id="969dc-175">Russia</span></span> 
- <span data-ttu-id="969dc-176">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="969dc-176">Saudi Arabia</span></span> 
- <span data-ttu-id="969dc-177">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="969dc-177">South Africa</span></span> 
- <span data-ttu-id="969dc-178">南スーダン</span><span class="sxs-lookup"><span data-stu-id="969dc-178">South Sudan</span></span>  
- <span data-ttu-id="969dc-179">タジキスタン</span><span class="sxs-lookup"><span data-stu-id="969dc-179">Tajikistan</span></span> 
- <span data-ttu-id="969dc-180">タイ</span><span class="sxs-lookup"><span data-stu-id="969dc-180">Thailand</span></span>
- <span data-ttu-id="969dc-181">トルコ</span><span class="sxs-lookup"><span data-stu-id="969dc-181">Turkey</span></span> 
- <span data-ttu-id="969dc-182">ウクライナ</span><span class="sxs-lookup"><span data-stu-id="969dc-182">Ukraine</span></span> 
- <span data-ttu-id="969dc-183">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="969dc-183">United Arab Emirates</span></span> 
- <span data-ttu-id="969dc-184">ウズベキスタン</span><span class="sxs-lookup"><span data-stu-id="969dc-184">Uzbekistan</span></span> 
- <span data-ttu-id="969dc-185">ベネズエラ</span><span class="sxs-lookup"><span data-stu-id="969dc-185">Venezuela</span></span>
- <span data-ttu-id="969dc-186">ベトナム</span><span class="sxs-lookup"><span data-stu-id="969dc-186">Vietnam</span></span> 


<span data-ttu-id="969dc-187">詳細については、「[登録 ID 番号の情報](reg-number-id.md)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="969dc-187">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="969dc-188">場所を削除する</span><span class="sxs-lookup"><span data-stu-id="969dc-188">Delete a location</span></span>

<span data-ttu-id="969dc-189">アカウントから場所を削除するには、[パートナー サポート](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)に連絡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="969dc-189">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="969dc-190">このアクションによる影響を十分に理解してください。</span><span class="sxs-lookup"><span data-stu-id="969dc-190">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="969dc-191">削除された場所は取得できなくなり、その特定の MPN ID に関連付けられているものはすべて認識されなくなるか、貴社に対して有効でなくなります。</span><span class="sxs-lookup"><span data-stu-id="969dc-191">Deleted locations cannot be retrieved and anything tied to that specific MPN ID will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="969dc-192">パートナー グローバル アカウントの国を変更する</span><span class="sxs-lookup"><span data-stu-id="969dc-192">Change country of Partner global account</span></span> 

1. <span data-ttu-id="969dc-193">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="969dc-193">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="969dc-194">(MPN の資格情報は、CSP の資格情報と異なる場合があります)。MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="969dc-194">(Your MPN credentials may be different from your CSP credentials.) The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="969dc-195">**[パートナー]** タブの **[事業所]** で場所の一覧を確認し、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="969dc-195">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="969dc-196">場所を追加するには、 **[Add a location]\(場所の追加\)** をクリックし、ポップアップに、会社に追加する場所の法人名、住所、第一連絡先担当者など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="969dc-196">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="969dc-197">**[国/地域]** ドロップダウン リストの横にある **[Change your country]\(国の変更\)** を選択し、手順に従います。</span><span class="sxs-lookup"><span data-stu-id="969dc-197">Select **Change your country** next to the **Country/region** drop-down list and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法的ビジネス プロファイル データのポップアップ":::

5. <span data-ttu-id="969dc-199">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="969dc-199">Select **Save**.</span></span>

6. <span data-ttu-id="969dc-200">MPN グローバル アカウントの国が、新しい法律上の国に変更されます。</span><span class="sxs-lookup"><span data-stu-id="969dc-200">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="969dc-201">次のステップ</span><span class="sxs-lookup"><span data-stu-id="969dc-201">Next steps</span></span>

- <span data-ttu-id="969dc-202">[検証プロセス](verification-responses.md)に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="969dc-202">Learn about the [verification process](verification-responses.md).</span></span>
