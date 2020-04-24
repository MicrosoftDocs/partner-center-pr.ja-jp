---
title: Partner Membership Center からパートナー センターへの移行を準備する | パートナー センター
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: PMC からパートナー センターにビジネスを移行する前に、役立つ情報とよく寄せられる質問を確認します。
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 06167a667152ddaf65702547783df93726f6cadc
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "78340105"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="6aefc-103">Partner Membership Center (PMC) からパートナー センターへの移行を準備する</span><span class="sxs-lookup"><span data-stu-id="6aefc-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="6aefc-104">**適切なロール**</span><span class="sxs-lookup"><span data-stu-id="6aefc-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="6aefc-105">グローバル管理者</span><span class="sxs-lookup"><span data-stu-id="6aefc-105">Global admin</span></span>
-    <span data-ttu-id="6aefc-106">ユーザー管理者</span><span class="sxs-lookup"><span data-stu-id="6aefc-106">User admin</span></span>
-    <span data-ttu-id="6aefc-107">販売代理店</span><span class="sxs-lookup"><span data-stu-id="6aefc-107">Sales agent</span></span>
-    <span data-ttu-id="6aefc-108">管理エージェント</span><span class="sxs-lookup"><span data-stu-id="6aefc-108">Admin agent</span></span>

<span data-ttu-id="6aefc-109">当社では、メンバーシップの管理を Partner Membership Center (PMC) から、お客様の Microsoft との取引関係を管理するための単一の目的地であるパートナー センターに移行しています。</span><span class="sxs-lookup"><span data-stu-id="6aefc-109">We are moving membership management from Partner Membership Center (PMC) to the partner center - the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="6aefc-110">お客のパートナー センターへの移行をできるだけ効率的かつ簡単にしたいと考えています。</span><span class="sxs-lookup"><span data-stu-id="6aefc-110">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="6aefc-111">当社はパートナー センターが PMC とは異なるいくつかの領域を識別しており、お客様は移行を行う前にこれを理解し、準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-111">We've identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="6aefc-112">アカウントと ID のセットアップ</span><span class="sxs-lookup"><span data-stu-id="6aefc-112">Account and identity setup</span></span>

