---
title: パートナー センターで支払いと税金のプロファイルを作成および管理する
ms.topic: how-to
ms.date: 06/29/2020
description: インセンティブの作業に対して支払いを受けるには、支払いと税金のプロファイルを作成する必要があります。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: 3e7424ff1329d9c2bf13e9a6c4181c312396e073
ms.sourcegitcommit: 8dc139749916c822c5c438f54a03d2f147697dd5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/04/2020
ms.locfileid: "87546043"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a11df-103">パートナー センターでの支払いプロファイルと税務プロファイル</span><span class="sxs-lookup"><span data-stu-id="a11df-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a11df-104">適用対象:</span><span class="sxs-lookup"><span data-stu-id="a11df-104">Applies to:</span></span>

- <span data-ttu-id="a11df-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a11df-105">Partner Center</span></span>

<span data-ttu-id="a11df-106">特定の MPN の場所についてインセンティブ プログラムの支払いを受けるには、有効な支払いおよび税務プロファイルを、プログラムおよび MPN の場所に事前に関連付けて、登録を完了しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="a11df-107">支払いの発行には、この支払いおよび税務プロファイルが使用されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="a11df-108">インセンティブ プログラムのルールによっては、支払いに対して銀行の電子送信やクレジット ノートを使用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="a11df-109">適切なロール:</span><span class="sxs-lookup"><span data-stu-id="a11df-109">Appropriate roles:</span></span>

