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
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702894"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="c84e2-103">MPN アカウントの所在地を管理し、場所を追加 (削除) する</span><span class="sxs-lookup"><span data-stu-id="c84e2-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="c84e2-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c84e2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="c84e2-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c84e2-105">Global admin</span></span>
- <span data-ttu-id="c84e2-106">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="c84e2-106">Account admin</span></span>

<span data-ttu-id="c84e2-107">所在地 MPN ID では、貴社の特定の各場所が示されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="c84e2-108">所在地 MPN ID を使用して、インセンティブ プログラムに登録し、クラウド ソリューション プロバイダー (CSP) ビジネスの取引を行い、他のビジネス トランザクションを行います。</span><span class="sxs-lookup"><span data-stu-id="c84e2-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="c84e2-109">グローバル MPN ID は、サポート リクエストなどの非トランザクション アクティビティに使用されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="c84e2-110">以下は、一般的なシナリオです。</span><span class="sxs-lookup"><span data-stu-id="c84e2-110">The following scenario is typical:</span></span>

<span data-ttu-id="c84e2-111">Contoso のパートナー グローバル アカウント (PGA) の場所はイギリスです。</span><span class="sxs-lookup"><span data-stu-id="c84e2-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="c84e2-112">PGA は、登録された法的な事業所であり、そのグローバル MPN ID はすべての非トランザクション ビジネスを管理するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="c84e2-113">Contoso には、イギリスの別の場所、フランス、米国にある子会社または部門に相当するパートナー ロケーション アカウント (PLA) もあります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="c84e2-114">MPN アカウントの構造では、これらの PLA は一意の所在地 MPN ID として表現されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="c84e2-115">PLA は、CSP またはインセンティブ プログラムなどのトランザクション ビジネスに使用されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="c84e2-116">支払いは、特定の場所に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="c84e2-117">CSP テナントと MPN 所在地 ID の間には 1 対 1 の関係があります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="MPN 所在地の構造":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="c84e2-119">CSP ビジネスの新しいアカウントを追加するための前提条件</span><span class="sxs-lookup"><span data-stu-id="c84e2-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="c84e2-120">新しい CSP ビジネス アカウントを追加するには、まず前提条件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="c84e2-121">CSP ビジネスを遂行する国に、所在地 MPN ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="c84e2-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="c84e2-122">新しい MPN 所在地を作成するには、以下の「MPN 所在地を追加する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="c84e2-123">新しい CSP Indirect Reseller 登録を作成するには、[間接プロバイダーとの連携](indirect-reseller-tasks-in-partner-center.md#get-started)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="c84e2-124">必ず、**新しい** CSP アカウントの **新しい** 資格情報でサインインするようにしてください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="c84e2-125">既存の資格情報を使用しないでください。既にアカウントを持っているものとしてパートナー センターに認識されてしまいます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="c84e2-126">Microsoft Partner Agreement に同意し、アカウントをアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="c84e2-127">直接請求パートナーとして登録する場合は、[直接請求パートナーの要件](direct-partner-new-requirements.md)に関する記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="c84e2-128">MPN 所在地の確認と更新</span><span class="sxs-lookup"><span data-stu-id="c84e2-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="c84e2-129">MPN アカウントの資格情報を使用して、パートナー センター [ダッシュボード](https://partner.microsoft.com/dashboard/home)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="c84e2-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="c84e2-130">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)</span><span class="sxs-lookup"><span data-stu-id="c84e2-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="c84e2-131">**[設定]** アイコンで、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[Legal]\(法務\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="c84e2-132">**[パートナー]** タブで、PMC から移行した場所の修正を求めるバナー エラー メッセージがないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="c84e2-133">場所が PMC で正しく設定されておらず、まだ PC に移行されていない場合は、それらの場所を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="場所を更新する方法を示すスクリーンショット。":::
 
4.  <span data-ttu-id="c84e2-135">**[Review PMC locations]\(PMC の場所の確認\)** 画面で、 **[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="c84e2-136">次のフィールドを更新します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-136">Update the following fields:</span></span>

- <span data-ttu-id="c84e2-137">**名前フィールド**: 会社の所在地の名前が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="c84e2-138">重複するエラーが表示された場合は、たとえば Contoso から Contoso, Inc. に変更してみてください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="c84e2-139">**法人フィールド**: 場所が関連付けられている法人を選択していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="c84e2-140">**住所行 1 および 2 フィールド**: 住所が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="c84e2-141">**市区町村/都道府県フィールド**: 市区町村と都道府県の組み合わせが正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="c84e2-142">市区町村/都道府県を選択するためのドロップダウン メニューが適用される国と、フィールドを手動で挿入する必要がある国があります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="c84e2-143">**郵便番号フィールド**: 郵便番号フィールドが、示されている国、地域、都市、または住所と一致していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="c84e2-144">**第一連絡先担当者情報フィールド**: 姓と名フィールドが入力されていること、および指定された電子メール アドレスが個人のものではなく、職場のものであることを確認します (@outlook.com、@live.com など)。</span><span class="sxs-lookup"><span data-stu-id="c84e2-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="c84e2-145">**電話番号フィールド**: 電話番号に特殊文字、スペース、または国番号が含まれていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="c84e2-146">電話番号フィールドに入力した値には、常に最大 10 文字が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="c84e2-147">エラー メッセージがない場合は、 **[設定]** で、 **[アカウント設定]** 、 **[組織プロファイル]** 、 **[識別子]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="c84e2-148">この CSP アカウントの国と一致する "Location (場所)" という種類の MPN ID を見つけ、それを使用して関連付けを完了します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="c84e2-149">使用する CSP アカウントと一致する場所の MPN ID が見つからない場合は、新しい場所を追加して新しい MPN ID を作成できます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="c84e2-150">下の「**MPN 所在地を追加する**」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="c84e2-151">MPN 所在地を追加する</span><span class="sxs-lookup"><span data-stu-id="c84e2-151">Add an MPN location</span></span>

1. <span data-ttu-id="c84e2-152">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="c84e2-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="c84e2-153">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="c84e2-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="c84e2-154">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="c84e2-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="c84e2-155">**設定アイコン** で、 **[Account settings]\(アカウント設定\)** を選択し、 **[組織プロファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="c84e2-156">**[Legal]\(法務\)** 選択し、 **[パートナー]** タブで **[事業所]** を選択してから、 **[Add a location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c84e2-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="c84e2-157">会社に追加する場所の法人名、住所、連絡先など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="c84e2-158">**[Add location]\(場所の追加\)** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c84e2-158">Click **Add location**.</span></span> <span data-ttu-id="c84e2-159">これにより、CSP 取引とインセンティブに使用できる新しい場所の新しい MPN ID が作成されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="新しい法的ビジネスの追加":::

> [!NOTE]
> <span data-ttu-id="c84e2-161">パートナー センターで追加された場所は、削除できません。</span><span class="sxs-lookup"><span data-stu-id="c84e2-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="c84e2-162">正しい MPN ID を使用してサインインすると、パートナー センターの左側のメニューに **MPN** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="c84e2-163">登録番号 ID の追加</span><span class="sxs-lookup"><span data-stu-id="c84e2-163">Add the registration number ID</span></span>

<span data-ttu-id="c84e2-164">間接プロバイダー、直接請求パートナー、または間接リセラーであり、次の国で新規または既存の顧客とビジネスを行う場合は、ビジネス用の登録 ID 番号を準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="c84e2-165">ビジネスを行っている国が以下に記載されていない場合、登録 ID はオプションです。</span><span class="sxs-lookup"><span data-stu-id="c84e2-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="c84e2-166">アルメニア</span><span class="sxs-lookup"><span data-stu-id="c84e2-166">Armenia</span></span> 
- <span data-ttu-id="c84e2-167">アゼルバイジャン</span><span class="sxs-lookup"><span data-stu-id="c84e2-167">Azerbaijan</span></span> 
- <span data-ttu-id="c84e2-168">ベラルーシ</span><span class="sxs-lookup"><span data-stu-id="c84e2-168">Belarus</span></span> 
- <span data-ttu-id="c84e2-169">ブラジル</span><span class="sxs-lookup"><span data-stu-id="c84e2-169">Brazil</span></span> 
- <span data-ttu-id="c84e2-170">ハンガリー</span><span class="sxs-lookup"><span data-stu-id="c84e2-170">Hungary</span></span> 
- <span data-ttu-id="c84e2-171">インド</span><span class="sxs-lookup"><span data-stu-id="c84e2-171">India</span></span> 
- <span data-ttu-id="c84e2-172">イラク</span><span class="sxs-lookup"><span data-stu-id="c84e2-172">Iraq</span></span> 
- <span data-ttu-id="c84e2-173">カザフスタン</span><span class="sxs-lookup"><span data-stu-id="c84e2-173">Kazakhstan</span></span> 
- <span data-ttu-id="c84e2-174">キルギスタン</span><span class="sxs-lookup"><span data-stu-id="c84e2-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="c84e2-175">モルドバ</span><span class="sxs-lookup"><span data-stu-id="c84e2-175">Moldova</span></span> 
- <span data-ttu-id="c84e2-176">ミャンマー</span><span class="sxs-lookup"><span data-stu-id="c84e2-176">Myanmar</span></span> 
- <span data-ttu-id="c84e2-177">ポーランド</span><span class="sxs-lookup"><span data-stu-id="c84e2-177">Poland</span></span> 
- <span data-ttu-id="c84e2-178">ロシア</span><span class="sxs-lookup"><span data-stu-id="c84e2-178">Russia</span></span> 
- <span data-ttu-id="c84e2-179">サウジアラビア</span><span class="sxs-lookup"><span data-stu-id="c84e2-179">Saudi Arabia</span></span> 
- <span data-ttu-id="c84e2-180">南アフリカ</span><span class="sxs-lookup"><span data-stu-id="c84e2-180">South Africa</span></span> 
- <span data-ttu-id="c84e2-181">南スーダン</span><span class="sxs-lookup"><span data-stu-id="c84e2-181">South Sudan</span></span>  
- <span data-ttu-id="c84e2-182">タジキスタン</span><span class="sxs-lookup"><span data-stu-id="c84e2-182">Tajikistan</span></span> 
- <span data-ttu-id="c84e2-183">タイ</span><span class="sxs-lookup"><span data-stu-id="c84e2-183">Thailand</span></span>
- <span data-ttu-id="c84e2-184">トルコ</span><span class="sxs-lookup"><span data-stu-id="c84e2-184">Turkey</span></span> 
- <span data-ttu-id="c84e2-185">ウクライナ</span><span class="sxs-lookup"><span data-stu-id="c84e2-185">Ukraine</span></span> 
- <span data-ttu-id="c84e2-186">アラブ首長国連邦</span><span class="sxs-lookup"><span data-stu-id="c84e2-186">United Arab Emirates</span></span> 
- <span data-ttu-id="c84e2-187">ウズベキスタン</span><span class="sxs-lookup"><span data-stu-id="c84e2-187">Uzbekistan</span></span> 
- <span data-ttu-id="c84e2-188">ベネズエラ</span><span class="sxs-lookup"><span data-stu-id="c84e2-188">Venezuela</span></span>
- <span data-ttu-id="c84e2-189">ベトナム</span><span class="sxs-lookup"><span data-stu-id="c84e2-189">Vietnam</span></span> 


<span data-ttu-id="c84e2-190">詳細については、「[登録 ID 番号の情報](reg-number-id.md)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="c84e2-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="c84e2-191">場所を削除する</span><span class="sxs-lookup"><span data-stu-id="c84e2-191">Delete a location</span></span>

<span data-ttu-id="c84e2-192">アカウントから場所を削除するには、[パートナー サポート](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b)に連絡する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="c84e2-193">このアクションによる影響を十分に理解してください。</span><span class="sxs-lookup"><span data-stu-id="c84e2-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="c84e2-194">削除された場所は取得できなくなり、その特定の MPN ID に関連付けられているものはすべて認識されなくなるか、貴社に対して有効でなくなります。</span><span class="sxs-lookup"><span data-stu-id="c84e2-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="c84e2-195">パートナー グローバル アカウントの国を変更する</span><span class="sxs-lookup"><span data-stu-id="c84e2-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="c84e2-196">パートナー センターで MPN アカウントを使用してサインインします</span><span class="sxs-lookup"><span data-stu-id="c84e2-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="c84e2-197">(MPN の資格情報は、CSP の資格情報とは異なる場合があります)。</span><span class="sxs-lookup"><span data-stu-id="c84e2-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="c84e2-198">MPN アカウントには、グローバル管理者またはアカウント管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="c84e2-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="c84e2-199">**[パートナー]** タブの **[事業所]** で場所の一覧を確認し、法人にしようとしている場所が一覧表示されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="c84e2-200">場所を追加するには、 **[Add a location]\(場所の追加\)** をクリックし、ポップアップに、会社に追加する場所の法人名、住所、第一連絡先担当者など、必要な詳細情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c84e2-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="c84e2-201">**[国/地域]** ドロップダウンの横にある **[Change your country]\(国の変更\)** を選択し、手順に従います。</span><span class="sxs-lookup"><span data-stu-id="c84e2-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="法的ビジネス プロファイル データのポップアップ":::

5. <span data-ttu-id="c84e2-203">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c84e2-203">Click **Save**.</span></span>

6. <span data-ttu-id="c84e2-204">MPN グローバル アカウントの国が、新しい法律上の国に変更されます。</span><span class="sxs-lookup"><span data-stu-id="c84e2-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="c84e2-205">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c84e2-205">Next steps</span></span>

- <span data-ttu-id="c84e2-206">[検証プロセス](verification-responses.md)に関する詳細情報。</span><span class="sxs-lookup"><span data-stu-id="c84e2-206">Learn about the [verification process](verification-responses.md).</span></span>
