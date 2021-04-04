---
title: パートナー センターでの支払いプロファイルと税務プロファイル
ms.topic: how-to
ms.date: 02/24/2021
description: 支払いと税金のプロファイルを作成および管理して、インセンティブの作業に対して支払うことができます。 さまざまなプロファイルの作成、管理、および使用が含まれます。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 5079649746d673ea4dee40264afe4ea61671a9a2
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179532"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="c236e-104">パートナーセンターでインセンティブの支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="c236e-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="c236e-105">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="c236e-105">**Appropriate roles**</span></span>

- <span data-ttu-id="c236e-106">インセンティブ管理者</span><span class="sxs-lookup"><span data-stu-id="c236e-106">Incentives admin</span></span>
- <span data-ttu-id="c236e-107">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="c236e-107">Account admin</span></span>
- <span data-ttu-id="c236e-108">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="c236e-108">Global admin</span></span>

<span data-ttu-id="c236e-109">特定の MPN の場所についてインセンティブ プログラムの支払いを受けるには、有効な支払いおよび税務プロファイルを、プログラムおよび MPN の場所に事前に関連付けて、登録を完了しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="c236e-110">支払いの発行には、この支払いおよび税務プロファイルが使用されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="c236e-111">インセンティブ プログラムのルールによっては、支払いに対して銀行の電子送信やクレジット ノートを使用できる場合があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="c236e-112">役割、通貨、およびその他の Microsoft プログラム</span><span class="sxs-lookup"><span data-stu-id="c236e-112">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="c236e-113">支払いと税金のプロファイルを開始する前に、以下の情報を理解しておくことが重要です。</span><span class="sxs-lookup"><span data-stu-id="c236e-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="c236e-114">ロールとアクセス許可</span><span class="sxs-lookup"><span data-stu-id="c236e-114">Roles and permissions</span></span>