- <span data-ttu-id="a11df-110">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="a11df-110">Incentives admin</span></span>
- <span data-ttu-id="a11df-111">課金管理者</span><span class="sxs-lookup"><span data-stu-id="a11df-111">Billing admin</span></span>
- <span data-ttu-id="a11df-112">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a11df-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a11df-113">パートナー センターで支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="a11df-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a11df-114">以下のセクションでは、パートナーセンターで支払いと税金のプロファイルを作成および管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a11df-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a11df-115">パートナーセンターで支払いプロファイルを作成または管理するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="a11df-116">インセンティブの役割は、各インセンティブプログラムの下にある各 MPN の場所に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="a11df-117">パートナーセンターでインセンティブ管理者を追加する方法の詳細については、「[パートナーセンターでインセンティブユーザーまたは管理者を追加する方法](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="a11df-118">パートナーセンターの支払いと税金のセクションにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a11df-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="a11df-119">AAD アカウント (会社のアカウント) を使用してパートナーセンターにログインします。または、適切な電子メールアドレスが割り当てられている場合は、それを使用します。</span><span class="sxs-lookup"><span data-stu-id="a11df-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="a11df-120">1つの AAD アカウント内に複数のドメインを登録できます。</span><span class="sxs-lookup"><span data-stu-id="a11df-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="a11df-121">グローバル管理者に連絡して、どのドメインが関連付けられているかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="a11df-122">ドメインでのみログインできる場合は、 **@onmicrosoft.com** アカウント管理者に連絡して、AAD アカウントにドメインを追加してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="a11df-123">**職場または学校**アカウントまたは**個人アカウント**を選択するよう求められた場合は、[**職場または学校アカウント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="a11df-124">歯車アイコンを選択して [**設定**] メニューを開き、[**パートナー設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="a11df-125">[**アカウント設定**] メニューで、[**支払いと税金**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="a11df-126">個々のプログラムに支払いと税金のプロファイルを割り当てる</span><span class="sxs-lookup"><span data-stu-id="a11df-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="a11df-127">パートナーセンターで歯車アイコンを選択して、[**設定**] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="a11df-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="a11df-128">[**パートナーの設定**] を選択し、[**支払いと税金] セクション**を展開して、[**支払いと税金のプロファイルの割り当て**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="a11df-129">プログラムの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="a11df-130">プログラムの横にある矢印を選択すると、プロファイルの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="a11df-131">[**税プロファイル**] ドロップダウンメニューで、必要な税プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a11df-132">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a11df-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="a11df-133">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a11df-134">新しい税プロファイルを作成するプロセスについては、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="a11df-135">**支払い方法**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="a11df-136">支払方法として [**電子銀行口座の転送**] を選択した場合は、[支払いプロファイル] ドロップダウンで、必要な支払いプロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="a11df-137">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a11df-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="a11df-138">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a11df-139">新しい支払いプロファイルを作成するプロセスを次に示します。</span><span class="sxs-lookup"><span data-stu-id="a11df-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="a11df-140">支払い方法として**クレジットメモ**を選択した場合は、参照されている SAP 番号が組織に属していることを確認するための確認を行います。</span><span class="sxs-lookup"><span data-stu-id="a11df-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a11df-141">複数の Microsoft ビジネスエンティティが一覧表示されている場合は、各エンティティの支払いプロファイルを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a11df-142">支払い方法の可用性は、インセンティブプログラムのルールに依存します。</span><span class="sxs-lookup"><span data-stu-id="a11df-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="a11df-143">**通貨**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="a11df-144">すべての支払いフィールドを完了したら、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="a11df-145">銀行のプロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="a11df-145">Create your bank profile</span></span>

<span data-ttu-id="a11df-146">銀行プロファイルは、組織レベルで作成されます。これにより、組織内の複数の MPN ID およびインセンティブプログラムに同じ銀行プロファイルを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a11df-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="a11df-147">異なる銀行や税金のルールが適用される可能性があるため、銀行のプロファイルを異なる国に適用するときに例外が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="a11df-148">次のページでは、アスタリスクの付いたフィールドが必要です。</span><span class="sxs-lookup"><span data-stu-id="a11df-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="a11df-149">フィールドの内容がわからない場合は、情報アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="a11df-150">[**詳細**] ページで、次のフィールドを入力します。 [**プロファイル名]:** この支払いプロファイルを識別する一意の名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="a11df-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="a11df-151">**銀行口座の場所:** 会社の銀行がある国。</span><span class="sxs-lookup"><span data-stu-id="a11df-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="a11df-152">**支払い方法:** パートナーセンターのお支払い方法としては、電子銀行の譲渡をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a11df-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="a11df-153">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-153">Select **Next**.</span></span>

3. <span data-ttu-id="a11df-154">[**銀行口座**] ページで、情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="a11df-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="a11df-155">このページに表示されるフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a11df-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="a11df-156">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-156">Select **Next**.</span></span>

5. <span data-ttu-id="a11df-157">[**受益者**] ページで、適切な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="a11df-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="a11df-158">受益者は、お客様がアカウントについて話し合う必要がある場合に、銀行が連絡する会社の人物です。</span><span class="sxs-lookup"><span data-stu-id="a11df-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="a11df-159">フィールドが完了したら、[**完了**] を選択し、[**確認**] を選択して、銀行プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="a11df-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="a11df-160">[**支払いと税金のプロファイル**] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a11df-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="a11df-161">新しいプロファイルの状態には、検証が完了するまで、**保留中の Microsoft 検証**が反映されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="a11df-162">これには最大48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="a11df-162">This may take up to 48 hours.</span></span> <span data-ttu-id="a11df-163">検証が完了すると、プロファイルの状態には、**承認済み**または**操作**が反映されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="a11df-164">**操作が必要な**場合は、上記の手順を繰り返して必要な情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="a11df-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="a11df-165">税務プロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="a11df-165">Create your tax profile</span></span>

<span data-ttu-id="a11df-166">次の手順を使用して、組織に必要な税金情報を Microsoft に提供します。</span><span class="sxs-lookup"><span data-stu-id="a11df-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="a11df-167">このセクションのページは動的であり、お住まいの国または地域によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a11df-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="a11df-168">正しい税金情報を特定するためのヘルプが必要な場合は、お住まいの国の適切な政府機関にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a11df-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="a11df-169">南北アメリカのパートナー企業の場合、W8 または W9 フォームの完了に関する情報が必要な場合は、次のアドレスを使用して IRS サイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="a11df-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="a11df-170">会社の詳細のみを入力してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-170">Enter only details for your company.</span></span> <span data-ttu-id="a11df-171">個人情報を入力しないでください。</span><span class="sxs-lookup"><span data-stu-id="a11df-171">Never enter personal details.</span></span>

1. <span data-ttu-id="a11df-172">[**ビジネスプロファイル**] ページで、必須フィールドに入力し、[**次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="a11df-173">[**セットアップ**] ページで、会社に適用するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="a11df-174">会社が米国に組み込まれている場合、またはこのプロファイルが個人向けの場合は、左側のオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="a11df-175">会社が米国の外部に組み込まれている場合は、右側のオプションを選択し、一覧から国/地域を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="a11df-176">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-176">Select **Next**.</span></span> 

4. <span data-ttu-id="a11df-177">[**納税の状態**] ページで必要な情報を入力し、[**次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="a11df-178">このページのフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a11df-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="a11df-179">詳細。</span><span class="sxs-lookup"><span data-stu-id="a11df-179">your details.</span></span> 

5. <span data-ttu-id="a11df-180">[**追加のドキュメント**] ページの [必須フィールド] をクリックし、[**次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="a11df-181">[**参照**] を選択して、お住まいの国または地域で必要なドキュメントをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="a11df-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="a11df-182">ドキュメント名が表示されたら、[**アップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="a11df-183">ドキュメントを削除する必要がある場合は、[**削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="a11df-184">保存して続行するには、[**完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="a11df-185">ポップアップメッセージで [**確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="a11df-186">[**支払いと税金の設定**] ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="a11df-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="a11df-187">支払いと税金プロファイルに関してよく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="a11df-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="a11df-188">支払いや税金の詳細を提供する必要があるのはなぜですか。</span><span class="sxs-lookup"><span data-stu-id="a11df-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="a11df-189">Microsoft インセンティブプログラムの支払いを受け取るには、有効な支払いと税金の詳細を提供して登録を完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="a11df-190">登録は、指定した支払いと税金プロファイルが Microsoft によって検証された場合にのみ完了したと見なされます。</span><span class="sxs-lookup"><span data-stu-id="a11df-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="a11df-191">支払いや税金の詳細を提供/更新する必要があることを操作方法していますか。</span><span class="sxs-lookup"><span data-stu-id="a11df-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="a11df-192">新しいインセンティブプログラムに登録するすべてのパートナーは、登録を完了するために有効な支払いと税金の詳細を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="a11df-193">また、インセンティブプログラムのルールが変更された場合、またはプロファイルのアスペクトが期限切れになった場合や古くなった場合にも、更新された情報を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="a11df-194">この場合、[概要] ページに [**アクションが必要] の状態 (更新プログラムの銀行または税プロファイル)** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="a11df-195">支払い/税金の詳細を提供/更新するには、どうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="a11df-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="a11df-196">パートナーセンターで支払いと税金の詳細を更新する方法の詳細については、「[パートナーセンターで銀行と税金のプロファイルを作成および管理する方法](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="a11df-197">支払いおよび税務プロファイルを割り当てるとき、登録が表示されないのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="a11df-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="a11df-198">支払いおよび税務プロファイルを作成または管理できるのは、MPN の場所のインセンティブ管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="a11df-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="a11df-199">適切なアクセス許可を持っていないか、これらのアクセス許可がないアカウントでログインしている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a11df-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="a11df-200">銀行と税金のアクセス許可の管理については、組織の管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="a11df-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="a11df-201">使用できる組織の支払いおよび税務プロファイルは、どこで確認できますか?</span><span class="sxs-lookup"><span data-stu-id="a11df-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="a11df-202">支払いと税金のプロファイルを表示するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="a11df-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="a11df-203">パートナー センターにログインします。</span><span class="sxs-lookup"><span data-stu-id="a11df-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="a11df-204">歯車アイコンを選択して **[設定]** メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="a11df-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="a11df-205">[**パートナーの設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="a11df-206">**[アカウントの設定]** で、 **[Payout and tax]\(支払いと税金\)** を選択し、 **[Payout and tax profile]\(支払いおよび税務プロファイル\)** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a11df-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="a11df-207">既存のすべての支払いおよび税務プロファイルとその状態が、編集可能な状態で表示されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="a11df-208">組織が複数のインセンティブプログラムに参加しています。</span><span class="sxs-lookup"><span data-stu-id="a11df-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="a11df-209">支払いと税金のプロファイルを何度も入力する必要がありますか。</span><span class="sxs-lookup"><span data-stu-id="a11df-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="a11df-210">支払いプロファイルを使用する場合は、ご自身が決めることができます。</span><span class="sxs-lookup"><span data-stu-id="a11df-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="a11df-211">支払いプロファイルは組織レベルで作成されます。このため、組織内の複数の MPN ID とインセンティブ プログラムに、同じ銀行プロファイルを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a11df-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="a11df-212">ほとんどの場合、既存のプロファイルを再利用するか、新しいプロファイルを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="a11df-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="a11df-213">ただし、銀行プロファイルをさまざまな国またはリージョンに適用するときは、現地の銀行または税法規が適用される場合があるため、例外が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="a11df-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="a11df-214">MPN の場所に対して作成された税務プロファイルは、その MPN の場所が他のインセンティブ プログラムに参加すると再利用され、自動的に入力されます。</span><span class="sxs-lookup"><span data-stu-id="a11df-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="a11df-215">ただし、例外が発生する場合もあります。</span><span class="sxs-lookup"><span data-stu-id="a11df-215">But there can be exceptions.</span></span> <span data-ttu-id="a11df-216">たとえば、新しいインセンティブ プログラムの支払いルールに基づいて、税務プロファイルの追加情報が求められることがあります。</span><span class="sxs-lookup"><span data-stu-id="a11df-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="a11df-217">自分のドメインでのみログインでき @onmicrosoft.com ます。</span><span class="sxs-lookup"><span data-stu-id="a11df-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="a11df-218">どうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="a11df-218">What should I do?</span></span>

<span data-ttu-id="a11df-219">ドメインを AAD アカウントに追加するには、アカウント管理者に連絡してください。</span><span class="sxs-lookup"><span data-stu-id="a11df-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
