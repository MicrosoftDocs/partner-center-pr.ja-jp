---
title: パートナー アカウントを別のパートナー アカウントにマージする
description: パートナーセンターでアクティブな Microsoft パートナーである企業は、自分のアカウントを統合できます。
ms.topic: article
author: parthpandyaMSFT
ms.author: parthp
ms.custom: seodec18
ms.date: 06/12/2020
ms.openlocfilehash: fb54d52d77c6ea80dc2b60f2889e8404c6aca3e0
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265205"
---
# <a name="merge-your-partner-account-with-another-partner-account"></a><span data-ttu-id="48724-103">パートナー アカウントを別のパートナー アカウントにマージする</span><span class="sxs-lookup"><span data-stu-id="48724-103">Merge your partner account with another partner account</span></span>

<span data-ttu-id="48724-104">**該当するロール**</span><span class="sxs-lookup"><span data-stu-id="48724-104">**Applicable roles**</span></span>

- <span data-ttu-id="48724-105">アカウント管理者</span><span class="sxs-lookup"><span data-stu-id="48724-105">Account admin</span></span>

<span data-ttu-id="48724-106">複数の企業がアクティブな Microsoft パートナーであり、パートナーセンターにアカウントを持っている場合、それらのアカウントをマージすることができます。</span><span class="sxs-lookup"><span data-stu-id="48724-106">Two or more companies who are active Microsoft partners and have accounts in Partner Center can choose to merge their accounts.</span></span>

## <a name="what-happens-when-two-partners-elect-to-merge-their-partner-center-accounts"></a><span data-ttu-id="48724-107">2つのパートナーがパートナーセンターのアカウントをマージすることを選択した場合の動作</span><span class="sxs-lookup"><span data-stu-id="48724-107">What happens when two partners elect to merge their Partner Center accounts</span></span>

- <span data-ttu-id="48724-108">マージを開始するパートナー組織は、パートナーグローバルアカウント (PGA) になります。</span><span class="sxs-lookup"><span data-stu-id="48724-108">The partner organization who initiates the merge will be the Partner global account (PGA).</span></span>

- <span data-ttu-id="48724-109">招待された組織の PGA が、発信元企業の場所になります。</span><span class="sxs-lookup"><span data-stu-id="48724-109">The invited organization’s PGA becomes a location of the initiating company.</span></span>

- <span data-ttu-id="48724-110">マージするアカウントのすべての場所は、PGA の下の場所になります。</span><span class="sxs-lookup"><span data-stu-id="48724-110">All the locations of the merging account become locations under the PGA.</span></span>

- <span data-ttu-id="48724-111">アカウントの合併が完了すると、PGA プロファイル内の場所やユーザーなど、両方のアカウントの詳細が表示されます。</span><span class="sxs-lookup"><span data-stu-id="48724-111">Once the account merger is complete, you will see both account’s details such as locations and users within the PGA profile.</span></span> <span data-ttu-id="48724-112">このプロセスを元に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="48724-112">You can't reverse this process.</span></span>

- <span data-ttu-id="48724-113">この統合中に、場所のすべての MPN Id が保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-113">All MPN IDs for locations are preserved during this consolidation.</span></span>

- <span data-ttu-id="48724-114">ユーザーのロールが引き継がれます。</span><span class="sxs-lookup"><span data-stu-id="48724-114">User's roles are brought over.</span></span> <span data-ttu-id="48724-115">たとえば、特定の場所のインセンティブ管理者であるユーザーは、合併後もそのロールを持ち、合併前に見たインセンティブを確認することができます。</span><span class="sxs-lookup"><span data-stu-id="48724-115">For example, if a user had been the incentives admin for a specific location, they would still have that role after the merger and be able to see the incentives they saw prior to the merger.</span></span>

- <span data-ttu-id="48724-116">Azure AD テナントと CSP アカウントはマージされず、影響もありません。</span><span class="sxs-lookup"><span data-stu-id="48724-116">Azure AD tenants and CSP accounts are not merged and have no impact.</span></span>

