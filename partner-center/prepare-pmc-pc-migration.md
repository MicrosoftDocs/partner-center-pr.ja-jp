---
title: Partner Membership Center からパートナー センターへの移行を準備する | パートナー センター
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: PMC からパートナー センターにビジネスを移行する前に、役立つ情報とよく寄せられる質問を確認します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 127919c92bf6fffca846dd92cde4c787bfd16641
ms.sourcegitcommit: 87b13da77c16a304d2a7682bf24422f8b9288b51
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2020
ms.locfileid: "82859355"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="542a0-103">Partner Membership Center (PMC) からパートナー センターへの移行を準備する</span><span class="sxs-lookup"><span data-stu-id="542a0-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="542a0-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="542a0-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="542a0-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="542a0-105">Global admin</span></span>
-    <span data-ttu-id="542a0-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="542a0-106">User admin</span></span>
-    <span data-ttu-id="542a0-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="542a0-107">Sales agent</span></span>
-    <span data-ttu-id="542a0-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="542a0-108">Admin agent</span></span>

<span data-ttu-id="542a0-109">当社では、メンバーシップの管理を Partner Membership Center (PMC) から、お客様の Microsoft との取引関係を管理するための単一の目的地であるパートナー センターに移行しています。</span><span class="sxs-lookup"><span data-stu-id="542a0-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="542a0-110">お客のパートナー センターへの移行をできるだけ効率的かつ簡単にしたいと考えています。</span><span class="sxs-lookup"><span data-stu-id="542a0-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="542a0-111">当社はパートナー センターが PMC とは異なるいくつかの領域を識別しており、お客様は移行を行う前にこれを理解し、準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="542a0-112">アカウントと ID のセットアップ</span><span class="sxs-lookup"><span data-stu-id="542a0-112">Account and identity setup</span></span>

