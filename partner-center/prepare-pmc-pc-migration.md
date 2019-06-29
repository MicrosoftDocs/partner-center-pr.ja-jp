---
title: Partner Membership Center からパートナー センターへの移行の準備 |パートナー センター
ms.topic: article
ms.date: 06/13/2019
description: PMC からビジネスをパートナー センターに移動する前に、考慮すべき点
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0f1df50c5fa94707ac733a91b0d981b6821de8c0
ms.sourcegitcommit: 7b3847a788365a05628a4cf2938dfd61782d6e4e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2019
ms.locfileid: "67468023"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a><span data-ttu-id="99a8a-103">パートナー センターにパートナー メンバーシップ センター (PMC) からの移行の準備します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-103">Prepare for your move from Partner Membership Center (PMC) to Partner Center</span></span>

<span data-ttu-id="99a8a-104">移行されますメンバーシップの管理パートナー メンバーシップ センター (PMC) から、パートナー センター – microsoft のビジネス関係を管理する 1 つの宛先です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-104">We are moving membership management from Partner Membership Center (PMC) to the partner center – the single destination to manage your business relationship with Microsoft.</span></span> <span data-ttu-id="99a8a-105">パートナー センターと効率性とできるだけ簡単に移行します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-105">We want your move to Partner Center to be as efficient and easy as possible.</span></span> <span data-ttu-id="99a8a-106">PMC から、パートナー センターとは異なる、いただけることを理解し、移動を行う前に準備をしますが、一部の領域を特定できました。</span><span class="sxs-lookup"><span data-stu-id="99a8a-106">We’ve identified some areas where the Partner Center differs from PMC, and we think you will want to understand and prepare for them before you make the move.</span></span>

## <a name="account-and-identity-setup"></a><span data-ttu-id="99a8a-107">アカウントと id のセットアップ</span><span class="sxs-lookup"><span data-stu-id="99a8a-107">Account and identity setup</span></span>

<span data-ttu-id="99a8a-108">**Azure Active Directory (Azure AD) の職場アカウントとは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-108">**What is an Azure Active Directory (Azure AD) work account?**</span></span>

<span data-ttu-id="99a8a-109">Azure 職場アカウントは、Azure パブリック クラウドにおける企業の分離された専用の仮想表現です。Azure、Microsoft Intune、Office 365などの Microsoft クラウド サービスにサブスクライブすると作成されます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-109">An Azure work account is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span>

<span data-ttu-id="99a8a-110">職場のアカウントは、Azure AD ユーザーと、電子メール、パスワード、プロファイル データ、アクセス許可、およびにそれらに関する情報をホストします。</span><span class="sxs-lookup"><span data-stu-id="99a8a-110">Your work account hosts your Azure AD users and the information about them - their email, passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="99a8a-111">職場アカウントには、グループ、アプリケーション、および企業およびそのセキュリティに関するその他の情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="99a8a-111">The work account also contains groups, applications, and other information pertaining to a company and its security.</span></span> <span data-ttu-id="99a8a-112">詳細情報を参照してください.</span><span class="sxs-lookup"><span data-stu-id="99a8a-112">For more information see …</span></span>

<span data-ttu-id="99a8a-113">パートナー センターでは、アカウントにサインインしない個人用の電子メールに、職場の電子メールを使用します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-113">In the Partner Center you will use your work email to sign into your account not your personal email.</span></span>
- <span data-ttu-id="99a8a-114">職場のアカウント: john@contoso.com</span><span class="sxs-lookup"><span data-stu-id="99a8a-114">Your work account: john@contoso.com</span></span>
- <span data-ttu-id="99a8a-115">個人のアカウント: John@outlook.com</span><span class="sxs-lookup"><span data-stu-id="99a8a-115">Your personal account: John@outlook.com</span></span>

<span data-ttu-id="99a8a-116">会社の電子メールは、Azure active directory テナントの一部です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-116">Your work email is part of your Azure active directory tenant.</span></span> <span data-ttu-id="99a8a-117">パートナー センター アカウントがある、AAD テナントを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-117">To have an account in Partner Center, you need to have an AAD tenant.</span></span> <span data-ttu-id="99a8a-118">Azure Active Directory の詳細については、読み取る[で Azure AD ディレクトリの作成](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad)です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-118">For more information on Azure Active Directory, read [Create your directory in Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).</span></span>

