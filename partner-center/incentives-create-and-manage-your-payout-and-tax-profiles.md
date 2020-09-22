---
title: パートナー センターでの支払いプロファイルと税務プロファイル
ms.topic: how-to
ms.date: 09/11/2020
description: 支払いと税金のプロファイルを作成および管理して、インセンティブの作業に対して支払うことができます。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: de143ecfae1b803e0743a28db5cda5ae9a3d5f2d
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999316"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a1527-103">パートナーセンターでインセンティブの支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="a1527-103">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a1527-104">**適用対象:**</span><span class="sxs-lookup"><span data-stu-id="a1527-104">**Applies to:**</span></span>

- <span data-ttu-id="a1527-105">パートナー センター</span><span class="sxs-lookup"><span data-stu-id="a1527-105">Partner Center</span></span>

<span data-ttu-id="a1527-106">**適切なロール:**</span><span class="sxs-lookup"><span data-stu-id="a1527-106">**Appropriate roles:**</span></span>

- <span data-ttu-id="a1527-107">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="a1527-107">Incentives admin</span></span>
- <span data-ttu-id="a1527-108">課金管理者</span><span class="sxs-lookup"><span data-stu-id="a1527-108">Billing admin</span></span>
- <span data-ttu-id="a1527-109">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="a1527-109">Global admin</span></span>

<span data-ttu-id="a1527-110">特定の MPN の場所についてインセンティブ プログラムの支払いを受けるには、有効な支払いおよび税務プロファイルを、プログラムおよび MPN の場所に事前に関連付けて、登録を完了しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-110">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="a1527-111">支払いの発行には、この支払いおよび税務プロファイルが使用されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-111">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="a1527-112">インセンティブ プログラムのルールによっては、支払いに対して銀行の電子送信やクレジット ノートを使用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-112">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="a1527-113">役割、通貨、およびその他の Microsoft プログラム</span><span class="sxs-lookup"><span data-stu-id="a1527-113">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="a1527-114">支払いと税金のプロファイルを開始する前に、以下の情報を理解しておくことが重要です。</span><span class="sxs-lookup"><span data-stu-id="a1527-114">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="a1527-115">ロールとアクセス許可</span><span class="sxs-lookup"><span data-stu-id="a1527-115">Roles and permissions</span></span>

<span data-ttu-id="a1527-116">インセンティブ支払いのために銀行および税金の情報を入力するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-116">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="a1527-117">MPN/アカウント管理者の場合は、自分または同僚を割り当てて、インセンティブ管理者にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a1527-117">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="a1527-118">インセンティブ管理者のアクセス許可を要求する必要がある場合は、MPN 管理者または全体管理者にお問い合わせください。 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインすることで、社内のユーザーがこれらのロールを持っていることを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a1527-118">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="a1527-119">右上にある [ **設定** ] アイコンから、[ **ユーザー管理** ] を選択し、グローバル管理者に対してフィルター処理を行います。</span><span class="sxs-lookup"><span data-stu-id="a1527-119">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="a1527-120">インセンティブのユーザーは、インセンティブの利益および支払いの詳細とレポートを表示できますが、銀行や税金の詳細を編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="a1527-120">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="a1527-121">出金通貨の選択</span><span class="sxs-lookup"><span data-stu-id="a1527-121">Choose your disbursement currency</span></span>

<span data-ttu-id="a1527-122">既定では、インセンティブ支払いはそれぞれのエンティティの現地通貨で行われます。</span><span class="sxs-lookup"><span data-stu-id="a1527-122">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="a1527-123">プロファイルの設定時に別の通貨を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="a1527-123">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="a1527-124">支払いは、Microsoft が毎月設定した換算レートを使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="a1527-125">通貨が選択されているため、値の変更について責任があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="a1527-126">銀行および税金に関する情報とその他のプログラム</span><span class="sxs-lookup"><span data-stu-id="a1527-126">Bank and tax information and other programs</span></span>