- <span data-ttu-id="48724-117">両方の会社に関連付けられている公開済みプランと共同販売パイプラインデータは保持されます</span><span class="sxs-lookup"><span data-stu-id="48724-117">Published offers and co-sell pipeline data associated to both companies are preserved</span></span>

### <a name="view-of-merged-accounts"></a><span data-ttu-id="48724-118">マージされたアカウントの表示</span><span class="sxs-lookup"><span data-stu-id="48724-118">View of merged accounts</span></span>

:::image type="content" source="images/merge-accounts/account-merge.png" alt-text="アカウントの合併":::

## <a name="what-to-expect-if-you-have-been-invited-to-merge-your-partner-center-account-with-another-partner-center-account"></a><span data-ttu-id="48724-120">パートナーセンターアカウントを別のパートナーセンターアカウントにマージするように招待されている場合の対処方法</span><span class="sxs-lookup"><span data-stu-id="48724-120">What to expect if you have been invited to merge your Partner Center account with another Partner Center account</span></span>

<span data-ttu-id="48724-121">アカウントの結合への招待に同意する場合は、次のようにします。MPN ID と場所は、招待されたパートナーアカウントの PGA にマージされます。</span><span class="sxs-lookup"><span data-stu-id="48724-121">If you decide to accept the invitation to merge accounts: · Your MPN ID(s) and locations will be merged into the PGA of the partner account that invited you.</span></span>

- <span data-ttu-id="48724-122">ユーザーは、自分のロールとそのままの状態で、統合されたアカウントに移動します。</span><span class="sxs-lookup"><span data-stu-id="48724-122">Your users will be brought into the merged account with their roles intact.</span></span>

- <span data-ttu-id="48724-123">既存の特典とコンピテンシーは、合併後に更新されるまで、両方の企業において保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-123">Existing benefits and competencies will be preserved for both companies after the merger until renewal.</span></span> <span data-ttu-id="48724-124">更新時、アカウントは1つの会社として扱われ、標準の更新規則が適用されます。</span><span class="sxs-lookup"><span data-stu-id="48724-124">At renewal, the accounts will be treated as one company and standard renewal rules will apply.</span></span>

## <a name="understand-the-impacts-to-programs-and-benefits-when-partners-elect-to-merge-accounts"></a><span data-ttu-id="48724-125">パートナーがアカウントを結合する場合のプログラムと利点への影響について理解する</span><span class="sxs-lookup"><span data-stu-id="48724-125">Understand the impacts to programs and benefits when partners elect to merge accounts</span></span>

- <span data-ttu-id="48724-126">すべての既存のコンピテンシー (Gold/シルバー)、購入 (Microsoft Action Pack など)、および関連する特典は、統合時に保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-126">All existing competencies (Gold/Silver), purchases (such as Microsoft Action Pack), and associated benefits are preserved during consolidation.</span></span> <span data-ttu-id="48724-127">両方の企業が同じコンピテンシーを持ち、もう1つはゴールドで、もう1つはゴールドの場合、最高レベルのスキルを持つコンピテンシーが獲得され、パートナーは次の更新まで、そのコンピテンシーに対して1つのシルバー特典とゴールド特典のセットを持ちます。</span><span class="sxs-lookup"><span data-stu-id="48724-127">If both companies have the same competency but one's is gold and the other silver, the competency with highest proficiency level will be awarded, and partners will have one set of silver benefits and one set of gold benefits for that competency until their next renewal.</span></span> 