<span data-ttu-id="99a8a-119">**移動すると、パートナー センター、PMC からどのようなアカウントにサインインしてパートナー センター場合を (たとえば Office 365) 用 Microsoft とすると、AAD テナントもが、CSP ビジネスのテナントですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-119">**When you move to Partner Center from PMC, what account should you sign into Partner Center with if you have an AAD tenant with Microsoft (for Office 365 for example) and you also have a tenant for your CSP business?**</span></span>

<span data-ttu-id="99a8a-120">CSP アカウントまたは MPN 職場の電子メール アカウントのいずれかで、パートナー センターにサインインすることができます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-120">You can sign into Partner Center with either the CSP account or your MPN work email account.</span></span> <span data-ttu-id="99a8a-121">CSP 職場の電子メールを使用してサインインする場合は、ダッシュ ボードの左側のナビゲーションには MPN と CSP の両方のプログラム情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-121">If you choose to sign in using your CSP work email, the left navigation on your dashboard will display both MPN and CSP program information.</span></span> <span data-ttu-id="99a8a-122">MPN Azure AD テナントの職場の電子メールでサインインする場合は、MPN プログラム情報のみが表示されます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-122">If you sign in with your MPN Azure AD tenant work email, you will see only your MPN program information.</span></span> <span data-ttu-id="99a8a-123">ユーザー ロールは、MPN、および CSP の間で異なる MPN と CSP の両方のビジネスを同じアカウントを使用する場合がそれに応じてユーザー ロールを割り当てることを確認するようにします。</span><span class="sxs-lookup"><span data-stu-id="99a8a-123">User roles differ between MPN and CSP so if you use the same account for both MPN and CSP business, be sure you assign user roles accordingly.</span></span> <span data-ttu-id="99a8a-124">ユーザー ロールについては、「[ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-124">For information on user roles, read [Assign user roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="99a8a-125">**AAD のグローバル管理者ロールと、PMC MPN のグローバル管理者ロールの違いは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-125">**What is the difference between the AAD global admin role and the PMC MPN global admin role?**</span></span>

<span data-ttu-id="99a8a-126">これらは、さまざまなアクセス許可を使用して、まったく異なる 2 つのロールです。</span><span class="sxs-lookup"><span data-stu-id="99a8a-126">These are two completely different roles with different permissions.</span></span> <span data-ttu-id="99a8a-127">パートナー センターで AAD テナントのグローバル管理者、テナントの管理 – 追加またはユーザーを削除しますとパスワード、ロール、アクセス許可を管理および提供パートナー センターで、会社のすべてのプログラムへのアクセスを持ちます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-127">The AAD tenant global admin in Partner Center administers the tenant – adds or removes users, provides and manages passwords, roles and permissions, and has access to all their company’s programs in Partner Center.</span></span> 

<span data-ttu-id="99a8a-128">PMC で、MPN のグローバル管理者ロールは、次の方法でした。</span><span class="sxs-lookup"><span data-stu-id="99a8a-128">The MPN global admin role in PMC could do the following:</span></span>

- <span data-ttu-id="99a8a-129">表示し、会社とそのすべての会社の場所に関連付けられているすべてのデータの編集</span><span class="sxs-lookup"><span data-stu-id="99a8a-129">View and edit all the data associated with the company and all of the  company's locations</span></span>

-  <span data-ttu-id="99a8a-130">グローバルまたはローカル レベルで管理者を追加します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-130">Add administrators at the global or local level.</span></span>  <span data-ttu-id="99a8a-131">また、グローバル管理者では、どの場所に関係なく関連付けられているグローバル アクセスを許可するグローバル管理者アクセスの任意の場所にあるすべてのユーザーを割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-131">Also, Global admins can assign any person at any location Global Administrator Access which grants them global access regardless of which location they're associated with.</span></span>
-  <span data-ttu-id="99a8a-132">関数などの UI に接続するすべてのパートナーを実行します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-132">Perform any partner facing UI function including:</span></span> 

-  <span data-ttu-id="99a8a-133">ユーザーの追加と削除</span><span class="sxs-lookup"><span data-stu-id="99a8a-133">Add/remove users</span></span>

 - <span data-ttu-id="99a8a-134">ロールの割り当てと削除</span><span class="sxs-lookup"><span data-stu-id="99a8a-134">Assign/remove roles</span></span> 

 - <span data-ttu-id="99a8a-135">追加/削除/更新の場所</span><span class="sxs-lookup"><span data-stu-id="99a8a-135">Add/remove/update locations</span></span> 

 - <span data-ttu-id="99a8a-136">コンピテンシー/マップを購入します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-136">Purchase competency/maps</span></span> 

-  <span data-ttu-id="99a8a-137">ビューの利点があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-137">View benefits</span></span>

<span data-ttu-id="99a8a-138">MPN のグローバル管理者は、パートナー センターに移動すると、ロールが呼び出されます、MPN パートナーの管理者はさまざまなアクセス許可と、パートナー センターのグローバル管理者よりも、タスクがあります。ロールとパートナー センターでのアクセス許可の詳細については、読み取る[ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)</span><span class="sxs-lookup"><span data-stu-id="99a8a-138">When the MPN global admin moves to Partner Center the role is called the MPN partner admin which has different permissions and tasks than the Partner Center global admin. For more information on roles and permissions in Partner Center, read [Assign users roles and permissions](permissions-overview.md)</span></span>

<span data-ttu-id="99a8a-139">**パートナー センターでゲスト ユーザーのロールを含むユーザー ロール**</span><span class="sxs-lookup"><span data-stu-id="99a8a-139">**User roles including guest user roles in Partner Center**</span></span>

<span data-ttu-id="99a8a-140">パートナー センターでは、さまざまな種類のロールを実行するために必要な作業の種類によってがあります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-140">Partner Center has different types of roles depending on the types of work needed to be done.</span></span> <span data-ttu-id="99a8a-141">Azure AD ロールには、グローバル管理者などのロールがあります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-141">There are roles such as global admin that are Azure AD roles.</span></span> <span data-ttu-id="99a8a-142">一部の役割は、クラウド サービス プロバイダー プログラム、インセンティブなどのプログラムに固有と MPN に固有のロールがあります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-142">Some of the roles are specific to programs such as the Cloud Service Provider program or incentives, and there are roles that are specific to MPN.</span></span> <span data-ttu-id="99a8a-143">パートナー センターのすべてのロールとは何を確認するには、読み取り[ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-143">To find out what all the Partner Center roles are, read [Assign users roles and permissions](permissions-overview.md).</span></span>



<span data-ttu-id="99a8a-144">**PMC からパートナー センターに移動したときのユーザーのロールにどうなりますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-144">**What happens to my users' roles when they move from PMC to Partner Center?**</span></span>

<span data-ttu-id="99a8a-145">PMC ですべてのユーザーは、MPN のグローバル管理者またはプライマリのプログラムの連絡先は、移行を実施を除く、管理者ロールを失われます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-145">Except for the MPN global admin or primary program contact who conducts the migration, all users in PMC will lose their admin roles.</span></span> <span data-ttu-id="99a8a-146">移行が完了すると、個人は、パートナー センターでロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-146">The individual who completes the migration will need to assign roles in Partner Center.</span></span> <span data-ttu-id="99a8a-147">パートナー センター内のロールは、PMC で内容と異なります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-147">The roles in Partner Center differ from those in PMC.</span></span> <span data-ttu-id="99a8a-148">読み取り[ユーザー ロールとアクセス許可を割り当てる](permissions-overview)と[PMC からパートナー センターへの移行](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles)のパートナー センターでのユーザー ロールの詳細。</span><span class="sxs-lookup"><span data-stu-id="99a8a-148">Read [Assign users roles and permissions](permissions-overview) and [Moving from PMC to Partner Center](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) for more on user roles in Partner Center.</span></span>


<span data-ttu-id="99a8a-149">**会社プロファイルとビジネス プロファイル間の違いは何ですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-149">**What’s the difference between my company profile and my business profile?**</span></span>

<span data-ttu-id="99a8a-150">自分の会社プロファイルは、住所、場所、主要な連絡先、銀行と税の詳細を含む会社に関する情報です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-150">Your company profile is the information about your company that includes address, locations, primary contact, bank and tax details.</span></span>

<span data-ttu-id="99a8a-151">ビジネス プロファイルは顧客の自分を提示する方法は、ロゴなど、ビジネスの焦点、専門知識などの詳細を表示するためのマーケティング ページです。</span><span class="sxs-lookup"><span data-stu-id="99a8a-151">Your business profile is how you present yourself to customers and is a marketing page that displays your logo, details on your business focus, your expertise, etc.</span></span>

<span data-ttu-id="99a8a-152">**統合アカウントの平均がどのアカウントがでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-152">**What does account consolidation mean for my account?**</span></span>

<span data-ttu-id="99a8a-153">パートナー センターに複数の MPN アカウントを移行する、同じ Azure AD テナントを使用する場合、システムは自動的にそれを認識し、アカウントを統合するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-153">If you use the same Azure AD tenant to migrate multiple MPN accounts into Partner Center, the system will automatically recognize that and ask you to consolidate your accounts.</span></span> <span data-ttu-id="99a8a-154">これは、同じ Azure AD テナントに関連付けられているドメインが複数ある場合でも当てはまります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-154">This is true even if you have multiple domains associated to the same Azure AD tenant.</span></span> 

<span data-ttu-id="99a8a-155">個別の AAD テナントを使用してパートナー センターに移行することできますが、これによって、分離された評価の自分の能力と余分なコストで購入に注意してください。</span><span class="sxs-lookup"><span data-stu-id="99a8a-155">You could still decide to migrate to Partner Center using separate AAD tenants, but please note this results in isolated evaluation of your competencies and extra purchase costs.</span></span> 

<span data-ttu-id="99a8a-156">**複数の AAD テナントと 1 つの MPN アカウントを設定した場合でがパートナー センターでそれらをリンクすることですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-156">**If I have multiple AAD tenants and a single MPN account, is it possible to link them in Partner Center?**</span></span>

<span data-ttu-id="99a8a-157">はい、パートナー センターでは、1 つのパートナー センター アカウントに複数の Azure AD テナントをリンクできます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-157">Yes, in Partner Center you can link multiple Azure AD tenants to single Partner Center account.</span></span>
<span data-ttu-id="99a8a-158">詳細について説明します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-158">Learn more here.</span></span> 

<span data-ttu-id="99a8a-159">**複数の Azure AD テナントを 1 つのパートナー センター アカウントに追加する場合に制限はありますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-159">**Are there restrictions to adding multiple Azure AD tenants to a single Partner Center account?**</span></span>

<span data-ttu-id="99a8a-160">Azure AD テナントが既に既存のパートナー センター アカウントに関連付けられている場合は、マルチ テナント機能を使用して新しいパートナー センター アカウントに関連付けすることはできません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-160">If the Azure AD tenant is already associated to an existing Partner Center account, it can't be associated to new Partner Center accounts using the multi-tenancy feature.</span></span> <span data-ttu-id="99a8a-161">考えてみると、別の方法は、Azure AD テナントを 1 つのパートナー センター アカウントに関連付けられているのみすることができますが、パートナー センター アカウントがそれに関連付けられている複数のテナントを持つことができます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-161">Another way to think of it is, an Azure AD tenant can only be associated to one Partner Center account, but a Partner Center account can have multiple tenants associated to it.</span></span>

## <a name="microsoft-partner-network-mpn-membership-migration"></a><span data-ttu-id="99a8a-162">Microsoft Partner Network (MPN) メンバーシップの移行</span><span class="sxs-lookup"><span data-stu-id="99a8a-162">Microsoft Partner Network (MPN) membership migration</span></span> 

<span data-ttu-id="99a8a-163">**PMC からの移行を実行すると、パートナー センターにユーザーことができますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-163">**Who can perform the move from PMC to Partner Center?**</span></span>

<span data-ttu-id="99a8a-164">会社 MPN のグローバル管理者または、プライマリのプログラムにお問い合わせください (これら 2 つのロールは、同じユーザーが保持される多くの場合) は開始し、移行を実行できます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-164">Your company MPN global admin or the primary program contact (these two roles are often held by the same person) can initiate and perform the move.</span></span>

<span data-ttu-id="99a8a-165">**移行を完了する人では、パートナー センターで会社の有効なプロファイルで主要連絡先になりますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-165">**Will the person completing the migration become the primary contact on the company legal profile in Partner Center?**</span></span>

<span data-ttu-id="99a8a-166">必ずしも、ただし、主要連絡先が必要契約に署名する承認を持っている人です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-166">Not necessarily, however, the primary contact needs to be someone who has authorization to sign agreements.</span></span>

<span data-ttu-id="99a8a-167">**Microsoft は私にとって、MPN メンバーシップを移行できますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-167">**Can Microsoft migrate my MPN membership for me?**</span></span>

<span data-ttu-id="99a8a-168">No.</span><span class="sxs-lookup"><span data-stu-id="99a8a-168">No.</span></span> <span data-ttu-id="99a8a-169">メンバーシップ アカウントをパートナー センターに移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-169">Microsoft cannot help you move your membership account to partner center.</span></span> <span data-ttu-id="99a8a-170">移行プロセスを開始する (サインイン資格情報)、職場アカウントを使って PMC にサインインして、アカウントを移動する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-170">You will need to move your account by signing into PMC with your work account (sign in credentials)to begin the migration process.</span></span> <span data-ttu-id="99a8a-171">自分のアカウントを移行する手順を完了した後、メンバーシップの管理を開始し、特典にアクセスし、メンバーシップの管理を支援できるように、自分のチームにユーザー ロールとアクセス許可を割り当てることがことができます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-171">After you’ve completed the steps to move your account you can start managing your membership and  assign user roles and permissions to your team so they can access benefits and help manage the membership.</span></span> <span data-ttu-id="99a8a-172">Microsoft は、現在コンピテンシー、利点、インセンティブ、および Partner University のアクセスを含む MCP アソシエーションの銀行または税金情報の場所については、自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-172">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="99a8a-173">Microsoft は、現在コンピテンシー、利点、インセンティブ、および Partner University のアクセスを含む MCP アソシエーションの銀行または税金情報の場所については、自動的に移行します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-173">Microsoft will automatically migrate the current competencies, benefits, location information, bank/tax information for incentives, and MCP associations including Partner University access.</span></span>

<span data-ttu-id="99a8a-174">**更新ポリシーはどのように変化するでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-174">**How will the renewal policy change?**</span></span>

 <span data-ttu-id="99a8a-175">パートナー センターで表示される更新ウィンドウは次の 30 日まで、記念日です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-175">In Partner Center, the renewal window is from your anniversary date through the following 30 days.</span></span>

<span data-ttu-id="99a8a-176">**コンピテンシー変わらないパートナー センターに移動した後ですか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-176">**Will our competencies remain unchanged after we move to Partner Center?**</span></span>

<span data-ttu-id="99a8a-177">はい、能力は、パートナー センターへの移行では影響ありません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-177">Yes, compentencies will not be affected by the move to Partner Center.</span></span> <span data-ttu-id="99a8a-178">矛盾する場合にお問い合わせください。[サポート](https://partner.microsoft.com/support)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-178">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>


 <span data-ttu-id="99a8a-179">**移動後に (クラウドのメリット、テクニカル サポート、ソフトウェアの特典、Visual Studio を含む) の特典が変更されますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-179">**Will my benefits (including cloud benefits, technical support, software benefits, Visual Studio) change after we move?**</span></span>

 <span data-ttu-id="99a8a-180">対象となる特典は変更されません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-180">Your eligible benefits will not change.</span></span> <span data-ttu-id="99a8a-181">矛盾する場合にお問い合わせください。[サポート](https://partner.microsoft.com/support)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-181">If you notice discrepancies, contact [Support](https://partner.microsoft.com/support).</span></span>

 <span data-ttu-id="99a8a-182">**Visual Studio 特典割り当てを持つ、Microsoft アカウントを受け入れられるでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-182">**Will our Microsoft accounts that have Visual Studio benefits allocations be honored?**</span></span>


 <span data-ttu-id="99a8a-183">[はい]。</span><span class="sxs-lookup"><span data-stu-id="99a8a-183">Yes.</span></span> <span data-ttu-id="99a8a-184">Msa に割り当てられている visual Studio の特典は受け入れられ、保持されます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-184">Visual Studio benefits allocated to MSAs will be honored and retained.</span></span> <span data-ttu-id="99a8a-185">また、パートナー センターでの更新後も保持されます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-185">They will also be preserved after renewal in Partner Center.</span></span> <span data-ttu-id="99a8a-186">ただし、MSA 割り当てを 1 回は、パートナー センターで移行を削除する場合は、パートナー センターに追加できません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-186">However, if you remove an MSA allocation once migrated in Partner Center, it can’t be added  back into Partner Center.</span></span>

<span data-ttu-id="99a8a-187">パートナー センターでは、パートナーは職場アカウントの場所は、パートナーは MPN 管理者は、Azure AD テナントに MSA を同じテナントでゲスト ユーザー アカウントを追加できます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-187">In Partner Center, a partner can add work accounts and guest user accounts which are MSA from the same tenant where the partner is MPN admin in the Azure AD tenant.</span></span> <span data-ttu-id="99a8a-188">複数の Azure AD テナントでグローバル管理者は、パートナーは、これらすべてのテナントが同じパートナー センター アカウントに関連付けられている場合は、パートナーは、Visual Studio の特典と Azure の使用量ベースの割り当てにこれらすべてのテナントでユーザーを追加する許可します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-188">If the partner is a global admin in multiple Azure AD tenants and all these tenants are associated to the same Partner Center account, then the partner is allowed to add users across all these tenants into the Visual Studio benefits and Azure usage-based allocations.</span></span>

<span data-ttu-id="99a8a-189">ゲスト ユーザーには、MPN の管理者または全体管理者によって Visual Studio の使用法に基づくサブスクリプションを割り当てることができますが、ゲスト ユーザーにサインインできないパートナー センターの MSA を使用します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-189">Although guest users can be assigned usage-based subscriptions of Visual Studio by the MPN admin or global admin, guest users can't sign in to Partner Center using their MSA.</span></span> <span data-ttu-id="99a8a-190">ゲスト ユーザーが、検証し、割り当てられた特典を使用するには、Azure と Visual Studio にサインインできる、ただし、します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-190">Guest users can, however, sign in to Azure and Visual Studio to validate and use their assigned benefits.</span></span>


 <span data-ttu-id="99a8a-191">**MCP、アソシエーションと、Partner University アクセスを管理にはどうする必要がありますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-191">**How should we manage our MCP associations and our Partner University access?**</span></span>

 <span data-ttu-id="99a8a-192">PMC から移動する MCP 関連付けを変更することはありません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-192">There are no changes to MCP associations that move from PMC.</span></span> <span data-ttu-id="99a8a-193">ただし、新しい新しい従業員パートナー センターに移動した後は、パートナー センターで関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-193">However, any new new employees after you move to Partner Center will need to be associated in Partner Center.</span></span> <span data-ttu-id="99a8a-194">既存のユーザーのすべての Partner University アクセス許可は残りますが、新しい従業員に移動する必要があります[トレーニング センター](https://partner.microsoft.com/training) Partner University にアクセスする方法について。</span><span class="sxs-lookup"><span data-stu-id="99a8a-194">All your Partner University permissions for existing users will remain but any new employees should go to [the training center](https://partner.microsoft.com/training) for information on how to gain access to Partner University.</span></span>

 <span data-ttu-id="99a8a-195">**パートナー センターで顧客の参照を使用しますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-195">**Are customer references used in Partner Center?**</span></span>

 <span data-ttu-id="99a8a-196">いいえ、パートナー センターの能力の要件を満たすために顧客の参照は不要です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-196">No, you don't need customer references to meet competency requirements in Partner Center.</span></span>

 <span data-ttu-id="99a8a-197">**パートナーのレコードの関連付けがパートナー センターに移動するのでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-197">**Will Partner of Record associations move to Partner Center?**</span></span>

 <span data-ttu-id="99a8a-198">はい、パートナーのレコードを変更することはありません。</span><span class="sxs-lookup"><span data-stu-id="99a8a-198">Yes, there is no change to Partner of Record.</span></span> <span data-ttu-id="99a8a-199">詳細について[お客様に貴社のパートナー ID をリンク](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-199">Find out more about [linking your partner ID to your customers](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).</span></span>

<span data-ttu-id="99a8a-200">**パートナー センターへの移行のためのインセンティブに対する影響はありますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-200">**Is there an impact to incentives because of the move to Partner Center?**</span></span>

<span data-ttu-id="99a8a-201">いいえ、影響はありませんインセンティブを統合することの位置指定のないアカウントに移動した場合です。</span><span class="sxs-lookup"><span data-stu-id="99a8a-201">No, there is no impact to incentives if you have moved your account without consolidating locations.</span></span> <span data-ttu-id="99a8a-202">PMC で、ビジネスが複数のアカウントを持つし、グローバル アカウントに統合することをパートナー センターに移動するときに場合、に奨励金が失われることはありませんがある可能性があります、遅延インセンティブの払い戻し金額で。</span><span class="sxs-lookup"><span data-stu-id="99a8a-202">If your business has multiple accounts in PMC and, when you move to Partner Center you decide to consolidate into a global account, there will be no loss to incentives but there may be a delay in incentive payout.</span></span> <span data-ttu-id="99a8a-203">インセンティブ プログラムに関係するすべての PMC アカウントを移動しない場合は、これらのアカウントに関連付けられているインセンティブを獲得を停止する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99a8a-203">If you don't move all your PMC accounts that have been involved in incentives programs, you may stop earning incentives that are tied to those accounts.</span></span>


<span data-ttu-id="99a8a-204">**パートナー センターでインセンティブのユーザーのロールとは**</span><span class="sxs-lookup"><span data-stu-id="99a8a-204">**What are the incentive user roles in Partner Center?**</span></span> 

<span data-ttu-id="99a8a-205">パートナー センターでのインセンティブの役割では、場所ベースし、インセンティブ管理者およびインセンティブのユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-205">Incentive roles in Partner Center are location-based and include Incentives admin and Incentives user.</span></span> <span data-ttu-id="99a8a-206">これらのロールで実行できる操作の詳細については、次を参照してください。[ユーザー ロールとアクセス許可を割り当てる](permissions-overview.md)します。</span><span class="sxs-lookup"><span data-stu-id="99a8a-206">For more information on what those roles can do, see [Assign users roles and permissions](permissions-overview.md).</span></span>

<span data-ttu-id="99a8a-207">**インセンティブのユーザーは、グローバルおよび場所レベルで割り当てることがでしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-207">**Can incentives users be assigned at the global and location level?**</span></span>

 <span data-ttu-id="99a8a-208">[はい]。</span><span class="sxs-lookup"><span data-stu-id="99a8a-208">Yes.</span></span> <span data-ttu-id="99a8a-209">すべての場所のインセンティブの管理者であるインセンティブ管理者を割り当てることができます。 か、それぞれの場所は独自のインセンティブの管理者があることができます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-209">You can assign an incentives admin to be the incentives admin for all locations or each location can have its own incentives admin.</span></span>

 <span data-ttu-id="99a8a-210">**グローバルまたは場所のレベルでインセンティブを有料できますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-210">**Can incentives be paid at the global or location level?**</span></span>

 <span data-ttu-id="99a8a-211">インセンティブは場所のレベルでのみ支払われます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-211">Incentives are paid only at the location level.</span></span>

<span data-ttu-id="99a8a-212">**参照に関するビジネス プロファイルの数作成できますか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-212">**Regarding referrals, how many business profiles can we create?**</span></span>

<span data-ttu-id="99a8a-213">会社は、必要な多くのビジネス プロファイルが、会社の関心を完全に表すように作成できます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-213">Your company can create as many business profiles as your need for fully represent your company's interests.</span></span> <span data-ttu-id="99a8a-214">各ビジネス プロファイルには、最大で 5 つの場所、国ごとに 1 つの場所を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-214">In each business profile, you can list up to five locations, one location per country.</span></span> <span data-ttu-id="99a8a-215">参照の場所の各ビジネス プロファイルの各受信できます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-215">Each of the business profiles can receive referrals for each of its locations.</span></span>

<span data-ttu-id="99a8a-216">**割り当ての参照をどのように、どのような変更を想定できますか?たとえば、他の市場で 1 つの市場で世界規模の企業と場所がある場合は、参照の割り当て方法でしょうか。**</span><span class="sxs-lookup"><span data-stu-id="99a8a-216">**How will referrals be assigned, what changes can I expect? For example, if I have a global company in one market and locations in other markets, how will referrals be assigned?**</span></span>

<span data-ttu-id="99a8a-217">参照では、お客様が定義する検索パラメーターに基づいて割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="99a8a-217">Referrals are assigned based on the search parameters that the customer defines.</span></span> <span data-ttu-id="99a8a-218">これは 1 つの場所または多くの場合、お客様が目的の場所を指定します、紹介とその場所に移動してください、他のパラメーターを満たしているビジネスがありますがある場合。</span><span class="sxs-lookup"><span data-stu-id="99a8a-218">So regardless of whether you have one location or many, if the customers specifies a desired location and you have a business there that meets the other parameters, then the referral would go to that location.</span></span>