<span data-ttu-id="542a0-113">**Azure Active Directory (Azure AD) 職場アカウントとは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="542a0-114">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="542a0-115">職場アカウントは、Azure AD ユーザーとそのユーザーに関する情報 (電子メール、パスワード、プロファイル データ、アクセス許可など) をホストします。</span><span class="sxs-lookup"><span data-stu-id="542a0-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="542a0-116">職場アカウントにはまた、グループ、アプリケーションや、会社とそのセキュリティに関連するその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="542a0-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="542a0-117">勤務先の電子メールは、Azure Active Directory テナントの一部です。</span><span class="sxs-lookup"><span data-stu-id="542a0-117">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="542a0-118">パートナー センターでアカウントを作成するには、AAD テナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="542a0-118">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="542a0-119">Azure Active Directory の詳細については、[Azure AD でのディレクトリの作成](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-119">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="542a0-120">パートナー センターでは、個人の電子メールではなく、勤務先の電子メールを使用してアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="542a0-120">In Partner Center, you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="542a0-121">職場アカウント: john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="542a0-121">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="542a0-122">個人アカウント: John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="542a0-122">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="542a0-123">**Microsoft に AAD テナント (たとえば Office 365 用) があり、さらに CSP ビジネス用のテナントも存在する場合、どのようなアカウントを使用してパートナー センターにサインインする必要がありますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-123">**What account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="542a0-124">CSP アカウントまたは MPN の勤務先の電子メール アカウントのどちらでもパートナー センターにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="542a0-124">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="542a0-125">CSP の勤務先の電子メールを使用してサインインすることを選択した場合、ダッシュボードの左側のナビゲーションには MPN と CSP の両方のプログラム情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-125">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="542a0-126">MPN Azure AD テナントの勤務先の電子メールを使用してサインインした場合は、MPN プログラム情報のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-126">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> 

<span data-ttu-id="542a0-127">**パートナー センターのために既存の Office 365 Azure AD テナントを使用したくない場合は、PMC からの移行の前に新しいテナントを作成できます。**</span><span class="sxs-lookup"><span data-stu-id="542a0-127">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="542a0-128">パートナー センター アカウントを設定するために既存の Azure AD テナントを使用したくない理由には多くのものがあります。</span><span class="sxs-lookup"><span data-stu-id="542a0-128">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="542a0-129">パートナー センターへの移行を開始する前に、[Azure portal](https://ms.portal.azure.com/#home) に移動して新しい Azure AD テナントを作成します。</span><span class="sxs-lookup"><span data-stu-id="542a0-129">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="542a0-130">[Azure Active Directory での新しいテナントの作成](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)に関するページのガイダンスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="542a0-130">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="542a0-131">新しい AAD テナントを使用して、パートナー センターアカウントを設定します。</span><span class="sxs-lookup"><span data-stu-id="542a0-131">Use the new AAD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="542a0-132">テナントを作成するには、グローバル管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-132">You must be a global admin to create the tenant.</span></span> 


<span data-ttu-id="542a0-133">**ロール パートナー センターのゲスト ユーザーを含むユーザー ロール**</span><span class="sxs-lookup"><span data-stu-id="542a0-133">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="542a0-134">パートナー センターには、実行する必要がある作業の種類に応じて、さまざまな種類のロールが存在します。</span><span class="sxs-lookup"><span data-stu-id="542a0-134">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="542a0-135">Azure AD ロールであるグローバル管理者などのロールがあります。</span><span class="sxs-lookup"><span data-stu-id="542a0-135">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="542a0-136">一部のロールは、クラウド サービス プロバイダー プログラムまたはインセンティブなどのプログラムに固有であり、MPN に固有のロールもあります。</span><span class="sxs-lookup"><span data-stu-id="542a0-136">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="542a0-137">すべてのパートナー センター ロールの種類を見つけるには、「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-137">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="542a0-138">**ユーザーが PMC からパートナー センターに移行すると、そのユーザーのロールはどうなりますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-138">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="542a0-139">MPN グローバル管理者、または移行を実行するプライマリ プログラムの連絡先を除き、PMC のすべてのユーザーがその管理者ロールを失います。</span><span class="sxs-lookup"><span data-stu-id="542a0-139">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="542a0-140">移行を完了する個人は、パートナー センターでロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-140">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="542a0-141">パートナー センターのロールは PMC のロールとは異なります。</span><span class="sxs-lookup"><span data-stu-id="542a0-141">The roles in Partner Center differ from the roles in PMC.</span></span> <span data-ttu-id="542a0-142">パートナー センターのユーザー ロールの詳細については、[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md) および「[PMC からパートナー センターに移動する](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-142">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="542a0-143">**会社プロファイルとビジネス プロファイルの違いは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-143">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="542a0-144">会社プロファイルは、住所、場所、主要連絡先、銀行、税金などの詳細が含まれている、会社に関する情報です。</span><span class="sxs-lookup"><span data-stu-id="542a0-144">Your company profile is the information about your company that includes address, locations, primary contact, bank, and tax details.</span></span>

<span data-ttu-id="542a0-145">ビジネス プロファイルは会社を顧客に紹介する方法であり、ロゴ、ビジネスの重点に関する詳細、専門知識などを表示するマーケティング ページです。</span><span class="sxs-lookup"><span data-stu-id="542a0-145">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="542a0-146">**アカウントの統合はアカウントに関してどのような意味がありますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-146">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="542a0-147">同じ Azure AD テナントを使用して複数の MPN アカウントをパートナー センターに移行する場合、システムはそれを自動的に認識し、アカウントを統合するようユーザーに依頼します。</span><span class="sxs-lookup"><span data-stu-id="542a0-147">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="542a0-148">これは、同じ Azure AD テナントに複数のドメインが関連付けられている場合でも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="542a0-148">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="542a0-149">引き続き、個別の AAD テナントを使用してパートナー センターに移行するようにもできますが、それにより、コンピテンシーの評価の分離や余分な購入コストが発生することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-149">You could still decide to migrate to Partner Center using separate AAD tenants, but note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> <span data-ttu-id="542a0-150">アカウントの統合の詳細については、「[会社のアカウントを統合する](consolidate-accounts.md)」をお読みください。</span><span class="sxs-lookup"><span data-stu-id="542a0-150">For more information about account consolidation, read [Consolidate your company accounts](consolidate-accounts.md)</span></span>

<span data-ttu-id="542a0-151">**複数の AAD テナントと 1 つの MPN アカウントがある場合、パートナー センターでそれらをリンクできますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-151">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="542a0-152">はい。パートナー センターでは、複数の Azure AD テナントを 1 つのパートナー センター アカウントにリンクできます。</span><span class="sxs-lookup"><span data-stu-id="542a0-152">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="542a0-153">アカウントの統合の詳細については、「[会社のアカウントを統合する](consolidate-accounts.md)」をお読みください。</span><span class="sxs-lookup"><span data-stu-id="542a0-153">For more information about account consolidation, read [Consolidate your company accounts](consolidate-accounts.md)</span></span>

<span data-ttu-id="542a0-154">**複数の Azure AD テナントを 1 つのパートナー センター アカウントに追加する場合の制限はありますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-154">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="542a0-155">Azure AD テナントが既存のパートナー センター アカウントに既に関連付けられている場合は、マルチテナント機能を使用して、それを新しいパートナー センター アカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="542a0-155">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="542a0-156">別の考え方をすると、Azure AD テナントは 1 つのパートナー センター アカウントにしか関連付けられませんが、パートナー センター アカウントには複数のテナントを関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="542a0-156">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="542a0-157">Microsoft Partner Network (MPN) メンバーシップの移行</span><span class="sxs-lookup"><span data-stu-id="542a0-157">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="542a0-158">**だれが PMC からパートナー センターへの移行を実行できますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-158">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="542a0-159">会社の MPN グローバル管理者またはプライマリ プログラムの連絡先 (この 2 つのロールは多くの場合、同じユーザーによって保持されます) が移行を開始および実行できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-159">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="542a0-160">**移行を完了するユーザーは、パートナー センターでの会社の法的プロファイル上の主要連絡先になりますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-160">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="542a0-161">必ずしもそうではありませんが、主要連絡先は、契約に署名する権限を持つだれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-161">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="542a0-162">**Microsoft は、ユーザーの代わりに MPN メンバーシップを移行できますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-162">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="542a0-163">いいえ。</span><span class="sxs-lookup"><span data-stu-id="542a0-163">No.</span></span> <span data-ttu-id="542a0-164">Microsoft は、ユーザーのメンバーシップ アカウントのパートナー センターへの移行を支援できません。</span><span class="sxs-lookup"><span data-stu-id="542a0-164">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="542a0-165">アカウントを移行するには、職場アカウント (サインイン資格情報) で PMC にサインインして移行プロセスを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-165">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="542a0-166">アカウントを移行する手順を完了したら、メンバーシップの管理を開始し、チームのメンバーが特典にアクセスしたり、メンバーシップを管理したりできるように、ユーザー ロールとアクセス許可をチームに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="542a0-166">After you've completed the steps to move your account, you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="542a0-167">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブのための銀行/税金情報、Partner University へのアクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="542a0-167">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="542a0-168">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブのための銀行/税金情報、Partner University へのアクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="542a0-168">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="542a0-169">**更新ポリシーはどのように変更されますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-169">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="542a0-170">パートナー センターでは、更新期間は今後 30 日間のユーザーの記念日から取得されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-170">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="542a0-171">**パートナー センターに移行した後もコンピテンシーは変更されないままですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-171">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="542a0-172">はい。コンピテンシーはパートナー センターへの移行の影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="542a0-172">Yes, competencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="542a0-173">不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="542a0-173">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="542a0-174">**移行した後、特典 (クラウドの特典、テクニカル サポート、ソフトウェア特典、Visual Studio を含む) は変更されますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-174">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="542a0-175">対象となる特典は変更されません。</span><span class="sxs-lookup"><span data-stu-id="542a0-175">Your eligible benefits will not change.</span></span> <span data-ttu-id="542a0-176">不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="542a0-176">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="542a0-177">**Visual Studio の特典が割り当てられた Microsoft アカウントは守られますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-177">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="542a0-178">はい。</span><span class="sxs-lookup"><span data-stu-id="542a0-178">Yes.</span></span> <span data-ttu-id="542a0-179">MSA に割り当てられた Visual Studio の特典が守られて、保持されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-179">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="542a0-180">それらは、パートナー センターで更新された後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-180">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="542a0-181">ただし、パートナー センターに移行された後に MSA の割り当てを削除した場合、それをパートナー センターに戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="542a0-181">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="542a0-182">パートナー センターでは、パートナーは、パートナーが Azure AD テナントの MPN 管理者である同じテナントから、MSA である職場アカウントとゲスト ユーザー アカウントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-182">In Partner Center, a partner can add work accounts and guest user accounts, which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="542a0-183">パートナーが複数の Azure AD テナントのグローバル管理者であり、これらすべてのテナントが同じパートナー センター アカウントに関連付けられている場合、パートナーは、これらすべてのテナントのユーザーを、Visual Studio の特典と Azure の使用量ベースの割り当てに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="542a0-183">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="542a0-184">MPN 管理者または全体管理者は Visual Studio の使用量ベースのサブスクリプションにゲスト ユーザーを割り当てることができますが、ゲスト ユーザーは MSA を使用してパートナー センターにサインインすることはできません。</span><span class="sxs-lookup"><span data-stu-id="542a0-184">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="542a0-185">ただし、ゲスト ユーザーは、Azure と Visual Studio にサインインして、割り当てられた特典を検証および使用できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-185">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="542a0-186">**MCP の関連付けや Partner University へのアクセスを管理するにはどうすればよいですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-186">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="542a0-187">PMC から移行する MCP の関連付けに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="542a0-187">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="542a0-188">ただし、パートナー センターに移行した後の新しい従業員はすべて、パートナー センターで関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-188">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="542a0-189">既存のユーザーの Partner University のアクセス許可はすべてそのままになりますが、新しい従業員は[トレーニング センター](https://partner.microsoft.com/training)に移動して、Partner University へのアクセスを取得する方法を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="542a0-189">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="542a0-190">**パートナー センターに移行した後に MCP 情報を表示するにはどうすればよいですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-190">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="542a0-191">ダッシュボードの左側のナビゲーションから **[コンピテンシー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="542a0-191">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="542a0-192">**[コンピテンシー]** ページから、スキル レポートをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="542a0-192">From the **Competencies** page, you are able to download the skills report.</span></span> <span data-ttu-id="542a0-193">スキル レポートには、パートナー センターのコンピテンシーやプログラムに関連するスキルを取得しているユーザーが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="542a0-193">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="542a0-194">ユーザーがスキルを取得しているが、それらのスキルが対象のコンピテンシーに関連していない場合、そのユーザーはレポートに一覧表示されません。</span><span class="sxs-lookup"><span data-stu-id="542a0-194">If your users have gained skills but those skills are not relevant to the competencies you're working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="542a0-195">**顧客参照はパートナー センターで使用されていますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-195">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="542a0-196">いいえ。パートナー センターでのコンピテンシー要件を満たすために顧客参照は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="542a0-196">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="542a0-197">**レコードのパートナーの関連付けはパートナー センターに移行されますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-197">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="542a0-198">はい。レコードのパートナーに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="542a0-198">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="542a0-199">[顧客へのパートナー ID のリンク](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)の詳細を確認してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-199">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="542a0-200">**パートナー センターへの移行によりインセンティブに影響はありますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-200">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="542a0-201">いいえ。場所を統合せずにアカウントを移行した場合、インセンティブに影響はありません。</span><span class="sxs-lookup"><span data-stu-id="542a0-201">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="542a0-202">PMC に複数のアカウントがあり、パートナー センターに移行するときにグローバル アカウントに統合することにした場合、インセンティブに損失は発生しませんが、インセンティブの支払いが遅延することがあります。</span><span class="sxs-lookup"><span data-stu-id="542a0-202">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="542a0-203">インセンティブ プログラムに関連するすべての PMC アカウントを移行するわけではない場合、それらのアカウントに関連付けられているインセンティブの獲得を停止できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-203">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="542a0-204">**パートナー センターのインセンティブ ロールとは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-204">**What are the incentive roles in Partner Center?**</span></span> 

<span data-ttu-id="542a0-205">パートナー センターのインセンティブ ロールは場所に基づいており、インセンティブ管理者とインセンティブ ユーザーを含んでいます。</span><span class="sxs-lookup"><span data-stu-id="542a0-205">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="542a0-206">これらのロールが実行できる操作の詳細については「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="542a0-206">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="542a0-207">**インセンティブ管理者をグローバル レベルと場所レベルで割り当てることはできますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-207">**Can incentives admins be assigned at the global and location level?**</span></span>

 <span data-ttu-id="542a0-208">はい。</span><span class="sxs-lookup"><span data-stu-id="542a0-208">Yes.</span></span> <span data-ttu-id="542a0-209">インセンティブ管理者をすべての場所のインセンティブ管理者になるように割り当てることも、各場所に独自のインセンティブ管理者を割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="542a0-209">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="542a0-210">**インセンティブをグローバル レベルまたは場所レベルで支払われるようにすることはできますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-210">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="542a0-211">インセンティブは、場所レベルでのみ支払われます。</span><span class="sxs-lookup"><span data-stu-id="542a0-211">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="542a0-212">**紹介に関連して、いくつのビジネス プロファイルを作成できますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-212">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="542a0-213">会社は、自社の関心を十分に示すため、必要に応じてビジネス プロファイルをいくつでも作成できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-213">Your company can create as many business profiles as you need to fully represent your company's interests.</span></span> <span data-ttu-id="542a0-214">各ビジネス プロファイルでは、最大 5 つの場所 (国ごとに 1 つの場所) を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="542a0-214">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="542a0-215">各ビジネス プロファイルは、その各場所の紹介を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="542a0-215">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="542a0-216">**紹介はどのように割り当てられ、どのような変化を期待できますか?たとえば、1 つの市場にグローバルな会社を持ち、その他の市場に複数の場所を持っている場合、紹介はどのように割り当てられますか?**</span><span class="sxs-lookup"><span data-stu-id="542a0-216">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="542a0-217">紹介は、顧客が定義する検索パラメーターに基づいて割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="542a0-217">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="542a0-218">持っている場所が 1 つか複数かには関係なく、顧客が目的の場所を指定し、そこに他のパラメーターを満たすビジネスがある場合、紹介はその場所に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="542a0-218">Regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