<span data-ttu-id="c236e-115">インセンティブ支払いのために銀行および税金の情報を入力するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="c236e-116">MPN/アカウント管理者の場合は、自分または同僚を割り当てて、インセンティブ管理者にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c236e-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="c236e-117">インセンティブ管理者のアクセス許可を要求する必要がある場合は、MPN 管理者または全体管理者にお問い合わせください。 [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインすることで、社内のユーザーがこれらのロールを持っていることを確認できます。</span><span class="sxs-lookup"><span data-stu-id="c236e-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="c236e-118">右上にある [ **設定** ] アイコンから、[ **ユーザー管理** ] を選択し、グローバル管理者に対してフィルター処理を行います。</span><span class="sxs-lookup"><span data-stu-id="c236e-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="c236e-119">インセンティブのユーザーは、インセンティブの利益および支払いの詳細とレポートを表示できますが、銀行や税金の詳細を編集することはできません。</span><span class="sxs-lookup"><span data-stu-id="c236e-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="c236e-120">出金通貨の選択</span><span class="sxs-lookup"><span data-stu-id="c236e-120">Choose your disbursement currency</span></span>

<span data-ttu-id="c236e-121">インセンティブ支払いは、支払いプロファイルの設定時に選択した通貨で行われます。</span><span class="sxs-lookup"><span data-stu-id="c236e-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="c236e-122">支払いは、Microsoft が毎月設定した換算レートを使用して計算されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="c236e-123">通貨が選択されているため、値の変更について責任があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="c236e-124">さまざまな Microsoft プログラムに異なるプロファイルを使用する</span><span class="sxs-lookup"><span data-stu-id="c236e-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="c236e-125">企業が複数のインセンティブプログラムに登録されている場合は、そのすべてに同じ支払いアカウントを使用することも、異なるプログラムに対して異なる支払いアカウントを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="c236e-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="c236e-126">パートナー センターで支払いと税金のプロファイルを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="c236e-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="c236e-127">以下のセクションでは、パートナーセンターで支払いと税金のプロファイルを作成および管理するプロセスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c236e-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="c236e-128">パートナーセンターで支払いプロファイルを作成または管理するには、インセンティブ管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-128">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="c236e-129">インセンティブの役割は、各インセンティブプログラムの下にある各 MPN の場所に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="c236e-130">パートナーセンターでインセンティブ管理者を追加する方法の詳細については、「 [ユーザーアカウントの作成](create-user-accounts-and-set-permissions.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="c236e-131">パートナーセンターの支払いと税金のセクションにアクセスする</span><span class="sxs-lookup"><span data-stu-id="c236e-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="c236e-132">Azure Active Directory (Azure AD) アカウント (会社のアカウント) を使用して [パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/) にサインインします。または、該当する電子メールアドレスが割り当てられている場合は、適切な電子メールアドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="c236e-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="c236e-133">1つの Azure AD アカウント内に複数のドメインを登録できます。</span><span class="sxs-lookup"><span data-stu-id="c236e-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="c236e-134">グローバル管理者に連絡して、どのドメインが関連付けられているかを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="c236e-135">ドメインでのみログインできる場合は、 @onmicrosoft.com アカウント管理者に連絡して、Azure AD アカウントにドメインを追加してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-135">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="c236e-136">**職場または学校** のアカウントまたは **個人のアカウント** を選択するように求められたら、[**職場または学校アカウント**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="c236e-137">歯車アイコンを選択して [ **設定** ] メニューを開き、[ **アカウント設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="c236e-138">[ **アカウント設定** ] メニューで、[ **支払いと税金**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-138">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="c236e-139">個々のプログラムに支払いと税金のプロファイルを割り当てる</span><span class="sxs-lookup"><span data-stu-id="c236e-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="c236e-140">[パートナーセンターのダッシュボード](https://partner.microsoft.com/dashboard/)にサインインし、歯車アイコンを選択して [**設定**] メニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="c236e-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="c236e-141">[ **アカウントの設定**] を選択し、[ **支払いと税金] セクション** を展開して、[ **支払いと税金のプロファイルの割り当て**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="c236e-142">プログラムの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="c236e-143">プログラムの横にある矢印を選択すると、プロファイルの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="c236e-144">[ **税プロファイル** ] ドロップダウンメニューで、必要な税プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="c236e-145">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="c236e-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="c236e-146">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-146">Select Continue in the pop-up window.</span></span> <span data-ttu-id="c236e-147">新しい税プロファイルを作成するプロセスについては、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-147">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="c236e-148">**支払い方法** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="c236e-149">支払い方法として [ **電子銀行の転送** ] を選択した場合は、目的の支払プロファイルを選択するか、新しいプロファイルを作成するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="c236e-150">新しいプロファイルを作成するオプションを選択すると、適切にリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="c236e-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="c236e-151">ポップアップウィンドウで [続行] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="c236e-152">新しい支払いプロファイルを作成するプロセスを次に示します。</span><span class="sxs-lookup"><span data-stu-id="c236e-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="c236e-153">支払い方法として **クレジットメモ** を選択した場合は、検証を完了します。</span><span class="sxs-lookup"><span data-stu-id="c236e-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="c236e-154">これにより、参照されている SAP 番号が組織に属していることが確認されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c236e-155">複数の Microsoft ビジネスエンティティが一覧表示されている場合は、各エンティティの支払いプロファイルを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="c236e-156">支払い方法の可用性は、インセンティブプログラムのルールに依存します。</span><span class="sxs-lookup"><span data-stu-id="c236e-156">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="c236e-157">場所の MPN ID が特定のインセンティブプログラムのローカルの Microsoft 子会社によって支払われ、LRD (制限されたリスクディストリビューター) クレジットメモが支払い方法として許可されている場合、支払いプロファイルには LRD クレジットメモの支払い方法が事前に設定されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-157">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="c236e-158">各インセンティブプログラムと location MPN ID の LRD クレジットメモ支払方法の行で、[支払いプロファイル] セクションの状態として [ **確認** ] または [ **確認が必要** ] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-158">On the LRD credit note payment method row for the respective incentive program and location MPN ID you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="c236e-159">場所 MPN および支払い方法に関連付けられている CSP テナント ID の詳細を確認して確認するために **必要な** 確認を選択し、クレジットメモの支払いを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="c236e-159">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="c236e-160">[ **クレジットメモの詳細** ] ダイアログボックスで、指定された CSP テナント ID と詳細が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c236e-160">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="c236e-161">複数のテナント ID が表示される場合は、支払いを受け取る CSP テナント ID を慎重に選択してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-161">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="c236e-162">次に、[確認] を選択して会社の詳細が正しいことと、選択した CSP テナント ID に対してインセンティブ支払いを行う必要があることを **確認** します。</span><span class="sxs-lookup"><span data-stu-id="c236e-162">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="c236e-163">状態が [ **確認** 済み] になっている場合は、CSP テナント ID の割り当てが完了しているため、これ以上の操作は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="c236e-163">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="c236e-164">[確認] を選択して、割り当ての詳細を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="c236e-164">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="c236e-165">課税控除を適用するためにパートナーに明示的に要求する必要がある国では、インセンティブプログラムと場所 MPN の税プロファイルセクションの税プロファイルの横に課税控除を適用するオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="c236e-165">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="c236e-166">このチェックボックスをオンにすると、インセンティブクレジットメモに免税の特典が適用されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-166">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="c236e-167">現在、この支払い方法は、Microsoft コマースインセンティブプログラムのオーストラリア、ニュージーランド、およびカナダのパートナーに対してのみご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="c236e-167">Currently, this payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="c236e-168">この3つの国で、MCI プログラムに登録されているダイレクト請求パートナーまたは間接プロバイダーの場合、使用可能な支払い方法として LRD クレジットメモが表示されない場合は、テナント ID が関連する partner MPN location アカウントに関連付けられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-168">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="c236e-169">詳細については [、「組織のプロファイルを更新する方法](update-your-partner-profile.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-169">For more information on this read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="c236e-170">**通貨** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-170">Select the **Currency**.</span></span>

6. <span data-ttu-id="c236e-171">すべての支払いフィールドを完了したら、[ **送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-171">When you’ve completed all of the payment fields, select **Submit**.</span></span>


## <a name="create-your-bank-profile"></a><span data-ttu-id="c236e-172">銀行のプロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="c236e-172">Create your bank profile</span></span>

<span data-ttu-id="c236e-173">銀行のプロファイルは、組織レベルで作成されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-173">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="c236e-174">これにより、組織内の複数の MPN ID およびインセンティブプログラムに対して1つの銀行プロファイルを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="c236e-174">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="c236e-175">異なる銀行や税金のルールが適用される可能性があるため、銀行のプロファイルを異なる国に適用するときに例外が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="c236e-175">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="c236e-176">次のページでは、アスタリスクの付いたフィールドが必要です。</span><span class="sxs-lookup"><span data-stu-id="c236e-176">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="c236e-177">フィールドの内容がわからない場合は、情報アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-177">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="c236e-178">[ **詳細** ] ページで、次のフィールドを入力します。 [ **プロファイル名]:** この支払いプロファイルを識別する一意の名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="c236e-178">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="c236e-179">**銀行口座の場所:** 会社の銀行がある国。</span><span class="sxs-lookup"><span data-stu-id="c236e-179">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="c236e-180">**支払い方法:** パートナーセンターのお支払い方法として、電子銀行の譲渡をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c236e-180">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="c236e-181">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-181">Select **Next**.</span></span>

3. <span data-ttu-id="c236e-182">[ **銀行口座** ] ページで、情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c236e-182">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="c236e-183">このページに表示されるフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="c236e-183">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="c236e-184">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-184">Select **Next**.</span></span>

5. <span data-ttu-id="c236e-185">[ **受益者** ] ページで、適切な情報を入力します。</span><span class="sxs-lookup"><span data-stu-id="c236e-185">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="c236e-186">受益者は、お客様がアカウントについて話し合う必要がある場合に、銀行が連絡する会社の人物です。</span><span class="sxs-lookup"><span data-stu-id="c236e-186">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="c236e-187">フィールドが完了したら、[ **完了**] を選択し、[ **確認** ] を選択して、銀行プロファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="c236e-187">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="c236e-188">[ **支払いと税金のプロファイル** ] ページにリダイレクトされます。</span><span class="sxs-lookup"><span data-stu-id="c236e-188">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="c236e-189">新しいプロファイルの状態には、検証が完了するまで、 **保留中の Microsoft 検証** が反映されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-189">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="c236e-190">このプロセスには最大48時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="c236e-190">This process may take up to 48 hours.</span></span> <span data-ttu-id="c236e-191">検証が完了すると、プロファイルの状態には、 **承認済み** または **操作** が反映されます。</span><span class="sxs-lookup"><span data-stu-id="c236e-191">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="c236e-192">**操作が必要な** 場合は、上記の手順を繰り返して必要な情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="c236e-192">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="c236e-193">税務プロファイルを作成する</span><span class="sxs-lookup"><span data-stu-id="c236e-193">Create your tax profile</span></span>

<span data-ttu-id="c236e-194">次の手順を使用して、組織に必要な税金情報を Microsoft に提供します。</span><span class="sxs-lookup"><span data-stu-id="c236e-194">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="c236e-195">このセクションのページは動的であり、お住まいの国または地域によって異なります。</span><span class="sxs-lookup"><span data-stu-id="c236e-195">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="c236e-196">正しい税金情報を特定するためのヘルプが必要な場合は、お住まいの国の適切な政府機関にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="c236e-196">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="c236e-197">南北アメリカのパートナー企業の場合、W8 または W9 フォームの完了に関する情報が必要な場合は、次のアドレスを使用して IRS サイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="c236e-197">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="c236e-198">会社の詳細のみを入力してください。</span><span class="sxs-lookup"><span data-stu-id="c236e-198">Enter only details for your company.</span></span> <span data-ttu-id="c236e-199">個人情報を入力しないでください。</span><span class="sxs-lookup"><span data-stu-id="c236e-199">Never enter personal details.</span></span>

1. <span data-ttu-id="c236e-200">[ **ビジネスプロファイル** ] ページで、必須フィールドに入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-200">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="c236e-201">[ **セットアップ** ] ページで、会社に適用するオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-201">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="c236e-202">会社が米国に組み込まれている場合、またはこのプロファイルが個人向けの場合は、左側のオプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-202">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="c236e-203">会社が米国の外部に組み込まれている場合は、右側のオプションを選択し、一覧から国/地域を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-203">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="c236e-204">**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-204">Select **Next**.</span></span> 

4. <span data-ttu-id="c236e-205">[ **納税の状態** ] ページで必要な情報を入力し、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-205">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="c236e-206">このページのフィールドは、国によって異なります。</span><span class="sxs-lookup"><span data-stu-id="c236e-206">Fields on this page will vary by country.</span></span> <span data-ttu-id="c236e-207">詳細。</span><span class="sxs-lookup"><span data-stu-id="c236e-207">your details.</span></span> 

5. <span data-ttu-id="c236e-208">[ **追加のドキュメント** ] ページの [必須フィールド] をクリックし、[ **次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-208">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="c236e-209">[ **参照** ] を選択して、お住まいの国または地域で必要なドキュメントをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="c236e-209">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="c236e-210">ドキュメント名が表示されたら、[ **アップロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-210">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="c236e-211">ドキュメントを削除する必要がある場合は、[ **削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-211">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="c236e-212">保存して続行するには、[ **完了**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-212">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="c236e-213">ポップアップメッセージで [ **確認** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c236e-213">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="c236e-214">[ **支払いと税金の設定** ] ページに戻ります。</span><span class="sxs-lookup"><span data-stu-id="c236e-214">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c236e-215">次のステップ</span><span class="sxs-lookup"><span data-stu-id="c236e-215">Next steps</span></span>

- [<span data-ttu-id="c236e-216">支払いと税金に関してよく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="c236e-216">Common questions about payouts and taxes</span></span>](payout-faq.md)