<span data-ttu-id="a1527-127">Microsoft が既に銀行データを支払いに使用している場合でも、以下に説明する情報を入力してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-127">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="a1527-128">これにより、会社のデータのプライバシーとセキュリティが確保されます。新しいツールにプロファイルをコピーすると、機密情報が公開される可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="a1527-128">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="a1527-129">このプロセスを実行することで、データが完全で正確であることを確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="a1527-129">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="a1527-130">さまざまな Microsoft プログラムに異なるプロファイルを使用する</span><span class="sxs-lookup"><span data-stu-id="a1527-130">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="a1527-131">小売業では、5つの小売インセンティブプログラムごとに、同じ銀行口座に支払うことができます。</span><span class="sxs-lookup"><span data-stu-id="a1527-131">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="a1527-132">別の方法として、製品版の Xbox 支払いを1つの銀行口座にすることもできます。この場合、小売オフィスは別の銀行口座に支払われます。</span><span class="sxs-lookup"><span data-stu-id="a1527-132">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a1527-133">パートナー センターで支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="a1527-133">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a1527-134">以下のセクションでは、パートナーセンターで支払いと税金のプロファイルを作成および管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a1527-134">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a1527-135">パートナーセンターで支払いプロファイルを作成または管理するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-135">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="a1527-136">インセンティブの役割は、各インセンティブプログラムの下にある各 MPN の場所に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-136">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="a1527-137">パートナーセンターでインセンティブ管理者を追加する方法の詳細については、「 [ユーザーアカウントの作成](create-user-accounts-and-set-permissions.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-137">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="a1527-138">パートナーセンターの支払いと税金のセクションにアクセスする</span><span class="sxs-lookup"><span data-stu-id="a1527-138">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="a1527-139">Azure Active Directory (Azure AD) アカウント (会社のアカウント) を使用して [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインします。または、該当する電子メールアドレスが割り当てられている場合は、適切な電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="a1527-139">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="a1527-140">1つの Azure AD アカウント内に複数のドメインを登録できます。</span><span class="sxs-lookup"><span data-stu-id="a1527-140">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="a1527-141">グローバル管理者に連絡して、どのドメインが関連付けられているかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-141">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="a1527-142">ドメインでのみログインできる場合は、 @onmicrosoft.com アカウント管理者に連絡して、Azure AD アカウントにドメインを追加してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-142">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="a1527-143">**職場または学校**のアカウントまたは**個人のアカウント**を選択するように求められたら、[**職場または学校アカウント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-143">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="a1527-144">歯車アイコンを選択して [ **設定** ] メニューを開き、[ **パートナー設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-144">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="a1527-145">[ **アカウント設定** ] メニューで、[ **支払いと税金**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-145">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="a1527-146">個々のプログラムに支払いと税金のプロファイルを割り当てる</span><span class="sxs-lookup"><span data-stu-id="a1527-146">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="a1527-147">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、歯車アイコンを選択して [**設定**] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="a1527-147">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="a1527-148">[ **パートナーの設定**] を選択し、[ **支払いと税金] セクション**を展開して、[ **支払いと税金のプロファイルの割り当て**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-148">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="a1527-149">プログラムの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-149">A list of your programs will be displayed.</span></span> <span data-ttu-id="a1527-150">プログラムの横にある矢印を選択すると、プロファイルの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-150">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="a1527-151">[ **税プロファイル** ] ドロップダウンメニューで、必要な税プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-151">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a1527-152">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a1527-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="a1527-153">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a1527-154">新しい税プロファイルを作成するプロセスについては、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-154">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="a1527-155">**支払い方法**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-155">Select **Payment method**.</span></span>

   - <span data-ttu-id="a1527-156">支払い方法として [ **電子銀行の転送** ] を選択した場合は、目的の支払プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-156">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a1527-157">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a1527-157">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="a1527-158">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-158">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a1527-159">新しい支払いプロファイルを作成するプロセスを次に示します。</span><span class="sxs-lookup"><span data-stu-id="a1527-159">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="a1527-160">支払い方法として **クレジットメモ** を選択した場合は、検証を完了します。</span><span class="sxs-lookup"><span data-stu-id="a1527-160">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="a1527-161">これにより、参照されている SAP 番号が組織に属していることが確認されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-161">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a1527-162">複数の Microsoft ビジネスエンティティが一覧表示されている場合は、各エンティティの支払いプロファイルを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-162">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a1527-163">支払い方法の可用性は、インセンティブプログラムのルールに依存します。</span><span class="sxs-lookup"><span data-stu-id="a1527-163">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="a1527-164">**通貨**を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-164">Select the **Currency**.</span></span>

6. <span data-ttu-id="a1527-165">すべての支払いフィールドを完了したら、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-165">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="a1527-166">銀行のプロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="a1527-166">Create your bank profile</span></span>

<span data-ttu-id="a1527-167">銀行のプロファイルは、組織レベルで作成されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-167">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="a1527-168">これにより、組織内の複数の MPN ID およびインセンティブプログラムに対して1つの銀行プロファイルを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a1527-168">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="a1527-169">異なる銀行や税金のルールが適用される可能性があるため、銀行のプロファイルを異なる国に適用するときに例外が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="a1527-169">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="a1527-170">次のページでは、アスタリスクの付いたフィールドが必要です。</span><span class="sxs-lookup"><span data-stu-id="a1527-170">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="a1527-171">フィールドの内容がわからない場合は、情報アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-171">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="a1527-172">[ **詳細** ] ページで、次のフィールドを入力します。 [ **プロファイル名]:** この支払いプロファイルを識別する一意の名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="a1527-172">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="a1527-173">**銀行口座の場所:** 会社の銀行がある国。</span><span class="sxs-lookup"><span data-stu-id="a1527-173">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="a1527-174">**支払い方法:** パートナーセンターのお支払い方法として、電子銀行の譲渡をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a1527-174">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="a1527-175">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-175">Select **Next**.</span></span>

3. <span data-ttu-id="a1527-176">[ **銀行口座** ] ページで、情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="a1527-176">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="a1527-177">このページに表示されるフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a1527-177">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="a1527-178">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-178">Select **Next**.</span></span>

5. <span data-ttu-id="a1527-179">[ **受益者** ] ページで、適切な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="a1527-179">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="a1527-180">受益者は、お客様がアカウントについて話し合う必要がある場合に、銀行が連絡する会社の人物です。</span><span class="sxs-lookup"><span data-stu-id="a1527-180">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="a1527-181">フィールドが完了したら、[ **完了**] を選択し、[ **確認** ] を選択して、銀行プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="a1527-181">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="a1527-182">[ **支払いと税金のプロファイル** ] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="a1527-182">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="a1527-183">新しいプロファイルの状態には、検証が完了するまで、 **保留中の Microsoft 検証** が反映されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-183">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="a1527-184">このプロセスには最大48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="a1527-184">This process may take up to 48 hours.</span></span> <span data-ttu-id="a1527-185">検証が完了すると、プロファイルの状態には、 **承認済み** または **操作**が反映されます。</span><span class="sxs-lookup"><span data-stu-id="a1527-185">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="a1527-186">**操作が必要な**場合は、上記の手順を繰り返して必要な情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="a1527-186">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="a1527-187">税務プロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="a1527-187">Create your tax profile</span></span>

<span data-ttu-id="a1527-188">次の手順を使用して、組織に必要な税金情報を Microsoft に提供します。</span><span class="sxs-lookup"><span data-stu-id="a1527-188">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="a1527-189">このセクションのページは動的であり、お住まいの国または地域によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a1527-189">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="a1527-190">正しい税金情報を特定するためのヘルプが必要な場合は、お住まいの国の適切な政府機関にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a1527-190">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="a1527-191">南北アメリカのパートナー企業の場合、W8 または W9 フォームの完了に関する情報が必要な場合は、次のアドレスを使用して IRS サイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="a1527-191">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="a1527-192">会社の詳細のみを入力してください。</span><span class="sxs-lookup"><span data-stu-id="a1527-192">Enter only details for your company.</span></span> <span data-ttu-id="a1527-193">個人情報を入力しないでください。</span><span class="sxs-lookup"><span data-stu-id="a1527-193">Never enter personal details.</span></span>

1. <span data-ttu-id="a1527-194">[ **ビジネスプロファイル** ] ページで、必須フィールドに入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-194">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="a1527-195">[ **セットアップ** ] ページで、会社に適用するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-195">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="a1527-196">会社が米国に組み込まれている場合、またはこのプロファイルが個人向けの場合は、左側のオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-196">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="a1527-197">会社が米国の外部に組み込まれている場合は、右側のオプションを選択し、一覧から国/地域を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-197">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="a1527-198">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-198">Select **Next**.</span></span> 

4. <span data-ttu-id="a1527-199">[ **納税の状態** ] ページで必要な情報を入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-199">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="a1527-200">このページのフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="a1527-200">Fields on this page will vary by country.</span></span> <span data-ttu-id="a1527-201">詳細。</span><span class="sxs-lookup"><span data-stu-id="a1527-201">your details.</span></span> 

5. <span data-ttu-id="a1527-202">[ **追加のドキュメント** ] ページの [必須フィールド] をクリックし、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-202">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="a1527-203">[ **参照** ] を選択して、お住まいの国または地域で必要なドキュメントをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="a1527-203">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="a1527-204">ドキュメント名が表示されたら、[ **アップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-204">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="a1527-205">ドキュメントを削除する必要がある場合は、[ **削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-205">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="a1527-206">保存して続行するには、[ **完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-206">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="a1527-207">ポップアップメッセージで [ **確認** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a1527-207">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="a1527-208">[ **支払いと税金の設定** ] ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="a1527-208">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a1527-209">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a1527-209">Next steps</span></span>

- [<span data-ttu-id="a1527-210">インセンティブの支払いと税金のプロファイルに関する FAQ</span><span class="sxs-lookup"><span data-stu-id="a1527-210">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
