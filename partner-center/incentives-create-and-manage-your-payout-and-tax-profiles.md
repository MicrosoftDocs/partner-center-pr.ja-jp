---
title: パートナー センターでの支払いプロファイルと税務プロファイル
ms.topic: how-to
ms.date: 04/15/2021
description: 支払いと税金のプロファイルを作成および管理して、インセンティブの作業に対して支払うことができます。 さまざまなプロファイルの作成、管理、および使用が含まれます。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 4a931f1d971ea3e3bc288f70e85a6600596761cc
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528543"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="52d84-104">パートナーセンターでインセンティブの支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="52d84-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="52d84-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="52d84-105">**Appropriate roles**</span></span>

- <span data-ttu-id="52d84-106">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="52d84-106">Incentives admin</span></span>
- <span data-ttu-id="52d84-107">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="52d84-107">Account admin</span></span>
- <span data-ttu-id="52d84-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="52d84-108">Global admin</span></span>

<span data-ttu-id="52d84-109">特定の MPN の場所についてインセンティブ プログラムの支払いを受けるには、有効な支払いおよび税務プロファイルを、プログラムおよび MPN の場所に事前に関連付けて、登録を完了しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="52d84-110">支払いの発行には、この支払いおよび税務プロファイルが使用されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="52d84-111">インセンティブ プログラムのルールによっては、支払いに対して銀行の電子送信やクレジット ノートを使用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a><span data-ttu-id="52d84-112">役割、通貨、および複数の Microsoft インセンティブプログラム</span><span class="sxs-lookup"><span data-stu-id="52d84-112">Roles, currencies, and multiple Microsoft incentive programs</span></span>

<span data-ttu-id="52d84-113">支払いと税金のプロファイルを開始する前に、以下の情報を理解しておくことが重要です。</span><span class="sxs-lookup"><span data-stu-id="52d84-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="52d84-114">ロールとアクセス許可</span><span class="sxs-lookup"><span data-stu-id="52d84-114">Roles and permissions</span></span>

<span data-ttu-id="52d84-115">インセンティブ支払いのために銀行および税金の情報を入力するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="52d84-116">MPN/アカウント管理者の場合は、自分または同僚を割り当てて、インセンティブ管理者にすることができます。</span><span class="sxs-lookup"><span data-stu-id="52d84-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="52d84-117">インセンティブ管理者のアクセス許可を要求する必要がある場合は、MPN 管理者または全体管理者にお問い合わせください。 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインすることで、社内のユーザーがこれらのロールを持っていることを確認できます。</span><span class="sxs-lookup"><span data-stu-id="52d84-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="52d84-118">右上にある [ **設定** ] アイコンから、[ **ユーザー管理** ] を選択し、グローバル管理者に対してフィルター処理を行います。</span><span class="sxs-lookup"><span data-stu-id="52d84-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="52d84-119">インセンティブのユーザーは、インセンティブの利益および支払いの詳細とレポートを表示できますが、銀行や税金の詳細を編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="52d84-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="52d84-120">出金通貨の選択</span><span class="sxs-lookup"><span data-stu-id="52d84-120">Choose your disbursement currency</span></span>