<span data-ttu-id="6aefc-113">**Azure Active Directory (Azure AD) 職場アカウントとは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-113">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="6aefc-114">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-114">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="6aefc-115">職場アカウントは、Azure AD ユーザーとそのユーザーに関する情報 (電子メール、パスワード、プロファイル データ、アクセス許可など) をホストします。</span><span class="sxs-lookup"><span data-stu-id="6aefc-115">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="6aefc-116">職場アカウントにはまた、グループ、アプリケーションや、会社とそのセキュリティに関連するその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="6aefc-116">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="6aefc-117">パートナー センターでは、個人の電子メールではなく、勤務先の電子メールを使用してアカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="6aefc-117">In Partner Center, you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="6aefc-118">職場アカウント: john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="6aefc-118">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="6aefc-119">個人アカウント: John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="6aefc-119">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="6aefc-120">勤務先の電子メールは、Azure Active Directory テナントの一部です。</span><span class="sxs-lookup"><span data-stu-id="6aefc-120">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="6aefc-121">パートナー センターでアカウントを作成するには、AAD テナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="6aefc-121">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="6aefc-122">Azure Active Directory の詳細については、[Azure AD でのディレクトリの作成](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-122">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="6aefc-123">**Microsoft に AAD テナント (たとえば Office 365 用) があり、さらに CSP ビジネス用のテナントも存在する場合、PMC からパートナー センターに移行するときは、どのようなアカウントを使用してパートナー センターにサインインする必要がありますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-123">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="6aefc-124">CSP アカウントまたは MPN の勤務先の電子メール アカウントのどちらでもパートナー センターにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-124">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="6aefc-125">CSP の勤務先の電子メールを使用してサインインすることを選択した場合、ダッシュボードの左側のナビゲーションには MPN と CSP の両方のプログラム情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-125">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="6aefc-126">MPN Azure AD テナントの勤務先の電子メールを使用してサインインした場合は、MPN プログラム情報のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-126">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="6aefc-127">ユーザー ロールは MPN と CSP とで異なるため、MPN ビジネスと CSP ビジネスの両方に同じアカウントを使用する場合は、それに応じてユーザー ロールを割り当てるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-127">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="6aefc-128">ユーザー ロールについては、「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-128">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="6aefc-129">**パートナー センターのために既存の Office 365 Azure AD テナントを使用したくない場合は、PMC からの移行の前に新しいテナントを作成できます。**</span><span class="sxs-lookup"><span data-stu-id="6aefc-129">**If you don't want to use your existing Office 365 Azure AD tenant for Partner Center, you can create a new tenant prior to migrating from PMC.**</span></span>

<span data-ttu-id="6aefc-130">パートナー センター アカウントを設定するために既存の Azure AD テナントを使用したくない理由には多くのものがあります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-130">There may be many reasons you don't want to use an existing Azure AD tenant to set up your Partner Center account.</span></span> <span data-ttu-id="6aefc-131">パートナー センターへの移行を開始する前に、[Azure portal](https://ms.portal.azure.com/#home) に移動して新しい Azure AD テナントを作成します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-131">Before you begin migrating to Partner Center, go to the [Azure portal](https://ms.portal.azure.com/#home) to create a new Azure AD tenant.</span></span> <span data-ttu-id="6aefc-132">[Azure Active Directory での新しいテナントの作成](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant)に関するページのガイダンスに従ってください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-132">Follow the guidance in [Create a new tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant).</span></span> <span data-ttu-id="6aefc-133">新しいテナントを作成したら、PMC からパートナー センターに移行するときに、この AAD テナントを使用してパートナー センター アカウントを設定します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-133">Once you have created the new tenant, use this AAD tenant to set up your Partner Center account when you move from PMC to Partner Center.</span></span> <span data-ttu-id="6aefc-134">テナントを作成するには、グローバル管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-134">You must be a global admin to create the tenant.</span></span> <span data-ttu-id="6aefc-135">この新しいディレクトリを使用してパートナー センターに移行します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-135">Use this new directory to migrate to Partner Center.</span></span>


<span data-ttu-id="6aefc-136">**AAD グローバル管理者ロールと PMC MPN グローバル管理者ロールの違いは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-136">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="6aefc-137">これらは、異なるアクセス許可を持つ 2 つの異なるロールです。</span><span class="sxs-lookup"><span data-stu-id="6aefc-137">These are two different roles with different permissions.</span></span> <span data-ttu-id="6aefc-138">パートナー センターの AAD テナント グローバル管理者はテナントを管理します。つまり、ユーザーを追加または削除し、パスワード、ロール、アクセス許可を提供および管理し、さらにパートナー センターにある会社のすべてのプログラムへのアクセス権を持っています。</span><span class="sxs-lookup"><span data-stu-id="6aefc-138">The AAD tenant global admin in Partner Center administers the tenant - adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company's programs in Partner Center.</span></span> 

<span data-ttu-id="6aefc-139">PMC の MPN グローバル管理者ロールは、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-139">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="6aefc-140">会社および会社のすべての場所に関連したすべてのデータを表示および編集する。</span><span class="sxs-lookup"><span data-stu-id="6aefc-140">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="6aefc-141">グローバルまたはローカル レベルで管理者を追加する。</span><span class="sxs-lookup"><span data-stu-id="6aefc-141">Add administrators at the global or local level.</span></span>  <span data-ttu-id="6aefc-142">また、グローバル管理者は、任意の場所にいる任意のユーザーにグローバル管理者アクセスを割り当てることもできます。これにより、どの場所に関連付けられているかには関係なく、グローバル アクセスが付与されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-142">Also, Global admins can assign any person at any location Global Administrator Access, which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="6aefc-143">次のような任意のパートナー向け UI 機能を実行する。</span><span class="sxs-lookup"><span data-stu-id="6aefc-143">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="6aefc-144">ユーザーの追加/削除</span><span class="sxs-lookup"><span data-stu-id="6aefc-144">Add/remove users</span></span>

 - <span data-ttu-id="6aefc-145">ロールの割り当て/削除</span><span class="sxs-lookup"><span data-stu-id="6aefc-145">Assign/remove roles</span></span> 

 - <span data-ttu-id="6aefc-146">場所の追加/削除/更新</span><span class="sxs-lookup"><span data-stu-id="6aefc-146">Add/remove/update locations</span></span> 

 - <span data-ttu-id="6aefc-147">コンピテンシー/マップの購入</span><span class="sxs-lookup"><span data-stu-id="6aefc-147">Purchase competency/maps</span></span> 

-  <span data-ttu-id="6aefc-148">特典の表示</span><span class="sxs-lookup"><span data-stu-id="6aefc-148">View benefits</span></span>

<span data-ttu-id="6aefc-149">MPN グローバル管理者がパートナー センターに移行した場合、そのロールは MPN パートナー管理者と呼ばれます。これには、パートナー センターのグローバル管理者とは異なるアクセス許可とタスクが割り当てられます。パートナー センターのロールとアクセス許可の詳細については、「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-149">When the MPN global admin moves to Partner Center the role is called the MPN partner admin, which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="6aefc-150">**ロール パートナー センターのゲスト ユーザーを含むユーザー ロール**</span><span class="sxs-lookup"><span data-stu-id="6aefc-150">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="6aefc-151">パートナー センターには、実行する必要がある作業の種類に応じて、さまざまな種類のロールが存在します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-151">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="6aefc-152">Azure AD ロールであるグローバル管理者などのロールがあります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-152">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="6aefc-153">一部のロールは、クラウド サービス プロバイダー プログラムまたはインセンティブなどのプログラムに固有であり、MPN に固有のロールもあります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-153">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="6aefc-154">すべてのパートナー センター ロールの種類を見つけるには、「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-154">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="6aefc-155">**ユーザーが PMC からパートナー センターに移行すると、そのユーザーのロールはどうなりますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-155">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="6aefc-156">MPN グローバル管理者、または移行を実行するプライマリ プログラムの連絡先を除き、PMC のすべてのユーザーがその管理者ロールを失います。</span><span class="sxs-lookup"><span data-stu-id="6aefc-156">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="6aefc-157">移行を完了する個人は、パートナー センターでロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-157">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="6aefc-158">パートナー センターのロールは PMC のロールとは異なります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-158">The roles in Partner Center differ from the roles in PMC.</span></span> <span data-ttu-id="6aefc-159">パートナー センターのユーザー ロールの詳細については、[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md) および「[PMC からパートナー センターに移動する](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-159">Read [Assign users roles and permissions](permissions-overview.md and [Moving from PMC to Partner Center](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="6aefc-160">**会社プロファイルとビジネス プロファイルの違いは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-160">**What's the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="6aefc-161">会社プロファイルは、住所、場所、主要連絡先、銀行、税金などの詳細が含まれている、会社に関する情報です。</span><span class="sxs-lookup"><span data-stu-id="6aefc-161">Your company profile is the information about your company that includes address, locations, primary contact, bank, and tax details.</span></span>

<span data-ttu-id="6aefc-162">ビジネス プロファイルは会社を顧客に紹介する方法であり、ロゴ、ビジネスの重点に関する詳細、専門知識などを表示するマーケティング ページです。</span><span class="sxs-lookup"><span data-stu-id="6aefc-162">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="6aefc-163">**アカウントの統合はアカウントに関してどのような意味がありますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-163">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="6aefc-164">同じ Azure AD テナントを使用して複数の MPN アカウントをパートナー センターに移行する場合、システムはそれを自動的に認識し、アカウントを統合するようユーザーに依頼します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-164">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="6aefc-165">これは、同じ Azure AD テナントに複数のドメインが関連付けられている場合でも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-165">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="6aefc-166">引き続き、個別の AAD テナントを使用してパートナー センターに移行するようにもできますが、それにより、コンピテンシーの評価の分離や余分な購入コストが発生することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-166">You could still decide to migrate to Partner Center using separate AAD tenants, but note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="6aefc-167">**複数の AAD テナントと 1 つの MPN アカウントがある場合、パートナー センターでそれらをリンクできますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-167">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="6aefc-168">はい。パートナー センターでは、複数の Azure AD テナントを 1 つのパートナー センター アカウントにリンクできます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-168">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="6aefc-169">詳細については、ここを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-169">Learn more here.</span></span> 

<span data-ttu-id="6aefc-170">**複数の Azure AD テナントを 1 つのパートナー センター アカウントに追加する場合の制限はありますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-170">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="6aefc-171">Azure AD テナントが既存のパートナー センター アカウントに既に関連付けられている場合は、マルチテナント機能を使用して、それを新しいパートナー センター アカウントに関連付けることはできません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-171">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="6aefc-172">別の考え方をすると、Azure AD テナントは 1 つのパートナー センター アカウントにしか関連付けられませんが、パートナー センター アカウントには複数のテナントを関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-172">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="6aefc-173">Microsoft Partner Network (MPN) メンバーシップの移行</span><span class="sxs-lookup"><span data-stu-id="6aefc-173">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="6aefc-174">**だれが PMC からパートナー センターへの移行を実行できますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-174">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="6aefc-175">会社の MPN グローバル管理者またはプライマリ プログラムの連絡先 (この 2 つのロールは多くの場合、同じユーザーによって保持されます) が移行を開始および実行できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-175">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="6aefc-176">**移行を完了するユーザーは、パートナー センターでの会社の法的プロファイル上の主要連絡先になりますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-176">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="6aefc-177">必ずしもそうではありませんが、主要連絡先は、契約に署名する権限を持つだれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-177">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="6aefc-178">**Microsoft は、ユーザーの代わりに MPN メンバーシップを移行できますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-178">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="6aefc-179">いいえ。</span><span class="sxs-lookup"><span data-stu-id="6aefc-179">No.</span></span> <span data-ttu-id="6aefc-180">Microsoft は、ユーザーのメンバーシップ アカウントのパートナー センターへの移行を支援できません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-180">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="6aefc-181">アカウントを移行するには、職場アカウント (サインイン資格情報) で PMC にサインインして移行プロセスを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-181">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="6aefc-182">アカウントを移行する手順を完了したら、メンバーシップの管理を開始し、チームのメンバーが特典にアクセスしたり、メンバーシップを管理したりできるように、ユーザー ロールとアクセス許可をチームに割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-182">After you've completed the steps to move your account, you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="6aefc-183">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブのための銀行/税金情報、Partner University へのアクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-183">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="6aefc-184">Microsoft は、現在のコンピテンシー、特典、場所情報、インセンティブのための銀行/税金情報、Partner University へのアクセスを含む MCP の関連付けを自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-184">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="6aefc-185">**更新ポリシーはどのように変更されますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-185">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="6aefc-186">パートナー センターでは、更新期間は今後 30 日間のユーザーの記念日から取得されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-186">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="6aefc-187">**パートナー センターに移行した後もコンピテンシーは変更されないままですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-187">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="6aefc-188">はい。コンピテンシーはパートナー センターへの移行の影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-188">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="6aefc-189">不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-189">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="6aefc-190">**移行した後、特典 (クラウドの特典、テクニカル サポート、ソフトウェア特典、Visual Studio を含む) は変更されますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-190">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="6aefc-191">対象となる特典は変更されません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-191">Your eligible benefits will not change.</span></span> <span data-ttu-id="6aefc-192">不一致に気が付いた場合は、[サポート](https://partner.microsoft.com/support)に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-192">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="6aefc-193">**Visual Studio の特典が割り当てられた Microsoft アカウントは守られますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-193">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="6aefc-194">はい。</span><span class="sxs-lookup"><span data-stu-id="6aefc-194">Yes.</span></span> <span data-ttu-id="6aefc-195">MSA に割り当てられた Visual Studio の特典が守られて、保持されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-195">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="6aefc-196">それらは、パートナー センターで更新された後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-196">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="6aefc-197">ただし、パートナー センターに移行された後に MSA の割り当てを削除した場合、それをパートナー センターに戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-197">However, if you remove an MSA allocation once migrated in Partner Center, it can't be added  back into Partner Center.</span></span>

<span data-ttu-id="6aefc-198">パートナー センターでは、パートナーは、パートナーが Azure AD テナントの MPN 管理者である同じテナントから、MSA である職場アカウントとゲスト ユーザー アカウントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-198">In Partner Center, a partner can add work accounts and guest user accounts, which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="6aefc-199">パートナーが複数の Azure AD テナントのグローバル管理者であり、これらすべてのテナントが同じパートナー センター アカウントに関連付けられている場合、パートナーは、これらすべてのテナントのユーザーを、Visual Studio の特典と Azure の使用量ベースの割り当てに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-199">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="6aefc-200">MPN 管理者または全体管理者は Visual Studio の使用量ベースのサブスクリプションにゲスト ユーザーを割り当てることができますが、ゲスト ユーザーは MSA を使用してパートナー センターにサインインすることはできません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-200">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="6aefc-201">ただし、ゲスト ユーザーは、Azure と Visual Studio にサインインして、割り当てられた特典を検証および使用できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-201">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="6aefc-202">**MCP の関連付けや Partner University へのアクセスを管理するにはどうすればよいですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-202">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="6aefc-203">PMC から移行する MCP の関連付けに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-203">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="6aefc-204">ただし、パートナー センターに移行した後の新しい従業員はすべて、パートナー センターで関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-204">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="6aefc-205">既存のユーザーの Partner University のアクセス許可はすべてそのままになりますが、新しい従業員は[トレーニング センター](https://partner.microsoft.com/training)に移動して、Partner University へのアクセスを取得する方法を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-205">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="6aefc-206">**パートナー センターに移行した後に MCP 情報を表示するにはどうすればよいですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-206">**How do I view MCP information once I move to Partner Center?**</span></span>

<span data-ttu-id="6aefc-207">ダッシュボードの左側のナビゲーションから **[コンピテンシー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6aefc-207">Select **Competencies** from the left nav on the dashboard.</span></span> <span data-ttu-id="6aefc-208">**[コンピテンシー]** ページから、スキル レポートをダウンロードできます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-208">From the **Competencies** page, you are able to download the skills report.</span></span> <span data-ttu-id="6aefc-209">スキル レポートには、パートナー センターのコンピテンシーやプログラムに関連するスキルを取得しているユーザーが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-209">The skills report will list your users who have acquired skills relevant to the competencies and programs in Partner Center.</span></span> <span data-ttu-id="6aefc-210">ユーザーがスキルを取得しているが、それらのスキルが対象のコンピテンシーに関連していない場合、そのユーザーはレポートに一覧表示されません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-210">If your users have gained skills but those skills are not relevant to the competencies you're working toward, they will not be listed in the report.</span></span>


 <span data-ttu-id="6aefc-211">**顧客参照はパートナー センターで使用されていますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-211">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="6aefc-212">いいえ。パートナー センターでのコンピテンシー要件を満たすために顧客参照は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-212">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="6aefc-213">**レコードのパートナーの関連付けはパートナー センターに移行されますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-213">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="6aefc-214">はい。レコードのパートナーに変更はありません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-214">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="6aefc-215">[顧客へのパートナー ID のリンク](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)の詳細を確認してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-215">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="6aefc-216">**パートナー センターへの移行によりインセンティブに影響はありますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-216">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="6aefc-217">いいえ。場所を統合せずにアカウントを移行した場合、インセンティブに影響はありません。</span><span class="sxs-lookup"><span data-stu-id="6aefc-217">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="6aefc-218">PMC に複数のアカウントがあり、パートナー センターに移行するときにグローバル アカウントに統合することにした場合、インセンティブに損失は発生しませんが、インセンティブの支払いが遅延することがあります。</span><span class="sxs-lookup"><span data-stu-id="6aefc-218">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="6aefc-219">インセンティブ プログラムに関連するすべての PMC アカウントを移行するわけではない場合、それらのアカウントに関連付けられているインセンティブの獲得を停止できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-219">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="6aefc-220">**パートナー センターのインセンティブ ユーザー ロールとは何ですか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-220">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="6aefc-221">パートナー センターのインセンティブ ロールは場所に基づいており、インセンティブ管理者とインセンティブ ユーザーを含んでいます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-221">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="6aefc-222">これらのロールが実行できる操作の詳細については「[ユーザー ロールとアクセス許可の割り当て](permissions-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6aefc-222">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="6aefc-223">**インセンティブ ユーザーをグローバル レベルと場所レベルで割り当てることはできますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-223">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="6aefc-224">はい。</span><span class="sxs-lookup"><span data-stu-id="6aefc-224">Yes.</span></span> <span data-ttu-id="6aefc-225">インセンティブ管理者をすべての場所のインセンティブ管理者になるように割り当てることも、各場所に独自のインセンティブ管理者を割り当てることもできます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-225">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="6aefc-226">**インセンティブをグローバル レベルまたは場所レベルで支払われるようにすることはできますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-226">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="6aefc-227">インセンティブは、場所レベルでのみ支払われます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-227">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="6aefc-228">**紹介に関連して、いくつのビジネス プロファイルを作成できますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-228">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="6aefc-229">会社は、自社の関心を完全に表す必要性に応じてビジネス プロファイルをいくつでも作成できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-229">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="6aefc-230">各ビジネス プロファイルでは、最大 5 つの場所 (国ごとに 1 つの場所) を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-230">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="6aefc-231">各ビジネス プロファイルは、その各場所の紹介を受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-231">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="6aefc-232">**紹介はどのように割り当てられ、どのような変化を期待できますか?たとえば、1 つの市場にグローバルな会社を持ち、その他の市場に複数の場所を持っている場合、紹介はどのように割り当てられますか?**</span><span class="sxs-lookup"><span data-stu-id="6aefc-232">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="6aefc-233">紹介は、顧客が定義する検索パラメーターに基づいて割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-233">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="6aefc-234">そのため、持っている場所が 1 つか複数かには関係なく、顧客が目的の場所を指定し、そこに他のパラメーターを満たすビジネスがある場合、紹介はその場所に割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="6aefc-234">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








