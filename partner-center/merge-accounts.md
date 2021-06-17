---
title: パートナー アカウントを別のパートナー アカウントにマージする
description: パートナーアカウントをパートナーセンターの別のパートナーアカウントにマージする方法について説明します。パートナーセンターで、Microsoft パートナーがアクティブである場合に使用します。
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: bcef4c771d748b0e2fbeae8cf1daaf41d7f53b43
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276639"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="9a052-103">パートナー アカウントを別のパートナー アカウントにマージする</span><span class="sxs-lookup"><span data-stu-id="9a052-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="9a052-104">**適切なロール**: アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="9a052-104">**Appropriate roles**: Account admin</span></span>

<span data-ttu-id="9a052-105">複数の企業がアクティブな Microsoft パートナーであり、パートナーセンターにアカウントを持っている場合、それらのアカウントをマージすることができます。</span><span class="sxs-lookup"><span data-stu-id="9a052-105">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="9a052-106">2つのパートナーがパートナーセンターのアカウントをマージすることを選択した場合の動作</span><span class="sxs-lookup"><span data-stu-id="9a052-106">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="9a052-107">マージを開始するパートナー組織は、パートナーグローバルアカウント (PGA) になります。</span><span class="sxs-lookup"><span data-stu-id="9a052-107">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="9a052-108">招待された組織の PGA が、発信元企業の場所になります。</span><span class="sxs-lookup"><span data-stu-id="9a052-108">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="9a052-109">マージするアカウントのすべての場所は、PGA の下の場所になります。</span><span class="sxs-lookup"><span data-stu-id="9a052-109">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="9a052-110">アカウントの合併が完了すると、PGA プロファイル内の場所やユーザーなど、両方のアカウントの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-110">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="9a052-111">このプロセスを元に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="9a052-111">You can't reverse this process.</span></span>

- <span data-ttu-id="9a052-112">この統合中に、場所のすべての MPN Id が保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-112">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="9a052-113">ユーザーのロールが引き継がれます。</span><span class="sxs-lookup"><span data-stu-id="9a052-113">User's roles are brought over.</span></span> <span data-ttu-id="9a052-114">たとえば、特定の場所のインセンティブ管理者であるユーザーは、合併後もそのロールを持ち、合併前に見たインセンティブを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="9a052-114">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="9a052-115">Azure AD テナントと CSP アカウントはマージされず、影響もありません。</span><span class="sxs-lookup"><span data-stu-id="9a052-115">Azure AD tenants and CSP accounts are not merged and have no effect.</span></span>

- <span data-ttu-id="9a052-116">両方の会社に関連付けられている公開済みプランと共同販売パイプラインデータは保持されます</span><span class="sxs-lookup"><span data-stu-id="9a052-116">Published offers and Co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="9a052-117">マージされたアカウントの表示</span><span class="sxs-lookup"><span data-stu-id="9a052-117">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="アカウントの合併。":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="9a052-119">パートナーセンターアカウントを別のパートナーセンターアカウントにマージするように招待されている場合の対処方法</span><span class="sxs-lookup"><span data-stu-id="9a052-119">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="9a052-120">アカウントの結合への招待に同意する場合は、次のようにします。MPN ID と場所は、招待されたパートナーアカウントの PGA にマージされます。</span><span class="sxs-lookup"><span data-stu-id="9a052-120">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="9a052-121">ユーザーは、自分のロールとそのままの状態で、統合されたアカウントに移動します。</span><span class="sxs-lookup"><span data-stu-id="9a052-121">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="9a052-122">既存の特典とコンピテンシーは、合併後に更新されるまで、両方の企業において保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-122">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="9a052-123">更新時、アカウントは1つの会社として扱われ、標準の更新規則が適用されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-123">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="9a052-124">パートナーがアカウントを結合する場合のプログラムと利点への影響について理解する</span><span class="sxs-lookup"><span data-stu-id="9a052-124">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="9a052-125">すべての既存のコンピテンシー (Gold/シルバー)、購入 (Microsoft Action Pack など)、および関連する特典は、統合時に保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-125">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="9a052-126">両方の企業が同じコンピテンシーを持ち、もう1つはゴールドで、もう1つはゴールドの場合、最高レベルのスキルを持つコンピテンシーが獲得され、パートナーは次の更新まで、そのコンピテンシーに対して1つのシルバー特典とゴールド特典のセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="9a052-126">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="9a052-127">Microsoft Action Pack の最高の記念日は、合併後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-127">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="9a052-128">たとえば、会社1の記念日が Action Pack 更新の場合は6月2020、会社2の Action Pack 更新の記念日が2020年10月である場合、Microsoft では、マージされた会社の新しい記念日として2020年10月日を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a052-128">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="9a052-129">アカウントの合併中、次回の更新までは、各アカウントは Action Pack やコンピテンシーの特典を保持します。</span><span class="sxs-lookup"><span data-stu-id="9a052-129">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="9a052-130">更新時には、標準 Action Pack とコンピテンシー更新ルールが適用されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-130">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="9a052-131">更新が行われると、コンピテンシーの達成と Action Pack に含まれている特典が、パートナー企業のパートナーグローバルアカウントに実装されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-131">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="9a052-132">Microsoft Action Pack: パートナー企業は、パートナーのグローバルアカウントごとに1つの Action Pack を購入できます。</span><span class="sxs-lookup"><span data-stu-id="9a052-132">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="9a052-133">コンピテンシー: パートナー企業は、最大の達成度に関連するコア特典の1つのパッケージと、パートナーがパートナーグローバルアカウントごとの資格を持つコンピテンシー固有の特典を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="9a052-133">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="9a052-134">すべてのメリットについては、 [Microsoft Partner Network 特典の使用方法](https://aka.ms/partner-benefits-use-guide)に関するガイドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a052-134">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="9a052-135">例: アクティブ化された O365 E3 トークンは、アクティブ化してから12か月間機能します。</span><span class="sxs-lookup"><span data-stu-id="9a052-135">For example: an activated O365 E3 token is functional for 12 months after activation.</span></span> <span data-ttu-id="9a052-136">トークンがテナントのライセンスに対してアクティブ化されると、そのライセンスは別のテナントに移動されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="9a052-136">Once a token has been activated for licenses on a tenant, those licenses may not be moved to another tenant.</span></span>