- <span data-ttu-id="48724-128">Microsoft Action Pack の最高の記念日は、合併後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-128">Highest anniversary date for Microsoft Action Pack will be retained after the merger.</span></span> <span data-ttu-id="48724-129">たとえば、会社1の記念日が Action Pack 更新の場合は6月2020、会社2の Action Pack 更新の記念日が2020年10月である場合、Microsoft では、マージされた会社の新しい記念日として2020年10月日を使用します。</span><span class="sxs-lookup"><span data-stu-id="48724-129">For example, if the anniversary date for company 1 is June 2020 for Action Pack renewal and the anniversary date for Action Pack renewal for company 2 is October 2020, Microsoft will use the October 2020 date as the new anniversary date for the merged company.</span></span>

- <span data-ttu-id="48724-130">アカウントの合併中、次回の更新までは、各アカウントは Action Pack やコンピテンシーの特典を保持します。</span><span class="sxs-lookup"><span data-stu-id="48724-130">During the account merger and until your next renewal, each account will retain their Action Pack and/or competency benefits.</span></span> <span data-ttu-id="48724-131">更新時には、標準 Action Pack とコンピテンシー更新ルールが適用されます。</span><span class="sxs-lookup"><span data-stu-id="48724-131">At renewal, standard Action Pack and competency renewal rules apply.</span></span>

- <span data-ttu-id="48724-132">更新が行われると、コンピテンシーの達成と Action Pack に含まれている特典が、パートナー企業のパートナーグローバルアカウントに実装されます。</span><span class="sxs-lookup"><span data-stu-id="48724-132">Upon renewal, benefits that are included with competency attainment and Action Pack are implemented for the partner company’s partner global account:</span></span>

  - <span data-ttu-id="48724-133">Microsoft Action Pack: パートナー企業は、パートナーのグローバルアカウントごとに1つの Action Pack を購入できます。</span><span class="sxs-lookup"><span data-stu-id="48724-133">Microsoft Action Pack: The partner company will be able to purchase one Action Pack per partner global account.</span></span>

  - <span data-ttu-id="48724-134">コンピテンシー: パートナー企業は、最大の達成度に関連するコア特典の1つのパッケージと、パートナーがパートナーグローバルアカウントごとの資格を持つコンピテンシー固有の特典を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="48724-134">Competency: The partner company will receive one package of core benefits, associated to their highest attainment, plus competency-specific benefits the partner is eligible for per partner global account.</span></span>