<span data-ttu-id="52d84-121">インセンティブ支払いは、支払いプロファイルの設定時に選択した通貨で行われます。</span><span class="sxs-lookup"><span data-stu-id="52d84-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="52d84-122">支払いは、Microsoft が毎月設定した換算レートを使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="52d84-123">通貨が選択されているため、値の変更について責任があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="52d84-124">さまざまな Microsoft プログラムに異なるプロファイルを使用する</span><span class="sxs-lookup"><span data-stu-id="52d84-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="52d84-125">企業が複数のインセンティブプログラムに登録されている場合は、そのすべてに同じ支払いアカウントを使用することも、異なるプログラムに対して異なる支払いアカウントを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="52d84-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="52d84-126">パートナー センターで支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="52d84-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="52d84-127">以下のセクションでは、パートナーセンターで支払いと税金のプロファイルを作成および管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="52d84-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="52d84-128">パートナーセンターで支払いと税金のプロファイルを作成または管理するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-128">You must be an Incentive admin to create or manage payment and tax profiles in Partner Center.</span></span> <span data-ttu-id="52d84-129">インセンティブの役割は、各インセンティブプログラムの下にある各 MPN の場所に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="52d84-130">パートナーセンターでインセンティブ管理者を追加する方法の詳細については、「 [ユーザーアカウントの作成](create-user-accounts-and-set-permissions.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="52d84-131">パートナーセンターの支払いと税金のセクションにアクセスする</span><span class="sxs-lookup"><span data-stu-id="52d84-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="52d84-132">Azure Active Directory (Azure AD) アカウント (会社のアカウント) を使用して [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインします。または、該当する電子メールアドレスが割り当てられている場合は、適切な電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="52d84-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="52d84-133">1つの Azure AD アカウント内に複数のドメインを登録できます。</span><span class="sxs-lookup"><span data-stu-id="52d84-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="52d84-134">グローバル管理者に連絡して、どのドメインが関連付けられているかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="52d84-135">ドメインでサインインでき、 @onmicrosoft.com 追加のドメインが必要な場合は、アカウント管理者に連絡して、Azure AD アカウントにドメインを追加してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-135">If you're only able to sign in with the @onmicrosoft.com domain and you need additional domains, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="52d84-136">**職場または学校** のアカウントまたは **個人のアカウント** を選択するように求められたら、[**職場または学校アカウント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="52d84-137">歯車アイコンを選択して [ **設定** ] メニューを開き、[ **アカウント設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="52d84-138">[ **アカウント設定** ] メニューで、[ **支払いと税金**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-138">In the **Account settings** menu, select **Payout and tax**.</span></span>

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="52d84-139">個々のプログラムに支払いと税金のプロファイルを割り当てる</span><span class="sxs-lookup"><span data-stu-id="52d84-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="52d84-140">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、歯車アイコンを選択して [**設定**] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="52d84-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="52d84-141">[ **アカウントの設定**] を選択し、[ **支払いと税金] セクション** を展開して、[ **支払いと税金のプロファイルの割り当て**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="52d84-142">プログラムの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="52d84-143">プログラムの横にある矢印を選択すると、プロファイルの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="52d84-144">[ **税プロファイル** ] ドロップダウンメニューで、必要な税プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="52d84-145">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="52d84-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="52d84-146">ポップアップウィンドウで [ **続行** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-146">Select **Continue** in the pop-up window.</span></span> <span data-ttu-id="52d84-147">新しい税プロファイルを作成するプロセスを次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d84-147">The process for creating a new tax profile is provided below.</span></span>

4. <span data-ttu-id="52d84-148">**支払い方法** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="52d84-149">支払い方法として [ **電子銀行の転送** ] を選択した場合は、目的の支払プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="52d84-150">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="52d84-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="52d84-151">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="52d84-152">新しい支払いプロファイルを作成するプロセスを次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d84-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="52d84-153">支払い方法として **クレジットメモ** を選択した場合は、検証を完了します。</span><span class="sxs-lookup"><span data-stu-id="52d84-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="52d84-154">これにより、参照されている SAP 番号が組織に属していることが確認されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="52d84-155">複数の Microsoft ビジネスエンティティが一覧表示されている場合は、各エンティティの支払いプロファイルを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="52d84-156">支払い方法の可用性は、インセンティブプログラムのルールに依存します。</span><span class="sxs-lookup"><span data-stu-id="52d84-156">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="52d84-157">場所の MPN ID が特定のインセンティブプログラムのローカルの Microsoft 子会社によって支払われ、LRD (制限されたリスクディストリビューター) クレジットメモが支払い方法として許可されている場合、支払いプロファイルには LRD クレジットメモの支払い方法が事前に設定されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-157">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="52d84-158">各インセンティブプログラムと location MPN ID の LRD クレジットメモ支払方法の行で、[支払いプロファイル] セクションの状態として [ **確認** ] または [ **確認が必要** ] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-158">On the LRD credit note payment method row for the respective incentive program and location MPN ID you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="52d84-159">場所 MPN および支払い方法に関連付けられている CSP テナント ID の詳細を確認して確認するために **必要な** 確認を選択し、クレジットメモの支払いを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="52d84-159">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="52d84-160">[ **クレジットメモの詳細** ] ダイアログボックスで、指定された CSP テナント ID と詳細が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="52d84-160">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="52d84-161">複数のテナント ID が表示される場合は、支払いを受け取る CSP テナント ID を慎重に選択してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-161">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="52d84-162">次に、[確認] を選択して会社の詳細が正しいことと、選択した CSP テナント ID に対してインセンティブ支払いを行う必要があることを **確認** します。</span><span class="sxs-lookup"><span data-stu-id="52d84-162">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="52d84-163">状態が [ **確認** 済み] になっている場合は、CSP テナント ID の割り当てが完了しているため、これ以上の操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="52d84-163">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="52d84-164">[確認] を選択して、割り当ての詳細を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="52d84-164">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="52d84-165">課税控除を適用するためにパートナーに明示的に要求する必要がある国では、インセンティブプログラムと場所 MPN の税プロファイルセクションの税プロファイルの横に課税控除を適用するオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="52d84-165">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="52d84-166">このチェックボックスをオンにすると、インセンティブクレジットメモに免税の特典が適用されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-166">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="52d84-167">現在、LRD クレジットの支払い方法は、Microsoft コマースインセンティブプログラムのオーストラリア、ニュージーランド、およびカナダのパートナーに対してのみご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="52d84-167">Currently, the LRD Credit Note payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="52d84-168">この3つの国で、MCI プログラムに登録されているダイレクト請求パートナーまたは間接プロバイダーの場合、使用可能な支払い方法として LRD クレジットメモが表示されない場合は、テナント ID が関連する partner MPN location アカウントに関連付けられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-168">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="52d84-169">詳細については [、「組織のプロファイルを更新する方法](update-your-partner-profile.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-169">For more information on this read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="52d84-170">**通貨** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-170">Select the **Currency**.</span></span>

6. <span data-ttu-id="52d84-171">すべての支払いフィールドを完了したら、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-171">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="set-up-a-default-bank-profile"></a><span data-ttu-id="52d84-172">既定の銀行プロファイルを設定する</span><span class="sxs-lookup"><span data-stu-id="52d84-172">Set up a default bank profile</span></span>

<span data-ttu-id="52d84-173">既定の銀行プロファイルを設定し、MPN の場所に割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="52d84-173">You can setup default bank profiles and assign them to MPN locations.</span></span> <span data-ttu-id="52d84-174">これらの既定のプロファイルは、その MPN の場所の後続の登録に Microsoft によって使用されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-174">These defaults profiles will be used by Microsoft for subsequent enrollments for that MPN location.</span></span> 

1. <span data-ttu-id="52d84-175">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、歯車アイコンを選択して [ **設定**   ] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="52d84-175">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/),  and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="52d84-176">[ **アカウント設定**] を選択し、[ **支払いと税金** ] セクションを展開して、[ **支払いと税金のプロファイル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-176">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profiles**.</span></span> 

3. <span data-ttu-id="52d84-177">[**支払いプロファイル**] セクションで、[**既定のプロファイルを管理** する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-177">Select **Manage default profiles** under the **Payment profiles** section.</span></span> 

4. <span data-ttu-id="52d84-178">既定の銀行プロファイルを作成するには **、[既定の銀行プロファイルを追加** する] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-178">To create a default bank profiles select **Add a default bank profile**.</span></span> 

5. <span data-ttu-id="52d84-179">会社の利用可能な銀行プロファイルの一覧から銀行プロファイルを選択し、この銀行プロファイルで使用する通貨を選択して、この既定のプロファイルを適用する MPN の場所の一覧を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-179">Select a bank profile from the list of available bank profiles of your company, select the currency to be used with this bank profile, and then select the list of MPN locations for which you want this default profile to apply.</span></span>

6. <span data-ttu-id="52d84-180">選択が完了したら、[ **完了** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-180">Select **Done** once you have completed the selections.</span></span> <span data-ttu-id="52d84-181">必須フィールドがすべて完了するまで、[完了] ボタンはクリックできません。</span><span class="sxs-lookup"><span data-stu-id="52d84-181">The Done button will not be clickable until all required fields have been completed.</span></span> 

>[!NOTE]
><span data-ttu-id="52d84-182">同じ銀行および通貨のペアリングを複数の場所に適用できます。</span><span class="sxs-lookup"><span data-stu-id="52d84-182">The same bank and currency pairing can be applied to multiple locations.</span></span> <span data-ttu-id="52d84-183">場所 MPN に1回既定のプロファイルと通貨の組み合わせが割り当てられている場合は、今後の既定のプロファイルの割り当ての [場所] ドロップダウンに表示されなくなります。</span><span class="sxs-lookup"><span data-stu-id="52d84-183">If the location MPN has been assigned a default profile and currency combination once, it will no longer appear in the location dropdown for future default profile assignments.</span></span> <span data-ttu-id="52d84-184">既定の選択が削除された場合、その後の既定のプロファイルの割り当てについては、場所 MPN が再表示されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-184">If the default selection is deleted, the location MPN will reappear for future default profile assignments.</span></span> <span data-ttu-id="52d84-185">各銀行のプロファイルと通貨の組み合わせは、一意の編集可能な行として追加されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-185">Each bank profile and currency combination is added as an unique, editable row.</span></span>

7. <span data-ttu-id="52d84-186">必要な変更がすべて追加されたら、[ **保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-186">Once all the required changes have been added, select **Save**.</span></span>  

## <a name="create-your-bank-profile"></a><span data-ttu-id="52d84-187">銀行のプロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="52d84-187">Create your bank profile</span></span>

<span data-ttu-id="52d84-188">銀行のプロファイルは、会社レベルで作成されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-188">Bank profiles are created at an company level.</span></span> <span data-ttu-id="52d84-189">これにより、企業内の複数の MPN ID およびインセンティブプログラムに対して1つの銀行プロファイルを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="52d84-189">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within a company.</span></span> <span data-ttu-id="52d84-190">異なる銀行や税金のルールが適用される可能性があるため、銀行のプロファイルを異なる国に適用するときに例外が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="52d84-190">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="52d84-191">次のページでは、アスタリスクの付いたフィールドが必要です。</span><span class="sxs-lookup"><span data-stu-id="52d84-191">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="52d84-192">フィールドの内容がわからない場合は、情報アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-192">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="52d84-193">[ **詳細** ] ページで、次のフィールドを入力します。 [ **プロファイル名]:** この支払いプロファイルを識別する一意の名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="52d84-193">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="52d84-194">**銀行口座の場所:** 会社の銀行がある国。</span><span class="sxs-lookup"><span data-stu-id="52d84-194">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="52d84-195">**支払い方法:** パートナーセンターのお支払い方法として、電子銀行の譲渡をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="52d84-195">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="52d84-196">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-196">Select **Next**.</span></span>

3. <span data-ttu-id="52d84-197">[ **銀行口座** ] ページで、情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="52d84-197">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="52d84-198">このページに表示されるフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="52d84-198">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="52d84-199">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-199">Select **Next**.</span></span>

5. <span data-ttu-id="52d84-200">[ **受益者** ] ページで、適切な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="52d84-200">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="52d84-201">受益者は、お客様がアカウントについて話し合う必要がある場合に、銀行が連絡する会社の人物です。</span><span class="sxs-lookup"><span data-stu-id="52d84-201">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="52d84-202">フィールドが完了したら、[ **完了**] を選択し、[ **確認** ] を選択して、銀行プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="52d84-202">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="52d84-203">[ **支払いと税金のプロファイル** ] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="52d84-203">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="52d84-204">新しいプロファイルの状態には、検証が完了するまで、 **保留中の Microsoft 検証** が反映されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-204">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="52d84-205">このプロセスには最大48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="52d84-205">This process may take up to 48 hours.</span></span> <span data-ttu-id="52d84-206">検証が完了すると、プロファイルの状態には、 **承認済み** または **操作** が反映されます。</span><span class="sxs-lookup"><span data-stu-id="52d84-206">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="52d84-207">**操作が必要な** 場合は、上記の手順を繰り返して必要な情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="52d84-207">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="52d84-208">税務プロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="52d84-208">Create your tax profile</span></span>

<span data-ttu-id="52d84-209">次の手順を使用して、組織に必要な税金情報を Microsoft に提供します。</span><span class="sxs-lookup"><span data-stu-id="52d84-209">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="52d84-210">このセクションのページは動的であり、お住まいの国または地域によって異なります。</span><span class="sxs-lookup"><span data-stu-id="52d84-210">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="52d84-211">正しい税金情報を特定するためのヘルプが必要な場合は、お住まいの国の適切な政府機関にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="52d84-211">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="52d84-212">南北アメリカのパートナー企業の場合、W8 または W9 フォームの完了に関する情報が必要な場合は、次のアドレスを使用して IRS サイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="52d84-212">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="52d84-213">会社の詳細のみを入力してください。</span><span class="sxs-lookup"><span data-stu-id="52d84-213">Enter only details for your company.</span></span> <span data-ttu-id="52d84-214">個人情報を入力しないでください。</span><span class="sxs-lookup"><span data-stu-id="52d84-214">Never enter personal details.</span></span>

1. <span data-ttu-id="52d84-215">[ **ビジネスプロファイル** ] ページで、必須フィールドに入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-215">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="52d84-216">[ **セットアップ** ] ページで、会社に適用するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-216">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="52d84-217">会社が米国に組み込まれている場合、またはこのプロファイルが個人向けの場合は、左側のオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-217">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="52d84-218">会社が米国の外部に組み込まれている場合は、右側のオプションを選択し、一覧から国/地域を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-218">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="52d84-219">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-219">Select **Next**.</span></span> 

4. <span data-ttu-id="52d84-220">[ **納税の状態** ] ページで必要な情報を入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-220">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="52d84-221">このページのフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="52d84-221">Fields on this page will vary by country.</span></span> <span data-ttu-id="52d84-222">詳細。</span><span class="sxs-lookup"><span data-stu-id="52d84-222">your details.</span></span> 

5. <span data-ttu-id="52d84-223">[ **追加のドキュメント** ] ページの [必須フィールド] をクリックし、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-223">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="52d84-224">[ **参照** ] を選択して、お住まいの国または地域で必要なドキュメントをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="52d84-224">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="52d84-225">ドキュメント名が表示されたら、[ **アップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-225">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="52d84-226">ドキュメントを削除する必要がある場合は、[ **削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-226">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="52d84-227">保存して続行するには、[ **完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-227">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="52d84-228">ポップアップメッセージで [ **確認** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-228">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="52d84-229">[ **支払いと税金の設定** ] ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="52d84-229">You’ll be taken back to the **Payout and tax setup** page.</span></span>
 
## <a name="update-expired-tax-profiles"></a><span data-ttu-id="52d84-230">期限切れの税プロファイルの更新</span><span class="sxs-lookup"><span data-stu-id="52d84-230">Update expired tax profiles</span></span>

1. <span data-ttu-id="52d84-231">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、歯車アイコンを選択して [**設定**] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="52d84-231">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span>

1. <span data-ttu-id="52d84-232">[ **アカウントの設定**] を選択し、[ **支払いと税金** ] セクションを展開して、[ **支払いと税金のプロファイル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-232">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profile**.</span></span>

1. <span data-ttu-id="52d84-233">[ **税プロファイル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-233">Select **Tax profile**.</span></span>

1. <span data-ttu-id="52d84-234">列の **有効期限** を確認し、有効期限が切れたか、期限切れになる税金プロファイルに移動します。</span><span class="sxs-lookup"><span data-stu-id="52d84-234">Check the column **Expiration Date** and navigate to the tax profile that is expired or about to expire.</span></span>

1. <span data-ttu-id="52d84-235">**[編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="52d84-235">Select **Edit**.</span></span>

1. <span data-ttu-id="52d84-236">[税フォーム] セクションで、新しい詳細を入力して、税フォームを更新します。</span><span class="sxs-lookup"><span data-stu-id="52d84-236">In the tax form section, update the tax forms by providing the new details.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="52d84-237">次のステップ</span><span class="sxs-lookup"><span data-stu-id="52d84-237">Next steps</span></span>

- [<span data-ttu-id="52d84-238">支払いと税金に関してよく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="52d84-238">Common questions about payouts and taxes</span></span>](payout-faq.md)