- <span data-ttu-id="9a052-137">両方の企業の MCP ID の関連付けが保持され、PGA MPN ID に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="9a052-137">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="9a052-138">市場投入と技術的なメリットは、コンピテンシーコア特典として提供されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-138">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="9a052-139">マージ後、銀行と税の情報を確認して正確さを確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9a052-139">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="9a052-140">会社が Azure エキスパート MSP プログラムに含まれている場合、特典は更新されるまで保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-140">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="9a052-141">会社が高度な特殊化を獲得している場合は、両方のアカウントで保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-141">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="9a052-142">ソフトウェアアシュアランスのバウチャーは、両方のアカウントにわたって保持されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-142">Any software assurance vouchers are retained across both accounts.</span></span> 

- <span data-ttu-id="9a052-143">または PAL の関連付けには影響しません。</span><span class="sxs-lookup"><span data-stu-id="9a052-143">There is no effect to DPOR or PAL association.</span></span> <span data-ttu-id="9a052-144">関連付けられた収益の投稿は、新しいパートナーグローバルアカウントへのフローを開始します。</span><span class="sxs-lookup"><span data-stu-id="9a052-144">Any associated revenue contributions will begin to flow into the new Partner Global Account</span></span>

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="9a052-145">パートナーセンターアカウントをパートナーセンターアカウントにマージするように会社を招待する</span><span class="sxs-lookup"><span data-stu-id="9a052-145">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="9a052-146">アカウントの合併を実行するには、会社の **アカウント管理者** である必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a052-146">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="9a052-147">パートナーセンターのダッシュボードから [ **設定** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a052-147">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="9a052-148">[ **Account merge**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a052-148">Select **Account merge**.</span></span>

3. <span data-ttu-id="9a052-149">自分と結合するために招待するアカウントの **パートナープロファイル** にある MPN ID を追加します。</span><span class="sxs-lookup"><span data-stu-id="9a052-149">Add the MPN ID located in the **Partner profile** of the account that you want to invite to merge with you.</span></span> <span data-ttu-id="9a052-150">パートナーのグローバル MPN ID を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a052-150">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="9a052-151">Location MPN ID を使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="9a052-151">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="9a052-152">[ **マージ**] を選択すると、パートナー企業に招待が送信されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-152">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="9a052-153">要求を受け入れると、パートナーセンター内でアカウントのマージを開始できます。</span><span class="sxs-lookup"><span data-stu-id="9a052-153">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="9a052-154">組織がアカウントのマージ要求を拒否した場合、その要求が拒否された理由を説明することができます。</span><span class="sxs-lookup"><span data-stu-id="9a052-154">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="9a052-155">[ **マージ履歴**] では、すべてのアカウントのマージの一覧を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9a052-155">A list of all your account merges is available to you under **Merge history**.</span></span>
 
### <a name="example-of-two-companies-merging-accounts"></a><span data-ttu-id="9a052-156">アカウントをマージする2つの企業の例</span><span class="sxs-lookup"><span data-stu-id="9a052-156">Example of two companies merging accounts</span></span>

1. <span data-ttu-id="9a052-157">Contoso, Ltd.</span><span class="sxs-lookup"><span data-stu-id="9a052-157">Contoso, Ltd. has</span></span> 

    <span data-ttu-id="9a052-158">a.</span><span class="sxs-lookup"><span data-stu-id="9a052-158">a.</span></span> <span data-ttu-id="9a052-159">[グローバル MPN id 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile)と[MPN id 2222222 の](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)1 つの下位の場所。</span><span class="sxs-lookup"><span data-stu-id="9a052-159">a [global MPN ID of 1111111](https://partner.microsoft.com/pcv/accountsettings/connectedpartnerprofile) and one subordinate [location MPN IDs of 2222222](https://partner.microsoft.com/pcv/accountsettings/locationsprofile).</span></span>
  
    <span data-ttu-id="9a052-160">b.</span><span class="sxs-lookup"><span data-stu-id="9a052-160">b.</span></span> <span data-ttu-id="9a052-161">Azure AD テナント = @contoso.com</span><span class="sxs-lookup"><span data-stu-id="9a052-161">an Azure AD tenant = @contoso.com</span></span>
 
    <span data-ttu-id="9a052-162">c.</span><span class="sxs-lookup"><span data-stu-id="9a052-162">c.</span></span> <span data-ttu-id="9a052-163">2020年10月1日に有効期限が切れる gold コンピテンシー</span><span class="sxs-lookup"><span data-stu-id="9a052-163">a gold competency that expires October 1, 2020</span></span>
2. <span data-ttu-id="9a052-164">Fabrikam, Inc. は</span><span class="sxs-lookup"><span data-stu-id="9a052-164">Fabrikam, Inc. has</span></span>
 
    <span data-ttu-id="9a052-165">a.</span><span class="sxs-lookup"><span data-stu-id="9a052-165">a.</span></span>  <span data-ttu-id="9a052-166">グローバル MPN ID 3333333 と MPN Id 4444444 と5555555の2つの下位の場所</span><span class="sxs-lookup"><span data-stu-id="9a052-166">a global MPN ID of 3333333 and two subordinate location MPN IDs of 4444444 and 5555555</span></span>

    <span data-ttu-id="9a052-167">b.</span><span class="sxs-lookup"><span data-stu-id="9a052-167">b.</span></span>  <span data-ttu-id="9a052-168">Azure AD テナント = @fabrikam.com</span><span class="sxs-lookup"><span data-stu-id="9a052-168">an Azure AD tenant = @fabrikam.com</span></span>

    <span data-ttu-id="9a052-169">c.</span><span class="sxs-lookup"><span data-stu-id="9a052-169">c.</span></span>  <span data-ttu-id="9a052-170">2020年12月1日に有効期限が切れる2つの gold コンピテンシー</span><span class="sxs-lookup"><span data-stu-id="9a052-170">two gold competencies that expire December 1, 2020</span></span>
3.  <span data-ttu-id="9a052-171">Contoso 社が Fabrikam を購入し、 [ここ](https://partner.microsoft.com/dashboard/account/merger) に移動して、merge 要求を開始します。</span><span class="sxs-lookup"><span data-stu-id="9a052-171">Contoso buys Fabrikam and goes [here](https://partner.microsoft.com/dashboard/account/merger) to initiate a merge request.</span></span>
4.  <span data-ttu-id="9a052-172">Fabrikam はパートナーセンターにサインインし、手順 #3 で Contoso が行ったのと同じページに移動して、Contoso の要求を承認します。</span><span class="sxs-lookup"><span data-stu-id="9a052-172">Fabrikam signs into Partner Center and goes to the same page as Contoso did in step #3, to approve Contoso’s request.</span></span>
5.  <span data-ttu-id="9a052-173">Contoso は、同じページでのマージの詳細を確認し、アカウントの合併を続行するための確認を提供します。</span><span class="sxs-lookup"><span data-stu-id="9a052-173">Contoso reviews the details of the merge on that same page and provides confirmation to proceed with the account merger.</span></span>
6.  <span data-ttu-id="9a052-174">合併後、会社のアカウントは次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="9a052-174">After the merger, the company account will display as:</span></span>

    <span data-ttu-id="9a052-175">a.</span><span class="sxs-lookup"><span data-stu-id="9a052-175">a.</span></span>  <span data-ttu-id="9a052-176">グローバル MPN ID 1111111 と4の下位の location MPN Id (2222222、3333333、4444444、5555555) を持つ Contoso という会社。</span><span class="sxs-lookup"><span data-stu-id="9a052-176">A company named Contoso with a global MPN ID of 1111111 and 4 subordinate location MPN IDs of 2222222, 3333333, 4444444, and 5555555</span></span>
    
    <span data-ttu-id="9a052-177">b.</span><span class="sxs-lookup"><span data-stu-id="9a052-177">b.</span></span>  <span data-ttu-id="9a052-178">@contoso.com @fabrikam.com 同じパートナーセンターアカウントにアクセスできる2つの Azure AD テナント (+) があります。</span><span class="sxs-lookup"><span data-stu-id="9a052-178">It will have two Azure AD tenants (@contoso.com + @fabrikam.com) that have access to the same Partner Center account</span></span>
    
    <span data-ttu-id="9a052-179">c.</span><span class="sxs-lookup"><span data-stu-id="9a052-179">c.</span></span>  <span data-ttu-id="9a052-180">これには、2020年10月1日に有効期限が切れ、もう1つは2020年12月1日という2つのコンピテンシー特典パッケージがあります。</span><span class="sxs-lookup"><span data-stu-id="9a052-180">It will have two competency benefits packages, one that expires October 1, 2020 and another that expires December 1, 2020.</span></span> <span data-ttu-id="9a052-181">2020年12月1日に、1つのコンピテンシー特典パッケージとして更新することができます。</span><span class="sxs-lookup"><span data-stu-id="9a052-181">They'll be able to renew as a single competency benefits package on December 1, 2020.</span></span> <span data-ttu-id="9a052-182">これらの機能を更新すると、Contoso は1つの特典パッケージのみを保持できる場合でも、3つのコンピテンシーをすべて保持します。</span><span class="sxs-lookup"><span data-stu-id="9a052-182">When they renew, Contoso will retain all three competencies even though they can only maintain a single benefits package.</span></span>
    
7.  <span data-ttu-id="9a052-183">Contoso の管理者は、ユーザーのパートナーセンターの役割を引き続き管理し @contoso.com ます。</span><span class="sxs-lookup"><span data-stu-id="9a052-183">Contoso’s admins will continue to manage Partner Center roles for @contoso.com’s users.</span></span> <span data-ttu-id="9a052-184">Fabrikam の管理者は、ユーザーのパートナーセンターの役割を引き続き管理し @fabrikam.com ます。</span><span class="sxs-lookup"><span data-stu-id="9a052-184">Fabrikam’s admins will continue to manage Partner Center roles for @fabrikam.com’s users.</span></span> <span data-ttu-id="9a052-185">Contoso の管理者は、fabrikam のテナントにゲストとして招待されている場合にのみ、Fabrikam のユーザーを管理できます。</span><span class="sxs-lookup"><span data-stu-id="9a052-185">Contoso’s admins can only administer Fabrikam’s users if they are invited as a guest into Fabrikam’s tenant.</span></span>
8.  <span data-ttu-id="9a052-186">Contoso は @fabrikam.com テナントを無視し、 @contoso.com 新しいロールとアクセス許可を持つ Fabrikam の従業員に新しい資格情報を再発行することができます。</span><span class="sxs-lookup"><span data-stu-id="9a052-186">Contoso could decide to ignore the @fabrikam.com tenant, and reissue the Fabrikam employees new @contoso.com credentials with new roles and permissions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9a052-187">次のステップ</span><span class="sxs-lookup"><span data-stu-id="9a052-187">Next steps</span></span>

- [<span data-ttu-id="9a052-188">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="9a052-188">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="9a052-189">パートナー プロファイルの情報を確認する</span><span class="sxs-lookup"><span data-stu-id="9a052-189">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="9a052-190">パートナーが自分で使用するために Azure サブスクリプションを購入できるように Azure パートナー共有サービスを追加する</span><span class="sxs-lookup"><span data-stu-id="9a052-190">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