- <span data-ttu-id="48724-135">すべてのメリットについては、 [Microsoft Partner Network 特典の使用方法](https://aka.ms/partner-benefits-use-guide)に関するガイドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="48724-135">All benefits are subject to the [Microsoft Partner Network benefits usage guide](https://aka.ms/partner-benefits-use-guide).</span></span> <span data-ttu-id="48724-136">例: アクティブ化された O365 E3 トークンは、アクティブ化してから12か月以内に機能します。</span><span class="sxs-lookup"><span data-stu-id="48724-136">For example: an activated O365 E3 token is functional for twelve (12) months after activation.</span></span> <span data-ttu-id="48724-137">テナントの接続クライアントに対してトークンがアクティブ化されると、その接続クライアントは別のテナントに移動されない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="48724-137">Once a token has been activated for seats on a tenant, those seats may not be moved to another tenant.</span></span>

- <span data-ttu-id="48724-138">両方の企業の MCP ID の関連付けが保持され、PGA MPN ID に関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="48724-138">The MCP ID associations for both companies will be retained and associated with the PGA MPN ID.</span></span>

- <span data-ttu-id="48724-139">市場投入と技術的なメリットは、コンピテンシーコア特典として提供されます。</span><span class="sxs-lookup"><span data-stu-id="48724-139">Go-to-market and technical benefits are offered as competency core benefit.</span></span> <span data-ttu-id="48724-140">マージ後、銀行と税の情報を確認して正確さを確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="48724-140">Post-merge, it’s recommended that you check your bank and tax information to ensure accuracy.</span></span>

- <span data-ttu-id="48724-141">会社が Azure エキスパート MSP プログラムに含まれている場合、特典は更新されるまで保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-141">If your company is in the Azure Expert MSP program, benefits are retained until renewal.</span></span>

- <span data-ttu-id="48724-142">会社が高度な特殊化を獲得している場合は、両方のアカウントで保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-142">If your company has earned advanced specializations, they are retained across both accounts are retained.</span></span>

- <span data-ttu-id="48724-143">ソフトウェアアシュアランスのバウチャーは、両方のアカウントにわたって保持されます。</span><span class="sxs-lookup"><span data-stu-id="48724-143">Any software assurance vouchers are retained across both accounts.</span></span> 

## <a name="invite-a-company-to-merge-their-partner-center-account-with-your-partner-center-account"></a><span data-ttu-id="48724-144">パートナーセンターアカウントをパートナーセンターアカウントにマージするように会社を招待する</span><span class="sxs-lookup"><span data-stu-id="48724-144">Invite a company to merge their Partner Center account with your Partner Center account</span></span>

>[!Note]
><span data-ttu-id="48724-145">アカウントの合併を実行するには、会社の**アカウント管理者**である必要があります。</span><span class="sxs-lookup"><span data-stu-id="48724-145">To perform the account merger, you must be the **Account admin** for your company.</span></span>

1. <span data-ttu-id="48724-146">パートナーセンターのダッシュボードから [**設定**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="48724-146">Select **Settings** from your Partner Center dashboard.</span></span> 

2. <span data-ttu-id="48724-147">[ **Account merge**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="48724-147">Select **Account merge**.</span></span>

3. <span data-ttu-id="48724-148">自分と結合するために招待するアカウントの**パートナープロファイル**にある MPN ID を追加します。</span><span class="sxs-lookup"><span data-stu-id="48724-148">Add the MPN ID located in the **Partner profile** of the account you want to invite to merge with you.</span></span> <span data-ttu-id="48724-149">パートナーのグローバル MPN ID を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="48724-149">You must use their Partner global MPN ID.</span></span> <span data-ttu-id="48724-150">Location MPN ID を使用することはできません。</span><span class="sxs-lookup"><span data-stu-id="48724-150">You can't use a location MPN ID.</span></span>

4. <span data-ttu-id="48724-151">[**マージ**] を選択すると、パートナー企業に招待が送信されます。</span><span class="sxs-lookup"><span data-stu-id="48724-151">When you select **Merge**, an invitation is sent to the partner company.</span></span> <span data-ttu-id="48724-152">要求を受け入れると、パートナーセンター内でアカウントのマージを開始できます。</span><span class="sxs-lookup"><span data-stu-id="48724-152">When they accept your request, you can initiate the account merge within Partner Center.</span></span> <span data-ttu-id="48724-153">組織がアカウントのマージ要求を拒否した場合、その要求が拒否された理由を説明することができます。</span><span class="sxs-lookup"><span data-stu-id="48724-153">If the company rejects your request to merge accounts, they can explain why they rejected the request.</span></span> <span data-ttu-id="48724-154">[**マージ履歴**] では、すべてのアカウントのマージの一覧を使用できます。</span><span class="sxs-lookup"><span data-stu-id="48724-154">A list of all your account merges is available to you under **Merge history**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="48724-155">次のステップ</span><span class="sxs-lookup"><span data-stu-id="48724-155">Next steps</span></span>

- [<span data-ttu-id="48724-156">ユーザー ロールとアクセス許可の割り当て</span><span class="sxs-lookup"><span data-stu-id="48724-156">Assign users roles and permissions</span></span>](permissions-overview.md)

- [<span data-ttu-id="48724-157">パートナー プロファイルの情報を確認する</span><span class="sxs-lookup"><span data-stu-id="48724-157">Verify your partner profile information</span></span>](update-your-partner-profile.md)

- [<span data-ttu-id="48724-158">パートナーが自分で使用するために Azure サブスクリプションを購入できるように Azure パートナー共有サービスを追加する</span><span class="sxs-lookup"><span data-stu-id="48724-158">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>](shared-services.md)
